# Comparing `tmp/wp-math3d-0.6.7.tar.gz` & `tmp/wp-math3d-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wp-math3d-0.6.7.tar", last modified: Tue Dec  5 03:20:06 2023, max compression
+gzip compressed data, was "wp-math3d-0.6.9.tar", last modified: Sat Dec 23 21:15:45 2023, max compression
```

## Comparing `wp-math3d-0.6.7.tar` & `wp-math3d-0.6.9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.616720 wp-math3d-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/.cmake-format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-05 03:20:06.616720 wp-math3d-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.600720 wp-math3d-0.6.7/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/cmake/MathDependencies.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.596720 wp-math3d-0.6.7/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.604720 wp-math3d-0.6.7/include/math/
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/euler_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/euler_t_decl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.608720 wp-math3d-0.6.7/include/math/impl/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat2_t_avx_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat2_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13672 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat2_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat3_t_avx_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat3_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat3_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat4_t_avx_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat4_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13525 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/mat4_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/quat_t_avx_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/quat_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/quat_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec2_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec2_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec3_t_avx_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec3_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec3_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec4_t_avx_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec4_t_scalar_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/impl/vec4_t_sse_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/mat2_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/mat2_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9841 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/mat3_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/mat3_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/mat4_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/mat4_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/pose3d_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/pose3d_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13365 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/quat_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/quat_t_decl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.608720 wp-math3d-0.6.7/include/math/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8278 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/utils/geometry_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/utils/spherical_coordinates.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/vec2_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/vec2_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/vec3_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/vec3_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/vec4_t.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/include/math/vec4_t_decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.600720 wp-math3d-0.6.7/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.608720 wp-math3d-0.6.7/python/math3d/
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.608720 wp-math3d-0.6.7/python/math3d/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/bindings_py.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15429 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/common_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/conversions_py.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/conversions_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/euler_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/mat2_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/mat3_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/mat4_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/pose3d_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/quat_py.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.608720 wp-math3d-0.6.7/python/math3d/bindings/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/utils/geometry_helpers_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/vec2_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/vec3_py.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/python/math3d/bindings/vec4_py.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.616720 wp-math3d-0.6.7/python/wp_math3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-05 03:20:06.000000 wp-math3d-0.6.7/python/wp_math3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-12-05 03:20:06.000000 wp-math3d-0.6.7/python/wp_math3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 03:20:06.000000 wp-math3d-0.6.7/python/wp_math3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 03:20:06.000000 wp-math3d-0.6.7/python/wp_math3d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-05 03:20:06.000000 wp-math3d-0.6.7/python/wp_math3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-05 03:20:06.616720 wp-math3d-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.600720 wp-math3d-0.6.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.616720 wp-math3d-0.6.7/tests/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/common_math_generators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/common_math_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_euler_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_geometry_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat2_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat2_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat2_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat3_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat3_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat3_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat4_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11254 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat4_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_mat4_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_pose3d_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_quat_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_quat_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_utils_spherical_coordinates.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_vec2_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_vec2_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_vec3_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_vec3_type.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_vec4_operations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/cpp/test_vec4_type.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 03:20:06.616720 wp-math3d-0.6.7/tests/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/conversions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/euler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14207 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/geometry_helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/mat2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/mat3_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18477 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/mat4_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/pose3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/quat_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/vec2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/vec3_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7695 2023-12-05 03:19:58.000000 wp-math3d-0.6.7/tests/python/vec4_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.185383 wp-math3d-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/.cmake-format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-23 21:15:45.185383 wp-math3d-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.165383 wp-math3d-0.6.9/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/cmake/MathDependencies.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.165383 wp-math3d-0.6.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.169383 wp-math3d-0.6.9/include/math/
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/euler_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/euler_t_decl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.173383 wp-math3d-0.6.9/include/math/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat2_t_avx_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat2_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13672 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat2_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat3_t_avx_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat3_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15556 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat3_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat4_t_avx_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat4_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13525 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/mat4_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/quat_t_avx_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/quat_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/quat_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec2_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec2_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec3_t_avx_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec3_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec3_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec4_t_avx_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec4_t_scalar_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/impl/vec4_t_sse_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/mat2_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/mat2_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/mat3_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/mat3_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/mat4_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/mat4_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/pose3d_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/pose3d_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13365 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/quat_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/quat_t_decl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.173383 wp-math3d-0.6.9/include/math/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8278 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/utils/geometry_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/utils/spherical_coordinates.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/vec2_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/vec2_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/vec3_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/vec3_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13382 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/vec4_t.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/include/math/vec4_t_decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.165383 wp-math3d-0.6.9/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.173383 wp-math3d-0.6.9/python/math3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.177383 wp-math3d-0.6.9/python/math3d/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/bindings_py.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15429 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/common_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/conversions_py.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11915 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/conversions_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/euler_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/mat2_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/mat3_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/mat4_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/pose3d_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/quat_py.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.177383 wp-math3d-0.6.9/python/math3d/bindings/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/utils/geometry_helpers_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/vec2_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/vec3_py.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/python/math3d/bindings/vec4_py.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.185383 wp-math3d-0.6.9/python/wp_math3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-23 21:15:45.000000 wp-math3d-0.6.9/python/wp_math3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-12-23 21:15:45.000000 wp-math3d-0.6.9/python/wp_math3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 21:15:45.000000 wp-math3d-0.6.9/python/wp_math3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 21:15:44.000000 wp-math3d-0.6.9/python/wp_math3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-23 21:15:45.000000 wp-math3d-0.6.9/python/wp_math3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-23 21:15:45.185383 wp-math3d-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.165383 wp-math3d-0.6.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.181383 wp-math3d-0.6.9/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/common_math_generators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/common_math_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_euler_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_geometry_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat2_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat2_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat2_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat3_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat3_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat3_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat4_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat4_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_mat4_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_pose3d_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_quat_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_quat_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_utils_spherical_coordinates.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_vec2_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_vec2_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_vec3_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_vec3_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_vec4_operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/cpp/test_vec4_type.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:45.185383 wp-math3d-0.6.9/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/conversions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/euler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14207 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/geometry_helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/mat2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/mat3_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18477 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/mat4_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/pose3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/quat_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/vec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/vec3_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2023-12-23 21:15:35.000000 wp-math3d-0.6.9/tests/python/vec4_test.py
```

### Comparing `wp-math3d-0.6.7/.cmake-format.py` & `wp-math3d-0.6.9/.cmake-format.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/CMakeLists.txt` & `wp-math3d-0.6.9/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 # -------------------------------------
 # Get loco_cmake to help us configure our CMake based project
 include(FetchContent)
 FetchContent_Declare(
   loco_cmake
   GIT_REPOSITORY https://github.com/wpumacay/loco_cmake.git
-  GIT_TAG d1ba4734dcf29bbc7318deea16213452a80b3f2a # Version v0.1.4
+  GIT_TAG 0270626101bec01dbf9ae7f1b5febfb82092bf0c # Version v0.1.5
   GIT_PROGRESS FALSE
   GIT_SHALLOW TRUE)
 FetchContent_MakeAvailable(loco_cmake)
 include(${loco_cmake_SOURCE_DIR}/Index.cmake)
 
 # -------------------------------------
 # Define our project :)
 project(
   math3d
-  VERSION 0.6.7
+  VERSION 0.6.9
   DESCRIPTION "A basic math library for spatial algebra"
   HOMEPAGE_URL "https://github.com/wpumacay/math"
   LANGUAGES C CXX)
 
 # -------------------------------------
 # Define some options the user can set before|while configuring the project
 option(MATH_BUILD_SSE "Build using SSE SIMD-extensions support" ON)
