# Comparing `tmp/cdbt-0.1.0.tar.gz` & `tmp/cdbt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.1.0.tar", last modified: Sat May 11 23:41:02 2024, max compression
+gzip compressed data, was "cdbt-0.1.1.tar", last modified: Sat May 11 23:49:49 2024, max compression
```

## Comparing `cdbt-0.1.0.tar` & `cdbt-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-11 23:41:02.005302 cdbt-0.1.0/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      385 2024-05-11 23:41:02.004588 cdbt-0.1.0/PKG-INFO
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-11 23:41:01.995545 cdbt-0.1.0/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.0/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6177 2024-05-11 23:35:04.000000 cdbt-0.1.0/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6642 2024-05-11 23:20:14.000000 cdbt-0.1.0/cdbt/main_backup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-11 23:41:02.004049 cdbt-0.1.0/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      385 2024-05-11 23:41:01.000000 cdbt-0.1.0/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      228 2024-05-11 23:41:01.000000 cdbt-0.1.0/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-11 23:41:01.000000 cdbt-0.1.0/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       40 2024-05-11 23:41:01.000000 cdbt-0.1.0/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-11 23:41:01.000000 cdbt-0.1.0/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-11 23:41:01.000000 cdbt-0.1.0/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-11 23:41:02.005394 cdbt-0.1.0/setup.cfg
--rwxrwx---   0 craiglathrop   (501) staff       (20)      635 2024-05-11 23:38:20.000000 cdbt-0.1.0/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-11 23:49:49.919317 cdbt-0.1.1/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      385 2024-05-11 23:49:49.918676 cdbt-0.1.1/PKG-INFO
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-11 23:49:49.909680 cdbt-0.1.1/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.1/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7582 2024-05-11 23:48:42.000000 cdbt-0.1.1/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6642 2024-05-11 23:20:14.000000 cdbt-0.1.1/cdbt/main_backup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-11 23:49:49.918149 cdbt-0.1.1/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      385 2024-05-11 23:49:49.000000 cdbt-0.1.1/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      228 2024-05-11 23:49:49.000000 cdbt-0.1.1/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-11 23:49:49.000000 cdbt-0.1.1/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       40 2024-05-11 23:49:49.000000 cdbt-0.1.1/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-11 23:49:49.000000 cdbt-0.1.1/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-11 23:49:49.000000 cdbt-0.1.1/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-11 23:49:49.919388 cdbt-0.1.1/setup.cfg
+-rwxrwx---   0 craiglathrop   (501) staff       (20)      635 2024-05-11 23:46:40.000000 cdbt-0.1.1/setup.py
```

### Comparing `cdbt-0.1.0/cdbt/main.py` & `cdbt-0.1.1/cdbt/main_backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,18 +83,20 @@
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 def sbuild(full_refresh):
     print('Starting a state build based on local manifest.json')
     artifact_dir = '_artifacts'
     target_dir = 'target'
     # Path to the artifacts file that will be generated by the dbt compile command representing the current state.
     manifest_path = os.path.join('./', target_dir, 'manifest.json')
+    # Path to the backup file to create in case of an error.
+    manifest_backup_path = os.path.join('./', artifact_dir, 'manifest.json_bak')
     # Path to the artifact file that represents the prior build state.
     manifest_artifact_path = os.path.join('./', artifact_dir, 'manifest.json')
 
-    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_path, full_refresh,
+    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_backup_path, manifest_path, full_refresh,
                               roll_back_manifest_flag=True)
 
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 def pbuild(full_refresh):
     print('Starting a state build based on production manifest.json')
@@ -104,78 +106,83 @@
     try:
         subprocess.run(['dbt', 'run-operation', 'get_last_artifacts'], check=True)
     except subprocess.CalledProcessError as e:
         print(e)
         sys.exit(1)
 
     manifest_path = os.path.join('.', target_dir, 'manifest.json')
+    manifest_backup_path = os.path.join('.', artifact_dir, 'manifest.json_bak')
     manifest_artifact_path = os.path.join('.', artifact_dir, 'manifest.json')
 
-    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_path, full_refresh,
+    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_backup_path, manifest_path, full_refresh,
                               roll_back_manifest_flag=False)
 
 
-def execute_state_based_build(artifact_dir: str, manifest_artifact_path: str, manifest_path: str, full_refresh: bool,
-                              roll_back_manifest_flag: bool):
+def execute_state_based_build(artifact_dir: str, manifest_artifact_path: str, manifest_backup_path: str,
+                              manifest_path: str, full_refresh: bool, roll_back_manifest_flag: bool):
+    print(f'Pulling manifest from {manifest_artifact_path}')
     if roll_back_manifest_flag:
