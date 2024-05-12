# Comparing `tmp/DNSBruter-1.0.3.tar.gz` & `tmp/DNSBruter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DNSBruter-1.0.3.tar", last modified: Thu Feb  8 11:21:03 2024, max compression
+gzip compressed data, was "DNSBruter-1.0.4.tar", last modified: Sun May 12 15:35:24 2024, max compression
```

## Comparing `DNSBruter-1.0.3.tar` & `DNSBruter-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/DNSBruter.egg-info/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      169 2024-02-08 11:21:03.000000 DNSBruter-1.0.3/DNSBruter.egg-info/PKG-INFO
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      810 2024-02-08 11:21:03.000000 DNSBruter-1.0.3/DNSBruter.egg-info/SOURCES.txt
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        1 2024-02-08 11:21:03.000000 DNSBruter-1.0.3/DNSBruter.egg-info/dependency_links.txt
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)       55 2024-02-08 11:21:03.000000 DNSBruter-1.0.3/DNSBruter.egg-info/entry_points.txt
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      146 2024-02-08 11:21:03.000000 DNSBruter-1.0.3/DNSBruter.egg-info/requires.txt
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)       10 2024-02-08 11:21:03.000000 DNSBruter-1.0.3/DNSBruter.egg-info/top_level.txt
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      169 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/PKG-INFO
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 12:34:17.000000 DNSBruter-1.0.3/dnsbruter/__init__.py
--rwxr-xr-x   0 sanjai    (1000) sanjai    (1000)      122 2024-02-08 10:44:19.000000 DNSBruter-1.0.3/dnsbruter/dnsbruter.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 12:34:26.000000 DNSBruter-1.0.3/dnsbruter/modules/__init__.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/banner/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 12:41:40.000000 DNSBruter-1.0.3/dnsbruter/modules/banner/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      834 2024-02-07 12:39:17.000000 DNSBruter-1.0.3/dnsbruter/modules/banner/banner.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/cli/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 12:41:49.000000 DNSBruter-1.0.3/dnsbruter/modules/cli/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)     2142 2024-02-08 10:14:03.000000 DNSBruter-1.0.3/dnsbruter/modules/cli/cli.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/core/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 13:14:58.000000 DNSBruter-1.0.3/dnsbruter/modules/core/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)     4235 2024-02-08 10:36:01.000000 DNSBruter-1.0.3/dnsbruter/modules/core/core.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/extender/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 10:36:25.000000 DNSBruter-1.0.3/dnsbruter/modules/extender/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      812 2024-02-07 13:17:56.000000 DNSBruter-1.0.3/dnsbruter/modules/extender/extender.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)     3226 2024-02-08 11:13:56.000000 DNSBruter-1.0.3/dnsbruter/modules/handler.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/help/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 12:48:01.000000 DNSBruter-1.0.3/dnsbruter/modules/help/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)     2165 2024-02-08 10:37:25.000000 DNSBruter-1.0.3/dnsbruter/modules/help/help.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/version/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 12:53:09.000000 DNSBruter-1.0.3/dnsbruter/modules/version/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)     1838 2024-02-07 13:14:39.000000 DNSBruter-1.0.3/dnsbruter/modules/version/version.py
-drwxr-xr-x   0 sanjai    (1000) sanjai    (1000)        0 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/dnsbruter/modules/wordlist/
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)        0 2024-02-07 13:12:44.000000 DNSBruter-1.0.3/dnsbruter/modules/wordlist/__init__.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      939 2024-02-07 13:14:12.000000 DNSBruter-1.0.3/dnsbruter/modules/wordlist/wordlist.py
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)       38 2024-02-08 11:21:03.709138 DNSBruter-1.0.3/setup.cfg
--rw-r--r--   0 sanjai    (1000) sanjai    (1000)      659 2024-02-08 11:20:13.000000 DNSBruter-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/DNSBruter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-12 15:35:24.000000 DNSBruter-1.0.4/DNSBruter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-12 15:35:24.000000 DNSBruter-1.0.4/DNSBruter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:35:24.000000 DNSBruter-1.0.4/DNSBruter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-12 15:35:24.000000 DNSBruter-1.0.4/DNSBruter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-12 15:35:24.000000 DNSBruter-1.0.4/DNSBruter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 15:35:24.000000 DNSBruter-1.0.4/DNSBruter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/dnsbruter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/modules/banner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/banner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/banner/banner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/modules/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/modules/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/modules/core/wildcard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/core/wildcard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/core/wildcard/wildcard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.244815 DNSBruter-1.0.4/dnsbruter/modules/extender/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/extender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/extender/extender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/dnsbruter/modules/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/dnsbruter/modules/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/verify/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/dnsbruter/modules/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/dnsbruter/modules/wordlist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/wordlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/dnsbruter/modules/wordlist/wordlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:35:24.248815 DNSBruter-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-12 15:35:09.000000 DNSBruter-1.0.4/setup.py
```

### Comparing `DNSBruter-1.0.3/dnsbruter/modules/banner/banner.py` & `DNSBruter-1.0.4/dnsbruter/modules/banner/banner.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,21 +29,17 @@
 colors = [ green, cyan, blue, white, magenta]
 
 random_color = random.choice(colors)
 
 
 def banner():
     