@@ -123,14 +123,17 @@
 
 # -------------------------------------
 # Add C++ tests to the build process
 if(MATH_BUILD_TESTS)
   add_subdirectory(tests/cpp)
 endif()
 
+# HACK: Add the conversions headers directly, without exposing target math_py
+target_include_directories(
+  MathCpp INTERFACE ${PROJECT_SOURCE_DIR}/python/math3d/bindings/)
 # -------------------------------------
 # Add Python bindings to the build process
 if(MATH_BUILD_PYTHON_BINDINGS)
   add_subdirectory(python/math3d/bindings)
 endif()
 
 # -------------------------------------
```

### Comparing `wp-math3d-0.6.7/LICENSE.txt` & `wp-math3d-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/PKG-INFO` & `wp-math3d-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wp-math3d
-Version: 0.6.7
+Version: 0.6.9
 Summary: A basic math library for spatial algebra
 Home-page: https://github.com/wpumacay/loco-math
 Author: Wilbert Santos Pumacay Huallpa
 Author-email: wpumacay@gmail.com
 License: MIT License
 Keywords: math
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wp-math3d-0.6.7/README.md` & `wp-math3d-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/cmake/MathDependencies.cmake` & `wp-math3d-0.6.9/cmake/MathDependencies.cmake`

 * *Files 15% similar despite different names*

```diff
@@ -12,57 +12,58 @@
 # ~~~
 
 set(MATH_DEP_VERSION_catch2
     182c910b4b63ff587a3440e08f84f70497e49a81 # Release 2.13.10
     CACHE STRING "Version of Catch2 to be fetched (used for unittests)")
 
 set(MATH_DEP_VERSION_pybind11
-    5b0a6fc2017fcc176545afe3e09c9f9885283242 # Release v2.10.4
+    8a099e44b3d5f85b20f05828d919d2332a8de841 # Release v2.11.1
     CACHE STRING "Version of PyBind11 to be fetched (used for python bindings)")
 
 mark_as_advanced(MATH_DEP_VERSION_catch2)
 mark_as_advanced(MATH_DEP_VERSION_pybind11)
 
 # cmake-format: off
 # ------------------------------------------------------------------------------
 # Catch2 is used for generating unittests for our C++ codebase
 # ------------------------------------------------------------------------------
