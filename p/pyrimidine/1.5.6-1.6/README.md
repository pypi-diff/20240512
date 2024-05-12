# Comparing `tmp/pyrimidine-1.5.6.tar.gz` & `tmp/pyrimidine-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrimidine-1.5.6.tar", max compression
+gzip compressed data, was "pyrimidine-1.6.tar", max compression
```

## Comparing `pyrimidine-1.5.6.tar` & `pyrimidine-1.6.tar`

### file list

```diff
@@ -1,94 +1,97 @@
--rw-r--r--   0        0        0    13288 2023-12-13 08:35:34.078661 pyrimidine-1.5.6/README.md
--rw-r--r--   0        0        0      949 2024-01-03 12:11:36.555015 pyrimidine-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     2829 2023-12-10 11:53:19.296931 pyrimidine-1.5.6/pyrimidine/-aco.py
--rwxr-xr-x   0        0        0     1932 2024-01-02 03:41:10.031481 pyrimidine-1.5.6/pyrimidine/__init__.py
--rw-r--r--   0        0        0     2204 2023-12-14 03:06:01.675590 pyrimidine-1.5.6/pyrimidine/_stat.py
--rw-r--r--   0        0        0     2546 2023-12-15 03:28:15.996519 pyrimidine-1.5.6/pyrimidine/ba.py
--rwxr-xr-x   0        0        0    16023 2024-01-02 04:03:21.777910 pyrimidine-1.5.6/pyrimidine/base.py
--rwxr-xr-x   0        0        0      348 2024-01-02 04:17:25.365477 pyrimidine-1.5.6/pyrimidine/benchmarks/__init__.py
--rw-r--r--   0        0        0      716 2024-01-02 04:18:32.947565 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-12-05 05:48:05.462908 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      662 2023-12-05 05:48:05.463366 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2217 2024-01-02 04:01:35.521899 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-310.pyc
--rw-r--r--   0        0        0     1689 2023-12-05 05:48:05.464269 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-37.pyc
--rw-r--r--   0        0        0     1826 2023-12-05 05:48:05.464558 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-38.pyc
--rw-r--r--   0        0        0      708 2023-12-05 05:48:05.464789 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     1902 2024-01-02 05:12:50.602257 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-310.pyc
--rw-r--r--   0        0        0     1808 2023-12-05 05:48:05.465132 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-37.pyc
--rw-r--r--   0        0        0     1851 2023-12-05 05:48:05.465416 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-38.pyc
--rw-r--r--   0        0        0     4379 2024-01-02 04:01:35.548711 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-310.pyc
--rw-r--r--   0        0        0     4289 2023-12-05 05:48:05.465684 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-37.pyc
--rw-r--r--   0        0        0     4746 2023-12-05 05:48:05.465987 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-38.pyc
--rw-r--r--   0        0        0      626 2024-01-02 04:01:35.592141 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-310.pyc
--rw-r--r--   0        0        0      592 2023-12-05 05:48:05.466335 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-37.pyc
--rw-r--r--   0        0        0      608 2023-12-05 05:48:05.466582 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-38.pyc
--rw-r--r--   0        0        0     1221 2024-01-02 04:01:35.604739 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-310.pyc
--rw-r--r--   0        0        0     1003 2023-12-05 05:48:05.467121 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-37.pyc
--rw-r--r--   0        0        0     1090 2023-12-05 05:48:05.467437 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-38.pyc
--rw-r--r--   0        0        0     2603 2024-01-02 04:15:37.431044 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-310.pyc
--rw-r--r--   0        0        0     1405 2023-12-05 05:48:05.468267 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-37.pyc
--rw-r--r--   0        0        0     1461 2023-12-05 05:48:05.468567 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-38.pyc
--rw-r--r--   0        0        0    10564 2023-12-07 05:36:36.325546 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-310.pyc
--rw-r--r--   0        0        0     3519 2023-12-05 05:48:05.470033 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-37.pyc
--rw-r--r--   0        0        0     7984 2023-12-05 05:48:05.470653 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-38.pyc
--rw-r--r--   0        0        0      840 2024-01-02 05:11:40.420055 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/others.cpython-310.pyc
--rw-r--r--   0        0        0      779 2023-12-05 05:48:05.471006 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/others.cpython-38.pyc
--rw-r--r--   0        0        0     2060 2023-12-07 05:36:36.456069 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/special.cpython-310.pyc
--rw-r--r--   0        0        0      627 2023-12-05 05:48:05.471747 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/special.cpython-37.pyc
--rw-r--r--   0        0        0     2174 2023-12-05 05:48:05.472438 pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/special.cpython-38.pyc
--rwxr-xr-x   0        0        0     1006 2023-12-05 05:48:05.472821 pyrimidine-1.5.6/pyrimidine/benchmarks/approximation.py
--rwxr-xr-x   0        0        0     1676 2024-01-02 05:12:43.025669 pyrimidine-1.5.6/pyrimidine/benchmarks/cluster.py
--rwxr-xr-x   0        0        0     1918 2023-12-05 05:48:05.474971 pyrimidine-1.5.6/pyrimidine/benchmarks/fitting.py
--rwxr-xr-x   0        0        0      248 2023-12-05 05:48:05.475902 pyrimidine-1.5.6/pyrimidine/benchmarks/linear_model.py
--rwxr-xr-x   0        0        0      703 2023-12-05 05:48:05.476351 pyrimidine-1.5.6/pyrimidine/benchmarks/matrix.py
--rwxr-xr-x   0        0        0     1597 2024-01-02 04:13:08.749759 pyrimidine-1.5.6/pyrimidine/benchmarks/neural_network.py
--rwxr-xr-x   0        0        0     6169 2023-12-05 05:48:05.477853 pyrimidine-1.5.6/pyrimidine/benchmarks/optimization.py
--rw-r--r--   0        0        0      382 2024-01-02 05:02:39.747004 pyrimidine-1.5.6/pyrimidine/benchmarks/others.py
--rwxr-xr-x   0        0        0      958 2024-01-02 06:09:15.826675 pyrimidine-1.5.6/pyrimidine/benchmarks/special.py
--rw-r--r--   0        0        0  5498962 2023-12-05 05:48:05.535865 pyrimidine-1.5.6/pyrimidine/benchmarks/test_dataset.csv
--rw-r--r--   0        0        0  5698411 2023-12-05 05:48:05.677089 pyrimidine-1.5.6/pyrimidine/benchmarks/train_dataset.csv
--rwxr-xr-x   0        0        0    11938 2023-12-23 04:56:22.696038 pyrimidine-1.5.6/pyrimidine/chromosome.py
--rw-r--r--   0        0        0     1837 2023-12-20 07:05:17.904508 pyrimidine-1.5.6/pyrimidine/de.py
--rwxr-xr-x   0        0        0    10827 2024-01-02 04:01:17.416097 pyrimidine-1.5.6/pyrimidine/deco.py
--rw-r--r--   0        0        0     2210 2023-12-18 12:07:39.422454 pyrimidine-1.5.6/pyrimidine/ep.py
--rwxr-xr-x   0        0        0      803 2023-12-05 06:32:40.371036 pyrimidine-1.5.6/pyrimidine/errors.py
--rw-r--r--   0        0        0      992 2023-12-12 03:34:32.067491 pyrimidine-1.5.6/pyrimidine/es.py
--rwxr-xr-x   0        0        0     1306 2023-12-14 07:57:02.075957 pyrimidine-1.5.6/pyrimidine/fa.py
--rwxr-xr-x   0        0        0     1281 2024-01-02 04:07:34.731303 pyrimidine-1.5.6/pyrimidine/gene.py
--rw-r--r--   0        0        0     3060 2023-12-07 07:55:48.978651 pyrimidine-1.5.6/pyrimidine/gsa.py
--rwxr-xr-x   0        0        0     4935 2023-12-20 06:38:30.629705 pyrimidine-1.5.6/pyrimidine/individual.py
--rwxr-xr-x   0        0        0     1225 2023-12-18 12:26:01.940087 pyrimidine-1.5.6/pyrimidine/learn/__init__.py
--rw-r--r--   0        0        0     1387 2023-12-18 12:42:17.821710 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      321 2023-12-05 05:48:05.686055 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      569 2023-12-07 05:37:13.576194 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      559 2023-12-05 05:48:05.686504 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     2457 2023-12-18 12:47:26.435254 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/linear_regression.cpython-310.pyc
--rw-r--r--   0        0        0     2462 2023-12-18 12:47:26.384859 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/neural_network.cpython-310.pyc
--rw-r--r--   0        0        0     2564 2023-12-05 05:48:05.686730 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/neural_network.cpython-38.pyc
--rw-r--r--   0        0        0     4244 2023-12-05 05:48:05.688948 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/regression.cpython-310.pyc
--rw-r--r--   0        0        0     3171 2023-12-05 05:48:05.689506 pyrimidine-1.5.6/pyrimidine/learn/__pycache__/regression.cpython-38.pyc
--rwxr-xr-x   0        0        0     1101 2023-12-18 12:49:54.583019 pyrimidine-1.5.6/pyrimidine/learn/cluster.py
--rwxr-xr-x   0        0        0     1579 2023-12-18 12:47:22.823421 pyrimidine-1.5.6/pyrimidine/learn/linear_regression.py
--rw-r--r--   0        0        0     1976 2023-12-18 12:47:15.999017 pyrimidine-1.5.6/pyrimidine/learn/neural_network.py
--rwxr-xr-x   0        0        0      113 2023-12-05 05:48:05.691660 pyrimidine-1.5.6/pyrimidine/local_search/__init__.py
--rw-r--r--   0        0        0      257 2023-12-08 11:57:02.186848 pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1138 2023-12-08 11:57:02.191124 pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/random_walk.cpython-310.pyc
--rw-r--r--   0        0        0     1453 2024-01-02 04:15:37.632494 pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/simulated_annealing.cpython-310.pyc
--rw-r--r--   0        0        0     1909 2023-12-12 03:50:17.125328 pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/tabu_search.cpython-310.pyc
--rwxr-xr-x   0        0        0      619 2023-12-05 05:48:05.693189 pyrimidine-1.5.6/pyrimidine/local_search/random_walk.py
--rwxr-xr-x   0        0        0     1344 2024-01-02 04:14:18.326893 pyrimidine-1.5.6/pyrimidine/local_search/simulated_annealing.py
--rwxr-xr-x   0        0        0     1871 2023-12-10 12:40:49.542863 pyrimidine-1.5.6/pyrimidine/local_search/tabu_search.py
--rwxr-xr-x   0        0        0    17571 2024-01-02 04:15:24.933811 pyrimidine-1.5.6/pyrimidine/meta.py
--rwxr-xr-x   0        0        0    14851 2024-01-02 03:36:45.640212 pyrimidine-1.5.6/pyrimidine/mixin.py
--rwxr-xr-x   0        0        0     3337 2024-01-02 03:22:42.946226 pyrimidine-1.5.6/pyrimidine/multipopulation.py
--rw-r--r--   0        0        0     4324 2023-12-20 06:14:44.434504 pyrimidine-1.5.6/pyrimidine/optimize.py
--rwxr-xr-x   0        0        0     3427 2023-12-22 12:41:48.326734 pyrimidine-1.5.6/pyrimidine/parallel.py
--rwxr-xr-x   0        0        0     6324 2023-12-15 04:11:50.189396 pyrimidine-1.5.6/pyrimidine/population.py
--rwxr-xr-x   0        0        0     6022 2023-12-22 03:11:16.959134 pyrimidine-1.5.6/pyrimidine/pso.py
--rwxr-xr-x   0        0        0      636 2023-12-10 11:13:25.083406 pyrimidine-1.5.6/pyrimidine/qga.py
--rwxr-xr-x   0        0        0     3928 2023-12-29 13:52:10.427547 pyrimidine-1.5.6/pyrimidine/saga.py
--rwxr-xr-x   0        0        0     2010 2023-12-15 04:14:52.881686 pyrimidine-1.5.6/pyrimidine/sma.py
--rw-r--r--   0        0        0      879 2023-12-10 11:20:27.348322 pyrimidine-1.5.6/pyrimidine/studga.py
--rwxr-xr-x   0        0        0     5199 2023-12-23 04:23:49.239524 pyrimidine-1.5.6/pyrimidine/utils.py
--rw-r--r--   0        0        0    14505 2024-01-03 13:17:35.318850 pyrimidine-1.5.6/setup.py
--rw-r--r--   0        0        0    14368 2024-01-03 13:17:35.320730 pyrimidine-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0    14708 2024-05-12 15:21:33.211063 pyrimidine-1.6/README.md
+-rw-r--r--   0        0        0     1181 2024-05-12 15:34:14.204118 pyrimidine-1.6/pyproject.toml
+-rw-r--r--   0        0        0     8196 2023-11-10 03:51:23.712167 pyrimidine-1.6/pyrimidine/.DS_Store
+-rwxr-xr-x   0        0        0     1954 2024-05-12 15:15:16.912175 pyrimidine-1.6/pyrimidine/__init__.py
+-rw-r--r--   0        0        0     2204 2023-12-14 03:06:01.675590 pyrimidine-1.6/pyrimidine/_stat.py
+-rw-r--r--   0        0        0     4250 2024-05-10 06:37:21.648433 pyrimidine-1.6/pyrimidine/aco.py
+-rw-r--r--   0        0        0     2546 2023-12-15 03:28:15.996519 pyrimidine-1.6/pyrimidine/ba.py
+-rwxr-xr-x   0        0        0    16324 2024-05-10 10:05:52.716308 pyrimidine-1.6/pyrimidine/base.py
+-rw-r--r--   0        0        0     6148 2020-07-30 07:57:24.710084 pyrimidine-1.6/pyrimidine/benchmarks/.DS_Store
+-rwxr-xr-x   0        0        0      348 2023-12-04 09:44:43.549814 pyrimidine-1.6/pyrimidine/benchmarks/__init__.py
+-rw-r--r--   0        0        0      710 2023-12-04 09:48:15.352629 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2020-07-04 07:37:10.190991 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      662 2021-08-13 05:25:35.712525 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2203 2023-12-04 10:00:54.437015 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-310.pyc
+-rw-r--r--   0        0        0     1689 2020-07-30 08:00:31.360866 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-37.pyc
+-rw-r--r--   0        0        0     1826 2020-11-10 12:55:01.202783 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-38.pyc
+-rw-r--r--   0        0        0      708 2021-08-13 00:24:41.103769 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     1851 2023-12-04 11:10:31.273741 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-310.pyc
+-rw-r--r--   0        0        0     1808 2020-07-14 07:44:19.152719 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-37.pyc
+-rw-r--r--   0        0        0     1851 2020-09-17 08:36:11.664304 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-38.pyc
+-rw-r--r--   0        0        0     4534 2023-12-04 12:14:53.380570 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-310.pyc
+-rw-r--r--   0        0        0     4289 2020-07-31 13:21:21.631748 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-37.pyc
+-rw-r--r--   0        0        0     4746 2020-10-29 02:54:11.961270 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-38.pyc
+-rw-r--r--   0        0        0      612 2023-12-04 11:10:31.334123 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-310.pyc
+-rw-r--r--   0        0        0      592 2020-07-04 07:37:29.120579 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-37.pyc
+-rw-r--r--   0        0        0      608 2020-11-10 12:55:01.691457 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-38.pyc
+-rw-r--r--   0        0        0     1207 2023-12-04 10:14:10.040756 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-310.pyc
+-rw-r--r--   0        0        0     1003 2020-07-21 03:52:18.364202 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-37.pyc
+-rw-r--r--   0        0        0     1090 2021-08-06 07:25:28.378549 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-38.pyc
+-rw-r--r--   0        0        0     2594 2023-12-04 12:36:35.286700 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-310.pyc
+-rw-r--r--   0        0        0     1405 2020-07-14 12:23:22.447040 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-37.pyc
+-rw-r--r--   0        0        0     1461 2020-11-30 07:36:47.262387 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-38.pyc
+-rw-r--r--   0        0        0    10558 2023-12-25 06:04:05.331354 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-310.pyc
+-rw-r--r--   0        0        0     3519 2020-07-17 07:41:24.379611 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-37.pyc
+-rw-r--r--   0        0        0     7984 2021-08-12 09:46:10.050883 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-38.pyc
+-rw-r--r--   0        0        0      822 2023-12-04 11:10:31.622414 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/others.cpython-310.pyc
+-rw-r--r--   0        0        0      779 2020-11-10 12:55:02.521074 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/others.cpython-38.pyc
+-rw-r--r--   0        0        0     2054 2023-12-04 12:36:35.411747 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/special.cpython-310.pyc
+-rw-r--r--   0        0        0      627 2020-07-05 10:27:58.776919 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/special.cpython-37.pyc
+-rw-r--r--   0        0        0     2174 2020-11-09 05:38:14.047855 pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/special.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1006 2023-12-04 10:00:51.595600 pyrimidine-1.6/pyrimidine/benchmarks/approximation.py
+-rwxr-xr-x   0        0        0     1641 2023-12-04 09:44:43.552791 pyrimidine-1.6/pyrimidine/benchmarks/cluster.py
+-rwxr-xr-x   0        0        0     2081 2023-12-04 12:14:37.504477 pyrimidine-1.6/pyrimidine/benchmarks/fitting.py
+-rwxr-xr-x   0        0        0      248 2023-12-04 09:44:43.550854 pyrimidine-1.6/pyrimidine/benchmarks/linear_model.py
+-rwxr-xr-x   0        0        0      703 2023-12-04 09:44:43.547825 pyrimidine-1.6/pyrimidine/benchmarks/matrix.py
+-rwxr-xr-x   0        0        0     6169 2023-12-25 06:03:59.901052 pyrimidine-1.6/pyrimidine/benchmarks/optimization.py
+-rw-r--r--   0        0        0      369 2023-12-04 09:44:43.556776 pyrimidine-1.6/pyrimidine/benchmarks/others.py
+-rwxr-xr-x   0        0        0      957 2023-12-04 11:53:26.723266 pyrimidine-1.6/pyrimidine/benchmarks/special.py
+-rw-r--r--   0        0        0  5498962 2019-01-17 06:04:08.000000 pyrimidine-1.6/pyrimidine/benchmarks/test_dataset.csv
+-rw-r--r--   0        0        0  5698411 2019-01-17 06:22:22.000000 pyrimidine-1.6/pyrimidine/benchmarks/train_dataset.csv
+-rwxr-xr-x   0        0        0    12135 2024-03-21 05:29:01.979339 pyrimidine-1.6/pyrimidine/chromosome.py
+-rw-r--r--   0        0        0     1837 2023-12-20 07:05:17.904508 pyrimidine-1.6/pyrimidine/de.py
+-rwxr-xr-x   0        0        0    10827 2024-01-02 04:01:17.416097 pyrimidine-1.6/pyrimidine/deco.py
+-rw-r--r--   0        0        0     2406 2024-05-10 10:03:47.301122 pyrimidine-1.6/pyrimidine/ep.py
+-rwxr-xr-x   0        0        0      803 2023-12-05 06:32:40.371036 pyrimidine-1.6/pyrimidine/errors.py
+-rw-r--r--   0        0        0     1146 2024-03-05 14:58:03.606050 pyrimidine-1.6/pyrimidine/es.py
+-rwxr-xr-x   0        0        0     1573 2024-03-21 05:31:33.402864 pyrimidine-1.6/pyrimidine/fa.py
+-rwxr-xr-x   0        0        0     1281 2024-01-02 04:07:34.731303 pyrimidine-1.6/pyrimidine/gene.py
+-rw-r--r--   0        0        0     3893 2024-03-21 05:48:22.371602 pyrimidine-1.6/pyrimidine/gsa.py
+-rwxr-xr-x   0        0        0     5044 2024-03-05 15:05:45.401927 pyrimidine-1.6/pyrimidine/individual.py
+-rwxr-xr-x   0        0        0     1225 2023-12-18 12:26:01.940087 pyrimidine-1.6/pyrimidine/learn/__init__.py
+-rw-r--r--   0        0        0     1381 2023-12-29 13:52:52.223197 pyrimidine-1.6/pyrimidine/learn/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      321 2023-12-05 05:48:05.686055 pyrimidine-1.6/pyrimidine/learn/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      569 2023-12-07 05:37:13.576194 pyrimidine-1.6/pyrimidine/learn/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      559 2023-12-05 05:48:05.686504 pyrimidine-1.6/pyrimidine/learn/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     2377 2023-12-29 13:52:52.369361 pyrimidine-1.6/pyrimidine/learn/__pycache__/linear_regression.cpython-310.pyc
+-rw-r--r--   0        0        0     2456 2023-12-29 13:52:52.619156 pyrimidine-1.6/pyrimidine/learn/__pycache__/neural_network.cpython-310.pyc
+-rw-r--r--   0        0        0     2564 2023-12-05 05:48:05.686730 pyrimidine-1.6/pyrimidine/learn/__pycache__/neural_network.cpython-38.pyc
+-rw-r--r--   0        0        0     4244 2023-12-05 05:48:05.688948 pyrimidine-1.6/pyrimidine/learn/__pycache__/regression.cpython-310.pyc
+-rw-r--r--   0        0        0     3171 2023-12-05 05:48:05.689506 pyrimidine-1.6/pyrimidine/learn/__pycache__/regression.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1058 2023-12-15 08:36:16.772521 pyrimidine-1.6/pyrimidine/learn/cluster.py
+-rwxr-xr-x   0        0        0     1478 2023-12-18 12:37:50.163723 pyrimidine-1.6/pyrimidine/learn/linear_regression.py
+-rw-r--r--   0        0        0     1976 2023-12-18 11:41:50.883032 pyrimidine-1.6/pyrimidine/learn/neural_network.py
+-rw-r--r--   0        0        0     6148 2020-07-28 04:09:15.923549 pyrimidine-1.6/pyrimidine/local_search/.DS_Store
+-rwxr-xr-x   0        0        0      113 2023-12-04 09:44:43.538832 pyrimidine-1.6/pyrimidine/local_search/__init__.py
+-rw-r--r--   0        0        0      251 2023-12-04 11:10:33.337894 pyrimidine-1.6/pyrimidine/local_search/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1132 2023-12-04 11:10:33.342586 pyrimidine-1.6/pyrimidine/local_search/__pycache__/random_walk.cpython-310.pyc
+-rw-r--r--   0        0        0     1500 2023-12-04 11:10:33.340147 pyrimidine-1.6/pyrimidine/local_search/__pycache__/simulated_annealing.cpython-310.pyc
+-rw-r--r--   0        0        0     1903 2023-12-14 05:53:21.967930 pyrimidine-1.6/pyrimidine/local_search/__pycache__/tabu_search.cpython-310.pyc
+-rwxr-xr-x   0        0        0      619 2023-12-04 10:04:14.927386 pyrimidine-1.6/pyrimidine/local_search/random_walk.py
+-rwxr-xr-x   0        0        0     1344 2024-05-10 09:59:17.614626 pyrimidine-1.6/pyrimidine/local_search/simulated_annealing.py
+-rwxr-xr-x   0        0        0     2111 2024-03-21 05:25:57.393312 pyrimidine-1.6/pyrimidine/local_search/tabu_search.py
+-rw-r--r--   0        0        0    17771 2024-05-10 10:07:26.872894 pyrimidine-1.6/pyrimidine/meta.py
+-rwxr-xr-x   0        0        0    15697 2024-05-12 14:43:41.640398 pyrimidine-1.6/pyrimidine/mixin.py
+-rwxr-xr-x   0        0        0     3337 2024-01-02 03:22:42.946226 pyrimidine-1.6/pyrimidine/multipopulation.py
+-rw-r--r--   0        0        0     5262 2024-05-10 09:55:47.943846 pyrimidine-1.6/pyrimidine/optimize.py
+-rwxr-xr-x   0        0        0     3427 2023-12-22 12:41:48.326734 pyrimidine-1.6/pyrimidine/parallel.py
+-rwxr-xr-x   0        0        0     6380 2024-03-05 15:05:30.624597 pyrimidine-1.6/pyrimidine/population.py
+-rwxr-xr-x   0        0        0     6033 2024-03-21 05:45:03.508822 pyrimidine-1.6/pyrimidine/pso.py
+-rwxr-xr-x   0        0        0      636 2023-12-10 11:13:25.083406 pyrimidine-1.6/pyrimidine/qga.py
+-rwxr-xr-x   0        0        0     3928 2023-12-29 13:52:10.427547 pyrimidine-1.6/pyrimidine/saga.py
+-rwxr-xr-x   0        0        0     2010 2023-12-15 04:14:52.881686 pyrimidine-1.6/pyrimidine/sma.py
+-rw-r--r--   0        0        0     3039 2024-03-25 05:59:26.223292 pyrimidine-1.6/pyrimidine/ssa.py
+-rw-r--r--   0        0        0      879 2023-12-10 11:20:27.348322 pyrimidine-1.6/pyrimidine/studga.py
+-rwxr-xr-x   0        0        0     5121 2024-04-08 02:16:50.855302 pyrimidine-1.6/pyrimidine/utils.py
+-rw-r--r--   0        0        0    16194 2024-05-12 15:34:26.982848 pyrimidine-1.6/setup.py
+-rw-r--r--   0        0        0    16052 2024-05-12 15:34:26.984002 pyrimidine-1.6/PKG-INFO
```

### Comparing `pyrimidine-1.5.6/README.md` & `pyrimidine-1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -65,19 +65,39 @@
 - BaseGene: the gene of chromosome
 - BaseChromosome: sequence of genes, represents part of a solution
 - BaseIndividual: sequence of chromosomes, represents a solution of a problem
 - BasePopulation: a container of individuals, represents a container of a problem
                 also the state of a stachostic process
 - BaseMultipopulation: a container of population for more complicated optimalization
 
-
 ### import
-Just use the command `from pyrimidine import *` import all of the algorithms.
 
-### subclass
+To import all algorithms for beginners, simply use the command `from pyrimidine import *`.
+
+To speed the lib, use the following commands 
+```
+from pyrimidine import BaseChromosome, BaseIndividual, BasePopulation # import the base classes form `base.py` to build your own classes
+
+# Commands used frequently
+from pyrimidine.base import BinaryChromosome, FloatChromosome # import the Chromosome classes and utilize them directly
+# equivalent to `from pyrimidine import BinaryChromosome, FloatChromosome`
+from pyrimidine.population import StandardPopulation, HOFPopulation # For creating population with standard GA 
+# the same effect with `from pyrimidine import StandardPopulation, HOFPopulation`
+from pyrimidine.indiviual import makeIndividual # a helper to make Individual objects, or `from pyrimidine import makeIndividual`
+
+from pyrimidine import MultiPopulation # build the multi-populations
+from pyrimidine import MetaContainer # meta class for socalled container class, that is recommended to be used for creating novel evolutionary algorithms.
+
+from pyrimidine.deco import * # import all decorators
+from pyrimidine.deco import fitness_cache, basic_memory # use the cache decorator and memory decorator
+
+from pyrimidine import optimize # do optimization implictly with GAs
+```
+
+### subclasses
 
 #### Chromosome
 
 Generally, it is an array of genes.
 
 As an array of 0-1s, `BinaryChromosome` is used most frequently.
 
@@ -236,14 +256,16 @@
 
 ```python
 t = np.random.randint(1, 5, 100)
 n = np.random.randint(1, 4, 100)
 
 import collections
 
+from pyrimidine.individual import makeBinaryIndividual
+from pyrimidine.population import StandardPopulation
 
 def max_repeat(x):
     # Maximum repetition
     c = collections.Counter(x)
     return np.max([b for a, b in c.items()])
 
 
@@ -264,14 +286,17 @@
 ```
 
 Note that there is only one chromosome in `MonoIndividual`, which could be got by `self.chromosome`.
 
 In fact, the population could be the container of chromosomes. Therefore, we can rewrite the classes as follows in a more natural way.
 
 ```python
+from pyrimidine.chromosome import BinaryChromosome
+from pyrimidine.population import StandardPopulation
+
 class MyChromosome(BinaryChromosome):
 
     def _fitness(self):
         x = abs(np.dot(n, self)-10)
         y = max_repeat(ti for ti, c in zip(t, self) if c==1)
         return - x - y
```

### Comparing `pyrimidine-1.5.6/pyrimidine/__init__.py` & `pyrimidine-1.6/pyrimidine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from .mixin import *
 from .errors import *
 from .gene import *
 from .chromosome import *
 from .individual import *
 from .population import *
 from .multipopulation import *
+
+# deprecated in future
 from .saga import *
 from .studga import *
 from .pso import *
 from .es import *
 from .ep import *
 from .de import *
 from .ba import *
 
 
-__version__ = "1.5.6"
+__version__ = "1.6"
 
 __template__ = """
 from pyrimidine.chromosome import BinaryChromosome
 from pyrimidine.individual import MonoIndividual, binaryIndividual
 from pyrimidine.population import StandardPopulation
 
 from pyrimidine.benchmarks.optimization import *
```

### Comparing `pyrimidine-1.5.6/pyrimidine/_stat.py` & `pyrimidine-1.6/pyrimidine/_stat.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/ba.py` & `pyrimidine-1.6/pyrimidine/ba.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/base.py` & `pyrimidine-1.6/pyrimidine/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,61 +2,67 @@
 
 """
 The base classes are defined here, mainly for implementation of GAs.
 
 This is the core module of pyrimidine. 
 
 Main classes:
+
     BaseGene: the gene of chromosome
     BaseChromosome: sequence of genes, represents part of a solution
     BaseIndividual: sequence of chromosomes, represents a solution of a problem
     BasePopulation: set of individuals, represents a set of a problem
                     also the state of a stachostic process
     BaseMultiPopulation/BaseCommunity: set of populations for more complicated optimalization
     BaseEnviorenment:
 
 Remark:
 1. Subclass the classes and override some main method esp. `_fitness`.
-2. `BaseGene` is not important
+2. `BaseGene` is not important, as a wrapper of np.int_ and np.float_
+3. The base classes have been crafted specifically for GA-style algorithms.
+  If your novel algorithm differs from GAs, it is advisable to derive from the mixin classes. 
 
 Example:
+
     select ti, ni from arraies t, n
     sum of ni ~ 10 (for example), while ti are exptected to be not repeated
 
-The opt. problem is
+    The opt. problem is
     min sum of {ni} and maximum of frequences in {ti}
     where i are selected indexes.
 
-t = np.random.randint(1, 5, 100)
-n = np.random.randint(1, 4, 100)
-
-import collections
-def max_repeat(x):
-    # maximum of numbers of repeats
-    c = collections.Counter(x)
-    bm=np.argmax([b for a, b in c.items()])
-    return list(c.keys())[bm]
-
-class MyIndividual(MonoIndividual):
-
-    element_class = BinaryChromosome
-
-    def _fitness(self):
-        x = self.evaluate()
-        return - x[0] - x[1]
-
-    def evaluate(self):
-        return np.dot(n, self.chromosomes[0]), max_repeat(ti for ti, c in zip(t, self.chromosomes[0]) if c==1)
-
-class MyPopulation(StandardPopulation):
-    element_class = MyIndividual
-
-pop = MyPopulation.random(n_individuals=50, size=100)
-pop.evolve()
-print(pop.best_individual)
+    ```
+    t = np.random.randint(1, 5, 100)
+    n = np.random.randint(1, 4, 100)
+
+    import collections
+    def max_repeat(x):
+        # maximum of numbers of repeats
+        c = collections.Counter(x)
+        bm=np.argmax([b for a, b in c.items()])
+        return list(c.keys())[bm]
+
+    class MyIndividual(MonoIndividual):
+
+        element_class = BinaryChromosome
+
+        def _fitness(self):
+            x = self.evaluate()
+            return - x[0] - x[1]
+
+        def evaluate(self):
+            return np.dot(n, self.chromosomes[0]), max_repeat(ti for ti, c in zip(t, self.chromosomes[0]) if c==1)
+
+    class MyPopulation(StandardPopulation):
+        element_class = MyIndividual
+
+    pop = MyPopulation.random(n_individuals=50, size=100)
+    pop.evolve()
+    print(pop.best_individual)
+    ```
 """
 
 from operator import attrgetter
 import typing
 from random import randint, random
 
 from toolz import concat
@@ -226,15 +232,15 @@
         """Decode an individual to a real solution
 
         For example, transform a 0-1 sequence to a real number.
         """
         return [chromosome.decode() for chromosome in self]
 
     def __eq__(self, other):
-        return np.all([c.equal(oc) for c, oc in zip(self, other)])
+        return np.all(list(map(np.equal, self, other)))
 
     def __mul__(self, n):
         """population = individual * n
         
         Args:
             n (TYPE): positive integer
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan  2 04:17:25 2024 UTC, .py size: 348 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 558e 9365 5c01 0000  o.......U..e\...
+00000000: 6f0d 0d0a 0000 0000 8b9f 6d65 5c01 0000  o.........me\...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 0002 0000 0040 0000 0073 1800 0000  .......@...s....
 00000060: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
 00000070: 8400 5a04 6404 5300 2905 da0b 4261 7365  ..Z.d.S.)...Base
@@ -21,25 +21,25 @@
 00000140: 7320 6e65 7665 7220 7573 6564 2c20 6a75  s never used, ju
 00000150: 7374 2061 2074 656d 706c 6174 652e 0a20  st a template.. 
 00000160: 2020 2063 0100 0000 0000 0000 0000 0000     c............
 00000170: 0300 0000 0100 0000 4f00 0000 7304 0000  ........O...s...
 00000180: 0074 0082 0129 014e 2901 da13 4e6f 7449  .t...).N)...NotI
 00000190: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
 000001a0: 03da 0473 656c 66da 0461 7267 73da 066b  ...self..args..k
-000001b0: 7761 7267 73a9 0072 0600 0000 fa50 2f55  wargs..r.....P/U
+000001b0: 7761 7267 73a9 0072 0600 0000 fa4a 2f55  wargs..r.....J/U
 000001c0: 7365 7273 2f77 696c 6c69 616d 2f50 726f  sers/william/Pro
-000001d0: 6772 616d 6d69 6e67 2f6d 7947 6974 6875  gramming/myGithu
-000001e0: 622f 7079 7269 6d69 6469 6e65 2f70 7972  b/pyrimidine/pyr
-000001f0: 696d 6964 696e 652f 6265 6e63 686d 6172  imidine/benchmar
-00000200: 6b73 2f5f 5f69 6e69 745f 5f2e 7079 da08  ks/__init__.py..
-00000210: 5f5f 6361 6c6c 5f5f 0e00 0000 7302 0000  __call__....s...
-00000220: 0004 017a 1442 6173 6550 726f 626c 656d  ...z.BaseProblem
-00000230: 2e5f 5f63 616c 6c5f 5f4e 2905 da08 5f5f  .__call__N)...__
-00000240: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000250: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000260: da07 5f5f 646f 635f 5f72 0800 0000 7206  ..__doc__r....r.
-00000270: 0000 0072 0600 0000 7206 0000 0072 0700  ...r....r....r..
-00000280: 0000 7201 0000 0004 0000 0073 0600 0000  ..r........s....
-00000290: 0800 0401 0c09 7201 0000 004e 2901 7201  ......r....N).r.
-000002a0: 0000 0072 0600 0000 7206 0000 0072 0600  ...r....r....r..
-000002b0: 0000 7207 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002c0: 3e01 0000 0073 0200 0000 1203            >....s......
+000001d0: 6772 616d 6d69 6e67 2f50 7974 686f 6e2f  gramming/Python/
+000001e0: 6d79 776f 726b 2f70 7972 696d 6964 696e  mywork/pyrimidin
+000001f0: 652f 6265 6e63 686d 6172 6b73 2f5f 5f69  e/benchmarks/__i
+00000200: 6e69 745f 5f2e 7079 da08 5f5f 6361 6c6c  nit__.py..__call
+00000210: 5f5f 0e00 0000 7302 0000 0004 017a 1442  __....s......z.B
+00000220: 6173 6550 726f 626c 656d 2e5f 5f63 616c  aseProblem.__cal
+00000230: 6c5f 5f4e 2905 da08 5f5f 6e61 6d65 5f5f  l__N)...__name__
+00000240: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000250: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000260: 635f 5f72 0800 0000 7206 0000 0072 0600  c__r....r....r..
+00000270: 0000 7206 0000 0072 0700 0000 7201 0000  ..r....r....r...
+00000280: 0004 0000 0073 0600 0000 0800 0401 0c09  .....s..........
+00000290: 7201 0000 004e 2901 7201 0000 0072 0600  r....N).r....r..
+000002a0: 0000 7206 0000 0072 0600 0000 7207 0000  ..r....r....r...
+000002b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000002c0: 0200 0000 1203                           ......
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 1006 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 ee03 0000  o.........ne....
+00000000: 6f0d 0d0a 0000 0000 53a3 6d65 ee03 0000  o.......S.me....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6403 6c05 6d06 5a06 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6405 8400 6406 6405 8400 6407 6405 8400  d...d.d...d.d...
 00000060: 6501 6a07 6501 6a08 6501 6a09 6501 6a0a  e.j.e.j.e.j.e.j.
 00000070: 6408 6405 8400 6409 6405 8400 6709 5a0b  d.d...d.d...g.Z.
@@ -10,130 +10,129 @@
 00000090: 4700 640c 640d 8400 640d 6506 8303 5a0f  G.d.d...d.e...Z.
 000000a0: 6401 5300 290e e900 0000 004e e902 0000  d.S.)......N....
 000000b0: 0029 01da 0b42 6173 6550 726f 626c 656d  .)...BaseProblem
 000000c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
 000000d0: 0004 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
 000000e0: a001 7402 7c00 8301 a101 5300 a901 4e29  ..t.|.....S...N)
 000000f0: 03da 026e 70da 046f 6e65 73da 036c 656e  ...np..ones..len
-00000100: a901 da01 78a9 0072 0a00 0000 fa5d 2f55  ....x..r.....]/U
+00000100: a901 da01 78a9 0072 0a00 0000 fa4f 2f55  ....x..r.....O/U
 00000110: 7365 7273 2f77 696c 6c69 616d 2f50 726f  sers/william/Pro
-00000120: 6772 616d 6d69 6e67 2f6d 7947 6974 6875  gramming/myGithu
-00000130: 622f 7079 7269 6d69 6469 6e65 2f64 6f63  b/pyrimidine/doc
-00000140: 732f 2e2e 2f70 7972 696d 6964 696e 652f  s/../pyrimidine/
-00000150: 6265 6e63 686d 6172 6b73 2f61 7070 726f  benchmarks/appro
-00000160: 7869 6d61 7469 6f6e 2e70 79da 083c 6c61  ximation.py..<la
-00000170: 6d62 6461 3e09 0000 0073 0200 0000 0e00  mbda>....s......
-00000180: 720c 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000190: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
-000001a0: 0000 007c 0053 0072 0400 0000 720a 0000  ...|.S.r....r...
-000001b0: 0072 0800 0000 720a 0000 0072 0a00 0000  .r....r....r....
-000001c0: 720b 0000 0072 0c00 0000 0900 0000 7302  r....r........s.
-000001d0: 0000 0004 0063 0100 0000 0000 0000 0000  .....c..........
-000001e0: 0000 0100 0000 0200 0000 4300 0000 7308  ..........C...s.
-000001f0: 0000 007c 0064 0113 0053 0029 024e 7202  ...|.d...S.).Nr.
-00000200: 0000 0072 0a00 0000 7208 0000 0072 0a00  ...r....r....r..
-00000210: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000220: 0009 0000 00f3 0200 0000 0800 6301 0000  ............c...
-00000230: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00000240: 0043 0000 0073 1400 0000 7400 a001 7400  .C...s....t...t.
-00000250: a002 7c00 a101 6401 1700 a101 5300 2902  ..|...d.....S.).
-00000260: 4ee9 0100 0000 2903 7205 0000 00da 036c  N.....).r......l
-00000270: 6f67 da03 6162 7372 0800 0000 720a 0000  og..absr....r...
-00000280: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000290: 0b00 0000 7302 0000 0014 0063 0100 0000  ....s......c....
-000002a0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000002b0: 4300 0000 7308 0000 007c 0064 016b 0453  C...s....|.d.k.S
-000002c0: 0029 024e 7201 0000 0072 0a00 0000 7208  .).Nr....r....r.
-000002d0: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-000002e0: 0000 720c 0000 000b 0000 0072 0d00 0000  ..r........r....
-000002f0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000300: 0005 0000 0003 0000 0073 2200 0000 7400  .........s"...t.
-00000310: 6a01 8700 6601 6401 6402 8408 7402 7c01  j...f.d.d...t.|.
-00000320: 7c02 8302 4400 8301 6403 6404 8d02 5300  |...D...d.d...S.
-00000330: 2905 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000340: 0300 0000 0500 0000 1300 0000 731c 0000  ............s...
-00000350: 0067 007c 005d 0a5c 027d 017d 027c 017c  .g.|.].\.}.}.|.|
-00000360: 0288 0083 0114 0091 0271 0253 0072 0a00  .........q.S.r..
-00000370: 0000 720a 0000 00a9 03da 022e 30da 0163  ..r.........0..c
-00000380: da01 6272 0800 0000 720a 0000 0072 0b00  ..br....r....r..
-00000390: 0000 da0a 3c6c 6973 7463 6f6d 703e 1100  ....<listcomp>..
-000003a0: 0000 7302 0000 001c 007a 1c6c 696e 5f63  ..s......z.lin_c
-000003b0: 6f6d 622e 3c6c 6f63 616c 733e 2e3c 6c69  omb.<locals>.<li
-000003c0: 7374 636f 6d70 3e72 0100 0000 a901 da04  stcomp>r........
-000003d0: 6178 6973 2903 7205 0000 00da 0373 756d  axis).r......sum
-000003e0: da03 7a69 7029 0372 0900 0000 da05 636f  ..zip).r......co
-000003f0: 6566 73da 0562 6173 6973 720a 0000 0072  efs..basisr....r
-00000400: 0800 0000 720b 0000 00da 086c 696e 5f63  ....r......lin_c
-00000410: 6f6d 6210 0000 0073 0200 0000 2201 721c  omb....s....".r.
-00000420: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000430: 0000 0000 0300 0000 4000 0000 7324 0000  ........@...s$..
-00000440: 0065 005a 0164 005a 0264 0164 0265 0366  .e.Z.d.Z.d.d.e.f
-00000450: 0364 0364 0484 015a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-00000460: 0564 0753 0029 08da 1746 756e 6374 696f  .d.S.)...Functio
-00000470: 6e31 4441 7070 726f 7869 6d61 7469 6f6e  n1DApproximation
-00000480: 7201 0000 0072 0e00 0000 6305 0000 0000  r....r....c.....
-00000490: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
-000004a0: 0000 0073 4400 0000 7c01 7c00 5f00 7c02  ...sD...|.|._.|.
-000004b0: 7c00 5f01 7c03 7c00 5f02 7403 a004 7c00  |._.|.|._.t...|.
-000004c0: 6a01 7c00 6a02 6401 a103 7c00 5f05 7c00  j.|.j.d...|._.|.
-000004d0: a000 7c00 6a05 a101 7c00 5f06 6402 7c00  ..|.j...|._.d.|.
-000004e0: 5f07 7c04 7c00 5f08 6400 5300 2903 4ee9  _.|.|._.d.S.).N.
-000004f0: 1e00 0000 720e 0000 0029 09da 0866 756e  ....r....)...fun
-00000500: 6374 696f 6eda 026c 62da 0275 6272 0500  ction..lb..ubr..
-00000510: 0000 da08 6c69 6e73 7061 6365 7209 0000  ....linspacer...
-00000520: 00da 0179 da09 7468 7265 7368 6f6c 6472  ...y..thresholdr
-00000530: 1b00 0000 2905 da04 7365 6c66 721f 0000  ....)...selfr...
-00000540: 0072 2000 0000 7221 0000 0072 1b00 0000  .r ...r!...r....
-00000550: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000560: 085f 5f69 6e69 745f 5f16 0000 0073 0e00  .__init__....s..
-00000570: 0000 0601 0601 0601 1401 0e01 0601 0a01  ................
-00000580: 7a20 4675 6e63 7469 6f6e 3144 4170 7072  z Function1DAppr
-00000590: 6f78 696d 6174 696f 6e2e 5f5f 696e 6974  oximation.__init
-000005a0: 5f5f 6302 0000 0000 0000 0000 0000 0004  __c.............
-000005b0: 0000 0008 0000 0003 0000 0073 6a00 0000  ...........sj...
-000005c0: 7400 6a01 8700 6601 6401 6402 8408 7402  t.j...f.d.d...t.
-000005d0: 7c01 8800 6a03 8302 4400 8301 6403 6404  |...j...D...d.d.
-000005e0: 8d02 7d02 6405 7d03 7400 a004 7400 a005  ..}.d.}.t...t...
-000005f0: 7c02 8800 6a06 1800 7400 a005 8800 6a06  |...j...t.....j.
-00000600: a101 6406 1700 1b00 a101 a101 0b00 7c03  ..d...........|.
-00000610: 7400 a004 7400 a005 7c01 a101 8800 6a07  t...t...|.....j.
-00000620: 6b00 a101 1400 1700 5300 2907 7a2d 413a  k.......S.).z-A:
-00000630: 204e 202a 204b 0a20 2020 2020 2020 2043   N * K.        C
-00000640: 3a20 4b0a 2020 2020 2020 2020 423a 204b  : K.        B: K
-00000650: 2a70 0a20 2020 2020 2020 2063 0100 0000  *p.        c....
-00000660: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000670: 1300 0000 731e 0000 0067 007c 005d 0b5c  ....s....g.|.].\
-00000680: 027d 017d 027c 017c 0288 006a 0083 0114  .}.}.|.|...j....
-00000690: 0091 0271 0253 0072 0a00 0000 7208 0000  ...q.S.r....r...
-000006a0: 0072 1100 0000 a901 7225 0000 0072 0a00  .r......r%...r..
-000006b0: 0000 720b 0000 0072 1500 0000 2500 0000  ..r....r....%...
-000006c0: 7302 0000 001e 007a 3446 756e 6374 696f  s......z4Functio
-000006d0: 6e31 4441 7070 726f 7869 6d61 7469 6f6e  n1DApproximation
-000006e0: 2e5f 5f63 616c 6c5f 5f2e 3c6c 6f63 616c  .__call__.<local
-000006f0: 733e 2e3c 6c69 7374 636f 6d70 3e72 0100  s>.<listcomp>r..
-00000700: 0000 7216 0000 0067 fca9 f1d2 4d62 503f  ..r....g....MbP?
-00000710: 720e 0000 0029 0872 0500 0000 7218 0000  r....).r....r...
-00000720: 0072 1900 0000 721b 0000 00da 046d 6561  .r....r......mea
-00000730: 6e72 1000 0000 7223 0000 0072 2400 0000  nr....r#...r$...
-00000740: 2904 7225 0000 0072 1a00 0000 da02 7979  ).r%...r......yy
-00000750: da01 7072 0a00 0000 7227 0000 0072 0b00  ..pr....r'...r..
-00000760: 0000 da08 5f5f 6361 6c6c 5f5f 1f00 0000  ....__call__....
-00000770: 7306 0000 0024 0604 0142 017a 2046 756e  s....$...B.z Fun
-00000780: 6374 696f 6e31 4441 7070 726f 7869 6d61  ction1DApproxima
-00000790: 7469 6f6e 2e5f 5f63 616c 6c5f 5f4e 2906  tion.__call__N).
-000007a0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000007b0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000007c0: 6d65 5f5f da06 5f62 6173 6973 7226 0000  me__.._basisr&..
-000007d0: 0072 2b00 0000 720a 0000 0072 0a00 0000  .r+...r....r....
-000007e0: 720a 0000 0072 0b00 0000 721d 0000 0014  r....r....r.....
-000007f0: 0000 0073 0600 0000 0800 1002 0c09 721d  ...s..........r.
-00000800: 0000 0029 10da 056e 756d 7079 7205 0000  ...)...numpyr...
-00000810: 00da 0c6e 756d 7079 2e6c 696e 616c 67da  ...numpy.linalg.
-00000820: 066c 696e 616c 67da 024c 41da 0a62 656e  .linalg..LA..ben
-00000830: 6368 6d61 726b 7372 0300 0000 da03 7369  chmarksr......si
-00000840: 6eda 0363 6f73 da03 7461 6eda 0365 7870  n..cos..tan..exp
-00000850: 722f 0000 0072 0700 0000 5a08 6e5f 6261  r/...r....Z.n_ba
-00000860: 7369 735f 721c 0000 0072 1d00 0000 720a  sis_r....r....r.
-00000870: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-00000880: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000890: 7314 0000 0008 030c 010c 0212 020c 0110  s...............
-000008a0: 0104 fe08 0408 0314 04                   .........
+00000120: 6772 616d 6d69 6e67 2f50 7974 686f 6e2f  gramming/Python/
+00000130: 6d79 776f 726b 2f70 7972 696d 6964 696e  mywork/pyrimidin
+00000140: 652f 6265 6e63 686d 6172 6b73 2f61 7070  e/benchmarks/app
+00000150: 726f 7869 6d61 7469 6f6e 2e70 79da 083c  roximation.py..<
+00000160: 6c61 6d62 6461 3e09 0000 0073 0200 0000  lambda>....s....
+00000170: 0e00 720c 0000 0063 0100 0000 0000 0000  ..r....c........
+00000180: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000190: 7304 0000 007c 0053 0072 0400 0000 720a  s....|.S.r....r.
+000001a0: 0000 0072 0800 0000 720a 0000 0072 0a00  ...r....r....r..
+000001b0: 0000 720b 0000 0072 0c00 0000 0900 0000  ..r....r........
+000001c0: 7302 0000 0004 0063 0100 0000 0000 0000  s......c........
+000001d0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000001e0: 7308 0000 007c 0064 0113 0053 0029 024e  s....|.d...S.).N
+000001f0: 7202 0000 0072 0a00 0000 7208 0000 0072  r....r....r....r
+00000200: 0a00 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
+00000210: 0000 0009 0000 00f3 0200 0000 0800 6301  ..............c.
+00000220: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00000230: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
+00000240: 7400 a002 7c00 a101 6401 1700 a101 5300  t...|...d.....S.
+00000250: 2902 4ee9 0100 0000 2903 7205 0000 00da  ).N.....).r.....
+00000260: 036c 6f67 da03 6162 7372 0800 0000 720a  .log..absr....r.
+00000270: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000280: 0000 0b00 0000 7302 0000 0014 0063 0100  ......s......c..
+00000290: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000002a0: 0000 4300 0000 7308 0000 007c 0064 016b  ..C...s....|.d.k
+000002b0: 0453 0029 024e 7201 0000 0072 0a00 0000  .S.).Nr....r....
+000002c0: 7208 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+000002d0: 0b00 0000 720c 0000 000b 0000 0072 0d00  ....r........r..
+000002e0: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+000002f0: 0000 0005 0000 0003 0000 0073 2200 0000  ...........s"...
+00000300: 7400 6a01 8700 6601 6401 6402 8408 7402  t.j...f.d.d...t.
+00000310: 7c01 7c02 8302 4400 8301 6403 6404 8d02  |.|...D...d.d...
+00000320: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000330: 0000 0300 0000 0500 0000 1300 0000 731c  ..............s.
+00000340: 0000 0067 007c 005d 0a5c 027d 017d 027c  ...g.|.].\.}.}.|
+00000350: 017c 0288 0083 0114 0091 0271 0253 0072  .|.........q.S.r
+00000360: 0a00 0000 720a 0000 00a9 03da 022e 30da  ....r.........0.
+00000370: 0163 da01 6272 0800 0000 720a 0000 0072  .c..br....r....r
+00000380: 0b00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+00000390: 1100 0000 7302 0000 001c 007a 1c6c 696e  ....s......z.lin
+000003a0: 5f63 6f6d 622e 3c6c 6f63 616c 733e 2e3c  _comb.<locals>.<
+000003b0: 6c69 7374 636f 6d70 3e72 0100 0000 a901  listcomp>r......
+000003c0: da04 6178 6973 2903 7205 0000 00da 0373  ..axis).r......s
+000003d0: 756d da03 7a69 7029 0372 0900 0000 da05  um..zip).r......
+000003e0: 636f 6566 73da 0562 6173 6973 720a 0000  coefs..basisr...
+000003f0: 0072 0800 0000 720b 0000 00da 086c 696e  .r....r......lin
+00000400: 5f63 6f6d 6210 0000 0073 0200 0000 2201  _comb....s....".
+00000410: 721c 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000420: 0000 0000 0000 0300 0000 4000 0000 7324  ..........@...s$
+00000430: 0000 0065 005a 0164 005a 0264 0164 0265  ...e.Z.d.Z.d.d.e
+00000440: 0366 0364 0364 0484 015a 0464 0564 0684  .f.d.d...Z.d.d..
+00000450: 005a 0564 0753 0029 08da 1746 756e 6374  .Z.d.S.)...Funct
+00000460: 696f 6e31 4441 7070 726f 7869 6d61 7469  ion1DApproximati
+00000470: 6f6e 7201 0000 0072 0e00 0000 6305 0000  onr....r....c...
+00000480: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+00000490: 0043 0000 0073 4400 0000 7c01 7c00 5f00  .C...sD...|.|._.
+000004a0: 7c02 7c00 5f01 7c03 7c00 5f02 7403 a004  |.|._.|.|._.t...
+000004b0: 7c00 6a01 7c00 6a02 6401 a103 7c00 5f05  |.j.|.j.d...|._.
+000004c0: 7c00 a000 7c00 6a05 a101 7c00 5f06 6402  |...|.j...|._.d.
+000004d0: 7c00 5f07 7c04 7c00 5f08 6400 5300 2903  |._.|.|._.d.S.).
+000004e0: 4ee9 1e00 0000 720e 0000 0029 09da 0866  N.....r....)...f
+000004f0: 756e 6374 696f 6eda 026c 62da 0275 6272  unction..lb..ubr
+00000500: 0500 0000 da08 6c69 6e73 7061 6365 7209  ......linspacer.
+00000510: 0000 00da 0179 da09 7468 7265 7368 6f6c  .....y..threshol
+00000520: 6472 1b00 0000 2905 da04 7365 6c66 721f  dr....)...selfr.
+00000530: 0000 0072 2000 0000 7221 0000 0072 1b00  ...r ...r!...r..
+00000540: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000550: 00da 085f 5f69 6e69 745f 5f16 0000 0073  ...__init__....s
+00000560: 0e00 0000 0601 0601 0601 1401 0e01 0601  ................
+00000570: 0a01 7a20 4675 6e63 7469 6f6e 3144 4170  ..z Function1DAp
+00000580: 7072 6f78 696d 6174 696f 6e2e 5f5f 696e  proximation.__in
+00000590: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
+000005a0: 0004 0000 0008 0000 0003 0000 0073 6a00  .............sj.
+000005b0: 0000 7400 6a01 8700 6601 6401 6402 8408  ..t.j...f.d.d...
+000005c0: 7402 7c01 8800 6a03 8302 4400 8301 6403  t.|...j...D...d.
+000005d0: 6404 8d02 7d02 6405 7d03 7400 a004 7400  d...}.d.}.t...t.
+000005e0: a005 7c02 8800 6a06 1800 7400 a005 8800  ..|...j...t.....
+000005f0: 6a06 a101 6406 1700 1b00 a101 a101 0b00  j...d...........
+00000600: 7c03 7400 a004 7400 a005 7c01 a101 8800  |.t...t...|.....
+00000610: 6a07 6b00 a101 1400 1700 5300 2907 7a2d  j.k.......S.).z-
+00000620: 413a 204e 202a 204b 0a20 2020 2020 2020  A: N * K.       
+00000630: 2043 3a20 4b0a 2020 2020 2020 2020 423a   C: K.        B:
+00000640: 204b 2a70 0a20 2020 2020 2020 2063 0100   K*p.        c..
+00000650: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00000660: 0000 1300 0000 731e 0000 0067 007c 005d  ......s....g.|.]
+00000670: 0b5c 027d 017d 027c 017c 0288 006a 0083  .\.}.}.|.|...j..
+00000680: 0114 0091 0271 0253 0072 0a00 0000 7208  .....q.S.r....r.
+00000690: 0000 0072 1100 0000 a901 7225 0000 0072  ...r......r%...r
+000006a0: 0a00 0000 720b 0000 0072 1500 0000 2500  ....r....r....%.
+000006b0: 0000 7302 0000 001e 007a 3446 756e 6374  ..s......z4Funct
+000006c0: 696f 6e31 4441 7070 726f 7869 6d61 7469  ion1DApproximati
+000006d0: 6f6e 2e5f 5f63 616c 6c5f 5f2e 3c6c 6f63  on.__call__.<loc
+000006e0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+000006f0: 0100 0000 7216 0000 0067 fca9 f1d2 4d62  ....r....g....Mb
+00000700: 503f 720e 0000 0029 0872 0500 0000 7218  P?r....).r....r.
+00000710: 0000 0072 1900 0000 721b 0000 00da 046d  ...r....r......m
+00000720: 6561 6e72 1000 0000 7223 0000 0072 2400  eanr....r#...r$.
+00000730: 0000 2904 7225 0000 0072 1a00 0000 da02  ..).r%...r......
+00000740: 7979 da01 7072 0a00 0000 7227 0000 0072  yy..pr....r'...r
+00000750: 0b00 0000 da08 5f5f 6361 6c6c 5f5f 1f00  ......__call__..
+00000760: 0000 7306 0000 0024 0604 0142 017a 2046  ..s....$...B.z F
+00000770: 756e 6374 696f 6e31 4441 7070 726f 7869  unction1DApproxi
+00000780: 6d61 7469 6f6e 2e5f 5f63 616c 6c5f 5f4e  mation.__call__N
+00000790: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000007a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000007b0: 6e61 6d65 5f5f da06 5f62 6173 6973 7226  name__.._basisr&
+000007c0: 0000 0072 2b00 0000 720a 0000 0072 0a00  ...r+...r....r..
+000007d0: 0000 720a 0000 0072 0b00 0000 721d 0000  ..r....r....r...
+000007e0: 0014 0000 0073 0600 0000 0800 1002 0c09  .....s..........
+000007f0: 721d 0000 0029 10da 056e 756d 7079 7205  r....)...numpyr.
+00000800: 0000 00da 0c6e 756d 7079 2e6c 696e 616c  .....numpy.linal
+00000810: 67da 066c 696e 616c 67da 024c 41da 0a62  g..linalg..LA..b
+00000820: 656e 6368 6d61 726b 7372 0300 0000 da03  enchmarksr......
+00000830: 7369 6eda 0363 6f73 da03 7461 6eda 0365  sin..cos..tan..e
+00000840: 7870 722f 0000 0072 0700 0000 5a08 6e5f  xpr/...r....Z.n_
+00000850: 6261 7369 735f 721c 0000 0072 1d00 0000  basis_r....r....
+00000860: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+00000870: 0b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000880: 0000 7314 0000 0008 030c 010c 0212 020c  ..s.............
+00000890: 0110 0104 fe08 0408 0314 04              ...........
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/approximation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/base.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan  2 05:12:43 2024 UTC, .py size: 1676 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,116 @@
-00000000: 6f0d 0d0a 0000 0000 4b9b 9365 8c06 0000  o.......K..e....
+00000000: 6f0d 0d0a 0000 0000 8b9f 6d65 6906 0000  o.........mei...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
+00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6402 6403 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
-00000050: 6404 6405 8400 6405 6506 8303 5a07 6401  d.d...d.e...Z.d.
-00000060: 5300 2906 e900 0000 004e e902 0000 0029  S.)......N.....)
-00000070: 01da 0b42 6173 6550 726f 626c 656d 6300  ...BaseProblemc.
-00000080: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000090: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
-000000a0: 6400 5a02 6401 5a03 640a 6403 6404 8401  d.Z.d.Z.d.d.d...
-000000b0: 5a04 6505 640a 6405 6406 8401 8301 5a06  Z.e.d.d.d.....Z.
-000000c0: 6407 6408 8400 5a07 6409 5300 290b da06  d.d...Z.d.S.)...
-000000d0: 4b4d 6561 6e73 7a55 4b4d 6561 6e73 2063  KMeanszUKMeans c
-000000e0: 6c75 7374 6572 696e 6720 5072 6f62 6c65  lustering Proble
-000000f0: 6d0a 0a20 2020 2045 524d 3a0a 2020 2020  m..    ERM:.    
-00000100: 6d69 6e20 4a28 632c 6d75 2920 3d20 7375  min J(c,mu) = su
-00000110: 6d5f 6320 7375 6d5f 7b78 3a63 7d20 7c7c  m_c sum_{x:c} ||
-00000120: 782d 6d75 5f63 7c7c 0a20 2020 2072 0200  x-mu_c||.    r..
-00000130: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00000140: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
-00000150: 7c01 7c00 5f00 7c02 7c00 5f01 6400 5300  |.|._.|.|._.d.S.
-00000160: 2901 4e29 02da 0158 da0c 6e5f 636f 6d70  ).N)...X..n_comp
-00000170: 6f6e 656e 7473 2903 da04 7365 6c66 7205  onents)...selfr.
-00000180: 0000 0072 0600 0000 a900 7208 0000 00fa  ...r......r.....
-00000190: 572f 5573 6572 732f 7769 6c6c 6961 6d2f  W/Users/william/
-000001a0: 5072 6f67 7261 6d6d 696e 672f 6d79 4769  Programming/myGi
-000001b0: 7468 7562 2f70 7972 696d 6964 696e 652f  thub/pyrimidine/
-000001c0: 646f 6373 2f2e 2e2f 7079 7269 6d69 6469  docs/../pyrimidi
-000001d0: 6e65 2f62 656e 6368 6d61 726b 732f 636c  ne/benchmarks/cl
-000001e0: 7573 7465 722e 7079 da08 5f5f 696e 6974  uster.py..__init
-000001f0: 5f5f 0f00 0000 7304 0000 0006 010a 017a  __....s........z
-00000200: 0f4b 4d65 616e 732e 5f5f 696e 6974 5f5f  .KMeans.__init__
-00000210: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00000220: 0006 0000 0043 0000 0073 4200 0000 7400  .....C...sB...t.
-00000230: 6a01 a002 6401 6401 7c00 7c01 6602 a103  j...d.d.|.|.f...
-00000240: 7d02 7400 6a01 a002 6402 6401 7c00 7c01  }.t.j...d.d.|.|.
-00000250: 6602 a103 7d03 7400 a003 7c02 7c03 6602  f...}.t...|.|.f.
-00000260: a101 7d04 7404 7c04 6402 6403 8d02 5300  ..}.t.|.d.d...S.
-00000270: 2904 4ee9 0100 0000 7202 0000 0029 0172  ).N.....r....).r
-00000280: 0600 0000 2905 da02 6e70 da06 7261 6e64  ....)...np..rand
-00000290: 6f6d da06 6e6f 726d 616c da06 7673 7461  om..normal..vsta
-000002a0: 636b 7204 0000 0029 05da 014e da01 70da  ckr....)...N..p.
-000002b0: 0258 31da 0258 3272 0500 0000 7208 0000  .X1..X2r....r...
-000002c0: 0072 0800 0000 7209 0000 0072 0d00 0000  .r....r....r....
-000002d0: 1300 0000 7308 0000 0014 0214 010e 010c  ....s...........
-000002e0: 017a 0d4b 4d65 616e 732e 7261 6e64 6f6d  .z.KMeans.random
-000002f0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00000300: 0005 0000 0003 0000 0073 3800 0000 7400  .........s8...t.
-00000310: 8801 8301 7d02 8700 8701 6602 6401 6402  ....}.....f.d.d.
-00000320: 8408 7c02 4400 8301 7d03 7401 a002 6403  ..|.D...}.t...d.
-00000330: 6404 8400 7c03 a003 a100 4400 8301 a101  d...|.....D.....
-00000340: 7d04 7c04 5300 2905 4e63 0100 0000 0000  }.|.S.).Nc......
-00000350: 0000 0000 0000 0100 0000 0600 0000 1300  ................
-00000360: 0000 7326 0000 0069 007c 005d 0f89 0088  ..s&...i.|.]....
-00000370: 0087 0087 0166 0264 0064 0184 0874 0088  .....f.d.d...t..
-00000380: 0283 0144 0083 0193 0271 0253 0029 0263  ...D.....q.S.).c
-00000390: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000003a0: 0400 0000 1300 0000 7322 0000 0067 007c  ........s"...g.|
-000003b0: 005d 0d5c 027d 017d 027c 0288 006b 0272  .].\.}.}.|...k.r
-000003c0: 0288 016a 007c 0119 0091 0271 0253 0072  ...j.|.....q.S.r
-000003d0: 0800 0000 2901 7205 0000 0029 03da 022e  ....).r....)....
-000003e0: 30da 0169 da01 6b29 02da 0163 7207 0000  0..i..k)...cr...
-000003f0: 0072 0800 0000 7209 0000 00da 0a3c 6c69  .r....r......<li
-00000400: 7374 636f 6d70 3e1d 0000 0073 0200 0000  stcomp>....s....
-00000410: 2200 7a2e 4b4d 6561 6e73 2e5f 5f63 616c  ".z.KMeans.__cal
-00000420: 6c5f 5f2e 3c6c 6f63 616c 733e 2e3c 6469  l__.<locals>.<di
-00000430: 6374 636f 6d70 3e2e 3c6c 6973 7463 6f6d  ctcomp>.<listcom
-00000440: 703e 2901 da09 656e 756d 6572 6174 6529  p>)...enumerate)
-00000450: 0172 1400 0000 a902 7207 0000 00da 0178  .r......r......x
-00000460: 2901 7217 0000 0072 0900 0000 da0a 3c64  ).r....r......<d
-00000470: 6963 7463 6f6d 703e 1d00 0000 7302 0000  ictcomp>....s...
-00000480: 0026 007a 234b 4d65 616e 732e 5f5f 6361  .&.z#KMeans.__ca
-00000490: 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64  ll__.<locals>.<d
-000004a0: 6963 7463 6f6d 703e 6301 0000 0000 0000  ictcomp>c.......
-000004b0: 0000 0000 0002 0000 0007 0000 0013 0000  ................
-000004c0: 0073 2800 0000 6700 7c00 5d10 5c02 7d01  .s(...g.|.].\.}.
-000004d0: 8900 7400 a001 8700 6601 6400 6401 8408  ..t.....f.d.d...
-000004e0: 8800 4400 8301 a101 9102 7102 5300 2902  ..D.......q.S.).
-000004f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000500: 0009 0000 0013 0000 0073 2400 0000 6700  .........s$...g.
-00000510: 7c00 5d0e 7d01 7400 a001 7c01 7402 6a03  |.].}.t...|.t.j.
-00000520: 8800 6400 6401 8d02 1800 a101 9102 7102  ..d.d.........q.
-00000530: 5300 2902 7201 0000 0029 01da 0461 7869  S.).r....)...axi
-00000540: 7329 04da 024c 41da 046e 6f72 6d72 0c00  s)...LA..normr..
-00000550: 0000 da04 6d65 616e 2902 7214 0000 00da  ....mean).r.....
-00000560: 0278 69a9 0172 1b00 0000 7208 0000 0072  .xi..r....r....r
-00000570: 0900 0000 7218 0000 001e 0000 0073 0200  ....r........s..
-00000580: 0000 2400 7a2e 4b4d 6561 6e73 2e5f 5f63  ..$.z.KMeans.__c
-00000590: 616c 6c5f 5f2e 3c6c 6f63 616c 733e 2e3c  all__.<locals>.<
-000005a0: 6c69 7374 636f 6d70 3e2e 3c6c 6973 7463  listcomp>.<listc
-000005b0: 6f6d 703e 2902 720c 0000 00da 0373 756d  omp>).r......sum
-000005c0: 2902 7214 0000 0072 1700 0000 7208 0000  ).r....r....r...
-000005d0: 0072 2200 0000 7209 0000 0072 1800 0000  .r"...r....r....
-000005e0: 1e00 0000 7302 0000 0028 007a 234b 4d65  ....s....(.z#KMe
-000005f0: 616e 732e 5f5f 6361 6c6c 5f5f 2e3c 6c6f  ans.__call__.<lo
-00000600: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000610: 2904 da03 7365 7472 0c00 0000 7220 0000  )...setr....r ..
-00000620: 00da 0569 7465 6d73 2905 7207 0000 0072  ...items).r....r
-00000630: 1b00 0000 da02 6373 da02 7873 da01 4a72  ......cs..xs..Jr
-00000640: 0800 0000 721a 0000 0072 0900 0000 da08  ....r....r......
-00000650: 5f5f 6361 6c6c 5f5f 1a00 0000 7308 0000  __call__....s...
-00000660: 0008 0214 0118 0104 017a 0f4b 4d65 616e  .........z.KMean
-00000670: 732e 5f5f 6361 6c6c 5f5f 4e29 0172 0200  s.__call__N).r..
-00000680: 0000 2908 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00000690: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000006a0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-000006b0: 5f72 0a00 0000 da0c 7374 6174 6963 6d65  _r......staticme
-000006c0: 7468 6f64 720d 0000 0072 2900 0000 7208  thodr....r)...r.
-000006d0: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-000006e0: 0000 7204 0000 0009 0000 0073 0c00 0000  ..r........s....
-000006f0: 0800 0401 0a05 0204 0c01 0c06 7204 0000  ............r...
-00000700: 0029 08da 056e 756d 7079 720c 0000 00da  .)...numpyr.....
-00000710: 0c6e 756d 7079 2e6c 696e 616c 67da 066c  .numpy.linalg..l
-00000720: 696e 616c 6772 1e00 0000 da09 6265 6e63  inalgr......benc
-00000730: 686d 6172 6b72 0300 0000 7204 0000 0072  hmarkr....r....r
-00000740: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-00000750: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000760: 0073 0800 0000 0803 0c01 0c01 1403       .s............
+00000040: 0100 4700 6402 6403 8400 6403 6505 8303  ..G.d.d...d.e...
+00000050: 5a06 6401 5300 2904 e900 0000 004e 6300  Z.d.S.)......Nc.
+00000060: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000070: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
+00000080: 6400 5a02 6401 5a03 640a 6403 6404 8401  d.Z.d.Z.d.d.d...
+00000090: 5a04 6505 640a 6405 6406 8401 8301 5a06  Z.e.d.d.d.....Z.
+000000a0: 6407 6408 8400 5a07 6409 5300 290b da06  d.d...Z.d.S.)...
+000000b0: 4b4d 6561 6e73 7a55 4b4d 6561 6e73 2063  KMeanszUKMeans c
+000000c0: 6c75 7374 6572 696e 6720 5072 6f62 6c65  lustering Proble
+000000d0: 6d0a 0a20 2020 2045 524d 3a0a 2020 2020  m..    ERM:.    
+000000e0: 6d69 6e20 4a28 632c 6d75 2920 3d20 7375  min J(c,mu) = su
+000000f0: 6d5f 6320 7375 6d5f 7b78 3a63 7d20 7c7c  m_c sum_{x:c} ||
+00000100: 782d 6d75 5f63 7c7c 0a20 2020 20e9 0200  x-mu_c||.    ...
+00000110: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00000120: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
+00000130: 7c01 7c00 5f00 7c02 7c00 5f01 6400 5300  |.|._.|.|._.d.S.
+00000140: 2901 4e29 02da 0158 da0c 6e5f 636f 6d70  ).N)...X..n_comp
+00000150: 6f6e 656e 7473 2903 da04 7365 6c66 7204  onents)...selfr.
+00000160: 0000 0072 0500 0000 a900 7207 0000 00fa  ...r......r.....
+00000170: 492f 5573 6572 732f 7769 6c6c 6961 6d2f  I/Users/william/
+00000180: 5072 6f67 7261 6d6d 696e 672f 5079 7468  Programming/Pyth
+00000190: 6f6e 2f6d 7977 6f72 6b2f 7079 7269 6d69  on/mywork/pyrimi
+000001a0: 6469 6e65 2f62 656e 6368 6d61 726b 732f  dine/benchmarks/
+000001b0: 636c 7573 7465 722e 7079 da08 5f5f 696e  cluster.py..__in
+000001c0: 6974 5f5f 0f00 0000 7304 0000 0006 010a  it__....s.......
+000001d0: 017a 0f4b 4d65 616e 732e 5f5f 696e 6974  .z.KMeans.__init
+000001e0: 5f5f 6302 0000 0000 0000 0000 0000 0005  __c.............
+000001f0: 0000 0006 0000 0043 0000 0073 4200 0000  .......C...sB...
+00000200: 7400 6a01 a002 6401 6401 7c00 7c01 6602  t.j...d.d.|.|.f.
+00000210: a103 7d02 7400 6a01 a002 6402 6401 7c00  ..}.t.j...d.d.|.
+00000220: 7c01 6602 a103 7d03 7400 a003 7c02 7c03  |.f...}.t...|.|.
+00000230: 6602 a101 7d04 7404 7c04 6402 6403 8d02  f...}.t.|.d.d...
+00000240: 5300 2904 4ee9 0100 0000 7203 0000 0029  S.).N.....r....)
+00000250: 0172 0500 0000 2905 da02 6e70 da06 7261  .r....)...np..ra
+00000260: 6e64 6f6d da06 6e6f 726d 616c da06 7673  ndom..normal..vs
+00000270: 7461 636b 7202 0000 0029 05da 014e da01  tackr....)...N..
+00000280: 70da 0258 31da 0258 3272 0400 0000 7207  p..X1..X2r....r.
+00000290: 0000 0072 0700 0000 7208 0000 0072 0c00  ...r....r....r..
+000002a0: 0000 1300 0000 7308 0000 0014 0214 010e  ......s.........
+000002b0: 010c 017a 0d4b 4d65 616e 732e 7261 6e64  ...z.KMeans.rand
+000002c0: 6f6d 6302 0000 0000 0000 0000 0000 0005  omc.............
+000002d0: 0000 0005 0000 0003 0000 0073 3800 0000  ...........s8...
+000002e0: 7400 8801 8301 7d02 8700 8701 6602 6401  t.....}.....f.d.
+000002f0: 6402 8408 7c02 4400 8301 7d03 7401 a002  d...|.D...}.t...
+00000300: 6403 6404 8400 7c03 a003 a100 4400 8301  d.d...|.....D...
+00000310: a101 7d04 7c04 5300 2905 4e63 0100 0000  ..}.|.S.).Nc....
+00000320: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00000330: 1300 0000 7326 0000 0069 007c 005d 0f89  ....s&...i.|.]..
+00000340: 0088 0087 0087 0166 0264 0064 0184 0874  .......f.d.d...t
+00000350: 0088 0283 0144 0083 0193 0271 0253 0029  .....D.....q.S.)
+00000360: 0263 0100 0000 0000 0000 0000 0000 0300  .c..............
+00000370: 0000 0400 0000 1300 0000 7322 0000 0067  ..........s"...g
+00000380: 007c 005d 0d5c 027d 017d 027c 0288 006b  .|.].\.}.}.|...k
+00000390: 0272 0288 016a 007c 0119 0091 0271 0253  .r...j.|.....q.S
+000003a0: 0072 0700 0000 2901 7204 0000 0029 03da  .r....).r....)..
+000003b0: 022e 30da 0169 da01 6b29 02da 0163 7206  ..0..i..k)...cr.
+000003c0: 0000 0072 0700 0000 7208 0000 00da 0a3c  ...r....r......<
+000003d0: 6c69 7374 636f 6d70 3e1d 0000 0073 0200  listcomp>....s..
+000003e0: 0000 2200 7a2e 4b4d 6561 6e73 2e5f 5f63  ..".z.KMeans.__c
+000003f0: 616c 6c5f 5f2e 3c6c 6f63 616c 733e 2e3c  all__.<locals>.<
+00000400: 6469 6374 636f 6d70 3e2e 3c6c 6973 7463  dictcomp>.<listc
+00000410: 6f6d 703e 2901 da09 656e 756d 6572 6174  omp>)...enumerat
+00000420: 6529 0172 1300 0000 a902 7206 0000 00da  e).r......r.....
+00000430: 0178 2901 7216 0000 0072 0800 0000 da0a  .x).r....r......
+00000440: 3c64 6963 7463 6f6d 703e 1d00 0000 7302  <dictcomp>....s.
+00000450: 0000 0026 007a 234b 4d65 616e 732e 5f5f  ...&.z#KMeans.__
+00000460: 6361 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e  call__.<locals>.
+00000470: 3c64 6963 7463 6f6d 703e 6301 0000 0000  <dictcomp>c.....
+00000480: 0000 0000 0000 0002 0000 0007 0000 0013  ................
+00000490: 0000 0073 2800 0000 6700 7c00 5d10 5c02  ...s(...g.|.].\.
+000004a0: 7d01 8900 7400 a001 8700 6601 6400 6401  }...t.....f.d.d.
+000004b0: 8408 8800 4400 8301 a101 9102 7102 5300  ....D.......q.S.
+000004c0: 2902 6301 0000 0000 0000 0000 0000 0002  ).c.............
+000004d0: 0000 0009 0000 0013 0000 0073 2400 0000  ...........s$...
+000004e0: 6700 7c00 5d0e 7d01 7400 a001 7c01 7402  g.|.].}.t...|.t.
+000004f0: 6a03 8800 6400 6401 8d02 1800 a101 9102  j...d.d.........
+00000500: 7102 5300 2902 7201 0000 0029 01da 0461  q.S.).r....)...a
+00000510: 7869 7329 04da 024c 41da 046e 6f72 6d72  xis)...LA..normr
+00000520: 0b00 0000 da04 6d65 616e 2902 7213 0000  ......mean).r...
+00000530: 00da 0278 69a9 0172 1a00 0000 7207 0000  ...xi..r....r...
+00000540: 0072 0800 0000 7217 0000 001e 0000 0073  .r....r........s
+00000550: 0200 0000 2400 7a2e 4b4d 6561 6e73 2e5f  ....$.z.KMeans._
+00000560: 5f63 616c 6c5f 5f2e 3c6c 6f63 616c 733e  _call__.<locals>
+00000570: 2e3c 6c69 7374 636f 6d70 3e2e 3c6c 6973  .<listcomp>.<lis
+00000580: 7463 6f6d 703e 2902 720b 0000 00da 0373  tcomp>).r......s
+00000590: 756d 2902 7213 0000 0072 1600 0000 7207  um).r....r....r.
+000005a0: 0000 0072 2100 0000 7208 0000 0072 1700  ...r!...r....r..
+000005b0: 0000 1e00 0000 7302 0000 0028 007a 234b  ......s....(.z#K
+000005c0: 4d65 616e 732e 5f5f 6361 6c6c 5f5f 2e3c  Means.__call__.<
+000005d0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000005e0: 703e 2904 da03 7365 7472 0b00 0000 721f  p>)...setr....r.
+000005f0: 0000 00da 0569 7465 6d73 2905 7206 0000  .....items).r...
+00000600: 0072 1a00 0000 da02 6373 da02 7873 da01  .r......cs..xs..
+00000610: 4a72 0700 0000 7219 0000 0072 0800 0000  Jr....r....r....
+00000620: da08 5f5f 6361 6c6c 5f5f 1a00 0000 7308  ..__call__....s.
+00000630: 0000 0008 0214 0118 0104 017a 0f4b 4d65  ...........z.KMe
+00000640: 616e 732e 5f5f 6361 6c6c 5f5f 4e29 0172  ans.__call__N).r
+00000650: 0300 0000 2908 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000660: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000670: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000680: 635f 5f72 0900 0000 da0c 7374 6174 6963  c__r......static
+00000690: 6d65 7468 6f64 720c 0000 0072 2800 0000  methodr....r(...
+000006a0: 7207 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
+000006b0: 0800 0000 7202 0000 0009 0000 0073 0c00  ....r........s..
+000006c0: 0000 0800 0401 0a05 0204 0c01 0c06 7202  ..............r.
+000006d0: 0000 0029 07da 056e 756d 7079 720b 0000  ...)...numpyr...
+000006e0: 00da 0c6e 756d 7079 2e6c 696e 616c 67da  ...numpy.linalg.
+000006f0: 066c 696e 616c 6772 1d00 0000 da0b 4261  .linalgr......Ba
+00000700: 7365 5072 6f62 6c65 6d72 0200 0000 7207  seProblemr....r.
+00000710: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
+00000720: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000730: 7306 0000 0008 030c 0114 04              s..........
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/cluster.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 1918 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 7e07 0000  o.........ne~...
+00000000: 6f0d 0d0a 0000 0000 adc2 6d65 2108 0000  o.........me!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6403 6c05 6d06 5a06 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6405 8400 6406 6405 8400 6407 6405 8400  d...d.d...d.d...
 00000060: 6408 6405 8400 6409 6405 8400 6501 6a07  d.d...d.d...e.j.
 00000070: 6501 6a08 6501 6a09 6501 6a0a 640a 6405  e.j.e.j.e.j.d.d.
@@ -16,259 +16,269 @@
 000000f0: 8400 6417 650f 8303 5a16 6401 5300 2918  ..d.e...Z.d.S.).
 00000100: e900 0000 004e e902 0000 0029 01da 0b42  .....N.....)...B
 00000110: 6173 6550 726f 626c 656d 6301 0000 0000  aseProblemc.....
 00000120: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
 00000130: 0000 0073 0e00 0000 7400 a001 7402 7c00  ...s....t...t.|.
 00000140: 8301 a101 5300 a901 4e29 03da 026e 70da  ....S...N)...np.
 00000150: 046f 6e65 73da 036c 656e a901 da01 78a9  .ones..len....x.
-00000160: 0072 0a00 0000 fa57 2f55 7365 7273 2f77  .r.....W/Users/w
+00000160: 0072 0a00 0000 fa49 2f55 7365 7273 2f77  .r.....I/Users/w
 00000170: 696c 6c69 616d 2f50 726f 6772 616d 6d69  illiam/Programmi
-00000180: 6e67 2f6d 7947 6974 6875 622f 7079 7269  ng/myGithub/pyri
-00000190: 6d69 6469 6e65 2f64 6f63 732f 2e2e 2f70  midine/docs/../p
-000001a0: 7972 696d 6964 696e 652f 6265 6e63 686d  yrimidine/benchm
-000001b0: 6172 6b73 2f66 6974 7469 6e67 2e70 79da  arks/fitting.py.
-000001c0: 083c 6c61 6d62 6461 3e09 0000 0073 0200  .<lambda>....s..
-000001d0: 0000 0e00 720c 0000 0063 0100 0000 0000  ....r....c......
-000001e0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-000001f0: 0000 7304 0000 007c 0053 0072 0400 0000  ..s....|.S.r....
-00000200: 720a 0000 0072 0800 0000 720a 0000 0072  r....r....r....r
-00000210: 0a00 0000 720b 0000 0072 0c00 0000 0900  ....r....r......
-00000220: 0000 7302 0000 0004 0063 0100 0000 0000  ..s......c......
-00000230: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000240: 0000 f308 0000 007c 0064 0113 0053 0029  .......|.d...S.)
-00000250: 024e 7202 0000 0072 0a00 0000 7208 0000  .Nr....r....r...
-00000260: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000270: 720c 0000 0009 0000 00f3 0200 0000 0800  r...............
-00000280: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000290: 0002 0000 0043 0000 0072 0d00 0000 2902  .....C...r....).
-000002a0: 4ee9 0300 0000 720a 0000 0072 0800 0000  N.....r....r....
-000002b0: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-000002c0: 0c00 0000 0900 0000 720e 0000 0063 0100  ........r....c..
-000002d0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000002e0: 0000 4300 0000 720d 0000 0029 024e e904  ..C...r....).N..
-000002f0: 0000 0072 0a00 0000 7208 0000 0072 0a00  ...r....r....r..
-00000300: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000310: 0009 0000 0072 0e00 0000 6301 0000 0000  .....r....c.....
-00000320: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000330: 0000 0073 0800 0000 7c00 6401 6b04 5300  ...s....|.d.k.S.
-00000340: a902 4e72 0100 0000 720a 0000 0072 0800  ..Nr....r....r..
-00000350: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000360: 0072 0c00 0000 0a00 0000 720e 0000 0063  .r........r....c
-00000370: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000380: 0200 0000 4300 0000 7308 0000 007c 0064  ....C...s....|.d
-00000390: 016b 0053 0072 1100 0000 720a 0000 0072  .k.S.r....r....r
-000003a0: 0800 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-000003b0: 0000 0072 0c00 0000 0a00 0000 720e 0000  ...r........r...
-000003c0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-000003d0: 0000 0500 0000 4300 0000 7314 0000 0074  ......C...s....t
-000003e0: 00a0 0174 00a0 027c 00a1 0164 0117 00a1  ...t...|...d....
-000003f0: 0153 0029 024e 679a 9999 9999 99b9 3f29  .S.).Ng.......?)
-00000400: 0372 0500 0000 da03 6c6f 67da 0361 6273  .r......log..abs
-00000410: 7208 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000420: 0b00 0000 720c 0000 000b 0000 0073 0200  ....r........s..
-00000430: 0000 1400 6300 0000 0000 0000 0000 0000  ....c...........
-00000440: 0000 0000 0002 0000 0040 0000 0073 2c00  .........@...s,.
-00000450: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-00000460: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
-00000470: 5a05 6407 6408 8400 5a06 6409 5300 290a  Z.d.d...Z.d.S.).
-00000480: da07 4669 7474 696e 6763 0300 0000 0000  ..Fittingc......
-00000490: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-000004a0: 0000 731c 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
-000004b0: 005f 0174 02a0 037c 02a1 017c 005f 0464  ._.t...|...|._.d
-000004c0: 0053 0072 0400 0000 2905 da01 58da 0179  .S.r....)...X..y
-000004d0: da02 4c41 da04 6e6f 726d da01 6e29 03da  ..LA..norm..n)..
-000004e0: 0473 656c 6672 1500 0000 7216 0000 0072  .selfr....r....r
-000004f0: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
-00000500: 5f5f 696e 6974 5f5f 1100 0000 7306 0000  __init__....s...
-00000510: 0006 0106 0110 017a 1046 6974 7469 6e67  .......z.Fitting
-00000520: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-00000530: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-00000540: 0000 7304 0000 0064 0053 0072 0400 0000  ..s....d.S.r....
-00000550: 720a 0000 0029 02da 014e da01 7072 0a00  r....)...N..pr..
-00000560: 0000 720a 0000 0072 0b00 0000 da06 7261  ..r....r......ra
-00000570: 6e64 6f6d 1600 0000 7302 0000 0004 017a  ndom....s......z
-00000580: 0e46 6974 7469 6e67 2e72 616e 646f 6d63  .Fitting.randomc
-00000590: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000005a0: 0400 0000 0700 0000 7320 0000 0074 006a  ........s ...t.j
-000005b0: 0187 0066 0164 0164 0284 0874 027c 018e  ...f.d.d...t.|..
-000005c0: 0044 0083 0164 0364 048d 0253 0029 054e  .D...d.d...S.).N
-000005d0: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-000005e0: 0007 0000 0013 0000 0073 2a00 0000 6700  .........s*...g.
-000005f0: 7c00 5d11 5c03 7d01 7d02 7d03 7c03 7400  |.].\.}.}.}.|.t.
-00000600: a001 7c02 8800 6a02 1400 7c01 1800 a101  ..|...j...|.....
-00000610: 1400 9102 7102 5300 720a 0000 0029 0372  ....q.S.r....).r
-00000620: 0500 0000 da04 7461 6e68 7215 0000 00a9  ......tanhr.....
-00000630: 04da 022e 30da 0161 da01 62da 0163 a901  ....0..a..b..c..
-00000640: 721a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000650: 0a3c 6c69 7374 636f 6d70 3e1a 0000 0073  .<listcomp>....s
-00000660: 0200 0000 2a00 7a1f 4669 7474 696e 672e  ....*.z.Fitting.
-00000670: 6669 742e 3c6c 6f63 616c 733e 2e3c 6c69  fit.<locals>.<li
-00000680: 7374 636f 6d70 3e72 0100 0000 a901 da04  stcomp>r........
-00000690: 6178 6973 2903 7205 0000 00da 0373 756d  axis).r......sum
-000006a0: da03 7a69 70a9 0272 1a00 0000 da06 7061  ..zip..r......pa
-000006b0: 7261 6d73 720a 0000 0072 2500 0000 720b  ramsr....r%...r.
-000006c0: 0000 00da 0366 6974 1900 0000 7302 0000  .....fit....s...
-000006d0: 0020 017a 0b46 6974 7469 6e67 2e66 6974  . .z.Fitting.fit
-000006e0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000006f0: 0004 0000 0047 0000 0073 2400 0000 7c00  .....G...s$...|.
-00000700: 6a00 7c01 8e00 7d02 7401 a002 7c00 6a03  j.|...}.t...|.j.
-00000710: 7c02 1800 6401 a102 0b00 7c00 6a04 1b00  |...d.....|.j...
-00000720: 5300 2902 4ee9 0100 0000 2905 722d 0000  S.).N.....).r-..
-00000730: 0072 1700 0000 7218 0000 0072 1600 0000  .r....r....r....
-00000740: 7219 0000 00a9 0372 1a00 0000 722c 0000  r......r....r,..
-00000750: 00da 0279 7972 0a00 0000 720a 0000 0072  ...yyr....r....r
-00000760: 0b00 0000 da08 5f5f 6361 6c6c 5f5f 1c00  ......__call__..
-00000770: 0000 7304 0000 000a 011a 017a 1046 6974  ..s........z.Fit
-00000780: 7469 6e67 2e5f 5f63 616c 6c5f 5f4e 2907  ting.__call__N).
-00000790: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000007a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000007b0: 6d65 5f5f 721b 0000 0072 1e00 0000 722d  me__r....r....r-
-000007c0: 0000 0072 3100 0000 720a 0000 0072 0a00  ...r1...r....r..
-000007d0: 0000 720a 0000 0072 0b00 0000 7214 0000  ..r....r....r...
-000007e0: 0010 0000 0073 0a00 0000 0800 0801 0805  .....s..........
-000007f0: 0803 0c03 7214 0000 0063 0000 0000 0000  ....r....c......
-00000800: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00000810: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00000820: 0164 0284 005a 0364 0353 0029 04da 0c43  .d...Z.d.S.)...C
-00000830: 7572 7665 4669 7474 696e 6763 0100 0000  urveFittingc....
-00000840: 0000 0000 0000 0000 0200 0000 0900 0000  ................
-00000850: 0700 0000 7356 0000 0074 00a0 0174 006a  ....sV...t...t.j
-00000860: 0287 0066 0164 0164 0284 0874 037c 0164  ...f.d.d...t.|.d
-00000870: 0064 0385 0219 008e 0044 0083 0164 0464  .d.......D...d.d
-00000880: 058d 0274 006a 0287 0066 0164 0664 0284  ...t.j...f.d.d..
-00000890: 0874 037c 0164 0364 0085 0219 008e 0044  .t.|.d.d.......D
-000008a0: 0083 0164 0464 058d 0266 02a1 0153 0029  ...d.d...f...S.)
-000008b0: 074e 6301 0000 0000 0000 0000 0000 0004  .Nc.............
-000008c0: 0000 0006 0000 0013 0000 00f3 2800 0000  ............(...
-000008d0: 6700 7c00 5d10 5c03 7d01 7d02 7d03 7c03  g.|.].\.}.}.}.|.
-000008e0: 7400 7c02 8800 6a01 1400 7c01 1800 8301  t.|...j...|.....
-000008f0: 1400 9102 7102 5300 720a 0000 00a9 025a  ....q.S.r......Z
-00000900: 0472 656c 7572 1500 0000 7220 0000 0072  .relur....r ...r
-00000910: 2500 0000 720a 0000 0072 0b00 0000 7226  %...r....r....r&
-00000920: 0000 0024 0000 00f3 0200 0000 2800 7a24  ...$........(.z$
-00000930: 4375 7276 6546 6974 7469 6e67 2e66 6974  CurveFitting.fit
-00000940: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000950: 6f6d 703e 720f 0000 0072 0100 0000 7227  omp>r....r....r'
-00000960: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000970: 0400 0000 0600 0000 1300 0000 7236 0000  ............r6..
-00000980: 0072 0a00 0000 7237 0000 0072 2000 0000  .r....r7...r ...
-00000990: 7225 0000 0072 0a00 0000 720b 0000 0072  r%...r....r....r
-000009a0: 2600 0000 2500 0000 7238 0000 0029 0472  &...%...r8...).r
-000009b0: 0500 0000 da06 7673 7461 636b 7229 0000  ......vstackr)..
-000009c0: 0072 2a00 0000 722b 0000 0072 0a00 0000  .r*...r+...r....
-000009d0: 7225 0000 0072 0b00 0000 722d 0000 0023  r%...r....r-...#
-000009e0: 0000 0073 0600 0000 2a01 2601 06ff 7a10  ...s....*.&...z.
-000009f0: 4375 7276 6546 6974 7469 6e67 2e66 6974  CurveFitting.fit
-00000a00: 4e29 0472 3200 0000 7233 0000 0072 3400  N).r2...r3...r4.
-00000a10: 0000 722d 0000 0072 0a00 0000 720a 0000  ..r-...r....r...
-00000a20: 0072 0a00 0000 720b 0000 0072 3500 0000  .r....r....r5...
-00000a30: 2100 0000 7304 0000 0008 000c 0272 3500  !...s........r5.
-00000a40: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00000a50: 0000 0004 0000 0043 0000 0073 3200 0000  .......C...s2...
-00000a60: 6401 7c00 0400 0300 6b01 6f09 6402 6b01  d.|.....k.o.d.k.
-00000a70: 6e02 0200 0100 6401 7c01 0400 0300 6b01  n.....d.|.....k.
-00000a80: 6f15 6402 6b01 4000 5300 0200 0100 4000  o.d.k.@.S.....@.
-00000a90: 5300 2903 4e72 0100 0000 e905 0000 0072  S.).Nr.........r
-00000aa0: 0a00 0000 a902 7209 0000 0072 1600 0000  ......r....r....
-00000ab0: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000ac0: 0c00 0000 2800 0000 7302 0000 0032 00a9  ....(...s....2..
-00000ad0: 02da 0363 6f73 da03 7369 6e63 0400 0000  ...cos..sinc....
-00000ae0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000af0: 0300 0000 732e 0000 0074 0064 017c 0014  ....s....t.d.|..
-00000b00: 0083 0189 0174 0164 017c 0014 0083 0189  .....t.d.|......
-00000b10: 0287 0087 0187 0287 0366 0464 0264 0384  .........f.d.d..
-00000b20: 087d 047c 0453 0029 044e 671f 85eb 51b8  .}.|.S.).Ng...Q.
-00000b30: 1e09 4063 0200 0000 0000 0000 0000 0000  ..@c............
-00000b40: 0200 0000 0600 0000 1300 0000 734a 0000  ............sJ..
-00000b50: 0074 00a0 017c 0188 0364 0119 0018 007c  .t...|...d.....|
-00000b60: 0088 0364 0219 0018 00a1 025c 027d 017d  ...d.......\.}.}
-00000b70: 0074 0288 0088 017c 0014 0088 027c 0114  .t.....|.....|..
-00000b80: 0018 0014 0088 0188 027c 0014 0088 017c  .........|.....|
-00000b90: 0114 0017 0014 0083 0253 0029 034e 7201  .........S.).Nr.
-00000ba0: 0000 0072 2e00 0000 2903 7205 0000 00da  ...r....).r.....
-00000bb0: 086d 6573 6867 7269 64da 0a5f 696e 6469  .meshgrid.._indi
-00000bc0: 6361 746f 7272 3b00 0000 a904 7223 0000  catorr;.....r#..
-00000bd0: 0072 2400 0000 da01 73da 0174 720a 0000  .r$.....s..tr...
-00000be0: 0072 0b00 0000 da02 5f66 2f00 0000 7304  .r......_f/...s.
-00000bf0: 0000 0020 012a 017a 1162 6173 6973 2e3c  ... .*.z.basis.<
-00000c00: 6c6f 6361 6c73 3e2e 5f66 723c 0000 0029  locals>._fr<...)
-00000c10: 0572 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00000c20: 7243 0000 0072 4400 0000 720a 0000 0072  rC...rD...r....r
-00000c30: 4100 0000 720b 0000 00da 0562 6173 6973  A...r......basis
-00000c40: 2b00 0000 7308 0000 000c 020c 0112 0104  +...s...........
-00000c50: 0372 4500 0000 2901 da05 496d 6167 6563  .rE...)...Imagec
-00000c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c70: 0300 0000 4000 0000 7326 0000 0065 005a  ....@...s&...e.Z
-00000c80: 0164 005a 0264 0964 0364 0484 015a 0364  .d.Z.d.d.d...Z.d
-00000c90: 0564 0684 005a 0464 0764 0884 005a 0564  .d...Z.d.d...Z.d
-00000ca0: 0153 0029 0ada 0850 6169 6e74 696e 674e  .S.)...PaintingN
-00000cb0: 7201 0000 0063 0500 0000 0000 0000 0000  r....c..........
-00000cc0: 0000 0500 0000 0500 0000 4300 0000 734c  ..........C...sL
-00000cd0: 0000 007c 0270 047c 016a 007c 005f 007c  ...|.p.|.j.|._.|
-00000ce0: 0370 0a7c 016a 017c 005f 0174 02a0 037c  .p.|.j.|._.t...|
-00000cf0: 01a0 047c 006a 00a1 0174 026a 05a1 0264  ...|.j...t.j...d
-00000d00: 0064 0085 0264 0064 0085 027c 0466 0319  .d...d.d...|.f..
-00000d10: 007c 005f 0664 017c 005f 0764 0053 0029  .|._.d.|._.d.S.)
-00000d20: 024e e900 0100 0029 08da 0473 697a 65da  .N.....)...size.
-00000d30: 046d 6f64 6572 0500 0000 da07 6173 6172  .moder......asar
-00000d40: 7261 79da 0672 6573 697a 65da 0666 6c6f  ray..resize..flo
-00000d50: 6174 5f72 1600 0000 7219 0000 0029 0572  at_r....r....).r
-00000d60: 1a00 0000 da05 696d 6167 6572 4900 0000  ......imagerI...
-00000d70: 724a 0000 00da 0763 6861 6e6e 656c 720a  rJ.....channelr.
-00000d80: 0000 0072 0a00 0000 720b 0000 0072 1b00  ...r....r....r..
-00000d90: 0000 3800 0000 7308 0000 000c 020c 012a  ..8...s........*
-00000da0: 010a 017a 1150 6169 6e74 696e 672e 5f5f  ...z.Painting.__
-00000db0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000dc0: 0000 0002 0000 0004 0000 0007 0000 0073  ...............s
-00000dd0: 4200 0000 7400 a001 7c00 6a02 6401 1900  B...t...|.j.d...
-00000de0: a101 8900 7400 a001 7c00 6a02 6402 1900  ....t...|.j.d...
-00000df0: a101 8901 7400 6a03 8700 8701 6602 6403  ....t.j.....f.d.
-00000e00: 6404 8408 7404 7c01 8e00 4400 8301 6401  d...t.|...D...d.
-00000e10: 6405 8d02 5300 2906 4e72 0100 0000 722e  d...S.).Nr....r.
-00000e20: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000e30: 0600 0000 0800 0000 1300 0000 732e 0000  ............s...
-00000e40: 0067 007c 005d 135c 057d 017d 027d 037d  .g.|.].\.}.}.}.}
-00000e50: 047d 057c 0574 007c 017c 027c 037c 0483  .}.|.t.|.|.|.|..
-00000e60: 0488 0088 0183 0214 0091 0271 0253 0072  ...........q.S.r
-00000e70: 0a00 0000 2901 7245 0000 0029 0672 2100  ....).rE...).r!.
-00000e80: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-00000e90: 0072 4300 0000 da01 64a9 02da 026b 73da  .rC.....d....ks.
-00000ea0: 026c 7372 0a00 0000 720b 0000 0072 2600  .lsr....r....r&.
-00000eb0: 0000 4200 0000 7302 0000 002e 007a 2050  ..B...s......z P
-00000ec0: 6169 6e74 696e 672e 6669 742e 3c6c 6f63  ainting.fit.<loc
-00000ed0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-00000ee0: 2700 0000 2905 7205 0000 00da 0661 7261  '...).r......ara
-00000ef0: 6e67 6572 4900 0000 7229 0000 0072 2a00  ngerI...r)...r*.
-00000f00: 0000 722b 0000 0072 0a00 0000 7251 0000  ..r+...r....rQ..
-00000f10: 0072 0b00 0000 722d 0000 003f 0000 0073  .r....r-...?...s
-00000f20: 0600 0000 1001 1001 2201 7a0c 5061 696e  ........".z.Pain
-00000f30: 7469 6e67 2e66 6974 6301 0000 0000 0000  ting.fitc.......
-00000f40: 0000 0000 0003 0000 0005 0000 0047 0000  .............G..
-00000f50: 0073 2200 0000 7c00 6a00 7c01 8e00 7d02  .s"...|.j.|...}.
-00000f60: 7401 a002 7c02 a003 6401 a101 a101 a004  t...|...d.......
-00000f70: 7c00 6a05 a101 5300 2902 4eda 0575 696e  |.j...S.).N..uin
-00000f80: 7438 2906 722d 0000 0072 4600 0000 da09  t8).r-...rF.....
-00000f90: 6672 6f6d 6172 7261 79da 0661 7374 7970  fromarray..astyp
-00000fa0: 65da 0763 6f6e 7665 7274 724a 0000 0072  e..convertrJ...r
-00000fb0: 2f00 0000 720a 0000 0072 0a00 0000 720b  /...r....r....r.
-00000fc0: 0000 00da 0774 6f69 6d61 6765 4400 0000  .....toimageD...
-00000fd0: 7304 0000 000a 0118 017a 1050 6169 6e74  s........z.Paint
-00000fe0: 696e 672e 746f 696d 6167 6529 034e 4e72  ing.toimage).NNr
-00000ff0: 0100 0000 2906 7232 0000 0072 3300 0000  ....).r2...r3...
-00001000: 7234 0000 0072 1b00 0000 722d 0000 0072  r4...r....r-...r
-00001010: 5900 0000 720a 0000 0072 0a00 0000 720a  Y...r....r....r.
-00001020: 0000 0072 0b00 0000 7247 0000 0037 0000  ...r....rG...7..
-00001030: 0073 0800 0000 0800 0a01 0807 0c05 7247  .s............rG
-00001040: 0000 0029 17da 056e 756d 7079 7205 0000  ...)...numpyr...
-00001050: 00da 0c6e 756d 7079 2e6c 696e 616c 67da  ...numpy.linalg.
-00001060: 066c 696e 616c 6772 1700 0000 da0a 6265  .linalgr......be
-00001070: 6e63 686d 6172 6b73 7203 0000 0072 3e00  nchmarksr....r>.
-00001080: 0000 723d 0000 00da 0374 616e 7213 0000  ..r=.....tanr...
-00001090: 00da 0365 7870 da06 5f62 6173 6973 7207  ...exp.._basisr.
-000010a0: 0000 00da 086e 5f62 6173 6973 5f72 1400  .....n_basis_r..
-000010b0: 0000 7235 0000 0072 4000 0000 da04 6d61  ..r5...r@.....ma
-000010c0: 7468 7245 0000 00da 0350 494c 7246 0000  thrE.....PILrF..
-000010d0: 0072 4700 0000 720a 0000 0072 0a00 0000  .rG...r....r....
-000010e0: 720a 0000 0072 0b00 0000 da08 3c6d 6f64  r....r......<mod
-000010f0: 756c 653e 0100 0000 731e 0000 0008 030c  ule>....s.......
-00001100: 010c 021e 021c 010a 0104 fe08 0410 0310  ................
-00001110: 1108 0710 0208 010c 0a14 02              ...........
+00000180: 6e67 2f50 7974 686f 6e2f 6d79 776f 726b  ng/Python/mywork
+00000190: 2f70 7972 696d 6964 696e 652f 6265 6e63  /pyrimidine/benc
+000001a0: 686d 6172 6b73 2f66 6974 7469 6e67 2e70  hmarks/fitting.p
+000001b0: 79da 083c 6c61 6d62 6461 3e09 0000 0073  y..<lambda>....s
+000001c0: 0200 0000 0e00 720c 0000 0063 0100 0000  ......r....c....
+000001d0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000001e0: 4300 0000 7304 0000 007c 0053 0072 0400  C...s....|.S.r..
+000001f0: 0000 720a 0000 0072 0800 0000 720a 0000  ..r....r....r...
+00000200: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000210: 0900 0000 7302 0000 0004 0063 0100 0000  ....s......c....
+00000220: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000230: 4300 0000 f308 0000 007c 0064 0113 0053  C........|.d...S
+00000240: 0029 024e 7202 0000 0072 0a00 0000 7208  .).Nr....r....r.
+00000250: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+00000260: 0000 720c 0000 0009 0000 00f3 0200 0000  ..r.............
+00000270: 0800 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000280: 0000 0002 0000 0043 0000 0072 0d00 0000  .......C...r....
+00000290: 2902 4ee9 0300 0000 720a 0000 0072 0800  ).N.....r....r..
+000002a0: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+000002b0: 0072 0c00 0000 0900 0000 720e 0000 0063  .r........r....c
+000002c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000002d0: 0200 0000 4300 0000 720d 0000 0029 024e  ....C...r....).N
+000002e0: e904 0000 0072 0a00 0000 7208 0000 0072  .....r....r....r
+000002f0: 0a00 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
+00000300: 0000 0009 0000 0072 0e00 0000 6301 0000  .......r....c...
+00000310: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000320: 0043 0000 0073 0800 0000 7c00 6401 6b04  .C...s....|.d.k.
+00000330: 5300 a902 4e72 0100 0000 720a 0000 0072  S...Nr....r....r
+00000340: 0800 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000350: 0000 0072 0c00 0000 0a00 0000 720e 0000  ...r........r...
+00000360: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000370: 0000 0200 0000 4300 0000 7308 0000 007c  ......C...s....|
+00000380: 0064 016b 0053 0072 1100 0000 720a 0000  .d.k.S.r....r...
+00000390: 0072 0800 0000 720a 0000 0072 0a00 0000  .r....r....r....
+000003a0: 720b 0000 0072 0c00 0000 0a00 0000 720e  r....r........r.
+000003b0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000003c0: 0100 0000 0500 0000 4300 0000 7314 0000  ........C...s...
+000003d0: 0074 00a0 0174 00a0 027c 00a1 0164 0117  .t...t...|...d..
+000003e0: 00a1 0153 0029 024e 679a 9999 9999 99b9  ...S.).Ng.......
+000003f0: 3f29 0372 0500 0000 da03 6c6f 67da 0361  ?).r......log..a
+00000400: 6273 7208 0000 0072 0a00 0000 720a 0000  bsr....r....r...
+00000410: 0072 0b00 0000 720c 0000 000b 0000 0073  .r....r........s
+00000420: 0200 0000 1400 6300 0000 0000 0000 0000  ......c.........
+00000430: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00000440: 2c00 0000 6500 5a01 6400 5a02 6401 6402  ,...e.Z.d.Z.d.d.
+00000450: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+00000460: 8400 5a05 6407 6408 8400 5a06 6409 5300  ..Z.d.d...Z.d.S.
+00000470: 290a da07 4669 7474 696e 6763 0300 0000  )...Fittingc....
+00000480: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000490: 4300 0000 731c 0000 007c 017c 005f 007c  C...s....|.|._.|
+000004a0: 027c 005f 0174 02a0 037c 02a1 017c 005f  .|._.t...|...|._
+000004b0: 0464 0053 0072 0400 0000 2905 da01 58da  .d.S.r....)...X.
+000004c0: 0179 da02 4c41 da04 6e6f 726d da01 6e29  .y..LA..norm..n)
+000004d0: 03da 0473 656c 6672 1500 0000 7216 0000  ...selfr....r...
+000004e0: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
+000004f0: da08 5f5f 696e 6974 5f5f 1100 0000 7306  ..__init__....s.
+00000500: 0000 0006 0106 0110 017a 1046 6974 7469  .........z.Fitti
+00000510: 6e67 2e5f 5f69 6e69 745f 5f63 0200 0000  ng.__init__c....
+00000520: 0000 0000 0000 0000 0200 0000 0100 0000  ................
+00000530: 4300 0000 7304 0000 0064 0053 0072 0400  C...s....d.S.r..
+00000540: 0000 720a 0000 0029 02da 014e da01 7072  ..r....)...N..pr
+00000550: 0a00 0000 720a 0000 0072 0b00 0000 da06  ....r....r......
+00000560: 7261 6e64 6f6d 1600 0000 7302 0000 0004  random....s.....
+00000570: 017a 0e46 6974 7469 6e67 2e72 616e 646f  .z.Fitting.rando
+00000580: 6d63 0100 0000 0000 0000 0000 0000 0200  mc..............
+00000590: 0000 0400 0000 0700 0000 7320 0000 0074  ..........s ...t
+000005a0: 006a 0187 0066 0164 0164 0284 0874 027c  .j...f.d.d...t.|
+000005b0: 018e 0044 0083 0164 0364 048d 0253 0029  ...D...d.d...S.)
+000005c0: 054e 6301 0000 0000 0000 0000 0000 0004  .Nc.............
+000005d0: 0000 0007 0000 0013 0000 0073 2a00 0000  ...........s*...
+000005e0: 6700 7c00 5d11 5c03 7d01 7d02 7d03 7c03  g.|.].\.}.}.}.|.
+000005f0: 7400 a001 7c02 8800 6a02 1400 7c01 1800  t...|...j...|...
+00000600: a101 1400 9102 7102 5300 720a 0000 0029  ......q.S.r....)
+00000610: 0372 0500 0000 da04 7461 6e68 7215 0000  .r......tanhr...
+00000620: 00a9 04da 022e 30da 0161 da01 62da 0163  ......0..a..b..c
+00000630: a901 721a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000640: 00da 0a3c 6c69 7374 636f 6d70 3e1a 0000  ...<listcomp>...
+00000650: 0073 0200 0000 2a00 7a1f 4669 7474 696e  .s....*.z.Fittin
+00000660: 672e 6669 742e 3c6c 6f63 616c 733e 2e3c  g.fit.<locals>.<
+00000670: 6c69 7374 636f 6d70 3e72 0100 0000 a901  listcomp>r......
+00000680: da04 6178 6973 2903 7205 0000 00da 0373  ..axis).r......s
+00000690: 756d da03 7a69 70a9 0272 1a00 0000 da06  um..zip..r......
+000006a0: 7061 7261 6d73 720a 0000 0072 2500 0000  paramsr....r%...
+000006b0: 720b 0000 00da 0366 6974 1900 0000 7302  r......fit....s.
+000006c0: 0000 0020 017a 0b46 6974 7469 6e67 2e66  ... .z.Fitting.f
+000006d0: 6974 6301 0000 0000 0000 0000 0000 0003  itc.............
+000006e0: 0000 0004 0000 0047 0000 0073 2400 0000  .......G...s$...
+000006f0: 7c00 6a00 7c01 8e00 7d02 7401 a002 7c00  |.j.|...}.t...|.
+00000700: 6a03 7c02 1800 6401 a102 0b00 7c00 6a04  j.|...d.....|.j.
+00000710: 1b00 5300 2902 4ee9 0100 0000 2905 722d  ..S.).N.....).r-
+00000720: 0000 0072 1700 0000 7218 0000 0072 1600  ...r....r....r..
+00000730: 0000 7219 0000 00a9 0372 1a00 0000 722c  ..r......r....r,
+00000740: 0000 00da 0279 7972 0a00 0000 720a 0000  .....yyr....r...
+00000750: 0072 0b00 0000 da08 5f5f 6361 6c6c 5f5f  .r......__call__
+00000760: 1c00 0000 7304 0000 000a 011a 017a 1046  ....s........z.F
+00000770: 6974 7469 6e67 2e5f 5f63 616c 6c5f 5f4e  itting.__call__N
+00000780: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000790: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000007a0: 6e61 6d65 5f5f 721b 0000 0072 1e00 0000  name__r....r....
+000007b0: 722d 0000 0072 3100 0000 720a 0000 0072  r-...r1...r....r
+000007c0: 0a00 0000 720a 0000 0072 0b00 0000 7214  ....r....r....r.
+000007d0: 0000 0010 0000 0073 0a00 0000 0800 0801  .......s........
+000007e0: 0805 0803 0c03 7214 0000 0063 0000 0000  ......r....c....
+000007f0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00000800: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000810: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
+00000820: 0c43 7572 7665 4669 7474 696e 6763 0100  .CurveFittingc..
+00000830: 0000 0000 0000 0000 0000 0200 0000 0900  ................
+00000840: 0000 0700 0000 7356 0000 0074 00a0 0174  ......sV...t...t
+00000850: 006a 0287 0066 0164 0164 0284 0874 037c  .j...f.d.d...t.|
+00000860: 0164 0064 0385 0219 008e 0044 0083 0164  .d.d.......D...d
+00000870: 0464 058d 0274 006a 0287 0066 0164 0664  .d...t.j...f.d.d
+00000880: 0284 0874 037c 0164 0364 0085 0219 008e  ...t.|.d.d......
+00000890: 0044 0083 0164 0464 058d 0266 02a1 0153  .D...d.d...f...S
+000008a0: 0029 074e 6301 0000 0000 0000 0000 0000  .).Nc...........
+000008b0: 0004 0000 0006 0000 0013 0000 00f3 2800  ..............(.
+000008c0: 0000 6700 7c00 5d10 5c03 7d01 7d02 7d03  ..g.|.].\.}.}.}.
+000008d0: 7c03 7400 7c02 8800 6a01 1400 7c01 1800  |.t.|...j...|...
+000008e0: 8301 1400 9102 7102 5300 720a 0000 00a9  ......q.S.r.....
+000008f0: 025a 0472 656c 7572 1500 0000 7220 0000  .Z.relur....r ..
+00000900: 0072 2500 0000 720a 0000 0072 0b00 0000  .r%...r....r....
+00000910: 7226 0000 0024 0000 00f3 0200 0000 2800  r&...$........(.
+00000920: 7a24 4375 7276 6546 6974 7469 6e67 2e66  z$CurveFitting.f
+00000930: 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  it.<locals>.<lis
+00000940: 7463 6f6d 703e 720f 0000 0072 0100 0000  tcomp>r....r....
+00000950: 7227 0000 0063 0100 0000 0000 0000 0000  r'...c..........
+00000960: 0000 0400 0000 0600 0000 1300 0000 7236  ..............r6
+00000970: 0000 0072 0a00 0000 7237 0000 0072 2000  ...r....r7...r .
+00000980: 0000 7225 0000 0072 0a00 0000 720b 0000  ..r%...r....r...
+00000990: 0072 2600 0000 2500 0000 7238 0000 0029  .r&...%...r8...)
+000009a0: 0472 0500 0000 da06 7673 7461 636b 7229  .r......vstackr)
+000009b0: 0000 0072 2a00 0000 722b 0000 0072 0a00  ...r*...r+...r..
+000009c0: 0000 7225 0000 0072 0b00 0000 722d 0000  ..r%...r....r-..
+000009d0: 0023 0000 0073 0600 0000 2a01 2601 06ff  .#...s....*.&...
+000009e0: 7a10 4375 7276 6546 6974 7469 6e67 2e66  z.CurveFitting.f
+000009f0: 6974 4e29 0472 3200 0000 7233 0000 0072  itN).r2...r3...r
+00000a00: 3400 0000 722d 0000 0072 0a00 0000 720a  4...r-...r....r.
+00000a10: 0000 0072 0a00 0000 720b 0000 0072 3500  ...r....r....r5.
+00000a20: 0000 2100 0000 7304 0000 0008 000c 0272  ..!...s........r
+00000a30: 3500 0000 6302 0000 0000 0000 0000 0000  5...c...........
+00000a40: 0002 0000 0003 0000 0043 0000 0073 2000  .........C...s .
+00000a50: 0000 6401 7c00 6b01 7c00 6402 6b01 1400  ..d.|.k.|.d.k...
+00000a60: 6401 7c01 6b01 1400 7c01 6402 6b01 1400  d.|.k...|.d.k...
+00000a70: 5300 2903 4e72 0100 0000 e905 0000 0072  S.).Nr.........r
+00000a80: 0a00 0000 a902 7209 0000 0072 1600 0000  ......r....r....
+00000a90: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00000aa0: 0c00 0000 2800 0000 7302 0000 0020 00a9  ....(...s.... ..
+00000ab0: 02da 0363 6f73 da03 7369 6e63 0400 0000  ...cos..sinc....
+00000ac0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
+00000ad0: 0300 0000 7330 0000 0074 0064 017c 0014  ....s0...t.d.|..
+00000ae0: 0083 0189 0074 0164 017c 0014 0083 0189  .....t.d.|......
+00000af0: 0387 0087 0187 0287 0387 0466 0564 0264  ...........f.d.d
+00000b00: 0384 087d 047c 0453 0029 047a b362 6173  ...}.|.S.).z.bas
+00000b10: 6973 0a20 2020 200a 2020 2020 4172 6773  is.    .    Args
+00000b20: 3a0a 2020 2020 2020 2020 6120 286e 756d  :.        a (num
+00000b30: 6265 7229 3a20 526f 7461 7469 6f6e 0a20  ber): Rotation. 
+00000b40: 2020 2020 2020 2064 3120 286e 756d 6265         d1 (numbe
+00000b50: 7229 3a20 5363 616c 696e 670a 2020 2020  r): Scaling.    
+00000b60: 2020 2020 6432 2028 6e75 6d62 6572 293a      d2 (number):
+00000b70: 2053 6361 6c69 6e67 0a20 2020 2020 2020   Scaling.       
+00000b80: 2074 2028 6e75 6d62 6572 293a 2054 7261   t (number): Tra
+00000b90: 6e73 6c61 7469 6f6e 0a20 2020 200a 2020  nslation.    .  
+00000ba0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00000bb0: 2020 2066 756e 6374 696f 6e0a 2020 2020     function.    
+00000bc0: 671f 85eb 51b8 1e09 4063 0200 0000 0000  g...Q...@c......
+00000bd0: 0000 0000 0000 0200 0000 0600 0000 1300  ................
+00000be0: 0000 734a 0000 0074 00a0 017c 0188 0464  ..sJ...t...|...d
+00000bf0: 0119 0018 007c 0088 0464 0219 0018 00a1  .....|...d......
+00000c00: 025c 027d 017d 0074 0288 0188 007c 0014  .\.}.}.t.....|..
+00000c10: 0088 037c 0114 0018 0014 0088 0288 037c  ...|...........|
+00000c20: 0014 0088 007c 0114 0017 0014 0083 0253  .....|.........S
+00000c30: 0029 034e 7201 0000 0072 2e00 0000 2903  .).Nr....r....).
+00000c40: 7205 0000 00da 086d 6573 6867 7269 64da  r......meshgrid.
+00000c50: 0a5f 696e 6469 6361 746f 7272 3b00 0000  ._indicatorr;...
+00000c60: a905 7224 0000 00da 0264 31da 0264 32da  ..r$.....d1..d2.
+00000c70: 0173 da01 7472 0a00 0000 720b 0000 00da  .s..tr....r.....
+00000c80: 025f 663b 0000 0073 0400 0000 2001 2a01  ._f;...s.... .*.
+00000c90: 7a11 6261 7369 732e 3c6c 6f63 616c 733e  z.basis.<locals>
+00000ca0: 2e5f 6672 3c00 0000 2905 7222 0000 0072  ._fr<...).r"...r
+00000cb0: 4200 0000 7243 0000 0072 4500 0000 7246  B...rC...rE...rF
+00000cc0: 0000 0072 0a00 0000 7241 0000 0072 0b00  ...r....rA...r..
+00000cd0: 0000 da05 6261 7369 732c 0000 0073 0800  ....basis,...s..
+00000ce0: 0000 0c0d 0c01 1401 0403 7247 0000 0029  ..........rG...)
+00000cf0: 01da 0549 6d61 6765 6300 0000 0000 0000  ...Imagec.......
+00000d00: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000d10: 0073 2600 0000 6500 5a01 6400 5a02 6409  .s&...e.Z.d.Z.d.
+00000d20: 6403 6404 8401 5a03 6405 6406 8400 5a04  d.d...Z.d.d...Z.
+00000d30: 6407 6408 8400 5a05 6401 5300 290a da08  d.d...Z.d.S.)...
+00000d40: 5061 696e 7469 6e67 4e72 0100 0000 6305  PaintingNr....c.
+00000d50: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+00000d60: 0000 0043 0000 0073 4c00 0000 7c02 7004  ...C...sL...|.p.
+00000d70: 7c01 6a00 7c00 5f00 7c03 700a 7c01 6a01  |.j.|._.|.p.|.j.
+00000d80: 7c00 5f01 7402 a003 7c01 a004 7c00 6a00  |._.t...|...|.j.
+00000d90: a101 7402 6a05 a102 6400 6400 8502 6400  ..t.j...d.d...d.
+00000da0: 6400 8502 7c04 6603 1900 7c00 5f06 6401  d...|.f...|._.d.
+00000db0: 7c00 5f07 6400 5300 2902 4ee9 0001 0000  |._.d.S.).N.....
+00000dc0: 2908 da04 7369 7a65 da04 6d6f 6465 7205  )...size..moder.
+00000dd0: 0000 00da 0761 7361 7272 6179 da06 7265  .....asarray..re
+00000de0: 7369 7a65 da06 666c 6f61 745f 7216 0000  size..float_r...
+00000df0: 0072 1900 0000 2905 721a 0000 00da 0569  .r....).r......i
+00000e00: 6d61 6765 724b 0000 0072 4c00 0000 5a07  magerK...rL...Z.
+00000e10: 6368 616e 6e65 6c72 0a00 0000 720a 0000  channelr....r...
+00000e20: 0072 0b00 0000 721b 0000 0045 0000 0073  .r....r....E...s
+00000e30: 0800 0000 0c01 0c01 2a01 0a01 7a11 5061  ........*...z.Pa
+00000e40: 696e 7469 6e67 2e5f 5f69 6e69 745f 5f63  inting.__init__c
+00000e50: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000e60: 0400 0000 0700 0000 7342 0000 0074 00a0  ........sB...t..
+00000e70: 017c 006a 0264 0119 00a1 0189 0074 00a0  .|.j.d.......t..
+00000e80: 017c 006a 0264 0219 00a1 0189 0174 006a  .|.j.d.......t.j
+00000e90: 0387 0087 0166 0264 0364 0484 0874 047c  .....f.d.d...t.|
+00000ea0: 018e 0044 0083 0164 0164 058d 0253 0029  ...D...d.d...S.)
+00000eb0: 064e 7201 0000 0072 2e00 0000 6301 0000  .Nr....r....c...
+00000ec0: 0000 0000 0000 0000 0006 0000 0008 0000  ................
+00000ed0: 0013 0000 0073 2e00 0000 6700 7c00 5d13  .....s....g.|.].
+00000ee0: 5c05 7d01 7d02 7d03 7d04 7d05 7c05 7400  \.}.}.}.}.}.|.t.
+00000ef0: 7c01 7c02 7c03 7c04 8304 8800 8801 8302  |.|.|.|.........
+00000f00: 1400 9102 7102 5300 720a 0000 0029 0172  ....q.S.r....).r
+00000f10: 4700 0000 2906 7221 0000 0072 2200 0000  G...).r!...r"...
+00000f20: 7242 0000 0072 4300 0000 7245 0000 0072  rB...rC...rE...r
+00000f30: 2400 0000 a902 da02 6b73 da02 6c73 720a  $.......ks..lsr.
+00000f40: 0000 0072 0b00 0000 7226 0000 004e 0000  ...r....r&...N..
+00000f50: 0073 0200 0000 2e00 7a20 5061 696e 7469  .s......z Painti
+00000f60: 6e67 2e66 6974 2e3c 6c6f 6361 6c73 3e2e  ng.fit.<locals>.
+00000f70: 3c6c 6973 7463 6f6d 703e 7227 0000 0029  <listcomp>r'...)
+00000f80: 0572 0500 0000 da06 6172 616e 6765 724b  .r......arangerK
+00000f90: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00000fa0: 0000 720a 0000 0072 5100 0000 720b 0000  ..r....rQ...r...
+00000fb0: 0072 2d00 0000 4b00 0000 7306 0000 0010  .r-...K...s.....
+00000fc0: 0110 0122 017a 0c50 6169 6e74 696e 672e  ...".z.Painting.
+00000fd0: 6669 7463 0100 0000 0000 0000 0000 0000  fitc............
+00000fe0: 0300 0000 0500 0000 4700 0000 7322 0000  ........G...s"..
+00000ff0: 007c 006a 007c 018e 007d 0274 01a0 027c  .|.j.|...}.t...|
+00001000: 02a0 0364 01a1 01a1 01a0 047c 006a 05a1  ...d.......|.j..
+00001010: 0153 0029 024e da05 7569 6e74 3829 0672  .S.).N..uint8).r
+00001020: 2d00 0000 7248 0000 005a 0966 726f 6d61  -...rH...Z.froma
+00001030: 7272 6179 da06 6173 7479 7065 da07 636f  rray..astype..co
+00001040: 6e76 6572 7472 4c00 0000 722f 0000 0072  nvertrL...r/...r
+00001050: 0a00 0000 720a 0000 0072 0b00 0000 da07  ....r....r......
+00001060: 746f 696d 6167 6550 0000 0073 0400 0000  toimageP...s....
+00001070: 0a01 1801 7a10 5061 696e 7469 6e67 2e74  ....z.Painting.t
+00001080: 6f69 6d61 6765 2903 4e4e 7201 0000 0029  oimage).NNr....)
+00001090: 0672 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
+000010a0: 721b 0000 0072 2d00 0000 7258 0000 0072  r....r-...rX...r
+000010b0: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000010c0: 0000 0072 4900 0000 4300 0000 7308 0000  ...rI...C...s...
+000010d0: 0008 000a 0208 060c 0572 4900 0000 2917  .........rI...).
+000010e0: da05 6e75 6d70 7972 0500 0000 da0c 6e75  ..numpyr......nu
+000010f0: 6d70 792e 6c69 6e61 6c67 da06 6c69 6e61  mpy.linalg..lina
+00001100: 6c67 7217 0000 00da 0a62 656e 6368 6d61  lgr......benchma
+00001110: 726b 7372 0300 0000 723e 0000 0072 3d00  rksr....r>...r=.
+00001120: 0000 da03 7461 6e72 1300 0000 da03 6578  ....tanr......ex
+00001130: 705a 065f 6261 7369 7372 0700 0000 5a08  pZ._basisr....Z.
+00001140: 6e5f 6261 7369 735f 7214 0000 0072 3500  n_basis_r....r5.
+00001150: 0000 7240 0000 00da 046d 6174 6872 4700  ..r@.....mathrG.
+00001160: 0000 da03 5049 4c72 4800 0000 7249 0000  ....PILrH...rI..
+00001170: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00001180: 720b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001190: 0000 0073 1e00 0000 0803 0c01 0c02 1e02  ...s............
+000011a0: 1c01 0a01 04fe 0804 1003 1011 0807 1002  ................
+000011b0: 0802 0c15 1402                           ......
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/fitting.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 f800 0000  o.........ne....
+00000000: 6f0d 0d0a 0000 0000 8b9f 6d65 f800 0000  o.........me....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6408 6403 6404 8401 5a05 6405 6406  ..d.d.d...Z.d.d.
 00000050: 8400 5a06 6407 5a07 6401 5300 2909 e900  ..Z.d.Z.d.S.)...
 00000060: 0000 004e e79a 9999 9999 99b9 3f63 0400  ...N........?c..
 00000070: 0000 0000 0000 0000 0000 0400 0000 0600  ................
 00000080: 0000 4300 0000 7324 0000 0074 00a0 0174  ..C...s$...t...t
 00000090: 02a0 037c 017c 00a1 027c 0218 00a1 017c  ...|.|...|.....|
 000000a0: 0374 00a0 017c 00a1 0114 0017 0053 0029  .t...|.......S.)
 000000b0: 014e 2904 da02 4c41 da04 6e6f 726d da02  .N)...LA..norm..
 000000c0: 6e70 da03 646f 7429 04da 0158 da01 41da  np..dot)...X..A.
 000000d0: 0142 da05 616c 7068 61a9 0072 0b00 0000  .B..alpha..r....
-000000e0: fa5c 2f55 7365 7273 2f77 696c 6c69 616d  .\/Users/william
-000000f0: 2f50 726f 6772 616d 6d69 6e67 2f6d 7947  /Programming/myG
-00000100: 6974 6875 622f 7079 7269 6d69 6469 6e65  ithub/pyrimidine
-00000110: 2f64 6f63 732f 2e2e 2f70 7972 696d 6964  /docs/../pyrimid
-00000120: 696e 652f 6265 6e63 686d 6172 6b73 2f6c  ine/benchmarks/l
-00000130: 696e 6561 725f 6d6f 6465 6c2e 7079 da03  inear_model.py..
-00000140: 6c73 7107 0000 0073 0200 0000 2401 720d  lsq....s....$.r.
-00000150: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000160: 0100 0000 0500 0000 4300 0000 732c 0000  ........C...s,..
-00000170: 0064 017c 0064 0219 0018 0064 0313 0064  .d.|.d.....d...d
-00000180: 047c 0064 0119 007c 0064 0219 0064 0313  .|.d...|.d...d..
-00000190: 0018 0064 0313 0014 0017 0053 0029 054e  ...d.......S.).N
-000001a0: e901 0000 0072 0100 0000 e902 0000 00e9  .....r..........
-000001b0: 6400 0000 720b 0000 0029 01da 0178 720b  d...r....)...xr.
-000001c0: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
-000001d0: 6c61 6d62 6461 3e0b 0000 0073 0200 0000  lambda>....s....
-000001e0: 2c00 7212 0000 0029 0229 02e9 feff ffff  ,.r....).)......
-000001f0: 720f 0000 0029 02e9 ffff ffff e903 0000  r....)..........
-00000200: 0029 0172 0200 0000 2908 da05 6e75 6d70  .).r....)...nump
-00000210: 7972 0500 0000 da0c 6e75 6d70 792e 6c69  yr......numpy.li
-00000220: 6e61 6c67 da06 6c69 6e61 6c67 7203 0000  nalg..linalgr...
-00000230: 0072 0d00 0000 da03 6675 6eda 0462 6e64  .r......fun..bnd
-00000240: 7372 0b00 0000 720b 0000 0072 0b00 0000  sr....r....r....
-00000250: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000260: 0000 0073 0a00 0000 0802 0c01 0a03 0804  ...s............
-00000270: 0801                                     ..
+000000e0: fa4e 2f55 7365 7273 2f77 696c 6c69 616d  .N/Users/william
+000000f0: 2f50 726f 6772 616d 6d69 6e67 2f50 7974  /Programming/Pyt
+00000100: 686f 6e2f 6d79 776f 726b 2f70 7972 696d  hon/mywork/pyrim
+00000110: 6964 696e 652f 6265 6e63 686d 6172 6b73  idine/benchmarks
+00000120: 2f6c 696e 6561 725f 6d6f 6465 6c2e 7079  /linear_model.py
+00000130: da03 6c73 7107 0000 0073 0200 0000 2401  ..lsq....s....$.
+00000140: 720d 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000150: 0000 0100 0000 0500 0000 4300 0000 732c  ..........C...s,
+00000160: 0000 0064 017c 0064 0219 0018 0064 0313  ...d.|.d.....d..
+00000170: 0064 047c 0064 0119 007c 0064 0219 0064  .d.|.d...|.d...d
+00000180: 0313 0018 0064 0313 0014 0017 0053 0029  .....d.......S.)
+00000190: 054e e901 0000 0072 0100 0000 e902 0000  .N.....r........
+000001a0: 00e9 6400 0000 720b 0000 0029 01da 0178  ..d...r....)...x
+000001b0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+000001c0: 083c 6c61 6d62 6461 3e0b 0000 0073 0200  .<lambda>....s..
+000001d0: 0000 2c00 7212 0000 0029 0229 02e9 feff  ..,.r....).)....
+000001e0: ffff 720f 0000 0029 02e9 ffff ffff e903  ..r....)........
+000001f0: 0000 0029 0172 0200 0000 2908 da05 6e75  ...).r....)...nu
+00000200: 6d70 7972 0500 0000 da0c 6e75 6d70 792e  mpyr......numpy.
+00000210: 6c69 6e61 6c67 da06 6c69 6e61 6c67 7203  linalg..linalgr.
+00000220: 0000 0072 0d00 0000 da03 6675 6eda 0462  ...r......fun..b
+00000230: 6e64 7372 0b00 0000 720b 0000 0072 0b00  ndsr....r....r..
+00000240: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000250: 3e01 0000 0073 0a00 0000 0802 0c01 0a03  >....s..........
+00000260: 0804 0801                                ....
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/linear_model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 703 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 bf02 0000  o.........ne....
+00000000: 6f0d 0d0a 0000 0000 8b9f 6d65 bf02 0000  o.........me....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6403 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6506 8303 5a07 6401  d.d...d.e...Z.d.
 00000060: 5300 2906 e900 0000 004e e902 0000 0029  S.)......N.....)
 00000070: 01da 0b42 6173 6550 726f 626c 656d 6300  ...BaseProblemc.
@@ -12,66 +12,65 @@
 000000b0: 6405 6406 8401 8301 5a05 640b 6408 6409  d.d.....Z.d.d.d.
 000000c0: 8401 5a06 6407 5300 290c da03 4e4d 4663  ..Z.d.S.)...NMFc
 000000d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 000000e0: 0300 0000 4300 0000 7316 0000 007c 017c  ....C...s....|.|
 000000f0: 005f 0074 01a0 027c 01a1 017c 005f 0264  ._.t...|...|._.d
 00000100: 0053 00a9 014e 2903 da01 4dda 024c 41da  .S...N)...M..LA.
 00000110: 046e 6f72 6d29 02da 0473 656c 6672 0600  .norm)...selfr..
-00000120: 0000 a900 720a 0000 00fa 562f 5573 6572  ....r.....V/User
+00000120: 0000 a900 720a 0000 00fa 482f 5573 6572  ....r.....H/User
 00000130: 732f 7769 6c6c 6961 6d2f 5072 6f67 7261  s/william/Progra
-00000140: 6d6d 696e 672f 6d79 4769 7468 7562 2f70  mming/myGithub/p
-00000150: 7972 696d 6964 696e 652f 646f 6373 2f2e  yrimidine/docs/.
-00000160: 2e2f 7079 7269 6d69 6469 6e65 2f62 656e  ./pyrimidine/ben
-00000170: 6368 6d61 726b 732f 6d61 7472 6978 2e70  chmarks/matrix.p
-00000180: 79da 085f 5f69 6e69 745f 5f0c 0000 0073  y..__init__....s
-00000190: 0400 0000 0601 1001 7a0c 4e4d 462e 5f5f  ........z.NMF.__
-000001a0: 696e 6974 5f5f e9f4 0100 00e9 6400 0000  init__......d...
-000001b0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-000001c0: 0006 0000 0043 0000 0073 4a00 0000 7400  .....C...sJ...t.
-000001d0: 6a01 a002 7c00 7c01 a102 6401 1400 7d02  j...|.|...d...}.
-000001e0: 7c02 6a03 6402 6403 8d01 7d03 7404 7c00  |.j.d.d...}.t.|.
-000001f0: 8301 4400 5d0c 7d04 7c02 7c04 0500 1900  ..D.].}.|.|.....
-00000200: 7c03 7c04 1900 1d00 0300 3c00 7113 7405  |.|.......<.q.t.
-00000210: 7c02 6404 8d01 5300 2905 4ee9 0a00 0000  |.d...S.).N.....
-00000220: e901 0000 0029 01da 0461 7869 7329 0172  .....)...axis).r
-00000230: 0600 0000 2906 da02 6e70 da06 7261 6e64  ....)...np..rand
-00000240: 6f6d da04 7261 6e64 da03 7375 6dda 0572  om..rand..sum..r
-00000250: 616e 6765 7204 0000 0029 05da 014e da01  anger....)...N..
-00000260: 7072 0600 0000 da01 73da 016b 720a 0000  pr......s..kr...
-00000270: 0072 0a00 0000 720b 0000 0072 1300 0000  .r....r....r....
-00000280: 1000 0000 730a 0000 0012 020c 010c 0116  ....s...........
-00000290: 010a 017a 0a4e 4d46 2e72 616e 646f 6d4e  ...z.NMF.randomN
-000002a0: 6304 0000 0000 0000 0000 0000 0006 0000  c...............
-000002b0: 0007 0000 0043 0000 0073 6400 0000 7c01  .....C...sd...|.
-000002c0: 6a00 6401 1900 7d04 7c03 6402 7501 7222  j.d...}.|.d.u.r"
-000002d0: 7401 7c04 8301 4400 5d14 7d05 7c01 6402  t.|...D.].}.|.d.
-000002e0: 6402 8502 7c05 6602 1900 7c03 7c05 1900  d...|.f...|.|...
-000002f0: 1400 7c01 6402 6402 8502 7c05 6602 3c00  ..|.d.d...|.f.<.
-00000300: 710d 7402 a003 7c00 6a04 7405 a006 7c01  q.t...|.j.t...|.
-00000310: 7c02 a102 1800 a101 0b00 7c00 6a03 1b00  |.........|.j...
-00000320: 5300 2903 7a2f 413a 204e 202a 204b 0a20  S.).z/A: N * K. 
-00000330: 2020 2020 2020 2043 3a20 4b0a 2020 2020         C: K.    
-00000340: 2020 2020 423a 204b 202a 2070 0a20 2020      B: K * p.   
-00000350: 2020 2020 2072 1000 0000 4e29 07da 0573       r....N)...s
-00000360: 6861 7065 7216 0000 0072 0700 0000 7208  haper....r....r.
-00000370: 0000 0072 0600 0000 7212 0000 00da 0364  ...r....r......d
-00000380: 6f74 2906 7209 0000 00da 0141 da01 42da  ot).r......A..B.
-00000390: 0143 da01 63da 0169 720a 0000 0072 0a00  .C..c..ir....r..
-000003a0: 0000 720b 0000 00da 085f 5f63 616c 6c5f  ..r......__call_
-000003b0: 5f18 0000 0073 0a00 0000 0a05 0801 0c01  _....s..........
-000003c0: 2601 2001 7a0c 4e4d 462e 5f5f 6361 6c6c  &. .z.NMF.__call
-000003d0: 5f5f 2902 720d 0000 0072 0e00 0000 7205  __).r....r....r.
-000003e0: 0000 0029 07da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000003f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000400: 7561 6c6e 616d 655f 5f72 0c00 0000 da0c  ualname__r......
-00000410: 7374 6174 6963 6d65 7468 6f64 7213 0000  staticmethodr...
-00000420: 0072 2200 0000 720a 0000 0072 0a00 0000  .r"...r....r....
-00000430: 720a 0000 0072 0b00 0000 7204 0000 000a  r....r....r.....
-00000440: 0000 0073 0a00 0000 0800 0802 0204 0c01  ...s............
-00000450: 0e07 7204 0000 0029 08da 056e 756d 7079  ..r....)...numpy
-00000460: 7212 0000 00da 0c6e 756d 7079 2e6c 696e  r......numpy.lin
-00000470: 616c 67da 066c 696e 616c 6772 0700 0000  alg..linalgr....
-00000480: da0a 6265 6e63 686d 6172 6b73 7203 0000  ..benchmarksr...
-00000490: 0072 0400 0000 720a 0000 0072 0a00 0000  .r....r....r....
-000004a0: 720a 0000 0072 0b00 0000 da08 3c6d 6f64  r....r......<mod
-000004b0: 756c 653e 0100 0000 7308 0000 0008 030c  ule>....s.......
-000004c0: 010c 0214 03                             .....
+00000140: 6d6d 696e 672f 5079 7468 6f6e 2f6d 7977  mming/Python/myw
+00000150: 6f72 6b2f 7079 7269 6d69 6469 6e65 2f62  ork/pyrimidine/b
+00000160: 656e 6368 6d61 726b 732f 6d61 7472 6978  enchmarks/matrix
+00000170: 2e70 79da 085f 5f69 6e69 745f 5f0c 0000  .py..__init__...
+00000180: 0073 0400 0000 0601 1001 7a0c 4e4d 462e  .s........z.NMF.
+00000190: 5f5f 696e 6974 5f5f e9f4 0100 00e9 6400  __init__......d.
+000001a0: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
+000001b0: 0000 0006 0000 0043 0000 0073 4a00 0000  .......C...sJ...
+000001c0: 7400 6a01 a002 7c00 7c01 a102 6401 1400  t.j...|.|...d...
+000001d0: 7d02 7c02 6a03 6402 6403 8d01 7d03 7404  }.|.j.d.d...}.t.
+000001e0: 7c00 8301 4400 5d0c 7d04 7c02 7c04 0500  |...D.].}.|.|...
+000001f0: 1900 7c03 7c04 1900 1d00 0300 3c00 7113  ..|.|.......<.q.
+00000200: 7405 7c02 6404 8d01 5300 2905 4ee9 0a00  t.|.d...S.).N...
+00000210: 0000 e901 0000 0029 01da 0461 7869 7329  .......)...axis)
+00000220: 0172 0600 0000 2906 da02 6e70 da06 7261  .r....)...np..ra
+00000230: 6e64 6f6d da04 7261 6e64 da03 7375 6dda  ndom..rand..sum.
+00000240: 0572 616e 6765 7204 0000 0029 05da 014e  .ranger....)...N
+00000250: da01 7072 0600 0000 da01 73da 016b 720a  ..pr......s..kr.
+00000260: 0000 0072 0a00 0000 720b 0000 0072 1300  ...r....r....r..
+00000270: 0000 1000 0000 730a 0000 0012 020c 010c  ......s.........
+00000280: 0116 010a 017a 0a4e 4d46 2e72 616e 646f  .....z.NMF.rando
+00000290: 6d4e 6304 0000 0000 0000 0000 0000 0006  mNc.............
+000002a0: 0000 0007 0000 0043 0000 0073 6400 0000  .......C...sd...
+000002b0: 7c01 6a00 6401 1900 7d04 7c03 6402 7501  |.j.d...}.|.d.u.
+000002c0: 7222 7401 7c04 8301 4400 5d14 7d05 7c01  r"t.|...D.].}.|.
+000002d0: 6402 6402 8502 7c05 6602 1900 7c03 7c05  d.d...|.f...|.|.
+000002e0: 1900 1400 7c01 6402 6402 8502 7c05 6602  ....|.d.d...|.f.
+000002f0: 3c00 710d 7402 a003 7c00 6a04 7405 a006  <.q.t...|.j.t...
+00000300: 7c01 7c02 a102 1800 a101 0b00 7c00 6a03  |.|.........|.j.
+00000310: 1b00 5300 2903 7a2f 413a 204e 202a 204b  ..S.).z/A: N * K
+00000320: 0a20 2020 2020 2020 2043 3a20 4b0a 2020  .        C: K.  
+00000330: 2020 2020 2020 423a 204b 202a 2070 0a20        B: K * p. 
+00000340: 2020 2020 2020 2072 1000 0000 4e29 07da         r....N)..
+00000350: 0573 6861 7065 7216 0000 0072 0700 0000  .shaper....r....
+00000360: 7208 0000 0072 0600 0000 7212 0000 00da  r....r....r.....
+00000370: 0364 6f74 2906 7209 0000 00da 0141 da01  .dot).r......A..
+00000380: 42da 0143 da01 63da 0169 720a 0000 0072  B..C..c..ir....r
+00000390: 0a00 0000 720b 0000 00da 085f 5f63 616c  ....r......__cal
+000003a0: 6c5f 5f18 0000 0073 0a00 0000 0a05 0801  l__....s........
+000003b0: 0c01 2601 2001 7a0c 4e4d 462e 5f5f 6361  ..&. .z.NMF.__ca
+000003c0: 6c6c 5f5f 2902 720d 0000 0072 0e00 0000  ll__).r....r....
+000003d0: 7205 0000 0029 07da 085f 5f6e 616d 655f  r....)...__name_
+000003e0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000003f0: 5f71 7561 6c6e 616d 655f 5f72 0c00 0000  _qualname__r....
+00000400: da0c 7374 6174 6963 6d65 7468 6f64 7213  ..staticmethodr.
+00000410: 0000 0072 2200 0000 720a 0000 0072 0a00  ...r"...r....r..
+00000420: 0000 720a 0000 0072 0b00 0000 7204 0000  ..r....r....r...
+00000430: 000a 0000 0073 0a00 0000 0800 0802 0204  .....s..........
+00000440: 0c01 0e07 7204 0000 0029 08da 056e 756d  ....r....)...num
+00000450: 7079 7212 0000 00da 0c6e 756d 7079 2e6c  pyr......numpy.l
+00000460: 696e 616c 67da 066c 696e 616c 6772 0700  inalg..linalgr..
+00000470: 0000 da0a 6265 6e63 686d 6172 6b73 7203  ....benchmarksr.
+00000480: 0000 0072 0400 0000 720a 0000 0072 0a00  ...r....r....r..
+00000490: 0000 720a 0000 0072 0b00 0000 da08 3c6d  ..r....r......<m
+000004a0: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
+000004b0: 030c 010c 0214 03                        .......
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/matrix.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan  2 04:13:08 2024 UTC, .py size: 1597 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-00000000: 6f0d 0d0a 0000 0000 548d 9365 3d06 0000  o.......T..e=...
+00000000: 6f0d 0d0a 0000 0000 a0bd 6d65 3d06 0000  o.........me=...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6402 6403 6c05 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
-00000050: 6404 6c07 6d08 5a08 0100 6508 5a09 6405  d.l.m.Z...e.Z.d.
-00000060: 6406 8400 5a0a 4700 6407 6408 8400 6408  d...Z.G.d.d...d.
-00000070: 6506 8303 5a0b 640d 6409 640a 8401 5a0c  e...Z.d.d.d...Z.
-00000080: 4700 640b 640c 8400 640c 6506 8303 5a0d  G.d.d...d.e...Z.
-00000090: 6401 5300 290e e900 0000 004e e902 0000  d.S.)......N....
+00000040: 0100 6402 6403 6c05 6d06 5a06 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6405 6c07 6d08 5a08 0100 6508 5a09 6406  d.l.m.Z...e.Z.d.
+00000060: 6407 8400 5a0a 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
+00000070: 6506 8303 5a0b 640e 640a 640b 8401 5a0c  e...Z.d.d.d...Z.
+00000080: 4700 640c 640d 8400 640d 6506 8303 5a0d  G.d.d...d.e...Z.
+00000090: 6401 5300 290f e900 0000 004e e902 0000  d.S.)......N....
 000000a0: 0029 01da 0b42 6173 6550 726f 626c 656d  .)...BaseProblem
-000000b0: 2901 da04 6d61 7830 6305 0000 0000 0000  )...max0c.......
-000000c0: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
-000000d0: 0073 4600 0000 7c00 6a00 6401 1900 7d05  .sF...|.j.d...}.
-000000e0: 7401 7402 a003 7c00 7c01 a102 7402 a004  t.t...|.|...t...
-000000f0: 7c02 7c05 6402 6602 a102 1700 8301 7d06  |.|.d.f.......}.
-00000100: 7402 a003 7c06 7c03 a102 7402 a004 7c04  t...|.|...t...|.
-00000110: 7c05 6402 6602 a102 1700 5300 a903 4e72  |.d.f.....S...Nr
-00000120: 0100 0000 e901 0000 00a9 05da 0573 6861  .............sha
-00000130: 7065 da04 7265 6c75 da02 6e70 da03 646f  pe..relu..np..do
-00000140: 74da 0474 696c 6529 07da 0158 da02 4131  t..tile)...X..A1
-00000150: da02 6231 da02 4132 da02 6232 da01 4eda  ..b1..A2..b2..N.
-00000160: 024f 31a9 0072 1400 0000 fa5e 2f55 7365  .O1..r.....^/Use
-00000170: 7273 2f77 696c 6c69 616d 2f50 726f 6772  rs/william/Progr
-00000180: 616d 6d69 6e67 2f6d 7947 6974 6875 622f  amming/myGithub/
-00000190: 7079 7269 6d69 6469 6e65 2f64 6f63 732f  pyrimidine/docs/
-000001a0: 2e2e 2f70 7972 696d 6964 696e 652f 6265  ../pyrimidine/be
-000001b0: 6e63 686d 6172 6b73 2f6e 6575 7261 6c5f  nchmarks/neural_
-000001c0: 6e65 7477 6f72 6b2e 7079 da04 5f6d 6c70  network.py.._mlp
-000001d0: 0d00 0000 7306 0000 000a 0120 011c 0172  ....s...... ...r
-000001e0: 1600 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000001f0: 0000 0000 0004 0000 0040 0000 0073 2e00  .........@...s..
-00000200: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000210: 6403 8400 5a04 6505 640b 6406 6407 8401  d...Z.e.d.d.d...
-00000220: 8301 5a06 6408 6409 8400 5a07 640a 5300  ..Z.d.d...Z.d.S.
-00000230: 290c da03 4d4c 507a 204d 4c50 0a0a 2020  )...MLPz MLP..  
-00000240: 2020 5920 3d20 4132 6628 4131 582b 6231    Y = A2f(A1X+b1
-00000250: 292b 6232 0a20 2020 2063 0300 0000 0000  )+b2.    c......
-00000260: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
-00000270: 0000 f310 0000 007c 017c 005f 007c 027c  .......|.|._.|.|
-00000280: 005f 0164 0053 00a9 014e a902 720d 0000  ._.d.S...N..r...
-00000290: 00da 0159 a903 da04 7365 6c66 720d 0000  ...Y....selfr...
-000002a0: 0072 1b00 0000 7214 0000 0072 1400 0000  .r....r....r....
-000002b0: 7215 0000 00da 085f 5f69 6e69 745f 5f19  r......__init__.
-000002c0: 0000 00f3 0400 0000 0601 0a01 7a0c 4d4c  ............z.ML
-000002d0: 502e 5f5f 696e 6974 5f5f e964 0000 0072  P.__init__.d...r
-000002e0: 0200 0000 6302 0000 0000 0000 0000 0000  ....c...........
-000002f0: 0004 0000 0007 0000 0043 0000 0073 9200  .........C...s..
-00000300: 0000 7400 6a01 6a01 7c00 7c01 6602 6401  ..t.j.j.|.|.f.d.
-00000310: 8d01 7d02 7400 a002 7c02 6400 6400 8502  ..}.t...|.d.d...
-00000320: 6402 6602 1900 a101 7400 a003 7c02 6400  d.f.....t...|.d.
-00000330: 6400 8502 6403 6602 1900 a101 1700 7400  d...d.f.......t.
-00000340: a002 7c02 6400 6400 8502 6402 6602 1900  ..|.d.d...d.f...
-00000350: 6404 1400 a101 1700 7400 a003 7c02 6400  d.......t...|.d.
-00000360: 6400 8502 6403 6602 1900 6404 1400 a101  d...d.f...d.....
-00000370: 7400 a003 7c02 6400 6400 8502 6404 6602  t...|.d.d...d.f.
-00000380: 1900 a101 1400 1700 7d03 7404 7c02 7c03  ........}.t.|.|.
-00000390: 8302 5300 2905 4ea9 01da 0473 697a 6572  ..S.).N....sizer
-000003a0: 0100 0000 7206 0000 0072 0200 0000 2905  ....r....r....).
-000003b0: 720a 0000 00da 0672 616e 646f 6dda 0373  r......random..s
-000003c0: 696e da03 636f 7372 1700 0000 2904 7212  in..cosr....).r.
-000003d0: 0000 00da 0170 720d 0000 0072 1b00 0000  .....pr....r....
-000003e0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-000003f0: 2300 0000 1d00 0000 7306 0000 0012 0276  #.......s......v
-00000400: 010a 017a 0a4d 4c50 2e72 616e 646f 6d63  ...z.MLP.randomc
-00000410: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000420: 0500 0000 4300 0000 7330 0000 0074 00a0  ....C...s0...t..
-00000430: 0174 027c 006a 0367 017c 01a2 0152 008e  .t.|.j.g.|...R..
-00000440: 007c 006a 0418 00a1 0174 00a0 017c 006a  .|.j.....t...|.j
-00000450: 04a1 011b 007d 027c 020b 0053 0072 1900  .....}.|...S.r..
-00000460: 0000 2905 da02 4c41 da04 6e6f 726d 7216  ..)...LA..normr.
-00000470: 0000 0072 0d00 0000 721b 0000 0029 0372  ...r....r....).r
-00000480: 1d00 0000 da01 78da 0145 7214 0000 0072  ......x..Er....r
-00000490: 1400 0000 7215 0000 00da 085f 5f63 616c  ....r......__cal
-000004a0: 6c5f 5f24 0000 0073 0400 0000 2a01 0601  l__$...s....*...
-000004b0: 7a0c 4d4c 502e 5f5f 6361 6c6c 5f5f 4ea9  z.MLP.__call__N.
-000004c0: 0272 2000 0000 7202 0000 00a9 08da 085f  .r ...r........_
-000004d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000004e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000004f0: 5fda 075f 5f64 6f63 5f5f 721e 0000 00da  _..__doc__r.....
-00000500: 0c73 7461 7469 636d 6574 686f 6472 2300  .staticmethodr#.
-00000510: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
-00000520: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
-00000530: 1300 0000 730c 0000 0008 0004 0108 0502  ....s...........
-00000540: 040c 010c 0672 1700 0000 630a 0000 0000  .....r....c.....
-00000550: 0000 0000 0000 000d 0000 0007 0000 0043  ...............C
-00000560: 0000 0073 8600 0000 7c00 6a00 6401 1900  ...s....|.j.d...
-00000570: 7d0a 7c09 6401 6b02 720c 6402 7d0b 6e05  }.|.d.k.r.d.}.n.
-00000580: 7c09 6a00 6401 1900 7d0b 7401 7402 a003  |.j.d...}.t.t...
-00000590: 7c00 7c01 a102 7402 a004 7c02 7c0a 6402  |.|...t...|.|.d.
-000005a0: 6602 a102 1700 7402 a003 7c05 7c09 a102  f.....t...|.|...
-000005b0: 1700 8301 7d0c 7402 a003 7c0c 7c03 a102  ....}.t...|.|...
-000005c0: 7402 a004 7c04 7c0a 6402 6602 a102 1700  t...|.|.d.f.....
-000005d0: 7402 a003 7c0c 7c07 a102 7402 a004 7c08  t...|.|...t...|.
-000005e0: 7c0b 6402 6602 a102 1700 6602 5300 7205  |.d.f.....f.S.r.
-000005f0: 0000 0072 0700 0000 290d 720d 0000 0072  ...r....).r....r
-00000600: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-00000610: 0000 00da 0243 31da 0263 31da 0243 32da  .....C1..c1..C2.
-00000620: 0263 32da 015a 7212 0000 00da 0148 7213  .c2..Zr......Hr.
-00000630: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00000640: 0000 da04 5f72 6e6e 2900 0000 730c 0000  ...._rnn)...s...
-00000650: 000a 0108 0106 010a 022c 0138 0172 3900  .........,.8.r9.
-00000660: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000670: 0000 0004 0000 0040 0000 0073 3000 0000  .......@...s0...
-00000680: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
-00000690: 8400 5a04 6505 640c 6406 6407 8401 8301  ..Z.e.d.d.d.....
-000006a0: 5a06 640d 6409 640a 8401 5a07 640b 5300  Z.d.d.d...Z.d.S.
-000006b0: 290e da03 524e 4e7a 4852 4e4e 0a0a 2020  )...RNNzHRNN..  
-000006c0: 2020 5974 2b31 203d 2041 3266 2841 3158    Yt+1 = A2f(A1X
-000006d0: 742b 4331 5a74 2b62 3129 2b62 320a 2020  t+C1Zt+b1)+b2.  
-000006e0: 2020 5a74 2b31 203d 2043 3267 2841 3158    Zt+1 = C2g(A1X
-000006f0: 2b43 315a 742b 6231 292b 6332 0a20 2020  +C1Zt+b1)+c2.   
-00000700: 2063 0300 0000 0000 0000 0000 0000 0300   c..............
-00000710: 0000 0200 0000 4300 0000 7218 0000 0072  ......C...r....r
-00000720: 1900 0000 721a 0000 0072 1c00 0000 7214  ....r....r....r.
-00000730: 0000 0072 1400 0000 7215 0000 0072 1e00  ...r....r....r..
-00000740: 0000 3a00 0000 721f 0000 007a 0c52 4e4e  ..:...r....z.RNN
-00000750: 2e5f 5f69 6e69 745f 5f72 2000 0000 7202  .__init__r ...r.
-00000760: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000770: 0300 0000 0300 0000 4300 0000 731c 0000  ........C...s...
-00000780: 0074 006a 016a 017c 007c 0166 0264 018d  .t.j.j.|.|.f.d..
-00000790: 017d 0274 027c 0274 0383 0253 0029 024e  .}.t.|.t...S.).N
-000007a0: 7221 0000 0029 0472 0a00 0000 7223 0000  r!...).r....r#..
-000007b0: 0072 1700 0000 721b 0000 0029 0372 1200  .r....r....).r..
-000007c0: 0000 7226 0000 0072 0d00 0000 7214 0000  ..r&...r....r...
-000007d0: 0072 1400 0000 7215 0000 0072 2300 0000  .r....r....r#...
-000007e0: 3e00 0000 7304 0000 0012 020a 017a 0a52  >...s........z.R
-000007f0: 4e4e 2e72 616e 646f 6d72 0600 0000 6303  NN.randomr....c.
-00000800: 0000 0000 0000 0000 0000 0008 0000 000c  ................
-00000810: 0000 0043 0000 0073 7400 0000 6401 7d03  ...C...st...d.}.
-00000820: 6700 7d04 7c01 6400 7c02 0b00 8502 1900  g.}.|.d.|.......
-00000830: 4400 5d16 7d05 7400 7c05 7401 7402 7403  D.].}.t.|.t.t.t.
-00000840: 7404 7405 7406 7407 7408 7c03 830a 5c02  t.t.t.t.t.|...\.
-00000850: 7d06 7d03 7c04 a009 7c06 a101 0100 710b  }.}.|...|.....q.
-00000860: 740a a00b 740c 7c00 6a0d 6701 7c05 a201  t...t.|.j.g.|...
-00000870: 5200 8e00 7c00 6a0e 1800 a101 740a a00b  R...|.j.....t...
-00000880: 7c00 6a0e a101 1b00 7d07 7c07 0b00 5300  |.j.....}.|...S.
-00000890: 2902 4e72 0100 0000 290f 7239 0000 0072  ).Nr....).r9...r
-000008a0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-000008b0: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
-000008c0: 0000 7236 0000 00da 0661 7070 656e 6472  ..r6.....appendr
-000008d0: 2700 0000 7228 0000 0072 1600 0000 720d  '...r(...r....r.
-000008e0: 0000 0072 1b00 0000 2908 721d 0000 00da  ...r....).r.....
-000008f0: 0278 73da 0168 7237 0000 00da 0258 7372  .xs..hr7.....Xsr
-00000900: 2900 0000 720d 0000 0072 2a00 0000 7214  )...r....r*...r.
-00000910: 0000 0072 1400 0000 7215 0000 0072 2b00  ...r....r....r+.
-00000920: 0000 4300 0000 730e 0000 0004 0104 0112  ..C...s.........
-00000930: 011e 010c 012a 0106 017a 0c52 4e4e 2e5f  .....*...z.RNN._
-00000940: 5f63 616c 6c5f 5f4e 722c 0000 0029 0172  _call__Nr,...).r
-00000950: 0600 0000 722d 0000 0072 1400 0000 7214  ....r-...r....r.
-00000960: 0000 0072 1400 0000 7215 0000 0072 3a00  ...r....r....r:.
-00000970: 0000 3300 0000 730c 0000 0008 0004 0108  ..3...s.........
-00000980: 0602 040c 010e 0472 3a00 0000 2901 7201  .......r:...).r.
-00000990: 0000 0029 0eda 056e 756d 7079 720a 0000  ...)...numpyr...
-000009a0: 00da 0c6e 756d 7079 2e6c 696e 616c 67da  ...numpy.linalg.
-000009b0: 066c 696e 616c 6772 2700 0000 da0a 6265  .linalgr'.....be
-000009c0: 6e63 686d 6172 6b73 7203 0000 00da 0575  nchmarksr......u
-000009d0: 7469 6c73 7204 0000 0072 0900 0000 7216  tilsr....r....r.
-000009e0: 0000 0072 1700 0000 7239 0000 0072 3a00  ...r....r9...r:.
-000009f0: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00000a00: 0072 1500 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000a10: 0100 0000 7312 0000 0008 020c 010c 020c  ....s...........
-00000a20: 0204 0308 0210 060a 1614 0a              ...........
+000000b0: e901 0000 0029 01da 046d 6178 3063 0500  .....)...max0c..
+000000c0: 0000 0000 0000 0000 0000 0700 0000 0700  ................
+000000d0: 0000 4300 0000 7346 0000 007c 006a 0064  ..C...sF...|.j.d
+000000e0: 0119 007d 0574 0174 02a0 037c 007c 01a1  ...}.t.t...|.|..
+000000f0: 0274 02a0 047c 027c 0564 0266 02a1 0217  .t...|.|.d.f....
+00000100: 0083 017d 0674 02a0 037c 067c 03a1 0274  ...}.t...|.|...t
+00000110: 02a0 047c 047c 0564 0266 02a1 0217 0053  ...|.|.d.f.....S
+00000120: 00a9 034e 7201 0000 0072 0400 0000 a905  ...Nr....r......
+00000130: da05 7368 6170 65da 0472 656c 75da 026e  ..shape..relu..n
+00000140: 70da 0364 6f74 da04 7469 6c65 2907 da01  p..dot..tile)...
+00000150: 58da 0241 31da 0262 31da 0241 32da 0262  X..A1..b1..A2..b
+00000160: 32da 014e da02 4f31 a900 7214 0000 00fa  2..N..O1..r.....
+00000170: 502f 5573 6572 732f 7769 6c6c 6961 6d2f  P/Users/william/
+00000180: 5072 6f67 7261 6d6d 696e 672f 5079 7468  Programming/Pyth
+00000190: 6f6e 2f6d 7977 6f72 6b2f 7079 7269 6d69  on/mywork/pyrimi
+000001a0: 6469 6e65 2f62 656e 6368 6d61 726b 732f  dine/benchmarks/
+000001b0: 6e65 7572 616c 5f6e 6574 776f 726b 2e70  neural_network.p
+000001c0: 79da 045f 6d6c 700e 0000 0073 0600 0000  y.._mlp....s....
+000001d0: 0a01 2001 1c01 7216 0000 0063 0000 0000  .. ...r....c....
+000001e0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000001f0: 4000 0000 732e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000200: 0264 015a 0364 0264 0384 005a 0465 0564  .d.Z.d.d...Z.e.d
+00000210: 0b64 0664 0784 0183 015a 0664 0864 0984  .d.d.....Z.d.d..
+00000220: 005a 0764 0a53 0029 0cda 034d 4c50 7a20  .Z.d.S.)...MLPz 
+00000230: 4d4c 500a 0a20 2020 2059 203d 2041 3266  MLP..    Y = A2f
+00000240: 2841 3158 2b62 3129 2b62 320a 2020 2020  (A1X+b1)+b2.    
+00000250: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00000260: 0002 0000 0043 0000 00f3 1000 0000 7c01  .....C........|.
+00000270: 7c00 5f00 7c02 7c00 5f01 6400 5300 a901  |._.|.|._.d.S...
+00000280: 4ea9 0272 0d00 0000 da01 59a9 03da 0473  N..r......Y....s
+00000290: 656c 6672 0d00 0000 721b 0000 0072 1400  elfr....r....r..
+000002a0: 0000 7214 0000 0072 1500 0000 da08 5f5f  ..r....r......__
+000002b0: 696e 6974 5f5f 1a00 0000 f304 0000 0006  init__..........
+000002c0: 010a 017a 0c4d 4c50 2e5f 5f69 6e69 745f  ...z.MLP.__init_
+000002d0: 5fe9 6400 0000 7202 0000 0063 0200 0000  _.d...r....c....
+000002e0: 0000 0000 0000 0000 0400 0000 0700 0000  ................
+000002f0: 4300 0000 7392 0000 0074 006a 016a 017c  C...s....t.j.j.|
+00000300: 007c 0166 0264 018d 017d 0274 00a0 027c  .|.f.d...}.t...|
+00000310: 0264 0064 0085 0264 0266 0219 00a1 0174  .d.d...d.f.....t
+00000320: 00a0 037c 0264 0064 0085 0264 0366 0219  ...|.d.d...d.f..
+00000330: 00a1 0117 0074 00a0 027c 0264 0064 0085  .....t...|.d.d..
+00000340: 0264 0266 0219 0064 0414 00a1 0117 0074  .d.f...d.......t
+00000350: 00a0 037c 0264 0064 0085 0264 0366 0219  ...|.d.d...d.f..
+00000360: 0064 0414 00a1 0174 00a0 037c 0264 0064  .d.....t...|.d.d
+00000370: 0085 0264 0466 0219 00a1 0114 0017 007d  ...d.f.........}
+00000380: 0374 047c 027c 0383 0253 0029 054e a901  .t.|.|...S.).N..
+00000390: da04 7369 7a65 7201 0000 0072 0400 0000  ..sizer....r....
+000003a0: 7202 0000 0029 0572 0a00 0000 da06 7261  r....).r......ra
+000003b0: 6e64 6f6d da03 7369 6eda 0363 6f73 7217  ndom..sin..cosr.
+000003c0: 0000 0029 0472 1200 0000 da01 7072 0d00  ...).r......pr..
+000003d0: 0000 721b 0000 0072 1400 0000 7214 0000  ..r....r....r...
+000003e0: 0072 1500 0000 7223 0000 001e 0000 0073  .r....r#.......s
+000003f0: 0600 0000 1202 7601 0a01 7a0a 4d4c 502e  ......v...z.MLP.
+00000400: 7261 6e64 6f6d 6302 0000 0000 0000 0000  randomc.........
+00000410: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+00000420: 3000 0000 7400 a001 7402 7c00 6a03 6701  0...t...t.|.j.g.
+00000430: 7c01 a201 5200 8e00 7c00 6a04 1800 a101  |...R...|.j.....
+00000440: 7400 a001 7c00 6a04 a101 1b00 7d02 7c02  t...|.j.....}.|.
+00000450: 0b00 5300 7219 0000 0029 05da 024c 41da  ..S.r....)...LA.
+00000460: 046e 6f72 6d72 1600 0000 720d 0000 0072  .normr....r....r
+00000470: 1b00 0000 2903 721d 0000 00da 0178 da01  ....).r......x..
+00000480: 4572 1400 0000 7214 0000 0072 1500 0000  Er....r....r....
+00000490: da08 5f5f 6361 6c6c 5f5f 2500 0000 7304  ..__call__%...s.
+000004a0: 0000 002a 0106 017a 0c4d 4c50 2e5f 5f63  ...*...z.MLP.__c
+000004b0: 616c 6c5f 5f4e a902 7220 0000 0072 0200  all__N..r ...r..
+000004c0: 0000 a908 da08 5f5f 6e61 6d65 5f5f da0a  ......__name__..
+000004d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000004e0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+000004f0: 5f72 1e00 0000 da0c 7374 6174 6963 6d65  _r......staticme
+00000500: 7468 6f64 7223 0000 0072 2b00 0000 7214  thodr#...r+...r.
+00000510: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00000520: 0000 7217 0000 0014 0000 0073 0c00 0000  ..r........s....
+00000530: 0800 0401 0805 0204 0c01 0c06 7217 0000  ............r...
+00000540: 0063 0a00 0000 0000 0000 0000 0000 0d00  .c..............
+00000550: 0000 0700 0000 4300 0000 7386 0000 007c  ......C...s....|
+00000560: 006a 0064 0119 007d 0a7c 0964 016b 0272  .j.d...}.|.d.k.r
+00000570: 0c64 027d 0b6e 057c 096a 0064 0119 007d  .d.}.n.|.j.d...}
+00000580: 0b74 0174 02a0 037c 007c 01a1 0274 02a0  .t.t...|.|...t..
+00000590: 047c 027c 0a64 0266 02a1 0217 0074 02a0  .|.|.d.f.....t..
+000005a0: 037c 057c 09a1 0217 0083 017d 0c74 02a0  .|.|.......}.t..
+000005b0: 037c 0c7c 03a1 0274 02a0 047c 047c 0a64  .|.|...t...|.|.d
+000005c0: 0266 02a1 0217 0074 02a0 037c 0c7c 07a1  .f.....t...|.|..
+000005d0: 0274 02a0 047c 087c 0b64 0266 02a1 0217  .t...|.|.d.f....
+000005e0: 0066 0253 0072 0600 0000 7207 0000 0029  .f.S.r....r....)
+000005f0: 0d72 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000600: 7210 0000 0072 1100 0000 da02 4331 da02  r....r......C1..
+00000610: 6331 da02 4332 da02 6332 da01 5a72 1200  c1..C2..c2..Zr..
+00000620: 0000 da01 4872 1300 0000 7214 0000 0072  ....Hr....r....r
+00000630: 1400 0000 7215 0000 00da 045f 726e 6e2a  ....r......_rnn*
+00000640: 0000 0073 0c00 0000 0a01 0801 0601 0a02  ...s............
+00000650: 2c01 3801 7239 0000 0063 0000 0000 0000  ,.8.r9...c......
+00000660: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000670: 0000 7330 0000 0065 005a 0164 005a 0264  ..s0...e.Z.d.Z.d
+00000680: 015a 0364 0264 0384 005a 0465 0564 0c64  .Z.d.d...Z.e.d.d
+00000690: 0664 0784 0183 015a 0664 0d64 0964 0a84  .d.....Z.d.d.d..
+000006a0: 015a 0764 0b53 0029 0eda 0352 4e4e 7a48  .Z.d.S.)...RNNzH
+000006b0: 524e 4e0a 0a20 2020 2059 742b 3120 3d20  RNN..    Yt+1 = 
+000006c0: 4132 6628 4131 5874 2b43 315a 742b 6231  A2f(A1Xt+C1Zt+b1
+000006d0: 292b 6232 0a20 2020 205a 742b 3120 3d20  )+b2.    Zt+1 = 
+000006e0: 4332 6728 4131 582b 4331 5a74 2b62 3129  C2g(A1X+C1Zt+b1)
+000006f0: 2b63 320a 2020 2020 6303 0000 0000 0000  +c2.    c.......
+00000700: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+00000710: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000720: 721c 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000730: 1500 0000 721e 0000 003b 0000 0072 1f00  ....r....;...r..
+00000740: 0000 7a0c 524e 4e2e 5f5f 696e 6974 5f5f  ..z.RNN.__init__
+00000750: 7220 0000 0072 0200 0000 6302 0000 0000  r ...r....c.....
+00000760: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
+00000770: 0000 0073 1c00 0000 7400 6a01 6a01 7c00  ...s....t.j.j.|.
+00000780: 7c01 6602 6401 8d01 7d02 7402 7c02 7403  |.f.d...}.t.|.t.
+00000790: 8302 5300 2902 4e72 2100 0000 2904 720a  ..S.).Nr!...).r.
+000007a0: 0000 0072 2300 0000 7217 0000 0072 1b00  ...r#...r....r..
+000007b0: 0000 2903 7212 0000 0072 2600 0000 720d  ..).r....r&...r.
+000007c0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+000007d0: 0000 7223 0000 003f 0000 0073 0400 0000  ..r#...?...s....
+000007e0: 1202 0a01 7a0a 524e 4e2e 7261 6e64 6f6d  ....z.RNN.random
+000007f0: 7204 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00000800: 0000 0800 0000 0c00 0000 4300 0000 7374  ..........C...st
+00000810: 0000 0064 017d 0367 007d 047c 0164 007c  ...d.}.g.}.|.d.|
+00000820: 020b 0085 0219 0044 005d 167d 0574 007c  .......D.].}.t.|
+00000830: 0574 0174 0274 0374 0474 0574 0674 0774  .t.t.t.t.t.t.t.t
+00000840: 087c 0383 0a5c 027d 067d 037c 04a0 097c  .|...\.}.}.|...|
+00000850: 06a1 0101 0071 0b74 0aa0 0b74 0c7c 006a  .....q.t...t.|.j
+00000860: 0d67 017c 05a2 0152 008e 007c 006a 0e18  .g.|...R...|.j..
+00000870: 00a1 0174 0aa0 0b7c 006a 0ea1 011b 007d  ...t...|.j.....}
+00000880: 077c 070b 0053 0029 024e 7201 0000 0029  .|...S.).Nr....)
+00000890: 0f72 3900 0000 720e 0000 0072 0f00 0000  .r9...r....r....
+000008a0: 7210 0000 0072 1100 0000 7233 0000 0072  r....r....r3...r
+000008b0: 3400 0000 7235 0000 0072 3600 0000 da06  4...r5...r6.....
+000008c0: 6170 7065 6e64 7227 0000 0072 2800 0000  appendr'...r(...
+000008d0: 7216 0000 0072 0d00 0000 721b 0000 0029  r....r....r....)
+000008e0: 0872 1d00 0000 da02 7873 da01 6872 3700  .r......xs..hr7.
+000008f0: 0000 da02 5873 7229 0000 0072 0d00 0000  ....Xsr)...r....
+00000900: 722a 0000 0072 1400 0000 7214 0000 0072  r*...r....r....r
+00000910: 1500 0000 722b 0000 0044 0000 0073 0e00  ....r+...D...s..
+00000920: 0000 0401 0401 1201 1e01 0c01 2a01 0601  ............*...
+00000930: 7a0c 524e 4e2e 5f5f 6361 6c6c 5f5f 4e72  z.RNN.__call__Nr
+00000940: 2c00 0000 2901 7204 0000 0072 2d00 0000  ,...).r....r-...
+00000950: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000960: 1500 0000 723a 0000 0034 0000 0073 0c00  ....r:...4...s..
+00000970: 0000 0800 0401 0806 0204 0c01 0e04 723a  ..............r:
+00000980: 0000 0029 0172 0100 0000 290e da05 6e75  ...).r....)...nu
+00000990: 6d70 7972 0a00 0000 da0c 6e75 6d70 792e  mpyr......numpy.
+000009a0: 6c69 6e61 6c67 da06 6c69 6e61 6c67 7227  linalg..linalgr'
+000009b0: 0000 00da 0a62 656e 6368 6d61 726b 7372  .....benchmarksr
+000009c0: 0300 0000 da05 7574 696c 7372 0500 0000  ......utilsr....
+000009d0: 7209 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+000009e0: 3900 0000 723a 0000 0072 1400 0000 7214  9...r:...r....r.
+000009f0: 0000 0072 1400 0000 7215 0000 00da 083c  ...r....r......<
+00000a00: 6d6f 6475 6c65 3e01 0000 0073 1200 0000  module>....s....
+00000a10: 0802 0c01 0c02 0c02 0403 0803 1006 0a16  ................
+00000a20: 140a                                     ..
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/neural_network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 6169 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 1918 0000  o.........ne....
+00000000: 6f0d 0d0a 0000 0000 4f1b 8965 1918 0000  o.......O..e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6505 8303 5a06 4700  d.d...d.e...Z.G.
 00000060: 6407 6408 8400 6408 6505 8303 5a07 4700  d.d...d.e...Z.G.
 00000070: 6409 640a 8400 640a 6505 8303 5a08 4700  d.d...d.e...Z.G.
@@ -65,597 +65,596 @@
 00000400: 6e61 6c74 7920 2864 6566 6175 6c74 3a20  nalty (default: 
 00000410: 7b31 3030 7d29 0a20 2020 2020 2020 20e9  {100}).        .
 00000420: 0100 0000 4e29 07da 026e 70da 0373 756d  ....N)...np..sum
 00000430: da01 77da 0163 da01 57da 014d da11 5f4b  ..w..c..W..M.._K
 00000440: 6e61 7073 6163 6b5f 5f73 6f72 7465 6429  napsack__sorted)
 00000450: 05da 0473 656c 6672 0b00 0000 720c 0000  ...selfr....r...
 00000460: 0072 0d00 0000 720e 0000 00a9 0072 1100  .r....r......r..
-00000470: 0000 fa54 2f55 7365 7273 2f77 696c 6c69  ...T/Users/willi
-00000480: 616d 2f50 726f 6772 616d 6d69 6e67 2f6d  am/Programming/m
-00000490: 7947 6974 6875 622f 7079 7269 6d69 6469  yGithub/pyrimidi
-000004a0: 6e65 2f70 7972 696d 6964 696e 652f 6265  ne/pyrimidine/be
-000004b0: 6e63 686d 6172 6b73 2f6f 7074 696d 697a  nchmarks/optimiz
-000004c0: 6174 696f 6e2e 7079 da08 5f5f 696e 6974  ation.py..__init
-000004d0: 5f5f 1100 0000 730e 0000 0008 0c0e 0106  __....s.........
-000004e0: 0206 0106 0106 010a 017a 114b 6e61 7073  .........z.Knaps
-000004f0: 6163 6b2e 5f5f 696e 6974 5f5f 6301 0000  ack.__init__c...
-00000500: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000510: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00000520: 8301 5300 a901 4e29 02da 036c 656e 720c  ..S...N)...lenr.
-00000530: 0000 00a9 0172 1000 0000 7211 0000 0072  .....r....r....r
-00000540: 1100 0000 7212 0000 00da 066e 5f62 6167  ....r......n_bag
-00000550: 7326 0000 0073 0200 0000 0a02 7a0f 4b6e  s&...s......z.Kn
-00000560: 6170 7361 636b 2e6e 5f62 6167 73e9 3200  apsack.n_bags.2.
-00000570: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
-00000580: 0000 0005 0000 0043 0000 0073 2e00 0000  .......C...s....
-00000590: 7400 6a01 a002 6401 6402 7c00 a103 7d02  t.j...d.d.|...}.
-000005a0: 7400 6a01 a002 6401 6402 7c00 a103 7d03  t.j...d.d.|...}.
-000005b0: 7403 7c02 7c03 7c01 6403 8d03 5300 2904  t.|.|.|.d...S.).
-000005c0: 4e72 0800 0000 e915 0000 00a9 0172 0d00  Nr...........r..
-000005d0: 0000 2904 7209 0000 00da 0672 616e 646f  ..).r......rando
-000005e0: 6dda 0772 616e 6469 6e74 7205 0000 0029  m..randintr....)
-000005f0: 0472 1700 0000 720d 0000 0072 0b00 0000  .r....r....r....
-00000600: 720c 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000610: 1200 0000 721b 0000 002a 0000 0073 0600  ....r....*...s..
-00000620: 0000 1002 1001 0e01 7a0f 4b6e 6170 7361  ........z.Knapsa
-00000630: 636b 2e72 616e 646f 6d63 0100 0000 0000  ck.randomc......
-00000640: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000650: 0000 731e 0000 0067 0064 01a2 017d 0167  ..s....g.d...}.g
-00000660: 0064 02a2 017d 0274 007c 017c 027c 0064  .d...}.t.|.|.|.d
-00000670: 038d 0353 0029 044e 2915 e947 0000 00e9  ...S.).N)..G....
-00000680: 2200 0000 e952 0000 00e9 1700 0000 7208  "....R........r.
-00000690: 0000 00e9 5800 0000 e90c 0000 00e9 3900  ....X.........9.
-000006a0: 0000 e90a 0000 00e9 4400 0000 e905 0000  ........D.......
-000006b0: 00e9 2100 0000 e925 0000 00e9 4500 0000  ..!....%....E...
-000006c0: e962 0000 00e9 1800 0000 e91a 0000 00e9  .b..............
-000006d0: 5300 0000 e910 0000 0072 2c00 0000 e908  S........r,.....
-000006e0: 0000 0029 1572 2c00 0000 e93b 0000 00e9  ...).r,....;....
-000006f0: 1e00 0000 e913 0000 00e9 4200 0000 e955  ..........B....U
-00000700: 0000 00e9 5e00 0000 722f 0000 00e9 0300  ....^...r/......
-00000710: 0000 e92c 0000 0072 2600 0000 7208 0000  ...,...r&...r...
-00000720: 00e9 2900 0000 721f 0000 00e9 4c00 0000  ..)...r.....L...
-00000730: 7208 0000 0072 2200 0000 e951 0000 00e9  r....r"....Q....
-00000740: 4900 0000 e920 0000 0072 3600 0000 721a  I.... ...r6...r.
-00000750: 0000 0029 0172 0500 0000 2903 720d 0000  ...).r....).r...
-00000760: 0072 0b00 0000 720c 0000 0072 1100 0000  .r....r....r....
-00000770: 7211 0000 0072 1200 0000 da07 6578 616d  r....r......exam
-00000780: 706c 6530 0000 0073 0600 0000 0802 0801  ple0...s........
-00000790: 0e01 7a10 4b6e 6170 7361 636b 2e65 7861  ..z.Knapsack.exa
-000007a0: 6d70 6c65 6301 0000 0000 0000 0000 0000  mplec...........
-000007b0: 0001 0000 0004 0000 0043 0000 0073 1200  .........C...s..
-000007c0: 0000 7400 a001 7c00 6a02 7c00 6a03 1b00  ..t...|.j.|.j...
-000007d0: a101 5300 7214 0000 0029 0472 0900 0000  ..S.r....).r....
-000007e0: da07 6172 6773 6f72 7472 0c00 0000 720b  ..argsortr....r.
-000007f0: 0000 0072 1600 0000 7211 0000 0072 1100  ...r....r....r..
-00000800: 0000 7212 0000 0072 3e00 0000 3600 0000  ..r....r>...6...
-00000810: 7302 0000 0012 017a 104b 6e61 7073 6163  s......z.Knapsac
-00000820: 6b2e 6172 6773 6f72 7463 0100 0000 0000  k.argsortc......
-00000830: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000840: 0000 731a 0000 007c 006a 0064 0075 0072  ..s....|.j.d.u.r
-00000850: 0a7c 00a0 01a1 007c 005f 007c 006a 0053  .|.....|._.|.j.S
-00000860: 0072 1400 0000 2902 720f 0000 0072 3e00  .r....).r....r>.
-00000870: 0000 7216 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00000880: 0072 1200 0000 da06 736f 7274 6564 3900  .r......sorted9.
-00000890: 0000 7306 0000 000a 020a 0106 027a 0f4b  ..s..........z.K
-000008a0: 6e61 7073 6163 6b2e 736f 7274 6564 6302  napsack.sortedc.
-000008b0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
-000008c0: 0000 0043 0000 0073 7400 0000 7c00 6a00  ...C...st...|.j.
-000008d0: 7c00 6a01 7c00 6a02 7c00 6a03 6604 5c04  |.j.|.j.|.j.f.\.
-000008e0: 7d02 7d03 7d04 7d05 7404 a005 6401 6402  }.}.}.}.t...d.d.
-000008f0: 8400 7406 7c01 7c02 8302 4400 8301 a101  ..t.|.|...D.....
-00000900: 7d06 7404 a005 6403 6402 8400 7406 7c01  }.t...d.d...t.|.
-00000910: 7c03 8302 4400 8301 a101 7d03 7c03 7c04  |...D.....}.|.|.
-00000920: 6b01 722e 7c06 5300 6404 6405 7404 a007  k.r.|.S.d.d.t...
-00000930: 7c06 0b00 a101 1700 1b00 7c05 1400 5300  |.........|...S.
-00000940: 2906 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00000950: 0300 0000 0400 0000 5300 0000 f31c 0000  ........S.......
-00000960: 0067 007c 005d 0a5c 027d 017d 027c 0164  .g.|.].\.}.}.|.d
-00000970: 006b 0272 027c 0291 0271 0253 00a9 0172  .k.r.|...q.S...r
-00000980: 0800 0000 7211 0000 0029 03da 022e 30da  ....r....)....0.
-00000990: 0169 da02 6369 7211 0000 0072 1100 0000  .i..cir....r....
-000009a0: 7212 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-000009b0: 3e43 0000 00f3 0200 0000 1c00 7a25 4b6e  >C..........z%Kn
-000009c0: 6170 7361 636b 2e5f 5f63 616c 6c5f 5f2e  apsack.__call__.
-000009d0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000009e0: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-000009f0: 0300 0000 0400 0000 5300 0000 7240 0000  ........S...r@..
-00000a00: 0072 4100 0000 7211 0000 0029 0372 4200  .rA...r....).rB.
-00000a10: 0000 7243 0000 00da 0277 6972 1100 0000  ..rC.....wir....
-00000a20: 7211 0000 0072 1200 0000 7245 0000 0044  r....r....rE...D
-00000a30: 0000 0072 4600 0000 e9ff ffff ff72 0800  ...rF........r..
-00000a40: 0000 2908 720c 0000 0072 0b00 0000 720d  ..).r....r....r.
-00000a50: 0000 0072 0e00 0000 7209 0000 0072 0a00  ...r....r....r..
-00000a60: 0000 da03 7a69 70da 0365 7870 a907 7210  ....zip..exp..r.
-00000a70: 0000 00da 0178 720c 0000 0072 0b00 0000  .....xr....r....
-00000a80: 720d 0000 0072 0e00 0000 da01 7672 1100  r....r......vr..
-00000a90: 0000 7211 0000 0072 1200 0000 da08 5f5f  ..r....r......__
-00000aa0: 6361 6c6c 5f5f 4000 0000 730c 0000 001c  call__@...s.....
-00000ab0: 021a 011a 0108 0104 0118 027a 114b 6e61  ...........z.Kna
-00000ac0: 7073 6163 6b2e 5f5f 6361 6c6c 5f5f 4ea9  psack.__call__N.
-00000ad0: 0272 0600 0000 7207 0000 0029 0272 1800  .r....r....).r..
-00000ae0: 0000 7206 0000 0029 0172 0600 0000 290d  ..r....).r....).
-00000af0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000b00: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000b10: 6d65 5f5f da07 5f5f 646f 635f 5f72 1300  me__..__doc__r..
-00000b20: 0000 da08 7072 6f70 6572 7479 7217 0000  ....propertyr...
-00000b30: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
-00000b40: 1b00 0000 723d 0000 0072 3e00 0000 723f  ....r=...r>...r?
-00000b50: 0000 0072 4e00 0000 7211 0000 0072 1100  ...rN...r....r..
-00000b60: 0000 7211 0000 0072 1200 0000 7205 0000  ..r....r....r...
-00000b70: 0009 0000 0073 1a00 0000 0800 0401 0a07  .....s..........
-00000b80: 0215 0a01 0203 0c01 0205 0c01 0805 0203  ................
-00000b90: 0a01 0c06 7205 0000 0063 0000 0000 0000  ....r....c......
-00000ba0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000bb0: 0000 7338 0000 0065 005a 0164 005a 0264  ..s8...e.Z.d.Z.d
-00000bc0: 015a 0364 0e64 0464 0584 015a 0465 0564  .Z.d.d.d...Z.e.d
-00000bd0: 0f64 0764 0884 0183 015a 0664 0964 0a84  .d.d.....Z.d.d..
-00000be0: 005a 0764 0b64 0c84 005a 0864 0d53 0029  .Z.d.d...Z.d.S.)
-00000bf0: 10da 0d4d 756c 7469 4b6e 6170 7361 636b  ...MultiKnapsack
-00000c00: 7a9f 4d75 6c74 6920 4368 6f69 6365 204b  z.Multi Choice K
-00000c10: 6e61 7073 6163 6b20 5072 6f62 6c65 6d0a  napsack Problem.
-00000c20: 0a20 2020 206d 6178 2073 756d 5f69 6a20  .    max sum_ij 
-00000c30: 6369 6a20 7869 6a0a 2020 2020 732e 742e  cij xij.    s.t.
-00000c40: 2073 756d 5f69 6a20 7769 6a20 7869 6a20   sum_ij wij xij 
-00000c50: 3c3d 2057 0a20 2020 207b 7869 6a7d 2069  <= W.    {xij} i
-00000c60: 7320 0a20 2020 2077 6865 7265 2078 696a  s .    where xij
-00000c70: 2069 7320 7468 6520 6368 6f69 6365 2076   is the choice v
-00000c80: 6172 6961 626c 652c 2074 6861 7420 6973  ariable, that is
-00000c90: 2073 756d 5f6a 2078 696a 3d31 0a20 2020   sum_j xij=1.   
-00000ca0: 2072 0600 0000 7207 0000 0063 0500 0000   r....r....c....
-00000cb0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000cc0: 4300 0000 734e 0000 007c 0364 016b 0072  C...sN...|.d.k.r
-00000cd0: 0e74 0074 0174 026a 007c 0183 0283 017c  .t.t.t.j.|.....|
-00000ce0: 0314 007d 037c 017c 005f 037c 027c 005f  ...}.|.|._.|.|._
-00000cf0: 047c 037c 005f 057c 047c 005f 0664 027c  .|.|._.|.|._.d.|
-00000d00: 005f 0774 0874 0174 097c 0283 0283 017c  ._.t.t.t.|.....|
-00000d10: 005f 0a64 0253 0029 0361 2901 0000 0a20  ._.d.S.).a).... 
-00000d20: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-00000d30: 3a0a 2020 2020 2020 2020 2020 2020 7773  :.            ws
-00000d40: 207b 7475 706c 6520 6f66 2061 7272 6179   {tuple of array
-00000d50: 737d 202d 2d20 7765 6967 6874 2061 7272  s} -- weight arr
-00000d60: 6179 206f 6620 676f 6f64 730a 2020 2020  ay of goods.    
-00000d70: 2020 2020 2020 2020 6373 207b 7475 706c          cs {tupl
-00000d80: 6520 6f66 2061 7272 6179 737d 202d 2d20  e of arrays} -- 
-00000d90: 7661 6c75 6520 6172 7261 7920 6f66 2067  value array of g
-00000da0: 6f6f 6473 0a20 2020 2020 2020 2020 2020  oods.           
-00000db0: 2057 207b 6e75 6d62 6572 7d20 2d2d 2075   W {number} -- u
-00000dc0: 7070 6572 2062 6f75 6e64 2028 7072 6f70  pper bound (prop
-00000dd0: 6f72 7469 6f6e 2920 6f66 2074 6f74 616c  ortion) of total
-00000de0: 2077 6569 6768 740a 2020 2020 2020 2020   weight.        
-00000df0: 0a20 2020 2020 2020 204b 6579 776f 7264  .        Keyword
-00000e00: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
-00000e10: 2020 2020 2020 2020 4d20 7b6e 756d 6265          M {numbe
-00000e20: 727d 202d 2d20 7065 6e61 6c74 7920 2864  r} -- penalty (d
-00000e30: 6566 6175 6c74 3a20 7b31 3030 7d29 0a20  efault: {100}). 
-00000e40: 2020 2020 2020 2072 0800 0000 4e29 0b72         r....N).r
-00000e50: 0a00 0000 da03 6d61 7072 0900 0000 da02  ......mapr......
-00000e60: 7773 da02 6373 720d 0000 0072 0e00 0000  ws..csr....r....
-00000e70: 5a16 5f4d 756c 7469 4b6e 6170 7361 636b  Z._MultiKnapsack
-00000e80: 5f5f 736f 7274 6564 da05 7475 706c 6572  __sorted..tupler
-00000e90: 1500 0000 da04 7369 7a65 2905 7210 0000  ......size).r...
-00000ea0: 0072 5800 0000 7259 0000 0072 0d00 0000  .rX...rY...r....
-00000eb0: 720e 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000ec0: 1200 0000 7213 0000 0056 0000 0073 1000  ....r....V...s..
-00000ed0: 0000 080b 1401 0602 0601 0601 0601 0601  ................
-00000ee0: 1401 7a16 4d75 6c74 694b 6e61 7073 6163  ..z.MultiKnapsac
-00000ef0: 6b2e 5f5f 696e 6974 5f5f a908 e904 0000  k.__init__......
-00000f00: 0072 2600 0000 7202 0000 00e9 0600 0000  .r&...r.........
-00000f10: 7226 0000 00e9 0700 0000 722f 0000 0072  r&........r/...r
-00000f20: 3600 0000 6302 0000 0000 0000 0000 0000  6...c...........
-00000f30: 0004 0000 0005 0000 0043 0000 0073 3200  .........C...s2.
-00000f40: 0000 7400 6401 6402 8400 7c00 4400 8301  ..t.d.d...|.D...
-00000f50: 8301 7d02 7400 6403 6402 8400 7c00 4400  ..}.t.d.d...|.D.
-00000f60: 8301 8301 7d03 7401 7c02 7c03 7c01 6404  ....}.t.|.|.|.d.
-00000f70: 8d03 5300 2905 4e63 0100 0000 0000 0000  ..S.).Nc........
-00000f80: 0000 0000 0200 0000 0600 0000 7300 0000  ............s...
-00000f90: f320 0000 0081 007c 005d 0b7d 0174 006a  . .....|.].}.t.j
-00000fa0: 01a0 0264 0064 017c 01a1 0356 0001 0071  ...d.d.|...V...q
-00000fb0: 0264 0253 0029 0372 0800 0000 e933 0000  .d.S.).r.....3..
-00000fc0: 004e a903 7209 0000 0072 1b00 0000 721c  .N..r....r....r.
-00000fd0: 0000 00a9 0272 4200 0000 da01 6e72 1100  .....rB.....nr..
-00000fe0: 0000 7211 0000 0072 1200 0000 da09 3c67  ..r....r......<g
-00000ff0: 656e 6578 7072 3e6d 0000 00f3 0400 0000  enexpr>m........
-00001000: 0280 1e00 7a27 4d75 6c74 694b 6e61 7073  ....z'MultiKnaps
-00001010: 6163 6b2e 7261 6e64 6f6d 2e3c 6c6f 6361  ack.random.<loca
-00001020: 6c73 3e2e 3c67 656e 6578 7072 3e63 0100  ls>.<genexpr>c..
-00001030: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00001040: 0000 7300 0000 7260 0000 0029 0372 0800  ..s...r`...).r..
-00001050: 0000 7219 0000 004e 7262 0000 0072 6300  ..r....Nrb...rc.
-00001060: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00001070: 0072 6500 0000 6e00 0000 7266 0000 0072  .re...n...rf...r
-00001080: 1a00 0000 2902 725a 0000 0072 5600 0000  ....).rZ...rV...
-00001090: 2904 725b 0000 0072 0d00 0000 7258 0000  ).r[...r....rX..
-000010a0: 0072 5900 0000 7211 0000 0072 1100 0000  .rY...r....r....
-000010b0: 7212 0000 0072 1b00 0000 6b00 0000 7306  r....r....k...s.
-000010c0: 0000 0012 0212 010e 017a 144d 756c 7469  .........z.Multi
-000010d0: 4b6e 6170 7361 636b 2e72 616e 646f 6d63  Knapsack.randomc
-000010e0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000010f0: 0400 0000 4300 0000 7322 0000 0074 007c  ....C...s"...t.|
-00001100: 006a 0183 017d 0174 007c 006a 0283 017d  .j...}.t.|.j...}
-00001110: 0274 03a0 047c 017c 021b 00a1 0153 0072  .t...|.|.....S.r
-00001120: 1400 0000 2905 da03 6d69 6e72 5900 0000  ....)...minrY...
-00001130: 7258 0000 0072 0900 0000 723e 0000 0029  rX...r....r>...)
-00001140: 0372 1000 0000 720c 0000 0072 0b00 0000  .r....r....r....
-00001150: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00001160: 3e00 0000 7100 0000 7306 0000 000a 010a  >...q...s.......
-00001170: 010e 017a 154d 756c 7469 4b6e 6170 7361  ...z.MultiKnapsa
-00001180: 636b 2e61 7267 736f 7274 6302 0000 0000  ck.argsortc.....
-00001190: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
-000011a0: 0000 0073 9200 0000 7400 6401 6402 8400  ...s....t.d.d...
-000011b0: 7401 7c01 7c00 6a02 8302 4400 8301 8301  t.|.|.j...D.....
-000011c0: 730f 4a00 8201 7c00 6a03 7c00 6a04 7c00  s.J...|.j.|.j.|.
-000011d0: 6a05 7c00 6a06 6604 5c04 7d02 7d03 7d04  j.|.j.f.\.}.}.}.
-000011e0: 7d05 7407 a008 6403 6404 8400 7401 7c01  }.t...d.d...t.|.
-000011f0: 7c02 8302 4400 8301 a101 7d06 7407 a008  |...D.....}.t...
-00001200: 6405 6404 8400 7401 7c01 7c03 8302 4400  d.d...t.|.|...D.
-00001210: 8301 a101 7d03 7c03 7c04 6b01 723d 7c06  ....}.|.|.k.r=|.
-00001220: 5300 6406 6407 7407 a009 7c06 0b00 a101  S.d.d.t...|.....
-00001230: 1700 1b00 7c05 1400 5300 2908 4e63 0100  ....|...S.).Nc..
-00001240: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00001250: 0000 7300 0000 732c 0000 0081 007c 005d  ..s...s,.....|.]
-00001260: 115c 027d 017d 0264 007c 0104 0003 006b  .\.}.}.d.|.....k
-00001270: 016f 0f7c 026b 006e 0202 0001 0056 0001  .o.|.k.n.....V..
-00001280: 0071 0264 0153 0029 0272 0100 0000 4e72  .q.d.S.).r....Nr
-00001290: 1100 0000 2903 7242 0000 00da 0278 69da  ....).rB.....xi.
-000012a0: 0173 7211 0000 0072 1100 0000 7212 0000  .sr....r....r...
-000012b0: 0072 6500 0000 7800 0000 7304 0000 0002  .re...x...s.....
-000012c0: 802a 007a 294d 756c 7469 4b6e 6170 7361  .*.z)MultiKnapsa
-000012d0: 636b 2e5f 5f63 616c 6c5f 5f2e 3c6c 6f63  ck.__call__.<loc
-000012e0: 616c 733e 2e3c 6765 6e65 7870 723e 6301  als>.<genexpr>c.
-000012f0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00001300: 0000 0053 0000 00f3 1800 0000 6700 7c00  ...S........g.|.
-00001310: 5d08 5c02 7d01 7d02 7c02 7c01 1900 9102  ].\.}.}.|.|.....
-00001320: 7102 5300 7211 0000 0072 1100 0000 2903  q.S.r....r....).
-00001330: 7242 0000 0072 6800 0000 7244 0000 0072  rB...rh...rD...r
-00001340: 1100 0000 7211 0000 0072 1200 0000 7245  ....r....r....rE
-00001350: 0000 007a 0000 00f3 0200 0000 1800 7a2a  ...z..........z*
-00001360: 4d75 6c74 694b 6e61 7073 6163 6b2e 5f5f  MultiKnapsack.__
-00001370: 6361 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e  call__.<locals>.
-00001380: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
-00001390: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
-000013a0: 0000 0072 6a00 0000 7211 0000 0072 1100  ...rj...r....r..
-000013b0: 0000 2903 7242 0000 0072 6800 0000 7247  ..).rB...rh...rG
-000013c0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-000013d0: 0000 7245 0000 007b 0000 0072 6b00 0000  ..rE...{...rk...
-000013e0: 7248 0000 0072 0800 0000 290a da03 616c  rH...r....)...al
-000013f0: 6c72 4900 0000 725b 0000 0072 0c00 0000  lrI...r[...r....
-00001400: 720b 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001410: 0900 0000 720a 0000 0072 4a00 0000 724b  ....r....rJ...rK
-00001420: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00001430: 0000 724e 0000 0076 0000 0073 0e00 0000  ..rN...v...s....
-00001440: 1e02 1c01 1a01 1a01 0801 0401 1802 7a16  ..............z.
-00001450: 4d75 6c74 694b 6e61 7073 6163 6b2e 5f5f  MultiKnapsack.__
-00001460: 6361 6c6c 5f5f 4e72 4f00 0000 2902 725c  call__NrO...).r\
-00001470: 0000 0072 0600 0000 2909 7250 0000 0072  ...r....).rP...r
-00001480: 5100 0000 7252 0000 0072 5300 0000 7213  Q...rR...rS...r.
-00001490: 0000 0072 5500 0000 721b 0000 0072 3e00  ...rU...r....r>.
-000014a0: 0000 724e 0000 0072 1100 0000 7211 0000  ..rN...r....r...
-000014b0: 0072 1100 0000 7212 0000 0072 5600 0000  .r....r....rV...
-000014c0: 4d00 0000 730e 0000 0008 0004 010a 0802  M...s...........
-000014d0: 150c 0108 050c 0572 5600 0000 6300 0000  .......rV...c...
-000014e0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-000014f0: 0040 0000 0073 2a00 0000 6500 5a01 6400  .@...s*...e.Z.d.
-00001500: 5a02 6401 6402 8400 5a03 6504 6409 6404  Z.d.d...Z.e.d.d.
-00001510: 6405 8401 8301 5a05 6406 6407 8400 5a06  d.....Z.d.d...Z.
-00001520: 6408 5300 290a da03 4d4c 4563 0300 0000  d.S.)...MLEc....
-00001530: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00001540: 4300 0000 7310 0000 0074 007c 005f 017c  C...s....t.|._.|
-00001550: 027c 005f 0264 0053 0072 1400 0000 2903  .|._.d.S.r....).
-00001560: da06 6c6f 6770 6466 da03 7064 6672 4c00  ..logpdf..pdfrL.
-00001570: 0000 2903 7210 0000 0072 6f00 0000 724c  ..).r....ro...rL
-00001580: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00001590: 0000 7213 0000 0085 0000 00f3 0400 0000  ..r.............
-000015a0: 0601 0a01 7a0c 4d4c 452e 5f5f 696e 6974  ....z.MLE.__init
-000015b0: 5f5f e92c 0100 0063 0100 0000 0000 0000  __.,...c........
-000015c0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-000015d0: 7326 0000 0064 0164 026c 006d 017d 0101  s&...d.d.l.m.}..
-000015e0: 007c 016a 027c 0064 038d 017d 0274 037c  .|.j.|.d...}.t.|
-000015f0: 016a 047c 0264 048d 0253 0029 054e 7201  .j.|.d...S.).Nr.
-00001600: 0000 00a9 01da 046e 6f72 6da9 0172 5b00  .......norm..r[.
-00001610: 0000 2902 726e 0000 0072 4c00 0000 2905  ..).rn...rL...).
-00001620: da0b 7363 6970 792e 7374 6174 7372 7300  ..scipy.statsrs.
-00001630: 0000 da03 7276 7372 6d00 0000 726e 0000  ....rvsrm...rn..
-00001640: 0029 0372 5b00 0000 7273 0000 0072 4c00  .).r[...rs...rL.
-00001650: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00001660: 0072 1b00 0000 8900 0000 7306 0000 000c  .r........s.....
-00001670: 020c 010e 017a 0a4d 4c45 2e72 616e 646f  .....z.MLE.rando
-00001680: 6d63 0200 0000 0000 0000 0000 0000 0200  mc..............
-00001690: 0000 0500 0000 0300 0000 731c 0000 0074  ..........s....t
-000016a0: 00a0 0187 0087 0166 0264 0164 0284 0888  .......f.d.d....
-000016b0: 006a 0244 0083 01a1 0153 0029 034e 6301  .j.D.....S.).Nc.
-000016c0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000016d0: 0000 0013 0000 0073 1e00 0000 6700 7c00  .......s....g.|.
-000016e0: 5d0b 7d01 8800 6a00 7c01 6701 8801 a201  ].}...j.|.g.....
-000016f0: 5200 8e00 9102 7102 5300 7211 0000 00a9  R.....q.S.r.....
-00001700: 0172 6e00 0000 a902 7242 0000 0072 6800  .rn.....rB...rh.
-00001710: 0000 a902 7210 0000 00da 0174 7211 0000  ....r......tr...
-00001720: 0072 1200 0000 7245 0000 0090 0000 0073  .r....rE.......s
-00001730: 0200 0000 1e00 7a20 4d4c 452e 5f5f 6361  ......z MLE.__ca
-00001740: 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c  ll__.<locals>.<l
-00001750: 6973 7463 6f6d 703e a903 7209 0000 0072  istcomp>..r....r
-00001760: 0a00 0000 724c 0000 0072 7900 0000 7211  ....rL...ry...r.
-00001770: 0000 0072 7900 0000 7212 0000 0072 4e00  ...ry...r....rN.
-00001780: 0000 8f00 0000 7302 0000 001c 017a 0c4d  ......s......z.M
-00001790: 4c45 2e5f 5f63 616c 6c5f 5f4e 2901 7271  LE.__call__N).rq
-000017a0: 0000 00a9 0772 5000 0000 7251 0000 0072  .....rP...rQ...r
-000017b0: 5200 0000 7213 0000 0072 5500 0000 721b  R...r....rU...r.
-000017c0: 0000 0072 4e00 0000 7211 0000 0072 1100  ...rN...r....r..
-000017d0: 0000 7211 0000 0072 1200 0000 726d 0000  ..r....r....rm..
-000017e0: 0082 0000 0073 0a00 0000 0800 0803 0204  .....s..........
-000017f0: 0c01 0c05 726d 0000 0063 0000 0000 0000  ....rm...c......
-00001800: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00001810: 0000 7332 0000 0065 005a 0164 005a 0264  ..s2...e.Z.d.Z.d
-00001820: 0164 0284 005a 0365 0464 0c64 0564 0684  .d...Z.e.d.d.d..
-00001830: 0183 015a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-00001840: 0a84 005a 0764 0b53 0029 0dda 064d 6978  ...Z.d.S.)...Mix
-00001850: 4d4c 4563 0300 0000 0000 0000 0000 0000  MLEc............
-00001860: 0300 0000 0200 0000 4300 0000 f310 0000  ........C.......
-00001870: 007c 017c 005f 007c 027c 005f 0164 0053  .|.|._.|.|._.d.S
-00001880: 0072 1400 0000 a902 da04 7064 6673 724c  .r........pdfsrL
-00001890: 0000 0029 0372 1000 0000 7280 0000 0072  ...).r....r....r
-000018a0: 4c00 0000 7211 0000 0072 1100 0000 7212  L...r....r....r.
-000018b0: 0000 0072 1300 0000 9600 0000 7270 0000  ...r........rp..
-000018c0: 007a 0f4d 6978 4d4c 452e 5f5f 696e 6974  .z.MixMLE.__init
-000018d0: 5f5f 7271 0000 0072 0200 0000 6302 0000  __rq...r....c...
-000018e0: 0000 0000 0000 0000 0006 0000 0004 0000  ................
-000018f0: 0043 0000 0073 4800 0000 6401 6402 6c00  .C...sH...d.d.l.
-00001900: 6d01 7d02 0100 7c02 6a02 7c00 6403 8d01  m.}...|.j.|.d...
-00001910: 7d03 7c02 6a02 6404 7c00 6405 8d02 7d04  }.|.j.d.|.d...}.
-00001920: 7403 a004 7c03 7c04 6602 a101 7d05 7405  t...|.|.f...}.t.
-00001930: 7c02 6a06 6601 7c01 1400 7c05 6406 8d02  |.j.f.|...|.d...
-00001940: 5300 2907 4e72 0100 0000 7272 0000 0072  S.).Nr....rr...r
-00001950: 7400 0000 7202 0000 0029 02da 036c 6f63  t...r....)...loc
-00001960: 725b 0000 0072 7f00 0000 2907 7275 0000  r[...r....).ru..
-00001970: 0072 7300 0000 7276 0000 0072 0900 0000  .rs...rv...r....
-00001980: da06 6873 7461 636b 727d 0000 0072 6f00  ..hstackr}...ro.
-00001990: 0000 2906 5a0c 6e5f 6f62 7365 7276 616e  ..).Z.n_observan
-000019a0: 7473 da0c 6e5f 636f 6d70 6f6e 656e 7473  ts..n_components
-000019b0: 7273 0000 00da 0278 31da 0278 3272 4c00  rs.....x1..x2rL.
-000019c0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-000019d0: 0072 1b00 0000 9a00 0000 730a 0000 000c  .r........s.....
-000019e0: 020c 010e 010e 0114 017a 0d4d 6978 4d4c  .........z.MixML
-000019f0: 452e 7261 6e64 6f6d 6304 0000 0000 0000  E.randomc.......
-00001a00: 0000 0000 0004 0000 0008 0000 0003 0000  ................
-00001a10: 0073 2800 0000 7400 a001 7400 a002 8700  .s(...t...t.....
-00001a20: 6601 6401 6402 8408 7403 7c00 6a04 7c02  f.d.d...t.|.j.|.
-00001a30: 8302 4400 8301 7c03 a102 a101 5300 2903  ..D...|.....S.).
-00001a40: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-00001a50: 0000 0500 0000 1300 0000 731a 0000 0067  ..........s....g
-00001a60: 007c 005d 095c 027d 017d 027c 0188 007c  .|.].\.}.}.|...|
-00001a70: 0283 0291 0271 0253 0072 1100 0000 7211  .....q.S.r....r.
-00001a80: 0000 0029 0372 4200 0000 726f 0000 00da  ...).rB...ro....
-00001a90: 0274 69a9 0172 4c00 0000 7211 0000 0072  .ti..rL...r....r
-00001aa0: 1200 0000 7245 0000 00a3 0000 00f3 0200  ....rE..........
-00001ab0: 0000 1a00 7a21 4d69 784d 4c45 2e6c 6f67  ....z!MixMLE.log
-00001ac0: 7064 662e 3c6c 6f63 616c 733e 2e3c 6c69  pdf.<locals>.<li
-00001ad0: 7374 636f 6d70 3e29 0572 0900 0000 da03  stcomp>).r......
-00001ae0: 6c6f 67da 0364 6f74 7249 0000 0072 8000  log..dotrI...r..
-00001af0: 0000 2904 7210 0000 0072 4c00 0000 727a  ..).r....rL...rz
-00001b00: 0000 00da 0161 7211 0000 0072 8700 0000  .....ar....r....
-00001b10: 7212 0000 0072 6e00 0000 a200 0000 f302  r....rn.........
-00001b20: 0000 0028 017a 0d4d 6978 4d4c 452e 6c6f  ...(.z.MixMLE.lo
-00001b30: 6770 6466 6303 0000 0000 0000 0000 0000  gpdfc...........
-00001b40: 0003 0000 0005 0000 0003 0000 0073 1e00  .............s..
-00001b50: 0000 7400 a001 8700 8701 8702 6603 6401  ..t.........f.d.
-00001b60: 6402 8408 8801 6a02 4400 8301 a101 5300  d.....j.D.....S.
-00001b70: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-00001b80: 0200 0000 0700 0000 1300 0000 731a 0000  ............s...
-00001b90: 0067 007c 005d 097d 0188 01a0 007c 0188  .g.|.].}.....|..
-00001ba0: 0288 00a1 0391 0271 0253 0072 1100 0000  .......q.S.r....
-00001bb0: 7277 0000 0072 7800 0000 a903 728b 0000  rw...rx.....r...
-00001bc0: 0072 1000 0000 727a 0000 0072 1100 0000  .r....rz...r....
-00001bd0: 7212 0000 0072 4500 0000 a700 0000 7288  r....rE.......r.
-00001be0: 0000 007a 234d 6978 4d4c 452e 5f5f 6361  ...z#MixMLE.__ca
-00001bf0: 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c  ll__.<locals>.<l
-00001c00: 6973 7463 6f6d 703e 727b 0000 0029 0372  istcomp>r{...).r
-00001c10: 1000 0000 727a 0000 0072 8b00 0000 7211  ....rz...r....r.
-00001c20: 0000 0072 8d00 0000 7212 0000 0072 4e00  ...r....r....rN.
-00001c30: 0000 a500 0000 7302 0000 001e 027a 0f4d  ......s......z.M
-00001c40: 6978 4d4c 452e 5f5f 6361 6c6c 5f5f 4e29  ixMLE.__call__N)
-00001c50: 0272 7100 0000 7202 0000 0029 0872 5000  .rq...r....).rP.
-00001c60: 0000 7251 0000 0072 5200 0000 7213 0000  ..rQ...rR...r...
-00001c70: 0072 5500 0000 721b 0000 0072 6e00 0000  .rU...r....rn...
-00001c80: 724e 0000 0072 1100 0000 7211 0000 0072  rN...r....r....r
-00001c90: 1100 0000 7212 0000 0072 7d00 0000 9300  ....r....r}.....
-00001ca0: 0000 730c 0000 0008 0008 0302 040c 0108  ..s.............
-00001cb0: 070c 0372 7d00 0000 2902 da05 7064 6973  ...r}...)...pdis
-00001cc0: 74da 0a73 7175 6172 6566 6f72 6d63 0000  t..squareformc..
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00001ce0: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
-00001cf0: 005a 0264 0164 0284 005a 0365 0464 0364  .Z.d.d...Z.e.d.d
-00001d00: 0484 0083 015a 0564 0564 0684 005a 0664  .....Z.d.d...Z.d
-00001d10: 0753 0029 08da 0c53 686f 7274 6573 7450  .S.)...ShortestP
-00001d20: 6174 6863 0200 0000 0000 0000 0000 0000  athc............
-00001d30: 0200 0000 0300 0000 4300 0000 7318 0000  ........C...s...
-00001d40: 007c 017c 005f 0074 0174 027c 0183 0183  .|.|._.t.t.|....
-00001d50: 017c 005f 0364 0153 0029 027a 6d54 5350  .|._.d.S.).zmTSP
-00001d60: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001d70: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
-00001d80: 2020 2020 2020 2020 2070 6f69 6e74 7320           points 
-00001d90: 7b61 7272 6179 2077 6974 6820 7368 6170  {array with shap
-00001da0: 6520 6f66 204e 202a 2032 7d20 2d2d 2070  e of N * 2} -- p
-00001db0: 6f69 6e74 7320 6f66 2074 6865 2070 6174  oints of the pat
-00001dc0: 680a 2020 2020 2020 2020 4e29 04da 0670  h.        N)...p
-00001dd0: 6f69 6e74 7372 8f00 0000 728e 0000 00da  ointsr....r.....
-00001de0: 035f 646d 2902 7210 0000 0072 9100 0000  ._dm).r....r....
-00001df0: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00001e00: 1300 0000 ad00 0000 7304 0000 0006 0612  ........s.......
-00001e10: 017a 1553 686f 7274 6573 7450 6174 682e  .z.ShortestPath.
-00001e20: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00001e30: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00001e40: 0073 1600 0000 7400 7401 6a02 6a02 7c00  .s....t.t.j.j.|.
-00001e50: 6401 6602 6402 8d01 8301 5300 2903 4e72  d.f.d.....S.).Nr
-00001e60: 0200 0000 7274 0000 0029 0372 9000 0000  ....rt...).r....
-00001e70: 7209 0000 0072 1b00 0000 2901 da01 4e72  r....r....)...Nr
-00001e80: 1100 0000 7211 0000 0072 1200 0000 721b  ....r....r....r.
-00001e90: 0000 00b6 0000 0073 0200 0000 1602 7a13  .......s......z.
-00001ea0: 5368 6f72 7465 7374 5061 7468 2e72 616e  ShortestPath.ran
-00001eb0: 646f 6d63 0200 0000 0000 0000 0000 0000  domc............
-00001ec0: 0200 0000 0800 0000 0300 0000 732e 0000  ............s...
-00001ed0: 0074 00a0 0187 0066 0164 0164 0284 0874  .t.....f.d.d...t
-00001ee0: 027c 0164 0064 0385 0219 007c 0164 0464  .|.d.d.....|.d.d
-00001ef0: 0085 0219 0083 0244 0083 01a1 0153 0029  .......D.....S.)
-00001f00: 054e 6301 0000 0000 0000 0000 0000 0003  .Nc.............
-00001f10: 0000 0005 0000 0013 0000 0073 3400 0000  ...........s4...
-00001f20: 6700 7c00 5d16 5c02 7d01 7d02 7c01 7c02  g.|.].\.}.}.|.|.
-00001f30: 6b00 7211 8800 6a00 7c01 7c02 6602 1900  k.r...j.|.|.f...
-00001f40: 6e06 8800 6a00 7c02 7c01 6602 1900 9102  n...j.|.|.f.....
-00001f50: 7102 5300 7211 0000 0029 0172 9200 0000  q.S.r....).r....
-00001f60: 2903 7242 0000 0072 4300 0000 da01 6a72  ).rB...rC.....jr
-00001f70: 1600 0000 7211 0000 0072 1200 0000 7245  ....r....r....rE
-00001f80: 0000 00bb 0000 0073 0200 0000 3400 7a29  .......s....4.z)
-00001f90: 5368 6f72 7465 7374 5061 7468 2e5f 5f63  ShortestPath.__c
-00001fa0: 616c 6c5f 5f2e 3c6c 6f63 616c 733e 2e3c  all__.<locals>.<
-00001fb0: 6c69 7374 636f 6d70 3e72 4800 0000 7208  listcomp>rH...r.
-00001fc0: 0000 0029 0372 0900 0000 720a 0000 0072  ...).r....r....r
-00001fd0: 4900 0000 a902 7210 0000 0072 4c00 0000  I.....r....rL...
-00001fe0: 7211 0000 0072 1600 0000 7212 0000 0072  r....r....r....r
-00001ff0: 4e00 0000 ba00 0000 7302 0000 002e 017a  N.......s......z
-00002000: 1553 686f 7274 6573 7450 6174 682e 5f5f  .ShortestPath.__
-00002010: 6361 6c6c 5f5f 4e72 7c00 0000 7211 0000  call__Nr|...r...
-00002020: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00002030: 7290 0000 00ac 0000 0073 0a00 0000 0800  r........s......
-00002040: 0801 0209 0a01 0c03 7290 0000 0063 0000  ........r....c..
-00002050: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00002060: 0000 0000 0000 731c 0000 0065 005a 0164  ......s....e.Z.d
-00002070: 005a 0287 0066 0164 0164 0284 085a 0387  .Z...f.d.d...Z..
-00002080: 0004 005a 0453 0029 03da 0943 7572 7665  ...Z.S.)...Curve
-00002090: 5061 7468 6303 0000 0000 0000 0000 0000  Pathc...........
-000020a0: 0004 0000 0004 0000 0003 0000 0073 1e00  .............s..
-000020b0: 0000 7400 a001 7c01 7c02 6702 a101 7d03  ..t...|.|.g...}.
-000020c0: 7402 8300 a003 7c03 a101 0100 6400 5300  t.....|.....d.S.
-000020d0: 7214 0000 0029 0472 0900 0000 da0c 636f  r....).r......co
-000020e0: 6c75 6d6e 5f73 7461 636b da05 7375 7065  lumn_stack..supe
-000020f0: 7272 1300 0000 2904 7210 0000 0072 4c00  rr....).r....rL.
-00002100: 0000 da01 79da 075f 706f 696e 7473 a901  ....y.._points..
-00002110: da09 5f5f 636c 6173 735f 5f72 1100 0000  ..__class__r....
-00002120: 7212 0000 0072 1300 0000 bf00 0000 7304  r....r........s.
-00002130: 0000 000e 0110 017a 1243 7572 7665 5061  .......z.CurvePa
-00002140: 7468 2e5f 5f69 6e69 745f 5f29 0572 5000  th.__init__).rP.
-00002150: 0000 7251 0000 0072 5200 0000 7213 0000  ..rQ...rR...r...
-00002160: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00002170: 7211 0000 0072 1100 0000 729b 0000 0072  r....r....r....r
-00002180: 1200 0000 7296 0000 00be 0000 0073 0400  ....r........s..
-00002190: 0000 0800 1401 7296 0000 0072 0800 0000  ......r....r....
-000021a0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-000021b0: 0005 0000 0043 0000 0073 3400 0000 7400  .....C...s4...t.
-000021c0: a001 7c00 a101 7d02 7400 a002 7c00 a101  ..|...}.t...|...
-000021d0: 7400 a003 7c02 6401 1300 6402 a102 1700  t...|.d...d.....
-000021e0: 7d03 7c01 7c02 1400 7c01 7c03 1400 6602  }.|.|...|.|...f.
-000021f0: 5300 2903 4e72 0200 0000 6755 5555 5555  S.).Nr....gUUUUU
-00002200: 55d5 3f29 0472 0900 0000 da03 636f 73da  U.?).r......cos.
-00002210: 0373 696e da05 706f 7765 7229 0472 7a00  .sin..power).rz.
-00002220: 0000 728b 0000 0072 4c00 0000 7299 0000  ..r....rL...r...
-00002230: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00002240: da06 5f68 6561 7274 c400 0000 7306 0000  .._heart....s...
-00002250: 000a 011a 0110 0172 a100 0000 7218 0000  .......r....r...
-00002260: 0067 cdcc cccc cccc f43f 2901 728b 0000  .g.......?).r...
-00002270: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002280: 0000 0300 0000 4000 0000 7322 0000 0065  ......@...s"...e
-00002290: 005a 0164 005a 0267 0064 0166 0264 0264  .Z.d.Z.g.d.f.d.d
-000022a0: 0384 015a 0364 0464 0584 005a 0464 0153  ...Z.d.d...Z.d.S
-000022b0: 0029 06da 0f4d 696e 5370 616e 6e69 6e67  .)...MinSpanning
-000022c0: 5472 6565 4e63 0400 0000 0000 0000 0000  TreeNc..........
-000022d0: 0000 0400 0000 0200 0000 4300 0000 7316  ..........C...s.
-000022e0: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
-000022f0: 037c 005f 0264 0053 0072 1400 0000 2903  .|._.d.S.r....).
-00002300: da05 6e6f 6465 73da 0565 6467 6573 da07  ..nodes..edges..
-00002310: 7765 6967 6874 7329 0472 1000 0000 72a3  weights).r....r.
-00002320: 0000 0072 a400 0000 72a5 0000 0072 1100  ...r....r....r..
-00002330: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00002340: 00d2 0000 0073 0600 0000 0601 0601 0a01  .....s..........
-00002350: 7a18 4d69 6e53 7061 6e6e 696e 6754 7265  z.MinSpanningTre
-00002360: 652e 5f5f 696e 6974 5f5f 6302 0000 0000  e.__init__c.....
-00002370: 0000 0000 0000 0003 0000 0004 0000 0003  ................
-00002380: 0000 0073 2200 0000 7400 7c01 8800 6a01  ...s"...t.|...j.
-00002390: 8302 7d02 7402 8700 6601 6401 6402 8408  ..}.t...f.d.d...
-000023a0: 7c02 4400 8301 8301 5300 2903 4e63 0100  |.D.....S.).Nc..
-000023b0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000023c0: 0000 3300 0000 731a 0000 0081 007c 005d  ..3...s......|.]
-000023d0: 087d 0188 006a 007c 0119 0056 0001 0071  .}...j.|...V...q
-000023e0: 0264 0053 0072 1400 0000 2901 72a5 0000  .d.S.r....).r...
-000023f0: 0029 0272 4200 0000 da04 6564 6765 7216  .).rB.....edger.
-00002400: 0000 0072 1100 0000 7212 0000 0072 6500  ...r....r....re.
-00002410: 0000 d900 0000 7304 0000 0002 8018 007a  ......s........z
-00002420: 2b4d 696e 5370 616e 6e69 6e67 5472 6565  +MinSpanningTree
-00002430: 2e5f 5f63 616c 6c5f 5f2e 3c6c 6f63 616c  .__call__.<local
-00002440: 733e 2e3c 6765 6e65 7870 723e 2903 7203  s>.<genexpr>).r.
-00002450: 0000 0072 a300 0000 720a 0000 0029 0372  ...r....r....).r
-00002460: 1000 0000 724c 0000 0072 a400 0000 7211  ....rL...r....r.
-00002470: 0000 0072 1600 0000 7212 0000 0072 4e00  ...r....r....rN.
-00002480: 0000 d700 0000 7304 0000 000c 0116 017a  ......s........z
-00002490: 184d 696e 5370 616e 6e69 6e67 5472 6565  .MinSpanningTree
-000024a0: 2e5f 5f63 616c 6c5f 5f29 0572 5000 0000  .__call__).rP...
-000024b0: 7251 0000 0072 5200 0000 7213 0000 0072  rQ...rR...r....r
-000024c0: 4e00 0000 7211 0000 0072 1100 0000 7211  N...r....r....r.
-000024d0: 0000 0072 1200 0000 72a2 0000 00d1 0000  ...r....r.......
-000024e0: 0073 0600 0000 0800 0e01 0c05 72a2 0000  .s..........r...
-000024f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002500: 0000 0300 0000 4000 0000 732c 0000 0065  ......@...s,...e
-00002510: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-00002520: 005a 0465 0564 0464 0584 0083 015a 0664  .Z.e.d.d.....Z.d
-00002530: 0664 0784 005a 0764 0853 0029 09da 0e46  .d...Z.d.S.)...F
-00002540: 6163 696c 6974 794c 6179 6f75 747a 170a  acilityLayoutz..
-00002550: 2020 2020 463a 2046 0a20 2020 2044 3a20      F: F.    D: 
-00002560: 440a 2020 2020 6303 0000 0000 0000 0000  D.    c.........
-00002570: 0000 0003 0000 0002 0000 0043 0000 0072  ...........C...r
-00002580: 7e00 0000 7214 0000 0029 02da 0146 da01  ~...r....)...F..
-00002590: 4429 0372 1000 0000 72a8 0000 0072 a900  D).r....r....r..
-000025a0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-000025b0: 0072 1300 0000 e200 0000 7270 0000 007a  .r........rp...z
-000025c0: 1746 6163 696c 6974 794c 6179 6f75 742e  .FacilityLayout.
-000025d0: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
-000025e0: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-000025f0: 0073 2e00 0000 7400 6a01 6a01 7c01 7c01  .s....t.j.j.|.|.
-00002600: 6602 6401 8d01 7d02 7400 6a01 6a01 7c01  f.d...}.t.j.j.|.
-00002610: 7c01 6602 6401 8d01 7d03 7402 7c02 7c03  |.f.d...}.t.|.|.
-00002620: 8302 5300 2902 4e72 7400 0000 2903 7209  ..S.).Nrt...).r.
-00002630: 0000 0072 1b00 0000 72a7 0000 0029 0472  ...r....r....).r
-00002640: 1000 0000 7264 0000 0072 a800 0000 72a9  ....rd...r....r.
-00002650: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00002660: 0000 721b 0000 00e6 0000 0073 0600 0000  ..r........s....
-00002670: 1202 1201 0a01 7a15 4661 6369 6c69 7479  ......z.Facility
-00002680: 4c61 796f 7574 2e72 616e 646f 6d63 0200  Layout.randomc..
-00002690: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-000026a0: 0000 0300 0000 7328 0000 0074 00a0 0188  ......s(...t....
-000026b0: 006a 02a0 03a1 0074 00a0 0487 0087 0166  .j.....t.......f
-000026c0: 0264 0164 0284 0888 0144 0083 01a1 01a1  .d.d.....D......
-000026d0: 0253 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-000026e0: 0000 0003 0000 0006 0000 0013 0000 0073  ...............s
-000026f0: 2400 0000 6700 7c00 5d0e 7d01 8801 4400  $...g.|.].}...D.
-00002700: 5d09 7d02 8800 6a00 7c02 7c01 6602 1900  ].}...j.|.|.f...
-00002710: 9103 7106 7102 5300 7211 0000 0029 0172  ..q.q.S.r....).r
-00002720: a900 0000 2903 7242 0000 00da 0278 6a72  ....).rB.....xjr
-00002730: 6800 0000 7295 0000 0072 1100 0000 7212  h...r....r....r.
-00002740: 0000 0072 4500 0000 ed00 0000 7302 0000  ...rE.......s...
-00002750: 0024 007a 2b46 6163 696c 6974 794c 6179  .$.z+FacilityLay
-00002760: 6f75 742e 5f5f 6361 6c6c 5f5f 2e3c 6c6f  out.__call__.<lo
-00002770: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00002780: 2905 7209 0000 0072 8a00 0000 72a8 0000  ).r....r....r...
-00002790: 00da 0572 6176 656c da05 6172 7261 7972  ...ravel..arrayr
-000027a0: 9500 0000 7211 0000 0072 9500 0000 7212  ....r....r....r.
-000027b0: 0000 0072 4e00 0000 ec00 0000 728c 0000  ...rN.......r...
-000027c0: 007a 1746 6163 696c 6974 794c 6179 6f75  .z.FacilityLayou
-000027d0: 742e 5f5f 6361 6c6c 5f5f 4e29 0872 5000  t.__call__N).rP.
-000027e0: 0000 7251 0000 0072 5200 0000 7253 0000  ..rQ...rR...rS..
-000027f0: 0072 1300 0000 7255 0000 0072 1b00 0000  .r....rU...r....
-00002800: 724e 0000 0072 1100 0000 7211 0000 0072  rN...r....r....r
-00002810: 1100 0000 7212 0000 0072 a700 0000 dc00  ....r....r......
-00002820: 0000 730c 0000 0008 0004 0108 0502 040a  ..s.............
-00002830: 010c 0572 a700 0000 7241 0000 0029 1dda  ...r....rA...)..
-00002840: 056e 756d 7079 7209 0000 00da 0575 7469  .numpyr......uti
-00002850: 6c73 7203 0000 00da 0a62 656e 6368 6d61  lsr......benchma
-00002860: 726b 7372 0400 0000 7205 0000 0072 5600  rksr....r....rV.
-00002870: 0000 726d 0000 0072 7d00 0000 da16 7363  ..rm...r}.....sc
-00002880: 6970 792e 7370 6174 6961 6c2e 6469 7374  ipy.spatial.dist
-00002890: 616e 6365 728e 0000 0072 8f00 0000 7290  ancer....r....r.
-000028a0: 0000 0072 9600 0000 72a1 0000 00da 086c  ...r....r......l
-000028b0: 696e 7370 6163 65da 0270 6972 7a00 0000  inspace..pirz...
-000028c0: 7284 0000 00da 0279 3172 8500 0000 da02  r......y1r......
-000028d0: 7932 7282 0000 0072 4c00 0000 7299 0000  y2r....rL...r...
-000028e0: 005a 0a68 6561 7274 5f70 6174 6872 a200  .Z.heart_pathr..
-000028f0: 0000 72a7 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00002900: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
-00002910: 6475 6c65 3e01 0000 0073 2600 0000 0802  dule>....s&.....
-00002920: 0c02 0c01 1003 1044 1035 1011 1017 1002  .......D.5......
-00002930: 1012 0a06 1405 0c01 1001 0e01 0e01 0a01  ................
-00002940: 1003 140b                                ....
+00000470: 0000 fa4e 2f55 7365 7273 2f77 696c 6c69  ...N/Users/willi
+00000480: 616d 2f50 726f 6772 616d 6d69 6e67 2f50  am/Programming/P
+00000490: 7974 686f 6e2f 6d79 776f 726b 2f70 7972  ython/mywork/pyr
+000004a0: 696d 6964 696e 652f 6265 6e63 686d 6172  imidine/benchmar
+000004b0: 6b73 2f6f 7074 696d 697a 6174 696f 6e2e  ks/optimization.
+000004c0: 7079 da08 5f5f 696e 6974 5f5f 1100 0000  py..__init__....
+000004d0: 730e 0000 0008 0c0e 0106 0206 0106 0106  s...............
+000004e0: 010a 017a 114b 6e61 7073 6163 6b2e 5f5f  ...z.Knapsack.__
+000004f0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000500: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000510: 0a00 0000 7400 7c00 6a01 8301 5300 a901  ....t.|.j...S...
+00000520: 4e29 02da 036c 656e 720c 0000 00a9 0172  N)...lenr......r
+00000530: 1000 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00000540: 0000 00da 066e 5f62 6167 7326 0000 0073  .....n_bags&...s
+00000550: 0200 0000 0a02 7a0f 4b6e 6170 7361 636b  ......z.Knapsack
+00000560: 2e6e 5f62 6167 73e9 3200 0000 6302 0000  .n_bags.2...c...
+00000570: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00000580: 0043 0000 0073 2e00 0000 7400 6a01 a002  .C...s....t.j...
+00000590: 6401 6402 7c00 a103 7d02 7400 6a01 a002  d.d.|...}.t.j...
+000005a0: 6401 6402 7c00 a103 7d03 7403 7c02 7c03  d.d.|...}.t.|.|.
+000005b0: 7c01 6403 8d03 5300 2904 4e72 0800 0000  |.d...S.).Nr....
+000005c0: e915 0000 00a9 0172 0d00 0000 2904 7209  .......r....).r.
+000005d0: 0000 00da 0672 616e 646f 6dda 0772 616e  .....random..ran
+000005e0: 6469 6e74 7205 0000 0029 0472 1700 0000  dintr....).r....
+000005f0: 720d 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000600: 1100 0000 7211 0000 0072 1200 0000 721b  ....r....r....r.
+00000610: 0000 002a 0000 0073 0600 0000 1002 1001  ...*...s........
+00000620: 0e01 7a0f 4b6e 6170 7361 636b 2e72 616e  ..z.Knapsack.ran
+00000630: 646f 6d63 0100 0000 0000 0000 0000 0000  domc............
+00000640: 0300 0000 0500 0000 4300 0000 731e 0000  ........C...s...
+00000650: 0067 0064 01a2 017d 0167 0064 02a2 017d  .g.d...}.g.d...}
+00000660: 0274 007c 017c 027c 0064 038d 0353 0029  .t.|.|.|.d...S.)
+00000670: 044e 2915 e947 0000 00e9 2200 0000 e952  .N)..G...."....R
+00000680: 0000 00e9 1700 0000 7208 0000 00e9 5800  ........r.....X.
+00000690: 0000 e90c 0000 00e9 3900 0000 e90a 0000  ........9.......
+000006a0: 00e9 4400 0000 e905 0000 00e9 2100 0000  ..D.........!...
+000006b0: e925 0000 00e9 4500 0000 e962 0000 00e9  .%....E....b....
+000006c0: 1800 0000 e91a 0000 00e9 5300 0000 e910  ..........S.....
+000006d0: 0000 0072 2c00 0000 e908 0000 0029 1572  ...r,........).r
+000006e0: 2c00 0000 e93b 0000 00e9 1e00 0000 e913  ,....;..........
+000006f0: 0000 00e9 4200 0000 e955 0000 00e9 5e00  ....B....U....^.
+00000700: 0000 722f 0000 00e9 0300 0000 e92c 0000  ..r/.........,..
+00000710: 0072 2600 0000 7208 0000 00e9 2900 0000  .r&...r.....)...
+00000720: 721f 0000 00e9 4c00 0000 7208 0000 0072  r.....L...r....r
+00000730: 2200 0000 e951 0000 00e9 4900 0000 e920  "....Q....I.... 
+00000740: 0000 0072 3600 0000 721a 0000 0029 0172  ...r6...r....).r
+00000750: 0500 0000 2903 720d 0000 0072 0b00 0000  ....).r....r....
+00000760: 720c 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000770: 1200 0000 da07 6578 616d 706c 6530 0000  ......example0..
+00000780: 0073 0600 0000 0802 0801 0e01 7a10 4b6e  .s..........z.Kn
+00000790: 6170 7361 636b 2e65 7861 6d70 6c65 6301  apsack.examplec.
+000007a0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000007b0: 0000 0043 0000 0073 1200 0000 7400 a001  ...C...s....t...
+000007c0: 7c00 6a02 7c00 6a03 1b00 a101 5300 7214  |.j.|.j.....S.r.
+000007d0: 0000 0029 0472 0900 0000 da07 6172 6773  ...).r......args
+000007e0: 6f72 7472 0c00 0000 720b 0000 0072 1600  ortr....r....r..
+000007f0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00000800: 0072 3e00 0000 3600 0000 7302 0000 0012  .r>...6...s.....
+00000810: 017a 104b 6e61 7073 6163 6b2e 6172 6773  .z.Knapsack.args
+00000820: 6f72 7463 0100 0000 0000 0000 0000 0000  ortc............
+00000830: 0100 0000 0200 0000 4300 0000 731a 0000  ........C...s...
+00000840: 007c 006a 0064 0075 0072 0a7c 00a0 01a1  .|.j.d.u.r.|....
+00000850: 007c 005f 007c 006a 0053 0072 1400 0000  .|._.|.j.S.r....
+00000860: 2902 720f 0000 0072 3e00 0000 7216 0000  ).r....r>...r...
+00000870: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000880: da06 736f 7274 6564 3900 0000 7306 0000  ..sorted9...s...
+00000890: 000a 020a 0106 027a 0f4b 6e61 7073 6163  .......z.Knapsac
+000008a0: 6b2e 736f 7274 6564 6302 0000 0000 0000  k.sortedc.......
+000008b0: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
+000008c0: 0073 7400 0000 7c00 6a00 7c00 6a01 7c00  .st...|.j.|.j.|.
+000008d0: 6a02 7c00 6a03 6604 5c04 7d02 7d03 7d04  j.|.j.f.\.}.}.}.
+000008e0: 7d05 7404 a005 6401 6402 8400 7406 7c01  }.t...d.d...t.|.
+000008f0: 7c02 8302 4400 8301 a101 7d06 7404 a005  |...D.....}.t...
+00000900: 6403 6402 8400 7406 7c01 7c03 8302 4400  d.d...t.|.|...D.
+00000910: 8301 a101 7d03 7c03 7c04 6b01 722e 7c06  ....}.|.|.k.r.|.
+00000920: 5300 6404 6405 7404 a007 7c06 0b00 a101  S.d.d.t...|.....
+00000930: 1700 1b00 7c05 1400 5300 2906 4e63 0100  ....|...S.).Nc..
+00000940: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000950: 0000 5300 0000 f31c 0000 0067 007c 005d  ..S........g.|.]
+00000960: 0a5c 027d 017d 027c 0164 006b 0272 027c  .\.}.}.|.d.k.r.|
+00000970: 0291 0271 0253 00a9 0172 0800 0000 7211  ...q.S...r....r.
+00000980: 0000 0029 03da 022e 30da 0169 da02 6369  ...)....0..i..ci
+00000990: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+000009a0: 0a3c 6c69 7374 636f 6d70 3e43 0000 00f3  .<listcomp>C....
+000009b0: 0200 0000 1c00 7a25 4b6e 6170 7361 636b  ......z%Knapsack
+000009c0: 2e5f 5f63 616c 6c5f 5f2e 3c6c 6f63 616c  .__call__.<local
+000009d0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+000009e0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+000009f0: 0000 5300 0000 7240 0000 0072 4100 0000  ..S...r@...rA...
+00000a00: 7211 0000 0029 0372 4200 0000 7243 0000  r....).rB...rC..
+00000a10: 00da 0277 6972 1100 0000 7211 0000 0072  ...wir....r....r
+00000a20: 1200 0000 7245 0000 0044 0000 0072 4600  ....rE...D...rF.
+00000a30: 0000 e9ff ffff ff72 0800 0000 2908 720c  .......r....).r.
+00000a40: 0000 0072 0b00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000a50: 0000 7209 0000 0072 0a00 0000 da03 7a69  ..r....r......zi
+00000a60: 70da 0365 7870 a907 7210 0000 00da 0178  p..exp..r......x
+00000a70: 720c 0000 0072 0b00 0000 720d 0000 0072  r....r....r....r
+00000a80: 0e00 0000 da01 7672 1100 0000 7211 0000  ......vr....r...
+00000a90: 0072 1200 0000 da08 5f5f 6361 6c6c 5f5f  .r......__call__
+00000aa0: 4000 0000 730c 0000 001c 021a 011a 0108  @...s...........
+00000ab0: 0104 0118 027a 114b 6e61 7073 6163 6b2e  .....z.Knapsack.
+00000ac0: 5f5f 6361 6c6c 5f5f 4ea9 0272 0600 0000  __call__N..r....
+00000ad0: 7207 0000 0029 0272 1800 0000 7206 0000  r....).r....r...
+00000ae0: 0029 0172 0600 0000 290d da08 5f5f 6e61  .).r....)...__na
+00000af0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000b00: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000b10: 5f5f 646f 635f 5f72 1300 0000 da08 7072  __doc__r......pr
+00000b20: 6f70 6572 7479 7217 0000 00da 0c73 7461  opertyr......sta
+00000b30: 7469 636d 6574 686f 6472 1b00 0000 723d  ticmethodr....r=
+00000b40: 0000 0072 3e00 0000 723f 0000 0072 4e00  ...r>...r?...rN.
+00000b50: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
+00000b60: 0072 1200 0000 7205 0000 0009 0000 0073  .r....r........s
+00000b70: 1a00 0000 0800 0401 0a07 0215 0a01 0203  ................
+00000b80: 0c01 0205 0c01 0805 0203 0a01 0c06 7205  ..............r.
+00000b90: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000ba0: 0000 0000 0400 0000 4000 0000 7338 0000  ........@...s8..
+00000bb0: 0065 005a 0164 005a 0264 015a 0364 0e64  .e.Z.d.Z.d.Z.d.d
+00000bc0: 0464 0584 015a 0465 0564 0f64 0764 0884  .d...Z.e.d.d.d..
+00000bd0: 0183 015a 0664 0964 0a84 005a 0764 0b64  ...Z.d.d...Z.d.d
+00000be0: 0c84 005a 0864 0d53 0029 10da 0d4d 756c  ...Z.d.S.)...Mul
+00000bf0: 7469 4b6e 6170 7361 636b 7a9f 4d75 6c74  tiKnapsackz.Mult
+00000c00: 6920 4368 6f69 6365 204b 6e61 7073 6163  i Choice Knapsac
+00000c10: 6b20 5072 6f62 6c65 6d0a 0a20 2020 206d  k Problem..    m
+00000c20: 6178 2073 756d 5f69 6a20 6369 6a20 7869  ax sum_ij cij xi
+00000c30: 6a0a 2020 2020 732e 742e 2073 756d 5f69  j.    s.t. sum_i
+00000c40: 6a20 7769 6a20 7869 6a20 3c3d 2057 0a20  j wij xij <= W. 
+00000c50: 2020 207b 7869 6a7d 2069 7320 0a20 2020     {xij} is .   
+00000c60: 2077 6865 7265 2078 696a 2069 7320 7468   where xij is th
+00000c70: 6520 6368 6f69 6365 2076 6172 6961 626c  e choice variabl
+00000c80: 652c 2074 6861 7420 6973 2073 756d 5f6a  e, that is sum_j
+00000c90: 2078 696a 3d31 0a20 2020 2072 0600 0000   xij=1.    r....
+00000ca0: 7207 0000 0063 0500 0000 0000 0000 0000  r....c..........
+00000cb0: 0000 0500 0000 0400 0000 4300 0000 734e  ..........C...sN
+00000cc0: 0000 007c 0364 016b 0072 0e74 0074 0174  ...|.d.k.r.t.t.t
+00000cd0: 026a 007c 0183 0283 017c 0314 007d 037c  .j.|.....|...}.|
+00000ce0: 017c 005f 037c 027c 005f 047c 037c 005f  .|._.|.|._.|.|._
+00000cf0: 057c 047c 005f 0664 027c 005f 0774 0874  .|.|._.d.|._.t.t
+00000d00: 0174 097c 0283 0283 017c 005f 0a64 0253  .t.|.....|._.d.S
+00000d10: 0029 0361 2901 0000 0a20 2020 2020 2020  .).a)....       
+00000d20: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
+00000d30: 2020 2020 2020 2020 7773 207b 7475 706c          ws {tupl
+00000d40: 6520 6f66 2061 7272 6179 737d 202d 2d20  e of arrays} -- 
+00000d50: 7765 6967 6874 2061 7272 6179 206f 6620  weight array of 
+00000d60: 676f 6f64 730a 2020 2020 2020 2020 2020  goods.          
+00000d70: 2020 6373 207b 7475 706c 6520 6f66 2061    cs {tuple of a
+00000d80: 7272 6179 737d 202d 2d20 7661 6c75 6520  rrays} -- value 
+00000d90: 6172 7261 7920 6f66 2067 6f6f 6473 0a20  array of goods. 
+00000da0: 2020 2020 2020 2020 2020 2057 207b 6e75             W {nu
+00000db0: 6d62 6572 7d20 2d2d 2075 7070 6572 2062  mber} -- upper b
+00000dc0: 6f75 6e64 2028 7072 6f70 6f72 7469 6f6e  ound (proportion
+00000dd0: 2920 6f66 2074 6f74 616c 2077 6569 6768  ) of total weigh
+00000de0: 740a 2020 2020 2020 2020 0a20 2020 2020  t.        .     
+00000df0: 2020 204b 6579 776f 7264 2041 7267 756d     Keyword Argum
+00000e00: 656e 7473 3a0a 2020 2020 2020 2020 2020  ents:.          
+00000e10: 2020 4d20 7b6e 756d 6265 727d 202d 2d20    M {number} -- 
+00000e20: 7065 6e61 6c74 7920 2864 6566 6175 6c74  penalty (default
+00000e30: 3a20 7b31 3030 7d29 0a20 2020 2020 2020  : {100}).       
+00000e40: 2072 0800 0000 4e29 0b72 0a00 0000 da03   r....N).r......
+00000e50: 6d61 7072 0900 0000 da02 7773 da02 6373  mapr......ws..cs
+00000e60: 720d 0000 0072 0e00 0000 5a16 5f4d 756c  r....r....Z._Mul
+00000e70: 7469 4b6e 6170 7361 636b 5f5f 736f 7274  tiKnapsack__sort
+00000e80: 6564 da05 7475 706c 6572 1500 0000 da04  ed..tupler......
+00000e90: 7369 7a65 2905 7210 0000 0072 5800 0000  size).r....rX...
+00000ea0: 7259 0000 0072 0d00 0000 720e 0000 0072  rY...r....r....r
+00000eb0: 1100 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00000ec0: 0000 0056 0000 0073 1000 0000 080b 1401  ...V...s........
+00000ed0: 0602 0601 0601 0601 0601 1401 7a16 4d75  ............z.Mu
+00000ee0: 6c74 694b 6e61 7073 6163 6b2e 5f5f 696e  ltiKnapsack.__in
+00000ef0: 6974 5f5f a908 e904 0000 0072 2600 0000  it__.......r&...
+00000f00: 7202 0000 00e9 0600 0000 7226 0000 00e9  r.........r&....
+00000f10: 0700 0000 722f 0000 0072 3600 0000 6302  ....r/...r6...c.
+00000f20: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00000f30: 0000 0043 0000 0073 3200 0000 7400 6401  ...C...s2...t.d.
+00000f40: 6402 8400 7c00 4400 8301 8301 7d02 7400  d...|.D.....}.t.
+00000f50: 6403 6402 8400 7c00 4400 8301 8301 7d03  d.d...|.D.....}.
+00000f60: 7401 7c02 7c03 7c01 6404 8d03 5300 2905  t.|.|.|.d...S.).
+00000f70: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00000f80: 0000 0600 0000 7300 0000 f320 0000 0081  ......s.... ....
+00000f90: 007c 005d 0b7d 0174 006a 01a0 0264 0064  .|.].}.t.j...d.d
+00000fa0: 017c 01a1 0356 0001 0071 0264 0253 0029  .|...V...q.d.S.)
+00000fb0: 0372 0800 0000 e933 0000 004e a903 7209  .r.....3...N..r.
+00000fc0: 0000 0072 1b00 0000 721c 0000 00a9 0272  ...r....r......r
+00000fd0: 4200 0000 da01 6e72 1100 0000 7211 0000  B.....nr....r...
+00000fe0: 0072 1200 0000 da09 3c67 656e 6578 7072  .r......<genexpr
+00000ff0: 3e6d 0000 00f3 0400 0000 0280 1e00 7a27  >m............z'
+00001000: 4d75 6c74 694b 6e61 7073 6163 6b2e 7261  MultiKnapsack.ra
+00001010: 6e64 6f6d 2e3c 6c6f 6361 6c73 3e2e 3c67  ndom.<locals>.<g
+00001020: 656e 6578 7072 3e63 0100 0000 0000 0000  enexpr>c........
+00001030: 0000 0000 0200 0000 0600 0000 7300 0000  ............s...
+00001040: 7260 0000 0029 0372 0800 0000 7219 0000  r`...).r....r...
+00001050: 004e 7262 0000 0072 6300 0000 7211 0000  .Nrb...rc...r...
+00001060: 0072 1100 0000 7212 0000 0072 6500 0000  .r....r....re...
+00001070: 6e00 0000 7266 0000 0072 1a00 0000 2902  n...rf...r....).
+00001080: 725a 0000 0072 5600 0000 2904 725b 0000  rZ...rV...).r[..
+00001090: 0072 0d00 0000 7258 0000 0072 5900 0000  .r....rX...rY...
+000010a0: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+000010b0: 1b00 0000 6b00 0000 7306 0000 0012 0212  ....k...s.......
+000010c0: 010e 017a 144d 756c 7469 4b6e 6170 7361  ...z.MultiKnapsa
+000010d0: 636b 2e72 616e 646f 6d63 0100 0000 0000  ck.randomc......
+000010e0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+000010f0: 0000 7322 0000 0074 007c 006a 0183 017d  ..s"...t.|.j...}
+00001100: 0174 007c 006a 0283 017d 0274 03a0 047c  .t.|.j...}.t...|
+00001110: 017c 021b 00a1 0153 0072 1400 0000 2905  .|.....S.r....).
+00001120: da03 6d69 6e72 5900 0000 7258 0000 0072  ..minrY...rX...r
+00001130: 0900 0000 723e 0000 0029 0372 1000 0000  ....r>...).r....
+00001140: 720c 0000 0072 0b00 0000 7211 0000 0072  r....r....r....r
+00001150: 1100 0000 7212 0000 0072 3e00 0000 7100  ....r....r>...q.
+00001160: 0000 7306 0000 000a 010a 010e 017a 154d  ..s..........z.M
+00001170: 756c 7469 4b6e 6170 7361 636b 2e61 7267  ultiKnapsack.arg
+00001180: 736f 7274 6302 0000 0000 0000 0000 0000  sortc...........
+00001190: 0007 0000 0006 0000 0043 0000 0073 9200  .........C...s..
+000011a0: 0000 7400 6401 6402 8400 7401 7c01 7c00  ..t.d.d...t.|.|.
+000011b0: 6a02 8302 4400 8301 8301 730f 4a00 8201  j...D.....s.J...
+000011c0: 7c00 6a03 7c00 6a04 7c00 6a05 7c00 6a06  |.j.|.j.|.j.|.j.
+000011d0: 6604 5c04 7d02 7d03 7d04 7d05 7407 a008  f.\.}.}.}.}.t...
+000011e0: 6403 6404 8400 7401 7c01 7c02 8302 4400  d.d...t.|.|...D.
+000011f0: 8301 a101 7d06 7407 a008 6405 6404 8400  ....}.t...d.d...
+00001200: 7401 7c01 7c03 8302 4400 8301 a101 7d03  t.|.|...D.....}.
+00001210: 7c03 7c04 6b01 723d 7c06 5300 6406 6407  |.|.k.r=|.S.d.d.
+00001220: 7407 a009 7c06 0b00 a101 1700 1b00 7c05  t...|.........|.
+00001230: 1400 5300 2908 4e63 0100 0000 0000 0000  ..S.).Nc........
+00001240: 0000 0000 0300 0000 0400 0000 7300 0000  ............s...
+00001250: 732c 0000 0081 007c 005d 115c 027d 017d  s,.....|.].\.}.}
+00001260: 0264 007c 0104 0003 006b 016f 0f7c 026b  .d.|.....k.o.|.k
+00001270: 006e 0202 0001 0056 0001 0071 0264 0153  .n.....V...q.d.S
+00001280: 0029 0272 0100 0000 4e72 1100 0000 2903  .).r....Nr....).
+00001290: 7242 0000 00da 0278 69da 0173 7211 0000  rB.....xi..sr...
+000012a0: 0072 1100 0000 7212 0000 0072 6500 0000  .r....r....re...
+000012b0: 7800 0000 7304 0000 0002 802a 007a 294d  x...s......*.z)M
+000012c0: 756c 7469 4b6e 6170 7361 636b 2e5f 5f63  ultiKnapsack.__c
+000012d0: 616c 6c5f 5f2e 3c6c 6f63 616c 733e 2e3c  all__.<locals>.<
+000012e0: 6765 6e65 7870 723e 6301 0000 0000 0000  genexpr>c.......
+000012f0: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
+00001300: 00f3 1800 0000 6700 7c00 5d08 5c02 7d01  ......g.|.].\.}.
+00001310: 7d02 7c02 7c01 1900 9102 7102 5300 7211  }.|.|.....q.S.r.
+00001320: 0000 0072 1100 0000 2903 7242 0000 0072  ...r....).rB...r
+00001330: 6800 0000 7244 0000 0072 1100 0000 7211  h...rD...r....r.
+00001340: 0000 0072 1200 0000 7245 0000 007a 0000  ...r....rE...z..
+00001350: 00f3 0200 0000 1800 7a2a 4d75 6c74 694b  ........z*MultiK
+00001360: 6e61 7073 6163 6b2e 5f5f 6361 6c6c 5f5f  napsack.__call__
+00001370: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001380: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00001390: 0003 0000 0004 0000 0053 0000 0072 6a00  .........S...rj.
+000013a0: 0000 7211 0000 0072 1100 0000 2903 7242  ..r....r....).rB
+000013b0: 0000 0072 6800 0000 7247 0000 0072 1100  ...rh...rG...r..
+000013c0: 0000 7211 0000 0072 1200 0000 7245 0000  ..r....r....rE..
+000013d0: 007b 0000 0072 6b00 0000 7248 0000 0072  .{...rk...rH...r
+000013e0: 0800 0000 290a da03 616c 6c72 4900 0000  ....)...allrI...
+000013f0: 725b 0000 0072 0c00 0000 720b 0000 0072  r[...r....r....r
+00001400: 0d00 0000 720e 0000 0072 0900 0000 720a  ....r....r....r.
+00001410: 0000 0072 4a00 0000 724b 0000 0072 1100  ...rJ...rK...r..
+00001420: 0000 7211 0000 0072 1200 0000 724e 0000  ..r....r....rN..
+00001430: 0076 0000 0073 0e00 0000 1e02 1c01 1a01  .v...s..........
+00001440: 1a01 0801 0401 1802 7a16 4d75 6c74 694b  ........z.MultiK
+00001450: 6e61 7073 6163 6b2e 5f5f 6361 6c6c 5f5f  napsack.__call__
+00001460: 4e72 4f00 0000 2902 725c 0000 0072 0600  NrO...).r\...r..
+00001470: 0000 2909 7250 0000 0072 5100 0000 7252  ..).rP...rQ...rR
+00001480: 0000 0072 5300 0000 7213 0000 0072 5500  ...rS...r....rU.
+00001490: 0000 721b 0000 0072 3e00 0000 724e 0000  ..r....r>...rN..
+000014a0: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+000014b0: 7212 0000 0072 5600 0000 4d00 0000 730e  r....rV...M...s.
+000014c0: 0000 0008 0004 010a 0802 150c 0108 050c  ................
+000014d0: 0572 5600 0000 6300 0000 0000 0000 0000  .rV...c.........
+000014e0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+000014f0: 2a00 0000 6500 5a01 6400 5a02 6401 6402  *...e.Z.d.Z.d.d.
+00001500: 8400 5a03 6504 6409 6404 6405 8401 8301  ..Z.e.d.d.d.....
+00001510: 5a05 6406 6407 8400 5a06 6408 5300 290a  Z.d.d...Z.d.S.).
+00001520: da03 4d4c 4563 0300 0000 0000 0000 0000  ..MLEc..........
+00001530: 0000 0300 0000 0200 0000 4300 0000 7310  ..........C...s.
+00001540: 0000 0074 007c 005f 017c 027c 005f 0264  ...t.|._.|.|._.d
+00001550: 0053 0072 1400 0000 2903 da06 6c6f 6770  .S.r....)...logp
+00001560: 6466 da03 7064 6672 4c00 0000 2903 7210  df..pdfrL...).r.
+00001570: 0000 0072 6f00 0000 724c 0000 0072 1100  ...ro...rL...r..
+00001580: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00001590: 0085 0000 00f3 0400 0000 0601 0a01 7a0c  ..............z.
+000015a0: 4d4c 452e 5f5f 696e 6974 5f5f e92c 0100  MLE.__init__.,..
+000015b0: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+000015c0: 0000 0400 0000 4300 0000 7326 0000 0064  ......C...s&...d
+000015d0: 0164 026c 006d 017d 0101 007c 016a 027c  .d.l.m.}...|.j.|
+000015e0: 0064 038d 017d 0274 037c 016a 047c 0264  .d...}.t.|.j.|.d
+000015f0: 048d 0253 0029 054e 7201 0000 00a9 01da  ...S.).Nr.......
+00001600: 046e 6f72 6da9 0172 5b00 0000 2902 726e  .norm..r[...).rn
+00001610: 0000 0072 4c00 0000 2905 da0b 7363 6970  ...rL...)...scip
+00001620: 792e 7374 6174 7372 7300 0000 da03 7276  y.statsrs.....rv
+00001630: 7372 6d00 0000 726e 0000 0029 0372 5b00  srm...rn...).r[.
+00001640: 0000 7273 0000 0072 4c00 0000 7211 0000  ..rs...rL...r...
+00001650: 0072 1100 0000 7212 0000 0072 1b00 0000  .r....r....r....
+00001660: 8900 0000 7306 0000 000c 020c 010e 017a  ....s..........z
+00001670: 0a4d 4c45 2e72 616e 646f 6d63 0200 0000  .MLE.randomc....
+00001680: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00001690: 0300 0000 731c 0000 0074 00a0 0187 0087  ....s....t......
+000016a0: 0166 0264 0164 0284 0888 006a 0244 0083  .f.d.d.....j.D..
+000016b0: 01a1 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
+000016c0: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+000016d0: 0073 1e00 0000 6700 7c00 5d0b 7d01 8800  .s....g.|.].}...
+000016e0: 6a00 7c01 6701 8801 a201 5200 8e00 9102  j.|.g.....R.....
+000016f0: 7102 5300 7211 0000 00a9 0172 6e00 0000  q.S.r......rn...
+00001700: a902 7242 0000 0072 6800 0000 a902 7210  ..rB...rh.....r.
+00001710: 0000 00da 0174 7211 0000 0072 1200 0000  .....tr....r....
+00001720: 7245 0000 0090 0000 0073 0200 0000 1e00  rE.......s......
+00001730: 7a20 4d4c 452e 5f5f 6361 6c6c 5f5f 2e3c  z MLE.__call__.<
+00001740: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001750: 703e a903 7209 0000 0072 0a00 0000 724c  p>..r....r....rL
+00001760: 0000 0072 7900 0000 7211 0000 0072 7900  ...ry...r....ry.
+00001770: 0000 7212 0000 0072 4e00 0000 8f00 0000  ..r....rN.......
+00001780: 7302 0000 001c 017a 0c4d 4c45 2e5f 5f63  s......z.MLE.__c
+00001790: 616c 6c5f 5f4e 2901 7271 0000 00a9 0772  all__N).rq.....r
+000017a0: 5000 0000 7251 0000 0072 5200 0000 7213  P...rQ...rR...r.
+000017b0: 0000 0072 5500 0000 721b 0000 0072 4e00  ...rU...r....rN.
+000017c0: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
+000017d0: 0072 1200 0000 726d 0000 0082 0000 0073  .r....rm.......s
+000017e0: 0a00 0000 0800 0803 0204 0c01 0c05 726d  ..............rm
+000017f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001800: 0000 0000 0400 0000 4000 0000 7332 0000  ........@...s2..
+00001810: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00001820: 0365 0464 0c64 0564 0684 0183 015a 0564  .e.d.d.d.....Z.d
+00001830: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
+00001840: 0b53 0029 0dda 064d 6978 4d4c 4563 0300  .S.)...MixMLEc..
+00001850: 0000 0000 0000 0000 0000 0300 0000 0200  ................
+00001860: 0000 4300 0000 f310 0000 007c 017c 005f  ..C........|.|._
+00001870: 007c 027c 005f 0164 0053 0072 1400 0000  .|.|._.d.S.r....
+00001880: a902 da04 7064 6673 724c 0000 0029 0372  ....pdfsrL...).r
+00001890: 1000 0000 7280 0000 0072 4c00 0000 7211  ....r....rL...r.
+000018a0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+000018b0: 0000 9600 0000 7270 0000 007a 0f4d 6978  ......rp...z.Mix
+000018c0: 4d4c 452e 5f5f 696e 6974 5f5f 7271 0000  MLE.__init__rq..
+000018d0: 0072 0200 0000 6302 0000 0000 0000 0000  .r....c.........
+000018e0: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+000018f0: 4800 0000 6401 6402 6c00 6d01 7d02 0100  H...d.d.l.m.}...
+00001900: 7c02 6a02 7c00 6403 8d01 7d03 7c02 6a02  |.j.|.d...}.|.j.
+00001910: 6404 7c00 6405 8d02 7d04 7403 a004 7c03  d.|.d...}.t...|.
+00001920: 7c04 6602 a101 7d05 7405 7c02 6a06 6601  |.f...}.t.|.j.f.
+00001930: 7c01 1400 7c05 6406 8d02 5300 2907 4e72  |...|.d...S.).Nr
+00001940: 0100 0000 7272 0000 0072 7400 0000 7202  ....rr...rt...r.
+00001950: 0000 0029 02da 036c 6f63 725b 0000 0072  ...)...locr[...r
+00001960: 7f00 0000 2907 7275 0000 0072 7300 0000  ....).ru...rs...
+00001970: 7276 0000 0072 0900 0000 da06 6873 7461  rv...r......hsta
+00001980: 636b 727d 0000 0072 6f00 0000 2906 5a0c  ckr}...ro...).Z.
+00001990: 6e5f 6f62 7365 7276 616e 7473 da0c 6e5f  n_observants..n_
+000019a0: 636f 6d70 6f6e 656e 7473 7273 0000 00da  componentsrs....
+000019b0: 0278 31da 0278 3272 4c00 0000 7211 0000  .x1..x2rL...r...
+000019c0: 0072 1100 0000 7212 0000 0072 1b00 0000  .r....r....r....
+000019d0: 9a00 0000 730a 0000 000c 020c 010e 010e  ....s...........
+000019e0: 0114 017a 0d4d 6978 4d4c 452e 7261 6e64  ...z.MixMLE.rand
+000019f0: 6f6d 6304 0000 0000 0000 0000 0000 0004  omc.............
+00001a00: 0000 0008 0000 0003 0000 0073 2800 0000  ...........s(...
+00001a10: 7400 a001 7400 a002 8700 6601 6401 6402  t...t.....f.d.d.
+00001a20: 8408 7403 7c00 6a04 7c02 8302 4400 8301  ..t.|.j.|...D...
+00001a30: 7c03 a102 a101 5300 2903 4e63 0100 0000  |.....S.).Nc....
+00001a40: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+00001a50: 1300 0000 731a 0000 0067 007c 005d 095c  ....s....g.|.].\
+00001a60: 027d 017d 027c 0188 007c 0283 0291 0271  .}.}.|...|.....q
+00001a70: 0253 0072 1100 0000 7211 0000 0029 0372  .S.r....r....).r
+00001a80: 4200 0000 726f 0000 00da 0274 69a9 0172  B...ro.....ti..r
+00001a90: 4c00 0000 7211 0000 0072 1200 0000 7245  L...r....r....rE
+00001aa0: 0000 00a3 0000 00f3 0200 0000 1a00 7a21  ..............z!
+00001ab0: 4d69 784d 4c45 2e6c 6f67 7064 662e 3c6c  MixMLE.logpdf.<l
+00001ac0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001ad0: 3e29 0572 0900 0000 da03 6c6f 67da 0364  >).r......log..d
+00001ae0: 6f74 7249 0000 0072 8000 0000 2904 7210  otrI...r....).r.
+00001af0: 0000 0072 4c00 0000 727a 0000 00da 0161  ...rL...rz.....a
+00001b00: 7211 0000 0072 8700 0000 7212 0000 0072  r....r....r....r
+00001b10: 6e00 0000 a200 0000 f302 0000 0028 017a  n............(.z
+00001b20: 0d4d 6978 4d4c 452e 6c6f 6770 6466 6303  .MixMLE.logpdfc.
+00001b30: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00001b40: 0000 0003 0000 0073 1e00 0000 7400 a001  .......s....t...
+00001b50: 8700 8701 8702 6603 6401 6402 8408 8801  ......f.d.d.....
+00001b60: 6a02 4400 8301 a101 5300 2903 4e63 0100  j.D.....S.).Nc..
+00001b70: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00001b80: 0000 1300 0000 731a 0000 0067 007c 005d  ......s....g.|.]
+00001b90: 097d 0188 01a0 007c 0188 0288 00a1 0391  .}.....|........
+00001ba0: 0271 0253 0072 1100 0000 7277 0000 0072  .q.S.r....rw...r
+00001bb0: 7800 0000 a903 728b 0000 0072 1000 0000  x.....r....r....
+00001bc0: 727a 0000 0072 1100 0000 7212 0000 0072  rz...r....r....r
+00001bd0: 4500 0000 a700 0000 7288 0000 007a 234d  E.......r....z#M
+00001be0: 6978 4d4c 452e 5f5f 6361 6c6c 5f5f 2e3c  ixMLE.__call__.<
+00001bf0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001c00: 703e 727b 0000 0029 0372 1000 0000 727a  p>r{...).r....rz
+00001c10: 0000 0072 8b00 0000 7211 0000 0072 8d00  ...r....r....r..
+00001c20: 0000 7212 0000 0072 4e00 0000 a500 0000  ..r....rN.......
+00001c30: 7302 0000 001e 027a 0f4d 6978 4d4c 452e  s......z.MixMLE.
+00001c40: 5f5f 6361 6c6c 5f5f 4e29 0272 7100 0000  __call__N).rq...
+00001c50: 7202 0000 0029 0872 5000 0000 7251 0000  r....).rP...rQ..
+00001c60: 0072 5200 0000 7213 0000 0072 5500 0000  .rR...r....rU...
+00001c70: 721b 0000 0072 6e00 0000 724e 0000 0072  r....rn...rN...r
+00001c80: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00001c90: 0000 0072 7d00 0000 9300 0000 730c 0000  ...r}.......s...
+00001ca0: 0008 0008 0302 040c 0108 070c 0372 7d00  .............r}.
+00001cb0: 0000 2902 da05 7064 6973 74da 0a73 7175  ..)...pdist..squ
+00001cc0: 6172 6566 6f72 6d63 0000 0000 0000 0000  areformc........
+00001cd0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00001ce0: 7328 0000 0065 005a 0164 005a 0264 0164  s(...e.Z.d.Z.d.d
+00001cf0: 0284 005a 0365 0464 0364 0484 0083 015a  ...Z.e.d.d.....Z
+00001d00: 0564 0564 0684 005a 0664 0753 0029 08da  .d.d...Z.d.S.)..
+00001d10: 0c53 686f 7274 6573 7450 6174 6863 0200  .ShortestPathc..
+00001d20: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001d30: 0000 4300 0000 7318 0000 007c 017c 005f  ..C...s....|.|._
+00001d40: 0074 0174 027c 0183 0183 017c 005f 0364  .t.t.|.....|._.d
+00001d50: 0153 0029 027a 6d54 5350 0a20 2020 2020  .S.).zmTSP.     
+00001d60: 2020 200a 2020 2020 2020 2020 4172 6775     .        Argu
+00001d70: 6d65 6e74 733a 0a20 2020 2020 2020 2020  ments:.         
+00001d80: 2020 2070 6f69 6e74 7320 7b61 7272 6179     points {array
+00001d90: 2077 6974 6820 7368 6170 6520 6f66 204e   with shape of N
+00001da0: 202a 2032 7d20 2d2d 2070 6f69 6e74 7320   * 2} -- points 
+00001db0: 6f66 2074 6865 2070 6174 680a 2020 2020  of the path.    
+00001dc0: 2020 2020 4e29 04da 0670 6f69 6e74 7372      N)...pointsr
+00001dd0: 8f00 0000 728e 0000 00da 035f 646d 2902  ....r......_dm).
+00001de0: 7210 0000 0072 9100 0000 7211 0000 0072  r....r....r....r
+00001df0: 1100 0000 7212 0000 0072 1300 0000 ad00  ....r....r......
+00001e00: 0000 7304 0000 0006 0612 017a 1553 686f  ..s........z.Sho
+00001e10: 7274 6573 7450 6174 682e 5f5f 696e 6974  rtestPath.__init
+00001e20: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00001e30: 0000 0004 0000 0043 0000 0073 1600 0000  .......C...s....
+00001e40: 7400 7401 6a02 6a02 7c00 6401 6602 6402  t.t.j.j.|.d.f.d.
+00001e50: 8d01 8301 5300 2903 4e72 0200 0000 7274  ....S.).Nr....rt
+00001e60: 0000 0029 0372 9000 0000 7209 0000 0072  ...).r....r....r
+00001e70: 1b00 0000 2901 da01 4e72 1100 0000 7211  ....)...Nr....r.
+00001e80: 0000 0072 1200 0000 721b 0000 00b6 0000  ...r....r.......
+00001e90: 0073 0200 0000 1602 7a13 5368 6f72 7465  .s......z.Shorte
+00001ea0: 7374 5061 7468 2e72 616e 646f 6d63 0200  stPath.randomc..
+00001eb0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+00001ec0: 0000 0300 0000 732e 0000 0074 00a0 0187  ......s....t....
+00001ed0: 0066 0164 0164 0284 0874 027c 0164 0064  .f.d.d...t.|.d.d
+00001ee0: 0385 0219 007c 0164 0464 0085 0219 0083  .....|.d.d......
+00001ef0: 0244 0083 01a1 0153 0029 054e 6301 0000  .D.....S.).Nc...
+00001f00: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00001f10: 0013 0000 0073 3400 0000 6700 7c00 5d16  .....s4...g.|.].
+00001f20: 5c02 7d01 7d02 7c01 7c02 6b00 7211 8800  \.}.}.|.|.k.r...
+00001f30: 6a00 7c01 7c02 6602 1900 6e06 8800 6a00  j.|.|.f...n...j.
+00001f40: 7c02 7c01 6602 1900 9102 7102 5300 7211  |.|.f.....q.S.r.
+00001f50: 0000 0029 0172 9200 0000 2903 7242 0000  ...).r....).rB..
+00001f60: 0072 4300 0000 da01 6a72 1600 0000 7211  .rC.....jr....r.
+00001f70: 0000 0072 1200 0000 7245 0000 00bb 0000  ...r....rE......
+00001f80: 0073 0200 0000 3400 7a29 5368 6f72 7465  .s....4.z)Shorte
+00001f90: 7374 5061 7468 2e5f 5f63 616c 6c5f 5f2e  stPath.__call__.
+00001fa0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001fb0: 6d70 3e72 4800 0000 7208 0000 0029 0372  mp>rH...r....).r
+00001fc0: 0900 0000 720a 0000 0072 4900 0000 a902  ....r....rI.....
+00001fd0: 7210 0000 0072 4c00 0000 7211 0000 0072  r....rL...r....r
+00001fe0: 1600 0000 7212 0000 0072 4e00 0000 ba00  ....r....rN.....
+00001ff0: 0000 7302 0000 002e 017a 1553 686f 7274  ..s......z.Short
+00002000: 6573 7450 6174 682e 5f5f 6361 6c6c 5f5f  estPath.__call__
+00002010: 4e72 7c00 0000 7211 0000 0072 1100 0000  Nr|...r....r....
+00002020: 7211 0000 0072 1200 0000 7290 0000 00ac  r....r....r.....
+00002030: 0000 0073 0a00 0000 0800 0801 0209 0a01  ...s............
+00002040: 0c03 7290 0000 0063 0000 0000 0000 0000  ..r....c........
+00002050: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00002060: 731c 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
+00002070: 0164 0164 0284 085a 0387 0004 005a 0453  .d.d...Z.....Z.S
+00002080: 0029 03da 0943 7572 7665 5061 7468 6303  .)...CurvePathc.
+00002090: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+000020a0: 0000 0003 0000 0073 1e00 0000 7400 a001  .......s....t...
+000020b0: 7c01 7c02 6702 a101 7d03 7402 8300 a003  |.|.g...}.t.....
+000020c0: 7c03 a101 0100 6400 5300 7214 0000 0029  |.....d.S.r....)
+000020d0: 0472 0900 0000 da0c 636f 6c75 6d6e 5f73  .r......column_s
+000020e0: 7461 636b da05 7375 7065 7272 1300 0000  tack..superr....
+000020f0: 2904 7210 0000 0072 4c00 0000 da01 79da  ).r....rL.....y.
+00002100: 075f 706f 696e 7473 a901 da09 5f5f 636c  ._points....__cl
+00002110: 6173 735f 5f72 1100 0000 7212 0000 0072  ass__r....r....r
+00002120: 1300 0000 bf00 0000 7304 0000 000e 0110  ........s.......
+00002130: 017a 1243 7572 7665 5061 7468 2e5f 5f69  .z.CurvePath.__i
+00002140: 6e69 745f 5f29 0572 5000 0000 7251 0000  nit__).rP...rQ..
+00002150: 0072 5200 0000 7213 0000 00da 0d5f 5f63  .rR...r......__c
+00002160: 6c61 7373 6365 6c6c 5f5f 7211 0000 0072  lasscell__r....r
+00002170: 1100 0000 729b 0000 0072 1200 0000 7296  ....r....r....r.
+00002180: 0000 00be 0000 0073 0400 0000 0800 1401  .......s........
+00002190: 7296 0000 0072 0800 0000 6302 0000 0000  r....r....c.....
+000021a0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+000021b0: 0000 0073 3400 0000 7400 a001 7c00 a101  ...s4...t...|...
+000021c0: 7d02 7400 a002 7c00 a101 7400 a003 7c02  }.t...|...t...|.
+000021d0: 6401 1300 6402 a102 1700 7d03 7c01 7c02  d...d.....}.|.|.
+000021e0: 1400 7c01 7c03 1400 6602 5300 2903 4e72  ..|.|...f.S.).Nr
+000021f0: 0200 0000 6755 5555 5555 55d5 3f29 0472  ....gUUUUUU.?).r
+00002200: 0900 0000 da03 636f 73da 0373 696e da05  ......cos..sin..
+00002210: 706f 7765 7229 0472 7a00 0000 728b 0000  power).rz...r...
+00002220: 0072 4c00 0000 7299 0000 0072 1100 0000  .rL...r....r....
+00002230: 7211 0000 0072 1200 0000 da06 5f68 6561  r....r......_hea
+00002240: 7274 c400 0000 7306 0000 000a 011a 0110  rt....s.........
+00002250: 0172 a100 0000 7218 0000 0067 cdcc cccc  .r....r....g....
+00002260: cccc f43f 2901 728b 0000 0063 0000 0000  ...?).r....c....
+00002270: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00002280: 4000 0000 7322 0000 0065 005a 0164 005a  @...s"...e.Z.d.Z
+00002290: 0267 0064 0166 0264 0264 0384 015a 0364  .g.d.f.d.d...Z.d
+000022a0: 0464 0584 005a 0464 0153 0029 06da 0f4d  .d...Z.d.S.)...M
+000022b0: 696e 5370 616e 6e69 6e67 5472 6565 4e63  inSpanningTreeNc
+000022c0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+000022d0: 0200 0000 4300 0000 7316 0000 007c 017c  ....C...s....|.|
+000022e0: 005f 007c 027c 005f 017c 037c 005f 0264  ._.|.|._.|.|._.d
+000022f0: 0053 0072 1400 0000 2903 da05 6e6f 6465  .S.r....)...node
+00002300: 73da 0565 6467 6573 da07 7765 6967 6874  s..edges..weight
+00002310: 7329 0472 1000 0000 72a3 0000 0072 a400  s).r....r....r..
+00002320: 0000 72a5 0000 0072 1100 0000 7211 0000  ..r....r....r...
+00002330: 0072 1200 0000 7213 0000 00d2 0000 0073  .r....r........s
+00002340: 0600 0000 0601 0601 0a01 7a18 4d69 6e53  ..........z.MinS
+00002350: 7061 6e6e 696e 6754 7265 652e 5f5f 696e  panningTree.__in
+00002360: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
+00002370: 0003 0000 0004 0000 0003 0000 0073 2200  .............s".
+00002380: 0000 7400 7c01 8800 6a01 8302 7d02 7402  ..t.|...j...}.t.
+00002390: 8700 6601 6401 6402 8408 7c02 4400 8301  ..f.d.d...|.D...
+000023a0: 8301 5300 2903 4e63 0100 0000 0000 0000  ..S.).Nc........
+000023b0: 0000 0000 0200 0000 0300 0000 3300 0000  ............3...
+000023c0: 731a 0000 0081 007c 005d 087d 0188 006a  s......|.].}...j
+000023d0: 007c 0119 0056 0001 0071 0264 0053 0072  .|...V...q.d.S.r
+000023e0: 1400 0000 2901 72a5 0000 0029 0272 4200  ....).r....).rB.
+000023f0: 0000 da04 6564 6765 7216 0000 0072 1100  ....edger....r..
+00002400: 0000 7212 0000 0072 6500 0000 d900 0000  ..r....re.......
+00002410: 7304 0000 0002 8018 007a 2b4d 696e 5370  s........z+MinSp
+00002420: 616e 6e69 6e67 5472 6565 2e5f 5f63 616c  anningTree.__cal
+00002430: 6c5f 5f2e 3c6c 6f63 616c 733e 2e3c 6765  l__.<locals>.<ge
+00002440: 6e65 7870 723e 2903 7203 0000 0072 a300  nexpr>).r....r..
+00002450: 0000 720a 0000 0029 0372 1000 0000 724c  ..r....).r....rL
+00002460: 0000 0072 a400 0000 7211 0000 0072 1600  ...r....r....r..
+00002470: 0000 7212 0000 0072 4e00 0000 d700 0000  ..r....rN.......
+00002480: 7304 0000 000c 0116 017a 184d 696e 5370  s........z.MinSp
+00002490: 616e 6e69 6e67 5472 6565 2e5f 5f63 616c  anningTree.__cal
+000024a0: 6c5f 5f29 0572 5000 0000 7251 0000 0072  l__).rP...rQ...r
+000024b0: 5200 0000 7213 0000 0072 4e00 0000 7211  R...r....rN...r.
+000024c0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+000024d0: 0000 72a2 0000 00d1 0000 0073 0600 0000  ..r........s....
+000024e0: 0800 0e01 0c05 72a2 0000 0063 0000 0000  ......r....c....
+000024f0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00002500: 4000 0000 732c 0000 0065 005a 0164 005a  @...s,...e.Z.d.Z
+00002510: 0264 015a 0364 0264 0384 005a 0465 0564  .d.Z.d.d...Z.e.d
+00002520: 0464 0584 0083 015a 0664 0664 0784 005a  .d.....Z.d.d...Z
+00002530: 0764 0853 0029 09da 0e46 6163 696c 6974  .d.S.)...Facilit
+00002540: 794c 6179 6f75 747a 170a 2020 2020 463a  yLayoutz..    F:
+00002550: 2046 0a20 2020 2044 3a20 440a 2020 2020   F.    D: D.    
+00002560: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00002570: 0002 0000 0043 0000 0072 7e00 0000 7214  .....C...r~...r.
+00002580: 0000 0029 02da 0146 da01 4429 0372 1000  ...)...F..D).r..
+00002590: 0000 72a8 0000 0072 a900 0000 7211 0000  ..r....r....r...
+000025a0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000025b0: e200 0000 7270 0000 007a 1746 6163 696c  ....rp...z.Facil
+000025c0: 6974 794c 6179 6f75 742e 5f5f 696e 6974  ityLayout.__init
+000025d0: 5f5f 6302 0000 0000 0000 0000 0000 0004  __c.............
+000025e0: 0000 0003 0000 0043 0000 0073 2e00 0000  .......C...s....
+000025f0: 7400 6a01 6a01 7c01 7c01 6602 6401 8d01  t.j.j.|.|.f.d...
+00002600: 7d02 7400 6a01 6a01 7c01 7c01 6602 6401  }.t.j.j.|.|.f.d.
+00002610: 8d01 7d03 7402 7c02 7c03 8302 5300 2902  ..}.t.|.|...S.).
+00002620: 4e72 7400 0000 2903 7209 0000 0072 1b00  Nrt...).r....r..
+00002630: 0000 72a7 0000 0029 0472 1000 0000 7264  ..r....).r....rd
+00002640: 0000 0072 a800 0000 72a9 0000 0072 1100  ...r....r....r..
+00002650: 0000 7211 0000 0072 1200 0000 721b 0000  ..r....r....r...
+00002660: 00e6 0000 0073 0600 0000 1202 1201 0a01  .....s..........
+00002670: 7a15 4661 6369 6c69 7479 4c61 796f 7574  z.FacilityLayout
+00002680: 2e72 616e 646f 6d63 0200 0000 0000 0000  .randomc........
+00002690: 0000 0000 0200 0000 0800 0000 0300 0000  ................
+000026a0: 7328 0000 0074 00a0 0188 006a 02a0 03a1  s(...t.....j....
+000026b0: 0074 00a0 0487 0087 0166 0264 0164 0284  .t.......f.d.d..
+000026c0: 0888 0144 0083 01a1 01a1 0253 0029 034e  ...D.......S.).N
+000026d0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000026e0: 0006 0000 0013 0000 0073 2400 0000 6700  .........s$...g.
+000026f0: 7c00 5d0e 7d01 8801 4400 5d09 7d02 8800  |.].}...D.].}...
+00002700: 6a00 7c02 7c01 6602 1900 9103 7106 7102  j.|.|.f.....q.q.
+00002710: 5300 7211 0000 0029 0172 a900 0000 2903  S.r....).r....).
+00002720: 7242 0000 00da 0278 6a72 6800 0000 7295  rB.....xjrh...r.
+00002730: 0000 0072 1100 0000 7212 0000 0072 4500  ...r....r....rE.
+00002740: 0000 ed00 0000 7302 0000 0024 007a 2b46  ......s....$.z+F
+00002750: 6163 696c 6974 794c 6179 6f75 742e 5f5f  acilityLayout.__
+00002760: 6361 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e  call__.<locals>.
+00002770: 3c6c 6973 7463 6f6d 703e 2905 7209 0000  <listcomp>).r...
+00002780: 0072 8a00 0000 72a8 0000 00da 0572 6176  .r....r......rav
+00002790: 656c da05 6172 7261 7972 9500 0000 7211  el..arrayr....r.
+000027a0: 0000 0072 9500 0000 7212 0000 0072 4e00  ...r....r....rN.
+000027b0: 0000 ec00 0000 728c 0000 007a 1746 6163  ......r....z.Fac
+000027c0: 696c 6974 794c 6179 6f75 742e 5f5f 6361  ilityLayout.__ca
+000027d0: 6c6c 5f5f 4e29 0872 5000 0000 7251 0000  ll__N).rP...rQ..
+000027e0: 0072 5200 0000 7253 0000 0072 1300 0000  .rR...rS...r....
+000027f0: 7255 0000 0072 1b00 0000 724e 0000 0072  rU...r....rN...r
+00002800: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00002810: 0000 0072 a700 0000 dc00 0000 730c 0000  ...r........s...
+00002820: 0008 0004 0108 0502 040a 010c 0572 a700  .............r..
+00002830: 0000 7241 0000 0029 1dda 056e 756d 7079  ..rA...)...numpy
+00002840: 7209 0000 00da 0575 7469 6c73 7203 0000  r......utilsr...
+00002850: 00da 0a62 656e 6368 6d61 726b 7372 0400  ...benchmarksr..
+00002860: 0000 7205 0000 0072 5600 0000 726d 0000  ..r....rV...rm..
+00002870: 0072 7d00 0000 da16 7363 6970 792e 7370  .r}.....scipy.sp
+00002880: 6174 6961 6c2e 6469 7374 616e 6365 728e  atial.distancer.
+00002890: 0000 0072 8f00 0000 7290 0000 0072 9600  ...r....r....r..
+000028a0: 0000 72a1 0000 00da 086c 696e 7370 6163  ..r......linspac
+000028b0: 65da 0270 6972 7a00 0000 7284 0000 00da  e..pirz...r.....
+000028c0: 0279 3172 8500 0000 da02 7932 7282 0000  .y1r......y2r...
+000028d0: 0072 4c00 0000 7299 0000 005a 0a68 6561  .rL...r....Z.hea
+000028e0: 7274 5f70 6174 6872 a200 0000 72a7 0000  rt_pathr....r...
+000028f0: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+00002900: 7212 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00002910: 0000 0073 2600 0000 0802 0c02 0c01 1003  ...s&...........
+00002920: 1044 1035 1011 1017 1002 1012 0a06 1405  .D.5............
+00002930: 0c01 1001 0e01 0e01 0a01 1003 140b       ..............
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/optimization.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/others.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/others.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan  2 05:02:39 2024 UTC, .py size: 382 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-00000000: 6f0d 0d0a 0000 0000 ef98 9365 7e01 0000  o..........e~...
+00000000: 6f0d 0d0a 0000 0000 8b9f 6d65 7101 0000  o.........meq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a01 6402 6403 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6404 6405 8400 6405 6503 8303  ..G.d.d...d.e...
 00000050: 5a04 6401 5300 2906 e900 0000 004e e902  Z.d.S.)......N..
-00000060: 0000 0029 01da 0b42 6173 6550 726f 626c  ...)...BaseProbl
-00000070: 656d 6300 0000 0000 0000 0000 0000 0000  emc.............
-00000080: 0000 0003 0000 0040 0000 0073 2200 0000  .......@...s"...
-00000090: 6500 5a01 6400 5a02 6401 5a03 6409 6404  e.Z.d.Z.d.Z.d.d.
-000000a0: 6405 8401 5a04 6406 6407 8400 5a05 6408  d...Z.d.d...Z.d.
-000000b0: 5300 290a da0b 4b61 6e74 6f72 6f76 6963  S.)...Kantorovic
-000000c0: 687a 170a 2020 2020 613a 2061 0a20 2020  hz..    a: a.   
-000000d0: 2062 3a20 620a 2020 2020 e700 0000 0000   b: b.    ......
-000000e0: 00e0 3fe9 0100 0000 6303 0000 0000 0000  ..?.....c.......
-000000f0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00000100: 0073 2000 0000 7c01 7c00 5f00 7c02 7c00  .s ...|.|._.|.|.
-00000110: 5f01 7402 a003 7c01 7c02 6401 a103 7c00  _.t...|.|.d...|.
-00000120: 5f04 6400 5300 2902 4ee9 6400 0000 2905  _.d.S.).N.d...).
-00000130: da01 61da 0162 da02 6e70 da08 6c69 6e73  ..a..b..np..lins
-00000140: 7061 6365 da01 7829 03da 0473 656c 6672  pace..x)...selfr
-00000150: 0800 0000 7209 0000 00a9 0072 0e00 0000  ....r......r....
-00000160: fa56 2f55 7365 7273 2f77 696c 6c69 616d  .V/Users/william
-00000170: 2f50 726f 6772 616d 6d69 6e67 2f6d 7947  /Programming/myG
-00000180: 6974 6875 622f 7079 7269 6d69 6469 6e65  ithub/pyrimidine
-00000190: 2f64 6f63 732f 2e2e 2f70 7972 696d 6964  /docs/../pyrimid
-000001a0: 696e 652f 6265 6e63 686d 6172 6b73 2f6f  ine/benchmarks/o
-000001b0: 7468 6572 732e 7079 da08 5f5f 696e 6974  thers.py..__init
-000001c0: 5f5f 0e00 0000 7306 0000 0006 0106 0114  __....s.........
-000001d0: 017a 144b 616e 746f 726f 7669 6368 2e5f  .z.Kantorovich._
-000001e0: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
-000001f0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00000200: 7320 0000 0074 00a0 017c 006a 027c 01a1  s ...t...|.j.|..
-00000210: 0274 00a0 0164 017c 006a 021b 007c 01a1  .t...d.|.j...|..
-00000220: 0214 0053 0029 024e 7206 0000 0029 0372  ...S.).Nr....).r
-00000230: 0a00 0000 da03 646f 7472 0c00 0000 2902  ......dotr....).
-00000240: 720d 0000 00da 0170 720e 0000 0072 0e00  r......pr....r..
-00000250: 0000 720f 0000 00da 085f 5f63 616c 6c5f  ..r......__call_
-00000260: 5f13 0000 0073 0200 0000 2002 7a14 4b61  _....s.... .z.Ka
-00000270: 6e74 6f72 6f76 6963 682e 5f5f 6361 6c6c  ntorovich.__call
-00000280: 5f5f 4e29 0272 0500 0000 7206 0000 0029  __N).r....r....)
-00000290: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000002a0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000002b0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7210  ame__..__doc__r.
-000002c0: 0000 0072 1300 0000 720e 0000 0072 0e00  ...r....r....r..
-000002d0: 0000 720e 0000 0072 0f00 0000 7204 0000  ..r....r....r...
-000002e0: 0008 0000 0073 0800 0000 0800 0401 0a05  .....s..........
-000002f0: 0c05 7204 0000 0029 05da 056e 756d 7079  ..r....)...numpy
-00000300: 720a 0000 00da 0a62 656e 6368 6d61 726b  r......benchmark
-00000310: 7372 0300 0000 7204 0000 0072 0e00 0000  sr....r....r....
-00000320: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000330: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-00000340: 0000 0802 0c02 1403                      ........
+00000060: 0000 0029 01da 0750 726f 626c 656d 6300  ...)...Problemc.
+00000070: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000080: 0000 0040 0000 0073 2200 0000 6500 5a01  ...@...s"...e.Z.
+00000090: 6400 5a02 6401 5a03 6409 6404 6405 8401  d.Z.d.Z.d.d.d...
+000000a0: 5a04 6406 6407 8400 5a05 6408 5300 290a  Z.d.d...Z.d.S.).
+000000b0: da0b 4b61 6e74 6f72 6f76 6963 687a 170a  ..Kantorovichz..
+000000c0: 2020 2020 613a 2061 0a20 2020 2062 3a20      a: a.    b: 
+000000d0: 620a 2020 2020 e700 0000 0000 00e0 3fe9  b.    ........?.
+000000e0: 0100 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000000f0: 0003 0000 0005 0000 0043 0000 0073 2000  .........C...s .
+00000100: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7402  ..|.|._.|.|._.t.
+00000110: a003 7c01 7c02 6401 a103 7c00 5f04 6400  ..|.|.d...|._.d.
+00000120: 5300 2902 4ee9 6400 0000 2905 da01 61da  S.).N.d...)...a.
+00000130: 0162 da02 6e70 da08 6c69 6e73 7061 6365  .b..np..linspace
+00000140: da01 7829 03da 0473 656c 6672 0800 0000  ..x)...selfr....
+00000150: 7209 0000 00a9 0072 0e00 0000 fa48 2f55  r......r.....H/U
+00000160: 7365 7273 2f77 696c 6c69 616d 2f50 726f  sers/william/Pro
+00000170: 6772 616d 6d69 6e67 2f50 7974 686f 6e2f  gramming/Python/
+00000180: 6d79 776f 726b 2f70 7972 696d 6964 696e  mywork/pyrimidin
+00000190: 652f 6265 6e63 686d 6172 6b73 2f6f 7468  e/benchmarks/oth
+000001a0: 6572 732e 7079 da08 5f5f 696e 6974 5f5f  ers.py..__init__
+000001b0: 0d00 0000 7306 0000 0006 0106 0114 017a  ....s..........z
+000001c0: 144b 616e 746f 726f 7669 6368 2e5f 5f69  .Kantorovich.__i
+000001d0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+000001e0: 0000 0200 0000 0500 0000 4300 0000 7320  ..........C...s 
+000001f0: 0000 0074 00a0 017c 006a 027c 01a1 0274  ...t...|.j.|...t
+00000200: 00a0 0164 017c 006a 021b 007c 01a1 0214  ...d.|.j...|....
+00000210: 0053 0029 024e 7206 0000 0029 0372 0a00  .S.).Nr....).r..
+00000220: 0000 da03 646f 7472 0c00 0000 2902 720d  ....dotr....).r.
+00000230: 0000 00da 0170 720e 0000 0072 0e00 0000  .....pr....r....
+00000240: 720f 0000 00da 085f 5f63 616c 6c5f 5f12  r......__call__.
+00000250: 0000 0073 0200 0000 2002 7a14 4b61 6e74  ...s.... .z.Kant
+00000260: 6f72 6f76 6963 682e 5f5f 6361 6c6c 5f5f  orovich.__call__
+00000270: 4e29 0272 0500 0000 7206 0000 0029 06da  N).r....r....)..
+00000280: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000290: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000002a0: 655f 5fda 075f 5f64 6f63 5f5f 7210 0000  e__..__doc__r...
+000002b0: 0072 1300 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000002c0: 720e 0000 0072 0f00 0000 7204 0000 0008  r....r....r.....
+000002d0: 0000 0073 0800 0000 0800 0401 0a04 0c05  ...s............
+000002e0: 7204 0000 0029 05da 056e 756d 7079 720a  r....)...numpyr.
+000002f0: 0000 00da 0a62 656e 6368 6d61 726b 7372  .....benchmarksr
+00000300: 0300 0000 7204 0000 0072 0e00 0000 720e  ....r....r....r.
+00000310: 0000 0072 0e00 0000 720f 0000 00da 083c  ...r....r......<
+00000320: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
+00000330: 0802 0c02 1403                           ......
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/others.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/others.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/special.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/special.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 957 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 bd03 0000  o.........ne....
+00000000: 6f0d 0d0a 0000 0000 b6bd 6d65 bd03 0000  o.........me....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 5a06 6404  m.Z...d.d.l.Z.d.
 00000050: 6506 6a07 6602 6405 6406 8404 5a08 6404  e.j.f.d.d...Z.d.
 00000060: 6506 6a07 6602 6407 6408 8404 5a09 6404  e.j.f.d.d...Z.d.
 00000070: 6506 6a07 6602 6409 640a 8404 5a0a 6414  e.j.f.d.d...Z.d.
@@ -18,112 +18,112 @@
 00000110: 00a0 0264 017c 0064 0264 0085 0219 007c  ...d.|.d.d.....|
 00000120: 0064 0064 0385 0219 0064 0413 0018 0064  .d.d.....d.....d
 00000130: 0413 0014 007c 0064 0064 0385 0219 0017  .....|.d.d......
 00000140: 0064 0218 0064 0413 00a1 0153 0029 054e  .d...d.....S.).N
 00000150: e964 0000 00e9 0100 0000 e9ff ffff ffe9  .d..............
 00000160: 0200 0000 2903 da02 6e70 da07 6173 6172  ....)...np..asar
 00000170: 7261 79da 0373 756d a901 7205 0000 00a9  ray..sum..r.....
-00000180: 0072 0e00 0000 fa4f 2f55 7365 7273 2f77  .r.....O/Users/w
+00000180: 0072 0e00 0000 fa49 2f55 7365 7273 2f77  .r.....I/Users/w
 00000190: 696c 6c69 616d 2f50 726f 6772 616d 6d69  illiam/Programmi
-000001a0: 6e67 2f6d 7947 6974 6875 622f 7079 7269  ng/myGithub/pyri
-000001b0: 6d69 6469 6e65 2f70 7972 696d 6964 696e  midine/pyrimidin
-000001c0: 652f 6265 6e63 686d 6172 6b73 2f73 7065  e/benchmarks/spe
-000001d0: 6369 616c 2e70 79da 0a72 6f73 656e 6272  cial.py..rosenbr
-000001e0: 6f63 6b0a 0000 0073 0400 0000 0a01 3e01  ock....s......>.
-000001f0: 7210 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000200: 0000 0200 0000 0500 0000 4300 0000 7336  ..........C...s6
-00000210: 0000 0074 00a0 017c 0064 0113 00a1 017d  ...t...|.d.....}
-00000220: 0174 0274 037c 0183 0183 0164 0113 0064  .t.t.|.....d...d
-00000230: 0218 0064 0364 047c 0164 0113 0014 0017  ...d.d.|.d......
-00000240: 0064 0113 001b 0053 0029 054e 7209 0000  .d.....S.).Nr...
-00000250: 0067 0000 0000 0000 e03f 7207 0000 0067  .g.......?r....g
-00000260: fca9 f1d2 4d62 503f 2904 720a 0000 0072  ....MbP?).r....r
-00000270: 0c00 0000 7202 0000 0072 0300 0000 2902  ....r....r....).
-00000280: 7205 0000 00da 0272 3272 0e00 0000 720e  r......r2r....r.
-00000290: 0000 0072 0f00 0000 da08 7363 6861 6666  ...r......schaff
-000002a0: 6572 0f00 0000 7304 0000 000e 0128 0172  er....s......(.r
-000002b0: 1200 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000002c0: 0001 0000 0008 0000 0043 0000 0073 2800  .........C...s(.
-000002d0: 0000 7400 a001 7c00 6401 1300 6402 7400  ..t...|.d...d.t.
-000002e0: a002 6401 7403 1400 7c00 1400 a101 1400  ..d.t...|.......
-000002f0: 1800 a101 6403 1700 5300 2904 4e72 0900  ....d...S.).Nr..
-00000300: 0000 e90a 0000 00e9 2800 0000 2904 720a  ........(...).r.
-00000310: 0000 0072 0c00 0000 da03 636f 7372 0400  ...r......cosr..
-00000320: 0000 720d 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-00000330: 0072 0f00 0000 da0a 7261 7374 7269 6772  .r......rastrigr
-00000340: 696e 1300 0000 7302 0000 0028 0172 1600  in....s....(.r..
-00000350: 0000 e905 0000 0063 0100 0000 0000 0000  .......c........
-00000360: 0000 0000 0200 0000 0400 0000 0300 0000  ................
-00000370: f318 0000 0064 0174 006a 0166 0287 0066  .....d.t.j.f...f
-00000380: 0164 0264 0384 0c7d 017c 0153 0029 044e  .d.d...}.|.S.).N
-00000390: 7205 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000003a0: 0000 0100 0000 0d00 0000 1300 0000 7338  ..............s8
-000003b0: 0000 0074 00a0 017c 0064 0113 00a1 0164  ...t...|.d.....d
-000003c0: 021b 0074 00a0 0274 00a0 037c 0074 00a0  ...t...t...|.t..
-000003d0: 0474 00a0 0564 0388 0064 0317 00a1 02a1  .t...d...d......
-000003e0: 011b 00a1 01a1 0118 0053 0029 044e 7209  .........S.).Nr.
-000003f0: 0000 00e9 a00f 0000 7207 0000 0029 0672  ........r....).r
-00000400: 0a00 0000 720c 0000 00da 0470 726f 6472  ....r......prodr
-00000410: 1500 0000 7203 0000 00da 0661 7261 6e67  ....r......arang
-00000420: 6572 0d00 0000 a901 da01 6e72 0e00 0000  er........nr....
-00000430: 720f 0000 00da 0166 1800 0000 7302 0000  r......f....s...
-00000440: 0038 017a 1467 7269 6577 616e 676b 2e3c  .8.z.griewangk.<
-00000450: 6c6f 6361 6c73 3e2e 66a9 0272 0a00 0000  locals>.f..r....
-00000460: da07 6e64 6172 7261 79a9 0272 1d00 0000  ..ndarray..r....
-00000470: 721e 0000 0072 0e00 0000 721c 0000 0072  r....r....r....r
-00000480: 0f00 0000 da09 6772 6965 7761 6e67 6b17  ......griewangk.
-00000490: 0000 00f3 0400 0000 1401 0402 7222 0000  ............r"..
-000004a0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000004b0: 0000 0400 0000 0300 0000 7218 0000 0029  ..........r....)
-000004c0: 044e 7205 0000 0063 0100 0000 0000 0000  .Nr....c........
-000004d0: 0000 0000 0100 0000 0800 0000 1300 0000  ................
-000004e0: 7336 0000 0074 0074 017c 0083 0174 0174  s6...t.t.|...t.t
-000004f0: 02a0 0364 0188 0064 0117 00a1 027c 0064  ...d...d.....|.d
-00000500: 0213 0014 0074 041b 0083 0164 0313 0014  .....t.....d....
-00000510: 0083 010b 0064 041b 0053 0029 054e 7207  .....d...S.).Nr.
-00000520: 0000 0072 0900 0000 e914 0000 0072 1900  ...r.........r..
-00000530: 0000 2905 720c 0000 0072 0200 0000 720a  ..).r....r....r.
-00000540: 0000 0072 1b00 0000 7204 0000 0072 0d00  ...r....r....r..
-00000550: 0000 721c 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000560: 0072 1e00 0000 1e00 0000 7302 0000 0036  .r........s....6
-00000570: 017a 166d 6963 6861 6c65 7769 657a 2e3c  .z.michalewiez.<
-00000580: 6c6f 6361 6c73 3e2e 6672 1f00 0000 7221  locals>.fr....r!
-00000590: 0000 0072 0e00 0000 721c 0000 0072 0f00  ...r....r....r..
-000005a0: 0000 da0b 6d69 6368 616c 6577 6965 7a1d  ....michalewiez.
-000005b0: 0000 0072 2300 0000 7225 0000 0063 0100  ...r#...r%...c..
-000005c0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000005d0: 0000 0300 0000 7218 0000 0029 044e 7205  ......r....).Nr.
-000005e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000005f0: 0100 0000 0b00 0000 1300 0000 7362 0000  ............sb..
-00000600: 0074 00a0 0174 00a0 0264 0188 0064 0117  .t...t...d...d..
-00000610: 00a1 0274 00a0 0374 00a0 0288 00a1 01a1  ...t...t........
-00000620: 017c 0014 0064 0117 0014 00a1 0174 00a0  .|...d.......t..
-00000630: 0174 00a0 0264 0188 0064 0117 00a1 0274  .t...d...d.....t
-00000640: 00a0 0374 00a0 0264 0288 0064 0217 00a1  ...t...d...d....
-00000650: 02a1 017c 0014 0064 0117 0014 00a1 0114  ...|...d........
-00000660: 0053 0029 034e 7207 0000 0072 0900 0000  .S.).Nr....r....
-00000670: 2904 720a 0000 0072 0c00 0000 721b 0000  ).r....r....r...
-00000680: 0072 1500 0000 720d 0000 0072 1c00 0000  .r....r....r....
-00000690: 720e 0000 0072 0f00 0000 721e 0000 0024  r....r....r....$
-000006a0: 0000 0073 0200 0000 6201 7a11 6861 6e73  ...s....b.z.hans
-000006b0: 656e 2e3c 6c6f 6361 6c73 3e2e 6672 1f00  en.<locals>.fr..
-000006c0: 0000 7221 0000 0072 0e00 0000 721c 0000  ..r!...r....r...
-000006d0: 0072 0f00 0000 da06 6861 6e73 656e 2300  .r......hansen#.
-000006e0: 0000 7223 0000 0072 2600 0000 6301 0000  ..r#...r&...c...
-000006f0: 0000 0000 0000 0000 0001 0000 0007 0000  ................
-00000700: 0043 0000 0073 1e00 0000 7400 a001 7400  .C...s....t...t.
-00000710: a002 7400 a003 7c00 a101 6401 1700 7c00  ..t...|...d...|.
-00000720: 1400 a101 a101 5300 2902 4e67 9a99 9999  ......S.).Ng....
-00000730: 9999 b93f 2904 720a 0000 0072 0c00 0000  ...?).r....r....
-00000740: da03 6162 7372 0200 0000 720d 0000 0072  ..absr....r....r
-00000750: 0e00 0000 720e 0000 0072 0f00 0000 da06  ....r....r......
-00000760: 616c 7069 6e65 2900 0000 7302 0000 001e  alpine)...s.....
-00000770: 0172 2800 0000 2901 7217 0000 0029 0fda  .r(...).r....)..
-00000780: 075f 5f64 6f63 5f5f da04 6d61 7468 7202  .__doc__..mathr.
-00000790: 0000 0072 0300 0000 7204 0000 00da 056e  ...r....r......n
-000007a0: 756d 7079 720a 0000 0072 2000 0000 7210  umpyr....r ...r.
-000007b0: 0000 0072 1200 0000 7216 0000 0072 2200  ...r....r....r".
-000007c0: 0000 7225 0000 0072 2600 0000 7228 0000  ..r%...r&...r(..
-000007d0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-000007e0: 720f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000007f0: 0000 0073 1400 0000 0402 1404 0801 1002  ...s............
-00000800: 1005 1004 0a04 0a06 0a06 0c06            ............
+000001a0: 6e67 2f50 7974 686f 6e2f 6d79 776f 726b  ng/Python/mywork
+000001b0: 2f70 7972 696d 6964 696e 652f 6265 6e63  /pyrimidine/benc
+000001c0: 686d 6172 6b73 2f73 7065 6369 616c 2e70  hmarks/special.p
+000001d0: 79da 0a72 6f73 656e 6272 6f63 6b0a 0000  y..rosenbrock...
+000001e0: 0073 0400 0000 0a01 3e01 7210 0000 0063  .s......>.r....c
+000001f0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000200: 0500 0000 4300 0000 7336 0000 0074 00a0  ....C...s6...t..
+00000210: 017c 0064 0113 00a1 017d 0174 0274 037c  .|.d.....}.t.t.|
+00000220: 0183 0183 0164 0113 0064 0218 0064 0364  .....d...d...d.d
+00000230: 047c 0164 0113 0014 0017 0064 0113 001b  .|.d.......d....
+00000240: 0053 0029 054e 7209 0000 0067 0000 0000  .S.).Nr....g....
+00000250: 0000 e03f 7207 0000 0067 fca9 f1d2 4d62  ...?r....g....Mb
+00000260: 503f 2904 720a 0000 0072 0c00 0000 7202  P?).r....r....r.
+00000270: 0000 0072 0300 0000 2902 7205 0000 00da  ...r....).r.....
+00000280: 0272 3272 0e00 0000 720e 0000 0072 0f00  .r2r....r....r..
+00000290: 0000 da08 7363 6861 6666 6572 0f00 0000  ....schaffer....
+000002a0: 7304 0000 000e 0128 0172 1200 0000 6301  s......(.r....c.
+000002b0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
+000002c0: 0000 0043 0000 0073 2800 0000 7400 a001  ...C...s(...t...
+000002d0: 7c00 6401 1300 6402 7400 a002 6401 7403  |.d...d.t...d.t.
+000002e0: 1400 7c00 1400 a101 1400 1800 a101 6403  ..|...........d.
+000002f0: 1700 5300 2904 4e72 0900 0000 e90a 0000  ..S.).Nr........
+00000300: 00e9 2800 0000 2904 720a 0000 0072 0c00  ..(...).r....r..
+00000310: 0000 da03 636f 7372 0400 0000 720d 0000  ....cosr....r...
+00000320: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000330: da0a 7261 7374 7269 6772 696e 1400 0000  ..rastrigrin....
+00000340: 7302 0000 0028 0172 1600 0000 e905 0000  s....(.r........
+00000350: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000360: 0000 0400 0000 0300 0000 f318 0000 0064  ...............d
+00000370: 0174 006a 0166 0287 0066 0164 0264 0384  .t.j.f...f.d.d..
+00000380: 0c7d 017c 0153 0029 044e 7205 0000 0063  .}.|.S.).Nr....c
+00000390: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000003a0: 0d00 0000 1300 0000 7338 0000 0074 00a0  ........s8...t..
+000003b0: 017c 0064 0113 00a1 0164 021b 0074 00a0  .|.d.....d...t..
+000003c0: 0274 00a0 037c 0074 00a0 0474 00a0 0564  .t...|.t...t...d
+000003d0: 0388 0064 0317 00a1 02a1 011b 00a1 01a1  ...d............
+000003e0: 0118 0053 0029 044e 7209 0000 00e9 a00f  ...S.).Nr.......
+000003f0: 0000 7207 0000 0029 0672 0a00 0000 720c  ..r....).r....r.
+00000400: 0000 00da 0470 726f 6472 1500 0000 7203  .....prodr....r.
+00000410: 0000 00da 0661 7261 6e67 6572 0d00 0000  .....aranger....
+00000420: a901 da01 6e72 0e00 0000 720f 0000 00da  ....nr....r.....
+00000430: 0166 1900 0000 7302 0000 0038 017a 1467  .f....s....8.z.g
+00000440: 7269 6577 616e 676b 2e3c 6c6f 6361 6c73  riewangk.<locals
+00000450: 3e2e 66a9 0272 0a00 0000 da07 6e64 6172  >.f..r......ndar
+00000460: 7261 79a9 0272 1d00 0000 721e 0000 0072  ray..r....r....r
+00000470: 0e00 0000 721c 0000 0072 0f00 0000 da09  ....r....r......
+00000480: 6772 6965 7761 6e67 6b18 0000 00f3 0400  griewangk.......
+00000490: 0000 1401 0402 7222 0000 0063 0100 0000  ......r"...c....
+000004a0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000004b0: 0300 0000 7218 0000 0029 044e 7205 0000  ....r....).Nr...
+000004c0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+000004d0: 0000 0800 0000 1300 0000 7336 0000 0074  ..........s6...t
+000004e0: 0074 017c 0083 0174 0174 02a0 0364 0188  .t.|...t.t...d..
+000004f0: 0064 0117 00a1 027c 0064 0213 0014 0074  .d.....|.d.....t
+00000500: 041b 0083 0164 0313 0014 0083 010b 0064  .....d.........d
+00000510: 041b 0053 0029 054e 7207 0000 0072 0900  ...S.).Nr....r..
+00000520: 0000 e914 0000 0072 1900 0000 2905 720c  .......r....).r.
+00000530: 0000 0072 0200 0000 720a 0000 0072 1b00  ...r....r....r..
+00000540: 0000 7204 0000 0072 0d00 0000 721c 0000  ..r....r....r...
+00000550: 0072 0e00 0000 720f 0000 0072 1e00 0000  .r....r....r....
+00000560: 1f00 0000 7302 0000 0036 017a 166d 6963  ....s....6.z.mic
+00000570: 6861 6c65 7769 657a 2e3c 6c6f 6361 6c73  halewiez.<locals
+00000580: 3e2e 6672 1f00 0000 7221 0000 0072 0e00  >.fr....r!...r..
+00000590: 0000 721c 0000 0072 0f00 0000 da0b 6d69  ..r....r......mi
+000005a0: 6368 616c 6577 6965 7a1e 0000 0072 2300  chalewiez....r#.
+000005b0: 0000 7225 0000 0063 0100 0000 0000 0000  ..r%...c........
+000005c0: 0000 0000 0200 0000 0400 0000 0300 0000  ................
+000005d0: 7218 0000 0029 044e 7205 0000 0063 0100  r....).Nr....c..
+000005e0: 0000 0000 0000 0000 0000 0100 0000 0b00  ................
+000005f0: 0000 1300 0000 7362 0000 0074 00a0 0174  ......sb...t...t
+00000600: 00a0 0264 0188 0064 0117 00a1 0274 00a0  ...d...d.....t..
+00000610: 0374 00a0 0288 00a1 01a1 017c 0014 0064  .t.........|...d
+00000620: 0117 0014 00a1 0174 00a0 0174 00a0 0264  .......t...t...d
+00000630: 0188 0064 0117 00a1 0274 00a0 0374 00a0  ...d.....t...t..
+00000640: 0264 0288 0064 0217 00a1 02a1 017c 0014  .d...d.......|..
+00000650: 0064 0117 0014 00a1 0114 0053 0029 034e  .d.........S.).N
+00000660: 7207 0000 0072 0900 0000 2904 720a 0000  r....r....).r...
+00000670: 0072 0c00 0000 721b 0000 0072 1500 0000  .r....r....r....
+00000680: 720d 0000 0072 1c00 0000 720e 0000 0072  r....r....r....r
+00000690: 0f00 0000 721e 0000 0025 0000 0073 0200  ....r....%...s..
+000006a0: 0000 6201 7a11 6861 6e73 656e 2e3c 6c6f  ..b.z.hansen.<lo
+000006b0: 6361 6c73 3e2e 6672 1f00 0000 7221 0000  cals>.fr....r!..
+000006c0: 0072 0e00 0000 721c 0000 0072 0f00 0000  .r....r....r....
+000006d0: da06 6861 6e73 656e 2400 0000 7223 0000  ..hansen$...r#..
+000006e0: 0072 2600 0000 6301 0000 0000 0000 0000  .r&...c.........
+000006f0: 0000 0001 0000 0007 0000 0043 0000 0073  ...........C...s
+00000700: 1e00 0000 7400 a001 7400 a002 7400 a003  ....t...t...t...
+00000710: 7c00 a101 6401 1700 7c00 1400 a101 a101  |...d...|.......
+00000720: 5300 2902 4e67 9a99 9999 9999 b93f 2904  S.).Ng.......?).
+00000730: 720a 0000 0072 0c00 0000 da03 6162 7372  r....r......absr
+00000740: 0200 0000 720d 0000 0072 0e00 0000 720e  ....r....r....r.
+00000750: 0000 0072 0f00 0000 da06 616c 7069 6e65  ...r......alpine
+00000760: 2a00 0000 7302 0000 001e 0172 2800 0000  *...s......r(...
+00000770: 2901 7217 0000 0029 0fda 075f 5f64 6f63  ).r....)...__doc
+00000780: 5f5f da04 6d61 7468 7202 0000 0072 0300  __..mathr....r..
+00000790: 0000 7204 0000 00da 056e 756d 7079 720a  ..r......numpyr.
+000007a0: 0000 0072 2000 0000 7210 0000 0072 1200  ...r ...r....r..
+000007b0: 0000 7216 0000 0072 2200 0000 7225 0000  ..r....r"...r%..
+000007c0: 0072 2600 0000 7228 0000 0072 0e00 0000  .r&...r(...r....
+000007d0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+000007e0: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
+000007f0: 0000 0402 1404 0801 1002 1005 1005 0a04  ................
+00000800: 0a06 0a06 0c06                           ......
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/special.cpython-37.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/special.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/__pycache__/special.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/benchmarks/__pycache__/special.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/approximation.py` & `pyrimidine-1.6/pyrimidine/benchmarks/approximation.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/cluster.py` & `pyrimidine-1.6/pyrimidine/benchmarks/cluster.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 
 import numpy as np
 import numpy.linalg as LA
-from ..benchmark import BaseProblem
+
 
 
 class KMeans(BaseProblem):
     """KMeans clustering Problem
 
     ERM:
     min J(c,mu) = sum_c sum_{x:c} ||x-mu_c||
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/fitting.py` & `pyrimidine-1.6/pyrimidine/benchmarks/fitting.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,39 +33,51 @@
 class CurveFitting(Fitting):
 
     def fit(self, *params):
         return np.vstack((np.sum([c*relu(b * self.X - a) for a, b, c in zip(*params[:3])], axis=0), 
             np.sum([c*relu(b * self.X - a) for a, b, c in zip(*params[3:])], axis=0)))
 
 
-_indicator = lambda x, y: (0<= x <= 5) & (0<= y <= 5)
+_indicator = lambda x, y: (0<= x) * (x<= 5) * (0<= y) * (y <= 5)
 
 from math import cos, sin
-def basis(a, b, c, t):
-    # basis in the form {di* indicator(Aix-ti)}
+
+def basis(a, d1, d2, t):
+    """basis
+    
+    Args:
+        a (number): Rotation
+        d1 (number): Scaling
+        d2 (number): Scaling
+        t (number): Translation
+    
+    Returns:
+        function
+    """
+
     c = cos(3.14*a)
     s = sin(3.14*a)
     def _f(x,y):
         y, x = np.meshgrid(y-t[0], x-t[1])
-        return _indicator(b*(c*x-s*y), c*(s*x+c*y))
+        return _indicator(d1*(c*x-s*y), d2*(s*x+c*y))
     return _f
 
 
 from PIL import Image
 
 class Painting(Fitting):
-    def __init__(self, image, size=None, mode=None, channel=0):
 
+    def __init__(self, image, size=None, mode=None, channel=0):
         self.size = size or image.size
         self.mode = mode or image.mode
         self.y = np.asarray(image.resize(self.size), np.float_)[:,:,channel]
         self.n = 256
 
     def fit(self, *params):
         ks = np.arange(self.size[0])
         ls = np.arange(self.size[1])
-        return np.sum([d * basis(a, b, c, t)(ks, ls) for a, b, c, t, d in zip(*params)], axis=0)
+        return np.sum([c * basis(a, d1, d2, t)(ks, ls) for a, d1, d2, t, c in zip(*params)], axis=0)
 
     def toimage(self, *params):
         yy = self.fit(*params)
         return Image.fromarray(yy.astype('uint8')).convert(self.mode)
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/matrix.py` & `pyrimidine-1.6/pyrimidine/benchmarks/matrix.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/optimization.py` & `pyrimidine-1.6/pyrimidine/benchmarks/optimization.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/special.py` & `pyrimidine-1.6/pyrimidine/benchmarks/special.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,7 @@
     def f(x:np.ndarray):
         return np.sum(np.arange(1, n+1)*(np.cos(np.arange(n))*x+1)) * np.sum(np.arange(1, n+1)*(np.cos(np.arange(2, n+2))*x+1))
     return f
 
 
 def alpine(x):
     return np.sum(np.abs((np.sin(x) + 0.1) * x))
-
```

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/test_dataset.csv` & `pyrimidine-1.6/pyrimidine/benchmarks/test_dataset.csv`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/benchmarks/train_dataset.csv` & `pyrimidine-1.6/pyrimidine/benchmarks/train_dataset.csv`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/chromosome.py` & `pyrimidine-1.6/pyrimidine/chromosome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 #!/usr/bin/env python3
 
+"""
+Chromosome classes, subclass of BaseChromosome
+
+A chromosome is an array of genes, or it can be customized by the user.
+It could be a part of an individual or encodes a solution directly.
+"""
+
 from random import choice, randint, gauss, random
 
 import numpy as np
 from scipy.stats import norm
 from scipy.special import softmax
 
 from .base import BaseChromosome, BaseGene
```

### Comparing `pyrimidine-1.5.6/pyrimidine/de.py` & `pyrimidine-1.6/pyrimidine/de.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/deco.py` & `pyrimidine-1.6/pyrimidine/deco.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/ep.py` & `pyrimidine-1.6/pyrimidine/ep.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 
 """Evolution Programming
 
 Invented by L. Fogel[1966] for designing FSM initially.
 
 General form of the algorithm:
-initialize a population with N individuals
-loop:
-    calculate f(x) for each x in population
-    mutate x for each x
-    get new population (mixed with the original population)
-    select best N individuals from the 2N mixed population
-
-The mutation:
-    x' <- x + r*sqrt(v)
-    v' <- v + c*r*sqrt(v) (make sure that v>epsilon)
 
-Caution: No cross operation in EP
+    initialize a population with N individuals
+    loop:
+        calculate f(x) for each x in population
+        mutate x for each x
+        get new population (mixed with the original population)
+        select best N individuals from the 2N mixed population
+
+    The mutation:
+        x' <- x + r*sqrt(v)
+        v' <- v + c*r*sqrt(v) (make sure that v>epsilon)
+
+Remark:
+    No cross operation in EP
 """
 
 from random import choice
 from toolz.itertoolz import groupby
 from operator import attrgetter
 
 import numpy as np
 
 from .base import PopulationMixin, BaseChromosome
 from .chromosome import FloatChromosome
 from .individual import MixedIndividual
-from .utils import max_lb
+
+from .deco import side_effect
 
 
 class BaseEPIndividual(MixedIndividual):
     """Base class of EP Individual Class
 
     A single solution in EP
     """
@@ -49,42 +52,49 @@
     def variance(self):
         return self.chromosomes[1]
 
     @variance.setter
     def variance(self, v):
         self.chromosomes[1] = v
     
+    @side_effect
     def mutate(self):
         rx = np.random.randn(*self.chromosomes[0].shape)
         self.chromosomes[0] += rx * np.sqrt(self.variance)
 
         rv = np.random.randn(*self.variance.shape)
         self.variance += self.c * rv * np.sqrt(self.variance)
-        self.variance = max_lb(self.epsilon)(self.variance)
+        self.variance = np.maximum(self.variance, self.epsilon)
 
 
-class EPPopulation(PopulationMixin):
+class EvolutionProgramming(PopulationMixin):
     """Evolution Programming
     
     Extends:
         PopulationMixin
     """
     
     element_class = BaseEPIndividual
 
     def select(self):
-        d = groupby(attrgetter('fitness'), self.sorted_individuals)
+        self.sort()
+        d = groupby(attrgetter('fitness'), self)
         inds = []
         ks = np.sort(list(d.keys()))[::-1]
-        while len(inds) < self.n_individuals:
+        flag = True
+        while flag:
             for k in ks:
                 if d[k]:
                     a = choice(d[k])
                     inds.append(a)
                     d[k].remove(a)
+                    if len(inds) <= self.default_size:
+                        flag = False
+                        break
         self.individuals = inds
 
     def transition(self, *args, **kwargs):
         cpy = self.clone()
         self.mutate()
         self.merge(cpy)
         self.select()
+
```

### Comparing `pyrimidine-1.5.6/pyrimidine/errors.py` & `pyrimidine-1.6/pyrimidine/errors.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/fa.py` & `pyrimidine-1.6/pyrimidine/fa.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 #!/usr/bin/env python3
 
 """Firefly Algorithm
+
+*References*
+Yang, X. S. (2010). "Firefly Algorithm: A New Approach for Optimization".
+  In Stochastic Algorithms: Foundations and Applications (pp. 169-178). Springer Berlin Heidelberg.
+Yang, X. S. (2013). "Nature-Inspired Metaheuristic Algorithms". Luniver Press.
 """
 
+from random import gauss, random
 from scipy.spatial.distance import pdist, squareform
 import numpy as np
 
 from .base import PopulationMixin
 from .chromosome import FloatChromosome
 from .individual import PolyIndividual
-from .utils import gauss, random
 
 from .pso import BaseParticle
 
 
 @basic_memory
 class BaseFirefly(BaseParticle):
```

### Comparing `pyrimidine-1.5.6/pyrimidine/gene.py` & `pyrimidine-1.6/pyrimidine/gene.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/individual.py` & `pyrimidine-1.6/pyrimidine/individual.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 
 """
 Individual classes
+
+An individual represents a solution of a optimization problem.
+It is defined as a container of chromosomes.
 """
 
 from .base import BaseIndividual
 from .chromosome import BinaryChromosome, BaseChromosome, FloatChromosome
 from .meta import MetaTuple, MetaList, MetaSingle
 from .utils import randint
```

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__init__.py` & `pyrimidine-1.6/pyrimidine/learn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/__init__.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Dec 18 12:26:01 2023 UTC, .py size: 1225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -28,60 +28,60 @@
 000001b0: 6c61 7469 6f6e 2066 6f72 2047 410a 2020  lation for GA.  
 000001c0: 2020 4ea9 0063 0300 0000 0000 0000 0000    N..c..........
 000001d0: 0000 0500 0000 0100 0000 4f00 0000 7304  ..........O...s.
 000001e0: 0000 0074 0082 01a9 014e 2901 da13 4e6f  ...t.....N)...No
 000001f0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
 00000200: 7229 05da 0363 6c73 da01 58da 0159 da04  r)...cls..X..Y..
 00000210: 6172 6773 da06 6b77 6172 6773 7205 0000  args..kwargsr...
-00000220: 0072 0500 0000 fa4b 2f55 7365 7273 2f77  .r.....K/Users/w
+00000220: 0072 0500 0000 fa45 2f55 7365 7273 2f77  .r.....E/Users/w
 00000230: 696c 6c69 616d 2f50 726f 6772 616d 6d69  illiam/Programmi
-00000240: 6e67 2f6d 7947 6974 6875 622f 7079 7269  ng/myGithub/pyri
-00000250: 6d69 6469 6e65 2f70 7972 696d 6964 696e  midine/pyrimidin
-00000260: 652f 6c65 6172 6e2f 5f5f 696e 6974 5f5f  e/learn/__init__
-00000270: 2e70 79da 0663 6f6e 6669 6716 0000 0073  .py..config....s
-00000280: 0200 0000 0403 7a14 4261 7365 4573 7469  ......z.BaseEsti
-00000290: 6d61 746f 722e 636f 6e66 6967 4663 0500  mator.configFc..
-000002a0: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-000002b0: 0000 4300 0000 733c 0000 007c 0472 0f7c  ..C...s<...|.r.|
-000002c0: 0370 0c7c 006a 0070 0c7c 00a0 017c 017c  .p.|.j.p.|...|.|
-000002d0: 02a1 027c 005f 006e 097c 0370 167c 00a0  ...|._.n.|.p.|..
-000002e0: 017c 017c 02a1 027c 005f 007c 00a0 02a1  .|.|...|._.|....
-000002f0: 0001 007c 0053 0072 0600 0000 2903 da03  ...|.S.r....)...
-00000300: 706f 7072 0e00 0000 da04 5f66 6974 2905  popr......_fit).
-00000310: da04 7365 6c66 7209 0000 0072 0a00 0000  ..selfr....r....
-00000320: 720f 0000 005a 0a77 6172 6d5f 7374 6172  r....Z.warm_star
-00000330: 7472 0500 0000 7205 0000 0072 0d00 0000  tr....r....r....
-00000340: da03 6669 741b 0000 0073 0a00 0000 0401  ..fit....s......
-00000350: 1a01 1202 0801 0401 7a11 4261 7365 4573  ........z.BaseEs
-00000360: 7469 6d61 746f 722e 6669 7463 0100 0000  timator.fitc....
-00000370: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-00000380: 4300 0000 733a 0000 007c 006a 006a 017c  C...s:...|.j.j.|
-00000390: 006a 0264 018d 0101 007c 006a 006a 037d  .j.d.....|.j.j.}
-000003a0: 017c 006a 0444 005d 0b7d 0274 057c 007c  .|.j.D.].}.t.|.|
-000003b0: 0274 067c 017c 0283 0283 0301 0071 0f64  .t.|.|.......q.d
-000003c0: 0053 0029 024e 2901 da06 6e5f 6974 6572  .S.).N)...n_iter
-000003d0: 2907 720f 0000 00da 0665 7a6f 6c76 65da  ).r......ezolve.
-000003e0: 086d 6178 5f69 7465 72da 0873 6f6c 7574  .max_iter..solut
-000003f0: 696f 6eda 1065 7374 696d 6174 6564 5f70  ion..estimated_p
-00000400: 6172 616d 73da 0773 6574 6174 7472 da07  arams..setattr..
-00000410: 6765 7461 7474 7229 0372 1100 0000 5a06  getattr).r....Z.
-00000420: 6d6f 6465 6c5f da01 6b72 0500 0000 7205  model_..kr....r.
-00000430: 0000 0072 0d00 0000 7210 0000 0023 0000  ...r....r....#..
-00000440: 0073 0a00 0000 1001 0801 0a01 1401 04ff  .s..............
-00000450: 7a12 4261 7365 4573 7469 6d61 746f 722e  z.BaseEstimator.
-00000460: 5f66 6974 7206 0000 0029 034e 4e46 290a  _fitr....).NNF).
-00000470: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000480: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000490: 6d65 5f5f da07 5f5f 646f 635f 5f72 0f00  me__..__doc__r..
-000004a0: 0000 7217 0000 00da 0b63 6c61 7373 6d65  ..r......classme
-000004b0: 7468 6f64 720e 0000 0072 1200 0000 7210  thodr....r....r.
-000004c0: 0000 0072 0500 0000 7205 0000 0072 0500  ...r....r....r..
-000004d0: 0000 720d 0000 0072 0200 0000 0a00 0000  ..r....r........
-000004e0: 7310 0000 0008 0004 0204 0704 0102 020c  s...............
-000004f0: 010a 040c 0872 0200 0000 2907 5a0c 736b  .....r....).Z.sk
-00000500: 6c65 6172 6e2e 6261 7365 7202 0000 00da  learn.baser.....
-00000510: 0242 45da 0877 6172 6e69 6e67 73da 026f  .BE..warnings..o
-00000520: 73da 0e66 696c 7465 7277 6172 6e69 6e67  s..filterwarning
-00000530: 73da 0765 6e76 6972 6f6e 7205 0000 0072  s..environr....r
-00000540: 0500 0000 7205 0000 0072 0d00 0000 da08  ....r....r......
-00000550: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000560: 000c 0210 020a 010a 0114 03              ...........
+00000240: 6e67 2f50 7974 686f 6e2f 6d79 776f 726b  ng/Python/mywork
+00000250: 2f70 7972 696d 6964 696e 652f 6c65 6172  /pyrimidine/lear
+00000260: 6e2f 5f5f 696e 6974 5f5f 2e70 79da 0663  n/__init__.py..c
+00000270: 6f6e 6669 6716 0000 0073 0200 0000 0403  onfig....s......
+00000280: 7a14 4261 7365 4573 7469 6d61 746f 722e  z.BaseEstimator.
+00000290: 636f 6e66 6967 4663 0500 0000 0000 0000  configFc........
+000002a0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+000002b0: 733c 0000 007c 0472 0f7c 0370 0c7c 006a  s<...|.r.|.p.|.j
+000002c0: 0070 0c7c 00a0 017c 017c 02a1 027c 005f  .p.|...|.|...|._
+000002d0: 006e 097c 0370 167c 00a0 017c 017c 02a1  .n.|.p.|...|.|..
+000002e0: 027c 005f 007c 00a0 02a1 0001 007c 0053  .|._.|.......|.S
+000002f0: 0072 0600 0000 2903 da03 706f 7072 0e00  .r....)...popr..
+00000300: 0000 da04 5f66 6974 2905 da04 7365 6c66  ...._fit)...self
+00000310: 7209 0000 0072 0a00 0000 720f 0000 005a  r....r....r....Z
+00000320: 0a77 6172 6d5f 7374 6172 7472 0500 0000  .warm_startr....
+00000330: 7205 0000 0072 0d00 0000 da03 6669 741b  r....r......fit.
+00000340: 0000 0073 0a00 0000 0401 1a01 1202 0801  ...s............
+00000350: 0401 7a11 4261 7365 4573 7469 6d61 746f  ..z.BaseEstimato
+00000360: 722e 6669 7463 0100 0000 0000 0000 0000  r.fitc..........
+00000370: 0000 0300 0000 0700 0000 4300 0000 733a  ..........C...s:
+00000380: 0000 007c 006a 006a 017c 006a 0264 018d  ...|.j.j.|.j.d..
+00000390: 0101 007c 006a 006a 037d 017c 006a 0444  ...|.j.j.}.|.j.D
+000003a0: 005d 0b7d 0274 057c 007c 0274 067c 017c  .].}.t.|.|.t.|.|
+000003b0: 0283 0283 0301 0071 0f64 0053 0029 024e  .......q.d.S.).N
+000003c0: 2901 da06 6e5f 6974 6572 2907 720f 0000  )...n_iter).r...
+000003d0: 00da 0665 7a6f 6c76 65da 086d 6178 5f69  ...ezolve..max_i
+000003e0: 7465 72da 0873 6f6c 7574 696f 6eda 1065  ter..solution..e
+000003f0: 7374 696d 6174 6564 5f70 6172 616d 73da  stimated_params.
+00000400: 0773 6574 6174 7472 da07 6765 7461 7474  .setattr..getatt
+00000410: 7229 0372 1100 0000 5a06 6d6f 6465 6c5f  r).r....Z.model_
+00000420: da01 6b72 0500 0000 7205 0000 0072 0d00  ..kr....r....r..
+00000430: 0000 7210 0000 0023 0000 0073 0a00 0000  ..r....#...s....
+00000440: 1001 0801 0a01 1401 04ff 7a12 4261 7365  ..........z.Base
+00000450: 4573 7469 6d61 746f 722e 5f66 6974 7206  Estimator._fitr.
+00000460: 0000 0029 034e 4e46 290a da08 5f5f 6e61  ...).NNF)...__na
+00000470: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000480: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000490: 5f5f 646f 635f 5f72 0f00 0000 7217 0000  __doc__r....r...
+000004a0: 00da 0b63 6c61 7373 6d65 7468 6f64 720e  ...classmethodr.
+000004b0: 0000 0072 1200 0000 7210 0000 0072 0500  ...r....r....r..
+000004c0: 0000 7205 0000 0072 0500 0000 720d 0000  ..r....r....r...
+000004d0: 0072 0200 0000 0a00 0000 7310 0000 0008  .r........s.....
+000004e0: 0004 0204 0704 0102 020c 010a 040c 0872  ...............r
+000004f0: 0200 0000 2907 5a0c 736b 6c65 6172 6e2e  ....).Z.sklearn.
+00000500: 6261 7365 7202 0000 00da 0242 45da 0877  baser......BE..w
+00000510: 6172 6e69 6e67 73da 026f 73da 0e66 696c  arnings..os..fil
+00000520: 7465 7277 6172 6e69 6e67 73da 0765 6e76  terwarnings..env
+00000530: 6972 6f6e 7205 0000 0072 0500 0000 7205  ironr....r....r.
+00000540: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000550: 653e 0100 0000 730a 0000 000c 0210 020a  e>....s.........
+00000560: 010a 0114 03                             .....
```

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/base.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/base.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/linear_regression.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/linear_regression.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Dec 18 12:47:22 2023 UTC, .py size: 1579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,149 @@
-00000000: 6f0d 0d0a 0000 0000 5a3f 8065 2b06 0000  o.......Z?.e+...
+00000000: 6f0d 0d0a 0000 0000 1e3d 8065 c605 0000  o........=.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a05 0100 6401 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000050: 0100 6404 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6404 6406 6c0b 6d0c 5a0c 0100 6404  ..d.d.l.m.Z...d.
-00000070: 6407 6c0d 6d0e 5a0e 0100 6404 6408 6c0f  d.l.m.Z...d.d.l.
-00000080: 6d10 5a10 0100 6401 6409 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
-00000090: 0100 6512 640a 640b 640c 8d02 5a13 4700  ..e.d.d.d...Z.G.
-000000a0: 640d 640e 8400 640e 6509 8303 5a14 4700  d.d...d.e...Z.G.
-000000b0: 640f 6410 8400 6410 6510 6507 8304 5a15  d.d...d.e.e...Z.
-000000c0: 6402 5300 2911 7a19 4741 2066 6f72 206c  d.S.).z.GA for l
-000000d0: 696e 6561 7220 7265 6772 6573 7369 6f6e  inear regression
-000000e0: 0ae9 0000 0000 4ea9 01da 104c 696e 6561  ......N....Linea
-000000f0: 7252 6567 7265 7373 696f 6ee9 0200 0000  rRegression.....
-00000100: 2902 da10 4269 6e61 7279 4368 726f 6d6f  )...BinaryChromo
-00000110: 736f 6d65 da0f 466c 6f61 7443 6872 6f6d  some..FloatChrom
-00000120: 6f73 6f6d 6529 01da 0f4d 6978 6564 496e  osome)...MixedIn
-00000130: 6469 7669 6475 616c 2901 da12 5374 616e  dividual)...Stan
-00000140: 6461 7264 506f 7075 6c61 7469 6f6e 2901  dardPopulation).
-00000150: da0d 4261 7365 4573 7469 6d61 746f 7229  ..BaseEstimator)
-00000160: 01da 1149 6e74 6572 7661 6c43 6f6e 7665  ...IntervalConve
-00000170: 7274 6572 69c4 ffff ffe9 3c00 0000 2902  rteri.....<...).
-00000180: da02 6c62 da02 7562 6300 0000 0000 0000  ..lb..ubc.......
-00000190: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-000001a0: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-000001b0: 6402 8400 5a03 6403 5300 2904 da11 5f42  d...Z.d.S.)..._B
-000001c0: 696e 6172 7943 6872 6f6d 6f73 6f6d 6563  inaryChromosomec
-000001d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000001e0: 0200 0000 4300 0000 7308 0000 0074 007c  ....C...s....t.|
-000001f0: 0083 0153 00a9 014e 2901 da01 6329 01da  ...S...N)...c)..
-00000200: 0473 656c 66a9 0072 1200 0000 fa54 2f55  .self..r.....T/U
-00000210: 7365 7273 2f77 696c 6c69 616d 2f50 726f  sers/william/Pro
-00000220: 6772 616d 6d69 6e67 2f6d 7947 6974 6875  gramming/myGithu
-00000230: 622f 7079 7269 6d69 6469 6e65 2f70 7972  b/pyrimidine/pyr
-00000240: 696d 6964 696e 652f 6c65 6172 6e2f 6c69  imidine/learn/li
-00000250: 6e65 6172 5f72 6567 7265 7373 696f 6e2e  near_regression.
-00000260: 7079 da06 6465 636f 6465 1500 0000 7302  py..decode....s.
-00000270: 0000 0008 017a 185f 4269 6e61 7279 4368  .....z._BinaryCh
-00000280: 726f 6d6f 736f 6d65 2e64 6563 6f64 654e  romosome.decodeN
-00000290: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000002a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000002b0: 6e61 6d65 5f5f 7214 0000 0072 1200 0000  name__r....r....
-000002c0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000002d0: 0e00 0000 1400 0000 7304 0000 0008 000c  ........s.......
-000002e0: 0172 0e00 0000 6300 0000 0000 0000 0000  .r....c.........
-000002f0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00000300: 2e00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000310: 6402 5a04 6505 6403 6404 8400 8301 5a06  d.Z.e.d.d.....Z.
-00000320: 6505 6409 6406 6407 8401 8301 5a07 6408  e.d.d.d.....Z.d.
-00000330: 5300 290a da12 4741 4c69 6e65 6172 5265  S.)...GALinearRe
-00000340: 6772 6573 7369 6f6e 7a1c 4c69 6e65 6172  gressionz.Linear
-00000350: 2052 6567 7265 7373 696f 6e20 6279 2047   Regression by G
-00000360: 410a 2020 2020 2902 da05 636f 6566 5fda  A.    )...coef_.
-00000370: 0a69 6e74 6572 6365 7074 5f63 0100 0000  .intercept_c....
-00000380: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000390: 4f00 0000 730e 0000 0074 007c 0169 007c  O...s....t.|.i.|
-000003a0: 02a4 018e 0153 0072 0f00 0000 7202 0000  .....S.r....r...
-000003b0: 0029 03da 0363 6c73 da04 6172 6773 da06  .)...cls..args..
-000003c0: 6b77 6172 6773 7212 0000 0072 1200 0000  kwargsr....r....
-000003d0: 7213 0000 00da 0c63 7265 6174 655f 6d6f  r......create_mo
-000003e0: 6465 6c1f 0000 0073 0200 0000 0e02 7a1f  del....s......z.
-000003f0: 4741 4c69 6e65 6172 5265 6772 6573 7369  GALinearRegressi
-00000400: 6f6e 2e63 7265 6174 655f 6d6f 6465 6ce9  on.create_model.
-00000410: 0a00 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00000420: 000a 0000 0006 0000 000f 0000 0073 5a00  .............sZ.
-00000430: 0000 8800 6a00 6401 1900 7d06 7401 a002  ....j.d...}.t...
-00000440: 8801 a101 6401 6b02 7310 4a00 6402 8301  ....d.k.s.J.d...
-00000450: 8201 4700 8700 8701 8702 8703 8704 6605  ..G...........f.
-00000460: 6403 6404 8408 6404 7403 8303 7d07 7404  d.d...d.t...}.t.
-00000470: 7c07 1900 7d08 7c08 6a05 7c03 7c06 6405  |...}.|.j.|.|.d.
-00000480: 6602 6406 8d02 7d09 7c09 5300 2907 4ee9  f.d...}.|.S.).N.
-00000490: 0100 0000 7a1d 6f6e 6c79 2073 7570 706f  ....z.only suppo
-000004a0: 7274 2031 4420 6172 7261 7920 666f 7220  rt 1D array for 
-000004b0: 6059 6063 0000 0000 0000 0000 0000 0000  `Y`c............
-000004c0: 0000 0000 0300 0000 0000 0000 7332 0000  ............s2..
-000004d0: 0065 005a 0164 005a 0265 0365 0466 025a  .e.Z.d.Z.e.e.f.Z
-000004e0: 0587 0287 0387 0466 0364 0164 0284 085a  .......f.d.d...Z
-000004f0: 0687 0087 0166 0264 0364 0484 085a 0764  .....f.d.d...Z.d
-00000500: 0553 0029 067a 2f47 414c 696e 6561 7252  .S.).z/GALinearR
-00000510: 6567 7265 7373 696f 6e2e 636f 6e66 6967  egression.config
-00000520: 2e3c 6c6f 6361 6c73 3e2e 4d79 496e 6469  .<locals>.MyIndi
-00000530: 7669 6475 616c 6301 0000 0000 0000 0000  vidualc.........
-00000540: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00000550: 3200 0000 8801 6a00 8800 6900 8802 a401  2.....j...i.....
-00000560: 8e01 7d01 7401 a002 7c00 6401 1900 a101  ..}.t...|.d.....
-00000570: 7c01 5f03 7c00 6402 1900 a004 a100 7c01  |._.|.d.......|.
-00000580: 5f05 7c01 5300 2903 4e72 0100 0000 7220  _.|.S.).Nr....r 
-00000590: 0000 0029 0672 1e00 0000 da02 6e70 da07  ...).r......np..
-000005a0: 6173 6172 7261 7972 1900 0000 7214 0000  asarrayr....r...
-000005b0: 0072 1a00 0000 a902 7211 0000 00da 056d  .r......r......m
-000005c0: 6f64 656c 2903 721c 0000 0072 1b00 0000  odel).r....r....
-000005d0: 721d 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000005e0: 1400 0000 2e00 0000 7308 0000 0010 0110  ........s.......
-000005f0: 010e 0104 017a 3647 414c 696e 6561 7252  .....z6GALinearR
-00000600: 6567 7265 7373 696f 6e2e 636f 6e66 6967  egression.config
-00000610: 2e3c 6c6f 6361 6c73 3e2e 4d79 496e 6469  .<locals>.MyIndi
-00000620: 7669 6475 616c 2e64 6563 6f64 6563 0100  vidual.decodec..
-00000630: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000640: 0000 1300 0000 7314 0000 007c 00a0 00a1  ......s....|....
-00000650: 007d 017c 01a0 0188 0088 01a1 0253 0072  .}.|.........S.r
-00000660: 0f00 0000 2902 7214 0000 00da 0573 636f  ....).r......sco
-00000670: 7265 7223 0000 0029 02da 0158 da01 5972  rer#...)...X..Yr
-00000680: 1200 0000 7213 0000 00da 085f 6669 746e  ....r......_fitn
-00000690: 6573 7334 0000 0073 0400 0000 0801 0c01  ess4...s........
-000006a0: 7a38 4741 4c69 6e65 6172 5265 6772 6573  z8GALinearRegres
-000006b0: 7369 6f6e 2e63 6f6e 6669 672e 3c6c 6f63  sion.config.<loc
-000006c0: 616c 733e 2e4d 7949 6e64 6976 6964 7561  als>.MyIndividua
-000006d0: 6c2e 5f66 6974 6e65 7373 4e29 0872 1500  l._fitnessN).r..
-000006e0: 0000 7216 0000 0072 1700 0000 7206 0000  ..r....r....r...
-000006f0: 0072 0e00 0000 da0d 656c 656d 656e 745f  .r......element_
-00000700: 636c 6173 7372 1400 0000 7228 0000 0072  classr....r(...r
-00000710: 1200 0000 a905 7226 0000 0072 2700 0000  ......r&...r'...
-00000720: 721c 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
-00000730: 1200 0000 7213 0000 00da 0c4d 7949 6e64  ....r......MyInd
-00000740: 6976 6964 7561 6c2a 0000 0073 0800 0000  ividual*...s....
-00000750: 0800 0802 1002 1206 722b 0000 00e9 0800  ........r+......
-00000760: 0000 2902 da0d 6e5f 696e 6469 7669 6475  ..)...n_individu
-00000770: 616c 73da 0473 697a 6529 06da 0573 6861  als..size)...sha
-00000780: 7065 7221 0000 00da 046e 6469 6d72 0700  per!.....ndimr..
-00000790: 0000 7208 0000 00da 0672 616e 646f 6d29  ..r......random)
-000007a0: 0a72 1b00 0000 7226 0000 0072 2700 0000  .r....r&...r'...
-000007b0: 722d 0000 0072 1c00 0000 721d 0000 00da  r-...r....r.....
-000007c0: 0969 6e70 7574 5f64 696d 722b 0000 00da  .input_dimr+....
-000007d0: 0c4d 7950 6f70 756c 6174 696f 6eda 0370  .MyPopulation..p
-000007e0: 6f70 7212 0000 0072 2a00 0000 7213 0000  opr....r*...r...
-000007f0: 00da 0663 6f6e 6669 6723 0000 0073 0c00  ...config#...s..
-00000800: 0000 0a03 1601 1c03 080e 1202 0402 7a19  ..............z.
-00000810: 4741 4c69 6e65 6172 5265 6772 6573 7369  GALinearRegressi
-00000820: 6f6e 2e63 6f6e 6669 674e 2901 721f 0000  on.configN).r...
-00000830: 0029 0872 1500 0000 7216 0000 0072 1700  .).r....r....r..
-00000840: 0000 da07 5f5f 646f 635f 5fda 1065 7374  ....__doc__..est
-00000850: 696d 6174 6564 5f70 6172 616d 73da 0b63  imated_params..c
-00000860: 6c61 7373 6d65 7468 6f64 721e 0000 0072  lassmethodr....r
-00000870: 3500 0000 7212 0000 0072 1200 0000 7212  5...r....r....r.
-00000880: 0000 0072 1300 0000 7218 0000 0019 0000  ...r....r.......
-00000890: 0073 0e00 0000 0800 0401 0403 0202 0a01  .s..............
-000008a0: 0203 1001 7218 0000 0029 1672 3600 0000  ....r....).r6...
-000008b0: da05 6e75 6d70 7972 2100 0000 da0c 6e75  ..numpyr!.....nu
-000008c0: 6d70 792e 6c69 6e61 6c67 da06 6c69 6e61  mpy.linalg..lina
-000008d0: 6c67 da02 4c41 5a14 736b 6c65 6172 6e2e  lg..LAZ.sklearn.
-000008e0: 6c69 6e65 6172 5f6d 6f64 656c 7203 0000  linear_modelr...
-000008f0: 00da 0a63 6872 6f6d 6f73 6f6d 6572 0500  ...chromosomer..
-00000900: 0000 7206 0000 00da 0a69 6e64 6976 6964  ..r......individ
-00000910: 7561 6c72 0700 0000 da0a 706f 7075 6c61  ualr......popula
-00000920: 7469 6f6e 7208 0000 00da 056c 6561 726e  tionr......learn
-00000930: 7209 0000 005a 0f64 6967 6974 5f63 6f6e  r....Z.digit_con
-00000940: 7665 7274 6572 720a 0000 0072 1000 0000  verterr....r....
-00000950: 720e 0000 0072 1800 0000 7212 0000 0072  r....r....r....r
-00000960: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
-00000970: 3c6d 6f64 756c 653e 0100 0000 7318 0000  <module>....s...
-00000980: 0004 0208 030c 010c 0110 020c 010c 010c  ................
-00000990: 020c 020c 0310 0116 05                   .........
+00000050: 0100 6404 6405 6c08 6d09 5a09 0100 6404  ..d.d.l.m.Z...d.
+00000060: 6406 6c0a 6d0b 5a0b 0100 6401 6407 6c0c  d.l.m.Z...d.d.l.
+00000070: 6d0d 5a0d 0100 650d 6408 6409 640a 8d02  m.Z...e.d.d.d...
+00000080: 5a0e 4700 640b 640c 8400 640c 650f 8303  Z.G.d.d...d.e...
+00000090: 5a10 4700 640d 640e 8400 640e 6509 6507  Z.G.d.d...d.e.e.
+000000a0: 8304 5a11 6402 5300 290f 7a19 4741 2066  ..Z.d.S.).z.GA f
+000000b0: 6f72 206c 696e 6561 7220 7265 6772 6573  or linear regres
+000000c0: 7369 6f6e 0ae9 0000 0000 4ea9 01da 104c  sion......N....L
+000000d0: 696e 6561 7252 6567 7265 7373 696f 6ee9  inearRegression.
+000000e0: 0200 0000 2901 da0d 4261 7365 4573 7469  ....)...BaseEsti
+000000f0: 6d61 746f 7229 01da 1253 7461 6e64 6172  mator)...Standar
+00000100: 6450 6f70 756c 6174 696f 6e29 01da 1149  dPopulation)...I
+00000110: 6e74 6572 7661 6c43 6f6e 7665 7274 6572  ntervalConverter
+00000120: 69c4 ffff ffe9 3c00 0000 2902 da02 6c62  i.....<...)...lb
+00000130: da02 7562 6300 0000 0000 0000 0000 0000  ..ubc...........
+00000140: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
+00000150: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00000160: 5a03 6403 5300 2904 da11 5f42 696e 6172  Z.d.S.)..._Binar
+00000170: 7943 6872 6f6d 6f73 6f6d 6563 0100 0000  yChromosomec....
+00000180: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000190: 4300 0000 7308 0000 0074 007c 0083 0153  C...s....t.|...S
+000001a0: 00a9 014e 2901 da01 6329 01da 0473 656c  ...N)...c)...sel
+000001b0: 66a9 0072 0f00 0000 fa4e 2f55 7365 7273  f..r.....N/Users
+000001c0: 2f77 696c 6c69 616d 2f50 726f 6772 616d  /william/Program
+000001d0: 6d69 6e67 2f50 7974 686f 6e2f 6d79 776f  ming/Python/mywo
+000001e0: 726b 2f70 7972 696d 6964 696e 652f 6c65  rk/pyrimidine/le
+000001f0: 6172 6e2f 6c69 6e65 6172 5f72 6567 7265  arn/linear_regre
+00000200: 7373 696f 6e2e 7079 da06 6465 636f 6465  ssion.py..decode
+00000210: 1000 0000 7302 0000 0008 017a 185f 4269  ....s......z._Bi
+00000220: 6e61 7279 4368 726f 6d6f 736f 6d65 2e64  naryChromosome.d
+00000230: 6563 6f64 654e 2904 da08 5f5f 6e61 6d65  ecodeN)...__name
+00000240: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000250: 5f5f 7175 616c 6e61 6d65 5f5f 7211 0000  __qualname__r...
+00000260: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00000270: 7210 0000 0072 0b00 0000 0f00 0000 7304  r....r........s.
+00000280: 0000 0008 000c 0172 0b00 0000 6300 0000  .......r....c...
+00000290: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+000002a0: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
+000002b0: 5a02 6401 5a03 6402 5a04 6505 6403 6404  Z.d.Z.d.Z.e.d.d.
+000002c0: 8400 8301 5a06 6505 6409 6406 6407 8401  ....Z.e.d.d.d...
+000002d0: 8301 5a07 6408 5300 290a da12 4741 4c69  ..Z.d.S.)...GALi
+000002e0: 6e65 6172 5265 6772 6573 7369 6f6e 7a1c  nearRegressionz.
+000002f0: 4c69 6e65 6172 2052 6567 7265 7373 696f  Linear Regressio
+00000300: 6e20 6279 2047 410a 2020 2020 2902 5a06  n by GA.    ).Z.
+00000310: 636f 6566 735f 5a0b 696e 7465 7263 6570  coefs_Z.intercep
+00000320: 7473 5f63 0100 0000 0000 0000 0000 0000  ts_c............
+00000330: 0300 0000 0400 0000 4f00 0000 730e 0000  ........O...s...
+00000340: 0074 007c 0169 007c 02a4 018e 0153 0072  .t.|.i.|.....S.r
+00000350: 0c00 0000 7202 0000 0029 03da 0363 6c73  ....r....)...cls
+00000360: da04 6172 6773 da06 6b77 6172 6773 720f  ..args..kwargsr.
+00000370: 0000 0072 0f00 0000 7210 0000 00da 0c63  ...r....r......c
+00000380: 7265 6174 655f 6d6f 6465 6c1a 0000 0073  reate_model....s
+00000390: 0200 0000 0e02 7a1f 4741 4c69 6e65 6172  ......z.GALinear
+000003a0: 5265 6772 6573 7369 6f6e 2e63 7265 6174  Regression.creat
+000003b0: 655f 6d6f 6465 6ce9 0a00 0000 6304 0000  e_model.....c...
+000003c0: 0000 0000 0000 0000 000a 0000 0006 0000  ................
+000003d0: 000f 0000 0073 5a00 0000 8800 6a00 6401  .....sZ.....j.d.
+000003e0: 1900 7d06 7401 a002 8801 a101 6401 6b02  ..}.t.......d.k.
+000003f0: 7310 4a00 6402 8301 8201 4700 8700 8701  s.J.d.....G.....
+00000400: 8702 8703 8704 6605 6403 6404 8408 6404  ......f.d.d...d.
+00000410: 7403 8303 7d07 7404 7c07 1900 7d08 7c08  t...}.t.|...}.|.
+00000420: 6a05 7c03 7c06 6405 6602 6406 8d02 7d09  j.|.|.d.f.d...}.
+00000430: 7c09 5300 2907 4ee9 0100 0000 7a1d 6f6e  |.S.).N.....z.on
+00000440: 6c79 2073 7570 706f 7274 2031 4420 6172  ly support 1D ar
+00000450: 7261 7920 666f 7220 6059 6063 0000 0000  ray for `Y`c....
+00000460: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000470: 0000 0000 7332 0000 0065 005a 0164 005a  ....s2...e.Z.d.Z
+00000480: 0265 0365 0466 025a 0587 0287 0387 0466  .e.e.f.Z.......f
+00000490: 0364 0164 0284 085a 0687 0087 0166 0264  .d.d...Z.....f.d
+000004a0: 0364 0484 085a 0764 0553 0029 067a 2f47  .d...Z.d.S.).z/G
+000004b0: 414c 696e 6561 7252 6567 7265 7373 696f  ALinearRegressio
+000004c0: 6e2e 636f 6e66 6967 2e3c 6c6f 6361 6c73  n.config.<locals
+000004d0: 3e2e 4d79 496e 6469 7669 6475 616c 6301  >.MyIndividualc.
+000004e0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000004f0: 0000 0013 0000 0073 3200 0000 8801 6a00  .......s2.....j.
+00000500: 8800 6900 8802 a401 8e01 7d01 7401 a002  ..i.......}.t...
+00000510: 7c00 6401 1900 a101 7c01 5f03 7c00 6402  |.d.....|._.|.d.
+00000520: 1900 a004 a100 7c01 5f05 7c01 5300 2903  ......|._.|.S.).
+00000530: 4e72 0100 0000 721b 0000 0029 0672 1900  Nr....r....).r..
+00000540: 0000 da02 6e70 da07 6173 6172 7261 795a  ....np..asarrayZ
+00000550: 0563 6f65 665f 7211 0000 005a 0a69 6e74  .coef_r....Z.int
+00000560: 6572 6365 7074 5fa9 0272 0e00 0000 da05  ercept_..r......
+00000570: 6d6f 6465 6c29 0372 1700 0000 7216 0000  model).r....r...
+00000580: 0072 1800 0000 720f 0000 0072 1000 0000  .r....r....r....
+00000590: 7211 0000 0029 0000 0073 0800 0000 1001  r....)...s......
+000005a0: 1001 0e01 0401 7a36 4741 4c69 6e65 6172  ......z6GALinear
+000005b0: 5265 6772 6573 7369 6f6e 2e63 6f6e 6669  Regression.confi
+000005c0: 672e 3c6c 6f63 616c 733e 2e4d 7949 6e64  g.<locals>.MyInd
+000005d0: 6976 6964 7561 6c2e 6465 636f 6465 6301  ividual.decodec.
+000005e0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000005f0: 0000 0013 0000 0073 1400 0000 7c00 a000  .......s....|...
+00000600: a100 7d01 7c01 a001 8800 8801 a102 5300  ..}.|.........S.
+00000610: 720c 0000 0029 0272 1100 0000 da05 7363  r....).r......sc
+00000620: 6f72 6572 1e00 0000 2902 da01 58da 0159  orer....)...X..Y
+00000630: 720f 0000 0072 1000 0000 da08 5f66 6974  r....r......_fit
+00000640: 6e65 7373 2f00 0000 7304 0000 0008 010c  ness/...s.......
+00000650: 017a 3847 414c 696e 6561 7252 6567 7265  .z8GALinearRegre
+00000660: 7373 696f 6e2e 636f 6e66 6967 2e3c 6c6f  ssion.config.<lo
+00000670: 6361 6c73 3e2e 4d79 496e 6469 7669 6475  cals>.MyIndividu
+00000680: 616c 2e5f 6669 746e 6573 734e 2908 7212  al._fitnessN).r.
+00000690: 0000 0072 1300 0000 7214 0000 00da 0f46  ...r....r......F
+000006a0: 6c6f 6174 4368 726f 6d6f 736f 6d65 720b  loatChromosomer.
+000006b0: 0000 00da 0d65 6c65 6d65 6e74 5f63 6c61  .....element_cla
+000006c0: 7373 7211 0000 0072 2300 0000 720f 0000  ssr....r#...r...
+000006d0: 00a9 0572 2100 0000 7222 0000 0072 1700  ...r!...r"...r..
+000006e0: 0000 7216 0000 0072 1800 0000 720f 0000  ..r....r....r...
+000006f0: 0072 1000 0000 da0c 4d79 496e 6469 7669  .r......MyIndivi
+00000700: 6475 616c 2500 0000 7308 0000 0008 0008  dual%...s.......
+00000710: 0210 0212 0672 2700 0000 e908 0000 0029  .....r'........)
+00000720: 02da 0d6e 5f69 6e64 6976 6964 7561 6c73  ...n_individuals
+00000730: da04 7369 7a65 2906 da05 7368 6170 6572  ..size)...shaper
+00000740: 1c00 0000 da04 6e64 696d da0f 4d69 7865  ......ndim..Mixe
+00000750: 6449 6e64 6976 6964 7561 6c72 0600 0000  dIndividualr....
+00000760: da06 7261 6e64 6f6d 290a 7216 0000 0072  ..random).r....r
+00000770: 2100 0000 7222 0000 0072 2900 0000 7217  !...r"...r)...r.
+00000780: 0000 0072 1800 0000 5a09 696e 7075 745f  ...r....Z.input_
+00000790: 6469 6d72 2700 0000 5a0c 4d79 506f 7075  dimr'...Z.MyPopu
+000007a0: 6c61 7469 6f6e da03 706f 7072 0f00 0000  lation..popr....
+000007b0: 7226 0000 0072 1000 0000 da06 636f 6e66  r&...r......conf
+000007c0: 6967 1e00 0000 730c 0000 000a 0316 011c  ig....s.........
+000007d0: 0308 0e12 0204 027a 1947 414c 696e 6561  .......z.GALinea
+000007e0: 7252 6567 7265 7373 696f 6e2e 636f 6e66  rRegression.conf
+000007f0: 6967 4e29 0172 1a00 0000 2908 7212 0000  igN).r....).r...
+00000800: 0072 1300 0000 7214 0000 00da 075f 5f64  .r....r......__d
+00000810: 6f63 5f5f da10 6573 7469 6d61 7465 645f  oc__..estimated_
+00000820: 7061 7261 6d73 da0b 636c 6173 736d 6574  params..classmet
+00000830: 686f 6472 1900 0000 7230 0000 0072 0f00  hodr....r0...r..
+00000840: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000850: 0072 1500 0000 1400 0000 730e 0000 0008  .r........s.....
+00000860: 0004 0104 0302 020a 0102 0310 0172 1500  .............r..
+00000870: 0000 2912 7231 0000 00da 056e 756d 7079  ..).r1.....numpy
+00000880: 721c 0000 00da 0c6e 756d 7079 2e6c 696e  r......numpy.lin
+00000890: 616c 67da 066c 696e 616c 67da 024c 415a  alg..linalg..LAZ
+000008a0: 1473 6b6c 6561 726e 2e6c 696e 6561 725f  .sklearn.linear_
+000008b0: 6d6f 6465 6c72 0300 0000 da05 6c65 6172  modelr......lear
+000008c0: 6e72 0500 0000 da0a 706f 7075 6c61 7469  nr......populati
+000008d0: 6f6e 7206 0000 00da 0f64 6967 6974 5f63  onr......digit_c
+000008e0: 6f6e 7665 7274 6572 7207 0000 0072 0d00  onverterr....r..
+000008f0: 0000 da10 4269 6e61 7279 4368 726f 6d6f  ....BinaryChromo
+00000900: 736f 6d65 720b 0000 0072 1500 0000 720f  somer....r....r.
+00000910: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+00000920: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000930: 7314 0000 0004 0208 030c 010c 010c 010c  s...............
+00000940: 020c 010c 0210 0116 05                   .........
```

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/neural_network.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/neural_network.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Dec 18 12:47:15 2023 UTC, .py size: 1976 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 533f 8065 b807 0000  o.......S?.e....
+00000000: 6f0d 0d0a 0000 0000 fe2f 8065 b807 0000  o......../.e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6404 6405 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6404 6406 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 650c 6504  ..G.d.d...d.e.e.
@@ -38,117 +38,117 @@
 00000250: 6573 da08 6d61 785f 6974 6572 da08 6964  es..max_iter..id
 00000260: 656e 7469 7479 2905 7202 0000 00da 0a68  entity).r......h
 00000270: 6964 6465 6e5f 6469 6dda 0f6f 7574 5f61  idden_dim..out_a
 00000280: 6374 6976 6174 696f 6e5f da08 6e5f 6c61  ctivation_..n_la
 00000290: 7965 7273 da09 6e5f 6c61 7965 7273 5f29  yers..n_layers_)
 000002a0: 04da 0363 6c73 da04 6172 6773 da06 6b77  ...cls..args..kw
 000002b0: 6172 6773 da05 6d6f 6465 6ca9 0072 1b00  args..model..r..
-000002c0: 0000 fa51 2f55 7365 7273 2f77 696c 6c69  ...Q/Users/willi
-000002d0: 616d 2f50 726f 6772 616d 6d69 6e67 2f6d  am/Programming/m
-000002e0: 7947 6974 6875 622f 7079 7269 6d69 6469  yGithub/pyrimidi
-000002f0: 6e65 2f70 7972 696d 6964 696e 652f 6c65  ne/pyrimidine/le
-00000300: 6172 6e2f 6e65 7572 616c 5f6e 6574 776f  arn/neural_netwo
-00000310: 726b 2e70 79da 0c63 7265 6174 655f 6d6f  rk.py..create_mo
-00000320: 6465 6c19 0000 0073 0800 0000 1803 0601  del....s........
-00000330: 0801 0401 7a1b 4741 4d4c 5052 6567 7265  ....z.GAMLPRegre
-00000340: 7373 6f72 2e63 7265 6174 655f 6d6f 6465  ssor.create_mode
-00000350: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
-00000360: 0000 0500 0000 0f00 0000 732c 0000 0074  ..........s,...t
-00000370: 0083 006a 017c 017c 006a 0266 0164 0164  ...j.|.|.j.f.d.d
-00000380: 029c 027c 02a4 018e 0101 0064 037c 005f  ...|.......d.|._
-00000390: 0364 047c 005f 0464 0053 0029 054e 720f  .d.|._.d.S.).Nr.
-000003a0: 0000 0072 1000 0000 7212 0000 0072 0c00  ...r....r....r..
-000003b0: 0000 2905 da05 7375 7065 72da 085f 5f69  ..)...super..__i
-000003c0: 6e69 745f 5f72 1300 0000 7214 0000 0072  nit__r....r....r
-000003d0: 1600 0000 2903 da04 7365 6c66 7218 0000  ....)...selfr...
-000003e0: 0072 1900 0000 a901 da09 5f5f 636c 6173  .r........__clas
-000003f0: 735f 5f72 1b00 0000 721c 0000 0072 1f00  s__r....r....r..
-00000400: 0000 2100 0000 7306 0000 001c 0206 010a  ..!...s.........
-00000410: 017a 1747 414d 4c50 5265 6772 6573 736f  .z.GAMLPRegresso
-00000420: 722e 5f5f 696e 6974 5f5f e90a 0000 0063  r.__init__.....c
-00000430: 0400 0000 0000 0000 0000 0000 0a00 0000  ................
-00000440: 0600 0000 0f00 0000 735c 0000 0088 006a  ........s\.....j
-00000450: 0064 0119 007d 0688 016a 0064 0119 007d  .d...}...j.d...}
-00000460: 0747 0087 0087 0187 0287 0387 0466 0564  .G...........f.d
-00000470: 0264 0384 0864 0374 0183 037d 0874 027c  .d...d.t...}.t.|
-00000480: 0819 007d 097c 096a 037c 037c 0688 036a  ...}.|.j.|.|...j
-00000490: 0466 0288 036a 0488 036a 047c 0766 027c  .f...j...j.|.f.|
-000004a0: 0766 0464 048d 0253 0029 054e 720f 0000  .f.d...S.).Nr...
-000004b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000004c0: 0000 0400 0000 0000 0000 7336 0000 0065  ..........s6...e
-000004d0: 005a 0164 005a 0265 0365 0465 0365 0466  .Z.d.Z.e.e.e.e.f
-000004e0: 045a 0587 0087 0166 0264 0164 0284 085a  .Z.....f.d.d...Z
-000004f0: 0687 0287 0387 0466 0364 0364 0484 085a  .......f.d.d...Z
-00000500: 0764 0553 0029 067a 2b47 414d 4c50 5265  .d.S.).z+GAMLPRe
-00000510: 6772 6573 736f 722e 636f 6e66 6967 2e3c  gressor.config.<
-00000520: 6c6f 6361 6c73 3e2e 4d79 496e 6469 7669  locals>.MyIndivi
-00000530: 6475 616c 6301 0000 0000 0000 0000 0000  dualc...........
-00000540: 0002 0000 0004 0000 0013 0000 0073 1400  .............s..
-00000550: 0000 7c00 a000 a100 7d01 7c01 a001 8800  ..|.....}.|.....
-00000560: 8801 a102 5300 2901 4e29 02da 0664 6563  ....S.).N)...dec
-00000570: 6f64 65da 0573 636f 7265 a902 7220 0000  ode..score..r ..
-00000580: 0072 1a00 0000 2902 da01 58da 0159 721b  .r....)...X..Yr.
-00000590: 0000 0072 1c00 0000 da08 5f66 6974 6e65  ...r......_fitne
-000005a0: 7373 3200 0000 7304 0000 0008 010c 017a  ss2...s........z
-000005b0: 3447 414d 4c50 5265 6772 6573 736f 722e  4GAMLPRegressor.
-000005c0: 636f 6e66 6967 2e3c 6c6f 6361 6c73 3e2e  config.<locals>.
-000005d0: 4d79 496e 6469 7669 6475 616c 2e5f 6669  MyIndividual._fi
-000005e0: 746e 6573 7363 0100 0000 0000 0000 0000  tnessc..........
-000005f0: 0000 0200 0000 0700 0000 1300 0000 7352  ..............sR
-00000600: 0000 0088 016a 0088 0069 0088 02a4 018e  .....j...i......
-00000610: 017d 0174 0174 0274 036a 047c 0064 0064  .}.t.t.t.j.|.d.d
-00000620: 0064 0185 0319 0083 0283 017c 015f 0574  .d.........|._.t
-00000630: 0174 0274 036a 047c 0064 0264 0064 0185  .t.t.j.|.d.d.d..
-00000640: 0319 0083 0283 017c 015f 0664 037c 015f  .......|._.d.|._
-00000650: 077c 0153 0029 044e 7203 0000 0072 0f00  .|.S.).Nr....r..
-00000660: 0000 720c 0000 0029 0872 1d00 0000 da05  ..r....).r......
-00000670: 7475 706c 65da 036d 6170 da02 6e70 da07  tuple..map..np..
-00000680: 6173 6172 7261 7972 0d00 0000 720e 0000  asarrayr....r...
-00000690: 0072 1600 0000 7226 0000 0029 0372 1800  .r....r&...).r..
-000006a0: 0000 7217 0000 0072 1900 0000 721b 0000  ..r....r....r...
-000006b0: 0072 1c00 0000 7224 0000 0036 0000 0073  .r....r$...6...s
-000006c0: 0a00 0000 1001 1c01 1c01 0601 0401 7a32  ..............z2
-000006d0: 4741 4d4c 5052 6567 7265 7373 6f72 2e63  GAMLPRegressor.c
-000006e0: 6f6e 6669 672e 3c6c 6f63 616c 733e 2e4d  onfig.<locals>.M
-000006f0: 7949 6e64 6976 6964 7561 6c2e 6465 636f  yIndividual.deco
-00000700: 6465 4e29 08da 085f 5f6e 616d 655f 5fda  deN)...__name__.
-00000710: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000720: 7561 6c6e 616d 655f 5f72 0600 0000 7205  ualname__r....r.
-00000730: 0000 00da 0d65 6c65 6d65 6e74 5f63 6c61  .....element_cla
-00000740: 7373 7229 0000 0072 2400 0000 721b 0000  ssr)...r$...r...
-00000750: 00a9 0572 2700 0000 7228 0000 0072 1800  ...r'...r(...r..
-00000760: 0000 7217 0000 0072 1900 0000 721b 0000  ..r....r....r...
-00000770: 0072 1c00 0000 da0c 4d79 496e 6469 7669  .r......MyIndivi
-00000780: 6475 616c 2e00 0000 7308 0000 0008 000c  dual....s.......
-00000790: 020e 0214 0472 3300 0000 2902 da0d 6e5f  .....r3...)...n_
-000007a0: 696e 6469 7669 6475 616c 73da 0473 697a  individuals..siz
-000007b0: 6529 05da 0573 6861 7065 7204 0000 0072  e)...shaper....r
-000007c0: 0700 0000 da06 7261 6e64 6f6d 7213 0000  ......randomr...
-000007d0: 0029 0a72 1700 0000 7227 0000 0072 2800  .).r....r'...r(.
-000007e0: 0000 7234 0000 0072 1800 0000 7219 0000  ..r4...r....r...
-000007f0: 005a 0969 6e70 7574 5f64 696d 5a0a 6f75  .Z.input_dimZ.ou
-00000800: 7470 7574 5f64 696d 7233 0000 005a 0c4d  tput_dimr3...Z.M
-00000810: 7950 6f70 756c 6174 696f 6e72 1b00 0000  yPopulationr....
-00000820: 7232 0000 0072 1c00 0000 da06 636f 6e66  r2...r......conf
-00000830: 6967 2700 0000 730a 0000 000a 040a 011c  ig'...s.........
-00000840: 0208 0f24 027a 1547 414d 4c50 5265 6772  ...$.z.GAMLPRegr
-00000850: 6573 736f 722e 636f 6e66 6967 2901 7223  essor.config).r#
-00000860: 0000 0029 0d72 2e00 0000 722f 0000 0072  ...).r....r/...r
-00000870: 3000 0000 da07 5f5f 646f 635f 5f72 1300  0.....__doc__r..
-00000880: 0000 7211 0000 0072 1500 0000 da10 6573  ..r....r......es
-00000890: 7469 6d61 7465 645f 7061 7261 6d73 da0b  timated_params..
-000008a0: 636c 6173 736d 6574 686f 6472 1d00 0000  classmethodr....
-000008b0: 721f 0000 0072 3800 0000 da0d 5f5f 636c  r....r8.....__cl
-000008c0: 6173 7363 656c 6c5f 5f72 1b00 0000 721b  asscell__r....r.
-000008d0: 0000 0072 2100 0000 721c 0000 0072 0900  ...r!...r....r..
-000008e0: 0000 0f00 0000 7316 0000 0008 0004 0104  ......s.........
-000008f0: 0304 0104 0104 0202 020a 010c 0702 0614  ................
-00000900: 0172 0900 0000 290e 7239 0000 00da 056e  .r....).r9.....n
-00000910: 756d 7079 722c 0000 005a 1673 6b6c 6561  umpyr,...Z.sklea
-00000920: 726e 2e6e 6575 7261 6c5f 6e65 7477 6f72  rn.neural_networ
-00000930: 6b72 0200 0000 da00 7204 0000 0072 0500  kr......r....r..
-00000940: 0000 7206 0000 00da 0a70 6f70 756c 6174  ..r......populat
-00000950: 696f 6e72 0700 0000 da05 6c65 6172 6e72  ionr......learnr
-00000960: 0800 0000 7209 0000 0072 1b00 0000 721b  ....r....r....r.
-00000970: 0000 0072 1b00 0000 721c 0000 00da 083c  ...r....r......<
-00000980: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-00000990: 0402 0803 0c02 1402 0c01 0c01 1603       ..............
+000002c0: 0000 fa4b 2f55 7365 7273 2f77 696c 6c69  ...K/Users/willi
+000002d0: 616d 2f50 726f 6772 616d 6d69 6e67 2f50  am/Programming/P
+000002e0: 7974 686f 6e2f 6d79 776f 726b 2f70 7972  ython/mywork/pyr
+000002f0: 696d 6964 696e 652f 6c65 6172 6e2f 6e65  imidine/learn/ne
+00000300: 7572 616c 5f6e 6574 776f 726b 2e70 79da  ural_network.py.
+00000310: 0c63 7265 6174 655f 6d6f 6465 6c19 0000  .create_model...
+00000320: 0073 0800 0000 1803 0601 0801 0401 7a1b  .s............z.
+00000330: 4741 4d4c 5052 6567 7265 7373 6f72 2e63  GAMLPRegressor.c
+00000340: 7265 6174 655f 6d6f 6465 6c63 0100 0000  reate_modelc....
+00000350: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+00000360: 0f00 0000 732c 0000 0074 0083 006a 017c  ....s,...t...j.|
+00000370: 017c 006a 0266 0164 0164 029c 027c 02a4  .|.j.f.d.d...|..
+00000380: 018e 0101 0064 037c 005f 0364 047c 005f  .....d.|._.d.|._
+00000390: 0464 0053 0029 054e 720f 0000 0072 1000  .d.S.).Nr....r..
+000003a0: 0000 7212 0000 0072 0c00 0000 2905 da05  ..r....r....)...
+000003b0: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
+000003c0: 1300 0000 7214 0000 0072 1600 0000 2903  ....r....r....).
+000003d0: da04 7365 6c66 7218 0000 0072 1900 0000  ..selfr....r....
+000003e0: a901 da09 5f5f 636c 6173 735f 5f72 1b00  ....__class__r..
+000003f0: 0000 721c 0000 0072 1f00 0000 2100 0000  ..r....r....!...
+00000400: 7306 0000 001c 0206 010a 017a 1747 414d  s..........z.GAM
+00000410: 4c50 5265 6772 6573 736f 722e 5f5f 696e  LPRegressor.__in
+00000420: 6974 5f5f e90a 0000 0063 0400 0000 0000  it__.....c......
+00000430: 0000 0000 0000 0a00 0000 0600 0000 0f00  ................
+00000440: 0000 735c 0000 0088 006a 0064 0119 007d  ..s\.....j.d...}
+00000450: 0688 016a 0064 0119 007d 0747 0087 0087  ...j.d...}.G....
+00000460: 0187 0287 0387 0466 0564 0264 0384 0864  .......f.d.d...d
+00000470: 0374 0183 037d 0874 027c 0819 007d 097c  .t...}.t.|...}.|
+00000480: 096a 037c 037c 0688 036a 0466 0288 036a  .j.|.|...j.f...j
+00000490: 0488 036a 047c 0766 027c 0766 0464 048d  ...j.|.f.|.f.d..
+000004a0: 0253 0029 054e 720f 0000 0063 0000 0000  .S.).Nr....c....
+000004b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000004c0: 0000 0000 7336 0000 0065 005a 0164 005a  ....s6...e.Z.d.Z
+000004d0: 0265 0365 0465 0365 0466 045a 0587 0087  .e.e.e.e.f.Z....
+000004e0: 0166 0264 0164 0284 085a 0687 0287 0387  .f.d.d...Z......
+000004f0: 0466 0364 0364 0484 085a 0764 0553 0029  .f.d.d...Z.d.S.)
+00000500: 067a 2b47 414d 4c50 5265 6772 6573 736f  .z+GAMLPRegresso
+00000510: 722e 636f 6e66 6967 2e3c 6c6f 6361 6c73  r.config.<locals
+00000520: 3e2e 4d79 496e 6469 7669 6475 616c 6301  >.MyIndividualc.
+00000530: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000540: 0000 0013 0000 0073 1400 0000 7c00 a000  .......s....|...
+00000550: a100 7d01 7c01 a001 8800 8801 a102 5300  ..}.|.........S.
+00000560: 2901 4e29 02da 0664 6563 6f64 65da 0573  ).N)...decode..s
+00000570: 636f 7265 a902 7220 0000 0072 1a00 0000  core..r ...r....
+00000580: 2902 da01 58da 0159 721b 0000 0072 1c00  )...X..Yr....r..
+00000590: 0000 da08 5f66 6974 6e65 7373 3200 0000  ...._fitness2...
+000005a0: 7304 0000 0008 010c 017a 3447 414d 4c50  s........z4GAMLP
+000005b0: 5265 6772 6573 736f 722e 636f 6e66 6967  Regressor.config
+000005c0: 2e3c 6c6f 6361 6c73 3e2e 4d79 496e 6469  .<locals>.MyIndi
+000005d0: 7669 6475 616c 2e5f 6669 746e 6573 7363  vidual._fitnessc
+000005e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000005f0: 0700 0000 1300 0000 7352 0000 0088 016a  ........sR.....j
+00000600: 0088 0069 0088 02a4 018e 017d 0174 0174  ...i.......}.t.t
+00000610: 0274 036a 047c 0064 0064 0064 0185 0319  .t.j.|.d.d.d....
+00000620: 0083 0283 017c 015f 0574 0174 0274 036a  .....|._.t.t.t.j
+00000630: 047c 0064 0264 0064 0185 0319 0083 0283  .|.d.d.d........
+00000640: 017c 015f 0664 037c 015f 077c 0153 0029  .|._.d.|._.|.S.)
+00000650: 044e 7203 0000 0072 0f00 0000 720c 0000  .Nr....r....r...
+00000660: 0029 0872 1d00 0000 da05 7475 706c 65da  .).r......tuple.
+00000670: 036d 6170 da02 6e70 da07 6173 6172 7261  .map..np..asarra
+00000680: 7972 0d00 0000 720e 0000 0072 1600 0000  yr....r....r....
+00000690: 7226 0000 0029 0372 1800 0000 7217 0000  r&...).r....r...
+000006a0: 0072 1900 0000 721b 0000 0072 1c00 0000  .r....r....r....
+000006b0: 7224 0000 0036 0000 0073 0a00 0000 1001  r$...6...s......
+000006c0: 1c01 1c01 0601 0401 7a32 4741 4d4c 5052  ........z2GAMLPR
+000006d0: 6567 7265 7373 6f72 2e63 6f6e 6669 672e  egressor.config.
+000006e0: 3c6c 6f63 616c 733e 2e4d 7949 6e64 6976  <locals>.MyIndiv
+000006f0: 6964 7561 6c2e 6465 636f 6465 4e29 08da  idual.decodeN)..
+00000700: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000710: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000720: 655f 5f72 0600 0000 7205 0000 00da 0d65  e__r....r......e
+00000730: 6c65 6d65 6e74 5f63 6c61 7373 7229 0000  lement_classr)..
+00000740: 0072 2400 0000 721b 0000 00a9 0572 2700  .r$...r......r'.
+00000750: 0000 7228 0000 0072 1800 0000 7217 0000  ..r(...r....r...
+00000760: 0072 1900 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000770: da0c 4d79 496e 6469 7669 6475 616c 2e00  ..MyIndividual..
+00000780: 0000 7308 0000 0008 000c 020e 0214 0472  ..s............r
+00000790: 3300 0000 2902 da0d 6e5f 696e 6469 7669  3...)...n_indivi
+000007a0: 6475 616c 73da 0473 697a 6529 05da 0573  duals..size)...s
+000007b0: 6861 7065 7204 0000 0072 0700 0000 da06  haper....r......
+000007c0: 7261 6e64 6f6d 7213 0000 0029 0a72 1700  randomr....).r..
+000007d0: 0000 7227 0000 0072 2800 0000 7234 0000  ..r'...r(...r4..
+000007e0: 0072 1800 0000 7219 0000 005a 0969 6e70  .r....r....Z.inp
+000007f0: 7574 5f64 696d 5a0a 6f75 7470 7574 5f64  ut_dimZ.output_d
+00000800: 696d 7233 0000 005a 0c4d 7950 6f70 756c  imr3...Z.MyPopul
+00000810: 6174 696f 6e72 1b00 0000 7232 0000 0072  ationr....r2...r
+00000820: 1c00 0000 da06 636f 6e66 6967 2700 0000  ......config'...
+00000830: 730a 0000 000a 040a 011c 0208 0f24 027a  s............$.z
+00000840: 1547 414d 4c50 5265 6772 6573 736f 722e  .GAMLPRegressor.
+00000850: 636f 6e66 6967 2901 7223 0000 0029 0d72  config).r#...).r
+00000860: 2e00 0000 722f 0000 0072 3000 0000 da07  ....r/...r0.....
+00000870: 5f5f 646f 635f 5f72 1300 0000 7211 0000  __doc__r....r...
+00000880: 0072 1500 0000 da10 6573 7469 6d61 7465  .r......estimate
+00000890: 645f 7061 7261 6d73 da0b 636c 6173 736d  d_params..classm
+000008a0: 6574 686f 6472 1d00 0000 721f 0000 0072  ethodr....r....r
+000008b0: 3800 0000 da0d 5f5f 636c 6173 7363 656c  8.....__classcel
+000008c0: 6c5f 5f72 1b00 0000 721b 0000 0072 2100  l__r....r....r!.
+000008d0: 0000 721c 0000 0072 0900 0000 0f00 0000  ..r....r........
+000008e0: 7316 0000 0008 0004 0104 0304 0104 0104  s...............
+000008f0: 0202 020a 010c 0702 0614 0172 0900 0000  ...........r....
+00000900: 290e 7239 0000 00da 056e 756d 7079 722c  ).r9.....numpyr,
+00000910: 0000 005a 1673 6b6c 6561 726e 2e6e 6575  ...Z.sklearn.neu
+00000920: 7261 6c5f 6e65 7477 6f72 6b72 0200 0000  ral_networkr....
+00000930: da00 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
+00000940: 00da 0a70 6f70 756c 6174 696f 6e72 0700  ...populationr..
+00000950: 0000 da05 6c65 6172 6e72 0800 0000 7209  ....learnr....r.
+00000960: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000970: 0000 721c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000980: 3e01 0000 0073 0e00 0000 0402 0803 0c02  >....s..........
+00000990: 1402 0c01 0c01 1603                      ........
```

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/neural_network.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/neural_network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/regression.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/regression.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/__pycache__/regression.cpython-38.pyc` & `pyrimidine-1.6/pyrimidine/learn/__pycache__/regression.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/cluster.py` & `pyrimidine-1.6/pyrimidine/learn/cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
 
 """GA for linear regression
 """
 
 import numpy as np
 from sklearn.cluster import KMeans
-
-from ..chromosome import FloatChromosome
-from ..population import StandardPopulation
-
 from ..learn import BaseEstimator
 
+from .population import StandardPopulation
+
 
 class GALinearRegression(BaseEstimator, KMeans):
-    """Linear Regression by GA
-    """
+    '''Linear Regression by GA
+    '''
 
     estimated_params = ('cluster_centers_',)
 
     @classmethod
     def create_model(cls, *args, **kwargs):
         return KMeans(*args, **kwargs)
```

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/linear_regression.py` & `pyrimidine-1.6/pyrimidine/learn/linear_regression.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,30 @@
 
 """GA for linear regression
 """
 
 import numpy as np
 import numpy.linalg as LA
 from sklearn.linear_model import LinearRegression
-
-from ..chromosome import BinaryChromosome, FloatChromosome
-from ..individual import MixedIndividual
-from ..population import StandardPopulation
-
 from ..learn import BaseEstimator
 
+from ..population import StandardPopulation
 from digit_converter import IntervalConverter
 
-
 c = IntervalConverter(lb=-60, ub=60)
 class _BinaryChromosome(BinaryChromosome):
     def decode(self):
         return c(self)
 
 
 class GALinearRegression(BaseEstimator, LinearRegression):
     '''Linear Regression by GA
     '''
 
-    estimated_params = ('coef_', 'intercept_')
+    estimated_params = ('coefs_', 'intercepts_')
 
     @classmethod
     def create_model(cls, *args, **kwargs):
         return LinearRegression(*args, **kwargs)
 
     @classmethod
     def config(cls, X, Y, n_individuals=10, *args, **kwargs):
```

### Comparing `pyrimidine-1.5.6/pyrimidine/learn/neural_network.py` & `pyrimidine-1.6/pyrimidine/learn/neural_network.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/random_walk.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/local_search/__pycache__/random_walk.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 05:48:05 2023 UTC, .py size: 619 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b9 6e65 6b02 0000  o.........nek...
+00000000: 6f0d 0d0a 0000 0000 1ea4 6d65 6b02 0000  o.........mek...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6503 8303 5a04 6406 5300 2907 e900 0000  e...Z.d.S.).....
 00000060: 0029 01da 046e 6f72 6de9 0200 0000 2901  .)...norm.....).
 00000070: da0c 4669 746e 6573 734d 6978 696e 6300  ..FitnessMixinc.
@@ -23,50 +23,49 @@
 00000160: 6400 5300 6400 5300 2904 4e67 ae47 e17a  d.S.d.S.).Ng.G.z
 00000170: 14ae ef3f 2901 da07 6669 746e 6573 7372  ...?)...fitnessr
 00000180: 0100 0000 2905 7206 0000 00da 0463 6f70  ....).r......cop
 00000190: 79da 066d 7574 6174 6572 0800 0000 da0b  y..mutater......
 000001a0: 6368 726f 6d6f 736f 6d65 7329 07da 0473  chromosomes)...s
 000001b0: 656c 66da 016b da04 6172 6773 da06 6b77  elf..k..args..kw
 000001c0: 6172 6773 7206 0000 00da 0363 7079 da01  argsr......cpy..
-000001d0: 44a9 0072 1200 0000 fa55 2f55 7365 7273  D..r.....U/Users
+000001d0: 44a9 0072 1200 0000 fa4f 2f55 7365 7273  D..r.....O/Users
 000001e0: 2f77 696c 6c69 616d 2f50 726f 6772 616d  /william/Program
-000001f0: 6d69 6e67 2f6d 7947 6974 6875 622f 7079  ming/myGithub/py
-00000200: 7269 6d69 6469 6e65 2f70 7972 696d 6964  rimidine/pyrimid
-00000210: 696e 652f 6c6f 6361 6c5f 7365 6172 6368  ine/local_search
-00000220: 2f72 616e 646f 6d5f 7761 6c6b 2e70 79da  /random_walk.py.
-00000230: 0774 7261 6e73 6974 0f00 0000 7310 0000  .transit....s...
-00000240: 0012 010c 010a 010c 0208 0108 010c 0104  ................
-00000250: fe7a 1252 616e 646f 6d57 616c 6b2e 7472  .z.RandomWalk.tr
-00000260: 616e 7369 7463 0200 0000 0000 0000 0000  ansitc..........
-00000270: 0000 0200 0000 0300 0000 0300 0000 7322  ..............s"
-00000280: 0000 0074 0064 017c 0183 0289 0087 0066  ...t.d.|.......f
-00000290: 0164 0264 0384 0874 0144 0083 017c 005f  .d.d...t.D...|._
-000002a0: 0264 0053 0029 044e 7201 0000 0063 0100  .d.S.).Nr....c..
-000002b0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000002c0: 0000 1300 0000 731c 0000 0067 007c 005d  ......s....g.|.]
-000002d0: 0a7d 017c 0188 00a0 007c 016a 01a1 0117  .}.|.....|.j....
-000002e0: 0091 0271 0253 0072 1200 0000 2902 da03  ...q.S.r....)...
-000002f0: 7276 735a 076e 5f67 656e 6573 2902 da02  rvsZ.n_genes)...
-00000300: 2e30 da0a 6368 726f 6d6f 736f 6d65 a901  .0..chromosome..
-00000310: da01 6e72 1200 0000 7213 0000 00da 0a3c  ..nr....r......<
-00000320: 6c69 7374 636f 6d70 3e1b 0000 0073 0200  listcomp>....s..
-00000330: 0000 1c00 7a25 5261 6e64 6f6d 5761 6c6b  ....z%RandomWalk
-00000340: 2e6d 7574 6174 652e 3c6c 6f63 616c 733e  .mutate.<locals>
-00000350: 2e3c 6c69 7374 636f 6d70 3e29 0372 0200  .<listcomp>).r..
-00000360: 0000 7210 0000 0072 0b00 0000 2902 720c  ..r....r....).r.
-00000370: 0000 0072 0600 0000 7212 0000 0072 1800  ...r....r....r..
-00000380: 0000 7213 0000 0072 0a00 0000 1900 0000  ..r....r........
-00000390: 7304 0000 000a 0118 017a 1152 616e 646f  s........z.Rando
-000003a0: 6d57 616c 6b2e 6d75 7461 7465 4e29 07da  mWalk.mutateN)..
-000003b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000003c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000003d0: 655f 5fda 075f 5f64 6f63 5f5f da06 7061  e__..__doc__..pa
-000003e0: 7261 6d73 7214 0000 0072 0a00 0000 7212  ramsr....r....r.
-000003f0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000400: 0000 7205 0000 0009 0000 0073 0a00 0000  ..r........s....
-00000410: 0800 0401 0803 0802 0c0a 7205 0000 004e  ..........r....N
-00000420: 2905 da0b 7363 6970 792e 7374 6174 7372  )...scipy.statsr
-00000430: 0200 0000 da05 6d69 7869 6e72 0400 0000  ......mixinr....
-00000440: 7205 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00000450: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
-00000460: 6c65 3e01 0000 0073 0600 0000 0c03 0c02  le>....s........
-00000470: 1403                                     ..
+000001f0: 6d69 6e67 2f50 7974 686f 6e2f 6d79 776f  ming/Python/mywo
+00000200: 726b 2f70 7972 696d 6964 696e 652f 6c6f  rk/pyrimidine/lo
+00000210: 6361 6c5f 7365 6172 6368 2f72 616e 646f  cal_search/rando
+00000220: 6d5f 7761 6c6b 2e70 79da 0774 7261 6e73  m_walk.py..trans
+00000230: 6974 0f00 0000 7310 0000 0012 010c 010a  it....s.........
+00000240: 010c 0208 0108 010c 0104 fe7a 1252 616e  ...........z.Ran
+00000250: 646f 6d57 616c 6b2e 7472 616e 7369 7463  domWalk.transitc
+00000260: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000270: 0300 0000 0300 0000 7322 0000 0074 0064  ........s"...t.d
+00000280: 017c 0183 0289 0087 0066 0164 0264 0384  .|.......f.d.d..
+00000290: 0874 0144 0083 017c 005f 0264 0053 0029  .t.D...|._.d.S.)
+000002a0: 044e 7201 0000 0063 0100 0000 0000 0000  .Nr....c........
+000002b0: 0000 0000 0200 0000 0600 0000 1300 0000  ................
+000002c0: 731c 0000 0067 007c 005d 0a7d 017c 0188  s....g.|.].}.|..
+000002d0: 00a0 007c 016a 01a1 0117 0091 0271 0253  ...|.j.......q.S
+000002e0: 0072 1200 0000 2902 da03 7276 735a 076e  .r....)...rvsZ.n
+000002f0: 5f67 656e 6573 2902 da02 2e30 da0a 6368  _genes)....0..ch
+00000300: 726f 6d6f 736f 6d65 a901 da01 6e72 1200  romosome....nr..
+00000310: 0000 7213 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000320: 6d70 3e1b 0000 0073 0200 0000 1c00 7a25  mp>....s......z%
+00000330: 5261 6e64 6f6d 5761 6c6b 2e6d 7574 6174  RandomWalk.mutat
+00000340: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00000350: 636f 6d70 3e29 0372 0200 0000 7210 0000  comp>).r....r...
+00000360: 0072 0b00 0000 2902 720c 0000 0072 0600  .r....).r....r..
+00000370: 0000 7212 0000 0072 1800 0000 7213 0000  ..r....r....r...
+00000380: 0072 0a00 0000 1900 0000 7304 0000 000a  .r........s.....
+00000390: 0118 017a 1152 616e 646f 6d57 616c 6b2e  ...z.RandomWalk.
+000003a0: 6d75 7461 7465 4e29 07da 085f 5f6e 616d  mutateN)...__nam
+000003b0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000003c0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+000003d0: 5f64 6f63 5f5f da06 7061 7261 6d73 7214  _doc__..paramsr.
+000003e0: 0000 0072 0a00 0000 7212 0000 0072 1200  ...r....r....r..
+000003f0: 0000 7212 0000 0072 1300 0000 7205 0000  ..r....r....r...
+00000400: 0009 0000 0073 0a00 0000 0800 0401 0803  .....s..........
+00000410: 0802 0c0a 7205 0000 004e 2905 da0b 7363  ....r....N)...sc
+00000420: 6970 792e 7374 6174 7372 0200 0000 da05  ipy.statsr......
+00000430: 6d69 7869 6e72 0400 0000 7205 0000 0072  mixinr....r....r
+00000440: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000450: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000460: 0073 0600 0000 0c03 0c02 1403            .s..........
```

### Comparing `pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/simulated_annealing.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/local_search/__pycache__/simulated_annealing.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan  2 04:14:18 2024 UTC, .py size: 1344 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a8d 9365 4005 0000  o..........e@...
+00000000: 6f0d 0d0a 0000 0000 8b9f 6d65 8605 0000  o.........me....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d03 5a03 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6502 8303 5a04 6406 5300 2907  ..d.e...Z.d.S.).
 00000060: 7a95 0a53 696d 756c 6174 6564 2041 6e6e  z..Simulated Ann
 00000070: 6561 6c69 6e67 2041 6c67 6f72 6974 686d  ealing Algorithm
@@ -13,79 +13,82 @@
 000000c0: 6174 696f 6e20 6279 2053 696d 756c 6174  ation by Simulat
 000000d0: 6564 2041 6e6e 6561 6c69 6e67 2e20 3139  ed Annealing. 19
 000000e0: 3833 3a20 3232 3028 3435 3938 293a 2036  83: 220(4598): 6
 000000f0: 3731 2d36 3739 0ae9 0200 0000 2901 da11  71-679......)...
 00000100: 5068 616e 746f 6d49 6e64 6976 6964 7561  PhantomIndividua
 00000110: 6c29 01da 0f6d 6574 726f 706f 6c69 735f  l)...metropolis_
 00000120: 7275 6c65 6300 0000 0000 0000 0000 0000  rulec...........
-00000130: 0000 0000 0006 0000 0040 0000 0073 3000  .........@...s0.
+00000130: 0000 0000 0006 0000 0040 0000 0073 3400  .........@...s4.
 00000140: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000150: 6402 6403 6404 6405 6406 9c05 5a04 6407  d.d.d.d.d...Z.d.
-00000160: 6408 8400 5a05 6409 640a 8400 5a06 640b  d...Z.d.d...Z.d.
-00000170: 5300 290c da12 5369 6d75 6c61 7465 6441  S.)...SimulatedA
-00000180: 6e6e 6561 6c69 6e67 7a5f 436c 6173 7320  nnealingz_Class 
-00000190: 666f 7220 5369 6d75 6c61 7465 6420 416e  for Simulated An
-000001a0: 6e65 616c 696e 670a 2020 2020 0a20 2020  nealing.    .   
-000001b0: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-000001c0: 2020 2020 2070 6172 616d 7320 2864 6963       params (dic
-000001d0: 7429 3a20 7061 7261 6d65 7465 7273 2069  t): parameters i
-000001e0: 6e20 5341 0a20 2020 2067 ae47 e17a 14ae  n SA.    g.G.z..
-000001f0: ef3f e9c8 0000 00e9 6400 0000 672d 431c  .?......d...g-C.
-00000200: ebe2 361a 3f29 05da 0565 7874 5f63 da05  ..6.?)...ext_c..
-00000210: 696e 745f 63da 086e 5f65 706f 6368 73da  int_c..n_epochs.
-00000220: 0569 6e69 7454 da05 7465 726d 5463 0100  .initT..termTc..
-00000230: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-00000240: 0000 4f00 0000 7350 0000 007c 006a 007d  ..O...sP...|.j.}
-00000250: 0374 017c 006a 0283 0144 005d 137d 047c  .t.|.j...D.].}.|
-00000260: 00a0 037c 03a1 0101 007c 037c 006a 0439  ...|.....|.|.j.9
-00000270: 007d 037c 037c 006a 056b 0072 1b01 006e  .}.|.|.j.k.r...n
-00000280: 0171 087c 00a0 06a1 0001 007c 037c 006a  .q.|.......|.|.j
-00000290: 0714 007c 005f 0064 0053 0029 014e 2908  ...|._.d.S.).N).
-000002a0: 720a 0000 00da 0572 616e 6765 7209 0000  r......ranger...
-000002b0: 00da 046d 6f76 6572 0800 0000 720b 0000  ...mover....r...
-000002c0: 00da 0662 6163 6b75 7072 0700 0000 2905  ...backupr....).
-000002d0: da04 7365 6c66 da04 6172 6773 da06 6b77  ..self..args..kw
-000002e0: 6172 6773 da01 54da 0565 706f 6368 a900  args..T..epoch..
-000002f0: 7214 0000 00fa 652f 5573 6572 732f 7769  r.....e/Users/wi
-00000300: 6c6c 6961 6d2f 5072 6f67 7261 6d6d 696e  lliam/Programmin
-00000310: 672f 6d79 4769 7468 7562 2f70 7972 696d  g/myGithub/pyrim
-00000320: 6964 696e 652f 646f 6373 2f2e 2e2f 7079  idine/docs/../py
-00000330: 7269 6d69 6469 6e65 2f6c 6f63 616c 5f73  rimidine/local_s
-00000340: 6561 7263 682f 7369 6d75 6c61 7465 645f  earch/simulated_
-00000350: 616e 6e65 616c 696e 672e 7079 da0a 7472  annealing.py..tr
-00000360: 616e 7369 7469 6f6e 1e00 0000 7312 0000  ansition....s...
-00000370: 0006 010e 010a 010a 010a 0104 0102 ff08  ................
-00000380: 0310 017a 1d53 696d 756c 6174 6564 416e  ...z.SimulatedAn
-00000390: 6e65 616c 696e 672e 7472 616e 7369 7469  nealing.transiti
-000003a0: 6f6e 6302 0000 0000 0000 0000 0000 0004  onc.............
-000003b0: 0000 0004 0000 0043 0000 0073 3600 0000  .......C...s6...
-000003c0: 7c00 6a00 a001 a100 7d02 7402 7c02 6a03  |.j.....}.t.|.j.
-000003d0: 7c00 6a00 6a03 1800 7c01 6401 8d02 7d03  |.j.j...|.d...}.
-000003e0: 7c03 7219 7c02 6a04 7c00 6a00 5f04 6402  |.r.|.j.|.j._.d.
-000003f0: 5300 6402 5300 2903 7a57 4d6f 7665 2070  S.d.S.).zWMove p
-00000400: 6861 6e74 6f6d 0a20 2020 2020 2020 200a  hantom.        .
-00000410: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-00000420: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00000430: 207b 6e75 6d62 6572 7d20 2d2d 2074 656d   {number} -- tem
-00000440: 7065 7261 7475 7265 0a20 2020 2020 2020  perature.       
-00000450: 2029 02da 0144 7212 0000 004e 2905 da07   )...Dr....N)...
-00000460: 7068 616e 746f 6dda 0d67 6574 5f6e 6569  phantom..get_nei
-00000470: 6768 626f 7572 7203 0000 00da 0766 6974  ghbourr......fit
-00000480: 6e65 7373 da0b 6368 726f 6d6f 736f 6d65  ness..chromosome
-00000490: 7329 0472 0f00 0000 7212 0000 00da 0363  s).r....r......c
-000004a0: 7079 da04 666c 6167 7214 0000 0072 1400  py..flagr....r..
-000004b0: 0000 7215 0000 0072 0d00 0000 2900 0000  ..r....r....)...
-000004c0: 730a 0000 000a 0716 0304 010e 0104 ff7a  s..............z
-000004d0: 1753 696d 756c 6174 6564 416e 6e65 616c  .SimulatedAnneal
-000004e0: 696e 672e 6d6f 7665 4e29 07da 085f 5f6e  ing.moveN)...__n
-000004f0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000500: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000510: 075f 5f64 6f63 5f5f da06 7061 7261 6d73  .__doc__..params
-00000520: 7216 0000 0072 0d00 0000 7214 0000 0072  r....r....r....r
-00000530: 1400 0000 7214 0000 0072 1500 0000 7204  ....r....r....r.
-00000540: 0000 0010 0000 0073 1400 0000 0800 0401  .......s........
-00000550: 0206 0201 0201 0201 0201 06fc 0807 0c0b  ................
-00000560: 7204 0000 004e 2905 7221 0000 00da 0072  r....N).r!.....r
-00000570: 0200 0000 7203 0000 0072 0400 0000 7214  ....r....r....r.
-00000580: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00000590: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000005a0: 7308 0000 0004 030c 080c 0114 03         s............
+00000150: 5a04 6403 6403 6404 6405 6406 6407 9c05  Z.d.d.d.d.d.d...
+00000160: 5a05 6408 6409 8400 5a06 640a 640b 8400  Z.d.d...Z.d.d...
+00000170: 5a07 6402 5300 290c da12 5369 6d75 6c61  Z.d.S.)...Simula
+00000180: 7465 6441 6e6e 6561 6c69 6e67 7a91 436c  tedAnnealingz.Cl
+00000190: 6173 7320 666f 7220 5369 6d75 6c61 7465  ass for Simulate
+000001a0: 6420 416e 6e65 616c 696e 670a 2020 2020  d Annealing.    
+000001b0: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+000001c0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+000001d0: 2864 6963 7429 3a20 7061 7261 6d65 7465  (dict): paramete
+000001e0: 7273 2069 6e20 5341 0a20 2020 2020 2020  rs in SA.       
+000001f0: 2070 6861 6e74 6f6d 3a20 7068 616e 746f   phantom: phanto
+00000200: 6d20 736f 6c75 7469 6f6e 2066 6f72 2065  m solution for e
+00000210: 7870 6c6f 7261 7469 6f6e 0a20 2020 204e  xploration.    N
+00000220: 67ae 47e1 7a14 aeef 3fe9 c800 0000 e964  g.G.z...?......d
+00000230: 0000 0067 2d43 1ceb e236 1a3f 2905 da05  ...g-C...6.?)...
+00000240: 6578 745f 63da 0569 6e74 5f63 da08 6e5f  ext_c..int_c..n_
+00000250: 6570 6f63 6873 da05 696e 6974 54da 0574  epochs..initT..t
+00000260: 6572 6d54 6301 0000 0000 0000 0000 0000  ermTc...........
+00000270: 0005 0000 0004 0000 004f 0000 0073 5000  .........O...sP.
+00000280: 0000 7c00 6a00 7d03 7401 7c00 6a02 8301  ..|.j.}.t.|.j...
+00000290: 4400 5d13 7d04 7c00 a003 7c03 a101 0100  D.].}.|...|.....
+000002a0: 7c03 7c00 6a04 3900 7d03 7c03 7c00 6a05  |.|.j.9.}.|.|.j.
+000002b0: 6b00 721b 0100 6e01 7108 7c00 a006 a100  k.r...n.q.|.....
+000002c0: 0100 7c03 7c00 6a07 1400 7c00 5f00 6400  ..|.|.j...|._.d.
+000002d0: 5300 2901 4e29 0872 0a00 0000 da05 7261  S.).N).r......ra
+000002e0: 6e67 6572 0900 0000 da04 6d6f 7665 7208  nger......mover.
+000002f0: 0000 0072 0b00 0000 da06 6261 636b 7570  ...r......backup
+00000300: 7207 0000 0029 05da 0473 656c 66da 0461  r....)...self..a
+00000310: 7267 73da 066b 7761 7267 73da 0154 da05  rgs..kwargs..T..
+00000320: 6570 6f63 68a9 0072 1400 0000 fa57 2f55  epoch..r.....W/U
+00000330: 7365 7273 2f77 696c 6c69 616d 2f50 726f  sers/william/Pro
+00000340: 6772 616d 6d69 6e67 2f50 7974 686f 6e2f  gramming/Python/
+00000350: 6d79 776f 726b 2f70 7972 696d 6964 696e  mywork/pyrimidin
+00000360: 652f 6c6f 6361 6c5f 7365 6172 6368 2f73  e/local_search/s
+00000370: 696d 756c 6174 6564 5f61 6e6e 6561 6c69  imulated_anneali
+00000380: 6e67 2e70 79da 0a74 7261 6e73 6974 696f  ng.py..transitio
+00000390: 6e21 0000 0073 1200 0000 0601 0e01 0a01  n!...s..........
+000003a0: 0a01 0a01 0401 02ff 0803 1001 7a1d 5369  ............z.Si
+000003b0: 6d75 6c61 7465 6441 6e6e 6561 6c69 6e67  mulatedAnnealing
+000003c0: 2e74 7261 6e73 6974 696f 6e63 0200 0000  .transitionc....
+000003d0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+000003e0: 4300 0000 7336 0000 007c 006a 00a0 01a1  C...s6...|.j....
+000003f0: 007d 0274 027c 026a 037c 006a 006a 0318  .}.t.|.j.|.j.j..
+00000400: 007c 0164 018d 027d 037c 0372 197c 026a  .|.d...}.|.r.|.j
+00000410: 047c 006a 005f 0464 0253 0064 0253 0029  .|.j._.d.S.d.S.)
+00000420: 037a 574d 6f76 6520 7068 616e 746f 6d0a  .zWMove phantom.
+00000430: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000440: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
+00000450: 2020 2020 2020 2020 5420 7b6e 756d 6265          T {numbe
+00000460: 727d 202d 2d20 7465 6d70 6572 6174 7572  r} -- temperatur
+00000470: 650a 2020 2020 2020 2020 2902 da01 4472  e.        )...Dr
+00000480: 1200 0000 4e29 05da 0770 6861 6e74 6f6d  ....N)...phantom
+00000490: da0d 6765 745f 6e65 6967 6862 6f75 7272  ..get_neighbourr
+000004a0: 0300 0000 da07 6669 746e 6573 73da 0b63  ......fitness..c
+000004b0: 6872 6f6d 6f73 6f6d 6573 2904 720f 0000  hromosomes).r...
+000004c0: 0072 1200 0000 da03 6370 79da 0466 6c61  .r......cpy..fla
+000004d0: 6772 1400 0000 7214 0000 0072 1500 0000  gr....r....r....
+000004e0: 720d 0000 002c 0000 0073 0a00 0000 0a07  r....,...s......
+000004f0: 1603 0401 0e01 04ff 7a17 5369 6d75 6c61  ........z.Simula
+00000500: 7465 6441 6e6e 6561 6c69 6e67 2e6d 6f76  tedAnnealing.mov
+00000510: 6529 08da 085f 5f6e 616d 655f 5fda 0a5f  e)...__name__.._
+00000520: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000530: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000540: 7218 0000 00da 0670 6172 616d 7372 1600  r......paramsr..
+00000550: 0000 720d 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00000560: 0072 1400 0000 7215 0000 0072 0400 0000  .r....r....r....
+00000570: 1000 0000 7316 0000 0008 0004 0104 0702  ....s...........
+00000580: 0202 0102 0102 0102 0106 fc08 070c 0b72  ...............r
+00000590: 0400 0000 4e29 0572 2100 0000 da00 7202  ....N).r!.....r.
+000005a0: 0000 0072 0300 0000 7204 0000 0072 1400  ...r....r....r..
+000005b0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+000005c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000005d0: 0800 0000 0403 0c08 0c01 1403            ............
```

### Comparing `pyrimidine-1.5.6/pyrimidine/local_search/__pycache__/tabu_search.cpython-310.pyc` & `pyrimidine-1.6/pyrimidine/local_search/__pycache__/tabu_search.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Dec 10 12:40:49 2023 UTC, .py size: 1871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d1b1 7565 4f07 0000  o.........ueO...
+00000000: 6f0d 0d0a 0000 0000 17b2 7565 4f07 0000  o.........ueO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6507 4700 6405  d.l.m.Z...e.G.d.
 00000060: 6406 8400 6406 6502 8303 8301 5a08 4700  d...d.e.....Z.G.
 00000070: 6407 6408 8400 6408 6508 8303 5a09 6409  d.d...d.e...Z.d.
@@ -47,74 +47,73 @@
 000002e0: 720d 0000 00da 0b63 6872 6f6d 6f73 6f6d  r......chromosom
 000002f0: 6573 da0a 7365 745f 6d65 6d6f 7279 da06  es..set_memory..
 00000300: 6465 636f 6465 7203 0000 00da 0661 7070  decoder......app
 00000310: 656e 64da 0672 656d 6f76 65da 1075 7064  end..remove..upd
 00000320: 6174 655f 7461 6275 5f6c 6973 7429 05da  ate_tabu_list)..
 00000330: 0473 656c 66da 0461 7267 73da 066b 7761  .self..args..kwa
 00000340: 7267 73da 0661 6374 696f 6eda 0363 7079  rgs..action..cpy
-00000350: a900 721b 0000 00fa 552f 5573 6572 732f  ..r.....U/Users/
+00000350: a900 721b 0000 00fa 4f2f 5573 6572 732f  ..r.....O/Users/
 00000360: 7769 6c6c 6961 6d2f 5072 6f67 7261 6d6d  william/Programm
-00000370: 696e 672f 6d79 4769 7468 7562 2f70 7972  ing/myGithub/pyr
-00000380: 696d 6964 696e 652f 7079 7269 6d69 6469  imidine/pyrimidi
-00000390: 6e65 2f6c 6f63 616c 5f73 6561 7263 682f  ne/local_search/
-000003a0: 7461 6275 5f73 6561 7263 682e 7079 da0a  tabu_search.py..
-000003b0: 7472 616e 7369 7469 6f6e 1700 0000 7330  transition....s0
-000003c0: 0000 000a 010a 010a 010c 0108 0104 0104  ................
-000003d0: 0106 010a fe0a 0508 0104 0104 0106 010a  ................
-000003e0: fe0e 050c 0208 0104 0104 0106 0108 fe0c  ................
-000003f0: 040c 017a 1942 6173 6554 6162 7553 6561  ...z.BaseTabuSea
-00000400: 7263 682e 7472 616e 7369 7469 6f6e 6301  rch.transitionc.
-00000410: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000420: 0000 0043 0000 0073 2400 0000 7400 7c00  ...C...s$...t.|.
-00000430: 6a01 8301 7c00 6a02 6b04 7210 7c00 6a01  j...|.j.k.r.|.j.
-00000440: a003 6401 a101 0100 6400 5300 6400 5300  ..d.....d.S.d.S.
-00000450: 2902 4e72 0700 0000 2904 da03 6c65 6e72  ).Nr....)...lenr
-00000460: 0a00 0000 720c 0000 00da 0370 6f70 2901  ....r......pop).
-00000470: 7216 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00000480: 1c00 0000 7215 0000 0034 0000 0073 0600  ....r....4...s..
-00000490: 0000 1001 1001 04ff 7a1f 4261 7365 5461  ........z.BaseTa
-000004a0: 6275 5365 6172 6368 2e75 7064 6174 655f  buSearch.update_
-000004b0: 7461 6275 5f6c 6973 7463 0200 0000 0000  tabu_listc......
-000004c0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-000004d0: 0000 7304 0000 0074 0082 01a9 014e 2901  ..s....t.....N).
-000004e0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-000004f0: 4572 726f 7229 0272 1600 0000 7219 0000  Error).r....r...
-00000500: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000510: 720f 0000 0038 0000 0073 0200 0000 0401  r....8...s......
-00000520: 7a1c 4261 7365 5461 6275 5365 6172 6368  z.BaseTabuSearch
-00000530: 2e67 6574 5f6e 6569 6768 626f 7572 4e29  .get_neighbourN)
-00000540: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000550: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000560: 616d 655f 5fda 075f 5f64 6f63 5f5f da06  ame__..__doc__..
-00000570: 7061 7261 6d73 721d 0000 0072 1500 0000  paramsr....r....
-00000580: 720f 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00000590: 1b00 0000 721c 0000 0072 0600 0000 0c00  ....r....r......
-000005a0: 0000 7314 0000 0008 0004 0202 0302 0102  ..s.............
-000005b0: 0102 0106 fd08 0608 1d0c 0472 0600 0000  ...........r....
-000005c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000005d0: 0002 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-000005e0: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-000005f0: 5300 2904 da10 5369 6d70 6c65 5461 6275  S.)...SimpleTabu
-00000600: 5365 6172 6368 6302 0000 0000 0000 0000  Searchc.........
-00000610: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
-00000620: 2800 0000 7c00 a000 a100 7d02 7c01 5c02  (...|.....}.|.\.
-00000630: 7d03 7d04 7c02 6a01 a002 a100 7c02 6a03  }.}.|.j.....|.j.
-00000640: 7c03 1900 7c04 3c00 7c02 5300 7220 0000  |...|.<.|.S.r ..
-00000650: 0029 04da 0463 6f70 79da 0467 656e 6572  .)...copy..gener
-00000660: 0300 0000 7210 0000 0029 0572 1600 0000  ....r....).r....
-00000670: 7219 0000 0072 1a00 0000 da01 69da 016a  r....r......i..j
-00000680: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00000690: 0f00 0000 3e00 0000 7308 0000 0008 0108  ....>...s.......
-000006a0: 0114 0104 017a 1e53 696d 706c 6554 6162  .....z.SimpleTab
-000006b0: 7553 6561 7263 682e 6765 745f 6e65 6967  uSearch.get_neig
-000006c0: 6862 6f75 724e 2904 7222 0000 0072 2300  hbourN).r"...r#.
-000006d0: 0000 7224 0000 0072 0f00 0000 721b 0000  ..r$...r....r...
-000006e0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-000006f0: 7227 0000 003c 0000 0073 0400 0000 0800  r'...<...s......
-00000700: 0c02 7227 0000 004e 290a 7225 0000 00da  ..r'...N).r%....
-00000710: 0462 6173 6572 0200 0000 da05 7574 696c  .baser......util
-00000720: 7372 0300 0000 7204 0000 00da 0464 6563  sr....r......dec
-00000730: 6f72 0500 0000 7206 0000 0072 2700 0000  or....r....r'...
-00000740: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00000750: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000760: 0000 730e 0000 0004 020c 0410 010c 0102  ..s.............
-00000770: 0312 0114 2f                             ..../
+00000370: 696e 672f 5079 7468 6f6e 2f6d 7977 6f72  ing/Python/mywor
+00000380: 6b2f 7079 7269 6d69 6469 6e65 2f6c 6f63  k/pyrimidine/loc
+00000390: 616c 5f73 6561 7263 682f 7461 6275 5f73  al_search/tabu_s
+000003a0: 6561 7263 682e 7079 da0a 7472 616e 7369  earch.py..transi
+000003b0: 7469 6f6e 1700 0000 7330 0000 000a 010a  tion....s0......
+000003c0: 010a 010c 0108 0104 0104 0106 010a fe0a  ................
+000003d0: 0508 0104 0104 0106 010a fe0e 050c 0208  ................
+000003e0: 0104 0104 0106 0108 fe0c 040c 017a 1942  .............z.B
+000003f0: 6173 6554 6162 7553 6561 7263 682e 7472  aseTabuSearch.tr
+00000400: 616e 7369 7469 6f6e 6301 0000 0000 0000  ansitionc.......
+00000410: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000420: 0073 2400 0000 7400 7c00 6a01 8301 7c00  .s$...t.|.j...|.
+00000430: 6a02 6b04 7210 7c00 6a01 a003 6401 a101  j.k.r.|.j...d...
+00000440: 0100 6400 5300 6400 5300 2902 4e72 0700  ..d.S.d.S.).Nr..
+00000450: 0000 2904 da03 6c65 6e72 0a00 0000 720c  ..)...lenr....r.
+00000460: 0000 00da 0370 6f70 2901 7216 0000 0072  .....pop).r....r
+00000470: 1b00 0000 721b 0000 0072 1c00 0000 7215  ....r....r....r.
+00000480: 0000 0034 0000 0073 0600 0000 1001 1001  ...4...s........
+00000490: 04ff 7a1f 4261 7365 5461 6275 5365 6172  ..z.BaseTabuSear
+000004a0: 6368 2e75 7064 6174 655f 7461 6275 5f6c  ch.update_tabu_l
+000004b0: 6973 7463 0200 0000 0000 0000 0000 0000  istc............
+000004c0: 0200 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000004d0: 0074 0082 01a9 014e 2901 da13 4e6f 7449  .t.....N)...NotI
+000004e0: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
+000004f0: 0272 1600 0000 7219 0000 0072 1b00 0000  .r....r....r....
+00000500: 721b 0000 0072 1c00 0000 720f 0000 0038  r....r....r....8
+00000510: 0000 0073 0200 0000 0401 7a1c 4261 7365  ...s......z.Base
+00000520: 5461 6275 5365 6172 6368 2e67 6574 5f6e  TabuSearch.get_n
+00000530: 6569 6768 626f 7572 4e29 08da 085f 5f6e  eighbourN)...__n
+00000540: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000550: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000560: 075f 5f64 6f63 5f5f da06 7061 7261 6d73  .__doc__..params
+00000570: 721d 0000 0072 1500 0000 720f 0000 0072  r....r....r....r
+00000580: 1b00 0000 721b 0000 0072 1b00 0000 721c  ....r....r....r.
+00000590: 0000 0072 0600 0000 0c00 0000 7314 0000  ...r........s...
+000005a0: 0008 0004 0202 0302 0102 0102 0106 fd08  ................
+000005b0: 0608 1d0c 0472 0600 0000 6300 0000 0000  .....r....c.....
+000005c0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+000005d0: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000005e0: 6401 6402 8400 5a03 6403 5300 2904 da10  d.d...Z.d.S.)...
+000005f0: 5369 6d70 6c65 5461 6275 5365 6172 6368  SimpleTabuSearch
+00000600: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
+00000610: 0003 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
+00000620: a000 a100 7d02 7c01 5c02 7d03 7d04 7c02  ....}.|.\.}.}.|.
+00000630: 6a01 a002 a100 7c02 6a03 7c03 1900 7c04  j.....|.j.|...|.
+00000640: 3c00 7c02 5300 7220 0000 0029 04da 0463  <.|.S.r ...)...c
+00000650: 6f70 79da 0467 656e 6572 0300 0000 7210  opy..gener....r.
+00000660: 0000 0029 0572 1600 0000 7219 0000 0072  ...).r....r....r
+00000670: 1a00 0000 da01 69da 016a 721b 0000 0072  ......i..jr....r
+00000680: 1b00 0000 721c 0000 0072 0f00 0000 3e00  ....r....r....>.
+00000690: 0000 7308 0000 0008 0108 0114 0104 017a  ..s............z
+000006a0: 1e53 696d 706c 6554 6162 7553 6561 7263  .SimpleTabuSearc
+000006b0: 682e 6765 745f 6e65 6967 6862 6f75 724e  h.get_neighbourN
+000006c0: 2904 7222 0000 0072 2300 0000 7224 0000  ).r"...r#...r$..
+000006d0: 0072 0f00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000006e0: 721b 0000 0072 1c00 0000 7227 0000 003c  r....r....r'...<
+000006f0: 0000 0073 0400 0000 0800 0c02 7227 0000  ...s........r'..
+00000700: 004e 290a 7225 0000 00da 0462 6173 6572  .N).r%.....baser
+00000710: 0200 0000 da05 7574 696c 7372 0300 0000  ......utilsr....
+00000720: 7204 0000 00da 0464 6563 6f72 0500 0000  r......decor....
+00000730: 7206 0000 0072 2700 0000 721b 0000 0072  r....r'...r....r
+00000740: 1b00 0000 721b 0000 0072 1c00 0000 da08  ....r....r......
+00000750: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
+00000760: 0004 020c 0410 010c 0102 0312 0114 2f    ............../
```

### Comparing `pyrimidine-1.5.6/pyrimidine/local_search/random_walk.py` & `pyrimidine-1.6/pyrimidine/local_search/random_walk.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/local_search/simulated_annealing.py` & `pyrimidine-1.6/pyrimidine/local_search/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/local_search/tabu_search.py` & `pyrimidine-1.6/pyrimidine/local_search/tabu_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 #!/usr/bin/env python3
 
 """
 Tabu Search was created by Fred W. Glover in 1986 and formalized in 1989
+
+*References*
+Glover, Fred W. and Manuel Laguna. “Tabu Search.” (1997).
+Glover, Fred W.. “Tabu Search - Part I.” INFORMS J. Comput. 1 (1989): 190-206.
+Glover, Fred W.. “Tabu Search - Part II.” INFORMS J. Comput. 2 (1989): 4-32.
 """
 
 from ..base import BaseIndividual
 from ..utils import random, choice
 from ..deco import basic_memory
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrimidine-1.5.6/pyrimidine/meta.py` & `pyrimidine-1.6/pyrimidine/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 class MetaContainer(ParamType):
     """Meta class of containers
 
     A container is a algebric system with elements of some type
     and operators acting on the elements
 
     Example:
+
         ```
         from collections import UserString
         class C(metaclass=MetaContainer):
             # container of strings
             element_class = UserString
             alias = {'strings': 'elements'}
 
@@ -145,45 +146,54 @@
         print(c.n_strings)
         print(c[1])
         for a in c:
             print(a)
 
         c.regester('upper')
         print(c.upper())
-
-        # <class 'collections.UserString'>
-        # <property object at 0x1065715e0>
-        # ['I', 'love', 'you']
-        # for ever
-        # 3
-        # love
-        # I
-        # love
-        # you
-        # ['I', 'LOVE', 'YOU']
         ```
+
+    Output:
+
+        <class 'collections.UserString'>
+        <property object at 0x1065715e0>
+        ['I', 'love', 'you']
+        for ever
+        3
+        love
+        I
+        love
+        you
+        ['I', 'LOVE', 'YOU']
     """
 
     def __new__(cls, name, bases, attrs):
         """
         Users have to define `element_class` in the class.
         """
+
         if 'element_class' in attrs:
             element_class = attrs['element_class']
         else:
             for base in bases:
                 if hasattr(base, 'element_class'):
                     element_class = base.element_class
                     break
             else:
                 raise Exception('Have not provided element class yet.')
         
         def _getitem(self, k):
             # print(DeprecationWarning('get item directly is not recommended now.'))
-            return self.__elements[k]
+            try:
+                return self.__elements[k]
+            except:
+                if isinstance(k, Iterable):
+                    return [self[_] for _ in k]
+                else:
+                    raise TypeError(f'The index must be int/tuple/slice or list-like iterable object! But what you provided is {type(k)}')
 
         def _setitem(self, k, v):
             # print(DeprecationWarning('get item directly is not recommended now.'))
             self.__elements[k] =v
             self.after_setter()
 
         def _iter(self):
@@ -196,15 +206,16 @@
             return e in self.__elements
 
         attrs.update(
             {'__getitem__': _getitem,
             '__setitem__': _setitem,
             '__iter__': _iter,
             '__len__': _len,
-            '__contains__': _contains})
+            '__contains__': _contains}
+            )
 
         def _apply(self, f, *args, **kwargs):
             return self.map(lambda o: f(o, *args, **kwargs), self.__elements)
 
         @property
         def _n_elements(self):
             return len(self.__elements)
@@ -253,14 +264,15 @@
         attrs.update({'isa': _isa})
 
         """
         Regester maps and operands
         if the mapping f is regestered, then A owns method f, automatically
         f(A) := {f(a), a in A} where f is a method of A.
         """
+
         def _regester_map(self, name, key=None, force=True):
             if key is None:
                 key = methodcaller(name)
 
             _map = self.map if hasattr(self, 'map') else map
 
             def m(obj, *args, **kwargs):
@@ -314,16 +326,14 @@
             #     e.__system = o
         else:
             raise TypeError('missing a list/tuple of elements as the unique positional argument!')
 
         for k, v in kwargs.items():
             setattr(o, k, v)
 
-        # if '_environment' in globals():
-        #     o.environment = globals()['_environment']
         return o
 
     def __getitem__(self, class_):
         """Helper to construct a container
 
             `C[a] // n` is equiv. to
 
@@ -367,15 +377,14 @@
         if isinstance(self.element_class, tuple):
             return self([C.random(*args, **kwargs) for C in self.element_class])
         else:
             n_elements = n_elements or self.default_size
             return self([self.element_class.random(*args, **kwargs) for _ in range(n_elements)])
 
 
-
 # class System(MetaContainer):
 #     """Metaclass of systems, considered in future!
 
 #     A system is a type of container, that defines operators on them.
 #     """
     
 #     def __new__(cls, name, bases=(), attrs={}): 
@@ -513,15 +522,15 @@
 class MetaArray(ParamType):
 
     """Metaclass for chromosomes
 
     Chromosomes could be seen as a container of genes. But we implement them
     by the arrays for convenience.
     """
-    
+
     def __new__(cls, name, bases, attrs):
         if 'element_class' in attrs:
             element_class = attrs['element_class']
         else:
             for base in bases:
                 if hasattr(base, 'element_class'):
                     element_class = base.element_class
```

### Comparing `pyrimidine-1.5.6/pyrimidine/mixin.py` & `pyrimidine-1.6/pyrimidine/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,45 +92,46 @@
 
         if isinstance(stat, dict): stat = Statistics(stat)
         
         if initialize:
             self.init()
 
         if history is True:
-            res = stat(self) if stat else {}
+            res = stat(self)
             history = pd.DataFrame(data={k:[v] for k, v in res.items()})
             history_flag = True
         elif history is False:
             history_flag = False
         elif isinstance(history, pd.DataFrame):
             history_flag = True
         else:
             raise TypeError('The argument `history` should be an instance of `pandas.DataFrame` or `bool`.')
         # n_iter = n_iter or self.n_iter
         if verbose:
             from toolz.itertoolz import concat
             if not history_flag:
-                res = stat(self) if stat else {}
+                res = stat(self)
             print(f"""
 {" & ".join(concat((("iteration",), attrs, res.keys())))}
 -------------------------------------------------------------
-{" & ".join(map(str, concat((("[0]",), (getattr(self, attr) for attr in attrs), map(str, res.values())))))}""")
+{" & ".join(map(str, concat((("[0]",), (getattr(self, attr) for attr in attrs), res.values()))))}""")
 
         for t in range(1, n_iter+1):
             self.transition(t)
             if history_flag and (period == 1 or t % period ==0):
-                res = stat(self) if stat else {}
+                res = stat(self)
                 history = pd.concat([history,
                     pd.Series(res.values(), index=res.keys()).to_frame().T],
                     ignore_index=True)
             if verbose and (period == 1 or t % period ==0):
-                print(f'{" & ".join(map(str, concat((("[%d]"%t,), (getattr(self, attr) for attr in attrs), map(str, res.values())))))}')
-            
+                print(f'{" & ".join(map(str, concat((("[%d]"%t,), (getattr(self, attr) for attr in attrs), res.values()))))}')
+
             if control:
                 if control(self):
+                    # if it satisfies the control condition
                     break
         return history
 
     def perf(self, n_repeats=10, timing=True, *args, **kwargs):
         """Get performance of Algo.
 
         Keyword Arguments:
@@ -295,14 +296,20 @@
             return type_([c.copy(type_=t) for c, t in zip(self, type_.element_class)])
         else:
             return type_([c.copy(type_=element_class) for c in self])
 
     def clone(self):
         return self.__class__(list(map(methodcaller('clone'), self)))
 
+    # def diff_fitness(self):
+    #     return self.fitness - self.previous_fitness
+
+    # def previous_fitness(self):
+    #     return self.memory['fitness']
+
 
 class CollectiveMixin(IterativeMixin):
     # mixin class for swarm intelligent algorithm
 
     map = map
 
     def init(self, *args, **kwargs):
@@ -326,14 +333,22 @@
     def extend(self, inds):
         self.elements.extend(inds)
 
     @side_effect
     def append(self, ind):
         self.elements.append(ind)
 
+    def random_select(self, n_sel=None, copy=False):
+        if n_sel is None:
+            k = np.random.randint(len(self))
+            return self[k]
+        else:
+            ks = np.random.randint(len(self), size=n_sel)
+            return self[ks]
+
 
 class PopulationMixin(FitnessMixin, CollectiveMixin):
     """mixin class for population-based heuristic algorithm
 
     It is consisted of a collection of solutions.
     """
 
@@ -451,37 +466,54 @@
         return self[k]
 
     @property
     def solution(self):
         return self.best_element.decode()
 
     def get_worst_element(self, copy=False):
+        # see get_best_element
         k = np.argmin(self.get_all_fitness())
         if copy:
             return self[k].copy()
         else:
             return self[k]
 
+    def get_worst_elements(self, n=1, copy=False):
+        # see get_best_elements
+        if n < 1:
+            n = int(self.n_elements * n)
+        elif not isinstance(n, int):
+            n = int(n)
+
+        if copy:
+            return [self[k].copy() for k in self.argsort()[:n]]
+        else:
+            return [self[k] for k in self.argsort()[:n]]
+
     @property
     def worst_element(self):
         k = np.argmin(self.get_all_fitness())
         return self[k]
 
     def sorted_(self):
         # return a list of sorted individuals
         return [self[k] for k in self.argsort()]
 
     def sort(self):
         # sort the whole population
         ks = self.argsort()
-        self.__elements = [self[k] for k in ks]
+        self.__elements = self[ks]
 
     def argsort(self):
         return np.argsort(self.get_all_fitness())
 
     def drop(self, n=1):
         if n < 1:
             n = int(self.n_elements * n)
         elif not isinstance(n, int):
             n = int(n)
         ks = self.argsort()
         self.elements = [self[k] for k in ks[n:]]
+
+    def observe(self):
+        for o in self:
+            o._population = self
```

### Comparing `pyrimidine-1.5.6/pyrimidine/multipopulation.py` & `pyrimidine-1.6/pyrimidine/multipopulation.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/parallel.py` & `pyrimidine-1.6/pyrimidine/parallel.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/population.py` & `pyrimidine-1.6/pyrimidine/population.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 
 """Variants of Population classes
 
+A population is defined as a container of individuals.
+
 StandardPopulation: Standard Genetic Algorithm
 HOFPopulation: Standard Genetic Algorithm with hall of fame
 """
 
 from operator import methodcaller, attrgetter
 from random import gauss, random
```

### Comparing `pyrimidine-1.5.6/pyrimidine/pso.py` & `pyrimidine-1.6/pyrimidine/pso.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """Particle Swarm Optimization
 
 Developed by J. Kennedy and R. Eberhart[Kennedy and Eberhart 2001]
 
-Each individual is represented position and velocity.
+Each individual is represented by the position and the velocity.
 """
 
 from random import random
 from operator import attrgetter
 
 import numpy as np
```

### Comparing `pyrimidine-1.5.6/pyrimidine/qga.py` & `pyrimidine-1.6/pyrimidine/qga.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/saga.py` & `pyrimidine-1.6/pyrimidine/saga.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/sma.py` & `pyrimidine-1.6/pyrimidine/sma.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/studga.py` & `pyrimidine-1.6/pyrimidine/studga.py`

 * *Files identical despite different names*

### Comparing `pyrimidine-1.5.6/pyrimidine/utils.py` & `pyrimidine-1.6/pyrimidine/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,14 @@
     return i, j
 
 
 def max0(x):
     return np.maximum(x, 0)
 
 
-def max_lb(lb):
-    def m(x):
-        return np.maximum(x, lb)
-    return m
-
-
 def hl(x):
     return np.clip(x, 0, 1) 
 
 
 def metropolis_rule(D, T, epsilon=0.000001):
     """
     Metropolis rule
```

### Comparing `pyrimidine-1.5.6/setup.py` & `pyrimidine-1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,33 @@
  'pyrimidine.benchmarks',
  'pyrimidine.learn',
  'pyrimidine.local_search']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['matplotlib>=3.8.0,<4.0.0',
+ 'numpy>=1.26.0,<2.0.0',
+ 'pandas>=2.1.0,<3.0.0',
+ 'scikit-learn>=1.1.0,<2.0.0',
+ 'scipy>=1.12.0,<2.0.0',
+ 'toolz>=0.12.0,<0.13.0']
+
 setup_kwargs = {
     'name': 'pyrimidine',
-    'version': '1.5.6',
-    'description': 'A competitive framework for GA, designed by thorough OOP/Algebra-inspried Programming',
-    'long_description': '# pyrimidine\n\n`pyrimidine` is an extensible framework of genetic/evolutionary algorithm by Python. See [pyrimidine\'s document](https://pyrimidine.readthedocs.io/) for more details.\n\n![LOGO](logo.png)\n\n## Why\n\nWhy is the package named as “pyrimidine”? Because it begins with “py”.\n\n> — Are you kiding?\n>\n> — No, I am serious.\n\n## Download\n\nIt has been uploaded to [pypi](https://pypi.org/project/pyrimidine/), so download it with `pip install pyrimidine`, and also could download it from github.\n\n## Idea\n\nWe regard the population as a container of individuals, an individual as a container of chromosomes\nand a chromosome as a container(array) of genes.\n\nThe container could be a list or an array.\nThe container class has an attribute `element_class`, telling itself the type of the elements in it.\n\nFollowing is the part of the source code of `BaseIndividual` and `BasePopulation`.\n\n```python\nclass BaseIndividual(FitnessModel, metaclass=MetaContainer):\n    element_class = BaseChromosome\n    default_size = 1\n\nclass BasePopulation(PopulationModel, metaclass=MetaContainer):\n    element_class = BaseIndividual\n    default_size = 20\n```\n\nThere is mainly tow kinds of containers: list and tuple as in programming language `Haskell`. See following examples.\n\n```python\n# individual with chromosomes of type _Chromosome\n_Individual1 = BaseIndividual[_Choromosome]\n# individual with 2 chromosomes of type _Chromosome1 and _Chromosome2 respectively\n_Individual2 = MixedIndividual[_Chromosome1, _Chromosome2]\n```\n\n### Math expression\n$s$ of type $S$ is a container of $a:A$, represented as follows:\n\n```\ns={a:A}:S\n```\n\nWe define a population as a container of individuals or chromosomes, and an individual is a container of chromosomes.\n\nAlgebraically, an indivdiual has only one chromosome is equivalent to a chromosome mathematically. A population could also be a container of chromosomes. If the individual has only one chromosome, then just build the population based on chromosomes directly.\n\nThe methods are the functions or operators defined on $s$.\n\n## Use\n\n### Main classes\n\n- BaseGene: the gene of chromosome\n- BaseChromosome: sequence of genes, represents part of a solution\n- BaseIndividual: sequence of chromosomes, represents a solution of a problem\n- BasePopulation: a container of individuals, represents a container of a problem\n                also the state of a stachostic process\n- BaseMultipopulation: a container of population for more complicated optimalization\n\n\n### import\nJust use the command `from pyrimidine import *` import all of the algorithms.\n\n### subclass\n\n#### Chromosome\n\nGenerally, it is an array of genes.\n\nAs an array of 0-1s, `BinaryChromosome` is used most frequently.\n\n#### Individual\njust subclass `MonoIndividual` in most cases.\n\n```python\nclass MyIndividual(MonoIndividual):\n    """individual with only one chromosome\n    we set the gene is 0 or 1 in the chromosome\n    """\n    element_class = BinaryChromosome\n\n    def _fitness(self):\n        ...\n```\n\nSince the helper `makeIndividual(n_chromosomes=1, size=8)` could create such individual, it is equivalent to\n\n```python\nclass MyIndividual(binaryIndividual()):\n    # only need define the fitness\n    def _fitness(self):\n        ...\n```\n\n\nIf an individual contains several chromosomes, then subclass `MultiIndividual` or `PolyIndividual`. It could be applied in multi-real-variable optimization problems where each variable has a separative binary encoding.\n\n\nIn most cases, we have to decode chromosomes to real numbers.\n\n```python\nclass _Chromosome(BinaryChromosome):\n    def decode(self):\n        """Decode a binary chromosome\n        \n        if the sequence of 0-1 represents a real number, then overide the method\n        to transform it to a nubmer\n        """\n\nclass ExampleIndividual(BaseIndividual):\n    element_class = _Chromosome\n\n    def _fitness(self):\n        # define the method to calculate the fitness\n        x = self.decode()  # will call decode method of _Chromosome\n        return evaluate(x)\n```\n\n\nIf the chromosomes in an individual are different with each other, then subclass `MixedIndividual`, meanwhile, the property `element_class` should be assigned with a tuple of classes for each chromosome.\n\n```python\nclass MyIndividual(MixedIndividual):\n    """\n    Inherit the fitness from ExampleIndividual directly.\n    It has 6 chromosomes, 5 are instances of _Chromosome, 1 is instance of FloatChromosome\n    """\n    element_class = (_Chromosome,)*5 + (FloatChromosome,)\n```\n\nIt equivalent to `MyIndividual=MixedIndividual[(_Chromosome,)*5 + (FloatChromosome,)]`\n\n#### Population\n\n```python\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual\n```\n\nIt is equivalent to `MyPopulation = StandardPopulation[MyIndividual]`.\n\n\n### Initialize randomly\n\n`random` is a factory method!\n\nGenerate a population, with 50 individuals and each individual has 100 genes:\n\n`pop = MyPopulation.random(n_individuals=50, size=100)`\n\nWhen each individual contains 5 chromosomes, use\n\n`pop = MyPopulation.random(n_individuals=10, n_chromosomes=5, size=10)`\n\nHowever, we recommand to set `default_size` in the classes, then run `MyPopulation.random()`\n\n```python\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual // 5\n    default_size = 10\n\n# equiv. to\n\nMyPopulation = StandardPopulation[MyIndividual//5]//10\n```\n\nIn fact, `random` method of `BasePopulation` will call random method of `BaseIndividual`. If you want to generate an individual, then just execute `MyIndividual.random(n_chromosomes=5, size=10)`, or set `default_size`, then execute `MyIndividual.random()`.\n\n\n### Evolution\n\n#### `evolve` method\nInitialize a population with `random` method, then call `evolve` method.\n\n```python\npop = MyPopulation.random(n_individuals=50, size=100)\npop.evolve()\nprint(pop.solution)\n```\n\nset `verbose=True` to display the data for each generation.\n\n`evolve` method mainly excute two methods: \n- `init`: initial configuration of the algo.\n- `transition`: do each step of the iteration.\n\n#### History\n\nGet the history of the evolution.\n\n```python\nstat={\'Mean Fitness\':\'mean_fitness\', \'Best Fitness\': lambda pop: pop.best_individual.fitness}\ndata = pop.history(stat=stat)  # use history instead of evolve\n```\n`stat` is a dict mapping keys to function, where string \'mean_fitness\' means function `lambda pop:pop.mean_fitness` which gets the mean fitness of the individuals in `pop`. Since we have defined pop.best_individual.fitness as a property, `stat` could be redefined as `{\'Fitness\': \'fitness\', \'Best Fitness\': \'max_fitness\'}`.\n\nIt requires `ezstat`, a easy statistical tool devoloped by the author.\n\n#### performance\n\nUse `pop.perf()` to check the performance, which calls `evolve` several times.\n\n\n## Example\n\n### Example 1\n\nDescription\n\n    select some of ti, ni, i=1,...,L, ti in {1,2,...,T}, ni in {1,2,...,N}\n    the sum of ni approx. 10, while ti dose not repeat\n\nThe opt. problem is\n\n    min abs(sum_i{ni}-10) + maximum of frequences in {ti}\n    where i is selected.\n\n$$\n\\min_I |\\sum_{i\\in I} n_i -10| + t_m\n\\\\\nI\\subset\\{1,\\cdots,L\\}\n$$\nwhere $t_m$ is the mode of $\\{t_i, i\\in I\\}$\n\n```python\nt = np.random.randint(1, 5, 100)\nn = np.random.randint(1, 4, 100)\n\nimport collections\n\n\ndef max_repeat(x):\n    # Maximum repetition\n    c = collections.Counter(x)\n    return np.max([b for a, b in c.items()])\n\n\nclass MyIndividual(makeBinaryIndividual()):\n\n    def _fitness(self):\n        x = abs(np.dot(n, self.chromosome)-10)\n        y = max_repeat(ti for ti, c in zip(t, self) if c==1)\n        return - x - y\n\n\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual\n\npop = MyPopulation.random(n_individuals=50, size=100)\npop.evolve()\nprint(pop.solution)  # or pop.best_individual.decode()\n```\n\nNote that there is only one chromosome in `MonoIndividual`, which could be got by `self.chromosome`.\n\nIn fact, the population could be the container of chromosomes. Therefore, we can rewrite the classes as follows in a more natural way.\n\n```python\nclass MyChromosome(BinaryChromosome):\n\n    def _fitness(self):\n        x = abs(np.dot(n, self)-10)\n        y = max_repeat(ti for ti, c in zip(t, self) if c==1)\n        return - x - y\n\nclass MyPopulation(StandardPopulation):\n    element_class = MyChromosome\n```\n\nIt is equiv. to\n```python\ndef _fitness(obj):\n    x = abs(np.dot(n, obj)-10)\n    y = max_repeat(ti for ti, c in zip(t, obj) if c==1)\n    return - x - y\n\nMyPopulation = StandardPopulation[BinaryChromosome].set_fitness(_fitness)\n```\n\n### Example2: Knapsack Problem\n\nOne of the famous problem is the knapsack problem. It is a good example for GA.\n\nWe set `history=True` in `evolve` method for the example, that will record the main data of the whole evolution. It will return an object of `pandas.DataFrame`. The argument `stat`  is a dict from a key to function/str(corresponding to a method) representing a mapping from a population to a number. these numbers of one generation will be stored in a row of the dataframe.\n\nsee `# examples/example0`\n\n```python\n#!/usr/bin/env python3\n\nfrom pyrimidine import binaryIndividual, StandardPopulation\nfrom pyrimidine.benchmarks.optimization import *\n\n# generate a knapsack problem randomly\nevaluate = Knapsack.random(n=20)\n\n\nclass MyIndividual(binaryIndividual(size=20)):\n    def _fitness(self):\n        return evaluate(self)\n\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual\n    default_size = 10\n\n\npop = MyPopulation.random()\n\nstat={\'Mean Fitness\':\'mean_fitness\', \'Best Fitness\':\'max_fitness\'}\ndata = pop.evolve(stat=stat, history=True) # an instance of `pandas.DataFrame`\n\n# Visualization\nimport matplotlib.pyplot as plt\nfig = plt.figure()\nax = fig.add_subplot(111)\ndata[[\'Mean Fitness\', \'Best Fitness\']].plot(ax=ax)\nax.set_xlabel(\'Generations\')\nax.set_ylabel(\'Fitness\')\nplt.show()\n```\n\n![plot-history](/Users/william/Programming/myGithub/pyrimidine/plot-history.png)\n\n\n## Extension\n\n`pyrimidine` is extremely extendable. It is easy to implement other iterative models or algorithms, such as simulation annealing(SA) and particle swarm optimization(PSO).\n\nCurrently, it is recommended to define subclasses based on `IterativeModel` as a mixin. (not mandatory)\n\nIn PSO, we regard a particle as an individual, and `ParticleSwarm` as a population. But in the following, we subclass it from `IterativeModel`\n\n```python\n# pso.py\n@basic_memory\nclass Particle(BaseIndividual):\n    """A particle in PSO\n\n    Extends BaseIndividual\n\n    Variables:\n        default_size {number} -- one individual represented by 2 chromosomes: position and velocity\n        phantom {Particle} -- the current state of the particle moving in the solution space.\n    """\n\n    element_class = FloatChromosome\n    default_size = 2\n\n    # other methods\n\nclass ParticleSwarm(PopulationMixin):\n    """Standard PSO\n    \n    Extends:\n        PopulationMixin\n    """\n\n    element_class = Particle\n    default_size = 20\n\n    params = {\'learning_factor\': 2, \'acceleration_coefficient\': 3,\n    \'inertia\':0.75, \'n_best_particles\':0.2, \'max_velocity\':None}\n\n    def init(self):\n        for particle in self:\n            particle.init()\n        self.hall_of_fame = self.get_best_individuals(self.n_best_particles, copy=True)\n\n    def update_hall_of_fame(self):\n        hof_size = len(self.hall_of_fame)\n        for ind in self:\n            for k in range(hof_size):\n                if self.hall_of_fame[-k-1].fitness < ind.fitness:\n                    self.hall_of_fame.insert(hof_size-k, ind.copy())\n                    self.hall_of_fame.pop(0)\n                    break\n\n    @property\n    def best_fitness(self):\n        if self.hall_of_fame:\n            return max(map(attrgetter(\'fitness\'), self.hall_of_fame))\n        else:\n            return super().best_fitness\n\n    def transition(self, *args, **kwargs):\n        """\n        Transitation of the states of particles\n        """\n        self.move()\n        self.backup()\n        self.update_hall_of_fame()\n\n    def backup(self):\n        # overwrite the memory of the particle if its current state is better its memory\n        for particle in self:\n            particle.backup(check=True)\n\n    def move(self):\n        """Move the particles\n\n        Define the moving rule of particles, according to the hall of fame and the best record\n        """\n\n        scale = random()\n        eta = random()\n        scale_fame = random()\n        for particle in self:\n            for fame in self.hall_of_fame:\n                if particle.fitness < fame.fitness:\n                    particle.update_vilocity_by_fame(fame, scale, scale_fame, \n                        self.inertia, self.learning_factor, self.acceleration_coefficient)\n                    particle.position = particle.position + particle.velocity\n                    break\n        for particle in self.hall_of_fame:\n            particle.update_vilocity(scale, self.inertia, self.learning_factor)\n            particle.position = particle.position + particle.velocity\n```\n\nIf you want to apply PSO, then you can define\n\n```python\nclass MyParticleSwarm(ParticleSwarm, BasePopulation):\n    element_class = _Particle\n    default_size = 20\n\npop = MyParticleSwarm.random()\n```\n\nOf course, it is not mandatory. It is allowed to inherit `ParticleSwarm` from for example `HOFPopulation` directly.\n',
+    'version': '1.6',
+    'description': 'A competitive framework tailored for GA, crafted with an emphasis on OOP and Algebra-Inspired Programming.',
+    'long_description': '# pyrimidine\n\n`pyrimidine` is an extensible framework of genetic/evolutionary algorithm by Python. See [pyrimidine\'s document](https://pyrimidine.readthedocs.io/) for more details.\n\n![LOGO](logo.png)\n\n## Why\n\nWhy is the package named as “pyrimidine”? Because it begins with “py”.\n\n> — Are you kiding?\n>\n> — No, I am serious.\n\n## Download\n\nIt has been uploaded to [pypi](https://pypi.org/project/pyrimidine/), so download it with `pip install pyrimidine`, and also could download it from github.\n\n## Idea\n\nWe regard the population as a container of individuals, an individual as a container of chromosomes\nand a chromosome as a container(array) of genes.\n\nThe container could be a list or an array.\nThe container class has an attribute `element_class`, telling itself the type of the elements in it.\n\nFollowing is the part of the source code of `BaseIndividual` and `BasePopulation`.\n\n```python\nclass BaseIndividual(FitnessModel, metaclass=MetaContainer):\n    element_class = BaseChromosome\n    default_size = 1\n\nclass BasePopulation(PopulationModel, metaclass=MetaContainer):\n    element_class = BaseIndividual\n    default_size = 20\n```\n\nThere is mainly tow kinds of containers: list and tuple as in programming language `Haskell`. See following examples.\n\n```python\n# individual with chromosomes of type _Chromosome\n_Individual1 = BaseIndividual[_Choromosome]\n# individual with 2 chromosomes of type _Chromosome1 and _Chromosome2 respectively\n_Individual2 = MixedIndividual[_Chromosome1, _Chromosome2]\n```\n\n### Math expression\n$s$ of type $S$ is a container of $a:A$, represented as follows:\n\n```\ns={a:A}:S\n```\n\nWe define a population as a container of individuals or chromosomes, and an individual is a container of chromosomes.\n\nAlgebraically, an indivdiual has only one chromosome is equivalent to a chromosome mathematically. A population could also be a container of chromosomes. If the individual has only one chromosome, then just build the population based on chromosomes directly.\n\nThe methods are the functions or operators defined on $s$.\n\n## Use\n\n### Main classes\n\n- BaseGene: the gene of chromosome\n- BaseChromosome: sequence of genes, represents part of a solution\n- BaseIndividual: sequence of chromosomes, represents a solution of a problem\n- BasePopulation: a container of individuals, represents a container of a problem\n                also the state of a stachostic process\n- BaseMultipopulation: a container of population for more complicated optimalization\n\n### import\n\nTo import all algorithms for beginners, simply use the command `from pyrimidine import *`.\n\nTo speed the lib, use the following commands \n```\nfrom pyrimidine import BaseChromosome, BaseIndividual, BasePopulation # import the base classes form `base.py` to build your own classes\n\n# Commands used frequently\nfrom pyrimidine.base import BinaryChromosome, FloatChromosome # import the Chromosome classes and utilize them directly\n# equivalent to `from pyrimidine import BinaryChromosome, FloatChromosome`\nfrom pyrimidine.population import StandardPopulation, HOFPopulation # For creating population with standard GA \n# the same effect with `from pyrimidine import StandardPopulation, HOFPopulation`\nfrom pyrimidine.indiviual import makeIndividual # a helper to make Individual objects, or `from pyrimidine import makeIndividual`\n\nfrom pyrimidine import MultiPopulation # build the multi-populations\nfrom pyrimidine import MetaContainer # meta class for socalled container class, that is recommended to be used for creating novel evolutionary algorithms.\n\nfrom pyrimidine.deco import * # import all decorators\nfrom pyrimidine.deco import fitness_cache, basic_memory # use the cache decorator and memory decorator\n\nfrom pyrimidine import optimize # do optimization implictly with GAs\n```\n\n### subclasses\n\n#### Chromosome\n\nGenerally, it is an array of genes.\n\nAs an array of 0-1s, `BinaryChromosome` is used most frequently.\n\n#### Individual\njust subclass `MonoIndividual` in most cases.\n\n```python\nclass MyIndividual(MonoIndividual):\n    """individual with only one chromosome\n    we set the gene is 0 or 1 in the chromosome\n    """\n    element_class = BinaryChromosome\n\n    def _fitness(self):\n        ...\n```\n\nSince the helper `makeIndividual(n_chromosomes=1, size=8)` could create such individual, it is equivalent to\n\n```python\nclass MyIndividual(binaryIndividual()):\n    # only need define the fitness\n    def _fitness(self):\n        ...\n```\n\n\nIf an individual contains several chromosomes, then subclass `MultiIndividual` or `PolyIndividual`. It could be applied in multi-real-variable optimization problems where each variable has a separative binary encoding.\n\n\nIn most cases, we have to decode chromosomes to real numbers.\n\n```python\nclass _Chromosome(BinaryChromosome):\n    def decode(self):\n        """Decode a binary chromosome\n        \n        if the sequence of 0-1 represents a real number, then overide the method\n        to transform it to a nubmer\n        """\n\nclass ExampleIndividual(BaseIndividual):\n    element_class = _Chromosome\n\n    def _fitness(self):\n        # define the method to calculate the fitness\n        x = self.decode()  # will call decode method of _Chromosome\n        return evaluate(x)\n```\n\n\nIf the chromosomes in an individual are different with each other, then subclass `MixedIndividual`, meanwhile, the property `element_class` should be assigned with a tuple of classes for each chromosome.\n\n```python\nclass MyIndividual(MixedIndividual):\n    """\n    Inherit the fitness from ExampleIndividual directly.\n    It has 6 chromosomes, 5 are instances of _Chromosome, 1 is instance of FloatChromosome\n    """\n    element_class = (_Chromosome,)*5 + (FloatChromosome,)\n```\n\nIt equivalent to `MyIndividual=MixedIndividual[(_Chromosome,)*5 + (FloatChromosome,)]`\n\n#### Population\n\n```python\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual\n```\n\nIt is equivalent to `MyPopulation = StandardPopulation[MyIndividual]`.\n\n\n### Initialize randomly\n\n`random` is a factory method!\n\nGenerate a population, with 50 individuals and each individual has 100 genes:\n\n`pop = MyPopulation.random(n_individuals=50, size=100)`\n\nWhen each individual contains 5 chromosomes, use\n\n`pop = MyPopulation.random(n_individuals=10, n_chromosomes=5, size=10)`\n\nHowever, we recommand to set `default_size` in the classes, then run `MyPopulation.random()`\n\n```python\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual // 5\n    default_size = 10\n\n# equiv. to\n\nMyPopulation = StandardPopulation[MyIndividual//5]//10\n```\n\nIn fact, `random` method of `BasePopulation` will call random method of `BaseIndividual`. If you want to generate an individual, then just execute `MyIndividual.random(n_chromosomes=5, size=10)`, or set `default_size`, then execute `MyIndividual.random()`.\n\n\n### Evolution\n\n#### `evolve` method\nInitialize a population with `random` method, then call `evolve` method.\n\n```python\npop = MyPopulation.random(n_individuals=50, size=100)\npop.evolve()\nprint(pop.solution)\n```\n\nset `verbose=True` to display the data for each generation.\n\n`evolve` method mainly excute two methods: \n- `init`: initial configuration of the algo.\n- `transition`: do each step of the iteration.\n\n#### History\n\nGet the history of the evolution.\n\n```python\nstat={\'Mean Fitness\':\'mean_fitness\', \'Best Fitness\': lambda pop: pop.best_individual.fitness}\ndata = pop.history(stat=stat)  # use history instead of evolve\n```\n`stat` is a dict mapping keys to function, where string \'mean_fitness\' means function `lambda pop:pop.mean_fitness` which gets the mean fitness of the individuals in `pop`. Since we have defined pop.best_individual.fitness as a property, `stat` could be redefined as `{\'Fitness\': \'fitness\', \'Best Fitness\': \'max_fitness\'}`.\n\nIt requires `ezstat`, a easy statistical tool devoloped by the author.\n\n#### performance\n\nUse `pop.perf()` to check the performance, which calls `evolve` several times.\n\n\n## Example\n\n### Example 1\n\nDescription\n\n    select some of ti, ni, i=1,...,L, ti in {1,2,...,T}, ni in {1,2,...,N}\n    the sum of ni approx. 10, while ti dose not repeat\n\nThe opt. problem is\n\n    min abs(sum_i{ni}-10) + maximum of frequences in {ti}\n    where i is selected.\n\n$$\n\\min_I |\\sum_{i\\in I} n_i -10| + t_m\n\\\\\nI\\subset\\{1,\\cdots,L\\}\n$$\nwhere $t_m$ is the mode of $\\{t_i, i\\in I\\}$\n\n```python\nt = np.random.randint(1, 5, 100)\nn = np.random.randint(1, 4, 100)\n\nimport collections\n\nfrom pyrimidine.individual import makeBinaryIndividual\nfrom pyrimidine.population import StandardPopulation\n\ndef max_repeat(x):\n    # Maximum repetition\n    c = collections.Counter(x)\n    return np.max([b for a, b in c.items()])\n\n\nclass MyIndividual(makeBinaryIndividual()):\n\n    def _fitness(self):\n        x = abs(np.dot(n, self.chromosome)-10)\n        y = max_repeat(ti for ti, c in zip(t, self) if c==1)\n        return - x - y\n\n\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual\n\npop = MyPopulation.random(n_individuals=50, size=100)\npop.evolve()\nprint(pop.solution)  # or pop.best_individual.decode()\n```\n\nNote that there is only one chromosome in `MonoIndividual`, which could be got by `self.chromosome`.\n\nIn fact, the population could be the container of chromosomes. Therefore, we can rewrite the classes as follows in a more natural way.\n\n```python\nfrom pyrimidine.chromosome import BinaryChromosome\nfrom pyrimidine.population import StandardPopulation\n\nclass MyChromosome(BinaryChromosome):\n\n    def _fitness(self):\n        x = abs(np.dot(n, self)-10)\n        y = max_repeat(ti for ti, c in zip(t, self) if c==1)\n        return - x - y\n\nclass MyPopulation(StandardPopulation):\n    element_class = MyChromosome\n```\n\nIt is equiv. to\n```python\ndef _fitness(obj):\n    x = abs(np.dot(n, obj)-10)\n    y = max_repeat(ti for ti, c in zip(t, obj) if c==1)\n    return - x - y\n\nMyPopulation = StandardPopulation[BinaryChromosome].set_fitness(_fitness)\n```\n\n### Example2: Knapsack Problem\n\nOne of the famous problem is the knapsack problem. It is a good example for GA.\n\nWe set `history=True` in `evolve` method for the example, that will record the main data of the whole evolution. It will return an object of `pandas.DataFrame`. The argument `stat`  is a dict from a key to function/str(corresponding to a method) representing a mapping from a population to a number. these numbers of one generation will be stored in a row of the dataframe.\n\nsee `# examples/example0`\n\n```python\n#!/usr/bin/env python3\n\nfrom pyrimidine import binaryIndividual, StandardPopulation\nfrom pyrimidine.benchmarks.optimization import *\n\n# generate a knapsack problem randomly\nevaluate = Knapsack.random(n=20)\n\n\nclass MyIndividual(binaryIndividual(size=20)):\n    def _fitness(self):\n        return evaluate(self)\n\nclass MyPopulation(StandardPopulation):\n    element_class = MyIndividual\n    default_size = 10\n\n\npop = MyPopulation.random()\n\nstat={\'Mean Fitness\':\'mean_fitness\', \'Best Fitness\':\'max_fitness\'}\ndata = pop.evolve(stat=stat, history=True) # an instance of `pandas.DataFrame`\n\n# Visualization\nimport matplotlib.pyplot as plt\nfig = plt.figure()\nax = fig.add_subplot(111)\ndata[[\'Mean Fitness\', \'Best Fitness\']].plot(ax=ax)\nax.set_xlabel(\'Generations\')\nax.set_ylabel(\'Fitness\')\nplt.show()\n```\n\n![plot-history](/Users/william/Programming/myGithub/pyrimidine/plot-history.png)\n\n\n## Extension\n\n`pyrimidine` is extremely extendable. It is easy to implement other iterative models or algorithms, such as simulation annealing(SA) and particle swarm optimization(PSO).\n\nCurrently, it is recommended to define subclasses based on `IterativeModel` as a mixin. (not mandatory)\n\nIn PSO, we regard a particle as an individual, and `ParticleSwarm` as a population. But in the following, we subclass it from `IterativeModel`\n\n```python\n# pso.py\n@basic_memory\nclass Particle(BaseIndividual):\n    """A particle in PSO\n\n    Extends BaseIndividual\n\n    Variables:\n        default_size {number} -- one individual represented by 2 chromosomes: position and velocity\n        phantom {Particle} -- the current state of the particle moving in the solution space.\n    """\n\n    element_class = FloatChromosome\n    default_size = 2\n\n    # other methods\n\nclass ParticleSwarm(PopulationMixin):\n    """Standard PSO\n    \n    Extends:\n        PopulationMixin\n    """\n\n    element_class = Particle\n    default_size = 20\n\n    params = {\'learning_factor\': 2, \'acceleration_coefficient\': 3,\n    \'inertia\':0.75, \'n_best_particles\':0.2, \'max_velocity\':None}\n\n    def init(self):\n        for particle in self:\n            particle.init()\n        self.hall_of_fame = self.get_best_individuals(self.n_best_particles, copy=True)\n\n    def update_hall_of_fame(self):\n        hof_size = len(self.hall_of_fame)\n        for ind in self:\n            for k in range(hof_size):\n                if self.hall_of_fame[-k-1].fitness < ind.fitness:\n                    self.hall_of_fame.insert(hof_size-k, ind.copy())\n                    self.hall_of_fame.pop(0)\n                    break\n\n    @property\n    def best_fitness(self):\n        if self.hall_of_fame:\n            return max(map(attrgetter(\'fitness\'), self.hall_of_fame))\n        else:\n            return super().best_fitness\n\n    def transition(self, *args, **kwargs):\n        """\n        Transitation of the states of particles\n        """\n        self.move()\n        self.backup()\n        self.update_hall_of_fame()\n\n    def backup(self):\n        # overwrite the memory of the particle if its current state is better its memory\n        for particle in self:\n            particle.backup(check=True)\n\n    def move(self):\n        """Move the particles\n\n        Define the moving rule of particles, according to the hall of fame and the best record\n        """\n\n        scale = random()\n        eta = random()\n        scale_fame = random()\n        for particle in self:\n            for fame in self.hall_of_fame:\n                if particle.fitness < fame.fitness:\n                    particle.update_vilocity_by_fame(fame, scale, scale_fame, \n                        self.inertia, self.learning_factor, self.acceleration_coefficient)\n                    particle.position = particle.position + particle.velocity\n                    break\n        for particle in self.hall_of_fame:\n            particle.update_vilocity(scale, self.inertia, self.learning_factor)\n            particle.position = particle.position + particle.velocity\n```\n\nIf you want to apply PSO, then you can define\n\n```python\nclass MyParticleSwarm(ParticleSwarm, BasePopulation):\n    element_class = _Particle\n    default_size = 20\n\npop = MyParticleSwarm.random()\n```\n\nOf course, it is not mandatory. It is allowed to inherit `ParticleSwarm` from for example `HOFPopulation` directly.\n',
     'author': 'William Song',
     'author_email': '30965609+Freakwill@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Freakwill/pyrimidine',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyrimidine-1.5.6/PKG-INFO` & `pyrimidine-1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyrimidine
-Version: 1.5.6
-Summary: A competitive framework for GA, designed by thorough OOP/Algebra-inspried Programming
+Version: 1.6
+Summary: A competitive framework tailored for GA, crafted with an emphasis on OOP and Algebra-Inspired Programming.
 Home-page: https://github.com/Freakwill/pyrimidine
 License: MIT
 Keywords: Genetic Algorithm,Artificial Intelligence,Intelligent Optimization
 Author: William Song
 Author-email: 30965609+Freakwill@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: MacOS X
@@ -15,14 +15,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
+Requires-Dist: numpy (>=1.26.0,<2.0.0)
+Requires-Dist: pandas (>=2.1.0,<3.0.0)
+Requires-Dist: scikit-learn (>=1.1.0,<2.0.0)
+Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: toolz (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://github.com/Freakwill/pyrimidine
 Description-Content-Type: text/markdown
 
 # pyrimidine
 
 `pyrimidine` is an extensible framework of genetic/evolutionary algorithm by Python. See [pyrimidine's document](https://pyrimidine.readthedocs.io/) for more details.
 
@@ -89,19 +95,39 @@
 - BaseGene: the gene of chromosome
 - BaseChromosome: sequence of genes, represents part of a solution
 - BaseIndividual: sequence of chromosomes, represents a solution of a problem
 - BasePopulation: a container of individuals, represents a container of a problem
                 also the state of a stachostic process
 - BaseMultipopulation: a container of population for more complicated optimalization
 
-
 ### import
-Just use the command `from pyrimidine import *` import all of the algorithms.
 
-### subclass
+To import all algorithms for beginners, simply use the command `from pyrimidine import *`.
+
+To speed the lib, use the following commands 
+```
+from pyrimidine import BaseChromosome, BaseIndividual, BasePopulation # import the base classes form `base.py` to build your own classes
+
+# Commands used frequently
+from pyrimidine.base import BinaryChromosome, FloatChromosome # import the Chromosome classes and utilize them directly
+# equivalent to `from pyrimidine import BinaryChromosome, FloatChromosome`
+from pyrimidine.population import StandardPopulation, HOFPopulation # For creating population with standard GA 
+# the same effect with `from pyrimidine import StandardPopulation, HOFPopulation`
+from pyrimidine.indiviual import makeIndividual # a helper to make Individual objects, or `from pyrimidine import makeIndividual`
+
+from pyrimidine import MultiPopulation # build the multi-populations
+from pyrimidine import MetaContainer # meta class for socalled container class, that is recommended to be used for creating novel evolutionary algorithms.
+
+from pyrimidine.deco import * # import all decorators
+from pyrimidine.deco import fitness_cache, basic_memory # use the cache decorator and memory decorator
+
+from pyrimidine import optimize # do optimization implictly with GAs
+```
+
+### subclasses
 
 #### Chromosome
 
 Generally, it is an array of genes.
 
 As an array of 0-1s, `BinaryChromosome` is used most frequently.
 
@@ -260,14 +286,16 @@
 
 ```python
 t = np.random.randint(1, 5, 100)
 n = np.random.randint(1, 4, 100)
 
 import collections
 
+from pyrimidine.individual import makeBinaryIndividual
+from pyrimidine.population import StandardPopulation
 
 def max_repeat(x):
     # Maximum repetition
     c = collections.Counter(x)
     return np.max([b for a, b in c.items()])
 
 
@@ -288,14 +316,17 @@
 ```
 
 Note that there is only one chromosome in `MonoIndividual`, which could be got by `self.chromosome`.
 
 In fact, the population could be the container of chromosomes. Therefore, we can rewrite the classes as follows in a more natural way.
 
 ```python
+from pyrimidine.chromosome import BinaryChromosome
+from pyrimidine.population import StandardPopulation
+
 class MyChromosome(BinaryChromosome):
 
     def _fitness(self):
         x = abs(np.dot(n, self)-10)
         y = max_repeat(ti for ti, c in zip(t, self) if c==1)
         return - x - y
```