-    tool_name = "DnsBruter"
+    tool_name = "dnsbruter"
     
     fonts = ["big", "ogre", "shadow", "script", "colossal" , "smslant", "graffiti", "slant"]
     selected_font = random.choice(fonts)
     banner = text2art(f"{tool_name}", font=selected_font)
     
     banner = f"""{bold}{random_color}{banner}{reset}
-    
-                     {bold}{white}Author : D.SanjaiKumar @CyberRevoltSecurities{reset}\n"""
-
-   
-
+                    {bold}{white}@RevoltSecurities{reset}\n"""
     return banner
```

### Comparing `DNSBruter-1.0.3/dnsbruter/modules/cli/cli.py` & `DNSBruter-1.0.4/dnsbruter/modules/cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,87 +1,63 @@
 #!/usr/bin/env python3
 from colorama import Fore,Back,Style
 import argparse
 import time as t
 import random
 
-
 red =  Fore.RED
-
 green = Fore.GREEN
-
 magenta = Fore.MAGENTA
-
 cyan = Fore.CYAN
-
 mixed = Fore.RED + Fore.BLUE
-
 blue = Fore.BLUE
-
 yellow = Fore.YELLOW
-
 white = Fore.WHITE
-
 reset = Style.RESET_ALL
-
 bold = Style.BRIGHT
-
 colors = [ green, cyan, blue]
-
 random_color = random.choice(colors)
 
-
 def cli():
     
     try:
         
         parser =  argparse.ArgumentParser(add_help=False,usage=argparse.SUPPRESS,exit_on_error=False )
-        
         parser.add_argument("-h", "--help", action="store_true")
-        
         parser.add_argument("-d", "--domain", type=str)
-        
+        parser.add_argument("-ip", "--ipaddress", action="store_true")
         parser.add_argument("-w", "--wordlist", type=str)
-        
         parser.add_argument("-c", "--concurrency", type=int, default=100)
-        
-        parser.add_argument("-rt", "--rate-limit", type=float, default=0)
-                         
         parser.add_argument("-up", "--update", action="store_true")
-        
         parser.add_argument("-vr", "--version", action="store_true")
-        
         parser.add_argument("-v", "--verbose", action="store_true")
-        
         parser.add_argument("-s", "--silent", action="store_true")
-        
         parser.add_argument("-nc", "--no-color",action="store_true")
-        
         parser.add_argument("-o", "--output", type=str)
-        
+        parser.add_argument("-duc", "--disable-check", action="store_true")
+        parser.add_argument("-rl", "--resolver", type=str)
+        parser.add_argument("-wd", "--wildcard-detect", action="store_true")
+        parser.add_argument("-wt", "--wildcard-threads", type=int, default=20)
+        parser.add_argument("-ov", "--override", action="store_true")
+        parser.add_argument("-ws", "--wildcard-output", type=str)
+        parser.add_argument("-sd", "--sec-deb", action="store_true")
         global args 
-                
         return parser.parse_args()
-        
-    
     except argparse.ArgumentError as e:
         
-        print(f"[{bold}{blue}INFO{reset}]: {bold}{white}Please use the command for more infromation:{reset} {bold}{blue}Dnsbruter -h {e}{reset}")
-        
+        print(f"[{bold}{blue}INFO{reset}]: {bold}{white}Please use the command for more infromation:{reset} {bold}{blue}dnsbruter -h {e}{reset}")
         quit()
         
     except argparse.ArgumentTypeError as e:
         
-        print(f"[{bold}{blue}INFO{reset}]: {bold}{white}Please use the command for more infromation:{reset} {bold}{blue}Dnsbruter -h {e}{reset}")
-        
+        print(f"[{bold}{blue}INFO{reset}]: {bold}{white}Please use the command for more infromation:{reset} {bold}{blue}dnsbruter -h {e}{reset}")
         quit()
         
-        
-    except Exception as e:
-        
-        pass
-    
     except KeyboardInterrupt as e:
         
         print(f"\n[{bold}{blue}INFO{reset}]: {bold}{white}Dnsbruter exits..{reset}")
+        quit()
         
-        quit()
+    except Exception as e:
+        pass
+    
+
```

### Comparing `DNSBruter-1.0.3/dnsbruter/modules/extender/extender.py` & `DNSBruter-1.0.4/dnsbruter/modules/extender/extender.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 import platform
-import os 
 import resource
 from colorama import Fore,Back,Style
 
 
 red =  Fore.RED
-
 green = Fore.GREEN
-
 magenta = Fore.MAGENTA
-
 cyan = Fore.CYAN
-
 mixed = Fore.RED + Fore.BLUE
-
 blue = Fore.BLUE
-
 yellow = Fore.YELLOW
-
 white = Fore.WHITE
-
 reset = Style.RESET_ALL
-
 bold = Style.BRIGHT
-
 colors = [ green, cyan, blue]
 
 
 
 def extender():  
     try:
-        
         soft , hard = resource.getrlimit(resource.RLIMIT_NOFILE)
-        
         new = 100000
-        
         osname = platform.system()
-        
         if osname == "Linux" or  osname == "Darwin":
             
-            
-            
             resource.setrlimit(resource.RLIMIT_NOFILE, (new, hard))
             
     except KeyboardInterrupt as e:
-        
         quit()
         
     except Exception as e:
-        
         pass
```

### Comparing `DNSBruter-1.0.3/dnsbruter/modules/version/version.py` & `DNSBruter-1.0.4/dnsbruter/modules/version/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,62 +36,42 @@
 def check_version():
     
     
     url = f"https://api.github.com/repos/sanjai-AK47/Dnsbruter/releases/latest"
     
     try:
         
-        
         response = requests.get(url, verify=True, timeout=10)
-        
         if response.status_code == 200:
-            
             data = response.json()
-            
             latest = data.get('tag_name')
-            
             return latest
-                 
-            
-        
+
     except KeyboardInterrupt as e:
         
         print(f"[{bold}{blue}INFO{reset}]: {bold}{white}Dnsbruter exits..{reset}")
-        
-        quit()
-        
-                
+        quit()       
     except Exception as e:
         
         pass
     
 
     
 def update_version():
     
-    url = f"https://api.github.com/repos/sanjai-AK47/Dnsbruter/releases/latest"
+    url = f"https://api.github.com/repos/RevoltSecurities/Dnsbruter/releases/latest"
     
     try:
-        
-        
         response = requests.get(url, verify=True, timeout=10)
-        
         if response.status_code == 200:
-            
             data = response.json()
-            
             latest = data.get('tarball_url')
-            
             return latest
-        
-        
-        
+
     except KeyboardInterrupt as e:
         
         print(f"[{bold}{blue}INFO{reset}]: {bold}{white}Dnsbruter exits..{reset}")
-        
         quit()
         
-                
     except Exception as e:
         
         pass
```

### Comparing `DNSBruter-1.0.3/dnsbruter/modules/wordlist/wordlist.py` & `DNSBruter-1.0.4/dnsbruter/modules/wordlist/wordlist.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,38 @@
 import os 
 from colorama import Fore,Back,Style
 import random 
 
 red =  Fore.RED
-
 green = Fore.GREEN
-
 magenta = Fore.MAGENTA
-
 cyan = Fore.CYAN
-
 mixed = Fore.RED + Fore.BLUE
-
 blue = Fore.BLUE
-
 yellow = Fore.YELLOW
-
 white = Fore.WHITE
-
 reset = Style.RESET_ALL
-
 bold = Style.BRIGHT
-
 colors = [ green, cyan, blue]
-
 random_color = random.choice(colors)
 
 
 def wordlist(filename):
     
     try:
-        
         with open(filename, "r") as data :
-            
             datas = data.read().splitlines()
-            
         return datas 
     
     except FileNotFoundError as e:
         
         print(f"[{bold}{red}INFO{reset}]: {bold}{white}Pleach check the wordlist file {filename} exists..{reset}")
-        
         quit()
         
     except KeyboardInterrupt as e:
         
         print(f"\n[{bold}{blue}INFO{reset}]: {bold}{white}Dnsbruter exits..{reset}")
-        
         quit()
         
     except Exception as e:
         
         pass
```