+
+set(CATCH_INSTALL_DOCS OFF CACHE BOOL "" FORCE)
+set(CATCH_INSTALL_EXTRAS OFF CACHE BOOL "" FORCE)
+set(CATCH_DEVELOPMENT_BUILD OFF CACHE BOOL "" FORCE)
+
 loco_find_or_fetch_dependency(
   USE_SYSTEM_PACKAGE FALSE
   PACKAGE_NAME Catch2
   LIBRARY_NAME catch2
   GIT_REPO https://github.com/catchorg/Catch2.git
   GIT_TAG ${MATH_DEP_VERSION_catch2}
   GIT_PROGRESS FALSE
   GIT_SHALLOW TRUE
   TARGETS Catch2::Catch2
-  BUILD_ARGS
-    -DCATCH_INSTALL_DOCS=OFF
-    -DCATCH_INSTALL_EXTRAS=OFF
-    -DCATCH_DEVELOPMENT_BUILD=OFF
   EXCLUDE_FROM_ALL)
 
 # Add custom scripts for test-case registration to the module path
 if (catch2_POPULATED)
   list(APPEND CMAKE_MODULE_PATH "${catch2_SOURCE_DIR}/contrib")
 endif()
 
 # ------------------------------------------------------------------------------
 # Pybind11 is used for generating Python bindings for this project's C++ API.
 # Notice that we're using a forked version in which usage of unique-ptr is
 # allowed, as we use this functionality in some other parent projects
 # ------------------------------------------------------------------------------
 