-        print(f'Making a backup of the current manifest.json at {manifest_path} to {manifest_artifact_path}')
-        # Move the manifest from ./target to ./_artifacts. This becomes the prior state. Only used for local state
-        # build. Not used for pdbuild (production build).
+        # Backup and move manifest.json. Only used for local state build. Not used for pdbuild (production build).
+        # First move the current manifest to the backup location
+        shutil.copy(manifest_artifact_path, manifest_backup_path)
+        #
         shutil.move(manifest_path, manifest_artifact_path)
     # Execute dbt compile
     try:
         subprocess.run(['dbt', 'compile'], check=True)
     except subprocess.CalledProcessError:
+        # Rollback if dbt compile fails
+        shutil.move(manifest_artifact_path, manifest_path)
+        shutil.move(manifest_backup_path, manifest_artifact_path)
         sys.exit(1)
     # Construct state commands
     state_flags = [
         '--select', 'state:modified+',
         '--state', os.path.join('.', artifact_dir) + '/'
     ]
 
     # Execute dbt seed
     try:
         execute_dbt_command('seed', state_flags)
     except subprocess.CalledProcessError as e:
         if roll_back_manifest_flag:
-            roll_back_manifest(e, manifest_artifact_path, manifest_path)
+            roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path)
         else:
             print(e)
             sys.exit(1)
 
     # Execute dbt run
     if full_refresh:
         run_flags = state_flags + ['--full-refresh']
     else:
         run_flags = state_flags
     try:
         execute_dbt_command('run', run_flags)
     except subprocess.CalledProcessError as e:
         if roll_back_manifest_flag:
-            roll_back_manifest(e, manifest_artifact_path, manifest_path)
+            roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path)
         else:
             print(e)
             sys.exit(1)
 
     # Execute dbt test
     try:
         execute_dbt_command('test', state_flags)
     except subprocess.CalledProcessError as e:
         if roll_back_manifest_flag:
-            roll_back_manifest(e, manifest_artifact_path, manifest_path)
+            roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path)
         else:
             print(e)
             sys.exit(1)
 
 
-def roll_back_manifest(e, manifest_artifact_path, manifest_path):
+def roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path):
     print(f"DBT build failed. Rolling back manifest state with error\n {e}")
-    # Move the manifest.json from _artifacts back to target dir. If the build failed, we want to rebuild against this
-    # state, not the one generated by the compile command.
     shutil.move(manifest_artifact_path, manifest_path)
+    shutil.move(manifest_backup_path, manifest_artifact_path)
     sys.exit(1)
 
 
 def execute_dbt_command(command: str, args: List[str]):
     command = ['dbt', command] + args
     print(f'Running command: {command}')
     try:
```

### Comparing `cdbt-0.1.0/cdbt/main_backup.py` & `cdbt-0.1.1/cdbt/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,14 +43,41 @@
 
     try:
         execute_dbt_command('test', args)
     except subprocess.CalledProcessError as e:
         print(e)
         sys.exit(1)
 
+@cdbt.command()
+@click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
+@click.option('--select', type=str, help='DBT style select string')
+@click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
+def trun(full_refresh, select, fail_fast):
+    args = []
+    if select:
+        args.append('--select')
+        args.append(select)
+    if fail_fast:
+        args.append('--fail-fast')
+    print(f'Starting a dbt build with args: {args}')
+    run_args = args
+    if full_refresh:
+        run_args.append('--full-refresh')
+    try:
+        execute_dbt_command('seed', run_args)
+    except subprocess.CalledProcessError as e:
+        print(e)
+        sys.exit(1)
+
+    try:
+        execute_dbt_command('test', args)
+    except subprocess.CalledProcessError as e:
+        print(e)
+        sys.exit(1)
+
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 @click.option('--select', type=str, help='DBT style select string')
 @click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
 def run(full_refresh, select, fail_fast):
     args = []
@@ -65,14 +92,33 @@
         run_args.append('--full-refresh')
     try:
         execute_dbt_command('seed', run_args)
     except subprocess.CalledProcessError as e:
         print(e)
         sys.exit(1)
 
+@cdbt.command()
+@click.option('--select', type=str, help='DBT style select string')
+@click.option('--fail-fast', is_flag=True, help='Fail fast on errors.')
+def test(full_refresh, select, fail_fast):
+    args = []
+    if select:
+        args.append('--select')
+        args.append(select)
+    if fail_fast:
+        args.append('--fail-fast')
+
+    run_args = args
+    if full_refresh:
+        run_args.append('--full-refresh')
+    try:
+        execute_dbt_command('seed', run_args)
+    except subprocess.CalledProcessError as e:
+        print(e)
+        sys.exit(1)
 
 @cdbt.command()
 def compile(full_refresh, select, fail_fast):
     try:
         subprocess.run(['dbt', 'compile'], check=True)
     except subprocess.CalledProcessError as e:
         print(e)
@@ -83,20 +129,18 @@
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 def sbuild(full_refresh):
     print('Starting a state build based on local manifest.json')
     artifact_dir = '_artifacts'
     target_dir = 'target'
     # Path to the artifacts file that will be generated by the dbt compile command representing the current state.
     manifest_path = os.path.join('./', target_dir, 'manifest.json')
