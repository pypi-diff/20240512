# Comparing `tmp/stackql_deploy-1.5.0.tar.gz` & `tmp/stackql_deploy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.5.0.tar", last modified: Tue Apr 30 05:55:00 2024, max compression
+gzip compressed data, was "stackql_deploy-1.5.1.tar", last modified: Sun May 12 18:09:13 2024, max compression
```

## Comparing `stackql_deploy-1.5.0.tar` & `stackql_deploy-1.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.684119 stackql_deploy-1.5.0/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.5.0/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)    14058 2024-04-30 05:55:00.668063 stackql_deploy-1.5.0/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)    13456 2024-04-30 05:54:37.000000 stackql_deploy-1.5.0/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-30 05:55:00.686119 stackql_deploy-1.5.0/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1705 2024-04-30 05:26:37.000000 stackql_deploy-1.5.0/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:54:59.798435 stackql_deploy-1.5.0/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-30 05:28:09.000000 stackql_deploy-1.5.0/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9137 2024-04-29 20:52:47.000000 stackql_deploy-1.5.0/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.140734 stackql_deploy-1.5.0/stackql_deploy/cmd/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    12761 2024-04-30 03:13:03.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/build.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3435 2024-04-29 20:52:47.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/teardown.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     4757 2024-04-30 03:14:29.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/test.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.340212 stackql_deploy-1.5.0/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.5.0/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.5.0/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     4061 2024-04-22 20:59:53.000000 stackql_deploy-1.5.0/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3985 2024-04-22 21:39:51.000000 stackql_deploy-1.5.0/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6689 2024-04-23 05:16:36.000000 stackql_deploy-1.5.0/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.383754 stackql_deploy-1.5.0/stackql_deploy/templates/
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.432341 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_docs/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
--rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_manifest.yml.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.478921 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_queries/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.599374 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_resources/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.649118 stackql_deploy-1.5.0/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)    14058 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      848 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.983848 stackql_deploy-1.5.1/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.5.1/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    14058 2024-05-12 18:09:13.974836 stackql_deploy-1.5.1/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    13456 2024-04-30 05:54:37.000000 stackql_deploy-1.5.1/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-05-12 18:09:13.985042 stackql_deploy-1.5.1/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1705 2024-05-12 18:08:22.000000 stackql_deploy-1.5.1/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.421332 stackql_deploy-1.5.1/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-05-12 18:08:22.000000 stackql_deploy-1.5.1/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9256 2024-05-11 21:42:52.000000 stackql_deploy-1.5.1/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.665283 stackql_deploy-1.5.1/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.5.1/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    13936 2024-05-12 08:51:35.000000 stackql_deploy-1.5.1/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3408 2024-05-11 21:45:58.000000 stackql_deploy-1.5.1/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5870 2024-05-12 08:51:35.000000 stackql_deploy-1.5.1/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.801463 stackql_deploy-1.5.1/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.5.1/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.5.1/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5860 2024-05-11 17:10:47.000000 stackql_deploy-1.5.1/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     4195 2024-05-11 05:38:21.000000 stackql_deploy-1.5.1/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6689 2024-04-23 05:16:36.000000 stackql_deploy-1.5.1/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.830088 stackql_deploy-1.5.1/stackql_deploy/templates/
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.864611 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_docs/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_manifest.yml.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.903587 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_queries/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.934931 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_resources/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.5.1/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-05-12 18:09:13.963536 stackql_deploy-1.5.1/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    14058 2024-05-12 18:09:13.000000 stackql_deploy-1.5.1/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      848 2024-05-12 18:09:13.000000 stackql_deploy-1.5.1/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-05-12 18:09:13.000000 stackql_deploy-1.5.1/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-05-12 18:09:13.000000 stackql_deploy-1.5.1/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-05-12 18:09:13.000000 stackql_deploy-1.5.1/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-05-12 18:09:13.000000 stackql_deploy-1.5.1/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.5.0/LICENSE` & `stackql_deploy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.5.0/PKG-INFO` & `stackql_deploy-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.5.0/README.rst` & `stackql_deploy-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.5.0/setup.py` & `stackql_deploy-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 # with open('LICENSE', encoding='utf-8') as f:
 #     license_text = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.5.0',