+set(PYBIND11_TEST OFF CACHE BOOL "" FORCE)
+
 loco_find_or_fetch_dependency(
   USE_SYSTEM_PACKAGE FALSE
   PACKAGE_NAME pybind11
   LIBRARY_NAME pybind11
   GIT_REPO https://github.com/pybind/pybind11.git
   GIT_TAG ${MATH_DEP_VERSION_pybind11}
   GIT_PROGRESS FALSE
   GIT_SHALLOW TRUE
   TARGETS pybind11::headers
-  BUILD_ARGS
-    -DPYBIND11_TEST=OFF
   EXCLUDE_FROM_ALL)
 
 # cmake-format: on
```

### Comparing `wp-math3d-0.6.7/include/math/common.hpp` & `wp-math3d-0.6.9/include/math/common.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     /// Terminates the operations of the initializer
     LM_INLINE auto _finished() -> void {
         assert(m_CurrentBuildIndex == (VECTOR_LAST_INDEX + 1));
     }
 
  private:
     /// Mutable reference to the vector we're currently constructing
-    VectorType& m_VectorRef;
+    VectorType& m_VectorRef;  // NOLINT
     /// Index of the current coefficient being 'built'
     uint32_t m_CurrentBuildIndex = VECTOR_FIRST_INDEX;
 };
 
 /// \class MatCommaInitializer
 ///
 /// \brief Helper class used during comma-initialization of matrix-types
@@ -235,15 +235,15 @@
     /// Terminates the operations of the initializer and returns the built vec3
     LM_INLINE auto _finished() -> void {
         assert(m_CurrentBuildIndex == (MATRIX_LAST_INDEX + 1));
     }
 
  private:
     /// Mutable reference to the matrix we're currently constructing
