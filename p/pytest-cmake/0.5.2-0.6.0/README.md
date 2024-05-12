# Comparing `tmp/pytest_cmake-0.5.2.tar.gz` & `tmp/pytest_cmake-0.6.0.tar.gz`

## Comparing `pytest_cmake-0.5.2.tar` & `pytest_cmake-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/build_backend.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/build_config.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/cmake/FindPytest.cmake
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/cmake/PytestAddTests.cmake
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/setup.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/LICENSE
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/README.md
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 pytest_cmake-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/build_backend.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/build_config.py
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/cmake/FindPytest.cmake
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/cmake/PytestAddTests.cmake
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/setup.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/README.md
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 pytest_cmake-0.6.0/PKG-INFO
```

### Comparing `pytest_cmake-0.5.2/build_config.py` & `pytest_cmake-0.6.0/build_config.py`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.2/cmake/FindPytest.cmake` & `pytest_cmake-0.6.0/cmake/FindPytest.cmake`

 * *Files 15% similar despite different names*

```diff
@@ -56,49 +56,43 @@
     function(pytest_discover_tests NAME)
         cmake_parse_arguments(
             PARSE_ARGV 1 "" ""
             "WORKING_DIRECTORY;TRIM_FROM_NAME;BUNDLE_TESTS"
             "LIBRARY_PATH_PREPEND;PYTHON_PATH_PREPEND;ENVIRONMENT;DEPENDS"
         )
 
-        # Set library path depending on the platform.
+        # Identify library path environment name depending on the platform.
         if (CMAKE_SYSTEM_NAME STREQUAL Windows)
-            set(LIB_ENV_PATH PATH)
-            set(_env_sep "\\\;")
+            set(LIBRARY_ENV_NAME PATH)
         elseif(CMAKE_SYSTEM_NAME STREQUAL Darwin)
-            set(LIB_ENV_PATH DYLD_LIBRARY_PATH)
-            set(_env_sep ":")
+            set(LIBRARY_ENV_NAME DYLD_LIBRARY_PATH)
         else()
-            set(LIB_ENV_PATH LD_LIBRARY_PATH)
-            set(_env_sep ":")
+            set(LIBRARY_ENV_NAME LD_LIBRARY_PATH)
         endif()
 
-        # Convert all paths into cmake paths.
-        cmake_path(CONVERT "$ENV{${LIB_ENV_PATH}}" TO_CMAKE_PATH_LIST libpath)
-        cmake_path(CONVERT "$ENV{PYTHONPATH}" TO_CMAKE_PATH_LIST pythonpath)
+        # Sanitize all paths for CMake.
+        cmake_path(CONVERT "$ENV{${LIBRARY_ENV_NAME}}" TO_CMAKE_PATH_LIST LIBRARY_PATH)
+        cmake_path(CONVERT "$ENV{PYTHONPATH}" TO_CMAKE_PATH_LIST PYTHON_PATH)
 
-        # Prepend input path to environment variables
+        # Prepend input path to environment variables.
         if (_LIBRARY_PATH_PREPEND)
             list(REVERSE _LIBRARY_PATH_PREPEND)
             foreach (_path ${_LIBRARY_PATH_PREPEND})
-                set(libpath "${_path}" "${libpath}")
+                set(LIBRARY_PATH "${_path}" "${LIBRARY_PATH}")
             endforeach()
         endif()
 
         if (_PYTHON_PATH_PREPEND)
             list(REVERSE _PYTHON_PATH_PREPEND)
             foreach (_path ${_PYTHON_PATH_PREPEND})
-                set(pythonpath "${_path}" "${pythonpath}")
+                set(PYTHON_PATH "${_path}" "${PYTHON_PATH}")
             endforeach()
         endif()
 
-        # Convert list into string.
-        list(JOIN libpath "${_env_sep}" libpath)
-        list(JOIN pythonpath "${_env_sep}" pythonpath)
-
+        # Default working directory to current build path if none is provided.
         if (NOT _WORKING_DIRECTORY)
             set(_WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})
         endif()
 
         get_filename_component(_WORKING_DIRECTORY "${_WORKING_DIRECTORY}" REALPATH)
 
         # Override option by environment variable if available.
@@ -112,17 +106,17 @@
             ${NAME} ALL VERBATIM
             BYPRODUCTS "${_tests_file}"
             DEPENDS ${_DEPENDS}
             COMMAND ${CMAKE_COMMAND}
             -D "PYTEST_EXECUTABLE=${PYTEST_EXECUTABLE}"
             -D "TEST_GROUP_NAME=${NAME}"
             -D "BUNDLE_TESTS=${_BUNDLE_TESTS}"
-            -D "LIB_ENV_PATH=${LIB_ENV_PATH}"
-            -D "LIBRARY_PATH=${libpath}"
-            -D "PYTHON_PATH=${pythonpath}"
+            -D "LIBRARY_ENV_NAME=${LIBRARY_ENV_NAME}"
+            -D "LIBRARY_PATH=${LIBRARY_PATH}"
+            -D "PYTHON_PATH=${PYTHON_PATH}"
             -D "TRIM_FROM_NAME=${_TRIM_FROM_NAME}"
             -D "WORKING_DIRECTORY=${_WORKING_DIRECTORY}"
             -D "ENVIRONMENT=${_ENVIRONMENT}"
             -D "PROJECT_SOURCE_DIR=${PROJECT_SOURCE_DIR}"
             -D "CTEST_FILE=${_tests_file}"
             -P "${CMAKE_CURRENT_FUNCTION_LIST_DIR}/PytestAddTests.cmake")
```