+    version='1.5.1',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/cli.py` & `stackql_deploy-1.5.1/stackql_deploy/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 def build(ctx, stack_dir, stack_env, log_level, env_file, env, dry_run, on_failure):
     """Create or update resources."""
     setup_logger(log_level, locals())
     env_vars = load_env_vars(env_file, env)
     stackql = get_stackql_instance(ctx.obj['custom_registry'], ctx.obj['download_dir'])
     provisioner = StackQLProvisioner(stackql, env_vars, logger, stack_dir, stack_env)
     provisioner.run(dry_run, on_failure)
-    click.echo(f"Build command executed. Dry run: {dry_run}")
+    click.echo(f"🚀 build complete (dry run: {dry_run})")
 
 #
 # teardown command
 #
 
 @cli.command()
 @click.argument('stack_dir')
@@ -105,15 +105,15 @@
     stackql = get_stackql_instance(
         custom_registry=ctx.obj.get('custom_registry'), 
         download_dir=ctx.obj.get('download_dir')
     )
     vars = load_env_vars(env_file, env)
     deprovisioner = StackQLDeProvisioner(stackql, vars, logger, stack_dir, stack_env)
     deprovisioner.run(dry_run, on_failure)
-
+    click.echo(f"🚧 teardown complete (dry run: {dry_run})")
 
 #
 # test command
 #
 
 @cli.command()
 @click.argument('stack_dir')
@@ -130,15 +130,15 @@
     stackql = get_stackql_instance(
         custom_registry=ctx.obj.get('custom_registry'), 
         download_dir=ctx.obj.get('download_dir')
     )
     vars = load_env_vars(env_file, env)
     test_runner = StackQLTestRunner(stackql, vars, logger, stack_dir, stack_env)
     test_runner.run(dry_run, on_failure)
-
+    click.echo(f"🔍 tests complete (dry run: {dry_run})")
 
 #
 # info command
 #
 
 # stackql-deploy --custom-registry="https://registry-dev.stackql.app/providers" --download-dir . info
 @cli.command()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/cmd/build.py` & `stackql_deploy-1.5.1/stackql_deploy/cmd/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,27 +47,27 @@
         for key in expected_exports:
             if key not in export:
                 catch_error_and_exit(f"exported key '{key}' not found in exports for {resource['name']}.", self.logger)
 
         for key, value in export.items():
             if key in protected_exports:
                 mask = '*' * len(str(value))
-                self.logger.info(f"set [{key}] to [{mask}] in exports")
+                self.logger.info(f"🔒  set protected variable [{key}] to [{mask}] in exports")
             else:
-                self.logger.info(f"set [{key}] to [{value}] in exports")
+                self.logger.info(f"➡️  set [{key}] to [{value}] in exports")
 
             self.global_context[key] = value  # Update global context with exported values        
 
 
     def run(self, dry_run, on_failure):
 
         self.logger.info(f"Deploying [{self.stack_name}] in [{self.stack_env}] environment {'(dry run)' if dry_run else ''}")
 
         # get global context and pull providers
-        self.global_context, self.providers = get_global_context_and_providers(self.env, self.manifest, self.vars, self.stack_env, self.stackql, self.logger)            
+        self.global_context, self.providers = get_global_context_and_providers(self.env, self.manifest, self.vars, self.stack_env, self.stack_name, self.stackql, self.logger)            
 
         for resource in self.manifest.get('resources', []):
 
             self.logger.info(f"processing resource: {resource['name']}")
 
             type = resource.get('type', 'resource')
 
@@ -130,15 +130,14 @@
 
             preflight_query = None
             postdeploy_query = None
             exports_query = None
 
             if test_queries == {}:
                 self.logger.info(f"test query file not found for {resource['name']}. Skipping tests.")
-                continue
             else:
                 if 'preflight' in test_queries:
                     preflight_query = test_queries['preflight']
                 
                 if 'postdeploy' in test_queries:
                     postdeploy_query = test_queries['postdeploy']
                     postdeploy_retries = test_query_options.get('postdeploy', {}).get('retries', 10)
@@ -212,35 +211,52 @@
                     self.logger.info(f"running post deploy check for [{resource['name']}]...")
                     post_deploy_check_passed = perform_retries(resource, postdeploy_query, postdeploy_retries, postdeploy_retry_delay, self.stackql, self.logger)
                     
                 #
                 # postdeploy check complete
                 #
                 if not post_deploy_check_passed:
