# Comparing `tmp/gym_pusht-0.1.3.tar.gz` & `tmp/gym_pusht-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_pusht-0.1.3.tar", max compression
+gzip compressed data, was "gym_pusht-0.1.4.tar", max compression
```

## Comparing `gym_pusht-0.1.3.tar` & `gym_pusht-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12625 2024-04-08 10:15:07.504261 gym_pusht-0.1.3/LICENSE
--rw-r--r--   0        0        0     4267 2024-05-06 15:12:34.087834 gym_pusht-0.1.3/README.md
--rw-r--r--   0        0        0      195 2024-04-09 08:02:09.966097 gym_pusht-0.1.3/gym_pusht/__init__.py
--rw-r--r--   0        0        0       66 2024-04-09 08:02:09.966273 gym_pusht-0.1.3/gym_pusht/envs/__init__.py
--rw-r--r--   0        0        0    17716 2024-05-06 15:12:34.088271 gym_pusht-0.1.3/gym_pusht/envs/pusht.py
--rw-r--r--   0        0        0     8375 2024-04-09 08:02:09.966831 gym_pusht-0.1.3/gym_pusht/envs/pymunk_override.py
--rw-r--r--   0        0        0     1714 2024-05-08 07:25:12.836161 gym_pusht-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 gym_pusht-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    12625 2024-04-08 10:15:07.504261 gym_pusht-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4267 2024-05-06 15:12:34.087834 gym_pusht-0.1.4/README.md
+-rw-r--r--   0        0        0      195 2024-05-11 10:08:07.647679 gym_pusht-0.1.4/gym_pusht/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-09 08:02:09.966273 gym_pusht-0.1.4/gym_pusht/envs/__init__.py
+-rw-r--r--   0        0        0    17752 2024-05-11 10:08:07.649093 gym_pusht-0.1.4/gym_pusht/envs/pusht.py
+-rw-r--r--   0        0        0     8375 2024-04-09 08:02:09.966831 gym_pusht-0.1.4/gym_pusht/envs/pymunk_override.py
+-rw-r--r--   0        0        0     1714 2024-05-12 06:17:00.821069 gym_pusht-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 gym_pusht-0.1.4/PKG-INFO
```

### Comparing `gym_pusht-0.1.3/LICENSE` & `gym_pusht-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.3/README.md` & `gym_pusht-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.3/gym_pusht/envs/pusht.py` & `gym_pusht-0.1.4/gym_pusht/envs/pusht.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,15 @@
         coverage = self._get_coverage()
         reward = np.clip(coverage / self.success_threshold, 0.0, 1.0)
         terminated = is_success = coverage > self.success_threshold
 
         observation = self.get_obs()
         info = self._get_info()
         info["is_success"] = is_success
+        info["coverage"] = coverage
 
         truncated = False
         return observation, reward, terminated, truncated, info
 
     def reset(self, seed=None, options=None):
         super().reset(seed=seed)
         self._setup()
```

### Comparing `gym_pusht-0.1.3/gym_pusht/envs/pymunk_override.py` & `gym_pusht-0.1.4/gym_pusht/envs/pymunk_override.py`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.3/pyproject.toml` & `gym_pusht-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-pusht"
-version = "0.1.3"
+version = "0.1.4"
 description = "A gymnasium environment for PushT."
 authors = [
     "Rémi Cadène <re.cadene@gmail.com>",
     "Quentin Gallouédec <quentin.gallouedec@ec-lyon.fr>",
     "Alexander Soare <alexander.soare159@gmail.com>",
     "Simon Alibert <alibert.sim@gmail.com>",
 ]
```

### Comparing `gym_pusht-0.1.3/PKG-INFO` & `gym_pusht-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-pusht
-Version: 0.1.3
+Version: 0.1.4
 Summary: A gymnasium environment for PushT.
 License: Apache-2.0
 Author: Rémi Cadène
 Author-email: re.cadene@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