-    MatrixType& m_MatrixRef;
+    MatrixType& m_MatrixRef;  // NOLINT
     /// Index of the current coefficient being built
     uint32_t m_CurrentBuildIndex = MATRIX_FIRST_INDEX;
 };
 
 /// Returns the value clamped to the given range
 template <typename T>
 auto clamp(T x, T x_min, T x_max) -> T {
```

### Comparing `wp-math3d-0.6.7/include/math/euler_t.hpp` & `wp-math3d-0.6.9/include/math/euler_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/euler_t_decl.hpp` & `wp-math3d-0.6.9/include/math/euler_t_decl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat2_t_avx_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat2_t_avx_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat2_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat2_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat2_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat2_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat3_t_avx_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat3_t_avx_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat3_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat3_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat3_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat3_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat4_t_avx_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat4_t_avx_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat4_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat4_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/mat4_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/mat4_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/quat_t_avx_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/quat_t_avx_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/quat_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/quat_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/quat_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/quat_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec2_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec2_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec2_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec2_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec3_t_avx_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec3_t_avx_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec3_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec3_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec3_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec3_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec4_t_avx_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec4_t_avx_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec4_t_scalar_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec4_t_scalar_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/impl/vec4_t_sse_impl.hpp` & `wp-math3d-0.6.9/include/math/impl/vec4_t_sse_impl.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/mat2_t.hpp` & `wp-math3d-0.6.9/include/math/mat2_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/mat2_t_decl.hpp` & `wp-math3d-0.6.9/include/math/mat2_t_decl.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     /// Returns a comma-initializer to construct the matrix via its coefficients
     auto operator<<(T coeff) -> MatCommaInitializer<Type> {
         return MatCommaInitializer<Type>(*this, coeff);
     }
 
     /// Returns a printable string-representation of the matrix
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         const auto& data_elms = m_Elements;
         std::stringstream sstr_result;
 
         sstr_result << "( " << data_elms[0][0] << ", " << data_elms[1][0]
                     << '\n';
         sstr_result << "  " << data_elms[0][1] << ", " << data_elms[1][1]
                     << ')';
```

### Comparing `wp-math3d-0.6.7/include/math/mat3_t.hpp` & `wp-math3d-0.6.9/include/math/mat3_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/mat3_t_decl.hpp` & `wp-math3d-0.6.9/include/math/mat3_t_decl.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
     /// Returns a comma-initializer to construct the matrix via its coefficients
     auto operator<<(T coeff) -> MatCommaInitializer<Type> {
         return MatCommaInitializer<Type>(*this, coeff);
     }
 
     /// Returns a printable string-representation of the matrix
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         const auto& data_elms = m_Elements;
         std::stringstream sstr_result;
 
         sstr_result << "( " << data_elms[0][0] << ", " << data_elms[1][0]
                     << ", " << data_elms[2][0] << ",\n";
         sstr_result << "  " << data_elms[0][1] << ", " << data_elms[1][1]
                     << ", " << data_elms[2][1] << ",\n";
```

### Comparing `wp-math3d-0.6.7/include/math/mat4_t.hpp` & `wp-math3d-0.6.9/include/math/mat4_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/mat4_t_decl.hpp` & `wp-math3d-0.6.9/include/math/mat4_t_decl.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
     /// Returns a comma-initializer to construct the matrix via its coefficients
     auto operator<<(T coeff) -> MatCommaInitializer<Type> {
         return MatCommaInitializer<Type>(*this, coeff);
     }
 
     /// Returns a printable string-representation of the matrix
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         const auto& data_elms = m_Elements;
         std::stringstream sstr_result;
 
         sstr_result << "( " << data_elms[0][0] << ", " << data_elms[1][0]
                     << ", " << data_elms[2][0] << ", " << data_elms[3][0]
                     << "\n";
         sstr_result << "  " << data_elms[0][1] << ", " << data_elms[1][1]
```

### Comparing `wp-math3d-0.6.7/include/math/pose3d_t.hpp` & `wp-math3d-0.6.9/include/math/pose3d_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/pose3d_t_decl.hpp` & `wp-math3d-0.6.9/include/math/pose3d_t_decl.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     /// Composes the given pose with this pose
     LM_INLINE auto operator*(const Pose3d<T>& rhs) const -> Pose3d<T>;
 
     /// Applies this transform to the given vector
     LM_INLINE auto operator*(const Vec3& rhs) const -> Vec3;
 
     /// Returns a printable string representation of this pose
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         std::stringstream str_result;
         str_result << "Pose3d(pos=" << this->position.toString() << ", ";
         str_result << "rot=" << this->orientation.toString() << ")";
         return str_result.str();
     }
 };
