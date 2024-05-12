# Comparing `tmp/torch_model_manager-0.2.0.dev9.tar.gz` & `tmp/torch_model_manager-0.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev9.tar", last modified: Tue May  7 09:26:11 2024, max compression
+gzip compressed data, was "torch_model_manager-0.3.0.dev1.tar", last modified: Sun May 12 19:00:22 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev9.tar` & `torch_model_manager-0.3.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     8746 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     1482 2024-05-07 09:26:09.000000 torch_model_manager-0.2.0.dev9/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.310966 torch_model_manager-0.2.0.dev9/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       95 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    29212 2024-05-07 09:07:22.000000 torch_model_manager-0.2.0.dev9/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18476 2024-05-07 08:49:09.000000 torch_model_manager-0.2.0.dev9/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     8746 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      545 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       47 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     7112 2024-05-07 07:32:10.000000 torch_model_manager-0.2.0.dev9/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.413189 torch_model_manager-0.3.0.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-12 19:00:22.413189 torch_model_manager-0.3.0.dev1/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 19:00:22.413189 torch_model_manager-0.3.0.dev1/setup.cfg
+-rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-12 19:00:17.000000 torch_model_manager-0.3.0.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.405189 torch_model_manager-0.3.0.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.409189 torch_model_manager-0.3.0.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.409189 torch_model_manager-0.3.0.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.409189 torch_model_manager-0.3.0.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31675 2024-05-11 18:27:25.000000 torch_model_manager-0.3.0.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1672 2024-05-11 19:12:46.000000 torch_model_manager-0.3.0.dev1/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev1/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev1/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.413189 torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-12 19:00:22.000000 torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 19:00:22.000000 torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 19:00:22.000000 torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-12 19:00:22.000000 torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 19:00:22.000000 torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 19:00:22.413189 torch_model_manager-0.3.0.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev9/PKG-INFO` & `torch_model_manager-0.3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev9
+Version: 0.3.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev9/README.md` & `torch_model_manager-0.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev9/setup.py` & `torch_model_manager-0.3.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev9',
+    version='0.3.0.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.3.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev9/tests/test_utils/test_helpers.py` & `torch_model_manager-0.3.0.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev9/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.3.0.dev1/torch_model_manager/neptune_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -166,14 +166,51 @@
                     NeptuneManager.project[namespace].append(File.as_image(to_pil(tensor)), name=name, description=description)
             else:
                 for name, tensor in zip(names, tensors):
                     NeptuneManager.project[namespace].append(File.as_image(to_pil(tensor)), name=name)            
 
         print(Fore.GREEN+"The tensors are successfully uploaded to Neptune.", Fore.WHITE)
 