-                    catch_error_and_exit(f"deployment failed for {resource['name']} after post-deploy checks.", self.logger)
+                    catch_error_and_exit(f"❌ deployment failed for {resource['name']} after post-deploy checks.", self.logger)
 
             #
             # exports
             #
             if exports_query:
                 expected_exports = resource.get('exports', [])
 
                 if len(expected_exports) > 0:
                     protected_exports = resource.get('protected', [])
 
                     if not dry_run:
                         self.logger.info(f"exporting variables for [{resource['name']}]...")
                         exports = run_stackql_query(exports_query, self.stackql, True, self.logger, exports_retries, exports_retry_delay)
                         self.logger.debug(f"exports: {exports}")
-                        if len(exports) != 1 or not isinstance(exports[0], dict):
-                            catch_error_and_exit("exports should include one row only", self.logger)
+                        
+                        if len(exports) > 1:
+                            catch_error_and_exit(f"exports should include one row only, received {str(len(exports))} rows", self.logger)
+
+                        if len(exports) == 1 and not isinstance(exports[0], dict):
+                            catch_error_and_exit(f"exports must be a dictionary, received {str(exports[0])}", self.logger)                            
 
                         export = exports[0]
-                        self._export_vars(resource, export, expected_exports, protected_exports)
+                        if len(exports) == 0:
+                            export = {key: '' for key in expected_exports}
+                        else:
+                            export_data = {}
+                            for key in expected_exports:
+                                # Check if the key's value is a simple string or needs special handling
+                                if isinstance(export.get(key), dict) and 'String' in export[key]:
+                                    # Assume complex object that needs extraction from 'String'
+                                    export_data[key] = export[key]['String']
+                                else:
+                                    # Treat as a simple key-value pair
+                                    export_data[key] = export.get(key, '')  # Default to empty string if key is missing
+
+                        self._export_vars(resource, export_data, expected_exports, protected_exports)
                     else:
                         self.logger.info(f"dry run exports query for [{resource['name']}]:\n\n{exports_query}\n")
 
             if not dry_run:
                 if type == 'resource':
-                    self.logger.info(f"successfully deployed {resource['name']}")
+                    self.logger.info(f"✅ successfully deployed {resource['name']}")
                 elif type == 'query':
