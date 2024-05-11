# Comparing `tmp/kfsconfig-2.1.3.tar.gz` & `tmp/kfsconfig-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.1.3.tar", max compression
+gzip compressed data, was "kfsconfig-2.1.4.tar", max compression
```

## Comparing `kfsconfig-2.1.3.tar` & `kfsconfig-2.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    15612 2024-05-11 21:43:13.411040 kfsconfig-2.1.3/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-11 21:43:13.411040 kfsconfig-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-11 21:43:13.411040 kfsconfig-2.1.3/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    16273 2024-05-11 22:33:45.399145 kfsconfig-2.1.4/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-11 22:33:45.399145 kfsconfig-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-11 22:33:45.399145 kfsconfig-2.1.4/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.4/PKG-INFO
```

### Comparing `kfsconfig-2.1.3/KFSconfig/KFSconfig.py` & `kfsconfig-2.1.4/KFSconfig/KFSconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,36 +78,40 @@
 
     Raises:
     - KeyError: config_default is missing key "content" while trying to save raw string content
     - ValueError: After going through all enabled sources, a setting is still None and setting_None_ok is false.
     """
 
     config: dict[str, typing.Any]={key: None for key in config_default.keys()}  # loaded config, initialised empty with same keys as config_default
+    sources_loaded: list[str]=[]                                                # sources loaded successfully
     
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
     if env==False and (config_filepaths==None or len(config_filepaths)==0): # if no source enabled: error
         logger.error(f"No config source is enabled. Loading config is impossible.")
         raise ValueError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: No config source is enabled. Loading config is impossible.")
 
 
     if env==True:
         config.update({k: v for k, v in _load_env().items() if k in config.keys() and config[k]==None}) # update config with environmental variables, only overwrite if key already exists and value is None
+        sources_loaded.append("environmental variables")                                                # log success
     
     if config_filepaths!=None and len(config_filepaths)!=0:
         for config_filepath in config_filepaths:
             try:
                 config.update({k: v for k, v in _load_config_file(config_filepath).items() if k in config.keys() and config[k]==None})  # update config with config file, only overwrite if key already exists and value is None
-            except (FileNotFoundError, IsADirectoryError):                                                                              # if fails: ignore source
+            except (FileNotFoundError, IsADirectoryError, OSError):                                                                     # if fails: ignore source
                 pass
-    logger.debug(f"Loaded all config sources.")
+            else:
+                sources_loaded.append(f"\"{config_filepath}\"")                                                                         # log success
+    logger.info(f"Loaded config from: {", ".join(sources_loaded)}")
     logger.debug(config)
 
 
     if any(v==None for v in config.values())==True and setting_None_ok==False:                                                                                  # if any setting is still None and not allowed to be None: error
         logger.error(f"After going through all enabled sources, settings {[k for k, v in config.items() if v==None]} are still None and setting_None_ok is false.")
         
         if config_filepaths!=None and 1<=len(config_filepaths) and all([os.path.exists(config_filepath)==False for config_filepath in config_filepaths])==True: # if a file source is enabled and no files at set filepaths exist: offer creation of default config file at highest priority filepath using config_default's values
@@ -137,17 +141,17 @@
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
 
-    logger.info(f"Loading environmental variables...")
+    logger.debug(f"Loading environmental variables...")
     config=dict(os.environ) # load environmental variables
-    logger.info(f"\rLoaded environmental variables.")
+    logger.debug(f"\rLoaded environmental variables.")
     logger.debug(config)
 
     return config
 
 
 def _load_config_file(config_filepath: str) -> dict[str, typing.Any]:
     """
@@ -158,50 +162,52 @@
 
     Returns:
     - config_filecontent: content of config file as a dictionary
 
     Raises:
     - FileNotFoundError: config_filepath does not exist
     - IsADirectoryError: config_filepath is a directory
+    - NotImplementedError: file extension is not implemented yet
+    - OSError: loading config_filepath failed
     """
 
     config: dict[str, typing.Any]   # config file
 
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
     if os.path.exists(config_filepath)==False:  # if config file does not exist: error
-        logger.error(f"Loading \"{config_filepath}\" failed, because it does not exist.")
-        raise FileNotFoundError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because file does not exist.")
+        logger.warning(f"Loading \"{config_filepath}\" failed, because it does not exist. Source will be skipped.")
+        raise FileNotFoundError(f"Warning in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because file does not exist. Source will be skipped.")
     if os.path.isdir(config_filepath)==True:    # if config file is a directory: error
-        logger.error(f"Loading \"{config_filepath}\" failed, because it is a directory.")
-        raise IsADirectoryError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because it is a directory.")
+        logger.warning(f"Loading \"{config_filepath}\" failed, because it is a directory. Source will be skipped.")
+        raise IsADirectoryError(f"Warning in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because it is a directory. Source will be skipped.")
 
 
-    logger.info(f"Loading \"{config_filepath}\"...")
+    logger.debug(f"Loading \"{config_filepath}\"...")
     try:
         with open(config_filepath, "rt", encoding="utf8") as config_file:                                                                                                               # read file
             match os.path.basename(config_filepath).rsplit(".", 1)[-1]:                                                                                                                 # parse file content
                 case "env":
                     config={line.strip(" ").split("=")[0]: line.strip(" ").split("=")[1] for line in config_file.readlines() if "=" in line and line.strip(" ").startswith("#")==False} # parse env
                 case "json":
                     config=json.loads(config_file.read())                                                                                                                               # parse json
                 case "token" | "txt":
                     config={"content": config_file.read()}                                                                                                                              # parse raw string
                 case _:
                     logger.critical(f"\rLoading \"{config_filepath}\" failed, because file extension is not implemented.")
                     raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because file extension is not implemented.")
     except OSError as e:                                                                                                                                                                # write to log, then forward exception
-        logger.error(f"\rLoading \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
+        logger.warning(f"\rLoading \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}. Source will be skipped.")
         raise
     else:
-        logger.info(f"\rLoaded \"{config_filepath}\".")
+        logger.debug(f"\rLoaded \"{config_filepath}\".")
         logger.debug(config)
     
     return config
 
 
 def _create_default_file(config_filepath: str, config_default: dict[str, typing.Any]) -> None:
     """
```

### Comparing `kfsconfig-2.1.3/pyproject.toml` & `kfsconfig-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "2.1.3"
+version     = "2.1.4"
 
 [tool.poetry.dependencies]
 kfslog = "^2.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
```

### Comparing `kfsconfig-2.1.3/readme.md` & `kfsconfig-2.1.4/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.1.3/PKG-INFO` & `kfsconfig-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.1.3
+Version: 2.1.4
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

