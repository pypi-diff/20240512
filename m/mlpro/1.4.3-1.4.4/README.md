# Comparing `tmp/mlpro-1.4.3.tar.gz` & `tmp/mlpro-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-1.4.3.tar", last modified: Thu May  9 05:32:50 2024, max compression
+gzip compressed data, was "mlpro-1.4.4.tar", last modified: Sun May 12 10:12:24 2024, max compression
```

## Comparing `mlpro-1.4.3.tar` & `mlpro-1.4.4.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.571494 mlpro-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 05:32:45.000000 mlpro-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 05:32:45.000000 mlpro-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-09 05:32:50.571494 mlpro-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-09 05:32:45.000000 mlpro-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 05:32:46.000000 mlpro-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 05:32:50.571494 mlpro-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.523494 mlpro-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.531494 mlpro-1.4.3/src/mlpro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/data/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/data/buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/data/datastoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/datasets/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.535494 mlpro-1.4.3/src/mlpro/bf/math/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/math/normalizers/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/normalizers/ztrans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/math/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/ml/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/ml/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ml/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/physics/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/physics/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/physics/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/streams/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.539494 mlpro-1.4.3/src/mlpro/bf/streams/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/min_wise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/reservoir_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/samplers/weighted_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/streams/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/csv_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/doublespiral2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/point_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/provider_mlpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/streams/rnd10d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/rearranger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/tasks/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/flipflops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.543494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.527494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.527494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
--rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.527494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
--rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
--rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/ur5.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.547494 mlpro-1.4.3/src/mlpro/bf/ui/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/scenario_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/bf/various.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/dynamicgames/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/dynamicgames/stackelberg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/native/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/native/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/boards/bglp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/native/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.551494 mlpro-1.4.3/src/mlpro/gt/pool/native/games/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/rockpaperscissors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/routingproblems_3p.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/games/supplydemand_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/greedypolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/randomsolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/gt/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/gt/pool/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/sciui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/iis.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/runme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/sciui/scenario_oa1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.555494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/boundarydetectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/tasks/normalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/streams/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/streams/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/systems/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.559494 mlpro-1.4.3/src/mlpro/oa/systems/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/oa/systems/pool/doublependulum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_env_ada.py
--rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_env_oa.py
--rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/mpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/bglp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/doublependulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/gridworld.py
--rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/envs/robotinhtm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.563494 mlpro-1.4.3/src/mlpro/rl/pool/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/policies/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/policies/randomgenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/rl/pool/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/pool/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/rl/sciui_rl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/fnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/models_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/models_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/afct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/sl/pool/afct/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.567494 mlpro-1.4.3/src/mlpro/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/wrappers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-09 05:32:46.000000 mlpro-1.4.3/src/mlpro/wrappers/mujoco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.571494 mlpro-1.4.3/src/mlpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 05:32:50.000000 mlpro-1.4.3/src/mlpro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:32:50.571494 mlpro-1.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_pool_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-09 05:32:46.000000 mlpro-1.4.3/test/test_various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.463186 mlpro-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-12 10:12:19.000000 mlpro-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 10:12:19.000000 mlpro-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-12 10:12:24.463186 mlpro-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-12 10:12:19.000000 mlpro-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-12 10:12:20.000000 mlpro-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-12 10:12:24.463186 mlpro-1.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.419186 mlpro-1.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.427186 mlpro-1.4.4/src/mlpro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.431186 mlpro-1.4.4/src/mlpro/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.431186 mlpro-1.4.4/src/mlpro/bf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/data/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/data/datastoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.431186 mlpro-1.4.4/src/mlpro/bf/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/datasets/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.431186 mlpro-1.4.4/src/mlpro/bf/math/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/math/normalizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/normalizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/normalizers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/normalizers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/normalizers/ztrans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/math/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55808 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ml/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/ml/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ml/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ml/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/ml/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ml/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37878 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/physics/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/physics/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32607 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64843 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.435186 mlpro-1.4.4/src/mlpro/bf/streams/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/samplers/min_wise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/samplers/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/samplers/reservoir_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/samplers/weighted_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.439186 mlpro-1.4.4/src/mlpro/bf/streams/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/csv_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/doublespiral2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/point_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/provider_mlpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/streams/rnd10d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.439186 mlpro-1.4.4/src/mlpro/bf/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/tasks/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/tasks/rearranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/tasks/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.439186 mlpro-1.4.4/src/mlpro/bf/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.439186 mlpro-1.4.4/src/mlpro/bf/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83676 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.439186 mlpro-1.4.4/src/mlpro/bf/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34965 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/flipflops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.439186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.423186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.423186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/
+-rw-r--r--   0 runner    (1001) docker     (127)   322794 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.423186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/boxontable.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/cartpole.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/mlpro.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/ur5.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/ui/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/ui/sciui/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/pool/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.443186 mlpro-1.4.4/src/mlpro/bf/ui/sciui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/ui/sciui/templates/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31658 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/bf/various.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/dynamicgames/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/dynamicgames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/dynamicgames/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/dynamicgames/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/dynamicgames/stackelberg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66293 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/native/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/pool/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/boards/bglp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/pool/native/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/pool/native/games/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/games/rockpaperscissors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/games/routingproblems_3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/games/supplydemand_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/pool/native/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/solvers/greedypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/native/solvers/randomsolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/gt/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/gt/pool/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.447186 mlpro-1.4.4/src/mlpro/oa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/sciui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/sciui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/sciui/iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/sciui/runme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/sciui/scenario_oa1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/boundarydetectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.451186 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/tasks/normalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/oa/streams/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/streams/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/oa/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/systems/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/oa/systems/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/systems/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/oa/systems/pool/doublependulum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36302 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/models_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/models_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/models_env_ada.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/models_env_oa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48989 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/rl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.455186 mlpro-1.4.4/src/mlpro/rl/pool/actionplanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/actionplanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/actionplanner/mpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/rl/pool/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/envs/bglp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/envs/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44837 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/envs/doublependulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/envs/gridworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/envs/robotinhtm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/rl/pool/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/policies/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/policies/randomgenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/rl/pool/sarsbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/sarsbuffer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/rl/pool/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/pool/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65877 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/rl/sciui_rl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/sl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/fnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/models_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40710 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/models_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/sl/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/sl/pool/afct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/pool/afct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/sl/pool/afct/fnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/pool/afct/fnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.459186 mlpro-1.4.4/src/mlpro/sl/pool/afct/fnn/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/pool/afct/fnn/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22451 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/sl/pool/afct/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.463186 mlpro-1.4.4/src/mlpro/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/wrappers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-12 10:12:20.000000 mlpro-1.4.4/src/mlpro/wrappers/mujoco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.463186 mlpro-1.4.4/src/mlpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-12 10:12:24.000000 mlpro-1.4.4/src/mlpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-12 10:12:24.000000 mlpro-1.4.4/src/mlpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:12:24.000000 mlpro-1.4.4/src/mlpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-12 10:12:24.000000 mlpro-1.4.4/src/mlpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 10:12:24.000000 mlpro-1.4.4/src/mlpro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:12:24.463186 mlpro-1.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-12 10:12:20.000000 mlpro-1.4.4/test/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-12 10:12:20.000000 mlpro-1.4.4/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-12 10:12:20.000000 mlpro-1.4.4/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-12 10:12:20.000000 mlpro-1.4.4/test/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-12 10:12:20.000000 mlpro-1.4.4/test/test_pool_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-12 10:12:20.000000 mlpro-1.4.4/test/test_various.py
```

### Comparing `mlpro-1.4.3/LICENSE` & `mlpro-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/PKG-INFO` & `mlpro-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.4.3
+Version: 1.4.4
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-1.4.3/README.md` & `mlpro-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/setup.cfg` & `mlpro-1.4.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro
-version = 1.4.3
+version = 1.4.4
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro.readthedocs.io
 project_urls =
