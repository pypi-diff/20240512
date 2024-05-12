# Comparing `tmp/aa_routing-0.2.1a0.tar.gz` & `tmp/aa_routing-0.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_routing-0.2.1a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_routing-0.2.2a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_routing-0.2.1a0.tar` & `aa_routing-0.2.2a0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1069 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/LICENSE
--rw-r--r--   0        0        0     1846 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/README.md
--rw-r--r--   0        0        0     2016 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0       91 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/__init__.py
--rw-r--r--   0        0        0      179 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/app_settings.py
--rw-r--r--   0        0        0      221 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/apps.py
--rw-r--r--   0        0        0     2384 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/edges.py
--rw-r--r--   0        0        0      791 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/graph.py
--rw-r--r--   0        0        0      328 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/management/commands/routing_precompute.py
--rw-r--r--   0        0        0     1666 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/migrations/0001_initial.py
--rw-r--r--   0        0        0      898 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/migrations/0002_solarsystemconnection_prefer_less_safe_and_more.py
--rw-r--r--   0        0        0     1061 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/migrations/0003_triginvasion.py
--rw-r--r--   0        0        0      723 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/migrations/0004_rename_prefer_less_safe_solarsystemconnection_p_less_safe_and_more.py
--rw-r--r--   0        0        0      427 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/migrations/0005_rename_security_status_solarsystem_security.py
--rw-r--r--   0        0        0        0 2023-11-08 12:17:49.190811 aa_routing-0.2.1a0/routing/migrations/__init__.py
--rw-r--r--   0        0        0     2202 2023-11-08 12:17:49.163809 aa_routing-0.2.1a0/routing/models.py
--rw-r--r--   0        0        0     7664 2023-11-08 12:17:49.164809 aa_routing-0.2.1a0/routing/routing.py
--rw-r--r--   0        0        0  1375787 2023-11-08 12:17:49.166809 aa_routing-0.2.1a0/routing/static_data.py
--rw-r--r--   0        0        0     2528 2023-11-08 12:17:49.166809 aa_routing-0.2.1a0/routing/tasks.py
--rw-r--r--   0        0        0        0 2023-11-08 12:17:49.190811 aa_routing-0.2.1a0/routing/tests/__init__.py
--rw-r--r--   0        0        0     1842 2023-11-08 12:17:49.166809 aa_routing-0.2.1a0/routing/tests/test_models.py
--rw-r--r--   0        0        0     6843 2023-11-08 12:17:49.166809 aa_routing-0.2.1a0/routing/tests/test_routing.py
--rw-r--r--   0        0        0     5229 2023-11-08 12:17:49.166809 aa_routing-0.2.1a0/routing/trigInvasionSystems.csv
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 aa_routing-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/LICENSE
+-rw-r--r--   0        0        0     1846 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/README.md
+-rw-r--r--   0        0        0     2016 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/routing/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/routing/app_settings.py
+-rw-r--r--   0        0        0      221 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/routing/apps.py
+-rw-r--r--   0        0        0     2543 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/routing/edges.py
+-rw-r--r--   0        0        0      791 2024-05-12 06:49:53.081677 aa_routing-0.2.2a0/routing/graph.py
+-rw-r--r--   0        0        0      380 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1819 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      328 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/management/commands/routing_precompute.py
+-rw-r--r--   0        0        0     1666 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/migrations/0001_initial.py
+-rw-r--r--   0        0        0      898 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/migrations/0002_solarsystemconnection_prefer_less_safe_and_more.py
+-rw-r--r--   0        0        0     1061 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/migrations/0003_triginvasion.py
+-rw-r--r--   0        0        0      723 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/migrations/0004_rename_prefer_less_safe_solarsystemconnection_p_less_safe_and_more.py
+-rw-r--r--   0        0        0      427 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/migrations/0005_rename_security_status_solarsystem_security.py
+-rw-r--r--   0        0        0        0 2024-05-12 06:49:53.117677 aa_routing-0.2.2a0/routing/migrations/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/models.py
+-rw-r--r--   0        0        0     7664 2024-05-12 06:49:53.082677 aa_routing-0.2.2a0/routing/routing.py
+-rw-r--r--   0        0        0  1375787 2024-05-12 06:49:53.086677 aa_routing-0.2.2a0/routing/static_data.py
+-rw-r--r--   0        0        0     2528 2024-05-12 06:49:53.086677 aa_routing-0.2.2a0/routing/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-12 06:49:53.118677 aa_routing-0.2.2a0/routing/tests/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-12 06:49:53.086677 aa_routing-0.2.2a0/routing/tests/test_models.py
+-rw-r--r--   0        0        0     6843 2024-05-12 06:49:53.086677 aa_routing-0.2.2a0/routing/tests/test_routing.py
+-rw-r--r--   0        0        0     5229 2024-05-12 06:49:53.086677 aa_routing-0.2.2a0/routing/trigInvasionSystems.csv
+-rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 aa_routing-0.2.2a0/PKG-INFO
```

### Comparing `aa_routing-0.2.1a0/LICENSE` & `aa_routing-0.2.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/README.md` & `aa_routing-0.2.2a0/README.md`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/pyproject.toml` & `aa_routing-0.2.2a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/edges.py` & `aa_routing-0.2.2a0/routing/edges.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,26 @@
     pass
 
 
 def include_corptools_jumpbridges(weight: float = 1.0) -> list[Tuple]:
     edges = []
     if corptools_active():
         for jb in MapJumpBridge.objects.values_list("from_solar_system_id", "to_solar_system_id").all():
-            edges.append((
-                jb.from_solar_system_id, jb.to_solar_system_id,
-                {'p_shortest': weight, 'p_safest': weight, 'p_less_safe': weight, "type": "jump_bridge"}))
+            edges.append(
+                (
+                    jb[0],
+                    jb[1],
+                    {
+                        'p_shortest': weight,
+                        'p_safest': weight,
+                        'p_less_safe': weight,
+                        "type": "jump_bridge"
+                    }
+                )
+            )
     else:
         return edges
 
     return edges
 
 
 def include_eve_scout(system: str = "thera") -> List[Tuple]:
```