```

### Comparing `wp-math3d-0.6.7/include/math/quat_t.hpp` & `wp-math3d-0.6.9/include/math/quat_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/quat_t_decl.hpp` & `wp-math3d-0.6.9/include/math/quat_t_decl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -180,20 +180,20 @@
 
     /// Returns an unmutable reference to the requested entry of the quaternion
     auto operator[](uint32_t index) const -> const T& {
         return m_Elements[index];
     }
 
     /// Returns a printable string-representation of the vector
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         std::stringstream str_result;
-        if (std::is_same<ElementType, float>()) {
+        if constexpr (std::is_same<ElementType, float>::value) {
             str_result << "Quaternionf(" << w() << ", " << x() << ", " << y()
                        << ", " << z() << ")";
-        } else if (std::is_same<ElementType, double>()) {
+        } else if constexpr (std::is_same<ElementType, double>::value) {
             str_result << "Quaterniond(" << w() << ", " << x() << ", " << y()
                        << ", " << z() << ")";
         } else {
             str_result << "QuaternionX(" << w() << ", " << x() << ", " << y()
                        << ", " << z() << ")";
         }
         return str_result.str();
```

### Comparing `wp-math3d-0.6.7/include/math/utils/geometry_helpers.hpp` & `wp-math3d-0.6.9/include/math/utils/geometry_helpers.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/utils/spherical_coordinates.hpp` & `wp-math3d-0.6.9/include/math/utils/spherical_coordinates.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/vec2_t.hpp` & `wp-math3d-0.6.9/include/math/vec2_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/vec2_t_decl.hpp` & `wp-math3d-0.6.9/include/math/vec2_t_decl.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -111,19 +111,19 @@
 
     /// Returns a comma-initializer to construct the vector via its coefficients
     auto operator<<(T coeff) -> VecCommaInitializer<Type> {
         return VecCommaInitializer<Type>(*this, coeff);
     }
 
     /// Returns a printable string-representation of the vector
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         std::stringstream str_result;
-        if (std::is_same<ElementType, float>()) {
+        if constexpr (std::is_same<ElementType, float>::value) {
             str_result << "Vector2f(" << x() << ", " << y() << ")";
-        } else if (std::is_same<ElementType, double>()) {
+        } else if constexpr (std::is_same<ElementType, double>::value) {
             str_result << "Vector2d(" << x() << ", " << y() << ")";
         } else {
             str_result << "Vector2X(" << x() << ", " << y() << ")";
         }
         return str_result.str();
     }
```

### Comparing `wp-math3d-0.6.7/include/math/vec3_t.hpp` & `wp-math3d-0.6.9/include/math/vec3_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/vec3_t_decl.hpp` & `wp-math3d-0.6.9/include/math/vec3_t_decl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -147,20 +147,20 @@
 
     /// Returns a comma-initializer to construct the vector via its coefficients
     auto operator<<(T coeff) -> VecCommaInitializer<Type> {
         return VecCommaInitializer<Type>(*this, coeff);
     }
 
     /// Returns a printable string-representation of the vector
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         std::stringstream str_result;
-        if (std::is_same<ElementType, float>()) {
+        if constexpr (std::is_same<ElementType, float>::value) {
             str_result << "Vector3f(" << x() << ", " << y() << ", " << z()
                        << ")";
-        } else if (std::is_same<ElementType, double>()) {
+        } else if constexpr (std::is_same<ElementType, double>::value) {
             str_result << "Vector3d(" << x() << ", " << y() << ", " << z()
                        << ")";
         } else {
             str_result << "Vector3X(" << x() << ", " << y() << ", " << z()
                        << ")";
         }
         return str_result.str();
```

### Comparing `wp-math3d-0.6.7/include/math/vec4_t.hpp` & `wp-math3d-0.6.9/include/math/vec4_t.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/include/math/vec4_t_decl.hpp` & `wp-math3d-0.6.9/include/math/vec4_t_decl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -161,20 +161,20 @@
 
     /// Returns a comma-initializer to construct the vector via its coefficients
     auto operator<<(T coeff) -> VecCommaInitializer<Type> {
         return VecCommaInitializer<Type>(*this, coeff);
     }
 
     /// Returns a printable string-representation of the vector
-    auto toString() const -> std::string {
+    [[nodiscard]] auto toString() const -> std::string {
         std::stringstream str_result;
-        if (std::is_same<ElementType, float>()) {
+        if constexpr (std::is_same<ElementType, float>::value) {
             str_result << "Vector4f(" << x() << ", " << y() << ", " << z()
                        << ", " << w() << ")";
-        } else if (std::is_same<ElementType, double>()) {
+        } else if constexpr (std::is_same<ElementType, double>::value) {
             str_result << "Vector4d(" << x() << ", " << y() << ", " << z()
                        << ", " << w() << ")";
         } else {
             str_result << "Vector4X(" << x() << ", " << y() << ", " << z()
                        << ", " << w() << ")";
         }
         return str_result.str();
```

### Comparing `wp-math3d-0.6.7/python/math3d/__init__.py` & `wp-math3d-0.6.9/python/math3d/__init__.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/CMakeLists.txt` & `wp-math3d-0.6.9/python/math3d/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/bindings_py.cpp` & `wp-math3d-0.6.9/python/math3d/bindings/bindings_py.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/common_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/common_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/conversions_py.cpp` & `wp-math3d-0.6.9/python/math3d/bindings/conversions_py.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/conversions_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/conversions_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/euler_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/euler_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/mat2_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/mat2_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/mat3_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/mat3_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/mat4_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/mat4_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/pose3d_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/pose3d_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/quat_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/quat_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/utils/geometry_helpers_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/utils/geometry_helpers_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/vec2_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/vec2_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/vec3_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/vec3_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/math3d/bindings/vec4_py.hpp` & `wp-math3d-0.6.9/python/math3d/bindings/vec4_py.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/python/wp_math3d.egg-info/PKG-INFO` & `wp-math3d-0.6.9/python/wp_math3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wp-math3d
-Version: 0.6.7
+Version: 0.6.9
 Summary: A basic math library for spatial algebra
 Home-page: https://github.com/wpumacay/loco-math
 Author: Wilbert Santos Pumacay Huallpa
 Author-email: wpumacay@gmail.com
 License: MIT License
 Keywords: math
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wp-math3d-0.6.7/python/wp_math3d.egg-info/SOURCES.txt` & `wp-math3d-0.6.9/python/wp_math3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/setup.cfg` & `wp-math3d-0.6.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wp-math3d
-version = 0.6.7
+version = 0.6.9
 description = A basic math library for spatial algebra
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Wilbert Santos Pumacay Huallpa
 license = MIT License
 author_email = wpumacay@gmail.com
 url = https://github.com/wpumacay/loco-math
```

### Comparing `wp-math3d-0.6.7/setup.py` & `wp-math3d-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/CMakeLists.txt` & `wp-math3d-0.6.9/tests/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/common_math_generators.hpp` & `wp-math3d-0.6.9/tests/cpp/common_math_generators.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/common_math_helpers.hpp` & `wp-math3d-0.6.9/tests/cpp/common_math_helpers.hpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_euler_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_euler_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_geometry_helpers.cpp` & `wp-math3d-0.6.9/tests/cpp/test_geometry_helpers.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat2_functions.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat2_functions.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat2_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat2_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat2_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat2_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat3_functions.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat3_functions.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat3_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat3_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat3_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat3_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat4_functions.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat4_functions.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat4_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat4_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_mat4_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_mat4_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_pose3d_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_pose3d_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_quat_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_quat_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_quat_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_quat_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_utils_spherical_coordinates.cpp` & `wp-math3d-0.6.9/tests/cpp/test_utils_spherical_coordinates.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_vec2_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_vec2_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_vec2_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_vec2_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_vec3_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_vec3_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_vec3_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_vec3_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_vec4_operations.cpp` & `wp-math3d-0.6.9/tests/cpp/test_vec4_operations.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/cpp/test_vec4_type.cpp` & `wp-math3d-0.6.9/tests/cpp/test_vec4_type.cpp`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/conversions_test.py` & `wp-math3d-0.6.9/tests/python/conversions_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/euler_test.py` & `wp-math3d-0.6.9/tests/python/euler_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/geometry_helpers_test.py` & `wp-math3d-0.6.9/tests/python/geometry_helpers_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/mat2_test.py` & `wp-math3d-0.6.9/tests/python/mat2_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/mat3_test.py` & `wp-math3d-0.6.9/tests/python/mat3_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/mat4_test.py` & `wp-math3d-0.6.9/tests/python/mat4_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/pose3d_test.py` & `wp-math3d-0.6.9/tests/python/pose3d_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/quat_test.py` & `wp-math3d-0.6.9/tests/python/quat_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/vec2_test.py` & `wp-math3d-0.6.9/tests/python/vec2_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/vec3_test.py` & `wp-math3d-0.6.9/tests/python/vec3_test.py`

 * *Files identical despite different names*

### Comparing `wp-math3d-0.6.7/tests/python/vec4_test.py` & `wp-math3d-0.6.9/tests/python/vec4_test.py`

 * *Files identical despite different names*