```

### Comparing `mlpro-1.4.3/src/mlpro/bf/data/buffers.py` & `mlpro-1.4.4/src/mlpro/bf/data/buffers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/data/datastoring.py` & `mlpro-1.4.4/src/mlpro/bf/data/datastoring.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/datasets/basics.py` & `mlpro-1.4.4/src/mlpro/bf/datasets/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/events.py` & `mlpro-1.4.4/src/mlpro/bf/events.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/exceptions.py` & `mlpro-1.4.4/src/mlpro/bf/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/math/basics.py` & `mlpro-1.4.4/src/mlpro/bf/math/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/math/geometry.py` & `mlpro-1.4.4/src/mlpro/bf/math/geometry.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/math/normalizers/basics.py` & `mlpro-1.4.4/src/mlpro/bf/math/normalizers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/math/normalizers/minmax.py` & `mlpro-1.4.4/src/mlpro/bf/math/normalizers/minmax.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/math/normalizers/ztrans.py` & `mlpro-1.4.4/src/mlpro/bf/math/normalizers/ztrans.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/math/properties.py` & `mlpro-1.4.4/src/mlpro/bf/math/properties.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ml/basics.py` & `mlpro-1.4.4/src/mlpro/bf/ml/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ml/systems/basics.py` & `mlpro-1.4.4/src/mlpro/bf/ml/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/mt.py` & `mlpro-1.4.4/src/mlpro/bf/mt.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ops.py` & `mlpro-1.4.4/src/mlpro/bf/ops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/physics/basics.py` & `mlpro-1.4.4/src/mlpro/bf/physics/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/physics/unitconverter.py` & `mlpro-1.4.4/src/mlpro/bf/physics/unitconverter.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/plot.py` & `mlpro-1.4.4/src/mlpro/bf/plot.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/models.py` & `mlpro-1.4.4/src/mlpro/bf/streams/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/samplers/min_wise.py` & `mlpro-1.4.4/src/mlpro/bf/streams/samplers/min_wise.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/samplers/random.py` & `mlpro-1.4.4/src/mlpro/bf/streams/samplers/random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/samplers/reservoir_sampling.py` & `mlpro-1.4.4/src/mlpro/bf/streams/samplers/reservoir_sampling.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/samplers/weighted_random.py` & `mlpro-1.4.4/src/mlpro/bf/streams/samplers/weighted_random.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/clouds.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/clouds.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/clusters.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/clusters.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/csv_file.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/csv_file.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/doublespiral2d.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/doublespiral2d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/point_outliers.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/point_outliers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/provider_mlpro.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/provider_mlpro.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/streams/rnd10d.py` & `mlpro-1.4.4/src/mlpro/bf/streams/streams/rnd10d.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/tasks/deriver.py` & `mlpro-1.4.4/src/mlpro/bf/streams/tasks/deriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 ## -- Package : mlpro.bf.streams.tasks
 ## -- Module  : deriver.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2023-02-02  0.0.0     SY       Creation
 ## -- 2023-02-05  1.0.0     SY       First version release
