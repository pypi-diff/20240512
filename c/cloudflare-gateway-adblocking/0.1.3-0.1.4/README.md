# Comparing `tmp/cloudflare_gateway_adblocking-0.1.3.tar.gz` & `tmp/cloudflare_gateway_adblocking-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_gateway_adblocking-0.1.3.tar", max compression
+gzip compressed data, was "cloudflare_gateway_adblocking-0.1.4.tar", max compression
```

## Comparing `cloudflare_gateway_adblocking-0.1.3.tar` & `cloudflare_gateway_adblocking-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/LICENSE
--rw-r--r--   0        0        0     2802 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/README.md
--rw-r--r--   0        0        0      784 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/src/__init__.py
--rw-r--r--   0        0        0     5145 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/src/__main__.py
--rw-r--r--   0        0        0        0 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/src/utils/__init__.py
--rw-r--r--   0        0        0     2126 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/src/utils/delete.py
--rw-r--r--   0        0        0     4154 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/src/utils/upload.py
--rw-r--r--   0        0        0     3755 2023-08-19 19:51:11.667288 cloudflare_gateway_adblocking-0.1.3/src/utils/utils.py
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 cloudflare_gateway_adblocking-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2961 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/README.md
+-rw-r--r--   0        0        0      789 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/src/__init__.py
+-rw-r--r--   0        0        0     5145 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/src/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/src/utils/__init__.py
+-rw-r--r--   0        0        0     2126 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/src/utils/delete.py
+-rw-r--r--   0        0        0     4154 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/src/utils/upload.py
+-rw-r--r--   0        0        0     3755 2024-05-12 21:21:25.094047 cloudflare_gateway_adblocking-0.1.4/src/utils/utils.py
+-rw-r--r--   0        0        0     3886 1970-01-01 00:00:00.000000 cloudflare_gateway_adblocking-0.1.4/PKG-INFO
```

### Comparing `cloudflare_gateway_adblocking-0.1.3/LICENSE` & `cloudflare_gateway_adblocking-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_gateway_adblocking-0.1.3/README.md` & `cloudflare_gateway_adblocking-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 These can either be set in the environment or in a `.env` file in the current working directory.  
 #### Command line flags  
 The following command line flags can be used to set the Cloudflare credentials:
 * Cloudflare Account ID: `--account-id` / `-a`  
 * Cloudflare Token: `--token` / `-t`  
 #### Passing blocklists  
 Blocklists can be passed to the program via the command line flag `--blocklist` / `-b`. This flag can either point to a hosts file or a directory containing hosts files. If this flag is not passed, the program will look for a file or directory named `blocklists` in the current working directory.  
-# Passing whitelists  
+#### Passing whitelists  
 Whitelists can be passed to the program via the command line flag `--whitelist` / `-w`. This flag can either point to a hosts file or a directory containing hosts files. If this flag is not passed, then if a file or directory named `whitelists` exists in the current working directory, it will be used. Domains in this whitelist will be excluded from the blocklists.  
 #### Uploading blocklists and creating a firewall policy
 To upload the blocklists to Cloudflare and create a firewall policy, use the `upload` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking upload`  
 #### Deleting blocklists and firewall policy  
 To delete the blocklists from Cloudflare and delete the firewall policy, use the `delete` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking delete`  
 ### Help  
-For help, use the `--help` flag.  
+For help, use the `--help` flag.  
+### Contributing  
+* [Sponsoring](https://github.com/sponsors/slashtechno) via GitHub
+* Contributing code via a pull request
+* Reporting encoutered issues
```

### Comparing `cloudflare_gateway_adblocking-0.1.3/pyproject.toml` & `cloudflare_gateway_adblocking-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloudflare-gateway-adblocking"
-version = "0.1.3"
+version = "0.1.4"
 description = "Serverless adblocking via Cloudflare Zero Trust Gateway"
 authors = ["slastechno <77907286+slashtechno@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/slashtechno/cloudflare-gateway-adblocking"
 keywords = ["cloudflare", "dns", "adblocking", "serverless"]
 
@@ -19,12 +19,12 @@
 loguru = "^0.7.0"
 python-dotenv = "^1.0.0"
 httpx = "^0.24.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.281"
-black = "^23.7.0"
+black = ">=23.7,<25.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cloudflare_gateway_adblocking-0.1.3/src/__main__.py` & `cloudflare_gateway_adblocking-0.1.4/src/__main__.py`

 * *Files identical despite different names*

### Comparing `cloudflare_gateway_adblocking-0.1.3/src/utils/delete.py` & `cloudflare_gateway_adblocking-0.1.4/src/utils/delete.py`

 * *Files identical despite different names*

### Comparing `cloudflare_gateway_adblocking-0.1.3/src/utils/upload.py` & `cloudflare_gateway_adblocking-0.1.4/src/utils/upload.py`

 * *Files identical despite different names*

### Comparing `cloudflare_gateway_adblocking-0.1.3/src/utils/utils.py` & `cloudflare_gateway_adblocking-0.1.4/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflare_gateway_adblocking-0.1.3/PKG-INFO` & `cloudflare_gateway_adblocking-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cloudflare-gateway-adblocking
-Version: 0.1.3
+Version: 0.1.4
 Summary: Serverless adblocking via Cloudflare Zero Trust Gateway
 Home-page: https://github.com/slashtechno/cloudflare-gateway-adblocking
 License: MIT
 Keywords: cloudflare,dns,adblocking,serverless
 Author: slastechno
 Author-email: 77907286+slashtechno@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/slashtechno/cloudflare-gateway-adblocking
 Description-Content-Type: text/markdown
 
@@ -52,19 +53,24 @@
 These can either be set in the environment or in a `.env` file in the current working directory.  
 #### Command line flags  
 The following command line flags can be used to set the Cloudflare credentials:
 * Cloudflare Account ID: `--account-id` / `-a`  
 * Cloudflare Token: `--token` / `-t`  
 #### Passing blocklists  
 Blocklists can be passed to the program via the command line flag `--blocklist` / `-b`. This flag can either point to a hosts file or a directory containing hosts files. If this flag is not passed, the program will look for a file or directory named `blocklists` in the current working directory.  
-# Passing whitelists  
+#### Passing whitelists  
 Whitelists can be passed to the program via the command line flag `--whitelist` / `-w`. This flag can either point to a hosts file or a directory containing hosts files. If this flag is not passed, then if a file or directory named `whitelists` exists in the current working directory, it will be used. Domains in this whitelist will be excluded from the blocklists.  
 #### Uploading blocklists and creating a firewall policy
 To upload the blocklists to Cloudflare and create a firewall policy, use the `upload` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking upload`  
 #### Deleting blocklists and firewall policy  
 To delete the blocklists from Cloudflare and delete the firewall policy, use the `delete` subcommand.  
 For example:  
 `cloudflare-gateway-adblocking delete`  
 ### Help  
 For help, use the `--help` flag.  
+### Contributing  
+* [Sponsoring](https://github.com/sponsors/slashtechno) via GitHub
+* Contributing code via a pull request
+* Reporting encoutered issues
+
```