### Comparing `pytest_cmake-0.5.2/cmake/PytestAddTests.cmake` & `pytest_cmake-0.6.0/cmake/PytestAddTests.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -2,49 +2,57 @@
 cmake_minimum_required(VERSION 3.20...3.29)
 
 if(CMAKE_SCRIPT_MODE_FILE)
 
     # Set Cmake test file to execute each test.
     set(_content "")
 
-    # Ensure that list environment variables are
-    # represented as a string on Windows.
-    string(REPLACE [[;]] [[\;]] LIBRARY_PATH "${LIBRARY_PATH}")
-    string(REPLACE [[;]] [[\;]] PYTHON_PATH "${PYTHON_PATH}")
+    cmake_path(CONVERT "${LIBRARY_PATH}" TO_NATIVE_PATH_LIST LIBRARY_PATH)
+    cmake_path(CONVERT "${PYTHON_PATH}" TO_NATIVE_PATH_LIST PYTHON_PATH)
+
+    # Serialize path values separated by semicolons (required on Windows).
+    macro(encode_value VARIABLE_NAME)
+        string(REPLACE [[\]] [[\\]] ${VARIABLE_NAME} "${${VARIABLE_NAME}}")
+        string(REPLACE [[;]] [[\\;]] ${VARIABLE_NAME} "${${VARIABLE_NAME}}")
+    endmacro()
+
+    encode_value(LIBRARY_PATH)
+    encode_value(PYTHON_PATH)
 
     if (BUNDLE_TESTS)
         string(APPEND _content
             "add_test(\n"
             "    \"${TEST_GROUP_NAME}\"\n"
             "    ${PYTEST_EXECUTABLE} \"${WORKING_DIRECTORY}\"\n"
             ")\n"
             "set_tests_properties(\n"
             "     \"${TEST_GROUP_NAME}\" PROPERTIES\n"
-            "     ENVIRONMENT \"${LIB_ENV_PATH}=${LIBRARY_PATH}\"\n"
+            "     ENVIRONMENT \"${LIBRARY_ENV_NAME}=${LIBRARY_PATH}\"\n"
             ")\n"
             "set_tests_properties(\n"
             "     \"${TEST_GROUP_NAME}\"\n"
             "     APPEND PROPERTIES\n"
             "     ENVIRONMENT \"PYTHONPATH=${PYTHON_PATH}\"\n"
             ")\n"
         )
 
         foreach(env ${ENVIRONMENT})