+## -- 2024-05-10  1.0.1     DA/SY    Bugfix in Deriver.__init__()
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.0.0 (2023-02-05)
+Ver. 1.0.1 (2024-05-10)
 
 This module provides a stream task class Deriver to derive the data of instances.
 """
 
 
 from mlpro.bf.exceptions import *
 from mlpro.bf.various import Log
@@ -112,14 +113,15 @@
             label = p_derived_label.copy()
             label._name_short = label._name_short + ' OD-' + str(self._order_derivative)
             label._name_long = label._name_long + ' OD-' + str(self._order_derivative)
             self._label_space.add_dim(p_dim=label)
         
         self._derivative_func = DerivativeFunction(p_name='derivative_func',
                                                    p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                                   p_logging=p_logging,
                                                    p_dt=0,
                                                    order=self._order_derivative)
 
 
 ## -------------------------------------------------------------------------------------------------
     def _derive_data(self, p_inst:Instance):
```

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/tasks/rearranger.py` & `mlpro-1.4.4/src/mlpro/bf/streams/tasks/rearranger.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/streams/tasks/windows.py` & `mlpro-1.4.4/src/mlpro/bf/streams/tasks/windows.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/basics.py` & `mlpro-1.4.4/src/mlpro/bf/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/doublependulum.py` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/flipflops.py` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/flipflops.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Arrow.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/X_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Y_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/mesh/Z_letter.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/mlpro/texture/logo.png`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/base.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/forearm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/shoulder.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/upperarm.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist1.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist2.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/assets/ur5/mesh/wrist3.stl`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/boxontable.xml` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/boxontable.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/cartpole.xml` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/cartpole.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/doublependulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/mlpro.xml` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/mlpro.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/pendulum.xml` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/pendulum.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/systems/pool/mujoco/ur5.xml` & `mlpro-1.4.4/src/mlpro/bf/systems/pool/mujoco/ur5.xml`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ui/sciui/framework.py` & `mlpro-1.4.4/src/mlpro/bf/ui/sciui/framework.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ui/sciui/main.py` & `mlpro-1.4.4/src/mlpro/bf/ui/sciui/main.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iis.py` & `mlpro-1.4.4/src/mlpro/bf/ui/sciui/pool/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py` & `mlpro-1.4.4/src/mlpro/bf/ui/sciui/pool/iisbenchmark.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/ui/sciui/templates/scenario_test.py` & `mlpro-1.4.4/src/mlpro/bf/ui/sciui/templates/scenario_test.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/bf/various.py` & `mlpro-1.4.4/src/mlpro/bf/various.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/dynamicgames/basics.py` & `mlpro-1.4.4/src/mlpro/gt/dynamicgames/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/dynamicgames/potential.py` & `mlpro-1.4.4/src/mlpro/gt/dynamicgames/potential.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/dynamicgames/stackelberg.py` & `mlpro-1.4.4/src/mlpro/gt/dynamicgames/stackelberg.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/native/basics.py` & `mlpro-1.4.4/src/mlpro/gt/native/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/boards/bglp.py` & `mlpro-1.4.4/src/mlpro/gt/pool/boards/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/games/prisonersdilemma_2p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/games/prisonersdilemma_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/games/rockpaperscissors.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/games/rockpaperscissors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/games/routingproblems_3p.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/games/routingproblems_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/games/supplydemand_3p.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/games/supplydemand_3p.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/greedypolicy.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/solvers/greedypolicy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/gt/pool/native/solvers/randomsolver.py` & `mlpro-1.4.4/src/mlpro/gt/pool/native/solvers/randomsolver.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/sciui/iis.py` & `mlpro-1.4.4/src/mlpro/oa/sciui/iis.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/sciui/runme.py` & `mlpro-1.4.4/src/mlpro/oa/sciui/runme.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/sciui/scenario_oa1.py` & `mlpro-1.4.4/src/mlpro/oa/sciui/scenario_oa1.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/basics.py` & `mlpro-1.4.4/src/mlpro/oa/streams/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/clusterbased.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/contextual.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/drift.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/group.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/anomalies/point.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/cb_detectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/anomalydetectors/paga_detectors.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/boundarydetectors.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/boundarydetectors.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,21 +25,23 @@
 ## -- 2023-02-13  1.1.7     LSB      Bug Fix: Setting initial boundaries to [0,0]
 ## -- 2023-04-09  1.2.0     DA       Refactoring of method BoundaryDetector._adapt()
 ## -- 2023-05-02  1.2.1     DA       Class BoundaryDetector
 ## --                                - constructor: removed parameter p_window
 ## --                                - method _adapt(): removed unnecessary code
 ## -- 2023-05-20  1.2.2     DA       Method BoundaryDetector._adapt_on_event: refactoring, corrections
 ## -- 2023-05-21  1.2.3     LSB      Bug Fix : p_scaler shall be generated as a vertical array
-## -- 2023-11-19  1.2.4     DA       Bugfix in Method BoundaryDetection._adapt(): scaler management
+## -- 2023-11-19  1.2.4     DA       Bugfix in method BoundaryDetector._adapt(): scaler management
+## -- 2024-05-12  1.3.0     DA       Removed the scaler functionality from BoundaryDetector
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.2.4 (2023-11-19)
+Ver. 1.3.0 (2024-05-12)
 
 This module provides pool of boundary detector object further used in the context of online adaptivity.
+
 """
 
 import matplotlib.colors
 
 from mlpro.bf.various import *
 from mlpro.bf.plot import *
 from mlpro.bf.math import *