+    def log_dataframe(self, 
+                        dataframe: pd.DataFrame, 
+                        namespace: str, 
+                        df_format: bool=True,
+                        csv_format: bool=False, 
+                        profile_report_title: str=None,
+                        profile_report_namespace: str=None,
+                        **kwargs):
+        """
+        Log a dataframe to Neptune.
+
+        Args:
+            dataframe (pd.DataFrame): The dataframe to log.
+            namespace (str): The namespace to log the dataframe.
+            df_format (bool, optional): Whether to log the dataframe in HTML format. Defaults to True.
+            csv_format (bool, optional): Whether to log the dataframe in CSV format. Defaults to False.
+            profile_report_title (str, optional): The title of the profile report. Defaults to None.
+            profile_report_namespace (str, optional): The name of the profile report. Defaults to None.
+        """
+        assert df_format or csv_format, "At least one format should be chosen."
+        to_csv_kwargs = kwargs.get("csv_kwargs", {})
+        profile_report_kwargs = kwargs.get("profile_report_kwargs", {"dark_mode": True})
+        if df_format:
+            NeptuneManager.project[namespace].upload(File.as_html(dataframe))
+        if csv_format:
+            # create the temporary folder if it doesn't exist
+            csv_buffer = StringIO()
+            dataframe.to_csv(csv_buffer, **to_csv_kwargs)
+            NeptuneManager.project[namespace].upload(File.from_stream(csv_buffer, extension="csv"))
+            
+        if profile_report_namespace is not None and profile_report_title is not None:
+            profile = ProfileReport(dataframe, title=profile_report_title, **profile_report_kwargs)
+            
+            NeptuneManager.project[profile_report_namespace].upload(
+                File.from_content(profile.to_html(), extension="html")
+            )
+
     def log_hidden_conv2d(self, 
                           model: nn.Module,
                           input_data: torch.Tensor, 
                           indexes, 
                           method="layercam",
                           row_index: List[str] = None, 
                           save_path=None,
@@ -262,15 +299,28 @@
             self.log_tensors(tensors=res_row, 
                             names = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
                             namespace=namespace,
                             on_series=True)
                 
         print(Fore.GREEN+"The hidden conv2d layer outputs are successfully logged to Neptune.", Fore.WHITE)
         return result, row_index, col_index 
+    
+    def fetch_pkl_data(self, namespace: str):        
+        tmp_file = tempfile.NamedTemporaryFile(delete=True)
+        try :
+            NeptuneManager.project[namespace].download(tmp_file.name)
+            with open(tmp_file.name, 'rb') as f:
+                data = pickle.load(f)
         
+            print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
+            return data
+            
+        except:
+            print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
+
     class Run:
         """
         A class representing a Neptune run.
         """
         def __init__(self, 
                     name: str, 
                     description: str = None, 
@@ -384,47 +434,45 @@
             except:
                 print(Fore.RED+"The data are not loaded to Neptune. Please check the path or the data format.\
                     This also might due to the existence of the same path in the namespace which risks to be overweighted."+Fore.WHITE)
         
         def log_dataframe(self, 
                           dataframe: pd.DataFrame, 
                           namespace: str, 
-                          df_name: str,
                           df_format: bool=True,
                           csv_format: bool=False, 
                           profile_report_title: str=None,
-                          profile_report_name: str=None,
+                          profile_report_namespace: str=None,
                           **kwargs):
             """
             Log a dataframe to Neptune.
 
             Args:
                 dataframe (pd.DataFrame): The dataframe to log.
                 namespace (str): The namespace to log the dataframe.
-                df_name (str): The name of the dataframe.
                 df_format (bool, optional): Whether to log the dataframe in HTML format. Defaults to True.
                 csv_format (bool, optional): Whether to log the dataframe in CSV format. Defaults to False.
                 profile_report_title (str, optional): The title of the profile report. Defaults to None.
-                profile_report_name (str, optional): The name of the profile report. Defaults to None.
+                profile_report_namespace (str, optional): The name of the profile report. Defaults to None.
             """
             assert df_format or csv_format, "At least one format should be chosen."
             to_csv_kwargs = kwargs.get("csv_kwargs", {})
             profile_report_kwargs = kwargs.get("profile_report_kwargs", {"dark_mode": True})
             if df_format:
-                self.run[namespace][df_name].upload(File.as_html(dataframe))
+                self.run[namespace].upload(File.as_html(dataframe))
             if csv_format:
                 # create the temporary folder if it doesn't exist
                 csv_buffer = StringIO()
                 dataframe.to_csv(csv_buffer, **to_csv_kwargs)
-                self.run[namespace][df_name].upload(File.from_stream(csv_buffer, extension="csv"))
+                self.run[namespace].upload(File.from_stream(csv_buffer, extension="csv"))
                 
-            if profile_report_name is not None and profile_report_title is not None:
+            if profile_report_namespace is not None and profile_report_title is not None:
                 profile = ProfileReport(dataframe, title=profile_report_title, **profile_report_kwargs)
                 
-                self.run[namespace][profile_report_name].upload(
+                self.run[profile_report_namespace].upload(
                     File.from_content(profile.to_html(), extension="html")
                 )
             
         
         def track_metric(self, 
                          metric: Union[float, int],
                          namespace: str,
@@ -437,31 +485,40 @@
             Args:
                 model (nn.Module): The model to track the metric for.
                 metric (Union[float, int]): The metric value.
                 namespace (str): The namespace to log the metric.
             """
             self.run[namespace].append(metric, step=step, timestamp=timestamp, wait=wait)
 
-        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, keep_only_last = True, wait=False, **kwargs):
+        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, keep=3, wait=False, **kwargs):
+            parent_namespace = "/".join(namespace.split("/")[:-1])
+
+
             state_dict = {
                 "model_state_dict": model.state_dict(),
                 "optimizer_state_dict": optimizer.state_dict(),
                 "loss": loss,
                 "epoch": epoch,
                 **kwargs
             }
             
             tmp_file = tempfile.NamedTemporaryFile(suffix = '.pth', delete=True)
             torch.save(state_dict, tmp_file.name)
                 
-                
             self.log_files(namespace=namespace, data= None, from_path=tmp_file.name, extension='pth', wait=wait)
             
             print(Fore.GREEN+"The checkpoint is successfully logged to Neptune.", Fore.WHITE)
 
+
+            struct = helpers.sort_string_list(self.fetch_files(parent_namespace))
+
+            if len(struct) > keep:
+                for file in struct[:-keep]:
+                    self.run.pop(os.path.join(parent_namespace, file), wait=wait)
+
         def log_hyperparameters(self, 
                                hyperparams: dict, 
                                namespace: str):  
             """
             Log hyperparameters.
 
             Args:
@@ -484,31 +541,23 @@
             Args:
                 figure: The figure to log.
                 namespace (str): The namespace to log the figure.
             """
             self.run[namespace].upload(File.as_html(figure))
             print(Fore.GREEN+"The figure is successfully uploaded to Neptune.", Fore.WHITE)
         
-        def log_text(self, text, namespace, logger_name, level):
+        def log_text(self, text, namespace):
             """
             Log text.
 
             Args:
                 text: The text to log.
                 namespace (str): The namespace to log the text.
-                logger_name (str): The name of the logger.
-                level (str): The level of the log.
             """
-            assert level in ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], "The level should be one of the following: 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'"
-            level = eval(f"logging.{level}")
-            logger = logging.getLogger(logger_name)
-            logger.setLevel(level)
-            npt_handler = NeptuneHandler(run=self.run)
-            
-            logger.addHandler(npt_handler)
+
             self.run[namespace].log(text)
             print(Fore.GREEN+"The text is successfully logged to Neptune.", Fore.WHITE)
         
         def log_args(self, args, namespace):
             """
             Log arguments.
 
@@ -631,64 +680,77 @@
                                 namespace=namespace,
                                 on_series=True)
                     
             print(Fore.GREEN+"The hidden conv2d layer outputs are successfully logged to Neptune.", Fore.WHITE)
             return result, row_index, col_index
         
         def fetch_pkl_data(self, namespace: str):
-            
+            """
+            Fetches pickle data from Neptune.
+
+            Args:
+                namespace (str): The namespace where the data is stored.
+
+            Returns:
+                data: The fetched data.
+            """
             tmp_file = tempfile.NamedTemporaryFile(delete=True)
             try :
                 self.run[namespace].download(tmp_file.name)
                 with open(tmp_file.name, 'rb') as f:
                     data = pickle.load(f)
             
                 print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
                 return data
                 
             except:
                 print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
         def load_model_checkpoint(self, namespace, **kwargs):
+            """
+            Loads a model checkpoint from Neptune.
+
+            Args:
+                namespace (str): The namespace where the checkpoint is stored.
+                **kwargs: Additional keyword arguments for torch.load().
+
+            Returns:
+                state_dict: The loaded model state dictionary.
+            """
             tmp_file = tempfile.NamedTemporaryFile(delete=True)
             try:
                 self.run[namespace].download(tmp_file.name)
                 state_dict = torch.load(tmp_file.name, **kwargs)
                 
                 return state_dict
             except:
                 print(Fore.RED+"The checkpoint is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
         def fetch_files(self, namespace):
+            """
+            Fetches files from a specified namespace in Neptune.
+
+            Args:
+                namespace (str): The namespace containing the files.
+
+            Returns:
+                list: A list of filenames in the specified namespace.
+            """
             ns = namespace.split("/")
             
             struct = self.run.get_structure()
             for elem in ns :
                 struct = struct[elem]
             
             return list(struct.keys())
         
         def fetch_data(self, namespace):
-            return self.run[namespace].fetch_values()
-        
-        
-nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-                    run_ids_path="run_ids.json")
-
-
-
-# run = nm.Run(name="Image GAT Message Passing")
-# data = run.fetch_pkl_data("embeddings")
-# print(data)
-
-# from mrg32k3a.mrg32k3a import MRG32k3a
-# from matplotlib import pyplot as plt
-# from torch.nn import init
-
-
+            """
+            Fetches data from a specified namespace in Neptune.
 
-# a = init.kaiming_uniform_(torch.empty(10000, 10000), generator=torch.Generator(device="cpu"))
-# print(a.shape)
-# plt.hist2d(a[0], a[1], bins=200)
-# plt.show()
+            Args:
+                namespace (str): The namespace containing the data.
 
+            Returns:
+                list: A list of fetched data values.
+            """
+            return self.run[namespace].fetch_values()
```

### Comparing `torch_model_manager-0.2.0.dev9/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.3.0.dev1/torch_model_manager/torch_model_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -470,40 +470,51 @@
                                             workspace=image_workspace,
                                             on_series=True)
                 
 
         return result, row_index, col_index
     
     def init_model_parameters(self, method_weight, method_bias, **kwargs):
-        weight_args = kwargs.get('weight_args', None)
-        bias_args = kwargs.get('bias_args', None)
+        weight_args = kwargs.get('weight_args', {})
+        bias_args = kwargs.get('bias_args', {})
         
-        for layer in self.model.children():
+        def init_layer(layer):
             if isinstance(layer, (nn.Conv2d, 
                         nn.Linear, 
                         nn.ConvTranspose2d, 
                         nn.Conv3d, 
                         nn.ConvTranspose3d,
-                        nn.Embedding)):
+                        nn.Embedding,
+                        nn.BatchNorm1d,
+                        nn.BatchNorm2d,
+                        nn.BatchNorm3d)):
                 