-    # Path to the backup file to create in case of an error.
-    manifest_backup_path = os.path.join('./', artifact_dir, 'manifest.json_bak')
     # Path to the artifact file that represents the prior build state.
     manifest_artifact_path = os.path.join('./', artifact_dir, 'manifest.json')
 
-    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_backup_path, manifest_path, full_refresh,
+    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_path, full_refresh,
                               roll_back_manifest_flag=True)
 
 
 @cdbt.command()
 @click.option('--full-refresh', is_flag=True, help='Run a full refresh on all models.')
 def pbuild(full_refresh):
     print('Starting a state build based on production manifest.json')
@@ -106,83 +150,78 @@
     try:
         subprocess.run(['dbt', 'run-operation', 'get_last_artifacts'], check=True)
     except subprocess.CalledProcessError as e:
         print(e)
         sys.exit(1)
 
     manifest_path = os.path.join('.', target_dir, 'manifest.json')
-    manifest_backup_path = os.path.join('.', artifact_dir, 'manifest.json_bak')
     manifest_artifact_path = os.path.join('.', artifact_dir, 'manifest.json')
 
-    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_backup_path, manifest_path, full_refresh,
+    execute_state_based_build(artifact_dir, manifest_artifact_path, manifest_path, full_refresh,
                               roll_back_manifest_flag=False)
 
 
-def execute_state_based_build(artifact_dir: str, manifest_artifact_path: str, manifest_backup_path: str,
-                              manifest_path: str, full_refresh: bool, roll_back_manifest_flag: bool):
-    print(f'Pulling manifest from {manifest_artifact_path}')
+def execute_state_based_build(artifact_dir: str, manifest_artifact_path: str, manifest_path: str, full_refresh: bool,
+                              roll_back_manifest_flag: bool):
     if roll_back_manifest_flag:
-        # Backup and move manifest.json. Only used for local state build. Not used for pdbuild (production build).
-        # First move the current manifest to the backup location
-        shutil.copy(manifest_artifact_path, manifest_backup_path)
-        #
+        print(f'Making a backup of the current manifest.json at {manifest_path} to {manifest_artifact_path}')
+        # Move the manifest from ./target to ./_artifacts. This becomes the prior state. Only used for local state
+        # build. Not used for pdbuild (production build).
         shutil.move(manifest_path, manifest_artifact_path)
     # Execute dbt compile
     try:
         subprocess.run(['dbt', 'compile'], check=True)
     except subprocess.CalledProcessError:
-        # Rollback if dbt compile fails
-        shutil.move(manifest_artifact_path, manifest_path)
-        shutil.move(manifest_backup_path, manifest_artifact_path)
         sys.exit(1)
     # Construct state commands
     state_flags = [
         '--select', 'state:modified+',
         '--state', os.path.join('.', artifact_dir) + '/'
     ]
 
     # Execute dbt seed
     try:
         execute_dbt_command('seed', state_flags)
     except subprocess.CalledProcessError as e:
         if roll_back_manifest_flag:
-            roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path)
+            roll_back_manifest(e, manifest_artifact_path, manifest_path)
         else:
             print(e)
             sys.exit(1)
 
     # Execute dbt run
     if full_refresh:
         run_flags = state_flags + ['--full-refresh']
     else:
         run_flags = state_flags
     try:
         execute_dbt_command('run', run_flags)
     except subprocess.CalledProcessError as e:
         if roll_back_manifest_flag:
-            roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path)
+            roll_back_manifest(e, manifest_artifact_path, manifest_path)
         else:
             print(e)
             sys.exit(1)
 
     # Execute dbt test
     try:
         execute_dbt_command('test', state_flags)
     except subprocess.CalledProcessError as e:
         if roll_back_manifest_flag:
-            roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path)
+            roll_back_manifest(e, manifest_artifact_path, manifest_path)
         else:
             print(e)
             sys.exit(1)
 
 
-def roll_back_manifest(e, manifest_artifact_path, manifest_backup_path, manifest_path):
+def roll_back_manifest(e, manifest_artifact_path, manifest_path):
     print(f"DBT build failed. Rolling back manifest state with error\n {e}")
+    # Move the manifest.json from _artifacts back to target dir. If the build failed, we want to rebuild against this
+    # state, not the one generated by the compile command.
     shutil.move(manifest_artifact_path, manifest_path)
-    shutil.move(manifest_backup_path, manifest_artifact_path)
     sys.exit(1)
 
 
 def execute_dbt_command(command: str, args: List[str]):
     command = ['dbt', command] + args
     print(f'Running command: {command}')
     try:
```

### Comparing `cdbt-0.1.0/setup.py` & `cdbt-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.1.0',
+    version='0.1.1',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='craiglathrop218@gmail.com',
     packages=find_packages(),
     install_requires=[
         'click',
     ],
```