@@ -49,16 +51,16 @@
 
 
 
 ## -------------------------------------------------------------------------------------------------
 ## -------------------------------------------------------------------------------------------------
 class BoundaryDetector (OATask):
     """
-    This is the base class for Boundary Detector object. It raises event when a change in the current boundaries is
-    detected based on the new data instances
+    This class provides the functionality of boundary observation of incoming instances. It raises 
+    event C_EVENT_ADAPTED when a change in the current boundaries is detected.
 
     Parameters
     ----------
     p_name: str, Optional.
         Name of the task.
     p_range_max
         Processing range of the task. Default is thread.
@@ -66,46 +68,42 @@
         True if the task has adaptivity. Default is True.
     p_duplicate_data : bool
         If True, instances will be duplicated before processing. Default = False.
     p_visualize: bool
         True to turn on the visualization.
     p_logging
         Logging level for the task, default is Log all.
-    p_scaler: float, np.ndarray
-        A scaler vector to scale the detected boundaries.
 
     """
 
     C_NAME                      = 'Boundary Detector'
 
     C_PLOT_ND_XLABEL_FEATURE    = 'Features'
     C_PLOT_ND_YLABEL            = 'Boundaries'
 
     C_PLOT_VALID_VIEWS          = [ PlotSettings.C_VIEW_ND ]
 
 ## -------------------------------------------------------------------------------------------------