-                weight_initializer = eval(method_weight)
-                bias_initializer = eval(method_bias)
+                weight_initializer = eval(f"{method_weight}_")
+                bias_initializer = eval(f"{method_bias}_")
                 
-                weight_initializer(layer.weight, weight_args)
+                weight_initializer(layer.weight, **weight_args)
                 if layer.bias is not None:
-                    bias_initializer(layer.bias, bias_args)
+                    bias_initializer(layer.bias, **bias_args)
+            
+            # Recursively initialize parameters for child layers
+            for sub_layer in layer.children():
+                init_layer(sub_layer)
+        
+        # Start initialization from the top-level layers
+        for layer in self.model.children():
+                init_layer(layer)
+
+        return self.model.state_dict()
+            
                     
-                
-                            
-                
-                
                         
-# model = nn.Embedding(12, 13)
-# for layer in model.modules():
-#     if isinstance(layer, (nn.Conv2d, nn.Linear, nn.Embedding)):
-#         layer.weight.data.fill_(1)
+# model = models.vgg16()
+# tmm = TorchModelManager(model)
+
+# tmm.init_model_parameters('zeros_', 'zeros_')
 
+# print(model)
         
 # for layer in model.modules():
 #     if isinstance(layer, (nn.Conv2d, nn.Linear, nn.Embedding)):
 #         print(layer.weight.data)
