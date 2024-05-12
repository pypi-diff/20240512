# Comparing `tmp/kfsconfig-2.1.4.tar.gz` & `tmp/kfsconfig-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-2.1.4.tar", max compression
+gzip compressed data, was "kfsconfig-2.1.5.tar", max compression
```

## Comparing `kfsconfig-2.1.4.tar` & `kfsconfig-2.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    16273 2024-05-11 22:33:45.399145 kfsconfig-2.1.4/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      514 2024-05-11 22:33:45.399145 kfsconfig-2.1.4/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-11 22:33:45.399145 kfsconfig-2.1.4/readme.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    17000 2024-05-11 23:42:17.260743 kfsconfig-2.1.5/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-11 23:42:17.260743 kfsconfig-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-11 23:42:17.260743 kfsconfig-2.1.5/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.1.5/PKG-INFO
```

### Comparing `kfsconfig-2.1.4/KFSconfig/KFSconfig.py` & `kfsconfig-2.1.5/KFSconfig/KFSconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,19 +162,19 @@
 
     Returns:
     - config_filecontent: content of config file as a dictionary
 
     Raises:
     - FileNotFoundError: config_filepath does not exist
     - IsADirectoryError: config_filepath is a directory
-    - NotImplementedError: file extension is not implemented yet
     - OSError: loading config_filepath failed
     """
 
     config: dict[str, typing.Any]   # config file
+    defaulted: bool=False           # defaulted to forwarding raw string content?
 
 
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
@@ -193,21 +193,24 @@
                 case "env":
                     config={line.strip(" ").split("=")[0]: line.strip(" ").split("=")[1] for line in config_file.readlines() if "=" in line and line.strip(" ").startswith("#")==False} # parse env
                 case "json":
                     config=json.loads(config_file.read())                                                                                                                               # parse json
                 case "token" | "txt":
                     config={"content": config_file.read()}                                                                                                                              # parse raw string
                 case _:
-                    logger.critical(f"\rLoading \"{config_filepath}\" failed, because file extension is not implemented.")
-                    raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Loading \"{config_filepath}\" failed, because file extension is not implemented.")
+                    defaulted=True                                                                                                                                                      # defaulted to forwarding raw string content
+                    config={"content": config_file.read()}                                                                                                                              # parse raw string
     except OSError as e:                                                                                                                                                                # write to log, then forward exception
         logger.warning(f"\rLoading \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}. Source will be skipped.")
         raise
     else:
-        logger.debug(f"\rLoaded \"{config_filepath}\".")
+        if defaulted==False:
+            logger.debug(f"\rLoaded \"{config_filepath}\".")
+        else:                   # if defaulted to forwarding raw string content: warn
+            logger.warning(f"\rLoaded \"{config_filepath}\", but custom behaviour for file extension \"{os.path.basename(config_filepath).rsplit(".", 1)[-1]}\" is not implemented. Defaulted to forwarding content unchanged into key \"content\".")
         logger.debug(config)
     
     return config
 
 
 def _create_default_file(config_filepath: str, config_default: dict[str, typing.Any]) -> None:
     """
@@ -216,18 +219,20 @@
     Arguments:
     - config_default: defaults to use for creation of a default config file, unformatted file formats like .txt require key "content"
     - config_filepath: filepath to config file, formats depending on file extension, unformatted formats like .txt save raw string value from key "content" in file
 
     Raises:
     - FileExistsError: config_filepath already exists
     - KeyError: config_default is missing key "content" while trying to save raw string content
-    - NotImplementedError: file extension is not implemented yet
     - OSError: creating config_filepath failed
     """
 
+    defaulted: bool=False   # defaulted to forwarding raw string content?
+
+
     if 1<=len(logging.getLogger("").handlers):  # if root logger defined handlers:
         logger=logging.getLogger("")            # also use root logger to match formats defined outside KFS
     else:                                       # if no root logger defined:
         logger=KFSlog.setup_logging("KFS")      # use KFS default format
 
     if os.path.exists(config_filepath)==True:   # if config filepath already exists: error
         logger.error(f"Creating \"{config_filepath}\" is not possible, because it already exists.")
@@ -243,19 +248,22 @@
                 case "env":
                     config_file.write("\n".join([f"{k}={v}" for k, v in config_default.items()]))
                 case "json":
                     config_file.write(json.dumps(config_default, indent=4))
                 case "token" | "txt":
                     config_file.write(config_default["content"])
                 case _:
-                    logger.critical(f"\rCreating default \"{config_filepath}\" failed, because file extension is not implemented.")
-                    raise NotImplementedError(f"Error in {load_config.__name__}{inspect.signature(load_config)}: Creating default \"{config_filepath}\" failed, because file extension is not implemented.")
+                    defaulted=True                                          # defaulted to forwarding raw string content
+                    config_file.write(config_default["content"])
     except KeyError:
         logger.error(f"\rCreating default \"{config_filepath}\" failed, because config_default is missing key \"content\".")
         raise
     except OSError as e:
         logger.error(f"\rCreating default \"{config_filepath}\" failed with {KFSfstr.full_class_name(e)}.")
         raise
     else:
-        logger.info(f"\rCreated default \"{config_filepath}\".")
+        if defaulted==False:
+            logger.info(f"\rCreated default \"{config_filepath}\".")
+        else:                   # if defaulted to forwarding raw string content: warn
+            logger.warning(f"Created default \"{config_filepath}\", but custom behaviour for file extension \"{os.path.basename(config_filepath).rsplit(".", 1)[-1]}\" is not implemented. Defaulted to forwarding content unchanged from key \"content\".")
 
     return
```

### Comparing `kfsconfig-2.1.4/pyproject.toml` & `kfsconfig-2.1.5/pyproject.toml`

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
-version     = "2.1.4"
+version     = "2.1.5"
 
 [tool.poetry.dependencies]
 kfslog = "^2.0.0"
 python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.0.0"
```

### Comparing `kfsconfig-2.1.4/readme.md` & `kfsconfig-2.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-2.1.4/PKG-INFO` & `kfsconfig-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 2.1.4
+Version: 2.1.5
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
 Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