-    def __init__(self,
-                 p_name:str = None,
-                 p_range_max = MLTask.C_RANGE_THREAD,
-                 p_ada : bool = True,
-                 p_duplicate_data : bool = False,
-                 p_visualize : bool = False,
-                 p_logging=Log.C_LOG_ALL,
-                 p_scaler:Union[float, Iterable] = np.ones(1),
-                 **p_kwargs):
-
-        super().__init__(p_name = p_name,
-                         p_range_max = p_range_max,
-                         p_ada = p_ada,
-                         p_duplicate_data = p_duplicate_data,
-                         p_visualize = p_visualize,
-                         p_logging = p_logging,
-                         **p_kwargs)
+    def __init__( self,
+                  p_name:str = None,
+                  p_range_max = MLTask.C_RANGE_THREAD,
+                  p_ada : bool = True,
+                  p_duplicate_data : bool = False,
+                  p_visualize : bool = False,
+                  p_logging=Log.C_LOG_ALL,
+                  **p_kwargs ):
+
+        super().__init__( p_name = p_name,
+                          p_range_max = p_range_max,
+                          p_ada = p_ada,
+                          p_duplicate_data = p_duplicate_data,
+                          p_visualize = p_visualize,
+                          p_logging = p_logging,
+                          **p_kwargs )
 
-        self._scaler = p_scaler
         self._related_set: Set = None
 
 
 ## -------------------------------------------------------------------------------------------------
     def _adapt(self, p_inst_new:List[Instance]):
         """
         Method to check if the new instances exceed the current boundaries of the Set.
@@ -130,29 +128,26 @@
                 feature_data = inst
 
             # Storing the related set for events
             self._related_set = feature_data.get_related_set()
 
             dim = feature_data.get_related_set().get_dims()
 
-            if len(self._scaler) == 1:
-                self._scaler = np.repeat(self._scaler[0], len(dim), axis=0)
-
             for i,value in enumerate(feature_data.get_values()):
                 boundary = dim[i].get_boundaries()
                 if len(boundary) == 0 or boundary is None:
                     boundary = [ 0,0 ]
                     dim[i].set_boundaries(boundary)
                     adapted = True
 
                 if value < boundary[0]:
-                    dim[i].set_boundaries([value*self._scaler[i], boundary[1]])
+                    dim[i].set_boundaries([value, boundary[1]])
                     adapted = True
                 elif value > boundary[1]:
-                    dim[i].set_boundaries([boundary[0],value*self._scaler[i]])
+                    dim[i].set_boundaries([boundary[0],value])
                     adapted = True
 
         return adapted
 
 
 ## -------------------------------------------------------------------------------------------------
     def _run(self, p_inst_new:List[Element], p_inst_del:List[Element]):
@@ -188,34 +183,34 @@
             bool
                 Returns true if adapted, false otherwise.
         """
 
         adapted = False
         
         try:
-            bd_new = self._scaler*p_event_object.get_raising_object().get_boundaries()
-            self._related_set = p_event_object.get_data()["p_related_set"]
-            dims = self._related_set.get_dims()
-
-            for i,dim in enumerate(dims):
-                bd_dim_current = dim.get_boundaries()
-                bd_dim_new     = bd_new[i]
-
-                if ( bd_dim_new[0] != bd_dim_current[0] ) or ( bd_dim_new[1] != bd_dim_current[1] ):
-                    dim.set_boundaries(bd_dim_new)
-                    adapted = True
+            bd_new = p_event_object.get_raising_object().get_boundaries()
         except: 
             raise ImplementationError("Event not raised by a window")
         
+        self._related_set = p_event_object.get_data()["p_related_set"]
+        dims = self._related_set.get_dims()
+
+        for i,dim in enumerate(dims):
+            bd_dim_current = dim.get_boundaries()
+            bd_dim_new     = bd_new[i]
+
+            if ( bd_dim_new[0] != bd_dim_current[0] ) or ( bd_dim_new[1] != bd_dim_current[1] ):
+                dim.set_boundaries(bd_dim_new)
+                adapted = True
+        
         return adapted
 
 
 ## -------------------------------------------------------------------------------------------------
     def get_related_set(self):