```

### Comparing `torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev9
+Version: 0.3.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.3.0.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 setup.py
 tests/test_torch_model_manager/__init__.py
 tests/test_torch_model_manager/test_torch_model_manager.py
 tests/test_utils/__init__.py
 tests/test_utils/test_helpers.py
 torch_model_manager/__init__.py
 torch_model_manager/neptune_manager.py
+torch_model_manager/notebook_manager.py
 torch_model_manager/torch_model_manager.py
+torch_model_manager/wandb_manager.py
 torch_model_manager.egg-info/PKG-INFO
 torch_model_manager.egg-info/SOURCES.txt
 torch_model_manager.egg-info/dependency_links.txt
 torch_model_manager.egg-info/requires.txt
 torch_model_manager.egg-info/top_level.txt
 utils/__init__.py
 utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev9/utils/helpers.py` & `torch_model_manager-0.3.0.dev1/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Any
 import matplotlib.pyplot as plt
 import torch
 from torchvision import transforms
 import json
+import pickle
 
 def required_kernel(in_size: int, out_size:int, stride=1, padding=1):
     assert in_size > 0, "Input size must be greater than 0"
     assert out_size > 0, "Output size must be greater than 0"
     assert in_size >= out_size, "Input size must be greater than or equal to output size"
     assert stride > 0, "Stride must be greater than 0"
     assert padding >= 0, "Padding must be greater than or equal to 0"
@@ -220,8 +221,56 @@
             recursive_delete(d[keys[0]], keys[1:])
     
     # Recursively search and delete item by key list
     recursive_delete(data, key_list)
     
     # Save the modified JSON data back to the file
     with open(json_file, 'w') as f:
-        json.dump(data, f, indent=4)
+        json.dump(data, f, indent=4)
+
+def sort_string_list(string_list, order='asc'):
+    def alphanum_key(s):
+        import re
+        return [int(text) if text.isdigit() else text.lower()
+                for text in re.split('([0-9]+)', s)]
+
+    return sorted(string_list, key=alphanum_key, reverse=(order == 'desc'))
+
+def load_data_from_path(file_path: str):
+    """
+    Load and deserialize data from a binary file using pickle.
+
+    Parameters:
+    - file_path (str): The path to the file from which data will be loaded.
+
+    Returns:
+    - loaded_data: The deserialized data.
+    """
+    assert isinstance(file_path, str), "file_path must be a string"
+
+    try:
+        # Load the data from the file
+        with open(file_path, 'rb') as file:
+            loaded_data = pickle.load(file)
+    
+
+        return loaded_data
+
+    except (IOError, FileNotFoundError, PermissionError, pickle.PickleError) as e:
+        print(f"Error during load_data_from_path: {e}")
+        return None
+    
+def dump_data(data, file_path: str) -> None:
+    """
+    Serialize and dump the data to a binary file using pickle.
+
+    Parameters:
+    - data: Any Python object to be serialized and saved.
+    - file_path (str): The path to the file where data will be saved.
+    """
+    assert isinstance(file_path, str), "file_path must be a string"
+    try:
+        with open(file_path, 'wb') as file:
+            pickle.dump(data, file)
+
+    except (IOError, FileNotFoundError, PermissionError) as e:
+        print(f"Error during dump_data: {e}")
```