-                    self.logger.info(f"successfully exported variables for query in {resource['name']}")
+                    self.logger.info(f"✅ successfully exported variables for query in {resource['name']}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/cmd/teardown.py` & `stackql_deploy-1.5.1/stackql_deploy/cmd/teardown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from ..lib.utils import perform_retries, run_stackql_command
+from ..lib.utils import perform_retries, run_stackql_command, catch_error_and_exit
 from ..lib.config import setup_environment, load_manifest, get_global_context_and_providers, get_full_context
 from ..lib.templating import get_queries
 
 class StackQLDeProvisioner:
 
     def __init__(self, stackql, vars, logger, stack_dir, stack_env):
         self.stackql = stackql
@@ -16,15 +16,15 @@
         self.stack_name = self.manifest.get('name', stack_dir)
 
     def run(self, dry_run, on_failure):
 
         self.logger.info(f"Tearing down [{self.stack_name}] in [{self.stack_env}] environment {'(dry run)' if dry_run else ''}")
 
         # get global context and pull providers
-        self.global_context, self.providers = get_global_context_and_providers(self.env, self.manifest, self.vars, self.stack_env, self.stackql, self.logger)
+        self.global_context, self.providers = get_global_context_and_providers(self.env, self.manifest, self.vars, self.stack_env, self.stack_name, self.stackql, self.logger)
 
         for resource in reversed(self.manifest['resources']):
             # process resources in reverse order
 
             # get full context
             full_context = get_full_context(self.env, self.global_context, resource, self.logger)    
 
@@ -65,12 +65,10 @@
                 self.logger.info(f"post delete (pre-flight) check not configured for [{resource['name']}]")
             elif dry_run:
                 self.logger.info(f"dry run delete (pre-flight) check for [{resource['name']}]:\n\n{preflight_query}\n")
             else:
                 resource_deleted = perform_retries(resource, preflight_query, 10, 10, self.stackql, self.logger, delete_test=True)
 
             if not dry_run and not resource_deleted:
-                error_message = f"failed to delete {resource['name']}."
-                self.logger.error(error_message)
-                sys.exit(error_message)
+                catch_error_and_exit(f"❌ failed to delete {resource['name']}.", self.logger)
             else:
-                self.logger.info(f"successfully deleted {resource['name']}")
+                self.logger.info(f"✅ successfully deleted {resource['name']}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/cmd/test.py` & `stackql_deploy-1.5.1/stackql_deploy/cmd/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,26 +19,26 @@
         for key in expected_exports:
             if key not in export:
                 catch_error_and_exit(f"exported key '{key}' not found in exports for {resource['name']}.", self.logger)
 
         for key, value in export.items():
             if key in protected_exports:
                 mask = '*' * len(str(value))
-                self.logger.info(f"set [{key}] to [{mask}] in exports")
+                self.logger.info(f"🔒  set protected variable [{key}] to [{mask}] in exports")
             else:
-                self.logger.info(f"set [{key}] to [{value}] in exports")
+                self.logger.info(f"➡️  set [{key}] to [{value}] in exports")
 
             self.global_context[key] = value  # Update global context with exported values
 
     def run(self, dry_run, on_failure):
         
         self.logger.info(f"Testing [{self.stack_name}] in [{self.stack_env}] environment {'(dry run)' if dry_run else ''}")
 
         # get global context and pull providers
-        self.global_context, self.providers = get_global_context_and_providers(self.env, self.manifest, self.vars, self.stack_env, self.stackql, self.logger)
+        self.global_context, self.providers = get_global_context_and_providers(self.env, self.manifest, self.vars, self.stack_env, self.stack_name, self.stackql, self.logger)
 
         for resource in self.manifest.get('resources', []):
 
             # get full context
             full_context = get_full_context(self.env, self.global_context, resource, self.logger)    
 
             # get resource queries
@@ -58,46 +58,61 @@
 
             #
             # postdeploy check
             #
             post_deploy_check_passed = False
             if not postdeploy_query:
                 post_deploy_check_passed = True
-                self.logger.info(f"test not configured for [{resource['name']}], not waiting...")
+                self.logger.info(f"❓ test not configured for [{resource['name']}]")
             elif dry_run:
                 post_deploy_check_passed = True
                 self.logger.info(f"test query for [{resource['name']}]:\n\n{postdeploy_query}\n")
             else:
                 post_deploy_check_passed = run_test(resource, postdeploy_query, self.stackql, self.logger)
 
             #
             # postdeploy check complete
             #
+
             if not post_deploy_check_passed:
-                error_message = f"test failed for {resource['name']}."
-                self.logger.error(error_message)
-                sys.exit(error_message)
+                catch_error_and_exit(f"❌ test failed for {resource['name']}.", self.logger)
 
             #
             # exports
             #
             if exports_query:
                 expected_exports = resource.get('exports', [])
 
                 if len(expected_exports) > 0:
                     protected_exports = resource.get('protected', [])
 
                     if not dry_run:
                         self.logger.info(f"exporting variables for [{resource['name']}]...")
                         exports = run_stackql_query(exports_query, self.stackql, True, self.logger, exports_retries, exports_retry_delay)
                         self.logger.debug(f"exports: {exports}")
-                        if len(exports) != 1 or not isinstance(exports[0], dict):
-                            catch_error_and_exit("exports should include one row only", self.logger)
+                        
+                        if len(exports) > 1:
+                            catch_error_and_exit(f"exports should include one row only, received {str(len(exports))} rows", self.logger)
+
+                        if len(exports) == 1 and not isinstance(exports[0], dict):
+                            catch_error_and_exit(f"exports must be a dictionary, received {str(exports[0])}", self.logger)                            
 
                         export = exports[0]
-                        self._export_vars(resource, export, expected_exports, protected_exports)
+                        if len(exports) == 0:
+                            export = {key: '' for key in expected_exports}
+                        else:
+                            export_data = {}
+                            for key in expected_exports:
+                                # Check if the key's value is a simple string or needs special handling
+                                if isinstance(export.get(key), dict) and 'String' in export[key]:
+                                    # Assume complex object that needs extraction from 'String'
+                                    export_data[key] = export[key]['String']
+                                else:
+                                    # Treat as a simple key-value pair
+                                    export_data[key] = export.get(key, '')  # Default to empty string if key is missing
+
+                        self._export_vars(resource, export_data, expected_exports, protected_exports)
                     else:
                         self.logger.info(f"dry run exports query for [{resource['name']}]:\n\n{exports_query}\n")
 
-
             if not dry_run:
-                self.logger.info(f"test passed for {resource['name']}")
+                self.logger.info(f"✅ test passed for {resource['name']}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/lib/config.py` & `stackql_deploy-1.5.1/stackql_deploy/lib/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,80 @@
 import os, yaml, json
 from .utils import pull_providers, catch_error_and_exit
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 from jinja2.utils import markupsafe
+from jinja2 import TemplateError
 
-def render_globals(env, vars, global_vars, stack_env):
-    # Render globals with vars and include the stack_env as a special variable
-    global_context = {'stack_env': stack_env}
-    # Render each global variable defined in the manifest
+def render_globals(env, vars, global_vars, stack_env, stack_name):
+    # Establish the context with stack environment and stack name, and other vars if needed
+    global_context = {'stack_env': stack_env, 'stack_name': stack_name}
+
+    def render_value(value, context):
+        """Handles recursive rendering of values that might be strings, lists, or dictionaries."""
+        if isinstance(value, str):
+            try:
+                # Render the string using Jinja2 with the current context to resolve any templates
+                template = env.from_string(value)
+                return template.render(**context)  # Use **context to spread the context dictionary
+            except TemplateError as e:
+                print(f"Error rendering template: {e}")
+                return value
+        elif isinstance(value, dict):
+            # Recursively process and serialize each dictionary after processing
+            processed_dict = {k: render_value(v, context) for k, v in value.items()}
+            return json.dumps(processed_dict, ensure_ascii=False).replace('True', 'true').replace('False', 'false')
+        elif isinstance(value, list):
+            # First resolve templates in list items, then serialize the list as a whole
+            processed_list = [render_value(item, context) for item in value]
+            # Ensure each item is treated as a resolved string before forming the JSON array
+            return '[' + ', '.join(processed_list) + ']'
+        else:
+            return value
+
+    # Update the global context with the rendered results
     for global_var in global_vars:
-        # Assume each global_var is a dictionary with 'name' and 'value' keys
-        template = env.from_string(global_var['value'])
-        global_context[global_var['name']] = template.render(globals=global_context, vars=vars)
+        global_context[global_var['name']] = render_value(global_var['value'], global_context)
+
     return global_context
 
 def render_properties(env, resource_props, global_context, logger):
-    # Render properties with globals and vars
     prop_context = {}
     for prop in resource_props:
         try:
             if 'value' in prop:
-                # Check if value is a dict, and convert it to a JSON string
                 if isinstance(prop['value'], (dict, list)):
-                    prop_context[prop['name']] = markupsafe.Markup(json.dumps(prop['value'], separators=(',', ':')))
+                    # Convert dict or list directly to JSON string
+                    json_string = json.dumps(prop['value'], separators=(',', ':')).replace('True', 'true').replace('False', 'false')
+                    template = env.from_string(json_string)
+                    rendered_json_string = template.render(global_context)
+                    prop_context[prop['name']] = rendered_json_string
                 else:
-                    # Single value for all environments
+                    # Render non-dict/list values as regular strings
                     template = env.from_string(str(prop['value']))
-                    prop_context[prop['name']] = template.render(globals=global_context)
+                    # rendered_value = template.render(globals=global_context)
+                    rendered_value = template.render(global_context)
+                    prop_context[prop['name']] = rendered_value
             elif 'values' in prop:
-                # Environment-specific values
                 env_value = prop['values'].get(global_context['stack_env'], {}).get('value')
                 if env_value is not None:
                     if isinstance(env_value, (dict, list)):
-                        prop_context[prop['name']] =  markupsafe.Markup(json.dumps(prop['value'], separators=(',', ':')))
+                        json_string = json.dumps(env_value, separators=(',', ':')).replace('True', 'true').replace('False', 'false')
+                        prop_context[prop['name']] = json_string
                     else:
                         template = env.from_string(str(env_value))
-                        prop_context[prop['name']] = template.render(globals=global_context)
+                        # rendered_value = template.render(globals=global_context)
+                        rendered_value = template.render(global_context)
+                        prop_context[prop['name']] = rendered_value
                 else:
                     catch_error_and_exit(f"No value specified for property '{prop['name']}' in stack_env '{global_context['stack_env']}'.", logger)
-
         except Exception as e:
             catch_error_and_exit(f"Failed to render property '{prop['name']}': {e}", logger)
-
     return prop_context
 
+
 #
 # exported functions
 #
 
 def load_manifest(stack_dir, logger):
     try:
         # Load and parse the stackql_manifest.yml
@@ -56,31 +84,32 @@
         catch_error_and_exit("failed to load manifest: " + str(e), logger)
 
 def setup_environment(stack_dir, logger):
     if not os.path.exists(stack_dir):
         catch_error_and_exit("stack directory does not exist.", logger)
     env = Environment(
         loader=FileSystemLoader(os.getcwd()),
-        autoescape=select_autoescape()
+        autoescape=False
     )
     return env
 
-def get_global_context_and_providers(env, manifest, vars, stack_env, stackql, logger):
+def get_global_context_and_providers(env, manifest, vars, stack_env, stack_name, stackql, logger):
     # Extract the global variables from the manifest and include stack_env
     try:
         global_vars = manifest.get('globals', [])
-        global_context = render_globals(env, vars, global_vars, stack_env)
+        global_context = render_globals(env, vars, global_vars, stack_env, stack_name)
         providers = manifest.get('providers', [])
         pull_providers(providers, stackql, logger)
         return global_context, providers
     except Exception as e:
         catch_error_and_exit("failed to prepare the context: " + str(e), logger)
 
 def get_full_context(env, global_context, resource, logger):
     try:
         resource_props = resource.get('props', {})
+        logger.debug(f"rendering properties for {resource['name']}...")
         prop_context = render_properties(env, resource_props, global_context, logger)
         full_context = {**global_context, **prop_context}
         logger.debug(f"full context: {full_context}")
         return full_context
     except Exception as e:
         catch_error_and_exit(f"failed to render properties for {resource.get('name', 'unknown')}: " + str(e), logger)
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/lib/templating.py` & `stackql_deploy-1.5.1/stackql_deploy/lib/templating.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import re
 from .utils import catch_error_and_exit
 from jinja2 import TemplateError
 from jinja2.utils import markupsafe
 
 def parse_anchor(anchor):
     """Parse anchor to extract key and options."""
     parts = anchor.split(',')
@@ -13,40 +14,43 @@
         if '=' in part:
             option_key, option_value = part.split('=')
             options[option_key.strip()] = int(option_value.strip())
     return key, options
 
 def is_json(myjson):
     try:
-        json_object = json.loads(myjson)
-    except (ValueError, TypeError):
+        obj = json.loads(myjson)
+        return isinstance(obj, (dict, list))  # Only return True for JSON objects or arrays
+    except ValueError:
         return False
-    return True
 
 def render_queries(env, queries, context):
     rendered_queries = {}
     for key, query in queries.items():
         try:
-            # Clone the context to avoid modifying the original context outside this function
             temp_context = context.copy()
-            
-            # Check and render JSON structures in the context
+
             for ctx_key, ctx_value in temp_context.items():
                 if isinstance(ctx_value, str) and is_json(ctx_value):
-                    # Process JSON string
                     properties = json.loads(ctx_value)
-                    properties_rendered = env.from_string(json.dumps(properties)).render(temp_context)
-                    temp_context[ctx_key] = markupsafe.Markup(json.dumps(json.loads(properties_rendered), separators=(',', ':')))
-            # Render the query using the updated context
+                    # Serialize JSON ensuring booleans are lower case and using correct JSON syntax
+                    json_str = json.dumps(properties, ensure_ascii=False, separators=(',', ':')).replace('True', 'true').replace('False', 'false')
+                    # Correctly format JSON to use double quotes and pass directly since template handles quoting
+                    json_str = json_str.replace("'", "\\'")  # escape single quotes if any within strings
+                    temp_context[ctx_key] = json_str
+                # No need to alter non-JSON strings, assume the template handles them correctly
+
             template = env.from_string(query)
-            rendered_queries[key] = template.render(temp_context)
+            rendered_query = template.render(temp_context)
+            rendered_queries[key] = rendered_query
+
         except TemplateError as e:
-            raise RuntimeError(f"Error rendering query '{key}': {e}") from e
-        except json.JSONDecodeError as e:
-            continue  # If it's not JSON, just skip it
+            raise RuntimeError(f"Error rendering query '{key}': {e}")
+        except json.JSONDecodeError:
+            continue  # Skip non-JSON content
 
     return rendered_queries
 
 def load_sql_queries(file_path):
     """Loads SQL queries from a file, splits them by anchors, and extracts options."""
     queries = {}
     options = {}
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy/lib/utils.py` & `stackql_deploy-1.5.1/stackql_deploy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.5.0/stackql_deploy/templates/stackql_manifest.yml.template` & `stackql_deploy-1.5.1/stackql_deploy/templates/stackql_manifest.yml.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.5.0/stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template` & `stackql_deploy-1.5.1/stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.5.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template` & `stackql_deploy-1.5.1/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.5.0/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.5.1/stackql_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.5.0/stackql_deploy.egg-info/SOURCES.txt` & `stackql_deploy-1.5.1/stackql_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