### Comparing `aa_routing-0.2.1a0/routing/graph.py` & `aa_routing-0.2.2a0/routing/graph.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/migrations/0001_initial.py` & `aa_routing-0.2.2a0/routing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/migrations/0002_solarsystemconnection_prefer_less_safe_and_more.py` & `aa_routing-0.2.2a0/routing/migrations/0002_solarsystemconnection_prefer_less_safe_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/migrations/0003_triginvasion.py` & `aa_routing-0.2.2a0/routing/migrations/0003_triginvasion.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/migrations/0004_rename_prefer_less_safe_solarsystemconnection_p_less_safe_and_more.py` & `aa_routing-0.2.2a0/routing/migrations/0004_rename_prefer_less_safe_solarsystemconnection_p_less_safe_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/models.py` & `aa_routing-0.2.2a0/routing/models.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/routing.py` & `aa_routing-0.2.2a0/routing/routing.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/static_data.py` & `aa_routing-0.2.2a0/routing/static_data.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/tasks.py` & `aa_routing-0.2.2a0/routing/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/tests/test_models.py` & `aa_routing-0.2.2a0/routing/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/tests/test_routing.py` & `aa_routing-0.2.2a0/routing/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/routing/trigInvasionSystems.csv` & `aa_routing-0.2.2a0/routing/trigInvasionSystems.csv`

 * *Files identical despite different names*

### Comparing `aa_routing-0.2.1a0/PKG-INFO` & `aa_routing-0.2.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_routing
-Version: 0.2.1a0
+Version: 0.2.2a0
 Summary: AllianceAuth Routing and Pathfinding
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
```