+            encode_value(env)
             string(APPEND _content
                 "set_tests_properties(\n"
                 "     \"${TEST_GROUP_NAME}\"\n"
                 "     APPEND PROPERTIES\n"
                 "     ENVIRONMENT ${env}\n"
                 ")\n"
             )
         endforeach()
 
     else()
         # Set environment for collecting tests.
-        set(ENV{${LIB_ENV_PATH}} "${LIBRARY_PATH}")
+        set(ENV{${LIBRARY_ENV_NAME}} "${LIBRARY_PATH}")
         set(ENV{PYTHONPATH} "${PYTHON_PATH}")
         set(ENV{PYTHONWARNINGS} "ignore")
 
         execute_process(
             COMMAND "${PYTEST_EXECUTABLE}"
                 --collect-only -q
                 --rootdir=${WORKING_DIRECTORY} .
@@ -95,24 +103,25 @@
             string(APPEND _content
                 "add_test(\n"
                 "    \"${test_name}\"\n"
                 "    ${PYTEST_EXECUTABLE} \"${test_case}\"\n"
                 ")\n"
                 "set_tests_properties(\n"
                 "     \"${test_name}\" PROPERTIES\n"
-                "     ENVIRONMENT \"${LIB_ENV_PATH}=${LIBRARY_PATH}\"\n"
+                "     ENVIRONMENT \"${LIBRARY_ENV_NAME}=${LIBRARY_PATH}\"\n"
                 ")\n"
                 "set_tests_properties(\n"
                 "     \"${test_name}\"\n"
                 "     APPEND PROPERTIES\n"
                 "     ENVIRONMENT \"PYTHONPATH=${PYTHON_PATH}\"\n"
                 ")\n"
             )
 
             foreach(env ${ENVIRONMENT})
+                encode_value(env)
                 string(APPEND _content
                     "set_tests_properties(\n"
                     "     \"${test_name}\"\n"
                     "     APPEND PROPERTIES\n"
                     "     ENVIRONMENT ${env}\n"
                     ")\n"
                 )
```

### Comparing `pytest_cmake-0.5.2/setup.py` & `pytest_cmake-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         subprocess.call(["cmake", "-P", str(script_path), "-VV"])
         return install.run(self)
 
 
 setup(
     name="pytest-cmake",
-    version="0.5.2",
+    version="0.6.0",
     data_files=[
         (
             "share/Pytest/cmake",
             [
                 "build/PytestConfig.cmake",
                 "build/PytestConfigVersion.cmake",
                 "cmake/FindPytest.cmake",
```

### Comparing `pytest_cmake-0.5.2/.gitignore` & `pytest_cmake-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.2/LICENSE` & `pytest_cmake-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.2/README.md` & `pytest_cmake-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.5.2/pyproject.toml` & `pytest_cmake-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "cmake >= 3.20, < 3.30"
 ]
 build-backend = "build_backend"
 backend-path = ["."]
 
 [project]
 name = "pytest-cmake"
-version = "0.5.2"
+version = "0.6.0"
 description = "Provide CMake module for Pytest"
 readme = "README.md"
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4"
 license = {file = "LICENSE"}
 keywords = ["cmake", "pytest", "development"]
 authors = [
     {name = "Jeremy Retailleau", email = "jeremy.retailleau@gmail.com" }
```

### Comparing `pytest_cmake-0.5.2/PKG-INFO` & `pytest_cmake-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-cmake
-Version: 0.5.2
+Version: 0.6.0
 Summary: Provide CMake module for Pytest
 Author-email: Jeremy Retailleau <jeremy.retailleau@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jeremy Retailleau
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