-
         return self._related_set
 
 
 ## -------------------------------------------------------------------------------------------------
     def _init_plot_nd(self, p_figure: Figure, p_settings: PlotSettings):
         """
         Custom method to initialize plot for Boundary Detectors tasks for N-dimensional plotting.
```

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/centroid.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/clusteranalyzers/clusters/properties/centroid.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/streams/tasks/normalizers.py` & `mlpro-1.4.4/src/mlpro/oa/streams/tasks/normalizers.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/systems/basics.py` & `mlpro-1.4.4/src/mlpro/oa/systems/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/oa/systems/pool/doublependulum.py` & `mlpro-1.4.4/src/mlpro/oa/systems/pool/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/models.py` & `mlpro-1.4.4/src/mlpro/rl/models.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/models_agents.py` & `mlpro-1.4.4/src/mlpro/rl/models_agents.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/models_env.py` & `mlpro-1.4.4/src/mlpro/rl/models_env.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/models_env_ada.py` & `mlpro-1.4.4/src/mlpro/rl/models_env_ada.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/models_env_oa.py` & `mlpro-1.4.4/src/mlpro/rl/models_env_oa.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/models_train.py` & `mlpro-1.4.4/src/mlpro/rl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/actionplanner/mpc.py` & `mlpro-1.4.4/src/mlpro/rl/pool/actionplanner/mpc.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/envs/bglp.py` & `mlpro-1.4.4/src/mlpro/rl/pool/envs/bglp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/envs/cartpole.py` & `mlpro-1.4.4/src/mlpro/rl/pool/envs/cartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/envs/doublependulum.py` & `mlpro-1.4.4/src/mlpro/rl/pool/envs/doublependulum.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/envs/gridworld.py` & `mlpro-1.4.4/src/mlpro/rl/pool/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/envs/robotinhtm.py` & `mlpro-1.4.4/src/mlpro/rl/pool/envs/robotinhtm.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/policies/dummy.py` & `mlpro-1.4.4/src/mlpro/rl/pool/policies/dummy.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/policies/randomgenerator.py` & `mlpro-1.4.4/src/mlpro/rl/pool/policies/randomgenerator.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py` & `mlpro-1.4.4/src/mlpro/rl/pool/sarsbuffer/PrioritizedBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py` & `mlpro-1.4.4/src/mlpro/rl/pool/sarsbuffer/RandomSARSBuffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/rl/sciui_rl.py` & `mlpro-1.4.4/src/mlpro/rl/sciui_rl.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/basics.py` & `mlpro-1.4.4/src/mlpro/sl/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py` & `mlpro-1.4.4/src/mlpro/sl/examples/howto_sl_afct_100_train_and_reload_pytorch_mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/fnn.py` & `mlpro-1.4.4/src/mlpro/sl/fnn.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/models_eval.py` & `mlpro-1.4.4/src/mlpro/sl/models_eval.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/models_train.py` & `mlpro-1.4.4/src/mlpro/sl/models_train.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py` & `mlpro-1.4.4/src/mlpro/sl/pool/afct/fnn/pytorch/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/sl/pool/afct/pytorch.py` & `mlpro-1.4.4/src/mlpro/sl/pool/afct/pytorch.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/wrappers/basics.py` & `mlpro-1.4.4/src/mlpro/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro/wrappers/mujoco.py` & `mlpro-1.4.4/src/mlpro/wrappers/mujoco.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/src/mlpro.egg-info/PKG-INFO` & `mlpro-1.4.4/src/mlpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro
-Version: 1.4.3
+Version: 1.4.4
 Summary: MLPro - The Integrative Middleware Framework for Standardized Machine Learning
 Home-page: https://mlpro.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-1.4.3/src/mlpro.egg-info/SOURCES.txt` & `mlpro-1.4.4/src/mlpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/test/test_buffer.py` & `mlpro-1.4.4/test/test_buffer.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/test/test_environment.py` & `mlpro-1.4.4/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/test/test_examples.py` & `mlpro-1.4.4/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/test/test_math.py` & `mlpro-1.4.4/test/test_math.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/test/test_pool_policies.py` & `mlpro-1.4.4/test/test_pool_policies.py`

 * *Files identical despite different names*

### Comparing `mlpro-1.4.3/test/test_various.py` & `mlpro-1.4.4/test/test_various.py`

 * *Files identical despite different names*

