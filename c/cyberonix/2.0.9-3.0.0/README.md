# Comparing `tmp/cyberonix-2.0.9.tar.gz` & `tmp/cyberonix-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberonix-2.0.9.tar", last modified: Thu Mar  9 16:27:11 2023, max compression
+gzip compressed data, was "cyberonix-3.0.0.tar", last modified: Sun May 12 17:29:52 2024, max compression
```

## Comparing `cyberonix-2.0.9.tar` & `cyberonix-3.0.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.798401 cyberonix-2.0.9/
--rw-r--r--   0 root         (0) root         (0)    16291 2023-03-09 16:27:11.798401 cyberonix-2.0.9/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    15521 2023-03-08 18:30:52.000000 cyberonix-2.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.790401 cyberonix-2.0.9/cyberonix/
--rwxr-xr-x   0 root         (0) root         (0)       44 2023-02-28 17:25:39.000000 cyberonix-2.0.9/cyberonix/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10466 2023-03-08 18:16:23.000000 cyberonix-2.0.9/cyberonix/cyberonix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.794401 cyberonix-2.0.9/cyberonix/main/
--rw-r--r--   0 root         (0) root         (0)     3354 2023-03-09 15:11:27.000000 cyberonix-2.0.9/cyberonix/main/Cheat_sheet.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18118 2023-03-08 16:36:27.000000 cyberonix-2.0.9/cyberonix/main/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-03-08 14:09:58.000000 cyberonix-2.0.9/cyberonix/main/news.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-03-08 14:08:38.000000 cyberonix-2.0.9/cyberonix/main/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.798401 cyberonix-2.0.9/cyberonix/main/tools/
--rw-r--r--   0 root         (0) root         (0)     7895 2023-03-07 18:37:06.000000 cyberonix-2.0.9/cyberonix/main/tools/Authentication.py
--rw-r--r--   0 root         (0) root         (0)    22162 2023-03-09 15:37:30.000000 cyberonix-2.0.9/cyberonix/main/tools/Authorization.py
--rw-r--r--   0 root         (0) root         (0)    20825 2023-03-09 15:38:06.000000 cyberonix-2.0.9/cyberonix/main/tools/Configuration_Management.py
--rw-r--r--   0 root         (0) root         (0)     8774 2023-03-06 20:27:23.000000 cyberonix-2.0.9/cyberonix/main/tools/Cryptography.py
--rw-r--r--   0 root         (0) root         (0)    10616 2023-03-07 18:38:18.000000 cyberonix-2.0.9/cyberonix/main/tools/Exploitation_Tools.py
--rw-r--r--   0 root         (0) root         (0)     5421 2023-03-07 18:38:29.000000 cyberonix-2.0.9/cyberonix/main/tools/File_Upload.py
--rw-r--r--   0 root         (0) root         (0)    30502 2023-03-09 16:12:02.000000 cyberonix-2.0.9/cyberonix/main/tools/Password_Hacking.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-03-07 18:39:05.000000 cyberonix-2.0.9/cyberonix/main/tools/Pentesting_Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)    21205 2023-03-07 18:31:17.000000 cyberonix-2.0.9/cyberonix/main/tools/PostExploitationAttacks.py
--rw-r--r--   0 root         (0) root         (0)    16842 2023-03-07 18:39:27.000000 cyberonix-2.0.9/cyberonix/main/tools/RiskyFuncPayment.py
--rw-r--r--   0 root         (0) root         (0)     5236 2023-03-07 18:39:39.000000 cyberonix-2.0.9/cyberonix/main/tools/Secure_Transmission.py
--rw-r--r--   0 root         (0) root         (0)    18659 2023-03-07 18:39:51.000000 cyberonix-2.0.9/cyberonix/main/tools/Session_Management.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-03-07 18:40:00.000000 cyberonix-2.0.9/cyberonix/main/tools/Sniffing_and_Spoofing.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-03-09 16:21:18.000000 cyberonix-2.0.9/cyberonix/main/tools/Vulnerability_Analysis.py
--rw-r--r--   0 root         (0) root         (0)    12318 2023-03-09 16:21:10.000000 cyberonix-2.0.9/cyberonix/main/tools/WEB_Application_Analysis.py
--rw-r--r--   0 root         (0) root         (0)     6003 2023-03-07 19:21:36.000000 cyberonix-2.0.9/cyberonix/main/tools/Wireless_Hacking.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/banner.py
--rw-r--r--   0 root         (0) root         (0)      207 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/colors.py
--rw-r--r--   0 root         (0) root         (0)    31538 2023-03-09 15:47:26.000000 cyberonix-2.0.9/cyberonix/main/tools/data_validation.py
--rw-r--r--   0 root         (0) root         (0)     5628 2023-03-07 18:38:08.000000 cyberonix-2.0.9/cyberonix/main/tools/dos.py
--rw-r--r--   0 root         (0) root         (0)     5273 2023-03-07 19:22:11.000000 cyberonix-2.0.9/cyberonix/main/tools/html5.py
--rw-r--r--   0 root         (0) root         (0)    10451 2023-03-09 15:51:45.000000 cyberonix-2.0.9/cyberonix/main/tools/information_gathering.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/run_on_browser.py
--rw-r--r--   0 root         (0) root         (0)    13411 2023-03-09 15:33:04.000000 cyberonix-2.0.9/cyberonix/main/tools/template.py
--rw-r--r--   0 root         (0) root         (0)       78 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/waiting.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-03-06 21:27:44.000000 cyberonix-2.0.9/cyberonix/main/tools/writeup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.790401 cyberonix-2.0.9/cyberonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16291 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 16:27:11.798401 cyberonix-2.0.9/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1274 2023-03-09 16:22:59.000000 cyberonix-2.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.037871 cyberonix-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:29:52.033871 cyberonix-3.0.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:51.993871 cyberonix-3.0.0/cyberonix/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.0/cyberonix/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13327 2024-05-12 17:28:26.000000 cyberonix-3.0.0/cyberonix/cyberonix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.005871 cyberonix-3.0.0/cyberonix/main/
+-rw-r--r--   0 root         (0) root         (0)    21630 2024-05-12 16:50:20.000000 cyberonix-3.0.0/cyberonix/main/Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31929 2024-05-12 16:49:42.000000 cyberonix-3.0.0/cyberonix/main/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-05-12 16:50:50.000000 cyberonix-3.0.0/cyberonix/main/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.033871 cyberonix-3.0.0/cyberonix/main/tools/
+-rw-r--r--   0 root         (0) root         (0)     3876 2024-05-12 16:51:19.000000 cyberonix-3.0.0/cyberonix/main/tools/Anonymity.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-05-12 16:51:44.000000 cyberonix-3.0.0/cyberonix/main/tools/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-12 16:52:23.000000 cyberonix-3.0.0/cyberonix/main/tools/Authorization.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2024-05-12 16:52:53.000000 cyberonix-3.0.0/cyberonix/main/tools/Configuration_Management.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-12 16:53:28.000000 cyberonix-3.0.0/cyberonix/main/tools/Cryptography.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2024-05-12 16:54:13.000000 cyberonix-3.0.0/cyberonix/main/tools/Exploitation_Tools.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-12 16:54:24.000000 cyberonix-3.0.0/cyberonix/main/tools/File_Upload.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-12 16:54:45.000000 cyberonix-3.0.0/cyberonix/main/tools/Framework.py
+-rw-r--r--   0 root         (0) root         (0)    28866 2024-05-12 16:55:48.000000 cyberonix-3.0.0/cyberonix/main/tools/Password_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)     4871 2024-05-12 16:56:00.000000 cyberonix-3.0.0/cyberonix/main/tools/Pentesting_Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2024-05-12 16:56:09.000000 cyberonix-3.0.0/cyberonix/main/tools/PostExploitationAttacks.py
+-rw-------   0 root         (0) root         (0)   169451 2024-05-12 16:56:29.000000 cyberonix-3.0.0/cyberonix/main/tools/Recommended_Tool.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-12 16:56:38.000000 cyberonix-3.0.0/cyberonix/main/tools/RiskyFuncPayment.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2024-05-12 16:56:52.000000 cyberonix-3.0.0/cyberonix/main/tools/Secure_Transmission.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2024-05-12 16:58:23.000000 cyberonix-3.0.0/cyberonix/main/tools/Session_Management.py
+-rw-r--r--   0 root         (0) root         (0)    10604 2024-05-12 16:58:33.000000 cyberonix-3.0.0/cyberonix/main/tools/Sniffing_and_Spoofing.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-05-12 16:58:54.000000 cyberonix-3.0.0/cyberonix/main/tools/Vulnerability_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)    13388 2024-05-12 16:59:05.000000 cyberonix-3.0.0/cyberonix/main/tools/WEB_Application_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-12 16:59:16.000000 cyberonix-3.0.0/cyberonix/main/tools/Wireless_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-12 17:00:57.000000 cyberonix-3.0.0/cyberonix/main/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-12 16:52:40.000000 cyberonix-3.0.0/cyberonix/main/tools/banner.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/tools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    27128 2024-05-12 16:53:49.000000 cyberonix-3.0.0/cyberonix/main/tools/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-05-12 16:53:59.000000 cyberonix-3.0.0/cyberonix/main/tools/dos.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-05-12 16:54:31.000000 cyberonix-3.0.0/cyberonix/main/tools/forensic.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-05-12 16:55:06.000000 cyberonix-3.0.0/cyberonix/main/tools/html5.py
+-rw-r--r--   0 root         (0) root         (0)    18178 2024-05-12 16:55:28.000000 cyberonix-3.0.0/cyberonix/main/tools/information_gathering.py
+-rw-r--r--   0 root         (0) root         (0)      654 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/tools/run_on_browser.py
+-rw-r--r--   0 root         (0) root         (0)    16803 2024-05-12 16:58:45.000000 cyberonix-3.0.0/cyberonix/main/tools/template.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-03-14 18:35:27.000000 cyberonix-3.0.0/cyberonix/main/tools/waiting.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-12 16:59:26.000000 cyberonix-3.0.0/cyberonix/main/tools/writeup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 17:29:52.001871 cyberonix-3.0.0/cyberonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23928 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-12 17:29:51.000000 cyberonix-3.0.0/cyberonix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 17:29:52.037871 cyberonix-3.0.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1337 2024-05-12 17:27:02.000000 cyberonix-3.0.0/setup.py
```

### Comparing `cyberonix-2.0.9/cyberonix/cyberonix.py` & `cyberonix-3.0.0/cyberonix/cyberonix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,164 +1,173 @@
 #!/usr/bin/python3
 import os
 import subprocess
-from cyberonix.main import *
-from cyberonix.main.tools import colors, banner
-import time, argparse
-
+from main.tools import banner,colors,template,Recommended_Tool,run_on_browser
+from main import * 
+import time,argparse
 
 def exit_program():
     os.system("clear")
     banner.main()
-    print("\033[38;5;105m", "[+] Thanks visit again".title())
+    print("\033[38;5;105m","[+] Thanks visit again".title())
     exit()
 
-
 try:
-
     def starting():
         parser = argparse.ArgumentParser(
             description="Cyberonix is a complete resource hub for Cyber Security Community. Our aim is to make this tool an 1 stop solution for all the Hackers out there to get resources of various topics in Cyber Security. We will keep updating this tool & adding new & updated resources on the go.",
         )
         main_args = parser.add_argument_group('Main Arguments')
             
         main_args.add_argument(
-            "--tools", "-t", action="store_true", help="Run Tools Function"
-        )
-        main_args.add_argument(
-            "--cheatsheet", "-c", action="store_true", help="Run Cheatsheet Function"
+            "--tools", "-t",type=str,help=": Access various cybersecurity tools."
         )
         main_args.add_argument(
-            "--news",
-            "-n",
-            nargs="?",
-            metavar="Date",
-            const="latest",
-            type=str,
-            help="Date In The Format yyyy-mm-dd",
+
+            "--cheatsheet", "-c", action="store_true", help=": Get a cybersecurity reference guide."
+
         )
         ip_args = parser.add_argument_group('IP')
         ip_args.add_argument(
-            "--getip", "-gip", help="Get Ip Of A Domain", metavar="Domain"
+            "--getip", "-gip", action="store_true",help=": Get Ip Of A Domain. \nCan use with: --domain, --file, --output",
         )
-        ip_args.add_argument("--ipinfo", "-ipi", metavar="IP", help="Get IP Infomation")
-                      
+                              
         dns_Args = parser.add_argument_group('DNS Records')
-        parser.add_argument("--domain", "-D", dest='domain',
-                    help='Specify the domain', option_strings=['--domain'])
+        parser.add_argument("--domain", "-D", dest='domain', nargs="?" , const="" ,help=': Specify the domain', option_strings=['--domain'])
         dns_Args.add_argument(
-            "--dnsrecord", "-dns", action="store_true", help="To Get DNS Records(options: --domain) and use --record to specify record name"
+            "--dnsrecord", "-dns", action="store_true", help=": To Get DNS Records of a domain. Can use with: --domain, --file, --output "
         )
         dns_Args.add_argument(
-            "--record", "-r", help="To Give Record For DNSrecord(Like: A,TXT,MX)"
+            "--record", "-r", help=": Specify the type of DNS record (e.g., A, TXT, MX). \nusage: --record <type>"
         )
         screenshot_Args = parser.add_argument_group('Screenshoting')
         screenshot_Args.add_argument(
             "--screenshot",
             "-s",
             action="store_true",
-            help="To Get Screenshot Of Websites(options: --file,--domain,--output)",
+            help=": To take a Screenshot Of Website/Websites. \nCan use with: --domain,--file,--output",
         )
-        parser.add_argument("--output", "-o", help="Specify An Output File (-o path/to/location)")
-        parser.add_argument("--file", "-f", help="Specify An Input File (-f path/to/file.txt)")
+        parser.add_argument("--output", "-o", help=": Save the results to the file Specify File location -o path/to/location")
+        parser.add_argument("--file", "-f", help=": Read input from a file Specify An Input File -f path/to/file.txt")
         
         asn_Args = parser.add_argument_group('ASN Record')
         parser.add_argument("--ip", "-ip", help="Specify IP Address")
         asn_Args.add_argument(
-                "--asnrecord", "-asn", action="store_true", help="To Get ASN Record(Options: --ip,--file,--output)"
+                "--asnrecord", "-asn", action="store_true", help=": Get ASN (network) information. \n Can use with:  --ip,--file,--output"
         )
         password_Args = parser.add_argument_group("Password Generation")
         password_Args.add_argument(
-            "--passwordgen", "-P", action="store_true", help="To Generate Password"
+            "--passwordgen", "-P", action="store_true", help=": To Generate a Password"
         )
         password_Args.add_argument(
             "--default-password-gen",
             "-pass",
             action="store_true",
-            help="To Generate Random Password (Recommended)(You can only use --length,--checkpassword)",
+            help=": To Generate Random Password (Recommended)(only use --length, --checkpassword for customization).",
         )
-
+        
         password_Args.add_argument(
-            "--upper", "-u", action="store_true", help="For Uppercase"
+            "--upper", "-u", action="store_true", help=": For Uppercase"
         )
         password_Args.add_argument(
-            "--lower", "-l", action="store_true", help="For Lowercase"
+            "--lower", "-l", action="store_true", help=": For Lowercase"
         )
         password_Args.add_argument(
-            "--digits", "-d", action="store_true", help="For Digits"
+            "--digits", "-d", action="store_true", help=": For Digits"
         )
         password_Args.add_argument(
-            "--punctuation", "-p", action="store_true", help="For Punctuation"
+            "--punctuation", "-p", action="store_true", help=": For Punctuation"
         )
         password_Args.add_argument(
-            "--length", "-L", help="To Specify Length Of Password (Default=8)"
+            "--length", "-L", help=": To Specify Length Of Password (Default=8)"
         )
         password_Args.add_argument(
             "--checkpassword",
             "-C",
             action="store_true",
-            help="To Check Your Generated Password",
+            help=": To Check Your Generated Password",
         )
-        
+        wordlist_Args = parser.add_argument_group("Wordlist Generation")
+        wordlist_Args.add_argument(
+            "--wordlist", "-w", action="store_true", help=": To Generate a Wordlist"
+        )
+        wordlist_Args.add_argument("-ch", "--characters", type=str, default="abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789",
+                   help=": Set of characters to include in the wordlist")
+        wordlist_Args.add_argument("-min", "--min_length", type=int, default=4, help=": Minimum length of the words ( Default = 4 )")
+        wordlist_Args.add_argument("-max", "--max_length", type=int, default=6, help=": Maximum length of the words ( Default = 6 )")
+        wordlist_Args.add_argument("-ot", "--output_file", type=str, default="custom_wordlist.txt", help=": Output file name ( Default = custom_wordlist.txt )")
+
         hstatus_Args = parser.add_argument_group('HTTP Status')
         hstatus_Args.add_argument(
             "--http-status",
             "-S",
             action="store_true",
-            help="To Get Http Status Code Of A Domain(Options: --domain,--file,--output)",
+            help=": Check a website's HTTP status code." "\nCan use with: --domain, --file, --output" ,
         )
         remove_dub_Args = parser.add_argument_group('remove duplicate')
         remove_dub_Args.add_argument(
             "--remove-duplicate",
             "-rd",
             action="store_true",
-            help="To Remove Dublicates From a File(Options: --file,--output)",
+            help=": To Remove Duplicates From a File. Can use with: --file,--output",
         )
         args = parser.parse_args()
-
         if args.tools:
-            tool.main()
+            arguments.tools(args.tools) 
         elif args.getip:
-            arguments.getip(args.getip)
-        elif args.cheatsheet:
-            Cheat_sheet.main()
-        elif args.news:
-            if args.news == "latest" or args.news is None:
-                news.main(args.news)
+            
+            if args.file:
+                if args.output:
+                    arguments.getip(path=args.file, output=args.output)
+                else:
+                    arguments.getip(path=args.file)
+            elif args.domain:
+                if args.output:
+                    arguments.getip(url=args.domain,output=args.output)                    
+                else:
+                    arguments.getip(url=args.domain)
             else:
-                news.main(args.news)
+                if args.output:
+                    arguments.getip(url=args.getip, output=args.output)
+                else:
+                    arguments.getip(url=args.getip)
+                #print(
+                    #f"{colors.red}[!] Please enter file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
+                #)
+
         elif args.cheatsheet:
-            Cheat_sheet.main()
+            run_on_browser.main("https://github.com/defronixpro/Defronix-Cybersecurity-Roadmap/blob/main/cheatsheet.md")
+       
         elif args.screenshot:
             if args.file:
                 if args.output:
                     arguments.screenshot(path=args.file,output=args.output)
                 else:
                     arguments.screenshot(path=args.file)
             elif args.domain:
                 if args.output:
                     arguments.screenshot(url=args.domain,output=args.output)
                 else:
                     arguments.screenshot(url=args.domain)
 
             else:
                 print(
-                    f"{colors.red}[!] Please file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
+                    f"{colors.red}[!] Please enter file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
                 )
         elif args.remove_duplicate:
             if args.file:
                 if args.output:
                     arguments.remove_dublicates(location=args.file, output=args.output)
                 else:
                     arguments.remove_dublicates(location=args.file)
 
             else:
                 print(
-                    f"{colors.red}[!] Please file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
-                )
+                    f"{colors.red}[!] Please enter file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
+)
 
         elif args.asnrecord:
             if args.file:
                 if args.output:
                     arguments.asnrecord(path=args.file, output=args.output)
                 else:
                     arguments.asnrecord(path=args.file)
@@ -166,15 +175,15 @@
                 if args.output:
                     arguments.asnrecord(url=args.ip, output=args.output)
                 else:
                     arguments.asnrecord(url=args.ip)
 
             else:
                 print(
-                    f"{colors.red}[!] Please file with --file path/to/file or pass a single ip with --ip 8.8.8.8{colors.reset}"
+                    f"{colors.red}[!] Please enter file with --file path/to/file or pass a single ip with --ip 8.8.8.8{colors.reset}"
                 )
 
         elif args.http_status:
             if args.file:
                 if args.output:
                     arguments.http_status_code(path=args.file, output=args.output)
                 else:
@@ -182,18 +191,17 @@
             elif args.domain:
                 if args.output:
                     arguments.http_status_code(url=args.domain, output=args.output)
                 else:
                     arguments.http_status_code(url=args.domain)
             else:
                 print(
-                    f"{colors.red}[!] Please file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
+                    f"{colors.red}[!] Please enter file with --file path/to/file or pass a single domain with --domain https://example.com{colors.reset}"
                 )
-        elif args.ipinfo:
-            arguments.ipinformation(args.ipinfo)
+
         elif args.passwordgen:
             if args.length:
                 arguments.password_gen(
                     args.upper,
                     args.lower,
                     args.digits,
                     args.punctuation,
@@ -209,65 +217,93 @@
                     check=args.checkpassword,
                 )
         elif args.default_password_gen:
             if args.length:
                 arguments.password_gen(length=args.length, check=args.checkpassword)
             else:
                 arguments.password_gen(check=args.checkpassword)
+
+        elif args.wordlist:
+            arguments.generate_wordlist(
+                args.characters,
+                args.min_length,
+                args.max_length,
+                args.output_file
+            )
+                
         elif args.dnsrecord:
-            if args.domain:
+            if args.record:
+                if args.file:
+                    if args.output:
+                        arguments.dnsrecords(path=args.file, names=args.record,output=args.output)
+                    else:
+                        arguments.dnsrecords(path=args.file, names=args.record)
+                elif args.domain:
+                    if args.output:
+                        arguments.dnsrecords(url=args.domain, names=args.record,output=args.output)
+                    else:
+                        arguments.dnsrecords(url=args.domain, names=args.record)
+                else:
+                    print("please give --domain/--file also")
+            elif args.domain:
                 if args.record:
-                    arguments.dnsrecords(args.domain, args.record)
+                    if args.output:
+                        arguments.dnsrecords(url=args.domain, names=args.record,output=args.output)
+                    else:
+                        arguments.dnsrecords(url=args.domain, names=args.record)
                 else:
                     print("please give --record also")
-            elif args.record:
-                if args.domain:
-                    arguments.dnsrecords(args.domain, args.record)
-                else:
-                    print("please give --domain also")
         else:
             main()
 
     def main():
+        #update()
         os.system("chmod +x *")
         proc = subprocess.Popen([f"id"], stdout=subprocess.PIPE, shell=True)
-        # there keyfor success output and noththere for error output
+        #there keyfor success output and noththere for error output
         (there, notthere) = proc.communicate()
-        there = there.decode()
+        there=there.decode()
         if "root" not in there:
             try:
-                subprocess.run("sudo cyberonix", shell=True, check=True)
+                subprocess.run('sudo cyberonix',shell=True, check = True)
             except Exception as err:
                 os.system("sudo python3 cyberonix.py")
+            # os.system("sudo cyberonix")
             exit()
         while True:
             os.system("clear")
             banner.main()
-            list_attacks = ["TOOLS", "CHEATSHEET", "NEWS", "exit"]
+            list_attacks=["TOOLS","CHEATSHEET","Bug Bounty","Certifications & Roadmap","Write Ups","Man Page","exit"]
             for i in range(len(list_attacks)):
-                print(colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset)
+                print(colors.options,f"{i+1}) {list_attacks[i]}".title(),colors.reset)
             try:
                 option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
             except KeyboardInterrupt:
                 exit_program()
-            if option == "0":
+            if option=="1":
                 os.system("clear")
                 tool.main()
-            elif option == "1":
+            elif option=="2":
+                run_on_browser.main("https://github.com/defronixpro/Defronix-Cybersecurity-Roadmap/blob/main/cheatsheet.md")
+            elif option == "3":
                 os.system("clear")
-                Cheat_sheet.main()
-            elif option == "2":
+                Bug_Bounty.main()
+            elif option =="4":
+                run_on_browser.main("https://github.com/defronixpro/Defronix-Cybersecurity-Roadmap/blob/main/README.md")
+            elif option == "5":
+                run_on_browser.main("https://github.com/defronixpro/Defronix-Cybersecurity-Roadmap/blob/main/Writeups.md")
+            elif option=="6":
                 os.system("clear")
-                news.main()
+                os.system("man cyberonix")
             else:
                 exit_program()
-
-    # to run file separately
-    if __name__ == "__main__":
+    #to run file separately
+    if __name__ == "__main__": 
         starting()
 except KeyboardInterrupt:
     exit_program()
 except Exception as err:
     os.system("clear")
     banner.main()
     banner.attack(f"{colors.red}ERROR{colors.reset}")
     banner.description(f"{colors.red}{err}{colors.reset}")
+
```

### Comparing `cyberonix-2.0.9/cyberonix/main/arguments.py` & `cyberonix-3.0.0/cyberonix/main/arguments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,400 @@
 import dns.resolver, requests, socket, os, time
 import random
+from cyberonix.main import tool
+from cyberonix.main.tools import *
 from selenium import webdriver
 from ipwhois import IPWhois
-from cyberonix.main.tools import colors, banner
+from cyberonix.main.tools import colors, banner,template,Recommended_Tool
+import argparse, itertools
 
-
-def getip(domain_name):
-    if not getip.called:
-        getip.called=True
-        ip_address = socket.gethostbyname(domain_name)
+def tools(name):
+    try:
+        getattr(information_gathering, name)()
+        getattr(Vulnerability_Analysis, name)()
+        getattr(WEB_Application_Analysis, name)()
+        getattr(Password_Hacking, name)()
+        getattr(Wireless_Hacking, name)()
+        getattr(Exploitation_Tools, name)()
+        getattr(Sniffing_and_Spoofing, name)()
+        getattr(PostExploitationAttacks, name)()
+        getattr(Anonymity, name)()
+        getattr(Framework, name)()
+        getattr(Pentesting_Bug_Bounty, name)()
+        getattr(forensic, name)()
+    except KeyboardInterrupt:
+        return
+    except Exception as err:
+        return
+    
+def getip(url='',path='',output=''):
         banner.main()
         banner.attack("Get Ip")
-        print(
-            f"{colors.green}The IP address of {domain_name} is {ip_address}{colors.reset}"
-        )
-
+        url=domain()['no_http'](url)
+        if url!="ip":
+            if path != "":
+                try:
+                    f = open(path, "r")
+                    urls = f.read()
+                    urls = urls.split("\n")
+                    for url in urls:
+                        if url != "":
+                            url=domain()['no_http'](url)
+                            if url!='ip':
+                                    try:
+                                        ip_address = socket.gethostbyname(url)
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t --> \t{ip_address}")
+
+                                        print(
+                                            f"{colors.green}[+]{url}\t --> \t{ip_address}{colors.reset}"
+                                        )
+                                    except Exception as err:
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t --> Something Went Wrong --> [!] {err}")
+                                        print(f"{colors.red}[-]{url}\t --> Something Went Wrong --> [!] {err}{colors.reset}")
+                            else:
+                                print(f"{colors.red}[-]{url}\t -->\tYou Have Entered IP{colors.reset}")
+                                if output != "":
+                                            outputfunc(output, f"{url}\t -->\tYou Have Entered IP")
 
-def ipinformation(ip):
-    if not ipinformation.called:
-        ipinformation.called=True
-        banner.main()
-        banner.attack("Get Ip Infomation")
-        print("waiting..\r", end="")
-        url = f"http://ip-api.com/json/{ip}"
-        response = requests.get(url)
-
-        data = response.json()
-        for key, value in data.items():
-            print(f"{colors.blue}[+] {key}\t --> \t{colors.green}{value}{colors.reset}")
+                except KeyboardInterrupt:
+                    exit_program()
+                except Exception as err:
+                    print(
+                        f"{colors.red}[-] Something Went Wrong\n[!] {err}\n[!] Check Your File location"
+                    )
+            else:
+                url=domain()['no_http'](url)
+                if url!='ip':
+                        try:
+                            ip_address = socket.gethostbyname(url)
+                            if output != "":
+                                outputfunc(output, f"{url}\t --> \t{ip_address}")
 
+                            print(
+                                f"{colors.green}[+]{url}\t --> \t{ip_address}{colors.reset}"
+                            )
+                        except Exception as err:
+                            if output != "":
+                                outputfunc(output, f"{url}\t --> Something Went Wrong --> [!] {err}")
+                            print(f"{colors.red}[-]{url}\t --> Something Went Wrong --> [!] {err}{colors.reset}")
+                else:
+                    print(f"{colors.red}[-]{url}\t -->\tYou Have Entered IP{colors.reset}")
+                    if output != "":
+                                outputfunc(output, f"{url}\t -->\tYou Have Entered IP")
+        else:
+            print(f"{colors.red}[-] Something Went Wrong\n[!] Maybe You have Entered Ip")
 
-def dnsrecords(domain, names):
-    if not dnsrecords.called:
-        dnsrecords.called=True
 
+def dnsrecords(url="", names='',path='',output=''):
         banner.main()
         banner.attack("DNS Records")
         names = names.upper()
         names = names.split(",")
-        for name in names:
-            try:
-                answers = dns.resolver.resolve(domain, name)
-                for answer in answers:
+        url=domain()['no_http'](url)
+        if url!="ip":
+            if path != "":
+                try:
+                    f = open(path, "r")
+                    urls = f.read()
+                    urls = urls.split("\n")
+                    for url in urls:
+                        if url != "":
+                            url=domain()['no_http'](url)
+                            if url!='ip':
+                                for name in names:
+                                    try:
+                                        answers = dns.resolver.resolve(url, name)
+                                        for answer in answers:
+                                            if output != "":
+                                                outputfunc(output, f"{url}\t -->\t{name}\t -->\t{answer}")
+                                            print(
+                                                f"{colors.blue}[+]{url}\t -->\t{name}\t -->\t{colors.green}{answer}{colors.reset}"
+                                            )
+                                    except dns.rdatatype.UnknownRdatatype:
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t -->\t{name}\t -->\tWrong Record Input")
+                                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\tWrong Record Input{colors.reset}")
+                                    except dns.resolver.NoAnswer:
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t -->\t{name}\t -->\tRecord Found")
+                                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\tNo {name} Record Found{colors.reset}")
+                                    except dns.resolver.NXDOMAIN:
+                                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\tHost {domain} Not Found{colors.reset}")
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t -->\t{name}\t -->\tHost {domain} Not Found")
+                                    except Exception as err:
+                                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\terr:{err}{colors.reset}")
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t -->\t{name}\t -->\terr:{err}")
+
+                            else:
+                                print(f"{colors.red}[-]{url}\t -->\tYou Have Entered IP{colors.reset}")
+                                if output != "":
+                                            outputfunc(output, f"{url}\t -->\tYou Have Entered IP")
+
+                except KeyboardInterrupt:
+                    exit_program()
+                except Exception as err:
                     print(
-                        f"{colors.blue}[+] {name}\t -->\t{colors.green}{answer}{colors.reset}"
+                        f"{colors.red}[-] Something Went Wrong\n[!] {err}\n[!] Check Your File location"
                     )
-            except dns.rdatatype.UnknownRdatatype:
-                print(f"{colors.red}[-] Wrong Record Input{colors.reset}")
-            except dns.resolver.NoAnswer:
-                print(f"{colors.red}[-] No {name} Record Found{colors.reset}")
-            except dns.resolver.NXDOMAIN:
-                print(f"{colors.red}[-] Host {domain} Not Found{colors.reset}")
+            else:
+                for name in names:
+                    try:
+                        answers = dns.resolver.resolve(url, name)
+                        for answer in answers:
+                            if output != "":
+                                outputfunc(output, f"{url}\t -->\t{name}\t -->\t{answer}")
+                            print(
+                                f"{colors.blue}[+]{url}\t -->\t{name}\t -->\t{colors.green}{answer}{colors.reset}"
+                            )
+                    except dns.rdatatype.UnknownRdatatype:
+                        if output != "":
+                            outputfunc(output, f"{url}\t -->\t{name}\t -->\tWrong Record Input")
+                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\tWrong Record Input{colors.reset}")
+                    except dns.resolver.NoAnswer:
+                        if output != "":
+                            outputfunc(output, f"{url}\t -->\t{name}\t -->\tRecord Found")
+                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\tNo {name} Record Found{colors.reset}")
+                    except dns.resolver.NXDOMAIN:
+                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\tHost {domain} Not Found{colors.reset}")
+                        if output != "":
+                            outputfunc(output, f"{url}\t -->\t{name}\t -->\tHost {domain} Not Found")
+                    except Exception as err:
+                        print(f"{colors.red}[-]{url}\t -->\t{name}\t -->\terr:{err}{colors.reset}")
+                        if output != "":
+                            outputfunc(output, f"{url}\t -->\t{name}\t -->\terr:{err}")
+
+        else:
+            print(f"{colors.red}[-] Something Went Wrong\n[!] Maybe You have Entered Ip")
+
 
 
 def checking(result_str):
 
         print(f"{colors.green}Checking for password{colors.reset}")
         passwords = [
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/xato-net-10-million-passwords.txt",
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Common-Credentials/10-million-password-list-top-1000000.txt",
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Common-Credentials/10-million-password-list-top-100000.txt",
             "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/xato-net-10-million-passwords-1000000.txt",
         ]
         for link in range(len(passwords)):
-            pass_check(passwords[link], result_str, link)
+            try:
+                pass_check(passwords[link], result_str, link)
+            except KeyboardInterrupt:
+                exit_program()
 
 
 def pass_check(url, password, number):
-    if not pass_check.called:
-        pass_check.called=True
         print(f"{colors.blue}Test {number}{colors.reset}")
-        raw = requests.get(url)
-        lists = raw.text.split("\n")
-        for i in lists:
-            if password == i:
-                print(f"{colors.red}FAILED{colors.reset}")
-        else:
-            print(f"{colors.green}PASSED{colors.reset}")
+        try:
+            raw = requests.get(url)
+            lists = raw.text.split("\n")
+            for i in lists:
+                if password == i:
+                    print(f"{colors.red}FAILED{colors.reset}")
+            else:
+                print(f"{colors.green}PASSED{colors.reset}")
 
+        except KeyboardInterrupt:
+                exit_program()
+        except Exception as err:
+            os.system("clear")
+            banner.main()
+            banner.attack(f"{colors.red}ERROR{colors.reset}")
+            banner.description(f"{colors.red}{err}{colors.reset}")
 
 def exit_program():
     print("\033[38;5;105m", "[+] Thanks visit again".title())
     exit()
 
 
 def asnrecord(path="", url="", output=""):
-    if not asnrecord.called:
-        asnrecord.called=True
-
         banner.main()
         banner.attack("ASN")
         if path != "":
             try:
                 f = open(path, "r")
                 urls = f.read()
                 urls = urls.split("\n")
                 for url in urls:
                     if url != "":
-                        try:
-                            ipwhois = IPWhois(url)
-                            result = ipwhois.lookup_rdap()
-                            if output != "":
-                                outputfunc(output, f"{url}\t --> {result['asn']}")
-                            print(
-                                f"{colors.blue}[+] {url}\t --> {colors.green}{result['asn']}{colors.reset}"
-                            )
-                        except KeyboardInterrupt:
-                            exit_program()
-                        except:
-                            if output != "":
-                                outputfunc(output, f"{url}\t --> Something Went Wrong")
-                            print(
-                                f"{colors.red}[+] {url}\t --> {colors.red}Something Went Wrong{colors.reset}"
-                            )
+                        valid=ip_valid(url)
+                        if valid==1:
+                            try:
+                                ipwhois = IPWhois(url)
+                                result = ipwhois.lookup_rdap()
+                                if output != "":
+                                    outputfunc(output, f"{url}\t --> {result['asn']}")
+                                print(
+                                    f"{colors.blue}[+] {url}\t --> {colors.green}{result['asn']}{colors.reset}"
+                                )
+                            except KeyboardInterrupt:
+                                exit_program()
+                            except Exception as err:
+                                if output != "":
+                                    outputfunc(output, f"{url}\t --> err:{err}")
+                                    print(
+                                        f"{colors.red}[+] {url}\t --> {colors.red}err:{err}{colors.reset}"
+                                    )
+                        else:
+                            print(f"{colors.red}[-] Something Went Wrong\n[!] Maybe You have Entered Domain Or Ip Range Is Wrong")
             except KeyboardInterrupt:
                 exit_program()
             except Exception as err:
                 print(
                     f"{colors.red}[-] Something Went Wrong\n[!] {err}\n[!] Check Your File location"
                 )
         else:
             try:
-                ipwhois = IPWhois(url)
-                result = ipwhois.lookup_rdap()
-                if output != "":
-                    outputfunc(output, f"{url}\t --> {result['asn']}")
-                print(
-                    f"{colors.blue}[+] {url}\t --> {colors.green}{result['asn']}{colors.reset}"
-                )
+                valid=ip_valid(url)
+                if valid==1:
+                    ipwhois = IPWhois(url)
+                    result = ipwhois.lookup_rdap()
+                    if output != "":
+                        outputfunc(output, f"{url}\t --> {result['asn']}")
+                    print(
+                        f"{colors.blue}[+] {url}\t --> {colors.green}{result['asn']}{colors.reset}"
+                    )
+                else:
+                    print(f"{colors.red}[-] Something Went Wrong\n[!] Maybe You have Entered Domain Or Ip Range Is Wrong")
             except KeyboardInterrupt:
                 exit_program()
             except:
                 if output != "":
                     outputfunc(output, f"{url}\t --> Something Went Wrong")
                 print(
                     f"{colors.red}[+] {url}\t --> {colors.red}Something Went Wrong{colors.reset}"
                 )
 
 
 def outputfunc(addr, line):
+
     f = open(addr, "a")
     f.write(line)
     f.write("\n")
     f.close()
 
 
 def http_status_code(path="", url="", output=""):
-    if not http_status_code.called:
-        http_status_code.called=True
-
-        link=domain(url)
+        link=domain()['check_http'](url)
         banner.main()
         banner.attack("HTTP Status Code")
-        if path != "":
-            try:
-                f = open(path, "r")
-                urls = f.read()
-                urls = urls.split("\n")
-                for url in urls:
+        if link=="ip":
+            print(f'{colors.red}Something Went Wrong\n[!] You Have Entered IP{colors.reset}')
+            return
+        else:
+            if path != "":
+                try:
+                    f = open(path, "r")
+                    urls = f.read()
+                    urls = urls.split("\n")
+                    for url in urls:
+                        if url != "":
+                            link=domain()['check_http'](url)
+                            if link=="ip":
+                                print(
+                                            f"{colors.red}[+] {url}\t --> {colors.red}You Have Entered Ip{colors.reset}"
+                                        )
+                            else:
+                                for url in link:
+                                    try:
+                                        headers = {
+                                            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36"
+                                        }
+                                        response = requests.get(url,allow_redirects=False, headers=headers, timeout=20)
+                                        status = str(response.status_code)
+                                        if status[0] == "1":
+                                            print(
+                                                f"{colors.blue}[+] {url}\t --> {colors.light_blue}{status}{colors.reset}"
+                                            )
+                                        elif status[0] == "2":
+                                            print(
+                                                f"{colors.blue}[+] {url}\t --> {colors.green}{status}{colors.reset}"
+                                            )
+                                        elif status[0] == "3":
+                                            print(
+                                                f"{colors.blue}[+] {url}\t --> {colors.yellow}{status}{colors.reset}",end=''
+                                            )
+                                            try:
+                                                response = requests.get(url, headers=headers, timeout=20)
+                                                status = str(response.status_code)
+                                                new_url=str(response.url)
+                                                if status[0] == "1":
+                                                    print(
+                                                        f"{colors.blue} --> {colors.light_blue}{status} -->{colors.blue} {new_url}{colors.reset}"
+                                                    )
+                                                elif status[0] == "2":
+                                                    print(
+                                                        f"{colors.blue} --> {colors.green}{status} -->{colors.blue} {new_url}{colors.reset}"
+                                                    )
+                                                elif status[0] == "3":
+                                                    print(
+                                                        f"{colors.blue} --> {colors.yellow}{status} -->{colors.blue} {new_url}{colors.reset}"
+                                                    )
+                                                elif status[0] == "4":
+                                                    print(
+                                                        f"{colors.blue} --> {colors.red}{status} -->{colors.blue} {new_url}{colors.reset}"
+                                                    )
+                                                elif status[0] == "5":
+                                                    print(
+                                                        f"{colors.blue} --> {colors.purple}{status} -->{colors.blue} {new_url}{colors.reset}"
+                                                    )
+                                                else:
+                                                    print(
+                                                        f"{colors.blue} --> {colors.green}{status} -->{colors.blue} {new_url}{colors.reset}"
+                                                    )
+                                            except Exception as err:
+                                                if "timed out" in str(err):
+                                                    err = "Connection Time Out"
+                                                print(
+                                                    f"{colors.red} --> {colors.red}{err}{colors.reset}"
+                                                )
+
+
+                                        elif status[0] == "4":
+                                            print(
+                                                f"{colors.blue}[+] {url}\t --> {colors.red}{status}{colors.reset}"
+                                            )
+                                        elif status[0] == "5":
+                                            print(
+                                                f"{colors.blue}[+] {url}\t --> {colors.purple}{status}{colors.reset}"
+                                            )
+                                        else:
+                                            print(
+                                                f"{colors.blue}[+] {url}\t --> {colors.green}{status}{colors.reset}"
+                                            )
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t --> {status}")
+                                    except Exception as err:
+                                        if "timed out" in str(err):
+                                            err = "Connection Time Out"
+                                        if output != "":
+                                            outputfunc(output, f"{url}\t --> {err}")
+                                        print(
+                                            f"{colors.red}[-] {url}\t --> {colors.red}{err}{colors.reset}"
+                                        )
+                                    time.sleep(0.5)
+                except KeyboardInterrupt:
+                    exit_program()
+
+                except Exception as err:
+                    print(f"{colors.red}[-] Something Went Wrong\n[!] {err}")
+            else:
+                try:
                     if url != "":
-                        link=domain(url)
                         for url in link:
-
                             try:
                                 headers = {
                                     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36"
                                 }
-                                response = requests.get(url, headers=headers, timeout=20)
+                                response = requests.get(url,allow_redirects=False , headers=headers, timeout=20)
                                 status = str(response.status_code)
                                 if status[0] == "1":
                                     print(
                                         f"{colors.blue}[+] {url}\t --> {colors.light_blue}{status}{colors.reset}"
                                     )
                                 elif status[0] == "2":
                                     print(
@@ -192,88 +416,31 @@
                                     print(
                                         f"{colors.blue}[+] {url}\t --> {colors.green}{status}{colors.reset}"
                                     )
                                 if output != "":
                                     outputfunc(output, f"{url}\t --> {status}")
                             except Exception as err:
                                 if "timed out" in str(err):
-                                    err = "Connection Time Outed"
-                                else:
-                                    err = "Something Went Wrong"
+                                    err = "Connection Time Out"
                                 if output != "":
                                     outputfunc(output, f"{url}\t --> {err}")
                                 print(
                                     f"{colors.red}[+] {url}\t --> {colors.red}{err}{colors.reset}"
                                 )
-                    time.sleep(0.5)
-            except KeyboardInterrupt:
-                exit_program()
-
-            except Exception as err:
-                print(f"{colors.red}[-] Something Went Wrong\n[!] {err}")
-        else:
-            try:
-                if url != "":
-                    for url in link:
-                        try:
-                            headers = {
-                                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36"
-                            }
-                            response = requests.get(url, headers=headers, timeout=20)
-                            status = str(response.status_code)
-                            if status[0] == "1":
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.light_blue}{status}{colors.reset}"
-                                )
-                            elif status[0] == "2":
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.green}{status}{colors.reset}"
-                                )
-                            elif status[0] == "3":
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.yellow}{status}{colors.reset}"
-                                )
-                            elif status[0] == "4":
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.red}{status}{colors.reset}"
-                                )
-                            elif status[0] == "5":
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.purple}{status}{colors.reset}"
-                                )
-                            else:
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.green}{status}{colors.reset}"
-                                )
-                            if output != "":
-                                outputfunc(output, f"{url}\t --> {status}")
-                        except Exception as err:
-                            if "timed out" in str(err):
-                                err = "Connection Time Outed"
-                            else:
-                                err = "Something Went Wrong"
-                            if output != "":
-                                outputfunc(output, f"{url}\t --> {err}")
-                            print(
-                                f"{colors.red}[+] {url}\t --> {colors.red}{err}{colors.reset}"
-                            )
-                        time.sleep(0.5)
-            except KeyboardInterrupt:
-                exit_program()
+                            time.sleep(0.5)
+                except KeyboardInterrupt:
+                    exit_program()
 
-            except Exception as err:
-                print(f"{colors.red}[-] Something Went Wrong\n[!] {err}")
+                except Exception as err:
+                    print(f"{colors.red}[-] Something Went Wrong\n[!] {err}")
 
 
 def password_gen(
     upper=True, lower=True, digit=True, punctuation=True, length="8", check=True
 ):
-    if not password_gen.called:
-        password_gen.called=True
-
         banner.main()
         banner.attack("Password Generators")
         ascii_lowercase = "abcdefghijklmnopqrstuvwxyz"
         ascii_uppercase = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
         string_digits = "0123456789"
         string_punctuation = r"""!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~"""
         main_password = ""
@@ -294,19 +461,28 @@
                 checking(result_str)
         except KeyboardInterrupt:
                 exit_program()
         except IndexError:
             print(
                 f"{colors.red}[-] Please Specify atleast one argument (--upper,--lower,--digits,--punctuation) {colors.reset}"
             )
-
+def generate_wordlist(characters=True, min_length=True, max_length=True, output_file=True):
+    try:
+        with open(output_file, 'w') as file:
+
+            for length in range(min_length, max_length + 1):
+
+                for combination in itertools.product(characters, repeat=length):
+
+                    word = ''.join(combination)
+                    file.write(word + '\n')
+        print(f"[+] Wordlist generated and saved to {output_file}.txt")
+    except KeyboardInterrupt:
+                exit_program()
 def remove_dublicates(location,output=''):
-    if not remove_dublicates.called:
-        remove_dublicates.called=True
-
         f=open(location,'r')
         lines=f.read()
         lines=lines.split('\n')
         readed=[]
         for line in lines:
             if line not in readed:
                 readed.append(line)
@@ -330,101 +506,142 @@
                 fn.write('\n')
             fn.close()
 
 
         
 
 def screenshot(path="", url="",output=''):
-    if not screenshot.called:
-        screenshot.called=True
-
-        link=domain(url)
+        link=domain()['check_http'](url)
         banner.main()
         banner.attack("Screenshotting")
-        if path != "":
-            try:
-                f = open(path, "r")
-                urls = f.read()
-                urls = urls.split("\n")
-                for url in urls:
-                    if url != "":
-                        link=domain(url)
-                        for url in link:
-                            driver_path = "main/tools/.driver/geckodriver"
-                            firefox_options = webdriver.FirefoxOptions()
-                            firefox_options.headless = True
-                            driver = webdriver.Firefox(
-                                executable_path=driver_path, options=firefox_options
-                            )
-                            try:
-                                driver.get(url)
-                                url_new = url.split("//")
-                                path = os.getcwd()
-                                if output!='':
-                                    screenshot_filename=f'{output}/{url_new[0]}_{url_new[1].replace("/","_")}.png'
-                                else:
-                                    if not os.path.isdir("Screenshot"):
-                                        os.system("mkdir Screenshot")
-                                    screenshot_filename = f'{path}/Screenshot/{url_new[0]}_{url_new[1].replace("/","_")}.png'
-                                driver.save_screenshot(screenshot_filename)
-                                print(
-                                    f"{colors.blue}[+] {url}\t --> {colors.green}Screenshot saved to {screenshot_filename}{colors.reset}"
-                                )
-                                driver.quit()
-                            except KeyboardInterrupt:
-                                exit_program()
-                            except Exception as err:
-                                print(
-                                    f"{colors.red}[+] {url}\t --> {colors.red}Something Went Wrong\n[!] {err}{colors.reset}"
-                                )
-                            time.sleep(0.5)
-            except Exception as err:
-                print(
-                    f"{colors.red}[-] Something Went Wrong\n[!] {err}\n[!] Check Your File location"
-                )
+        if link=="ip":
+            print(f'{colors.red}Something Went Wrong\n[!] You Have Entered IP{colors.reset}')
+            return
         else:
-            driver_path = "main/tools/.driver/geckodriver"
-            firefox_options = webdriver.FirefoxOptions()
-            firefox_options.headless = True
-            driver = webdriver.Firefox(executable_path=driver_path, options=firefox_options)
-            for url in link:
+            if path != "":
                 try:
-                    driver.get(url)
-                    url_new = url.split("//")
-                    path = os.getcwd()
-                    if output!='':
-                        screenshot_filename=f'{output}/{url_new[0]}_{url_new[1].replace("/","_")}.png'
-                    else:
-                        if not os.path.isdir("Screenshot"):
-                            os.system("mkdir Screenshot")
-                        screenshot_filename = f'{path}/Screenshot/{url_new[0]}_{url_new[1].replace("/","_")}.png'
-                    if not os.path.isdir("Screenshot"):
-                        os.system("mkdir Screenshot")
-                    driver.save_screenshot(screenshot_filename)
-                    print(
-                        f"{colors.blue}[+] {url}\t --> {colors.green}Screenshot saved to {screenshot_filename}{colors.reset}"
-                    )
-                    driver.quit()
-                except KeyboardInterrupt:
-                    exit_program()
+                    f = open(path, "r")
+                    urls = f.read()
+                    urls = urls.split("\n")
+                    for url in urls:
+                        if url != "":
+                            link=domain()['check_http'](url)
+                            if link=="ip":
+                                print(
+                                        f"{colors.red}[-] {url}\t --> {colors.red}It Is a IP{colors.reset}"
+                                    )
+                            else:
+                                for url in link:
+                                    driver_path = "main/tools/.driver/geckodriver"
+                                    firefox_options = webdriver.FirefoxOptions()
+                                    firefox_options.headless = True
+                                    driver = webdriver.Firefox(
+                                        executable_path=driver_path, options=firefox_options
+                                    )
+                                    try:
+                                        driver.get(url)
+                                        url_new = url.split("//")
+                                        path = os.getcwd()
+                                        if output!='':
+                                            screenshot_filename=f'{output}/{url_new[0]}_{url_new[1].replace("/","_")}.png'
+                                        else:
+                                            if not os.path.isdir("Screenshot"):
+                                                os.system("mkdir Screenshot")
+                                            screenshot_filename = f'{path}/Screenshot/{url_new[0]}_{url_new[1].replace("/","_")}.png'
+                                        driver.save_screenshot(screenshot_filename)
+                                        print(
+                                            f"{colors.blue}[+] {url}\t --> {colors.green}Screenshot saved to {screenshot_filename}{colors.reset}"
+                                        )
+                                        driver.quit()
+                                    except KeyboardInterrupt:
+                                        exit_program()
+                                    except Exception as err:
+                                        print(
+                                            f"{colors.red}[+] {url}\t --> {colors.red}Something Went Wrong\n[!] {err}{colors.reset}"
+                                        )
+                                    time.sleep(0.5)
                 except Exception as err:
                     print(
-                        f"{colors.red}[+] {url}\t --> {colors.red}Something Went Wrong\n[!] {err}{colors.reset}"
+                        f"{colors.red}[-] Something Went Wrong\n[!] {err}\n[!] Check Your File location"
                     )
-                time.sleep(0.5)
-def domain(url):
-    urls=[]
-    if "http://" and "https://" not in url:
-        urls.append("http://"+url)
-        urls.append("https://"+url)
-    else:
-        urls.append(url)
-    return urls
-getip.called=False
-ipinformation.called=False
-screenshot.called=False
-remove_dublicates.called=False
-password_gen.called=False
-http_status_code.called=False
-asnrecord.called=False
-dnsrecords.called=False
-pass_check.called=False
+            else:
+                driver_path = "./main/tools/.driver/geckodriver"
+                firefox_options = webdriver.FirefoxOptions()
+                firefox_options.headless = True
+                driver = webdriver.Firefox(executable_path=driver_path, options=firefox_options)
+                for url in link:
+                    try:
+                        driver.get(url)
+                        url_new = url.split("//")
+                        path = os.getcwd()
+                        if output!='':
+                            if not os.path.isdir(output):
+                                os.mkdir(output)
+                            screenshot_filename=f'{output}/{url_new[0]}_{url_new[1].replace("/","_")}.png'
+                        else:
+                            if not os.path.isdir("Screenshot"):
+                                os.system("mkdir Screenshot")
+                            screenshot_filename = f'{path}/Screenshot/{url_new[0]}_{url_new[1].replace("/","_")}.png'
+                        if not os.path.isdir("Screenshot"):
+                            os.system("mkdir Screenshot")
+                        driver.save_screenshot(screenshot_filename)
+                        print(
+                            f"{colors.blue}[+] {url}\t --> {colors.green}Screenshot saved to {screenshot_filename}{colors.reset}"
+                        )
+                        #driver.quit()
+                        #time.sleep(5)
+                    except KeyboardInterrupt:
+                        exit_program()
+                    except Exception as err:
+                        print(
+                            f"{colors.red}[+] {url}\t --> {colors.red}Something Went Wrong\n[!] {err}{colors.reset}"
+                        )
+                    time.sleep(0.5)
+                driver.quit()
+def domain():
+    def check_http(url):
+        urls=[]
+        if "https://" not in url and "http://" not in url:
+            valid=ip_valid(url)
+            if valid==3:
+                urls.append("http://"+url)
+                urls.append("https://"+url)
+            else:
+                urls="ip"
+        else:
+            urls.append(url)
+        return urls
+    def no_http(url):
+        if "http://" and "https://" not in url:
+            valid=ip_valid(url)
+            if valid==3:
+                return url
+            else:
+                url="ip"
+        else:
+            if "http://" in url:
+                url=url.split("http://")
+                url=url[1]
+            elif "https://" in url:
+                url=url.split("https://")
+                url=url[1]
+
+            return url
+    return {"check_http":check_http,"no_http":no_http}
+
+def ip_valid(user_input):
+    parts = user_input.split(".")
+    for part in parts:
+        try:
+            part=int(part)
+            if len(parts) == 4:
+                is_ip_address = True
+                for part in parts:
+                    if not part.isdigit() or not (0 <= int(part) <= 255):
+                        is_ip_address = False
+                        break
+                if is_ip_address:
+                    return 1
+                else:
+                    return 2
+        except:
+            return 3
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tool.py` & `cyberonix-3.0.0/cyberonix/main/tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,78 @@
 from cyberonix.main.tools import *
+#from main.tools import Anonymity
+#from main.tools import Framework
 import os
-import inspect
 def exit_program():
         os.system("clear")
         banner.main()
         print("\033[38;5;105m","[+] Thanks visit again".title())
-def main():
-    if inspect.stack()[1].function != "main":
-        if not main.called:
-              main.called=True
-              start()
-    else:
-        start()
 
-def start():
+def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("TOOLS")
         # import information_gathering
 
-        list_attacks=["Information Gathering","Vulnerability Analysis","Web Application Analysis","Password Attacks","Wireless Attacks","Exploitation Tools","Sniffing and Spoofing","Post Exploitation","Pentesting and Bug-Bounty","go back"]
+        list_attacks=[" Information Gathering"," Vulnerability Analysis"," Web Application Analysis"," Password Attacks"," Wireless Attacks"," Exploitation Tools"," Sniffing and Spoofing"," Post Exploitation"," Anonymity","Framework","Pentesting In Bug-Bounty","Digital Forensics Tools","go back"]
         #for output with index
         for i in range(len(list_attacks)):
-                print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+                print(colors.options,f"{i+1}) {list_attacks[i]}".title(),colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
+            return
+        if option == "1":
             print("\n[+] Information Gathering Section")
             os.system("clear")
             information_gathering.main()
-        elif option == "1":
+        elif option == "2":
             print("\n[+] Vulnerability Analysis")
             os.system("clear")
             Vulnerability_Analysis.main()
-        elif option == "2":
+        elif option == "3":
             print("\n[+] Web Application Analysis")
             os.system("clear")
             WEB_Application_Analysis.main()
-        elif option == "3":
+        elif option == "4":
             print("\n[+] Password Attacks")
             os.system("clear")
             Password_Hacking.main()
-        elif option == "4":
+        elif option == "5":
             print("\n[+] Wireless Attacks")
             os.system("clear")
             Wireless_Hacking.main()
-        elif option == "5":
+        elif option == "6":
             print("\n[+] Exploitation Tools")
             os.system("clear")
             Exploitation_Tools.main()
-        elif option == "6":
+        elif option == "7":
             print("\n[+] Sniffing and Spoofing")
             os.system("clear")
             Sniffing_and_Spoofing.main()
-        elif option == "7":
+        elif option == "8":
             print("\n[+] Post Exploitation")
             os.system("clear")
             PostExploitationAttacks.main()
-        elif option == "8":
-            print("\n[+] Pentesting and Bug-Bounty")
+        elif option == "9":
+            print("\n[+] Anonymity")
+            os.system("clear")
+            Anonymity.main()
+        elif option == "10":
+            print("\n[+]Framework")
+            os.system("clear")
+            Framework.main()
+        elif option == "11":
+            print("\n[+] Pentesting In Bug-Bounty")
             os.system("clear")
             Pentesting_Bug_Bounty.main()
+        elif option == "12":
+            print("\n[+] Digital Forensics Tools ")
+            os.system("clear")
+            forensic.main()
         else:
             exit_program()
             return
-main.called=False
 
 if __name__ == "__main__": 
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Authentication.py` & `cyberonix-3.0.0/cyberonix/main/tools/Authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,144 +6,145 @@
 
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Authentication")
         list_vulns = [
-            "User enumeration",
-            "Authentication bypass",
-            "vulnerable remember me functionality",
-            "Password reset",
-            "Captcha bypass",
-            "Autocomplete on ",
-            "multifactor authentication",
-            "Logout functionality",
-            "cache management",
+            " User enumeration",
+            " Authentication bypass",
+            " vulnerable remember me functionality",
+            " Password reset",
+            " Captcha bypass",
+            " Autocomplete on ",
+            " multifactor authentication",
+            " Logout functionality",
+            " cache management",
             "Default credentials",
             "Go back",
         ]
         for i in range(len(list_vulns)):
-            print(colors.options, f"{i}) {list_vulns[i]}".title(), colors.reset)
+            print(colors.options, f"{i+1}) {list_vulns[i]}".title(), colors.reset)
         try:
             vulns = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if vulns == "0":
+            return
+        
+        if vulns == "1":
             os.system("clear")
             template.template(
                 "Test for User enumeration",
                 "no-tools",
                 "",
                 {
                     "Testing for Account Enumeration and Guessable User Account": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/03-Identity_Management_Testing/04-Testing_for_Account_Enumeration_and_Guessable_User_Account",
                     "What Is User Enumeration?": "https://www.rapid7.com/blog/post/2017/06/15/about-user-enumeration/",
                 },
             )
-        elif vulns == "1":
+        elif vulns == "2":
             os.system("clear")
             template.template(
                 "Testing for authentication bypass",
                 "no-tools",
                 "",
                 {
                     "Testing for Bypassing Authentication Schema": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/04-Authentication_Testing/04-Testing_for_Bypassing_Authentication_Schema",
                     "5 Unusual Authentication Bypass Techniques": "https://www.synack.com/blog/exploits-explained-5-unusual-authentication-bypass-techniques/",
                     "Authentication vulnerabilities": "https://portswigger.net/web-security/authentication",
                 },
             )
 
-        elif vulns == "2":
+        elif vulns == "3":
             os.system("clear")
             template.template(
                 "Testing for vulnerable remember me functionality",
                 "no-tools",
                 "",
                 {
                     "Testing for Vulnerable Remember Password": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/04-Authentication_Testing/05-Testing_for_Vulnerable_Remember_Password",
                     "Exploiting Remember Me Cookie For Account Takeover": "https://gupta-bless.medium.com/exploiting-remember-me-cookie-for-account-takeover-4e8d5fd42d4b",
                 },
             )
 
-        elif vulns == "3":
+        elif vulns == "4":
             os.system("clear")
             template.template(
                 "Testing for Password reset",
                 "no-tools",
                 "",
                 {
                     "Password reset poisoning": "https://portswigger.net/web-security/host-header/exploiting/password-reset-poisoning",
-                    "Testing Forgot Password Functionality": "https://twitter.com/tuhin1729_/status/1437471718142976007?t=G7ODwQzc6ON2T6_DDC89jA&s=19",
+                    "Testing Forgot Password Functionality": "https://github.com/tuhin1729/Bug-Bounty-Methodology/blob/main/PasswordReset.md",
                     "Exploiting Password Reset Poisoning": "https://infosecwriteups.com/exploiting-password-reset-poisoning-b748797f0661",
                 },
             )
 
-        elif vulns == "4":
+        elif vulns == "5":
             os.system("clear")
             template.template(
                 "Testing for Captcha bypass",
                 "no-tools",
                 "",
                 {
                     "CAPTCHA BYPASS TECHNIQUES !": "https://honeyakshat999.medium.com/captcha-bypass-techniques-f768521516b2",
-                    "Bypass Captcha🤗(Google reCAPTCHA)": "https://twitter.com/Aacle_/status/1586735203481161728?t=Vz4U17f1nHQzoXRUuMVDiA&s=19",
+                    "Bypass Captcha (Google reCAPTCHA)": "https://twitter.com/Aacle_/status/1586735203481161728?t=Vz4U17f1nHQzoXRUuMVDiA&s=19",
                     "Captcha Bypass Techniques": "https://github.com/harsh-bothra/learn365/blob/main/days/day31.md",
                 },
             )
 
-        elif vulns == "5":
+        elif vulns == "6":
             os.system("clear")
             template.template(
                 "Test for autocomplete on",
                 "no-tools",
                 "",
                 {
-                    " Password field with autocomplete enabled ": "https://portswigger.net/kb/issues/00500800_password-field-with-autocomplete-enabled",
+                    "Password field with autocomplete enabled ": "https://portswigger.net/kb/issues/00500800_password-field-with-autocomplete-enabled",
                     "Finding and Fixing Vulnerabilities in AutoComplete Not Disabled ": "https://www.beyondsecurity.com/scan-pentest-network-vulnerabilities-autocomplete-not-disabled",
                 },
             )
 
-        elif vulns == "6":
+        elif vulns == "7":
             os.system("clear")
             template.template(
                 "Testing for multifactor authentication",
                 "no-tools",
                 "",
                 {
                     "Testing Multi-Factor Authentication (MFA)": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/04-Authentication_Testing/11-Testing_Multi-Factor_Authentication",
                     "Testing Two-Factor Authentication": "https://research.nccgroup.com/2021/06/10/testing-two-factor-authentication/",
                     "How to Test Two-Factor Authentication: A Guide with Use Cases": "https://www.browserstack.com/guide/test-two-factor-authentication",
                 },
             )
 
-        elif vulns == "7":
+        elif vulns == "8":
             os.system("clear")
             template.template(
-                "Check SSL Version, Algorithms",
+                "Tesing for Logout functionality",
                 "no-tools",
                 "",
                 {
                     "Testing for Logout Functionality": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/06-Session_Management_Testing/06-Testing_for_Logout_Functionality",
-                    " Test Cases For Logout | Test Scenarios For Logout ": "https://www.qaacharya.in/2019/06/test-cases-scenarios-for-logout.html",
+                    "Test Cases For Logout | Test Scenarios For Logout ": "https://www.qaacharya.in/2019/06/test-cases-scenarios-for-logout.html",
                 },
             )
 
-        elif vulns == "8":
+        elif vulns == "9":
             os.system("clear")
             template.template(
                 "Test for cache management",
                 "no-tools",
                 "",
                 {
                     "Testing for Browser Cache Weaknesses": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/04-Authentication_Testing/06-Testing_for_Browser_Cache_Weaknesses",
                     "Cache Controls Explained": "https://www.virtuesecurity.com/kb/cache-controls-explained/",
                 },
             )
 
-        elif vulns == "9":
+        elif vulns == "10":
             template.template(
                 "Test for Default credentials",
                 "no-tools",
                 "",
                 {
                     "Testing for Default Credentials": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/04-Authentication_Testing/02-Testing_for_Default_Credentials",
                     "How default credentials helped this Hacker to get 13337$": "https://medium.com/@ashishrohra/how-default-credentials-helped-this-hacker-to-get-13337-s-d1504ebf95e4",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Authorization.py` & `cyberonix-3.0.0/cyberonix/main/tools/data_validation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,420 @@
-from cyberonix.main.tools import banner, colors, template,WEB_Application_Analysis
-from cyberonix.main import Cheat_sheet
+from bs4 import BeautifulSoup
+from cyberonix.main.tools import banner, template, writeup, colors,Exploitation_Tools
 import os
 import requests
-from bs4 import BeautifulSoup
 
 
-# main function
 def main():
     while True:
         os.system("clear")
         banner.main()
-        banner.attack("Authorization")
-        list_attacks = ["Tools", "Writeups", "Burp Extensions", "Go Back"]
-        for i in range(len(list_attacks)):
-            print(colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset)
+        banner.attack("Data Validation Vulnerabilities")
+        list_vulns = [
+            "XSS",
+            "XXE - XML",
+            "HTML Injection",
+            "SQL Injection",
+            "Command Injection",
+            "HTTP Smuggling",
+            "HTTP Parameter Pollution",
+            "Open Redirection",
+            "LFI",
+            "Go Back",
+        ]
+        for i in range(len(list_vulns)):
+            print(colors.options, f"{i+1}) {list_vulns[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            vulns = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
+            return
+        if vulns == "1":
             while True:
-                print("\n[+] Tools")
                 os.system("clear")
                 banner.main()
-                banner.attack("Tools")
-                list_attacks = [
-                    "Burp Suite",
-                    "Wireshark",
-                    "OWASP ZAP",
-                    "Nessus",
-                    "Hydra",
-                    "BeEF",
-                    "Sqlmap",
-                    "Metasploit",
-                    "Nmap",
-                    "Penetration Testers Framework (PTF)",
-                    "Go Back",
-                ]
-                for i in range(len(list_attacks)):
-                    print(
-                        colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset
-                    )
-                try:
-                    option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
-                except KeyboardInterrupt:
-                    template.exit_program()
-                if option == "0":
-                    os.system("clear")
-                    WEB_Application_Analysis.burp_suite()
-                elif option == "1":
-                    os.system("clear")
-                    github = "Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. It can be used to examine data from a live network or from a previously saved capture file. Wireshark provides a graphical user interface (GUI) for capturing and analyzing network traffic."
-                    template.template(
-                        "wireshark",
-                        "wireshark",
-                        github.strip(),
-                        {
-                            "Wireshark Cheat-Sheet": "https://www.comparitech.com/net-admin/wireshark-cheat-sheet",
-                            "What-is-Wireshark-and-How-to-Use-it": "https://www.comptia.org/content/articles/what-is-wireshark-and-how-to-use-it ",
-                            "Video Resource Wireshark": "https://www.youtube.com/playlist?list=PLBf0hzazHTGPgyxeEj_9LBHiqjtNEjsgt",
-                        },
-                    )
-                elif option == "2":
-                    os.system("clear")
-                    github = "The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.\nIt is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox."
-                    template.template(
-                        "zaproxy",
-                        "zaproxy > /dev/null 2>&1",
-                        github.strip(),
-                        {
-                            "How to setup OWASP ZAP to scan your web application for security vulnerabilities": "https://www.linkedin.com/pulse/how-setup-owasp-zap-scan-your-web-application-security-botla/",
-                            "Authenticated Scan using OWASP-ZAP": "https://medium.com/@secureica/authenticated-scan-using-owasp-zap-f0a71dafe41",
-                            "OWASP ZAP: 6 Key Capabilities and a Quick Tutorial": "https://www.hackerone.com/knowledge-center/owasp-zap-6-key-capabilities-and-quick-tutorial",
-                            "Initial Setup": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/untitled",
-                            "Setup OWASP ZAP": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/setup-owasp-zap",
-                        },
-                    )
-                elif option == "3":
-                    os.system("clear")
-                    github = github_getting_text(
-                        "https://www.techtarget.com/searchnetworking/definition/Nessus",
-                        'section[id="content-body"]',
-                        0,
-                    )
-                    template.template(
-                        "nessus",
-                        "nessus",
-                        github.strip(),
-                        {
-                            "How To: Run Your First Vulnerability Scan with Nessus": "https://www.tenable.com/blog/how-to-run-your-first-vulnerability-scan-with-nessus",
-                            "A brief introduction to the Nessus vulnerability scanner": "https://resources.infosecinstitute.com/topic/a-brief-introduction-to-the-nessus-vulnerability-scanner/",
-                            "Beginner’s Guide to Nessus": "https://www.hackingarticles.in/beginners-guide-to-nessus/",
-                            "Nessus Ubuntu Installation and Tutorial": "https://linuxhint.com/nessus-ubuntu-installation-tutorial/",
-                        },
-                        link="https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.4.2-debian9_amd64.deb",
-                        method="deb",
-                    )
-                elif option == "4":
-                    os.system("clear")
-                    github_p1 = github_getting_text(
-                        "https://www.kali.org/tools/hydra/", "p", 2
-                    )
-                    github_p2 = github_getting_text(
-                        "https://www.kali.org/tools/hydra/", "p", 3
-                    )
-                    github_p3 = github_getting_text(
-                        "https://www.kali.org/tools/hydra/", "p", 4
-                    )
-                    github = github_p1 + github_p2 + github_p3
-                    template.template(
-                        "hydra",
-                        "hydra",
-                        github.strip(),
-                        {
-                            "How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool",
-                            "Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af",
-                        },
-                    )
-                elif option == "5":
-                    os.system("clear")
-                    github_p1 = github_getting_text(
-                        "https://github.com/beefproject/beef", 'p[dir="auto"]', 2
-                    )
-                    github_p2 = github_getting_text(
-                        "https://github.com/beefproject/beef", 'p[dir="auto"]', 3
-                    )
-                    github = github_p1 + github_p2
-                    template.template(
-                        "beef-xss",
-                        "beef-xss",
-                        github.strip(),
-                        {
-                            "BEeF Hacking Framework Tutorial [5 Easy Steps]": "https://www.golinuxcloud.com/beef-hacking-framework-tutorial/",
-                            "Browser Exploitation and Advanced Threat Actors: An Overview of BeEF": "https://medium.com/@andrearebora/browser-exploitation-and-advanced-threat-actors-an-overview-of-beef-bb907a5b73fa",
-                            "Hooking victims to Browser Exploitation Framework (BeEF) using Reflected and Stored XSS.": "https://medium.com/@secureica/hooking-victims-to-browser-exploitation-framework-beef-using-reflected-and-stored-xss-859266c5a00a",
-                            "Hijacking Browser with BeEF Framework": "https://medium.com/@krunalkumarpatel/hijacking-browser-with-beef-framework-bea784c03149",
-                        },
-                    )
-                elif option == "6":
-                    os.system("clear")
-                    github = github_getting_text("https://sqlmap.org/", "p", 0)
-                    template.template(
-                        "sqlmap",
-                        "sqlmap -h",
-                        github.strip(),
-                        {
-                            "Usage Of Sqlmap": "https://github.com/sqlmapproject/sqlmap/wiki/Usage",
-                            "How to use SQLMAP to test a website for SQL Injection vulnerability": "https://www.geeksforgeeks.org/use-sqlmap-test-website-sql-injection-vulnerability/",
-                            "How to Use SQLMap to Find Database Vulnerabilities": "https://www.freecodecamp.org/news/how-to-protect-against-sql-injection-attacks/",
-                            "SQLMap - Cheetsheat": "https://book.hacktricks.xyz/pentesting-web/sql-injection/sqlmap",
-                        },
-                    )
-                elif option == "7":
-                    os.system("clear")
-                    github = "The Metasploit Framework is an open-source tool for developing and executing exploit code against a remote target machine. It can be used to test the security of a computer system by finding and exploiting vulnerabilities. The framework includes a large collection of exploit modules, as well as various tools for payload generation, post-exploitation, and more. It can be used by security professionals for penetration testing, as well as by attackers for malicious purposes."
-                    template.template(
-                        "metasploit-framework",
-                        "msfconsole",
-                        github.strip(),
+                banner.attack("XSS")
+                # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
+                ask = vuln_options()
+                if ask == "1":
+                    while True:
+                        os.system("clear")
+                        banner.main()
+                        banner.attack("XSS")
+                        des = "It is recommended to test manually for XSS vulnerability to get better understanding & results.\nCheck out the writeup section to to learn about Cross Site Scripting"
+                        banner.description(des)
+                        list_tools = ["Dalfox", "XSStrike", "Xsser", "go back"]
+                        for i in range(len(list_tools)):
+                            print(
+                                colors.options,
+                                f"{i+1}) {list_tools[i]}".title(),
+                                colors.reset,
+                            )
+                        option = input(
+                            f"\n {colors.select}Select an Option ->{colors.reset} "
+                        )
+                        if option == "1":
+                            print("\n[+] Dalfox")
+                            dalfox()
+                        elif option == "2":
+                            print("\n[+] XSStrike")
+                            xsstrike()
+                        elif option == "3":
+                            print("\n[+] Xsser")
+                            xsser()
+                        else:
+                            # print(f"{colors.red}[-]Wrong Input{colors.reset}")
+                            break
+                elif ask == "2":
+                    writeup.writeup(
                         {
-                            "Msf-Community-Post-Exploitation": "https://www.offensive-security.com/metasploit-unleashed/msf-community-post-exploitation",
-                            "Post Exploitation In Linux With Metasploit": "https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/",
-                            "Privilege Escalation (Metasploit Unleashed)": "https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/",
-                            "Post Exploitation Metasploit Modules (Reference)": "https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference",
-                            "PSExec Pass the Hash (Horizontal Escalation)": "https://www.offensive-security.com/metasploit-unleashed/psexec-pass-hash/",
-                            "ms10_002_aurora (Vertical Escalation)": "https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/",
-                            "ms10_002_aurora (Horizontal Escalation)": "https://www.offensive-security.com/metasploit-unleashed/pivoting/ ",
-                            "jtr_crack_fast (Hash Cracking)": "https://www.offensive-security.com/metasploit-unleashed/john-ripper/",
-                            "warftpd_165_user (Keylogging)": "https://www.offensive-security.com/metasploit-unleashed/keylogging/",
-                            "3proxy (Backdoor)": "https://www.offensive-security.com/metasploit-unleashed/meterpreter-backdoor/",
-                            "persistence.rb (Persistent Backdoor)": "https://www.offensive-security.com/metasploit-unleashed/meterpreter-service/",
-                            "Enabling Remote Desktop": "https://www.offensive-security.com/metasploit-unleashed/enabling-remote-desktop/",
-                            "Post Exploitation in Linux with Metasploit": "https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/",
-                            "Post Exploitation Metasploit Modules Reference": "https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference/",
-                            "Hack Like Pro: Kill and Disable Antivirus Software Remote PC": "https://null-byte.wonderhowto.com/how-to/hack-like-pro-kill-and-disable-antivirus-software-remote-pc-0141906/",
-                            "Armitage Post Exploitation": "https://www.offensive-security.com/metasploit-unleashed/armitage-post-exploitation/",
-                            "Setup Armitage as a Command & Control Framework for Free": "https://infosecwriteups.com/setup-armitage-as-a-command-control-c2-framework-for-free-bae590064817",
-                            "Event Log Management": "https://www.offensive-security.com/metasploit-unleashed/event-log-management",
-                            "Interacting with the Registry": "https://www.offensive-security.com/metasploit-unleashed/interacting-registry",
+                            " The popping history of XSS": "https://thexssrat.medium.com/the-popping-history-of-xss-4122e34ac586",
+                            " Reflected Cross Site Scripting": "https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/07-Input_Validation_Testing/01-Testing_for_Reflected_Cross_Site_Scripting",
+                            " XXS HackerOne Report": "https://www.hacker101.com/sessions/xss",
+                            " From P5 to P2, from nothing to 1000+$": "https://medium.com/@mohameddaher/from-p5-to-p5-to-p2-from-nothing-to-1000-bxss-4dd26bc30a82",
+                            " Reflected XSS on Microsoft.com via Angular Js template injection": "https://infosecwriteups.com/reflected-xss-on-microsoft-com-via-angular-template-injection-2e26d80a7fd8",
+                            " From Self-XSS to Persistent XSS on Login Portal": "https://medium.com/@nnez/always-escalate-from-self-xss-to-persistent-xss-on-login-portal-54265b0adfd0",
+                            " Self XSS to Account Takeover": "https://medium.com/@Ch3ckM4te/self-xss-to-account-takeover-72c89775cf8f",
+                            " Blind Xss (A mind game to win the battle)": "https://medium.com/@dirtycoder0124/blind-xss-a-mind-game-to-win-the-battle-4fc67c524678?",
+                            " BugBounty | A Dom Xss": "https://jinone.github.io/bugbounty-a-dom-xss/",
+                            "How I turned Self XSS to Stored via CSRF": "https://medium.com/@abhishekY495/how-i-turned-self-xss-to-stored-via-csrf-d12eaaf59f2e",
+                            "XSS will never die": "https://medium.com/@Lekssik/xss-will-never-die-eb3584081a5f",
+                            "Cookie-based XSS exploitation": "https://medium.com/@ISecMax/cookie-based-xss-exploitation-2300-bug-bounty-story-9bc532ffa564",
+                            "Self XSS To Evil XSS": "https://saadahmedx.medium.com/self-xss-to-evil-xss-bcf2494a82a4",
+                            "CSRF Attack can lead to Stored XSS": "https://infosecwriteups.com/csrf-attack-can-lead-to-stored-xss-f40ba91f1e4f",
+                            "XSS by Tossing Cookies": "https://wesecureapp.com/blog/xss-by-tossing-cookies/",
+                            "Medium Content Spoofing Leads to XSS": "https://ahussam.me/Medium-content-spoofing-xss/",
+                            "3 Minutes & XSS!": "https://infosecwriteups.com/3-minutes-xss-71e3340ad66b",
+                            "The 2.5 BTC Stored XSS": "https://medium.com/@khaled.hassan/the-2-5-btc-stored-xss-f2f9393417f2",
                         },
+                        "XSS",
                     )
-                elif option == "8":
-                    os.system("clear")
-                    github = "Nmap (Network Mapper) is a network scanner created by Gordon Lyon (also known by his pseudonym Fyodor Vaskovich). Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses."
-                    template.template(
-                        "nmap",
-                        "nmap",
-                        github.strip(),
+                else:
+                    break
+
+        elif vulns == "2":
+            os.system("clear")
+            banner.main()
+            banner.attack("XXE - XML External Entity")
+            # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
+            github = "No tools available for this Vulnerability type.\nIt is recommended to test manually for XML External Entity (XXE) to get better understanding & results.\nCheck out the writeup section to to learn about XXE"
+            template.template(
+                "XXE",
+                "no-tools",
+                github.strip(),
+                {
+                    "XXE": "https://phonexicum.github.io/infosec/xxe.html",
+                    "XML External Entity Injection Processing (Intigriti)": "https://blog.intigriti.com/hackademy/xml-external-entity-processing-xxe/",
+                    "XML external entity (XXE) injection": "https://portswigger.net/web-security/xxe",
+                    "Exploitation: XXE Injection": "https://depthsecurity.com/blog/exploitation-xml-external-entity-xxe-injection",
+                    "XML External Entity Injection Processing (OWASP)": "https://owasp.org/www-community/vulnerabilities/XML_External_Entity_\(XXE\)_Processing",
+                    "XML External Entity Prevention Cheat Sheet": "https://cheatsheetseries.owasp.org/cheatsheets/XML_External_Entity_Prevention_Cheat_Sheet.html",
+                    "Testing for XML Injection": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/07-Input_Validation_Testing/07-Testing_for_XML_Injection",
+                    "XXE Injection Payload List": "https://github.com/payloadbox/xxe-injection-payload-list",
+                },
+            )
+
+        elif vulns == "3":
+            os.system("clear")
+            banner.main()
+            banner.attack("HTML Injection")
+            # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
+            github = "No tools available for this Vulnerability type.\nIt is recommended to test manually for HTML Injection to get better understanding & results.\nCheck out the writeup section to to learn about HTML Injection"
+            template.template(
+                "HTML Injection",
+                "no-tools",
+                github.strip(),
+                {
+                    "Comprehensive Guide on HTML Injection": "https://www.hackingarticles.in/comprehensive-guide-on-html-injection/",
+                    "HTML Injection(Unique Exploitation)": "https://medium.com/@pratiky054/html-injection-unique-exploitation-a5c3d4e6fed8",
+                    "Better Exfiltration via HTML Injection": "https://d0nut.medium.com/better-exfiltration-via-html-injection-31c72a2dae8b",
+                    "HTML injection via email confirmation!": "https://medium.com/cyberverse/got-easiest-bounty-with-html-injection-via-email-confirmation-b1b10575a105",
+                    "HTML Injection Tutorial": "https://www.softwaretestinghelp.com/html-injection-tutorial/",
+                },
+            )
+
+        elif vulns == "4":
+            while True:
+                os.system("clear")
+                banner.main()
+                banner.attack("SQL Injection")
+                # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
+                ask = vuln_options()
+                if ask == "1":
+                    while True:
+                        os.system("clear")
+                        banner.main()
+                        banner.attack("SQL Injection")
+                        des = "It is recommended to test manually for SQL Injection to get better understanding & results.\nCheck out the writeup section to to learn about SQL Injection"
+                        banner.description(des)
+                        list_tools = ["SqlMap", "go back"]
+                        for i in range(len(list_tools)):
+                            print(
+                                colors.options,
+                                f"{i+1}) {list_tools[i]}".title(),
+                                colors.reset,
+                            )
+                        option = input(
+                            f"\n {colors.select}Select an Option ->{colors.reset} "
+                        )
+                        if option == "1":
+                            print("\n[+] SQLMap")
+                            Exploitation_Tools.sqlmap()
+                        else:
+                            # print(f"{colors.red}[-]Wrong Input{colors.reset}")
+                            break
+                elif ask == "2":
+                    writeup.writeup(
                         {
-                            "Nmap Cheat-Sheet": "https://www.stationx.net/nmap-cheat-sheet/",
-                            "Official website": "https://nmap.org/ ",
-                            "Other resources": "https://linux.die.net/man/1/nmap",
+                            "SQL Injection Cheatsheet": "https://www.invicti.com/blog/web-security/sql-injection-cheat-sheet/",
+                            "SQL Injection payload lits": "https://infosecwriteups.com/sql-injection-payload-list-b97656cfd66b",
+                            "Admin Panel Accessed Via SQL Injection": "https://medium.com/@ratnadip1998/admin-panel-accessed-via-sql-injection-ezy-boooom-57dc60c2815f",
+                            "SQL Injection & Remote Code Execution": "https://shahjerry33.medium.com/sql-injection-remote-code-execution-double-p1-6038ca88a2ec",
+                            "Double quote Injection (Exploiting SQL Injection)": "https://medium.com/sud0root/bug-bounty-writeups-exploiting-sql-injection-vulnerability-20b019553716",
+                            "Blind (time-based) SQLi": "https://jspin.re/fileupload-blind-sqli/",
+                            "Exploiting “Google BigQuery” SQLI Vulnerability": "https://hackemall.live/index.php/2020/03/31/akamai-web-application-firewall-bypass-journey-exploiting-google-bigquery-sql-injection-vulnerability/",
                         },
-                    )
-                elif option == "9":
-                    os.system("clear")
-                    github = "The PenTesters Framework (PTF) is a Python script designed for Debian/Ubuntu/ArchLinux based distributions to create a similar and familiar distribution for Penetration Testing. PTF attempts to install all of your penetration testing tools (latest and greatest), compile them, build them, and make it so that you can install/update your distribution on any machine. Everything is organized in a fashion that is cohesive to the Penetration Testing Execution Standard (PTES) and eliminates a lot of things that are hardly used"
-                    template.template(
-                        "Penetration Testers Framework (PTF)",
-                        "./ptf",
-                        github.strip(),
-                        "no-writeups",
-                        method="github",
-                        github_install="git clone https://github.com/trustedsec/ptf.git && chmod +x ptf",
-                        github_check="ptf",
+                        "SQL Injection",
                     )
                 else:
                     break
 
-        elif option == "1":
+        elif vulns == "5":
+            os.system("clear")
+            banner.main()
+            banner.attack("Command Injection")
+            github = "No tools available for this Vulnerability type.\nIt is recommended to test manually for HTTP Req. Smuggling to get better understanding & results.\nCheck out the writeup section to to learn about HTTP Req. Smuggling"
+            template.template(
+                "Command Injection",
+                "no-tools",
+                github.strip(),
+                {
+
+                            "Breaking down — Command Injections": "https://infosecwriteups.com/breaking-down-command-injections-97d1029576",
+                            "Command Injection Payload List": "https://github.com/payloadbox/command-injection-payload-list",
+                            "Command Injection - PayloadAllTheThings": "https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Command%20Injection",
+                            "Comprehensive Guide on OS Command Injection": "https://www.hackingarticles.in/comprehensive-guide-on-os-command-injection/",
+                            "Command Injection - OWASP": "https://owasp.org/www-community/attacks/Command_Injection",
+                        },)
+
+        elif vulns == "6":
+            os.system("clear")
+            banner.main()
+            banner.attack("HTTP Request Smuggling")
+            github = "No tools available for this Vulnerability type.\nIt is recommended to test manually for HTTP Req. Smuggling to get better understanding & results.\nCheck out the writeup section to to learn about HTTP Req. Smuggling"
+            template.template(
+                "HTTP Request Smuggling",
+                "no-tools",
+                github.strip(),
+                {
+                    "HTTP request smuggling Explained": "https://infosecwriteups.com/http-request-smuggling-explained-and-exploited-part-0x1-89ce2956534f",
+                    "HTTP request smuggling": "https://portswigger.net/web-security/request-smuggling",
+                    "HTTP Request Smuggling - Cheat Sheet": "https://0xn3va.gitbook.io/cheat-sheets/web-application/http-request-smuggling",
+                    "Write up of two HTTP Requests Smuggling": "https://medium.com/@cc1h2e1/write-up-of-two-http-requests-smuggling-ff211656fe7d",
+                    "HTTP Request Smuggling - HackTricks": "https://book.hacktricks.xyz/pentesting-web/http-request-smuggling",
+                },
+            )
+
+        elif vulns == "7":
             os.system("clear")
             banner.main()
-            Cheat_sheet.cheat(
+            banner.attack("HTTP Parameter Pollution")
+            github = "No tools available for this Vulnerability type.\nIt is recommended to test manually for HTTP Parameter Pollution to get better understanding & results.\nCheck out the writeup section to to learn about HTTP Parameter Pollution"
+            template.template(
+                "HTTP Parameter Pollution",
+                "no-tools",
+                github.strip(),
                 {
-                    "Securing Applications with Better User Authorization": "https://medium.com/capital-one-tech/securing-applications-with-better-user-authorization-625ec07a7001",
-                    "Access Control": "https://portswigger.net/web-security/access-control",
-                    "Web Security: Authentication & Authorization": "https://coderstower.com/2020/03/23/web-security-authentication-authorization/",
-                    "Authentication & Authorization in Web Apps": "https://blog.jscrambler.com/authentication-authorization-in-web-apps",
-                    "Session IDs - OWASP": "https://www.cgisecurity.com/lib/SessionIDs.pdf",
-                    "JWT Authorization in Web Applications": "https://concisesoftware.com/blog/jwt-authorization-in-web-applications/",
-                    "Insecure Authorization": "https://www.appsealing.com/insecure-authorization/",
-                    "OAuth Vulnerabilities: Implementing Secure Authorization in Your Web Application": "https://medium.com/swlh/oauth-vulnerabilities-implementing-secure-authorization-in-your-web-application-3b9517b34798",
-                    "OWASP Top 10 - Broken Access Control": "https://owasp.org/Top10/A01_2021-Broken_Access_Control/",
-                    "Broken Authorization Vulnerability": "https://knowledge-base.secureflag.com/vulnerabilities/broken_authorization/broken_authorization_vulnerability.html",
-                    "OWASP Web Security Testing Guide - Authorization Testing": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/05-Authorization_Testing/README",
-                    "Web Authentication & Authorization": "https://www.slideshare.net/alex_pasaila/web-authentication-authorization-10930449",
-                    "Web Security - Authorization": "https://www3.rocketsoftware.com/rocketd3/support/documentation/Uniface/10/uniface/webApps/webSecurity/webSecurity_Authorization.htm",
-                    "Authorization Best Practices": "https://goteleport.com/blog/authorization-best-practices/",
-                    "Secure Your Web Application with Spring Security - Identify How to Secure Access to an App Using Authentication and Authorization": "https://openclassrooms.com/en/courses/5683681-secure-your-web-application-with-spring-security/6695816-identify-how-to-secure-access-to-an-app-using-authentication-and-authorization",
-                    "Preventing Broken Access Control": "https://crashtest-security.com/broken-access-control-prevention/",
-                    "Preventing Broken Access Control - The No. 1 Vulnerability in the OWASP Top 10 2021": "https://www.synack.com/blog/preventing-broken-access-control-the-no-1-vulnerability-in-the-owasp-top-10-2021/",
-                    "A Step-by-Step Guide to Broken Access Control Attacks": "https://www.polar.security/post/a-step-by-step-guide-to-broken-access-control-attacks",
-                    "Broken-Access-Control - packetlabs": "https://www.packetlabs.net/posts/broken-access-control",
-                    "Broken-Access-Control - qawerk": "https://qawerk.com/blog/broken-access-control/",
-                    "Testing for Broken Authentication in Web Apps": "https://www.section.io/engineering-education/testing-for-broken-authentication-in-web-apps/",
-                    "Broken-Access-Control (javascript) - Snyk": "https://learn.snyk.io/lessons/broken-access-control/javascript/",
-                    "JSON Web Tokens Decoder - JWT.IO": "https://jwt.io/",
-                    "Authorization Code Grant - Zine": "https://pbs.twimg.com/media/Et2T02KVcAEONV0?format=jpg&name=large",
-                    "OWASP API1: 2019 – Broken Object Level Authorization": "https://securityboulevard.com/2023/02/owasp-api1-2019-broken-object-level-authorization/",
-                    "BOLA: 3-Digit Bounty from Topcoder": "https://infosecwriteups.com/what-is-bola-3-digit-bounty-from-topcoder-a25e7fae0d64",
-                    "Broken Function Level Authorization (API Security) 0x2": "https://infosecwriteups.com/broken-function-level-authorization-api-security-0x2-23a6d7c1aa46",
-                    "A Deep Dive on the Most Critical API Vulnerability: BOLA": "https://inonst.medium.com/a-deep-dive-on-the-most-critical-api-vulnerability-bola-1342224ec3f2",
-                    "Broken Object Level Authorization (BOLA) - NordiAPIs": "https://nordicapis.com/what-is-broken-object-level-authorization-and-how-to-fix-it/",
-                    "Broken Function Level Authorization Leads to Disclosing PII Information of All Company Users": "https://webresearcher007.medium.com/broken-function-level-authorization-leads-to-disclosing-pii-information-of-all-company-users-35aee60b287b",
+                    "Behind the Scene : HTTP Parameter Pollution": "https://infosecwriteups.com/behind-the-scene-http-parameter-pollution-534b4fa2449c",
+                    "Testing for HTTP Parameter Pollution": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/07-Input_Validation_Testing/04-Testing_for_HTTP_Parameter_Pollution",
+                    "HTTP Parameter Pollution - HackTricks": "https://book.hacktricks.xyz/pentesting-web/parameter-pollution",
+                    "HTTP Parameter Pollution - Intigiti": "https://blog.intigriti.com/hackademy/http-parameter-pollution/",
+                    "Client-side HTTP parameter pollution": "https://portswigger.net/kb/issues/00501400_client-side-http-parameter-pollution-reflected",
                 },
-                "Authorization Write-UPS",
             )
 
-        elif option == "2":
-            print("\n[+] Burp Extensions")
+        elif vulns == "8":
+            while True:
+                os.system("clear")
+                banner.main()
+                banner.attack("Open Redirection")
+                # name,command,discription,writeups,link="",method="kali",github_install="",github_check=""
+                ask = vuln_options()
+                if ask == "1":
+                    while True:
+                        os.system("clear")
+                        banner.main()
+                        banner.attack("Open Redirection")
+                        des = "It is recommended to test manually for Open Redirection to get better understanding & results.\nCheck out the writeup section to to learn about Open Redirection"
+                        banner.description(des)
+                        list_tools = ["OpenRedireX", "Oralyzer", "go back"]
+                        for i in range(len(list_tools)):
+                            print(
+                                colors.options,
+                                f"{i+1}) {list_tools[i]}".title(),
+                                colors.reset,
+                            )
+                        option = input(
+                            f"\n {colors.select}Select an Option ->{colors.reset} "
+                        )
+                        if option == "1":
+                            print("\n[+] OpenRedireX")
+                            openredirex()                        
+                        elif option == "2":
+                            print("\n[+] Oralyzer")
+                            oralyzer()                        
+                        else:
+                            # print(f"{colors.red}[-]Wrong Input{colors.reset}")
+                            break
+                elif ask == "2":
+                    writeup.writeup(
+                        {
+                            "Open redirect - Improper validation of front-end provided redirect links": "https://learn.snyk.io/lessons/open-redirect/javascript/",
+                            "Open Redirect - Intigriti": "https://blog.intigriti.com/hackademy/open-redirect/",
+                            "Top 25 Open Redirect Bug Bounty Reports": "https://corneacristian.medium.com/top-25-open-redirect-bug-bounty-reports-5ffe11788794",
+                            "Open Redirect Payload List": "https://github.com/payloadbox/open-redirect-payload-list",
+                            "Open Redirect PayloadAllThethings": "https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Open%20Redirect",
+                            "Open-redirection leads to a bounty": "https://infosecwriteups.com/open-redirection-leads-to-a-bounty-d94029e11d17",
+                            "Strange Redirect (Fixed but no bounty)": "https://medium.com/@abhishekY495/strange-redirect-fixed-but-no-bounty-54425aea7f19",
+                            "Open Redirect To XSS on Login Page": "https://nassimchami.medium.com/1st-bug-bounty-writeup-open-redirect-to-xss-on-login-page-313221da2879",
+                        },
+                        "Open Redirection",
+                    )
+                else:
+                    break
+
+        elif vulns == "9":
             os.system("clear")
             banner.main()
-            Cheat_sheet.cheat(
+            banner.attack("LFI - Local File Inclusion")
+            github = "No tools available for this Vulnerability type.\nIt is recommended to test manually for LFI to get better understanding & results.\nCheck out the writeup section to to learn about Local File Inclusion"
+            template.template(
+                "LFI",
+                "no-tools",
+                github.strip(),
                 {
-                    "Portswigger - Auth Analyzer": "https://portswigger.net/bappstore/7db49799266c4f85866f54d9eab82c89",
-                    "Github - Auth Analyzer": "https://github.com/simioni87/auth_analyzer",
-                    "Portswigger - AutoRepeater": "https://portswigger.net/bappstore/f89f2837c22c4ab4b772f31522647ed8",
-                    "Github - AutoRepeater": "https://github.com/nccgroup/AutoRepeater",
-                    "Github - Burp-SessionAuthTool": "https://github.com/thomaspatzke/Burp-SessionAuthTool",
-                    "Github - BurpAuthzPlugin": "https://github.com/wuntee/BurpAuthzPlugin",
-                    "Github - Burp-uuid": "https://github.com/silentsignal/burp-uuid",
-                    "Github - Autorize": "https://github.com/Quitten/Autorize",
-                    "Github - AuthMatrix": "https://github.com/SecurityInnovation/AuthMatrix",
-                    "Github - Burplay": "https://github.com/SpiderLabs/burplay",
-                    "Github - Param-Miner": "https://github.com/PortSwigger/param-miner",
-                    "Portswigger - SAML Raider": "https://portswigger.net/bappstore/c61cfa893bb14db4b01775554f7b802e",
-                    "Portswigger - Authz": "https://portswigger.net/bappstore/4316cc18ac5f434884b2089831c7d19e",
+                    "LFI Attack Examples": "https://brightsec.com/blog/lfi-attack-real-life-attacks-and-attack-examples/",
+                    "What is Local File Inclusion (LFI)?": "https://www.acunetix.com/blog/articles/local-file-inclusion-lfi/",
+                    "Testing for Local File Inclusion": "https://wiki.owasp.org/index.php/Testing_for_Local_File_Inclusion",
+                    "CVV #1: Local File Inclusion": "https://infosecwriteups.com/cvv-1-local-file-inclusion-ebc48e0e479a",
                 },
-                "Authorization Burp Extensions",
             )
 
         else:
             return
 
 
+def vuln_options():
+    print(f"{colors.options}1) Tools")
+    print(f"2) Write-ups")
+    print(f"3) Go Back")
+    try:
+        ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+    except KeyboardInterrupt:
+        return
+    return ask
+
+
 def github_getting_text(link, selector, indexvalue):
     print("Please Wait....\r", end="")
     URL = link
     try:
         r = requests.get(URL)
         soup = BeautifulSoup(r.content, "html.parser")
         paras = soup.select(selector)
         # check index value from test file
         return paras[indexvalue].text
     except:
         return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
 
+def oralyzer():
+    github = github_getting_text(
+                                "https://github.com/r0075h3ll/Oralyzer",
+                                "p[dir=auto]",
+                                0,
+                            )
+    template.template(
+                                "Oralyzer",
+                                "python3 oralyzer.py -h",
+                                github.strip(),
+                                {
+                                    "Oralyzer : Linux Tool To Identify Open Redirection": "https://www.geeksforgeeks.org/oralyzer-linux-tool-to-identify-open-redirection/",
+                                    "Oralyzer – A Automatic Open Redirection Vulnerability Finder": "https://secnhack.in/oralyzer-a-automatic-open-redirection-vulnerability-finder/",
+                                    "Oralyzer : Tool To Identify Open Redirection": "https://kalilinuxtutorials.com/oralyzer",
+                                    "Oralyzer – Tool To Identify Open Redirection": "https://pentesttools.net/oralyzer-tool-to-identify-open-redirection/",
+                                },
+                                link="https://github.com/r0075h3ll/Oralyzer.git",
+                                method="github",
+                                github_install="git clone https://github.com/r0075h3ll/Oralyzer.git && pip3 install -r requirements.txt",
+                                github_check="Oralyzer",
+                            )
+def openredirex():
+    github = "Open redirect is a security defect in an app or a web page that causes it to fail to properly authenticate URLs. When apps and web pages have requests for URLs, they are supposed to prove that those URLs are part of the expected page’s domain."
+    template.template(
+                                "OpenRedireX",
+                                "python3 openredirex.py -h",
+                                github.strip(),
+                                {
+                                    "OpenRedireX – Open Redirection Vulnerability Finder Tool in Linux": "https://www.geeksforgeeks.org/openredirex-open-redirection-vulnerability-finder-tool-in-linux/",
+                                    "OpenRedireX – A Open Redirection Vulnerability Finder": "https://secnhack.in/openredirex-a-open-redirection-vulnerability-finder/",
+                                    "Open Redirect Scanner with Uber.com": "https://infosecwriteups.com/open-redirect-scanner-c72cd60d0bf",
+                                    "OpenRedireX – Asynchronous Open redirect Fuzzer for Humans": "https://pentesttools.net/openredirex-asynchronous-open-redirect-fuzzer-for-humans/",
+                                },
+                                link="https://github.com/devanshbatham/OpenRedireX",
+                                method="github",
+                                github_install="git clone https://github.com/devanshbatham/OpenRedireX.git",
+                                github_check="OpenRedireX",
+                            )
+
+def xsser():
+    github = github_getting_text(
+                                "https://www.kali.org/tools/xsser/", "p", 3
+                            )
+    template.template(
+                                "xsser",
+                                "xsser -h",
+                                github.strip(),
+                                {
+                                    "Detecting and Exploiting XSS Injections using XSSer Tool": "https://securityxploded.com/detecting-exploiting-xss-using-xsser-tool.php",
+                                    "XSSer - Detect and Exploit XSS vulnerabilities": "https://gbhackers.com/xsser-automated-framework-detectexploit-report-xss-vulnerabilities/",
+                                    "XSSer- Cross Site Scripting Penetration Tool": "https://www.ehacking.net/2011/02/xsser-cross-site-scripting-penetration.html",
+                                },
+                            )
+
+def xsstrike():
+    github = github_getting_text(
+                                "https://github.com/s0md3v/XSStrike", "p[dir=auto]", 3
+                            )
+    template.template(
+                                "XSStrike",
+                                "python3 xsstrike.py -h",
+                                github.strip(),
+                                {
+                                    "XSStrike – Hunting for low-hanging fruits in Kali Linux": "https://www.geeksforgeeks.org/xsstrike-hunting-for-low-hanging-fruits-in-kali-linux/",
+                                    "Hacker tools: XSStrike – Hunting for low-hanging fruits.": "https://blog.intigriti.com/2021/06/29/hacker-tools-xsstrike-hunting-for-low-hanging-fruits/",
+                                    "XSStrike Usage Example (v3.x)": "https://www.cyberpunk.rs/xsstrike-usage-example-v3-x",
+                                    "Advanced XSS Detection Suite – XSStrike": "https://www.cyberpunk.rs/advanced-xss-detection-suite-xsstrike",
+                                },
+                                link="https://github.com/s0md3v/XSStrike.git",
+                                method="github",
+                                github_install="git clone https://github.com/s0md3v/XSStrike.git && cd XSStrike && chmod +x xsstrike.py",
+                                github_check="XSStrike",
+                            )
+def dalfox():
+    github = github_getting_text(
+                                "https://github.com/hahwul/dalfox/blob/main/README.md", 'p', 1
+                            )
+    template.template(
+                                "dalfox",
+                                "dalfox",
+                                github.strip(),
+                                {
+                                    "DalFox - Parameter Analysis and XSS Scanning tool": "https://www.geeksforgeeks.org/dalfox-parameter-analysis-and-xss-scanning-tool/",
+                                    "Automating XSS using Dalfox, GF and Waybackurls": "https://infosecwriteups.com/automating-xss-using-dalfox-gf-and-waybackurls-bc6de16a5c75",
+                                    "Dalfox - Hacker Tools: XSS Scanning Made Easy": "https://blog.intigriti.com/2021/09/14/hacker-tools-dalfox/",
+                                    "Offensive Security Tool: Dalfox": "https://www.blackhatethicalhacking.com/tools/dalfox",
+                                },
+                                link="github.com/hahwul/dalfox/v2@latest",
+                                method="go",
+                            )
 
 if __name__ == "__main__":
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Exploitation_Tools.py` & `cyberonix-3.0.0/cyberonix/main/tools/Exploitation_Tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,122 @@
-from cyberonix.main.tools import banner,colors,template
+from cyberonix.main.tools import banner, colors, template
 import os
 import requests
 from bs4 import BeautifulSoup
 
-#main function
+# main function
+
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Exploitation Tools")
-        list_attacks=["Metasploit","CrackMapExec","Searchsploit","BeEF","RouterSploit","Sqlmap","Armitage","Commix","Go Back"]
+        list_attacks = [" Metasploit\t\t(Recommended)", " CrackMapExec", " Searchsploit\t(Recommended)", " BeEF\t\t(Recommended)",
+                        " RouterSploit", " Sqlmap\t\t(Recommended)", " Seclists\t\t(Recommended)", " Armitage", " Go Back"]
         for i in range(len(list_attacks)):
-                print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option=="0":
+            return
+        if option == "1":
             print("\n[+] Metasploit-Framework")
-            os.system("clear")
-            # name,command,discription,writeup,link=True,method="kali",github_install="",github_check=True
-            github = "The Metasploit Framework is an open-source tool for developing and executing exploit code against a remote target machine. It can be used to test the security of a computer system by finding and exploiting vulnerabilities. The framework includes a large collection of exploit modules, as well as various tools for payload generation, post-exploitation, and more. It can be used by security professionals for penetration testing, as well as by attackers for malicious purposes."
-            template.template("metasploit-framework","msfconsole",github.strip(),{"Msf-Community-Post-Exploitation":"https://www.offensive-security.com/metasploit-unleashed/msf-community-post-exploitation","Post Exploitation In Linux With Metasploit":"https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/","Privilege Escalation (Metasploit Unleashed)":"https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/","Post Exploitation Metasploit Modules (Reference)":"https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference","PSExec Pass the Hash (Horizontal Escalation)":"https://www.offensive-security.com/metasploit-unleashed/psexec-pass-hash/","ms10_002_aurora (Vertical Escalation)":"https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/","ms10_002_aurora (Horizontal Escalation)":"https://www.offensive-security.com/metasploit-unleashed/pivoting/ ","jtr_crack_fast (Hash Cracking)":"https://www.offensive-security.com/metasploit-unleashed/john-ripper/","warftpd_165_user (Keylogging)":"https://www.offensive-security.com/metasploit-unleashed/keylogging/","3proxy (Backdoor)":"https://www.offensive-security.com/metasploit-unleashed/meterpreter-backdoor/","persistence.rb (Persistent Backdoor)":"https://www.offensive-security.com/metasploit-unleashed/meterpreter-service/","Enabling Remote Desktop":"https://www.offensive-security.com/metasploit-unleashed/enabling-remote-desktop/","Post Exploitation in Linux with Metasploit":"https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/","Post Exploitation Metasploit Modules Reference":"https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference/","Hack Like Pro: Kill and Disable Antivirus Software Remote PC":"https://null-byte.wonderhowto.com/how-to/hack-like-pro-kill-and-disable-antivirus-software-remote-pc-0141906/","Armitage Post Exploitation":"https://www.offensive-security.com/metasploit-unleashed/armitage-post-exploitation/","Setup Armitage as a Command & Control Framework for Free":"https://infosecwriteups.com/setup-armitage-as-a-command-control-c2-framework-for-free-bae590064817","Event Log Management":"https://www.offensive-security.com/metasploit-unleashed/event-log-management","Interacting with the Registry":"https://www.offensive-security.com/metasploit-unleashed/interacting-registry"})        
-        elif option=="1":
-            print("\n[+] CrackMapExec")
-            os.system("clear")
-            github="CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks. Built with stealth in mind, CME follows the concept of Living off the Land : abusing built-in Active Directory features/protocols to achieve it's functionality and allowing it to evade most endpoint protection/IDS/IPS solutions."
-            template.template("crackmapexec","crackmapexec",github.strip(),{"CrackMapExec in Kali Linux":"https://www.kali.org/tools/crackmapexec/","How to Use CrackMapExec":"https://blog.netwrix.com/2022/12/16/crackmapexec_tutorial/","Lateral Movement on Active Directory: CrackMapExec":"https://www.hackingarticles.in/lateral-moment-on-active-directory-crackmapexec/","CrackMapExec Cheat sheet":"https://cheatsheet.haax.fr/windows-systems/exploitation/crackmapexec/"})
-        elif option=="2":
+            metasploit()
+        elif option == "2":
+            print("\n[+] crackmapexec")
+            crackmapexec()
+        elif option == "3":
             print("\n[+] Searchsploit")
-            os.system("clear")
-            github = "The Exploit Database is an archive of public exploits and corresponding vulnerable software, developed for use by penetration testers and vulnerability researchers. Its aim is to serve as the most comprehensive collection of exploits, shellcode and papers gathered through direct submissions, mailing lists, and other public sources, and present them in a freely-available and easy-to-navigate database."
-            template.template("exploitdb","searchsploit",github.strip(),{"How to install Searchsploit":"https://www.exploit-db.com/searchsploit","How to Use SearchSploit":"https://www.kali.org/tools/exploitdb/#searchsploit","Finding Exploit offline using Searchsploit in Kali Linux":"https://www.geeksforgeeks.org/finding-exploit-offline-using-searchsploit-in-kali-linux/","How to easy find exploits with Searchsploit on Linux":"https://medium.com/@hninja049/how-to-easy-find-exploits-with-searchsploit-on-linux-4ce0b82c82fd"})
-        elif option=="3":
-            print("\n[+] BeEF")
-            os.system("clear")
-            github_p1=github_getting_text("https://github.com/beefproject/beef",'p[dir="auto"]',2)
-            github_p2=github_getting_text("https://github.com/beefproject/beef",'p[dir="auto"]',3)
-            github=github_p1+github_p2
-            template.template("beef-xss","beef-xss",github.strip(),{"BEeF Hacking Framework Tutorial [5 Easy Steps]":"https://www.golinuxcloud.com/beef-hacking-framework-tutorial/","Browser Exploitation and Advanced Threat Actors: An Overview of BeEF":"https://medium.com/@andrearebora/browser-exploitation-and-advanced-threat-actors-an-overview-of-beef-bb907a5b73fa","Hooking victims to Browser Exploitation Framework (BeEF) using Reflected and Stored XSS.":"https://medium.com/@secureica/hooking-victims-to-browser-exploitation-framework-beef-using-reflected-and-stored-xss-859266c5a00a","Hijacking Browser with BeEF Framework":"https://medium.com/@krunalkumarpatel/hijacking-browser-with-beef-framework-bea784c03149"})
-        elif option=="4":
+            searchsploit()
+        elif option == "4":
+            print("\n[+] beef")
+            beef()
+        elif option == "5":
             print("\n[+] RouterSploit")
-            os.system("clear")
-            github = "The RouterSploit Framework is an open-source exploitation framework dedicated to embedded devices. It consists of various modules that aid penetration testing operations: exploits - modules that take advantage of identified vulnerabilities. creds - modules designed to test credentials against network services."
-            template.template("routersploit","routersploit",github.strip(),{"How to Use Routersploit":"https://www.kali.org/tools/routersploit/","Routersploit Tutorial":"https://kalitut.com/routersploit/","RouterSploit User Manual":"https://miloserdov.org/?p=1527"})
-        elif option=="5":
-            print("\n[+] Sqlmap")
-            os.system("clear")
-            github="sqlmap is an open source penetration testing tool that automates the process of detecting and exploiting SQL injection flaws and taking over of database servers. It comes with a powerful detection engine, many niche features for the ultimate penetration tester and a broad range of switches lasting from database fingerprinting, over data fetching from the database, to accessing the underlying file system and executing commands on the operating system via out-of-band connections"
-            template.template("sqlmap","sqlmap -h",github.strip(),{"Usage Of Sqlmap":"https://github.com/sqlmapproject/sqlmap/wiki/Usage","How to use SQLMAP to test a website for SQL Injection vulnerability":"https://www.geeksforgeeks.org/use-sqlmap-test-website-sql-injection-vulnerability/","How to Use SQLMap to Find Database Vulnerabilities":"https://www.freecodecamp.org/news/how-to-protect-against-sql-injection-attacks/","SQLMap - Cheetsheat":"https://book.hacktricks.xyz/pentesting-web/sql-injection/sqlmap"})
-        elif option=="6":
+            routersploit()            
+        elif option == "6":
+            print("\n[+] sqlmap")
+            sqlmap()
+        elif option == "7":
+            print("\n[+] seclists")
+            seclists()    
+        elif option == "8":
             print("\n[+] Armitage")
-            os.system("clear")
-            github = "Armitage is a fantastic Java-based GUI front-end for the Metasploit Framework developed by Raphael Mudge. Its goal is to help security professionals better understand hacking and help them realize the power and potential of Metasploit."
-            template.template("armitage","armitage",github.strip(),{"How to Install Armitage on Kali Linux":"https://linuxhint.com/install-armitage-kali-linux/","Armitage Setup":"https://www.offensive-security.com/metasploit-unleashed/armitage-setup/","Hacking With Armitage on Kali Linux / Backtrack ":"https://www.amirootyet.com/post/hacking-with-armitage-on-kali-linux/"})
-        elif option=="7":
-            print("\n[+] Commix")
-            os.system("clear")
-            github="Commix (short for [comm]and [i]njection e[x]ploiter) is an open source penetration testing tool, written by Anastasios Stasinopoulos (@ancst), that automates the detection and exploitation of command injection vulnerabilities."
-            template.template("commix","commix -h",github.strip(),{"Commix Usage Example":"https://www.kali.org/tools/commix/","OS Command Injection and Exploitation Tool":"https://www.geeksforgeeks.org/commix-os-command-injection-and-exploitation-tool/","An automated tool for command injection":" an automated tool for command injection"})
+            armitage()        
         else:
             return
-def github_getting_text(link,selector,indexvalue):
-    print("Please Wait....\r",end="")
+
+
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
     URL = link
     try:
+        if selector=="p" and "github" in link:
+            selector="p[dir=auto]"
         r = requests.get(URL)
         soup = BeautifulSoup(r.content, 'html.parser')
         paras = soup.select(selector)
-        #check index value from test file
+        # check index value from test file
         return paras[indexvalue].text
     except:
         return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
 
-if __name__=='__main__':
+
+def searchsploit():
+    github = "The Exploit Database is an archive of public exploits and corresponding vulnerable software, developed for use by penetration testers and vulnerability researchers. Its aim is to serve as the most comprehensive collection of exploits, shellcode and papers gathered through direct submissions, mailing lists, and other public sources, and present them in a freely-available and easy-to-navigate database."
+    template.template("exploitdb", "searchsploit", github.strip(), {"How to install Searchsploit": "https://www.exploit-db.com/searchsploit", "How to Use SearchSploit": "https://www.kali.org/tools/exploitdb/#searchsploit", "Finding Exploit offline using Searchsploit in Kali Linux":
+                              "https://www.geeksforgeeks.org/finding-exploit-offline-using-searchsploit-in-kali-linux/", "How to easy find exploits with Searchsploit on Linux": "https://medium.com/@hninja049/how-to-easy-find-exploits-with-searchsploit-on-linux-4ce0b82c82fd"})
+        
+def routersploit():
+    os.system("clear")
+    github = "The RouterSploit Framework is an open-source exploitation framework dedicated to embedded devices. It consists of various modules that aid penetration testing operations: exploits - modules that take advantage of identified vulnerabilities. creds - modules designed to test credentials against network services."
+    template.template("routersploit", "routersploit", github.strip(), {"How to Use Routersploit": "https://www.kali.org/tools/routersploit/",
+                              "Routersploit Tutorial": "https://kalitut.com/routersploit/", "RouterSploit User Manual": "https://miloserdov.org/?p=1527"})
+        
+def seclists():
+    os.system("clear")
+    github = github_getting_text(
+            "https://github.com/danielmiessler/SecLists", 'p', 1)
+    template.template("seclists", "seclists", github.strip(), {
+                              "Using SecLists for Penetration Testing": "https://www.varutra.com/using-seclists-for-penetration-testing/"},)
+        
+def armitage():
+    os.system("clear")
+    github = "Armitage is a fantastic Java-based GUI front-end for the Metasploit Framework developed by Raphael Mudge. Its goal is to help security professionals better understand hacking and help them realize the power and potential of Metasploit."
+    template.template("armitage", "armitage", github.strip(), {"How to Install Armitage on Kali Linux": "https://linuxhint.com/install-armitage-kali-linux/",
+                              "Armitage Setup": "https://www.offensive-security.com/metasploit-unleashed/armitage-setup/", "Hacking With Armitage on Kali Linux / Backtrack ": "https://www.amirootyet.com/post/hacking-with-armitage-on-kali-linux/"})
+        
+def metasploit():
+    os.system("clear")
+    # name,command,discription,writeup,link=True,method="kali",github_install="",github_check=True
+    github = "The Metasploit Framework is an open-source tool for developing and executing exploit code against a remote target machine. It can be used to test the security of a computer system by finding and exploiting vulnerabilities. The framework includes a large collection of exploit modules, as well as various tools for payload generation, post-exploitation, and more. It can be used by security professionals for penetration testing, as well as by attackers for malicious purposes."
+    template.template("metasploit-framework", "msfconsole", github.strip(), {" Msf-Community-Post-Exploitation": "https://www.offensive-security.com/metasploit-unleashed/msf-community-post-exploitation", " Post Exploitation In Linux With Metasploit": "https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/", " Privilege Escalation (Metasploit Unleashed)": "https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/", " Post Exploitation Metasploit Modules (Reference)": "https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference", " PSExec Pass the Hash (Horizontal Escalation)": "https://www.offensive-security.com/metasploit-unleashed/psexec-pass-hash/", " ms10_002_aurora (Vertical Escalation)": "https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/", " ms10_002_aurora (Horizontal Escalation)": "https://www.offensive-security.com/metasploit-unleashed/pivoting/ ", " jtr_crack_fast (Hash Cracking)": "https://www.offensive-security.com/metasploit-unleashed/john-ripper/", " warftpd_165_user (Keylogging)":
+                      "https://www.offensive-security.com/metasploit-unleashed/keylogging/", "3proxy (Backdoor)": "https://www.offensive-security.com/metasploit-unleashed/meterpreter-backdoor/", "persistence.rb (Persistent Backdoor)": "https://www.offensive-security.com/metasploit-unleashed/meterpreter-service/", "Enabling Remote Desktop": "https://www.offensive-security.com/metasploit-unleashed/enabling-remote-desktop/", "Hack Like Pro: Kill and Disable Antivirus Software Remote PC": "https://null-byte.wonderhowto.com/how-to/hack-like-pro-kill-and-disable-antivirus-software-remote-pc-0141906/", "Armitage Post Exploitation": "https://www.offensive-security.com/metasploit-unleashed/armitage-post-exploitation/", "Setup Armitage as a Command & Control Framework for Free": "https://infosecwriteups.com/setup-armitage-as-a-command-control-c2-framework-for-free-bae590064817", "Event Log Management": "https://www.offensive-security.com/metasploit-unleashed/event-log-management", "Interacting with the Registry": "https://www.offensive-security.com/metasploit-unleashed/interacting-registry"})
+
+
+def sqlmap():
+    os.system("clear")
+    github = "sqlmap is an open source penetration testing tool that automates the process of detecting and exploiting SQL injection flaws and taking over of database servers. It comes with a powerful detection engine, many niche features for the ultimate penetration tester and a broad range of switches lasting from database fingerprinting, over data fetching from the database, to accessing the underlying file system and executing commands on the operating system via out-of-band connections"
+    template.template("sqlmap", "sqlmap -h", github.strip(), {"Usage Of Sqlmap": "https://github.com/sqlmapproject/sqlmap/wiki/Usage", "How to use SQLMAP to test a website for SQL Injection vulnerability": "https://www.geeksforgeeks.org/use-sqlmap-test-website-sql-injection-vulnerability/",
+                      "How to Use SQLMap to Find Database Vulnerabilities": "https://www.freecodecamp.org/news/how-to-protect-against-sql-injection-attacks/", "SQLMap - Cheetsheat": "https://book.hacktricks.xyz/pentesting-web/sql-injection/sqlmap"})
+
+
+def crackmapexec():
+    os.system("clear")
+    github = "CrackMapExec (a.k.a CME) is a post-exploitation tool that helps automate assessing the security of large Active Directory networks. Built with stealth in mind, CME follows the concept of Living off the Land : abusing built-in Active Directory features/protocols to achieve it's functionality and allowing it to evade most endpoint protection/IDS/IPS solutions."
+    template.template("crackmapexec", "crackmapexec", github.strip(), {"CrackMapExec in Kali Linux": "https://www.kali.org/tools/crackmapexec/", "How to Use CrackMapExec": "https://bond-o.medium.com/crackmapexec-basics-839ef6180940",
+                      "Lateral Movement on Active Directory: CrackMapExec": "https://www.hackingarticles.in/lateral-moment-on-active-directory-crackmapexec/", "CrackMapExec Cheat sheet": "https://cheatsheet.haax.fr/windows-systems/exploitation/crackmapexec/"})
+
+
+def beef():
+    os.system("clear")
+    github_p1 = github_getting_text("https://beefproject.com/", 'p', 0)
+    github_p2 = github_getting_text("https://beefproject.com/", 'p', 1)
+    github = github_p1.strip().replace("\n", "").replace("\t", "")+github_p2.strip().replace("\n", "").replace("\t", "")
+    template.template("beef-xss", "beef-xss", github.strip(), {"BEeF Hacking Framework Tutorial [5 Easy Steps]": "https://www.golinuxcloud.com/beef-hacking-framework-tutorial/", "Browser Exploitation and Advanced Threat Actors: An Overview of BeEF": "https://medium.com/@andrearebora/browser-exploitation-and-advanced-threat-actors-an-overview-of-beef-bb907a5b73fa",
+                      "Hooking victims to Browser Exploitation Framework (BeEF) using Reflected and Stored XSS.": "https://medium.com/@secureica/hooking-victims-to-browser-exploitation-framework-beef-using-reflected-and-stored-xss-859266c5a00a", "Hijacking Browser with BeEF Framework": "https://medium.com/@krunalkumarpatel/hijacking-browser-with-beef-framework-bea784c03149"})
+
+
+if __name__ == '__main__':
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/File_Upload.py` & `cyberonix-3.0.0/cyberonix/main/tools/File_Upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,50 @@
 from cyberonix.main.tools import banner, template, colors, writeup
-from cyberonix.main import Cheat_sheet
 import os
 import requests
 from bs4 import BeautifulSoup
 
 
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack(f"File Upload")
         list_attacks = ["Tools", "Writeups", "Go Back"]
         for i in range(len(list_attacks)):
             print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
+            return
         if option == "1":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack(f"Tools")
-                list_tools = ["fuxploider", "Upload Scanner", "go back"]
+                list_tools = ["fuxploider","go back"]
                 for i in range(len(list_tools)):
                     print(
                         colors.options, f"{i+1}) {list_tools[i]}".title(), colors.reset
                     )
                 try:
                     option = input(f"\n {colors.select}Select an Option ->{colors.reset} ")
                 except KeyboardInterrupt:
-                    template.exit_program()
+                    return
                 if option == "1":
-                    github = github_getting_text(
-                        "https://github.com/almandin/fuxploider", 'p[dir="auto"]', 1
-                    )
-                    template.template(
-                        "flxploider",
-                        "python3 fuxploider.py -h",
-                        github,
-                        "no-writeups",
-                        link="https://github.com/almandin/fuxploider.git",
-                        method="github",
-                        github_install="git clone https://github.com/almandin/fuxploider.git && python3 -m pip install -r fuxploider/requirements.txt ",
-                        github_check="fuxploider"
-                    )
-                elif option == "2":
-                    github = github_getting_text(
-                        "https://github.com/portswigger/upload-scanner", "p[dir=auto]", 0
-                    )
-                    template.template(
-                        "Upload Scanner",
-                        "https://github.com/portswigger/upload-scanner",
-                        github,
-                        "no-writeups",
-                        method="browser"
-                    )
-
+                    print("\n[+] Fuxploider")
+                    fuxploider()
                 else:
                     break
         elif option == "2":
             # writeup.writeup({"Test Upload of Unexpected File Types":"https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/10-Business_Logic_Testing/08-Test_Upload_of_Unexpected_File_Types","What is Unrestricted File Upload?":"https://www.aptive.co.uk/blog/unrestricted-file-upload-testing/","File Upload General Methodology":"https://book.hacktricks.xyz/pentesting-web/file-upload","File upload vulnerabilities":"https://portswigger.net/web-security/file-upload","File Upload Attacks (Part 2)":"https://blog.yeswehack.com/yeswerhackers/file-upload-attacks-part-2/","Hunting for Bugs in File Upload Feature:":"https://sm4rty.medium.com/hunting-for-bugs-in-file-upload-feature-c3b364fb01ba","How I abused the file upload function to get a high severity vulnerability in Bug Bounty":"https://infosecwriteups.com/how-i-abused-the-file-upload-function-to-get-a-high-severity-vulnerability-in-bug-bounty-7cdcf349080b","Directory Traversal via PHP Multi-File Uploads":"https://nealpoole.com/blog/tag/file-upload/"},"Writups")
             writeup.writeup(
                 {
+                    "Upload Scanner Website":"https://github.com/portswigger/upload-scanner",
                     "Test Upload of Unexpected File Types": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/10-Business_Logic_Testing/08-Test_Upload_of_Unexpected_File_Types",
                     "What is Unrestricted File Upload?": "https://www.aptive.co.uk/blog/unrestricted-file-upload-testing/",
                     "File Upload General Methodology": "https://book.hacktricks.xyz/pentesting-web/file-upload",
                     "File upload vulnerabilities": "https://portswigger.net/web-security/file-upload",
                     "File Upload Attacks (Part 2)": "https://blog.yeswehack.com/yeswerhackers/file-upload-attacks-part-2/",
                     "Hunting for Bugs in File Upload Feature:": "https://sm4rty.medium.com/hunting-for-bugs-in-file-upload-feature-c3b364fb01ba",
                     "How I abused the file upload function to get a high severity vulnerability in Bug Bounty": "https://infosecwriteups.com/how-i-abused-the-file-upload-function-to-get-a-high-severity-vulnerability-in-bug-bounty-7cdcf349080b",
@@ -87,11 +65,24 @@
         soup = BeautifulSoup(r.content, "html.parser")
         paras = soup.select(selector)
         # check index value from test file
         return paras[indexvalue].text
     except:
         return f"{colors.red}NotLloaded Because No Internet Connection{colors.reset}"
 
-
+def fuxploider():
+    os.system("clear")
+    github = "Fuxploider is an open source penetration testing tool that automates the process of detecting and exploiting file upload forms flaws. This tool is able to detect the file types allowed to be uploaded and is able to detect which technique will work best to upload web shells or any malicious file on the desired web server."
+    template.template(
+                        "fuxploider",
+                        "python3 fuxploider.py -h",
+                        github,
+                        "no-writeups",
+                        link="https://github.com/almandin/fuxploider.git",
+                        method="github",
+                        github_install="git clone https://github.com/almandin/fuxploider.git && python3 -m pip install -r fuxploider/requirements.txt ",
+                        github_check="fuxploider"
+                    )
+                
 if __name__ == "__main__":
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Password_Hacking.py` & `cyberonix-3.0.0/cyberonix/main/tools/Password_Hacking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,196 +1,292 @@
 import os
-from cyberonix.main.tools import template,banner,colors
+from cyberonix.main.tools import template, banner, colors, WEB_Application_Analysis,Configuration_Management
+
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Password Hacking")
-        list_root_attacks = ["Brute Force Attacks", "Dictionary Attacks", "Rainbow Table Attack", "Wordlist Generator","Phishing Attacks", "Keylogger Attacks", "go back"]
+        list_root_attacks = ["Useful Sites","Brute Force Attacks", "Dictionary Attacks", "Rainbow Table Attack",
+                             "Wordlist Generator", "Phishing Attacks", "Keylogger Attacks", "go back"]
         for i in range(len(list_root_attacks)):
-            print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+            print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
+            return
+        if option == "1":
+            print("\n[+] Useful Websites")
+            os.system("clear")
+            template.template("Useful Websites", "no-tools", 'This is website for information gathering', {
+                "Salted Password Hashing - Doing it Right": "https://crackstation.net/hashing-security.htm", 
+                "CrackStation's Password Cracking Dictionary":"https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm", 
+                "Wordlist Download": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm",
+                "CyberChef - A must have security tool": "https://www.youtube.com/watch?v=rT_CjwKN380",
+                "CyberChef – Data decoding made easy": "https://www.csnp.org/post/cyberchef-data-decoding-made-easy",
+
+
+            })
+        elif option == "2":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Brute Force")
                 banner.description("A brute force attack is a method of attempting to gain unauthorized access to a computer or network by systematically trying every possible combination of charactersor words in order to discover a valid password or key. In a 'pure' brute force attack, all possible combinations are tried one after another until the correct one is found. This can be a time-consuming process, but it is often effective because many people use easily-guessed passwords.")
-                list_root_attacks = ["Hashcat", "John The Ripper", "Hydra", "Johnny (GUI John)","CrackStation (Website)", "CyberChef (Website)", "go back"]
+                list_root_attacks = ["Hashcat\t\t(Recommended)", "John The Ripper\t(Recommended)", "Hydra\t\t(Recommended)", "Dirsearch",
+                                     "Johnny (GUI John)","Dirbuster", "Reaver", "go back"]
                 for i in range(len(list_root_attacks)):
-                    print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+                    print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
-                    ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+                    ask = input(
+                        f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
-                    template.exit_program()
-                if ask == "0":
-                    github = "Hashcat is an open-source password cracking tool that can perform dictionary, brute force and combination attacks, it uses the power of GPUs to accelerate the cracking process, supports a wide variety of hashing algorithms and it can run on Windows, Linux and macOS. It's widely used for password recovery, security testing and penetration testing."
-                    template.template("hashcat", "hashcat -h", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/","How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
-                elif ask == "1":
-                    github = "John the Ripper is a free and open-source password cracking software tool. It can be run on a variety of operating systems, including Windows, macOS, and Linux. It uses a combination of wordlists and rules to try and guess the password for a given hash or file, and can support a variety of different hash types, including those used for Unix and Windows passwords. John the Ripper is commonly used by security professionals and system administrators to audit the security of their systems and detect weak or easily guessable passwords."
-                    template.template("john", "john", github.strip(), {"Open-wall John": "https://www.openwall.com/john/","Password Cracking With John The Ripper": "https://www.section.io/engineering-education/password-cracking-with-john-the-ripper/","Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
+                    return
+                if ask == "1":
+                    hashcat()
                 elif ask == "2":
-                    github = "Hydra is a password cracking tool that performs brute-force and dictionary attacks on network protocols such as Telnet, FTP, HTTP, and SSH. It is used to test the security of remote systems by attempting to log in with multiple username and password combinations. It can run on multiple operating systems and is commonly used by security professionals and penetration testers."
-                    template.template("hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool","Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
-
+                    john_the_ripper()
                 elif ask == "3":
-                    github = "Johnny is a GUI (Graphical User Interface) for the John the Ripper password cracking tool. It provides a user-friendly interface for managing and running John the Ripper's cracking tasks, rather than using command line commands. It is designed to make the process of cracking passwords more efficient and user-friendly. It can run on Windows, Linux and MacOS."
-                    template.template("johnny", "johnny", github.strip(), {"How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca","Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
+                    hydra()
                 elif ask == "4":
-                    github = "CrackStation is a website that provides a service to check if a given password has been previously compromised in a data breach. It uses a precomputed hash database of billions of real-world passwords to check if a given password is in the list. It's designed to help users and organizations check the security of their passwords and identify weak or easily guessable passwords that should be changed."
-                    template.template("CrackStation", "https://crackstation.net/",github.strip(), {"Salted Password Hashing - Doing it Right": "https://crackstation.net/hashing-security.htm","CrackStation's Password Cracking Dictionary": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm","Wordlist Download": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm"},method="browser")
+                    WEB_Application_Analysis.dirsearch()
                 elif ask == "5":
-                    github = "Cyber Chef is a web-based tool developed by the US Cyber Command, that allows users to perform digital forensic and incident response tasks, such as data carving, decoding, and exfiltration using pre-built 'recipes' or custom workflows using a visual, drag-and-drop interface. It can process various types of data and run on different platforms. It is generally used by security professionals to quickly process large amounts of data, extract useful information and identify potential malicious activity."
-                    template.template("CyberChef", "https://gchq.github.io/CyberChef/", github.strip(), {"CyberChef - A must have security tool": "https://www.youtube.com/watch?v=rT_CjwKN380","CyberChef – Data decoding made easy": "https://www.csnp.org/post/cyberchef-data-decoding-made-easy"},method="browser")
+                    johnny()
+                elif ask == "6":
+                    Configuration_Management.dirbuster()
+                elif ask == "7":
+                    reaver()
                 else:
                     break
 
-        elif option == "1":
+        elif option == "3":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Dictionary Attacks")
                 banner.description("A dictionary attack is a type of brute force attack that involves trying every word in a predefined list (a dictionary) as a password. This method is more efficient than a traditional brute force attack, where every possible combination of characters is tried, because most people use common words or phrases as passwords. The attacker can also use a list of commonly used passwords or publicly available information about the target (such as their name, birthdate, etc.) to create a custom dictionary.")
-                list_root_attacks = ["Hashcat", "John The Ripper", "Hydra", "Medusa", "Nrack", "Johnny (GUI John)","CrackStation (Website)", "CyberChef (Website)", "go back"]
+                list_root_attacks = ["Hashcat\t\t(Recommended)", "John The Ripper\t(Recommended)", "Hydra\t\t(Recommended)",
+                                     "Medusa", "Ncrack", "Johnny (GUI John)", "go back"]
                 for i in range(len(list_root_attacks)):
-                    print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+                    print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
-                    template.exit_program()
-                if ask == "0":
-                    github = "Hashcat is an open-source password cracking tool that can perform dictionary, brute force and combination attacks, it uses the power of GPUs to accelerate the cracking process, supports a wide variety of hashing algorithms and it can run on Windows, Linux and macOS. It's widely used for password recovery, security testing and penetration testing."
-                    template.template("hashcat", "hashcat", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/","How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
-                elif ask == "1":
-                    github = "John the Ripper is a free and open-source password cracking software tool. It can be run on a variety of operating systems, including Windows, macOS, and Linux. It uses a combination of wordlists and rules to try and guess the password for a given hash or file, and can support a variety of different hash types, including those used for Unix and Windows passwords. John the Ripper is commonly used by security professionals and system administrators to audit the security of their systems and detect weak or easily guessable passwords."
-                    template.template("john", "john", github.strip(), {"Open-wall John": "https://www.openwall.com/john/","Password Cracking With John The Ripper": "https://www.section.io/engineering-education/password-cracking-with-john-the-ripper/","Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
+                    return
+                if ask == "1":
+                    hashcat()
                 elif ask == "2":
-                    github = "Hydra is a password cracking tool that performs brute-force and dictionary attacks on network protocols such as Telnet, FTP, HTTP, and SSH. It is used to test the security of remote systems by attempting to log in with multiple username and password combinations. It can run on multiple operating systems and is commonly used by security professionals and penetration testers."
-                    template.template("hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool","Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
+                    john_the_ripper()    
                 elif ask == "3":
-                    github = "Medusa is a password cracking tool that is used to perform brute-force attacks on login credentials. It is a command-line tool that can be used to test the security of login systems by trying a large number of possible username and password combinations. Medusa is capable of testing various protocols such as HTTP, HTTPS, FTP, SSH, and more. It is mainly used by penetration testers and security professionals to identify weak passwords in a network and help improve the overall security of an organization. However, like other password cracking tools, it can also be used by malicious actors for illegal activities."
-                    template.template("medusa", "medusa", github.strip(), {"A Detailed Guide on Medusa": "https://www.hackingarticles.in/a-detailed-guide-on-medusa/","Bruteforce Password Cracking with Medusa": "https://www.yeahhub.com/bruteforce-password-cracking-medusa-kali-linux/"})
+                    hydra()    
                 elif ask == "4":
-                    github = "Ncrack is a network authentication cracking tool. It is designed to perform efficient brute-force and dictionary attacks against a variety of different network protocols, including Telnet, FTP, HTTP, HTTPS, SMB, and RDP. It can be used to test the security of networks and remote systems by attempting to log in with a large number of different username and password combinations.Ncrack is similar to other password cracking tools such as John the Ripper and Hydra, but it is specifically designed to work with network protocols. It can run on Windows, Linux, and macOS and is often used by security professionals and penetration testers to test the security of networks and web applications"
-                    template.template("ncrack", "ncrack", github.strip(), {"Comprehensive Guide on Ncrack – A Brute Forcing Tool": "https://www.hackingarticles.in/comprehensive-guide-on-ncrack-a-brute-forcing-tool/","Ncrack – Network Authentication and Password Cracking Tool": "https://secnhack.in/ncrack-network-authentication-and-password-cracking-tool/"})
+                    medusa()
                 elif ask == "5":
-                    github = "Johnny is a GUI (Graphical User Interface) for the John the Ripper password cracking tool. It provides a user-friendly interface for managing and running John the Ripper's cracking tasks, rather than using command line commands. It is designed to make the process of cracking passwords more efficient and user-friendly. It can run on Windows, Linux and MacOS."
-                    template.template("johnny", "johnny", github.strip(), {"How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca","Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
+                    ncrack()
                 elif ask == "6":
-                    github = "CrackStation is a website that provides a service to check if a given password has been previously compromised in a data breach. It uses a precomputed hash database of billions of real-world passwords to check if a given password is in the list. It's designed to help users and organizations check the security of their passwords and identify weak or easily guessable passwords that should be changed."
-                    template.template("CrackStation", "https://crackstation.net/",github.strip(), {"Salted Password Hashing - Doing it Right": "https://crackstation.net/hashing-security.htm","CrackStation's Password Cracking Dictionary": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm","Wordlist Download": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm"},method="browser")
-                elif ask == "7":
-                    github = "Cyber Chef is a web-based tool developed by the US Cyber Command, that allows users to perform digital forensic and incident response tasks, such as data carving, decoding, and exfiltration using pre-built 'recipes' or custom workflows using a visual, drag-and-drop interface. It can process various types of data and run on different platforms. It is generally used by security professionals to quickly process large amounts of data, extract useful information and identify potential malicious activity."
-                    template.template("CyberChef", "https://gchq.github.io/CyberChef/", github.strip(), {"CyberChef - A must have security tool": "https://www.youtube.com/watch?v=rT_CjwKN380","CyberChef – Data decoding made easy": "https://www.csnp.org/post/cyberchef-data-decoding-made-easy"},method="browser")
+                    johnny()
                 else:
                     break
-        elif option == "2":
+        elif option == "4":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Rainbow Table Attack")
                 banner.description("A rainbow table attack is a method of cracking password hashes by using precomputed tables of hash values, which can be faster than traditional brute force attack. It is particularly effective against hash functions that are fast to compute and vulnerable to collisions, but less effective against stronger hash functions.")
                 list_root_attacks = ["RainbowCrack", "ophCrack", "go back"]
                 for i in range(len(list_root_attacks)):
-                    print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+                    print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
-                    ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+                    ask = input(
+                        f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
-                    template.exit_program()
-                if ask == "0":
-                    github = "RainbowCrack is a password cracking tool that uses a large precomputed table of hash values to speed up the process of cracking passwords. It is commonly used to crack Windows LM hashes and NTLM hashes, as well as other types of hashes such as those used in Linux and Unix-based systems. The tool is named after the 'rainbow table' data structure it uses to efficiently store the precomputed hash values."
-                    template.template("rainbowcrack", "rcrack", github.strip(), {"How to use rainbow-crack tool": "https://null-byte.wonderhowto.com/how-to/rainbow-tables-create-use-them-crack-passwords-0131470/","Rainbow Tables & Rainbow-crack Cracking Passwords": "https://www.kalilinux.in/2021/03/rainbow-tables-rainbowcrack-kali-linux.html"})
-
-                elif ask == "1":
-                    github = "Ophcrack is a free, open-source password cracking tool specifically designed to crack Windows login passwords. It uses rainbow tables, a precomputed table of hash values, to crack passwords quickly. It can also recover LM and NTLM hashes, and it supports a variety of hash algorithms such as LM, NTLM, and MD5. The tool is available as a bootable CD or USB drive and can be used to recover lost or forgotten Windows passwords."
-                    template.template("ophcrack", "ophcrack", github.strip(), {"Crack Windows Passwords With Ophcrack and Rainbow Tables": "https://www.wikihow.com/Crack-Windows-Passwords-With-Ophcrack-and-Rainbow-Tables/"})
+                    return
+                if ask == "1":
+                    rainbowcrack()   
+                elif ask == "2":
+                    ophcrack()
                 else:
                     break
 
-        elif option == "3":
+        elif option == "5":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Wordlist Generator")
                 banner.description("A wordlist generator is a tool that generates a list of words or phrases that can be used in a dictionary attack. The list can be generated from a predefined dictionary, real-world data such as web pages, or by using a combination of commonly used words or patterns. This list of words is then used to try as potential passwords in a dictionary attack, which can be more efficient than a traditional brute force attack as it tries only words that are likely to be used as passwords.")
                 list_root_attacks = ["Crunch", "Cupp", "bopscrk", "go back"]
                 for i in range(len(list_root_attacks)):
-                    print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+                    print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
-                    ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+                    ask = input(
+                        f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
-                    template.exit_program()
-                if ask == "0":
-                    github = "Crunch is a wordlist generator tool that can be used to generate a list of all possible combinations of characters for a given set of parameters. It can be used to generate a wordlist for password cracking, testing password policies and other security related tasks. It is a simple command line tool that can be used to generate wordlists with different character sets, lengths, patterns and other parameters. It can also use a standard or a custom character set to generate the wordlist and can be used to generate a wordlist of any size."
-                    template.template("crunch", "crunch", github.strip(), {"Create Wordlist Using Crunch": "https://null-byte.wonderhowto.com/how-to/tutorial-create-wordlists-with-crunch-0165931/","Crunch Password List Generation": "https://www.hackingtutorials.org/general-tutorials/crunch-password-list-generation/","Complete Guide on Crunch Tool": "https://secnhack.in/complete-guide-on-crunch-tool/"})
-                elif ask == "1":
-                    github = "CUPP (Common User Passwords Profiler) is a tool that generates a custom wordlist based on personal information about a target. It can be used to generate a wordlist based on information such as the target's name, birthdate, address, and other personal details. CUPP can be used to perform a dictionary attack on a password hash, trying all the generated words as passwords, in order to crack the password. CUPP is written in Python and it's open source."
-                    template.template("cupp", "cupp", github.strip(), {"Cybrary CUPP Tool": "https://www.cybrary.it/blog/0p3n/using-cupp-tool-generate-powerful-password-lists/","How To Create Password List Using CUPP Tool": "https://programmercave0.github.io/blog/2019/10/10/How-to-create-Password-list-using-CUPP-tool-on-ubuntu","CUPP Tool Password Generator)": "https://www.geeksforgeeks.org/cupp-common-user-passwords-profiler/"})
+                    return
+                if ask == "1":
+                    crunch()
                 elif ask == "2":
-                    github = "Bopscrk (Before Outset Password Cracking is a tool to generate smart and powerful wordlists for targeted attacks. It is part of Black Arch Linux for as long as we can remember. It introduces personal information related to the target and combines every word and transforms it into possible passwords. It also contains a lyric pass module which allows it to search lyrics related to the favourite artist of the target and then include them into the wordlists."
-                    template.template("bopscrk", "bopscrk -i", github.strip(), {"Create Wordlist Like Pro by Zsecurity": "https://zsecurity.org/create-password-wordlists-like-a-pro-2/","Wordlist For Pentester": "https://www.hackingarticles.in/wordlists-for-pentester/"},method="pip")
+                    cupp()
+                elif ask == "3":
+                    bopscrk()
                 else:
                     break
 
-        elif option == "4":
+        elif option == "6":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Phishing Attacks")
                 banner.description("A phishing attack is a type of cyber attack in which an attacker uses fraudulent emails, websites, or other means of communication to trick a victim into providing sensitive information such as login credentials, personal information, or financial details. The attacker often poses as a trustworthy entity and attempts to convince the victim to click on a link, download an attachment, or enter information into a fake website. The goal of a phishing attack is to steal sensitive information or install malware on the victim's device.")
-                list_root_attacks = ["Social-Engineer Toolkit (SET)", "HiddenEye", "r3bu5", "zphisher", "Shellphish","Gophish (GUI)", "go back"]
+                list_root_attacks = ["Social-Engineer Toolkit (SET)", "HiddenEye", "r3bu5", "zphisher\t\t(Recommended)",
+                                     "Shellphish", "Gophish (GUI)\t(Recommended)", "Camphish\t\t(Recommended)", "go back"]
                 for i in range(len(list_root_attacks)):
-                    print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+                    print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
-                    ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+                    ask = input(
+                        f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
-                    template.exit_program()
-                if ask == "0":
-                    github = "The Social Engineering Toolkit (SET) is an open-source penetration testing framework that is used to perform various social engineering attacks. It is designed to be used for the purposes of penetration testing and vulnerability assessments, and it can be used to perform attacks such as phishing, website attacks, and other forms of social engineering. The toolkit is written in Python and is available for Windows, Linux, and Mac OS X. It can be used to test the security of an organization's employees and to evaluate the effectiveness of security awareness training programs."
-                    template.template("set", "setoolkit", github.strip(), {"Phishing using SET": "https://www.golinuxcloud.com/social-engineering-toolkit-phishing/","Phishing using SET by Hengky Sanjaya": "https://medium.com/hengky-sanjaya-blog/social-engineering-toolkit-set-23be8b66aa18"})
-
-                elif ask == "1":
-                    github = "HiddenEye is a modern phishing tool with advanced functionality. It is written in Python and can be run on Windows, Linux, and Mac OS X. It allows you to perform various phishing attacks."
-                    template.template("HiddenEye","python HiddenEye.py",github.strip(), {"HiddenEye by JohnJHacking": "https://johnjhacking.com/blog/hiddeneye/", "HiddenEye by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/", "HiddenEye by Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"},method="github",github_install="git clone https://github.com/Morsmalleo/HiddenEye && pip install -r requirements.txt",github_check="HiddenEye")
+                    return
+                if ask == "1":
+                    setoolkit()
                 elif ask == "2":
-                    github = "It is a Phishing tool that has latest and updated login pages, Mask URL support, Beginners Friendly, Multiple tunneling options"
-                    template.template("r3bu5", "./r3bu5.sh", github.strip(), {"Github Repo of r3bu5": " https://github.com/k46-db0y/r3bu5"}, method="github",github_install="git clone https://github.com/k46-db0y/r3bu5 && chmod +x r3bu5.sh",github_check="r3bu5")
+                    hiddeneye()
                 elif ask == "3":
-                    github = "Zphisher is an open-source phishing tool that automates the process of creating and deploying phishing pages. It allows users to easily create phishing pages for various popular websites, such as Google, Facebook, and LinkedIn, and can be used to perform phishing attacks on targeted individuals or organizations. It can also be used to test the security awareness of an organization's employees. Zphisher is written in Shell Script and it's available for Linux and Termux."
-                    template.template("zphisher", "chmod +x zphisher.sh && ./zphisher.sh", github.strip(), {"Zphisher phishing tool by reconshell": "https://reconshell.com/zphisher-an-automated-phishing-tool/","Zphisher phishing tool by vulners": "https://vulners.com/kitploit/KITPLOIT:1994086289094110137"},method="github", github_install="git clone https://github.com/htr-tech/zphisher",github_check="zphisher")
+                    r3bu5()
                 elif ask == "4":
-                    github = "Shellphish is a tool used for phishing attacks, specifically for the purpose of stealing login credentials. It automates the process of creating phishing pages for various websites, such as social media platforms and email services. The tool is typically used by ethical hackers and penetration testers to test the security of a system, but can also be used by malicious actors for illegal activities."
-                    template.template("ShellPhish", "./shellphish.sh", github.strip(),{"Shellphish Tool writeup.writeup": "https://www.kalilinux.in/2019/04/shellphish-phishing-page-creator.html"},method="github",github_install="git clone https://github.com/AbirHasan2005/ShellPhish && chmod +x shellphish.sh",github_check="ShellPhish")
+                    zphisher()
                 elif ask == "5":
-                    github = "Gophish is an open-source tool for conducting phishing campaigns. It allows users to create, send and track phishing campaigns, including the ability to create custom phishing templates and landing pages, as well as track user interactions with the phishing emails. Gophish is often used by penetration testers and security professionals to test the security of an organization's email system and educate employees on how to spot and avoid phishing attempts. However, like other phishing tools, it can also be used by malicious actors for illegal activities."
-                    template.template("Gophish","./gophish &",github.strip(), {"Create phishing campaign gophish": "https://www.golinuxcloud.com/create-phishing-campaign-gophish/","Phishing attack using gophish": "https://www.techrepublic.com/article/how-to-run-a-phishing-attack-simulation-with-gophish/"},method="github",github_install="mkdir Gophish && wget https://github.com/gophish/gophish/releases/download/v0.12.1/gophish-v0.12.1-linux-64bit.zip && unzip gophish-v0.12.1-linux-64bit.zip && chmod +x gophish",github_check="Gophish")
+                    shellphish()
+                elif ask == "6":
+                    gophish()
+                elif ask == "7":
+                    camphish()
                 else:
                     break
 
-        elif option == "5":
+        elif option == "7":
             while True:
                 os.system("clear")
                 banner.main()
                 banner.attack("Keylogger Attacks")
                 banner.description("A keylogger attack is a type of cyber attack in which an attacker uses malicious software, called a keylogger, to record every keystroke made by a victim on their computer or mobile device. This includes passwords, credit card numbers, personal information, and other sensitive data. The keylogger can also take screenshots of the victim's screen, record their internet browsing history, and even capture audio and video. The attacker can use this information to steal personal identities, login credentials, and financial information, or to gain access to sensitive systems. Keyloggers can be installed through malware, email attachments,or social engineering tactics like phishing.")
-                list_root_attacks = ["ZLogger", "go back"]
+                list_root_attacks = ["Keylogger", "go back"]
                 for i in range(len(list_root_attacks)):
-                    print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
+                    print(colors.options, f"{i+1}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
-                    ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+                    ask = input(
+                        f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
-                    template.exit_program()
-                if ask == "0":
-                    github = "zLogger is a Remote persistent keylogger it is written in python, and can generate executables that run on Windows and Linux, once executed on a system it’ll run the background, record every key-strike and report to the email specified when the keylogger was generated."
-                    template.template("ZLogger","python zlogger.py -h" ,github.strip(), {"ZLogger Tool in Medium": "https://medium.com/purple-team/make-a-keylogger-using-the-zlogger-tool-9945bc87922","ZLogger by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/","ZLogger in Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"},method="github", github_install="git clone https://github.com/z00z/ZLogger && pip install pynput && chmod +x *",github_check="ZLogger")
+                    return
+                if ask == "1":
+                    keylogger()    
                 else:
                     break
         else:
             return
+        
+
+
+def medusa():
+    github = "Medusa is a password cracking tool that is used to perform brute-force attacks on login credentials. It is a command-line tool that can be used to test the security of login systems by trying a large number of possible username and password combinations. Medusa is capable of testing various protocols such as HTTP, HTTPS, FTP, SSH, and more. It is mainly used by penetration testers and security professionals to identify weak passwords in a network and help improve the overall security of an organization. However, like other password cracking tools, it can also be used by malicious actors for illegal activities."
+    template.template("medusa", "medusa", github.strip(), {"A Detailed Guide on Medusa": "https://www.hackingarticles.in/a-detailed-guide-on-medusa/",
+                                      "Bruteforce Password Cracking with Medusa": "https://www.yeahhub.com/bruteforce-password-cracking-medusa-kali-linux/"})
+                
+def ncrack():
+    github = "Ncrack is a network authentication cracking tool. It is designed to perform efficient brute-force and dictionary attacks against a variety of different network protocols, including Telnet, FTP, HTTP, HTTPS, SMB, and RDP. It can be used to test the security of networks and remote systems by attempting to log in with a large number of different username and password combinations.Ncrack is similar to other password cracking tools such as John the Ripper and Hydra, but it is specifically designed to work with network protocols. It can run on Windows, Linux, and macOS and is often used by security professionals and penetration testers to test the security of networks and web applications"
+    template.template("ncrack", "ncrack", github.strip(), {"Comprehensive Guide on Ncrack – A Brute Forcing Tool": "https://www.hackingarticles.in/comprehensive-guide-on-ncrack-a-brute-forcing-tool/",
+                                      "Ncrack – Network Authentication and Password Cracking Tool": "https://secnhack.in/ncrack-network-authentication-and-password-cracking-tool/"})
+               
+def reaver():
+    github = "Reaver implements a brute force attack against Wifi Protected Setup (WPS) registrar PINs in order to recover WPA/WPA2 passphrases, as described in Brute forcing Wi-Fi Protected Setup When poor design meets poor implementation. by Stefan Viehböck. Reaver has been designed to be a robust and practical attack against Wi-Fi Protected Setup (WPS) registrar PINs in order to recover WPA/WPA2 passphrases and has been tested against a wide variety of access points and WPS implementations."
+    template.template("reaver", "reaver", github.strip(), {
+                                      "Revear cheatsheet": "https://cheatography.com/jlunz/cheat-sheets/reaver-cheat-sheet/", "Revear github": "https://github.com/t6x/reaver-wps-fork-t6x/blob/master/README.md", })
+                
+def johnny():
+    github = "Johnny is a GUI (Graphical User Interface) for the John the Ripper password cracking tool. It provides a user-friendly interface for managing and running John the Ripper's cracking tasks, rather than using command line commands. It is designed to make the process of cracking passwords more efficient and user-friendly. It can run on Windows, Linux and MacOS."
+    template.template("johnny", "johnny", github.strip(), {
+                                      "How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca", "Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
+                
+def hydra():
+    github = "Hydra is a password cracking tool that performs brute-force and dictionary attacks on network protocols such as Telnet, FTP, HTTP, and SSH. It is used to test the security of remote systems by attempting to log in with multiple username and password combinations. It can run on multiple operating systems and is commonly used by security professionals and penetration testers."
+    template.template("hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool",
+                                      "Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
+                
+def john_the_ripper():
+    github = "John the Ripper is a free and open-source password cracking software tool. It can be run on a variety of operating systems, including Windows, macOS, and Linux. It uses a combination of wordlists and rules to try and guess the password for a given hash or file, and can support a variety of different hash types, including those used for Unix and Windows passwords. John the Ripper is commonly used by security professionals and system administrators to audit the security of their systems and detect weak or easily guessable passwords."
+    template.template("john", "john -h", github.strip(), {"How to Crack Passwords using John The Ripper – Pentesting Tutorial": "https://www.freecodecamp.org/news/crack-passwords-using-john-the-ripper-pentesting-tutorial/", "How to use the John the Ripper password cracker": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-John-the-Ripper-password-cracker", "Unveiling the Power of John the Ripper: A Beginner’s Guide to Password Cracking":
+                                      "https://infosecwriteups.com/unveiling-the-power-of-john-the-ripper-a-beginners-guide-to-password-cracking-a9846172b35a", "Open-wall John": "https://www.openwall.com/john/", "Password Cracking With John The Ripper": "https://medium.com/@mohitdeswal_35470/john-the-ripper-a-comprehensive-guide-to-password-cracking-9335f44ed3f5", "Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
+                
+def hashcat():
+    github = "Hashcat is an open-source password cracking tool that can perform dictionary, brute force and combination attacks, it uses the power of GPUs to accelerate the cracking process, supports a wide variety of hashing algorithms and it can run on Windows, Linux and macOS. It's widely used for password recovery, security testing and penetration testing."
+    template.template("hashcat", "hashcat -h", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/",
+                                      "How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
+                
+def rainbowcrack():
+    github = "RainbowCrack is a password cracking tool that uses a large precomputed table of hash values to speed up the process of cracking passwords. It is commonly used to crack Windows LM hashes and NTLM hashes, as well as other types of hashes such as those used in Linux and Unix-based systems. The tool is named after the 'rainbow table' data structure it uses to efficiently store the precomputed hash values."
+    template.template("rainbowcrack", "rcrack", github.strip(), {"How to use rainbow-crack tool": "https://null-byte.wonderhowto.com/how-to/rainbow-tables-create-use-them-crack-passwords-0131470/",
+                                      "Rainbow Tables & Rainbow-crack Cracking Passwords": "https://www.kalilinux.in/2021/03/rainbow-tables-rainbowcrack-kali-linux.html"})
+
+def ophcrack():
+    github = "Ophcrack is a free, open-source password cracking tool specifically designed to crack Windows login passwords. It uses rainbow tables, a precomputed table of hash values, to crack passwords quickly. It can also recover LM and NTLM hashes, and it supports a variety of hash algorithms such as LM, NTLM, and MD5. The tool is available as a bootable CD or USB drive and can be used to recover lost or forgotten Windows passwords."
+    template.template("ophcrack", "ophcrack", github.strip(), {
+                                      "Crack Windows Passwords With Ophcrack and Rainbow Tables": "https://www.wikihow.com/Crack-Windows-Passwords-With-Ophcrack-and-Rainbow-Tables/"})
+                
+def crunch():
+    github = "Crunch is a wordlist generator tool that can be used to generate a list of all possible combinations of characters for a given set of parameters. It can be used to generate a wordlist for password cracking, testing password policies and other security related tasks. It is a simple command line tool that can be used to generate wordlists with different character sets, lengths, patterns and other parameters. It can also use a standard or a custom character set to generate the wordlist and can be used to generate a wordlist of any size."
+    template.template("crunch", "crunch", github.strip(), {"Create Wordlist Using Crunch": "https://null-byte.wonderhowto.com/how-to/tutorial-create-wordlists-with-crunch-0165931/",
+                                      "Crunch Password List Generation": "https://www.hackingtutorials.org/general-tutorials/crunch-password-list-generation/", "Complete Guide on Crunch Tool": "https://secnhack.in/complete-guide-on-crunch-tool/"})
+                
+def cupp():
+    github = "CUPP (Common User Passwords Profiler) is a tool that generates a custom wordlist based on personal information about a target. It can be used to generate a wordlist based on information such as the target's name, birthdate, address, and other personal details. CUPP can be used to perform a dictionary attack on a password hash, trying all the generated words as passwords, in order to crack the password. CUPP is written in Python and it's open source."
+    template.template("cupp", "cupp", github.strip(), {"Cybrary CUPP Tool": "https://www.cybrary.it/blog/0p3n/using-cupp-tool-generate-powerful-password-lists/", "How To Create Password List Using CUPP Tool":
+                                      "https://programmercave0.github.io/blog/2019/10/10/How-to-create-Password-list-using-CUPP-tool-on-ubuntu", "CUPP Tool Password Generator)": "https://www.geeksforgeeks.org/cupp-common-user-passwords-profiler/"})
+                
+def bopscrk():
+        github = "Bopscrk (Before Outset Password Cracking) is a tool to generate smart and powerful wordlists for targeted attacks. It is part of Black Arch Linux for as long as we can remember. It introduces personal information related to the target and combines every word and transforms it into possible passwords. It also contains a lyric pass module which allows it to search lyrics related to the favourite artist of the target and then include them into the wordlists."
+        template.template("bopscrk", "bopscrk -i", github.strip(), {"Create Wordlist Like Pro by Zsecurity": "https://zsecurity.org/create-password-wordlists-like-a-pro-2/",
+                                      "Wordlist For Pentester": "https://www.hackingarticles.in/wordlists-for-pentester/"}, method="pip")
+                
+
+def setoolkit():
+    github = "The Social Engineering Toolkit (SET) is an open-source penetration testing framework that is used to perform various social engineering attacks. It is designed to be used for the purposes of penetration testing and vulnerability assessments, and it can be used to perform attacks such as phishing, website attacks, and other forms of social engineering. The toolkit is written in Python and is available for Windows, Linux, and Mac OS X. It can be used to test the security of an organization's employees and to evaluate the effectiveness of security awareness training programs."
+    template.template("set", "setoolkit", github.strip(), {"Phishing using SET": "https://www.golinuxcloud.com/social-engineering-toolkit-phishing/",
+                                      "Phishing using SET by Hengky Sanjaya": "https://medium.com/hengky-sanjaya-blog/social-engineering-toolkit-set-23be8b66aa18"})
+
+
+def hiddeneye():
+    github = "HiddenEye is a modern phishing tool with advanced functionality. It is written in Python and can be run on Windows, Linux, and Mac OS X. It allows you to perform various phishing attacks."
+    template.template("HiddenEye", "python HiddenEye.py", github.strip(), {"HiddenEye by GeeksForGeeks": "https://www.geeksforgeeks.org/hiddeneye-modern-phishing-tool-with-advanced-functionality/", "HiddenEye by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/",
+                                      "HiddenEye by Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"}, method="github", github_install="git clone https://github.com/Morsmalleo/HiddenEye && cd HiddenEye && pip install -r requirements.txt", github_check="HiddenEye")
+def r3bu5():
+    github = "It is a Phishing tool that has latest and updated login pages, Mask URL support, Beginners Friendly, Multiple tunneling options"
+    template.template("r3bu5", "./r3bu5.sh", github.strip(), {"Github Repo of r3bu5": " https://github.com/k46-db0y/r3bu5"}, method="github",
+                                      github_install="git clone https://github.com/k46-db0y/r3bu5.git && cd r3bu5 && chmod +x r3bu5.sh", github_check="r3bu5")
+        
+def zphisher():
+    github = "Zphisher is an open-source phishing tool that automates the process of creating and deploying phishing pages. It allows users to easily create phishing pages for various popular websites, such as Google, Facebook, and LinkedIn, and can be used to perform phishing attacks on targeted individuals or organizations. It can also be used to test the security awareness of an organization's employees. Zphisher is written in Shell Script and it's available for Linux and Termux."
+    template.template("zphisher", "bash zphisher.sh", github.strip(), {"Zphisher – Automated Phishing Tool in Kali Linux": "https://www.geeksforgeeks.org/zphisher-automated-phishing-tool-in-kali-linux/",
+                                      "Creating Phishing Links with Zphisher": "https://medium.com/@jbtechmaven/creating-phishing-links-with-zphisher-db7cc8a1f013"}, method="github", github_install="git clone git://github.com/htr-tech/zphisher.git && cd zphisher && chmod +x zphisher.sh", github_check="zphisher")        
+def gophish():
+    github = "Gophish is an open-source tool for conducting phishing campaigns. It allows users to create, send and track phishing campaigns, including the ability to create custom phishing templates and landing pages, as well as track user interactions with the phishing emails. Gophish is often used by penetration testers and security professionals to test the security of an organization's email system and educate employees on how to spot and avoid phishing attempts. However, like other phishing tools, it can also be used by malicious actors for illegal activities."
+    template.template("Gophish", "gophish]", github.strip(), {"Create phishing campaign gophish": "https://www.golinuxcloud.com/create-phishing-campaign-gophish/", "Phishing attack using gophish": "https://www.techrepublic.com/article/how-to-run-a-phishing-attack-simulation-with-gophish/"},
+                                      method="github", github_install="git clone https://github.com/gophish/gophish.git && cd gophish && chmod +x gophish.go && go run gophish.go", github_check="Gophish")
+def shellphish():
+    github = "Shellphish is a tool used for phishing attacks, specifically for the purpose of stealing login credentials. It automates the process of creating phishing pages for various websites, such as social media platforms and email services. The tool is typically used by ethical hackers and penetration testers to test the security of a system, but can also be used by malicious actors for illegal activities."    
+    template.template("ShellPhish", "./shellphish.sh", github.strip(), {"Shellphish Tool": "https://www.kalilinux.in/2019/04/shellphish-phishing-page-creator.html"},
+                                      method="github", github_install="git clone https://github.com/AbirHasan2005/ShellPhish && cd ShellPhish && chmod +x shellphish.sh", github_check="ShellPhish")
+
+
+def keylogger():
+    github = "Welcome to the simple keylogger repo! A keylogger is a program that records your keystrokes, and this program saves them in a log file on your local computer."
+    template.template("Keylogger", "python Keylogger.py", github.strip(), {
+                                      "How to Set Up Keylogging on Your Linux Computer": "https://www.makeuseof.com/set-up-keylogging-on-linux/"}, method="github",github_install="git clone https://github.com/GiacomoLaw/Keylogger.git && cd Keylogger/linux && pip install -r requirements.txt ", github_check="Keylogger")
 
+def camphish():
+    github = "CamPhish is techniques to take cam shots of target's phone front camera or PC webcam. CamPhish Hosts a fake website on in built PHP server and uses ngrok & serveo to generate a link which we will forward to the target, which can be used on over internet. website asks for camera permission and if the target allows it, this tool grab camshots of target's device."
+    template.template("CamPhish", "camphish", github.strip(), {"How To Access Android Phone Camera Using Kali Linux": "https://blog.hackerassociate.com/how-to-access-android-phone-camera-using-kali-linux/", "Hack Android Phone Camera using CamPhish":
+                                      "https://systemweakness.com/hack-android-phone-camera-using-camphish-9d6126ae7786"}, method="github", github_install="git clone https://github.com/techchipnet/CamPhish && cd CamPhish && bash camphish.sh", github_check="camphish")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Pentesting_Bug_Bounty.py` & `cyberonix-3.0.0/cyberonix/main/tools/Pentesting_Bug_Bounty.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cyberonix.main.tools import (
     banner,
     colors,
     information_gathering,template
 )
-from cyberonix.main.tools import (
+from main.tools import (
     Configuration_Management,
     Secure_Transmission,
     Authentication,
     Session_Management,
     Authorization,
     data_validation,
     Cryptography,
@@ -24,84 +24,84 @@
 # main function
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Pentesting and Bug Bounty")
         list_attacks = [
-            "Information Gathering",
-            "Configuration Management",
-            "Secure Transmission",
-            "Authentication",
-            "Session Management",
-            "Authorization",
-            "Data Validation",
-            "Denial of Service",
-            "Business Logic",
+            " Information Gathering",
+            " Configuration Management",
+            " Secure Transmission",
+            " Authentication",
+            " Session Management",
+            " Authorization",
+            " Data Validation",
+            " Denial of Service(DOS)",
+            " Business Logic",
             "Cryptography",
             "Risky Functionality - File Uploads",
             "Risky Functionality - Card Payment",
             "HTML 5",
             "Go Back",
         ]
         for i in range(len(list_attacks)):
-            print(colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
+            return
+        if option == "1":
             print("\n[+] Information Gathering")
             os.system("clear")
             information_gathering.main()
-        elif option == "1":
+        elif option == "2":
             print("\n[+] Configuration Management")
             os.system("clear")
             Configuration_Management.main()
-        elif option == "2":
+        elif option == "3":
             print("\n[+] Secure Transmission")
             os.system("clear")
             Secure_Transmission.main()
-        elif option == "3":
+        elif option == "4":
             print("\n[+] Authentication")
             os.system("clear")
             Authentication.main()
-        elif option == "4":
+        elif option == "5":
             print("\n[+] Session Management")
             os.system("clear")
             Session_Management.main()
-        elif option == "5":
+        elif option == "6":
             print("\n[+] Authorization")
             os.system("clear")
             Authorization.main()
-        elif option == "6":
+        elif option == "7":
             print("\n[+] Data Validation")
             os.system("clear")
             data_validation.main()
-        elif option == "7":
+        elif option == "8":
             print("\n[+] Denial of Service")
             os.system("clear")
             dos.main()
-        elif option == "8":
+        elif option == "9":
             print("\n[+] Business Logic")
             os.system("clear")
             template.template("Business Logic","no-tools",'Business logic is the custom rules or algorithms that handle the exchange of information between a database and user interface. Business logic is essentially the part of a computer program that contains the information (in the form of business rules) that defines or constrains how a business operates. Such business rules are operational policies that are usually expressed in true or false binaries. Business logic can be seen in the workflows that they support, such as in sequences or steps that specify in detail the proper flow of information or data, and therefore decision-making. Business logic is also known as "domain logic."',{"Business Logic":"https://portswigger.net/web-security/logic-flaws/examples#top","Exploiting Business Logic Vulnerabilities":"https://medium.com/armourinfosec/exploiting-business-logic-vulnerabilities-234f97d6c4c0","WEB APPLICATION — BUSINESS LOGIC VULNERABILITIES":"https://infosecwriteups.com/web-application-business-logic-vulnerabilities-51be9c6b99fa","Business Logic Flaw":"https://www.wallarm.com/what/business-logic-flaw"})
-        elif option == "9":
+        elif option == "10":
             print("\n[+] Cryptography")
             os.system("clear")
             Cryptography.main()
-        elif option == "10":
+        elif option == "11":
             print("\n[+] Risky Functionality - File Uploads")
             os.system("clear")
             File_Upload.main()
-        elif option == "11":
+        elif option == "12":
             print("\n[+] Risky Functionality - Card Payment")
             os.system("clear")
             RiskyFuncPayment.main()
-        elif option == "12":
+        elif option == "13":
             print("\n[+] HTML 5")
             os.system("clear")
             html5.main()
         else:
             return
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/PostExploitationAttacks.py` & `cyberonix-3.0.0/cyberonix/main/tools/PostExploitationAttacks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,145 @@
-from cyberonix.main.tools import banner,colors,template
+from cyberonix.main.tools import banner, colors, template,Exploitation_Tools
 import os
 import requests
 from bs4 import BeautifulSoup
 
-#main function
+# main function
+
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Post Exploitation")
-        list_attacks=["Metasploit-Framework","LinPeas","LinEnum","Sudo killer","Beroot","Linux Exploit Suggester 2","LSE (Linux Smart Enumeration) ","PSPY","Bashark","Linux Private-i","Shellter","Amber","UPX (Ultimate Packer for Executable)","Covermyass","Go Back"]
+        list_attacks = [" Metasploit-Framework\t\t(Recommended)", " LinPeas", " LinEnum", " Sudo killer\t\t\t(Recommended)", " Beroot", " Linux Exploit Suggester 2", " LSE (Linux Smart Enumeration) ",
+                        " PSPY","Linux Private-i", "Shellter", "UPX (Ultimate Packer for Executable)", "Go Back"]
         for i in range(len(list_attacks)):
-                print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option=="0":
+            return
+        if option == "1":
             print("\n[+] Metasploit-Framework")
-            os.system("clear")
-            # name,command,discription,writeup,link=True,method="kali",github_install="",github_check=True
-            github = "The Metasploit Framework is an open-source tool for developing and executing exploit code against a remote target machine. It can be used to test the security of a computer system by finding and exploiting vulnerabilities. The framework includes a large collection of exploit modules, as well as various tools for payload generation, post-exploitation, and more. It can be used by security professionals for penetration testing, as well as by attackers for malicious purposes."
-            template.template("metasploit-framework","msfconsole",github.strip(),{"Msf-Community-Post-Exploitation":"https://www.offensive-security.com/metasploit-unleashed/msf-community-post-exploitation","Post Exploitation In Linux With Metasploit":"https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/","Privilege Escalation (Metasploit Unleashed)":"https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/","Post Exploitation Metasploit Modules (Reference)":"https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference","PSExec Pass the Hash (Horizontal Escalation)":"https://www.offensive-security.com/metasploit-unleashed/psexec-pass-hash/","ms10_002_aurora (Vertical Escalation)":"https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/","ms10_002_aurora (Horizontal Escalation)":"https://www.offensive-security.com/metasploit-unleashed/pivoting/ ","jtr_crack_fast (Hash Cracking)":"https://www.offensive-security.com/metasploit-unleashed/john-ripper/","warftpd_165_user (Keylogging)":"https://www.offensive-security.com/metasploit-unleashed/keylogging/","3proxy (Backdoor)":"https://www.offensive-security.com/metasploit-unleashed/meterpreter-backdoor/","persistence.rb (Persistent Backdoor)":"https://www.offensive-security.com/metasploit-unleashed/meterpreter-service/","Enabling Remote Desktop":"https://www.offensive-security.com/metasploit-unleashed/enabling-remote-desktop/","Post Exploitation in Linux with Metasploit":"https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/","Post Exploitation Metasploit Modules Reference":"https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference/","Hack Like Pro: Kill and Disable Antivirus Software Remote PC":"https://null-byte.wonderhowto.com/how-to/hack-like-pro-kill-and-disable-antivirus-software-remote-pc-0141906/","Armitage Post Exploitation":"https://www.offensive-security.com/metasploit-unleashed/armitage-post-exploitation/","Setup Armitage as a Command & Control Framework for Free":"https://infosecwriteups.com/setup-armitage-as-a-command-control-c2-framework-for-free-bae590064817","Event Log Management":"https://www.offensive-security.com/metasploit-unleashed/event-log-management","Interacting with the Registry":"https://www.offensive-security.com/metasploit-unleashed/interacting-registry"})        
-        elif option=="1":
+            Exploitation_Tools.metasploit()    
+        elif option == "2":
             print("\n[+] LinPeas")
-            os.system("clear")
-            github = "LinPeas is a script that automates the process of gathering information about a Linux system, similar to Windows' PowerShell script PEAS. This script can help identify potential vulnerabilities and misconfigurations on a Linux system, as well as provide information about system and network configuration. It can be useful for penetration testing, security assessments, and incident response. The script can be executed with arguments to specify which information to gather, or without arguments to gather all available information"
-            template.template("linpeas","chmod +x linpeas.sh && ./linpeas.sh -h",github.strip(),{"LinPeas Blog":"https://blog.cyberethical.me/linpeas","Linux-Privilege-Escalation":"https://delinea.com/blog/linux-privilege-escalation","Linux Privilege Escalation: Quick and Dirty":"https://johnjhacking.com/blog/linux-privilege-escalation-quick-and-dirty/","Outrunsec LinPeas":"https://outrunsec.com/tag/linpeas/","Linux-Privilege-Escalation-Suid-Binaries":"https://steflan-security.com/linux-privilege-escalation-suid-binaries"},method = "github", github_install = "wget --no-verbose https://github.com/carlospolop/PEASS-ng/releases/latest/download/linpeas.sh 2>/dev/null && mkdir LinPeas && mv linpeas.sh LinPeas", github_check = "LinPeas")
-        elif option=="2":
+            linpeas()        
+        elif option == "3":
             print("\n[+] LinEnum")
-            os.system("clear")
-            github = "LinEnum is a Linux enumeration script that can be used to enumerate information from a Linux system. It is designed to be run locally on a Linux system and will attempt to enumerate common files, folders, users, groups, services, configurations, and permissions. It can also be used to look for certain security vulnerabilities such as local privilege escalation. LinEnum can be run from the command line or can be automated using a script. The output of the script can be saved as a text file for later analysis."
-            template.template("LinEnum","chmod +x LinEnum.sh && ./LinEnum.sh -h",github.strip(),{"Use-LinEnum-Identify-Potential-Privilege-Escalation-Vectors":"https://null-byte.wonderhowto.com/how-to/use-linenum-identify-potential-privilege-escalation-vectors-0197225/","Linux-Privilege-Escalation-With-LinEnum":"https://trevorxcohen.medium.com/linux-privilege-escalation-with-linenum-75d20a3b59f6","LinEnum-Linux-Enumeration-Privilege-Escalation-Tool":"https://www.darknet.org.uk/2014/11/linenum-linux-enumeration-privilege-escalation-tool","Linux-Privilege-Escalation-Quick-And-Dirty":"https://johnjhacking.com/blog/linux-privilege-escalation-quick-and-dirty","Linux Enumeration And Privilege Escalation – LinEnum":"https://vulners.com/n0where/N0WHERE:24819"},method = "github", github_install = "curl -s https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh -o LinEnum.sh && mkdir LinEnum && mv LinEnum.sh LinEnum", github_check = "LinEnum")
-        elif option=="3":
+            linenum()       
+        elif option == "4":
             print("\n[+] Sudo killer")
-            os.system("clear")
-            github_text_6 = github_getting_text("https://github.com/TH3xACE/SUDO_KILLER",'p[dir="auto"]',6)
-            github_text_7 = github_getting_text("https://github.com/TH3xACE/SUDO_KILLER",'p[dir="auto"]',7)
-            github = github_text_6 + github_text_7
-            template.template("Sudo Killer","chmod u+x * && ./SUDO_KILLERv2.4.2.sh",github.strip(),{"SUDO_KILLER-Demos":"https://github.com/TH3xACE/SUDO_KILLER#demos","Sudo-Killer Briskinfosec":"https://www.briskinfosec.com/tooloftheday/toolofthedaydetail/SUDO-KILLER","Sudo-Killer-Identify-Abuse-Sudo-Misconfigurations":"https://null-byte.wonderhowto.com/how-to/use-sudo-killer-identify-abuse-sudo-misconfigurations-0202594"},method = "github", github_install = "git clone https://github.com/TH3xACE/SUDO_KILLER.git", github_check = "SUDO_KILLER")
-        elif option=="4":
+            sudokiller()    
+        elif option == "5":
             print("\n[+] Beroot")
-            os.system("clear")
-            github_text_0 = github_getting_text("https://github.com/AlessandroZ/BeRoot",'p[dir="auto"]',0)
-            github_text_1 = github_getting_text("https://github.com/AlessandroZ/BeRoot",'p[dir="auto"]',1)
-            github = github_text_0 + github_text_1
-            template.template("BeRoot","cd Linux && chmod u+x * && ./beroot.py",github.strip(),{"BeRoot-Linux-Privilege-Escalation":"https://www.kitploit.com/2018/06/beroot-for-linux-privilege-escalation.html?m=0","BeRoot-A-Post-Exploitation-Privilege-Escalation-Tool":"https://latesthackingnews.com/2019/08/02/beroot-a-post-exploitation-privilege-escalation-tool","BeRoot-Windows-Privilege-Escalation":"https://securityonline.info/beroot-windows-privilege-escalation"},method = "github", github_install = "git clone https://github.com/AlessandroZ/BeRoot.git", github_check = "BeRoot")
-        elif option=="5":
+            beroot()        
+        elif option == "6":
             print("\n[+] Linux Exploit Suggester 2")
-            os.system("clear")
-            github = "Linux Exploit Suggester 2 (LES 2) is a tool that can be used to identify potential vulnerabilities and exploits that can be used to compromise a Linux system. It works by analyzing the running kernel version and system information, and then comparing it to a local database of known vulnerabilities and exploits. LES 2 can also be used to determine whether a patch has been applied to a specific vulnerability, making it useful for identifying systems that are still vulnerable to known exploits. The tool is open-source and can be easily installed on a Linux system. It supports a wide range of Linux distributions, including Ubuntu, Debian, Fedora, Arch Linux and more. LES 2 is a command-line tool and requires Python to run.It's a useful tool for penetration testers and system administrators to identify and prioritize vulnerabilities on their systems."
-            template.template("linux-exploit-suggester-2","chmod u+x linux-exploit-suggester-2.pl && ./linux-exploit-suggester-2.pl",github.strip(),{"Kali Tools (linux-exploit-suggester)":"https://www.kali.org/tools/linux-exploit-suggester/","Find-Exploits-Get-Root-With-Linux-Exploit-Suggester":"https://null-byte.wonderhowto.com/how-to/find-exploits-get-root-with-linux-exploit-suggester-0206005","Pentest-Monkey Linux-Exploit-Suggester":"https://pentestmonkey.net/tools/audit/exploit-suggester","Linux-Exploit-Suggester-A-Kali-Linux-Tool-To-Find-The-Linux-Os-Kernel-Exploits":"https://gbhackers.com/linux-exploit-suggester-a-kali-linux-tool-to-find-the-linux-os-kernel-exploits","Securityonline Linux-Exploit Suggester":"https://securityonline.info/linux-exploit-suggester-2"},method="github",github_install="git clone https://github.com/jondonas/linux-exploit-suggester-2.git",github_check="linux-exploit-suggester-2")
-        elif option=="6":
+            linux_exploit_suggester2()        
+        elif option == "7":
             print("\n[+] LSE (Linux Smart Enumeration)")
-            os.system("clear")
-            github = "Linux Smart Enumeration (LSE) is a script written by Diego Treitos that automates the enumeration process for Linux systems. It is designed to run quickly and efficiently, and to provide detailed information about the system, including users, groups, permissions, network configuration, and more. LSE is intended to be used by penetration testers and security professionals to gather information about a target system during the reconnaissance phase of an engagement."
-            template.template("linux-smart-enumeration","chmod u+x lse.sh && ./lse.sh",github.strip(),{"Documentation (linux-smart-enumeration)":"https://github.com/diego-treitos/linux-smart-enumeration/blob/master/README.md","Use-Linux-Smart-Enumeration-Discover-Paths-Privesc":"https://null-byte.wonderhowto.com/how-to/use-linux-smart-enumeration-discover-paths-privesc-0330807","Hakin9 linux-smart-enumeration":"https://hakin9.org/linux-smart-enumeration"},method="github",github_install="git clone https://github.com/diego-treitos/linux-smart-enumeration.git",github_check="linux-smart-enumeration")
-        elif option=="7":
+            linux_smart_enumeration()        
+        elif option == "8":
             print("\n[+] PSPY")
-            os.system("clear")
-            github_text_0=github_getting_text("https://github.com/DominicBreuker/pspy",'p[dir="auto"]',2)
-            github_text_1=github_getting_text("https://github.com/DominicBreuker/pspy",'p[dir="auto"]',3)
-            github = github_text_0 + github_text_1
-            version = github_getting_text("https://github.com/DominicBreuker/pspy/releases/",'div[class="css-truncate css-truncate-target"]',0).strip()
-            template.template("pspy64","chmod u+x pspy64 && ./pspy64",github.strip(),{"Using-PSPY-To-Monitor-Linux-Processes":"https://infinitelogins.com/2020/09/04/using-ps-py-to-monitor-linux-processes","Cyberkendra Pspy-Tool-Monitor-Linux-Processes":"https://tools.cyberkendra.com/2020/04/pspy-tool-monitor-linux-processes.html","How-To-Enumerate-Services-In-Use-With-PSPY":"https://vk9-sec.com/how-to-enumerate-services-in-use-with-pspy","TryHackMe-ConvertMyVideo Writeup":"https://sparshjazz.medium.com/tryhackme-convertmyvideo-writeup-56b6c8217001","Bootlesshacker PSPY":"https://www.bootlesshacker.com/tag/pspy","SecurityOnline PSPY":"https://securityonline.info/pspy"},method="github",github_install=f"wget --no-verbose https://github.com/DominicBreuker/pspy/releases/download/{version}/pspy64 2>/dev/null && mkdir PSPY && mv pspy64 PSPY",github_check="PSPY")
-        elif option=="8":
-            print("\n[+] Bashark")
-            os.system("clear")
-            github = "Bashark is an open-source tool developed by redcode-labs that allows you to perform reconnaissance on a target by using various command-line tools and APIs. It can be used to gather information about a target's IP address, DNS information, WHOIS information, and more. Bashark is written in Bash and can be run on Linux and macOS systems. It is commonly used by penetration testers and security researchers to gather information during the reconnaissance phase of a penetration testing engagement"
-            template.template("Bashark","chmod u+x bashark.sh && ./bashark.sh",github.strip(),{"Documentation":"https://github.com/redcode-labs/Bashark/blob/master/README.md","SecurityOnline-Bashark":"https://securityonline.info/bashark/","Bashark-Bash-Post-Exploitation-Toolkit":"https://www.kitploit.com/2018/10/bashark-bash-post-exploitation-toolkit.html"},method = "github", github_install = "curl -s https://raw.githubusercontent.com/redcode-labs/Bashark/master/bashark.sh -o bashark.sh && mkdir Bashark && mv bashark.sh Bashark", github_check = "Bashark")
-        elif option=="9":
+            pspy()       
+        elif option == "9":
             print("\n[+] Linux Private-i")
-            os.system("clear")
-            github = "A Linux Enumeration & Privilege Escalation tool that automates the basic enumeration steps and displays the results in an easily readable format. The script comes loaded with a variety of 4 Options to choose from. Using Bash, execute private-i.sh on the local low privileged user. Select an option, execute & watch the show. Each mode uses common Linux binaries to enumerate the local system (find, grep, ps, etc). If you have a non-bash shell such as sh, use Noir-Private-i. Either script will not write or auto-exploit in any way"
-            template.template("Linux Private-i","chmod u+x private-i.sh && ./private-i.sh",github.strip(),{"Documentation":"https://github.com/rtcrowley/linux-private-i/blob/master/README.md","HackingArticles-linux-privilege-escalation-automated-script":"https://www.hackingarticles.in/linux-privilege-escalation-automated-script"},method = "github", github_install = "curl -s https://raw.githubusercontent.com/rtcrowley/linux-private-i/master/private-i.sh -o private-i.sh && mkdir Private-i && mv private-i.sh Private-i", github_check = "Private-i")
-        elif option=="10":
+            linux_private_i()        
+        elif option == "10":
             print("\n[+] Shellter")
-            os.system("clear")
-            github = "Shellter is a dynamic shellcode injection tool aka dynamic PE infector. It can be used in order to inject shellcode into native Windows applications (currently 32-bit apps only). The shellcode can be something yours or something generated through a framework, such as Metasploit. Shellter takes advantage of the original structure of the PE file and doesn't apply any  modification such as changing memory access permissions in sections (unless the user wants to), adding an extra section with RWE access, and whatever would look dodgy under an AV scan. Shellter is not just an EPO infector that tries to find a location to insert an instruction to redirect execution to the payload. Unlike any other infector, Shellter’s advanced infection engine never transfers the execution flow to a code cave or to an added section in the infected PE file. Shellter uses a unique dynamic approach which is based on the execution flow of the target application. This means that no static/predefined locations are used for shellcode injection. Shellter will launch and trace the target, while at the same time will log the execution flow of the application."
-            template.template("shellter","shellter",github.strip(),{"Introduction to Shellter": "https://github.com/ParrotSec/shellter#readme","Tool documentation for Shellter on Kali Linux": "https://www.kali.org/tools/shellter/#tool-documentation","Anti-virus Bypass with Shellter 5.1 on Kali Linux": "https://cyberarms.wordpress.com/2015/10/04/anti-virus-bypass-with-shellter-5-1-on-kali-linux/","Shellter: A Shellcode Injecting Tool": "https://www.hackingarticles.in/shellter-a-shellcode-injecting-tool/","Shellter - The Ultimate Tool for AV Evasion": "https://metalkey.github.io/shellter---the-ultimate-tool-for-av-evasion.html","Hack like a Pro: Evade AV Software with Shellter": "https://null-byte.wonderhowto.com/how-to/hack-like-pro-evade-av-software-with-shellter-0168504/"})    
-        elif option=="11":
-            print("\n[+] Amber")
-            os.system("clear")
-            github=github_getting_text("https://github.com/EgeBalci/amber",'p[dir="auto"]',1)
-            template.template("Amber","chmod u+x amber && ./amber",github.strip(),{"Amber README":"https://github.com/EgeBalci/amber/blob/master/README.md","Amber Video - 1 ":"https://www.youtube.com/watch?v=3en0ftnjEpE","Amber Video - 2 ":"https://www.youtube.com/watch?v=lCPdKSH6RMc","Amber Usage":"https://raw.githubusercontent.com/EgeBalci/amber/master/img/usage.gif"},method = "github", github_install = "wget --no-verbose https://github.com/EgeBalci/amber/releases/download/v3.1/amber_linux_amd64_3.1.zip 2>/dev/null && unzip -qq amber_linux_amd64_3.1.zip && rm amber_linux_amd64_3.1.zip", github_check = "amber_linux_amd64_3.1")    
-        elif option=="12":
+            shelter()        
+        elif option == "11":
             print("\n[+] UPX (Ultimate Packer for Executable)")
-            os.system("clear")
-            github = "UPX is a free, portable, extendable, high-performance executable packer for several different executable formats. It can be used to compress and obfuscate executable files to make them smaller and more difficult to reverse engineer. UPX supports a wide range of file formats, including Windows PE, Linux ELF, and more. UPX is available for a variety of platforms, including Windows, Linux, and macOS. The UPX compression algorithm is designed to compress the code section of an executable file, while leaving the data section uncompressed. This allows the compressed code to be executed directly from memory without the need to decompress it first. UPX is open-source and actively maintained, with updates and bug fixes released regularly."
-            template.template("UPX (Ultimate Packer for Executable)","chmod u+x upx && ./upx",github.strip(),{"UPX README":"https://github.com/upx/upx#readme","UPX Video - 1 ":"https://www.youtube.com/watch?v=upTXpDhI0ww"},method = "github", github_install = "wget --no-verbose https://github.com/upx/upx/releases/download/v4.0.1/upx-4.0.1-i386_linux.tar.xz 2>/dev/null && tar -xf upx-4.0.1-i386_linux.tar.xz && rm upx-4.0.1-i386_linux.tar.xz", github_check = "upx-4.0.1-i386_linux")    
-        elif option=="13":
-            print("\n[+] Covermyass")
-            os.system("clear")
-            github=github_getting_text("https://github.com/sundowndev/covermyass",'p[dir="auto"]',1)
-            template.template("Covermyass","chmod u+x covermyass_linux_amd64 && ./covermyass_linux_amd64",github.strip(),{"CoverMyAss README":"https://github.com/sundowndev/covermyass/blob/master/README.md","Clearing or Removing Tracks":"https://b14cky-notes.gitbook.io/untitled/"},method = "github", github_install = "wget --no-verbose https://github.com/sundowndev/covermyass/releases/download/v2.0.0-beta5/covermyass_linux_amd64 2>/dev/null && mkdir Covermyass && mv covermyass_linux_amd64 Covermyass", github_check = "Covermyass")    
+            upx()        
         else:
             return
-def github_getting_text(link,selector,indexvalue):
-    print("Please Wait....\r",end="")
+
+
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
     URL = link
-    # try:
-    r = requests.get(URL)
-    soup = BeautifulSoup(r.content, 'html.parser')
-    paras = soup.select(selector)
-    #check index value from test file
-    return paras[indexvalue].text
-    # except:
-    #     return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
+    try:
+        r = requests.get(URL)
+        soup = BeautifulSoup(r.content, 'html.parser')
+        paras = soup.select(selector)
+        # check index value from test file
+        return paras[indexvalue].text
+    except:
+         return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
+
+
+def upx():
+    os.system("clear")
+    github = "UPX is a free, portable, extendable, high-performance executable packer for several different executable formats. It can be used to compress and obfuscate executable files to make them smaller and more difficult to reverse engineer. UPX supports a wide range of file formats, including Windows PE, Linux ELF, and more. UPX is available for a variety of platforms, including Windows, Linux, and macOS. The UPX compression algorithm is designed to compress the code section of an executable file, while leaving the data section uncompressed. This allows the compressed code to be executed directly from memory without the need to decompress it first. UPX is open-source and actively maintained, with updates and bug fixes released regularly."
+    template.template("UPX (Ultimate Packer for Executable)", "chmod u+x upx && ./upx", github.strip(), {"UPX README": "https://github.com/upx/upx#readme", "UPX Video - 1 ": "https://www.youtube.com/watch?v=upTXpDhI0ww"}, method="github",
+                              github_install="wget  https://github.com/upx/upx/releases/download/v4.0.1/upx-4.0.1-i386_linux.tar.xz  && tar -xf upx-4.0.1-i386_linux.tar.xz && rm upx-4.0.1-i386_linux.tar.xz", github_check="upx-4.0.1-i386_linux")
+        
+def shelter():
+    os.system("clear")
+    github = "Shellter is a dynamic shellcode injection tool aka dynamic PE infector. It can be used in order to inject shellcode into native Windows applications (currently 32-bit apps only). The shellcode can be something yours or something generated through a framework, such as Metasploit. Shellter takes advantage of the original structure of the PE file and doesn't apply any  modification such as changing memory access permissions in sections (unless the user wants to), adding an extra section with RWE access, and whatever would look dodgy under an AV scan. Shellter is not just an EPO infector that tries to find a location to insert an instruction to redirect execution to the payload. Unlike any other infector, Shellter’s advanced infection engine never transfers the execution flow to a code cave or to an added section in the infected PE file. Shellter uses a unique dynamic approach which is based on the execution flow of the target application. This means that no static/predefined locations are used for shellcode injection. Shellter will launch and trace the target, while at the same time will log the execution flow of the application."
+    template.template("shellter", "shellter", github.strip(), {"Introduction to Shellter": "https://github.com/ParrotSec/shellter#readme", "Tool documentation for Shellter on Kali Linux": "https://www.kali.org/tools/shellter/#tool-documentation", "Anti-virus Bypass with Shellter 5.1 on Kali Linux": "https://cyberarms.wordpress.com/2015/10/04/anti-virus-bypass-with-shellter-5-1-on-kali-linux/",
+                              "Shellter: A Shellcode Injecting Tool": "https://www.hackingarticles.in/shellter-a-shellcode-injecting-tool/", "Shellter - The Ultimate Tool for AV Evasion": "https://metalkey.github.io/shellter---the-ultimate-tool-for-av-evasion.html", "Hack like a Pro: Evade AV Software with Shellter": "https://null-byte.wonderhowto.com/how-to/hack-like-pro-evade-av-software-with-shellter-0168504/"})
+        
+def linux_private_i():
+    os.system("clear")
+    github = "A Linux Enumeration & Privilege Escalation tool that automates the basic enumeration steps and displays the results in an easily readable format. The script comes loaded with a variety of 4 Options to choose from. Using Bash, execute private-i.sh on the local low privileged user. Select an option, execute & watch the show. Each mode uses common Linux binaries to enumerate the local system (find, grep, ps, etc). If you have a non-bash shell such as sh, use Noir-Private-i. Either script will not write or auto-exploit in any way"
+    template.template("linux-private-i", "./private-i.sh", github.strip(), {"Documentation": "https://github.com/rtcrowley/linux-private-i/blob/master/README.md", "HackingArticles-linux-privilege-escalation-automated-script":
+                              "https://www.hackingarticles.in/linux-privilege-escalation-automated-script"}, method="github", github_install="git clone https://github.com/rtcrowley/linux-private-i.git && cd linux-private-i && chmod +x *", github_check="linux-private-i")
+        
+def pspy():
+    os.system("clear")
+    github = "pspy is a command line tool designed to snoop on processes without need for root permissions. It allows you to see commands run by other users, cron jobs, etc. as they execute. Great for enumeration of Linux systems in CTFs. Also great to demonstrate your colleagues why passing secrets as arguments on the command line is a bad idea.This tool gathers the info from procfs scans. Inotify watchers placed on selected parts of the file system trigger these scans to catch short-lived processes."
+    version = github_getting_text("https://github.com/DominicBreuker/pspy/releases/",
+                                          'div[class="css-truncate css-truncate-target"]', 0).strip()
+    template.template("pspy64", "chmod u+x pspy64 && ./pspy64", github.strip(), {"Using-PSPY-To-Monitor-Linux-Processes": "https://infinitelogins.com/2020/09/04/using-ps-py-to-monitor-linux-processes", "Cyberkendra Pspy-Tool-Monitor-Linux-Processes": "https://tools.cyberkendra.com/2020/04/pspy-tool-monitor-linux-processes.html", "How-To-Enumerate-Services-In-Use-With-PSPY": "https://vk9-sec.com/how-to-enumerate-services-in-use-with-pspy",
+                              "TryHackMe-ConvertMyVideo Writeup": "https://sparshjazz.medium.com/tryhackme-convertmyvideo-writeup-56b6c8217001", "SecurityOnline PSPY": "https://securityonline.info/pspy"}, method="github", github_install=f"wget  https://github.com/DominicBreuker/pspy/releases/download/{version}/pspy64 && mkdir PSPY && mv pspy64 PSPY", github_check="PSPY")
+        
+def linux_smart_enumeration():
+    os.system("clear")
+    github = "Linux Smart Enumeration (LSE) is a script written by Diego Treitos that automates the enumeration process for Linux systems. It is designed to run quickly and efficiently, and to provide detailed information about the system, including users, groups, permissions, network configuration, and more. LSE is intended to be used by penetration testers and security professionals to gather information about a target system during the reconnaissance phase of an engagement."
+    template.template("linux-smart-enumeration", "chmod u+x lse.sh && ./lse.sh", github.strip(), {"Documentation (linux-smart-enumeration)": "https://github.com/diego-treitos/linux-smart-enumeration/blob/master/README.md", "Use-Linux-Smart-Enumeration-Discover-Paths-Privesc":
+                              "https://null-byte.wonderhowto.com/how-to/use-linux-smart-enumeration-discover-paths-privesc-0330807", "Hakin9 linux-smart-enumeration": "https://hakin9.org/linux-smart-enumeration"}, method="github", github_install="git clone https://github.com/diego-treitos/linux-smart-enumeration.git", github_check="linux-smart-enumeration")
+        
+def linux_exploit_suggester2():
+    os.system("clear")
+    github = "Linux Exploit Suggester 2 (LES 2) is a tool that can be used to identify potential vulnerabilities and exploits that can be used to compromise a Linux system. It works by analyzing the running kernel version and system information, and then comparing it to a local database of known vulnerabilities and exploits. LES 2 can also be used to determine whether a patch has been applied to a specific vulnerability, making it useful for identifying systems that are still vulnerable to known exploits. The tool is open-source and can be easily installed on a Linux system. It supports a wide range of Linux distributions, including Ubuntu, Debian, Fedora, Arch Linux and more. LES 2 is a command-line tool and requires Python to run.It's a useful tool for penetration testers and system administrators to identify and prioritize vulnerabilities on their systems."
+    template.template("linux-exploit-suggester-2", "chmod u+x linux-exploit-suggester-2.pl && ./linux-exploit-suggester-2.pl", github.strip(), {"Kali Tools (linux-exploit-suggester)": "https://www.kali.org/tools/linux-exploit-suggester/", "Find-Exploits-Get-Root-With-Linux-Exploit-Suggester": "https://null-byte.wonderhowto.com/how-to/find-exploits-get-root-with-linux-exploit-suggester-0206005", "Pentest-Monkey Linux-Exploit-Suggester": "https://pentestmonkey.net/tools/audit/exploit-suggester",
+                              "Linux-Exploit-Suggester-A-Kali-Linux-Tool-To-Find-The-Linux-Os-Kernel-Exploits": "https://gbhackers.com/linux-exploit-suggester-a-kali-linux-tool-to-find-the-linux-os-kernel-exploits", "Securityonline Linux-Exploit Suggester": "https://securityonline.info/linux-exploit-suggester-2"}, method="github", github_install="git clone https://github.com/jondonas/linux-exploit-suggester-2.git", github_check="linux-exploit-suggester-2")
+        
+def beroot():
+    os.system("clear")
+    github_text_0 = github_getting_text(
+                "https://github.com/AlessandroZ/BeRoot", 'p[dir=auto]', 0)
+    github_text_1 = github_getting_text(
+                "https://github.com/AlessandroZ/BeRoot", 'p[dir=auto]', 1)
+    github = github_text_0 + github_text_1
+    template.template("BeRoot", "cd Linux && chmod u+x * && ./beroot.py", github.strip(), {"BeRoot-Linux-Privilege-Escalation": "https://www.kitploit.com/2018/06/beroot-for-linux-privilege-escalation.html?m=0", "BeRoot-A-Post-Exploitation-Privilege-Escalation-Tool":
+                              "https://blog.hackersonlineclub.com/2018/07/beroot-post-exploitation-tool-to-check.html", "BeRoot-Windows-Privilege-Escalation": "https://sevenlayers.com/index.php/273-windows-privilege-escalation"}, method="github", github_install="git clone https://github.com/AlessandroZ/BeRoot.git", github_check="BeRoot")
+        
+def sudokiller():
+    os.system("clear")
+    github_text_6 = github_getting_text(
+                "https://github.com/TH3xACE/SUDO_KILLER", 'p[dir=auto]', 6)
+    github_text_7 = github_getting_text(
+                "https://github.com/TH3xACE/SUDO_KILLER", 'p[dir=auto]', 7)
+    github = github_text_6 + github_text_7
+    template.template("Sudo Killer", "chmod u+x * && ./SUDO_KILLERv2.4.2.sh", github.strip(), {"SUDO_KILLER-Demos": "https://github.com/TH3xACE/SUDO_KILLER#demos", "Sudo-Killer Information": "https://www.kitploit.com/2020/02/sudokiller-tool-to-identify-and-exploit.html",
+                              "Sudo-Killer-Identify-Abuse-Sudo-Misconfigurations": "https://null-byte.wonderhowto.com/how-to/use-sudo-killer-identify-abuse-sudo-misconfigurations-0202594"}, method="github", github_install="git clone https://github.com/TH3xACE/SUDO_KILLER.git", github_check="SUDO_KILLER")
+        
+def linenum():
+    os.system("clear")
+    github = "LinEnum is a Linux enumeration script that can be used to enumerate information from a Linux system. It is designed to be run locally on a Linux system and will attempt to enumerate common files, folders, users, groups, services, configurations, and permissions. It can also be used to look for certain security vulnerabilities such as local privilege escalation. LinEnum can be run from the command line or can be automated using a script. The output of the script can be saved as a text file for later analysis."
+    template.template("LinEnum", "chmod +x LinEnum.sh && ./LinEnum.sh -h", github.strip(), {"Use-LinEnum-Identify-Potential-Privilege-Escalation-Vectors": "https://null-byte.wonderhowto.com/how-to/use-linenum-identify-potential-privilege-escalation-vectors-0197225/", "Linux-Privilege-Escalation-With-LinEnum": "https://trevorxcohen.medium.com/linux-privilege-escalation-with-linenum-75d20a3b59f6", "LinEnum-Linux-Enumeration-Privilege-Escalation-Tool": "https://www.darknet.org.uk/2014/11/linenum-linux-enumeration-privilege-escalation-tool",
+                              "Linux-Privilege-Escalation-Quick-And-Dirty": "https://reboare.gitbooks.io/booj-security/content/general-linux/privilege-escalation.html", "Linux Enumeration And Privilege Escalation – LinEnum": "https://vulners.com/n0where/N0WHERE:24819"}, method="github", github_install="curl -s https://raw.githubusercontent.com/rebootuser/LinEnum/master/LinEnum.sh -o LinEnum.sh && mkdir LinEnum && mv LinEnum.sh LinEnum", github_check="LinEnum")
+        
+def linpeas():
+    os.system("clear")
+    github = "LinPeas is a script that automates the process of gathering information about a Linux system, similar to Windows' PowerShell script PEAS. This script can help identify potential vulnerabilities and misconfigurations on a Linux system, as well as provide information about system and network configuration. It can be useful for penetration testing, security assessments, and incident response. The script can be executed with arguments to specify which information to gather, or without arguments to gather all available information"
+    template.template("linPEAS", "chmod +x linpeas.sh && ./linpeas.sh -h", github.strip(), {"LinPeas Blog": "https://blog.cyberethical.me/linpeas", "Linux-Privilege-Escalation": "https://delinea.com/blog/linux-privilege-escalation", "Linux Privilege Escalation: Quick and Dirty": " https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS", "Outrunsec LinPeas":
+                              "https://outrunsec.com/tag/linpeas/", "Linux-Privilege-Escalation-Suid-Binaries": "https://steflan-security.com/linux-privilege-escalation-suid-binaries"}, method="github", github_install="wget https://github.com/carlospolop/PEASS-ng/releases/latest/download/linpeas.sh  && mkdir LinPeas && mv linpeas.sh LinPeas", github_check="LinPeas")
+        
 
-if __name__=='__main__':
+if __name__ == '__main__':
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/RiskyFuncPayment.py` & `cyberonix-3.0.0/cyberonix/main/tools/information_gathering.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,228 +1,346 @@
-from cyberonix.main.tools import banner, colors, template,WEB_Application_Analysis
-from cyberonix.main import Cheat_sheet
-import os
-import requests
-from bs4 import BeautifulSoup
-
-
-# main function
-def main():
-    while True:
-        os.system("clear")
-        banner.main()
-        banner.attack("Risky Functionality Card Payment")
-        list_attacks = ["Tools", "Writeups", "Go Back"]
-        for i in range(len(list_attacks)):
-            print(colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset)
-        try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
-        except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
-            while True:
-                print("\n[+] Tools")
-                os.system("clear")
-                banner.main()
-                banner.attack("Tools")
-                list_attacks = [
-                    "Burp Suite",
-                    "Wireshark",
-                    "OWASP ZAP",
-                    "Nessus",
-                    "Sqlmap",
-                    "Fiddler",
-                    "Metasploit",
-                    "Nmap",
-                    "Penetration Testers Framework (PTF)",
-                    "Go Back",
-                ]
-                for i in range(len(list_attacks)):
-                    print(
-                        colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset
-                    )
-                try:
-                    option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
-                except KeyboardInterrupt:
-                    template.exit_program()
-                if option == "0":
-                    os.system("clear")
-                    WEB_Application_Analysis.burp_suite()
-                elif option == "1":
-                    os.system("clear")
-                    github = "Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. It can be used to examine data from a live network or from a previously saved capture file. Wireshark provides a graphical user interface (GUI) for capturing and analyzing network traffic."
-                    template.template(
-                        "wireshark",
-                        "wireshark",
-                        github.strip(),
-                        {
-                            "Wireshark Cheat-Sheet": "https://www.comparitech.com/net-admin/wireshark-cheat-sheet",
-                            "What-is-Wireshark-and-How-to-Use-it": "https://www.comptia.org/content/articles/what-is-wireshark-and-how-to-use-it ",
-                            "Video Resource Wireshark": "https://www.youtube.com/playlist?list=PLBf0hzazHTGPgyxeEj_9LBHiqjtNEjsgt",
-                        },
-                    )
-                elif option == "2":
-                    os.system("clear")
-                    github = "The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.\nIt is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox."
-                    template.template(
-                        "zaproxy",
-                        "zaproxy > /dev/null 2>&1",
-                        github.strip(),
-                        {
-                            "How to setup OWASP ZAP to scan your web application for security vulnerabilities": "https://www.linkedin.com/pulse/how-setup-owasp-zap-scan-your-web-application-security-botla/",
-                            "Authenticated Scan using OWASP-ZAP": "https://medium.com/@secureica/authenticated-scan-using-owasp-zap-f0a71dafe41",
-                            "OWASP ZAP: 6 Key Capabilities and a Quick Tutorial": "https://www.hackerone.com/knowledge-center/owasp-zap-6-key-capabilities-and-quick-tutorial",
-                            "Initial Setup": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/untitled",
-                            "Setup OWASP ZAP": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/setup-owasp-zap",
-                        },
-                    )
-                elif option == "3":
-                    os.system("clear")
-                    github = github_getting_text(
-                        "https://www.techtarget.com/searchnetworking/definition/Nessus",
-                        'section[id="content-body"]',
-                        0,
-                    )
-                    template.template(
-                        "nessus",
-                        "nessus",
-                        github.strip(),
-                        {
-                            "How To: Run Your First Vulnerability Scan with Nessus": "https://www.tenable.com/blog/how-to-run-your-first-vulnerability-scan-with-nessus",
-                            "A brief introduction to the Nessus vulnerability scanner": "https://resources.infosecinstitute.com/topic/a-brief-introduction-to-the-nessus-vulnerability-scanner/",
-                            "Beginner’s Guide to Nessus": "https://www.hackingarticles.in/beginners-guide-to-nessus/",
-                            "Nessus Ubuntu Installation and Tutorial": "https://linuxhint.com/nessus-ubuntu-installation-tutorial/",
-                        },
-                        link="https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.4.2-debian9_amd64.deb",
-                        method="deb",
-                    )
-                elif option == "4":
-                    os.system("clear")
-                    github = github_getting_text("https://sqlmap.org/", "p", 0)
-                    template.template(
-                        "sqlmap",
-                        "sqlmap -h",
-                        github.strip(),
-                        {
-                            "Usage Of Sqlmap": "https://github.com/sqlmapproject/sqlmap/wiki/Usage",
-                            "How to use SQLMAP to test a website for SQL Injection vulnerability": "https://www.geeksforgeeks.org/use-sqlmap-test-website-sql-injection-vulnerability/",
-                            "How to Use SQLMap to Find Database Vulnerabilities": "https://www.freecodecamp.org/news/how-to-protect-against-sql-injection-attacks/",
-                            "SQLMap - Cheetsheat": "https://book.hacktricks.xyz/pentesting-web/sql-injection/sqlmap",
-                        },
-                    )
-                elif option == "5":
-                    os.system("clear")
-                    github = github_getting_text(
-                        "https://learn.microsoft.com/en-us/windows/win32/win7appqual/fiddler-web-debugger-tool/",
-                        "p",
-                        2,
-                    )
-                    template.template(
-                        "Fiddler",
-                        "chmod u+x fiddler-everywhere-4.1.2.AppImage && su -c ./fiddler-everywhere-4.1.2.AppImage $SUDO_USER > /dev/null 2>&1",
-                        github.strip(),
-                        "no-writeups",
-                        method="github",
-                        github_install="wget -q --show-progress https://downloads.getfiddler.com/linux/fiddler-everywhere-4.1.2.AppImage && mkdir Fiddler_Everywhere && mv fiddler-everywhere-4.1.2.AppImage Fiddler_Everywhere",
-                        github_check="Fiddler_Everywhere",
-                    )
-                elif option == "6":
-                    os.system("clear")
-                    github = "The Metasploit Framework is an open-source tool for developing and executing exploit code against a remote target machine. It can be used to test the security of a computer system by finding and exploiting vulnerabilities. The framework includes a large collection of exploit modules, as well as various tools for payload generation, post-exploitation, and more. It can be used by security professionals for penetration testing, as well as by attackers for malicious purposes."
-                    template.template(
-                        "metasploit-framework",
-                        "msfconsole",
-                        github.strip(),
-                        {
-                            "Msf-Community-Post-Exploitation": "https://www.offensive-security.com/metasploit-unleashed/msf-community-post-exploitation",
-                            "Post Exploitation In Linux With Metasploit": "https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/",
-                            "Privilege Escalation (Metasploit Unleashed)": "https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/",
-                            "Post Exploitation Metasploit Modules (Reference)": "https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference",
-                            "PSExec Pass the Hash (Horizontal Escalation)": "https://www.offensive-security.com/metasploit-unleashed/psexec-pass-hash/",
-                            "ms10_002_aurora (Vertical Escalation)": "https://www.offensive-security.com/metasploit-unleashed/privilege-escalation/",
-                            "ms10_002_aurora (Horizontal Escalation)": "https://www.offensive-security.com/metasploit-unleashed/pivoting/ ",
-                            "jtr_crack_fast (Hash Cracking)": "https://www.offensive-security.com/metasploit-unleashed/john-ripper/",
-                            "warftpd_165_user (Keylogging)": "https://www.offensive-security.com/metasploit-unleashed/keylogging/",
-                            "3proxy (Backdoor)": "https://www.offensive-security.com/metasploit-unleashed/meterpreter-backdoor/",
-                            "persistence.rb (Persistent Backdoor)": "https://www.offensive-security.com/metasploit-unleashed/meterpreter-service/",
-                            "Enabling Remote Desktop": "https://www.offensive-security.com/metasploit-unleashed/enabling-remote-desktop/",
-                            "Post Exploitation in Linux with Metasploit": "https://pentestlab.blog/2013/01/04/post-exploitation-in-linux-with-metasploit/",
-                            "Post Exploitation Metasploit Modules Reference": "https://www.infosecmatter.com/post-exploitation-metasploit-modules-reference/",
-                            "Hack Like Pro: Kill and Disable Antivirus Software Remote PC": "https://null-byte.wonderhowto.com/how-to/hack-like-pro-kill-and-disable-antivirus-software-remote-pc-0141906/",
-                            "Armitage Post Exploitation": "https://www.offensive-security.com/metasploit-unleashed/armitage-post-exploitation/",
-                            "Setup Armitage as a Command & Control Framework for Free": "https://infosecwriteups.com/setup-armitage-as-a-command-control-c2-framework-for-free-bae590064817",
-                            "Event Log Management": "https://www.offensive-security.com/metasploit-unleashed/event-log-management",
-                            "Interacting with the Registry": "https://www.offensive-security.com/metasploit-unleashed/interacting-registry",
-                        },
-                    )
-                elif option == "7":
-                    os.system("clear")
-                    github = "Nmap (Network Mapper) is a network scanner created by Gordon Lyon (also known by his pseudonym Fyodor Vaskovich). Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses."
-                    template.template(
-                        "nmap",
-                        "nmap",
-                        github.strip(),
-                        {
-                            "Nmap Cheat-Sheet": "https://www.stationx.net/nmap-cheat-sheet/",
-                            "Official website": "https://nmap.org/ ",
-                            "Other resources": "https://linux.die.net/man/1/nmap",
-                        },
-                    )
-                elif option == "8":
-                    os.system("clear")
-                    github = "The PenTesters Framework (PTF) is a Python script designed for Debian/Ubuntu/ArchLinux based distributions to create a similar and familiar distribution for Penetration Testing. PTF attempts to install all of your penetration testing tools (latest and greatest), compile them, build them, and make it so that you can install/update your distribution on any machine. Everything is organized in a fashion that is cohesive to the Penetration Testing Execution Standard (PTES) and eliminates a lot of things that are hardly used"
-                    template.template(
-                        "Penetration Testers Framework (PTF)",
-                        "chmod +x ptf && ./ptf",
-                        github.strip(),
-                        "no-writeups",
-                        method="github",
-                        github_install="git clone https://github.com/trustedsec/ptf.git",
-                        github_check="ptf",
-                    )
-                else:
-                    break
-
-        elif option == "1":
-            os.system("clear")
-            banner.main()
-            Cheat_sheet.cheat(
-                {
-                    "Exploiting Payment Gateways": "https://vasuyadav0786.medium.com/exploiting-payment-gateways-97ce7af5a9cf",
-                    "Let's Break Into Payment Gateways": "https://infosecwriteups.com/lets-break-into-payment-gateways-fc52523eeaca",
-                    "Common Vulnerabilities in Payment Functionality": "https://dl.packetstormsecurity.net/papers/general/common-vulnerabilities.pdf",
-                    "Bug Bounty Response Manipulation Leading to Payment Bypass": "https://infosecwriteups.com/bug-bounty-response-manipulation-leading-to-payment-bypass-cb5fde360b1a",
-                    "Web Application Security Testing - Testing Payment Functionality": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/10-Business_Logic_Testing/10-Test-Payment-Functionality",
-                    "Application Security Testing Techniques - Testing Payment Functionality": "https://www.softwaretestinghelp.com/how-to-test-application-security-web-and-desktop-application-security-testing-techniques/",
-                    "Parameter Tampering Vulnerability Using 3 Different Approaches": "https://www.cobalt.io/blog/parameter-tampering-vulnerability-using-3-different-approaches",
-                    "Webinar: Understanding Payment Gateway Related Vulnerabilities": "https://www.youtube.com/watch?v=oin2fplOazU",
-                    "Payment Gateway Security Measures Overview": "https://yashsali7.medium.com/an-overview-of-security-measures-used-in-payment-gateways-86375eb12364",
-                    "Payment Bypass Vulnerability on BigBasket": "https://medium.com/@ranjeetjagtap25/payment-bypass-vulnerability-on-bigbasket-2aab137e9631",
-                    "Security Features of Payment Gateway": "https://www.ukessays.com/essays/information-technology/security-features-of-payment-gateway-information-technology-essay.php",
-                    "Vulnerabilities in Electronic Payment Systems (EPS)": "https://www.linkedin.com/pulse/vulnerabilities-eps-electronic-payment-systems-from-david-joao-",
-                    "Security Threats to E-Commerce": "https://www.javatpoint.com/security-threat-to-e-commerce",
-                    "Visa's 3-D Secure Secure Online Payment Authentication": "https://www.giac.org/paper/gsec/4380/visa-039-s-3-d-secure-secure-online-payment-authentication/107245",
-                    "Researching Xiaomi's TEE": "https://research.checkpoint.com/2022/researching-xiaomis-tee/",
-                    "JazzCash Payment Gateway in PHP (Prevent Amount Tampering)": "https://www.youtube.com/watch?v=JEvYSlwb-yY",
-                },
-                " Risky Functionality Payment Systems Write-UPS",
-            )
-
-        else:
-            return
-
-
-def github_getting_text(link, selector, indexvalue):
-    print("Please Wait....\r", end="")
-    URL = link
-    try:
-        r = requests.get(URL)
-        soup = BeautifulSoup(r.content, "html.parser")
-        paras = soup.select(selector)
-        # check index value from test file
-        return paras[indexvalue].text
-    except:
-        return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
-
-
-if __name__ == "__main__":
-    main()
+from xml.dom.minidom import parse
+from cyberonix.main.tools import banner, colors, template
+import os
+import requests
+from bs4 import BeautifulSoup
+
+
+def main():
+    while True:
+        os.system("clear")
+        banner.main()
+        banner.attack("Information_gathering")
+        list_attacks = [
+            " Useful Website",
+            " Nmap     \t\t (Recommended)",
+            " subfinder \t\t (Recommended)",
+            " Maltego \t\t (Recommended)",
+            " Dracnmap",
+            " RED_HAWK",
+            " Th3inspector \t (Recommended)",
+            " Hping3",
+            " Arping",
+            "Netdiscover",
+            "The Harvester",
+            "Wafw00f",
+            "Recon-ng",
+            "Spiderfoot",
+            "amass",
+            "Sublist3r",
+            "go back",
+        ]
+        for i in range(len(list_attacks)):
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
+        try:
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
+        except KeyboardInterrupt:
+            return
+        if option == "1":
+            print("\n[+] Useful Websites")
+            os.system("clear")
+            template.template("Useful Websites", "no-tools", 'This is website for information gathering', {
+                " Social-Search Website": "https://www.social-searcher.com/",
+                " IP2info": "https://ipinfo.io/",
+                " Viewdns": "https://viewdns.info/",
+                " Shodan search engine": "https://www.shodan.io/",
+                " Hunter Search Engine": "https://hunter.how/",
+                " AHMIA Search Engine": "https://ahmia.fi/",
+                " Censys Search Engine": "https://censys.com/",
+                " Wayback Machine": "https://archive.org/web/",
+                " Dnsdumpster": "https://dnsdumpster.com/",
+                "MXToolbox": "https://mxtoolbox.com/",
+                "Lopseg": "https://www.lopseg.com.br/osint",
+                "Arin whois": "https://whois.arin.net/ui/",
+                "Dnschecker": "https://dnschecker.org/",
+                "BGP-Toolkit": "https://bgp.he.net/",
+                "Mattw.io": "https://mattw.io/",
+                "Searchftps": "https://www.searchftps.net/",
+                "Security Headers": "https://securityheaders.com/",
+                "Robtex": "https://www.robtex.com/",
+                "Builtwith": "https://builtwith.com/",
+                "Intodns": "https://www.intodns.com/",
+                "Serachdns": "https://searchdns.netcraft.com/",
+                "Hackertarget": "https://hackertarget.com/",
+                "Vulners": "https://vulners.com/",
+                "cvedetails": "https://www.cvedetails.com/",
+                "Zero Day initiative": "https://www.zerodayinitiative.com/",
+
+
+            })
+
+        elif option == "2":
+            print("\n[+] Nmap")
+            nmap()
+        elif option == "3":
+            print("\n[+] subfinder")
+            subfinder()
+        elif option == "4":
+            print("\n[+] Maltego")
+            maltego()
+        elif option == "5":
+            print("\n[+] Dracnmap")
+            dracnmap()
+        elif option == "6":
+            print("\n[+] RED_HAWK")
+            redhawk()
+        elif option == "7":
+            print("\n[+] Th3inspector")
+            th3inspector()
+        elif option == "8":
+            print("\n[+] Hping3")
+            hping3()
+        elif option == "9":
+            print("\n[+] Arping")
+            arping()
+        elif option == "10":
+            print("\n[+] Netdiscover")
+            netdiscover()
+        elif option == "11":
+            print("\n[+] The Harvester")
+            theharvester()
+        elif option == "12":
+            print("\n[+] Wafw00f")
+            wafw00f()
+        elif option == "13":
+            print("\n[+] Recon-ng")
+            recon_ng()
+        elif option == "14":
+            print("\n[+] spiderfoot")
+            spiderfoot()
+        elif option == "15":
+            print("\n[+] amass")
+            amass()
+        elif option == "16":
+            print("\n[+] Sublist3r")
+            sublist3r()
+        else:
+            return
+
+
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
+    URL = link
+    headers={'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'}
+    try:
+        r = requests.get(URL,headers=headers)
+        soup = BeautifulSoup(r.content, "html.parser")
+        paras = soup.select(selector)
+    #for i in paras:
+    #    print(i.text)
+    # check index value from test file
+        return paras[indexvalue].text
+    except:
+        return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
+
+def arping():
+    os.system("clear")
+    github = "arping is a tool for probing hosts in a network. Unlike the ping command, which operates at the network layer, arping operates at the data link layer and uses the Address Resolution Protocol (ARP). Using it involves sending ARP requests to a destination host and waiting for ARP replies."        
+    template.template(
+                "arping",
+                "arping --help",
+                github.strip(),
+                {
+                    "First resource": "https://www.networkworld.com/article/3601693/using-the-linux-arping-command-to-ping-local-systems.html",
+                    "How to use this command": "https://linuxhint.com/use-arping-command-linux/",
+                    "Other resources": "https://www.baeldung.com/linux/arping-command",
+                },
+            )
+def wafw00f():
+    os.system("clear")
+    github = "WAFW00F is a Python tool to help you fingerprint and identify Web Application Firewall (WAF) products. It is an active reconnaissance tool as it actually connects to the web server, but it starts out with a normal HTTP response and escalates as necessary."
+    template.template(
+                "wafw00f",
+                "wafw00f --help",
+                github.strip(),
+                {
+                    "First resource": "https://www.briskinfosec.com/tooloftheday/toolofthedaydetail/wafw00f-tool-to-fingerprint-and-identify-web-application-firewall",
+                    "Second resource": "https://null-byte.wonderhowto.com/how-to/identify-web-application-firewalls-with-wafw00f-nmap-0198145/",
+                    "Third resource": "https://www.geeksforgeeks.org/identification-of-web-application-firewall-using-wafw00f-in-kali-linux/",
+                    "Github resource": "https://github.com/EnableSecurity/wafw00f",
+                    "Video resource": "https://www.youtube.com/watch?v=EmWXfq51pE0",
+                },
+            )
+
+
+def nmap():
+    os.system("clear")
+    github = "Nmap (Network Mapper) is a network scanner created by Gordon Lyon (also known by his pseudonym Fyodor Vaskovich). Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses. "
+    template.template("nmap", "nmap -h", github.strip(), {"Nmap Cheat-Sheet": "https://www.stationx.net/nmap-cheat-sheet/",
+                      "Official website": "https://nmap.org/ ", "Other resources": "https://linux.die.net/man/1/nmap", },)
+
+
+def recon_ng():
+    os.system("clear")
+    github_p1 = github_getting_text(
+        "https://github.com/lanmaster53/recon-ng", 'p[dir=auto]', 1)
+    github_p2 = github_getting_text(
+        "https://github.com/lanmaster53/recon-ng", 'p[dir=auto]', 2)
+    github = github_p1+github_p2
+    template.template("recon-ng", "recon-ng --help", github.strip(),
+                      {"How to us Reco-ng": "https://hackertarget.com/recon-ng-tutorial/", },)
+
+
+def theharvester():
+    os.system("clear")
+    github = "theHarvester is a simple to use, yet powerful tool designed to be used during the reconnaissance stage of a red team assessment or penetration test. It performs open source intelligence (OSINT) gathering to help determine a domain's external threat landscape. The tool gathers names, emails, IPs, subdomains, and URLs by using multiple public resources that include."
+    template.template(
+        "theharvester",
+        "theharvester",
+        github.strip(),
+        {
+            "The harvester CheatSheet": "https://cheatography.com/classassignment124/cheat-sheets/theharvester-cheat-sheet/",
+            "How to use ": "https://thecybersecurityman.com/2018/08/01/pentest-edition-using-theharvester-to-gather-e-mail-accounts-subdomains-hosts-linkedin-users-banner-information-and-more/",
+            "Information Gathering using theHarvester in Kali Linux": "https://www.hacking-tutorial.com/tips-and-trick/information-gathering-using-theharvester-in-kali-linux/#google_vignette",
+            "theHarvester: a Classic Open Source Intelligence Tool": "https://securitytrails.com/blog/theharvester-tool",
+            "The Harvester OSINT Reconnaissance": "https://medium.com/hacker-toolbelt/the-harvester-osint-reconnaissance-91a18a294a30", },)
+
+
+def subfinder():
+    os.system("clear")
+    github = "subfinder is a subdomain discovery tool that returns valid subdomains for websites, using passive online sources. It has a simple, modular architecture and is optimized for speed. subfinder is built for doing one thing only - passive subdomain enumeration, and it does that very well."
+    template.template(
+        "subfinder",
+        "subfinder",
+        github.strip(),
+        {
+            "subfinder CheatSheet": "https://highon.coffee/blog/subfinder-cheat-sheet/",
+            "How to use ": "https://blog.projectdiscovery.io/do-you-really-know-subfinder-an-in-depth-guide-to-all-features-of-subfinder-beginner-to-advanced/",
+            "Uncover the Hidden Web: Discover the Power of Subfinder for Efficient Subdomain Enumeration": "https://medium.com/@cuncis/uncover-the-hidden-web-discover-the-power-of-subfinder-for-efficient-subdomain-enumeration-aad6fc05bcdd", },)
+
+
+def sublist3r():
+    os.system("clear")
+    github = "Sublist3r is a python tool designed to enumerate subdomains of websites using OSINT. It helps penetration testers and bug hunters collect and gather subdomains for the domain they are targeting. Sublist3r enumerates subdomains using many search engines such as Google, Yahoo, Bing, Baidu and Ask. Sublist3r also enumerates subdomains using Netcraft, Virustotal, ThreatCrowd, DNSdumpster and ReverseDNS."
+    template.template(
+        "sublist3r",
+        "sublist3r -h",
+        github.strip(),
+        {
+            "Sublist3r Cheatsheet": "https://github.com/shreyaschavhan/pentest-tools-cheatsheet/blob/main/sublist3r.md",
+            "Sublist3r – Fast Subdomains Enumeration Tool for Penetration Testers": "https://pentesttools.net/sublist3r-fast-subdomains-enumeration-tool-for-penetration-testers/", },)
+
+
+def spiderfoot():
+    os.system("clear")
+    github = github_getting_text(
+        "https://github.com/smicallef/spiderfoot", 'p[dir=auto]', 2)
+    template.template(
+        "spiderfoot",
+        "spiderfoot --help",
+        github.strip(),
+        {
+            "How to use Spiderfoot ": "https://www.geeksforgeeks.org/spiderfoot-a-automate-osint-framework-in-kali-linux/",
+        },)
+
+
+def amass():
+    os.system("clear")
+    github = "The OWASP Amass Project performs network mapping of attack surfaces and external asset discovery using open source information gathering and active reconnaissance techniques."
+    template.template(
+        "amass",
+        "amass --help",
+        github.strip(),
+        {
+            "Amass tutorial": "https://techyrick.com/amass-full-tutorial/",
+            "How to use amass ": "https://blog.intigriti.com/2021/06/08/hacker-tools-amass-hunting-for-subdomains/",
+            "amass user's guide": "https://github.com/owasp-amass/amass/blob/master/doc/user_guide.md", },)
+
+
+def netdiscover():
+    os.system("clear")
+    github = "Netdiscover is a command-line oriented TCP/IP packet assembler/analyzer. It supports TCP, UDP, ICMP and RAW-IP protocols, has a traceroute mode, the ability to send files between a covered channel, and many other features."
+    template.template(
+        "netdiscover",
+        "netdiscover -help",
+        github.strip(),
+        {
+            "Usage in details": "https://linuxcommandlibrary.com/man/netdiscover",
+            "Second resource": "https://www.cyberpratibha.com/blog/netdiscover/",
+            "Video resources": "https://www.youtube.com/watch?v=yMSq7QzQcX4", },)
+
+
+def maltego():
+    os.system("clear")
+    github = "Maltego is software used for open-source intelligence and forensics, developed by Paterva from Pretoria, South Africa. Maltego focuses on providing a library of transforms for discovery of data from open sources, and visualizing that information in a graph format, suitable for link analysis and data mining"
+    template.template(
+        "maltego",
+        "maltego",
+        github.strip(),
+        {
+            "Official website": "https://www.maltego.com/ ",
+            "How to use it": "https://www.geeksforgeeks.org/maltego-tool-in-kali-linux/ ",
+            "How to Conduct Person of Interest Investigations Using OSINT and Maltego": "https://www.maltego.com/blog/how-to-conduct-person-of-interest-investigations-using-osint-and-maltego/",
+            "How to Use Maltego: A Beginner’s Guide to OSINT Analysis": "https://www.stationx.net/how-to-use-maltego/",
+            "How to use Maltego": "https://medium.com/hengky-sanjaya-blog/how-to-use-maltego-f57fe77e36e2",
+            "Other resources": "https://www.cybervie.com/blog/what-is-maltego-how-to-use-it-for-information-gathering/", }, )
+
+
+def dracnmap():
+        os.system("clear")
+        github = "Dracnmap is an open source program which is using to exploit the network and gathering information with nmap help. Nmap command comes with lots of options that can make the utility more robust and difficult to follow for new users. Hence Dracnmap is designed to perform fast scaning with the utilizing script engine of nmap and nmap can perform various automatic scanning techniques with the advanced commands."
+        template.template(
+                "Dracnmap",
+                "./dracnmap-v2.2.sh",
+                github.strip(),
+                {
+                    "Github website": "https://github.com/Screetsec/Dracnmap",
+                    "How to use": "https://www.geeksforgeeks.org/dracnmap-information-gathering-and-network-exploitation-tool/ ",
+                    "Other resources": "https://www.hacking.land/2016/10/dracnmap-exploit-network-and-gathering.html?utm_source=dlvr.it&utm_medium=facebook&m=1 ",
+                },
+                method="github",
+                github_install="git clone https://github.com/Screetsec/Dracnmap.git && cd Dracnmap && chmod +x dracnmap-v2.2.sh",
+                github_check="Dracnmap",
+            )
+        
+
+def redhawk():
+        os.system("clear")
+        github = "Red Hawk is a free and open-source tool available on GitHub. Red Hawk is used to scanning websites for information gathering and finding vulnerabilities. Red Hawk is written in PHP. It uses PHP script to do reconnaissance. Red Hawk is so powerful that it can detect content management system while scanning, it can detect IP address, it can detect webserver record, it can detect Cloudflare information, and can detect robots.txt. Red Hawk can detect WordPress, Drupal, Joomla, and Magento CMS. Red Hawk looks for error-based SQL injections, WordPress sensitive files, and WordPress version-related vulnerabilities. RedHawk uses different modules for doing all the scannings."
+        template.template(
+                "RED_HAWK",
+                "php rhawk.php",
+                github.strip(),
+                {
+                    "How to use": "https://systemweakness.com/red-hawk-an-information-gathering-tool-d12a66da7c63 ",
+                    "Other resources": "https://www.geeksforgeeks.org/red-hawk-information-gathering-and-vulnerability-scanning-tool-in-kali-linux/ ",
+                },
+                method="github",
+                github_install="git clone https://github.com/Tuhinshubhra/RED_HAWK.git",
+                github_check="RED_HAWK",
+            )
+
+def th3inspector():
+        os.system("clear")
+        github = "Th3inspector is an open source program which is using to exploit the network and gathering information with nmap help. Nmap command comes with lots of options that can make the utility more robust and difficult to follow for new users. Hence Dracnmap is designed to perform fast scaning with the utilizing script engine of nmap and nmap can perform various automatic scanning techniques with the advanced commands."
+        template.template(
+                "Th3inspector",
+                "perl Th3inspector.pl",
+                github.strip(),
+                {
+                    "github Website": "https://github.com/Moham3dRiahi/Th3inspector ",
+                    "First resource": "https://www.geeksforgeeks.org/th3inspector-osint-tool-for-reconnaissance/ ",
+                    "Second resource": "https://pentesttools.net/th3inspector-tool-for-information-gathering/",
+                },
+                method="github",
+                github_install="git clone https://github.com/Moham3dRiahi/Th3inspector.git",
+                github_check="Th3inspector",
+            )
+
+def hping3():
+        os.system("clear")
+        github = "hping is a command-line oriented TCP/IP packet assembler/analyzer. It supports TCP, UDP, ICMP and RAW-IP protocols, has a traceroute mode, the ability to send files between a covered channel, and many other features."
+        template.template(
+                "hping3",
+                "hping3 -h",
+                github.strip(),
+                {
+                    "First resource": "https://linux.die.net/man/8/hping3",
+                    "Hping Tips and Tricks": "https://iphelix.medium.com/hping-tips-and-tricks-85698751179f",
+                    "Hping3: Full tutorial from noob to pro": "https://techyrick.com/hping3-full-tutorial-for-dummies-to-pro/",
+                },
+            )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Secure_Transmission.py` & `cyberonix-3.0.0/cyberonix/main/tools/Secure_Transmission.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,68 +15,68 @@
             "Check for Digital Certificate Validity",
             "Check credentials only delivered over HTTPS",
             "Check session tokens only delivered over HTTPS",
             "Check if HTTP Strict Transport Security (HSTS) in use",
             "Go back",
         ]
         for i in range(len(list_vulns)):
-            print(colors.options, f"{i}) {list_vulns[i]}".title(), colors.reset)
+            print(colors.options, f"{i+1}) {list_vulns[i]}".title(), colors.reset)
         try:
             vulns = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if vulns == "0":
+            return
+        if vulns == "1":
             os.system("clear")
             # github=github_getting_text("","")
             template.template(
                 "Check SSL Version, Algorithms",
                 "no-tools",
                 "",
                 {
                     "10 Online Tools to Test SSL, TLS and Latest Vulnerability": "https://geekflare.com/ssl-test-certificate/",
                     "Testing for Weak SSL TLS Ciphers": "https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/09-Testing_for_Weak_Cryptography/01-Testing_for_Weak_SSL_TLS_Ciphers_Insufficient_Transport_Layer_Protection",
                     "How to Verify the SSL Key Length": "https://www.rapidsslonline.com/ssl/how-to-verify-the-ssl-key-length",
                 },
             )
             # writeup.writeup({"10 Online Tools to Test SSL, TLS and Latest Vulnerability":"https://geekflare.com/ssl-test-certificate/","Testing for Weak SSL TLS Ciphers":"https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/09-Testing_for_Weak_Cryptography/01-Testing_for_Weak_SSL_TLS_Ciphers_Insufficient_Transport_Layer_Protection","How to Verify the SSL Key Length":"https://www.rapidsslonline.com/ssl/how-to-verify-the-ssl-key-length/"},"Check SSL Version, Algorithms, Key length")
-        elif vulns == "1":
+        elif vulns == "2":
             os.system("clear")
             # github
             template.template(
                 "Check for Digital Certificate Validity",
                 "no-tools",
                 "",
                 {
                     "A closer look at Digital Certificates": "https://medium.com/@mehulgala77/a-closer-look-at-digital-certificates-9ce5a4c56f75"
                 },
             )
-        elif vulns == "2":
+        elif vulns == "3":
             os.system("clear")
             template.template(
                 "Check credentials only delivered over HTTPS",
                 "no-tools",
                 "",
                 {
                     "Testing for Credentials Transported over an Encrypted Channel": "https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/04-Authentication_Testing/01-Testing_for_Credentials_Transported_over_an_Encrypted_Channel",
                     "Penetration testing of Credential Data over Encrypted Channel": "https://www.hackingloops.com/penetration-testing-of-credential-data-over-encrypted-channel/",
                 },
             )
-        elif vulns == "3":
+        elif vulns == "4":
             os.system("clear")
             template.template(
                 "Check session tokens only delivered over HTTPS",
                 "no-tools",
                 "",
                 {
                     "Testing for Exposed Session Variables": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/06-Session_Management_Testing/04-Testing_for_Exposed_Session_Variables",
                     "Using Burp to Test Session Token Handling": "https://portswigger.net/support/using-burp-to-test-session-token-handling",
                 },
             )
 
-        elif vulns == "4":
+        elif vulns == "5":
             os.system("clear")
             template.template(
                 "Check if HTTP Strict Transport Security (HSTS) in use",
                 "no-tools",
                 "",
                 {
                     "HSTS (HTTP Strict Transport Security) Test": "https://geekflare.com/tools/hsts-test",
@@ -90,15 +90,15 @@
 def vuln_options():
     print(f"{colors.options}1) Tools")
     print(f"2) Write-ups")
     print(f"3) Go Back..")
     try:
         ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
     except KeyboardInterrupt:
-        template.exit_program()
+        return
     return ask
 
 
 def github_getting_text(link, selector, indexvalue):
     print(f"Please Wait....\r", end="")
     URL = link
     try:
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Sniffing_and_Spoofing.py` & `cyberonix-3.0.0/cyberonix/main/tools/Sniffing_and_Spoofing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,159 @@
-from cyberonix.main.tools import banner,colors,template
+from cyberonix.main.tools import banner, colors, template,Vulnerability_Analysis
 import os
 import requests
 from bs4 import BeautifulSoup
 
-#main function
+# main function
+
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Sniffing & Spoofing")
-        list_attacks=[" Wireshark"," Bettercap"," Tcpdump"," Arpspoof"," Dsniff"," Scapy"," Netsniff-ng"," Macchanger"," Responder"," Airgeddon","Sharesniffer","Wifi-Pumpkin-3","Go Back"]
+        list_attacks = [" Wireshark\t\t(Recommended)", " Bettercap\t\t(Recommended)", " Tcpdump", " Dsniff", " Scapy", " Netsniff-ng", " Macchanger",
+                        " Responder", " Airgeddon",  "Wifi-Pumpkin-3\t(Recommended)", "mitmproxy\t\t(Recommended) ", "zaproxy ", "Go Back"]
         for i in range(len(list_attacks)):
-                print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option=="0":
+            return
+        if option == "0":
             print("\n[+] Wireshark")
-            os.system("clear")
-            # name,command,discription,writeup,link=True,method="kali",github_install="",github_check=True
-            github = "Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. It can be used to examine data from a live network or from a previously saved capture file. Wireshark provides a graphical user interface (GUI) for capturing and analyzing network traffic."
-            template.template("wireshark","wireshark",github.strip(),{"Wireshark Cheat-Sheet":"https://www.comparitech.com/net-admin/wireshark-cheat-sheet","What-is-Wireshark-and-How-to-Use-it":"https://www.comptia.org/content/articles/what-is-wireshark-and-how-to-use-it ","Video Resource Wireshark":"https://www.youtube.com/playlist?list=PLBf0hzazHTGPgyxeEj_9LBHiqjtNEjsgt"})        
-        elif option=="1":
+            Vulnerability_Analysis.wireshark()
+        elif option == "2":
             print("\n[+] Bettercap")
-            os.system("clear")
-            github=github_getting_text("https://github.com/bettercap/bettercap",'p[dir="auto"]',3)
-            template.template("bettercap","bettercap",github.strip(),{"Man in the Middle": "https://www.cybervie.com/blog/easy-and-better-man-in-the-middle-using-bettercap/", "MITM Labs Write-up": "https://charlesreid1.com/wiki/MITM_Labs/Bettercap_Over_Wifi", "NTLM Capturing": "https://blog.xpnsec.com/bettercap-capturing-ntlm/", "DNS Spoofing": "https://psychovik.medium.com/dns-spoofing-using-bettercap-24a8435f7a03"})
-        elif option=="2":
+            bettercap()
+        elif option == "3":
             print("\n[+] Tcpdump")
-            os.system("clear")
-            github = github_getting_text("https://opensource.com/article/18/10/introduction-tcpdump",'p',5)
-            template.template("tcpdump","tcpdump -h",github.strip()+'\r\n - '.join(github.strip().split('\n')),{"TCPDump": "https://www.qnx.com/developers/docs/7.0.0/index.html#com.qnx.doc.neutrino.utilities/topic/t/tcpdump.html","Deep Packet Analysis": "https://thwack.solarwinds.com/resources/b/geek-speak/posts/deep-packet-analysis---practical-applications-with-tcpdump","TCPDump F5": "https://support.f5.com/csp/article/K2289","TCPDump FreeBSD": "https://www.freebsd.org/cgi/man.cgi?tcpdump(1)"})
-        elif option=="3":
-            print("\n[+] Arpspoof")
-            os.system("clear")
-            github = "arpspoof is a utility for network auditing and penetration testing. It is part of the dsniff suite of tools, which is used to perform various types of network attacks and security auditing. It can be used to intercept and modify traffic on a local area network. It works by sending out specially crafted ARP (Address Resolution Protocol) packets, which can be used to redirect traffic from one host to another. This is known as ARP spoofing or ARP cache poisoning."
-            template.template("dsniff","arpspoof",github.strip(),{"Arp_Spoofing_Using_Man_In_The_Middle_Attack":"https://linuxhint.com/arp_spoofing_using_man_in_the_middle_attack/","ArpSpoof Video Resource":"https://www.youtube.com/watch?v=8SIP36Fym7U"})
-        elif option=="4":
+            tcpdump()    
+        elif option == "4":
             print("\n[+] Dsniff")
-            os.system("clear")
-            github = "dsniff is a collection of tools for network auditing and penetration testing. dsniff, filesnarf, mailsnarf, msgsnarf, urlsnarf, and webspy passively monitor a network for interesting data (passwords, e-mail, files, etc.). arpspoof, dnsspoof, and macof facilitate the interception of network traffic normally unavailable to an attacker (e.g, due to layer-2 switching). sshmitm and webmitm implement active monkey-in-the-middle attacks against redirected SSH and HTTPS sessions by exploiting weak bindings in ad-hoc PKI."
-            template.template("dsniff","dsniff -h",github.strip(),{"Dsniff Repo": "https://github.com/tecknicaltom/dsniff","Manpages Dsniff": "https://kaisenlinux.org/manpages/dsniff.html","Introduction": "http://www.ouah.org/dsniffintr.htm"})
-        elif option=="5":
+            dsniff()        
+        elif option == "5":
             print("\n[+] Scapy")
-            os.system("clear")
-            github=github_getting_text("https://scapy.net/",'p',0)
-            template.template("scapy","chmod +x run_scapy && ./run_scapy",github.strip(),{"what is Scapy": "https://santandergto.com/en/guide-using-scapy-with-python/#whatisScapy","Scapy Introduction": "https://scapy.readthedocs.io/en/latest/introduction.html","Scapy Usage": "https://python.astrotech.io/network/transport/scapy.html","Scapy Tutorial": "https://youtu.be/LvaII2PEwcQ"},method="github",github_install="git clone https://github.com/secdev/scapy.git",github_check="scapy")
-        elif option=="6":
+            scapy()
+        elif option == "6":
             print("\n[+] Netsniff-ng")
-            os.system("clear")
-            github_text_0=github_getting_text("http://netsniff-ng.org/",'p',0)
-            github_text_1=github_getting_text("http://netsniff-ng.org/",'p',1)
-            github_text_2=github_getting_text("http://netsniff-ng.org/",'p',2)
-            github = github_text_0 + github_text_1 + github_text_2
-            template.template("netsniff-ng","netsniff-ng -h",github.strip(),{"Netsniff-ng Website": "http://netsniff-ng.org/", "Sniffing Network Traffic": "https://medium.com/purple-team/sniffing-network-traffic-with-netsniff-ng-55b8f5d436c2", "Manual": "https://linux.die.net/man/8/netsniff-ng", "Video Resources": "https://www.irongeek.com/i.php?page=videos/hack3rcon4/09-netsniff-ng-jon-schipp"})
-        elif option=="7":
+            netsniff_ng()    
+        elif option == "7":
             print("\n[+] Macchanger")
-            os.system("clear")
-            github=github_getting_text("https://www.kali.org/tools/macchanger/",'p',0)
-            template.template("macchanger","macchanger --help",github.strip(),{"How to Change Mac Address": "https://linuxconfig.org/how-to-change-mac-address-using-macchanger-on-kali-linux/", "Macchanger on Kali Linux": "https://kennyvn.com/change-mac-address-macchanger-kali-linux/", "Permanently Change Mac Address": "https://www.linuxuprising.com/2018/05/how-to-permanently-change-mac-address.html"})
-        elif option=="8":
+            macchanger()        
+        elif option == "8":
             print("\n[+] Responder")
-            os.system("clear")
-            github_text_0=github_getting_text("https://www.kali.org/tools/responder/",'p',1)
-            github_text_1=github_getting_text("https://www.kali.org/tools/responder/",'p',2)
-            github = github_text_0 + github_text_1
-            template.template("responder","responder -h",github,{"Responder-Guide": "https://www.ivoidwarranties.tech/posts/pentesting-tuts/responder/guide/","How-To-Use-Responder-to-Capture-NETNTLM-and-Grab-a-Shell": "https://www.a2secure.com/blog-en/how-to-use-responder-to-capture-netntlm-and-grab-a-shell/","infinitelogins.com-Responder": "https://infinitelogins.com/tag/responder/","Capture-Window-10-NTLM-Hashes-Responder": "https://secnhack.in/capture-window-10-ntlm-hashes-responder"})
-        elif option=="9":
+            responder()    
+        elif option == "9":
             print("\n[+] Airgeddon")
-            os.system("clear")
-            github = "Airgeddon is a wireless security auditing tool that is used to assess the security of wireless networks. It can be used to perform various types of attacks, such as cracking WPA/WPA2 passwords, capturing WPA/WPA2 handshakes, and identifying vulnerable wireless access points. The tool is open-source and runs on Linux systems. Airgeddon is not intended for illegal use, and should only be used on networks that you have permission to test."
-            template.template("airgeddon","airgeddon",github.strip(),{"How to Use Airgeddon in Kali Linux":"https://www.systranbox.com/how-to-use-airgeddon-in-kali-linux/", "Airgeddon Wifi Crack in Kali Linux":"https://www.kalilinux.in/2021/03/airgeddon-wifi-crack-kalilinux.html", "Airgeddon Multi-Use Bash Script to Audit Wireless Networks":"https://xploitlab.com/airgeddon-multi-use-bash-script-to-audit-wireless-networks/", "Airgeddon Tool Installation and Fix All Errors":"https://www.hacknos.com/airgeddon-tool-installation-and-fix-all-errors/"})
-        elif option=="10":
-            print("\n[+] Sharesniffer")
-            os.system("clear")
-            github=github_getting_text("https://github.com/shirosaidev/sharesniffer",'p[dir="auto"]',2)
-            template.template("sharesniffer","pip install python-nmap netifaces >/dev/null 2>&1 && chmod +x sharesniffer.py && ./sharesniffer.py -h",github.strip(),{"Sharesniffer Github-Repo":"github.com/shirosaidev/sharesniffer","Sharesniffer Presentation":"slideplayer.com/slide/6055181/"},method="github",github_install="git clone https://github.com/shirosaidev/sharesniffer",github_check="sharesniffer")    
-        elif option=="11":
+            airgeddon()               
+        elif option == "10":
             print("\n[+] Wifi-Pumpkin-3")
-            os.system("clear")
-            github=github_getting_text("https://github.com/P0cL4bs/wifipumpkin3",'p[dir="auto"]',4)
-            template.template("wifipumpkin3","wifipumpkin3",github.strip(),{"Wireless Penetration Testing": "https://www.hackingarticles.in/wireless-penetration-testing-wifipumpkin3/", "WiFiPumpkin3 : Powerful Framework For Rogue Access Point Attack": "https://kalilinuxtutorials.com/wifipumpkin3/"})    
+            wifipumpkin3()        
+        elif option == "11":
+            print("\n[+] mitmproxy")
+            mitmproxy()        
+        elif option == "12":
+            print("\n[+] zaproxy")
+            zaproxy()        
         else:
             return
-def github_getting_text(link,selector,indexvalue):
-    print("Please Wait....\r",end="")
+
+
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
     URL = link
     try:
         r = requests.get(URL)
         soup = BeautifulSoup(r.content, 'html.parser')
         paras = soup.select(selector)
-        #check index value from test file
+        # check index value from test file
         return paras[indexvalue].text
     except:
         return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
 
-if __name__=='__main__':
+def tcpdump():
+    os.system("clear")
+    github = github_getting_text(
+                "https://opensource.com/article/18/10/introduction-tcpdump", 'p', 5)
+    template.template("tcpdump", "tcpdump -h", github.strip()+'\r\n - '.join(github.strip().split('\n')), {"TCPDump": "https://www.qnx.com/developers/docs/7.0.0/index.html#com.qnx.doc.neutrino.utilities/topic/t/tcpdump.html", "Deep Packet Analysis":
+                              "https://thwack.solarwinds.com/resources/b/geek-speak/posts/deep-packet-analysis---practical-applications-with-tcpdump", "TCPDump F5": "https://support.f5.com/csp/article/K2289", "TCPDump FreeBSD": "https://www.freebsd.org/cgi/man.cgi?tcpdump"})
+       
+       
+def dsniff():
+    os.system("clear")
+    github = "dsniff is a collection of tools for network auditing and penetration testing. dsniff, filesnarf, mailsnarf, msgsnarf, urlsnarf, and webspy passively monitor a network for interesting data (passwords, e-mail, files, etc.). arpspoof, dnsspoof, and macof facilitate the interception of network traffic normally unavailable to an attacker (e.g, due to layer-2 switching). sshmitm and webmitm implement active monkey-in-the-middle attacks against redirected SSH and HTTPS sessions by exploiting weak bindings in ad-hoc PKI."
+    template.template("dsniff", "dsniff -h", github.strip(), {"Dsniff Repo": "https://github.com/tecknicaltom/dsniff",
+                              "Manpages Dsniff": "https://www.unix.com/man-page/debian/8/dsniff/", "Introduction": "http://www.ouah.org/dsniffintr.htm"})
+        
+def scapy():
+    os.system("clear")
+    github = "Scapy is a Python program that enables the user to send, sniff and dissect and forge network packets. This capability allows construction of tools that can probe, scan or attack networks."
+    template.template("scapy", "chmod +x run_scapy && ./run_scapy", github.strip(), {"what is Scapy": "https://www.freecodecamp.org/news/how-to-use-scapy-python-networking/", "Scapy Introduction": "https://scapy.readthedocs.io/en/latest/introduction.html", "Scapy Usage": "https://python.astrotech.io/network/transport/scapy.html", "Scapy Tutorial": "https://youtu.be/LvaII2PEwcQ",
+                              "https://datascientest.com/en/scapy-everything-you-need-to-know-about-the-python-based-network-packaging-tool": "https://datascientest.com/en/scapy-everything-you-need-to-know-about-the-python-based-network-packaging-tool"}, method="github", github_install="git clone https://github.com/secdev/scapy.git", github_check="scapy")
+        
+def netsniff_ng():
+    os.system("clear")
+    github_text_0 = github_getting_text(
+                "http://netsniff-ng.org/", 'p', 0)
+    github_text_1 = github_getting_text(
+                "http://netsniff-ng.org/", 'p', 1)
+    github_text_2 = github_getting_text(
+                "http://netsniff-ng.org/", 'p', 2)
+    github = github_text_0 + github_text_1 + github_text_2
+    template.template("netsniff-ng", "netsniff-ng -h", github.strip(), {"Netsniff-ng Website": "http://netsniff-ng.org/", "Sniffing Network Traffic": "https://medium.com/purple-team/sniffing-network-traffic-with-netsniff-ng-55b8f5d436c2",
+                              "Manual": "https://linux.die.net/man/8/netsniff-ng", "Video Resources": "https://www.irongeek.com/i.php?page=videos/hack3rcon4/09-netsniff-ng-jon-schipp"})
+        
+def macchanger():
+    os.system("clear")
+    github_fetch = github_getting_text(
+                "https://www.kali.org/tools/macchanger/", 'p', 0)
+    github = github_fetch.strip().replace("\n", "").replace("\t", "")
+    template.template("macchanger", "macchanger --help", github.strip(), {"How to Change Mac Address": "https://linuxconfig.org/how-to-change-mac-address-using-macchanger-on-kali-linux/",
+                              "Macchanger on Kali Linux": "https://kennyvn.com/change-mac-address-macchanger-kali-linux/", "Permanently Change Mac Address": "https://www.linuxuprising.com/2018/05/how-to-permanently-change-mac-address.html"})
+        
+def responder():
+    os.system("clear")
+    github_text_0 = github_getting_text(
+                "https://www.kali.org/tools/responder/", 'p', 1)
+    github_text_1 = github_getting_text(
+                "https://www.kali.org/tools/responder/", 'p', 2)
+    github = github_text_0.strip().replace("\n", "").replace("\t", "") + github_text_1.strip().replace("\n", "").replace("\t", "")
+    template.template("responder", "responder -h", github, {"Responder-Guide": "https://www.ivoidwarranties.tech/posts/pentesting-tuts/responder/guide/", "How-To-Use-Responder-to-Capture-NETNTLM-and-Grab-a-Shell":
+                              "https://www.a2secure.com/blog-en/how-to-use-responder-to-capture-netntlm-and-grab-a-shell/", "infinitelogins.com-Responder": "https://infinitelogins.com/tag/responder/", "Capture-Window-10-NTLM-Hashes-Responder": "https://secnhack.in/capture-window-10-ntlm-hashes-responder"})
+        
+def airgeddon():
+    os.system("clear")
+    github = "Airgeddon is a wireless security auditing tool that is used to assess the security of wireless networks. It can be used to perform various types of attacks, such as cracking WPA/WPA2 passwords, capturing WPA/WPA2 handshakes, and identifying vulnerable wireless access points. The tool is open-source and runs on Linux systems. Airgeddon is not intended for illegal use, and should only be used on networks that you have permission to test."
+    template.template("airgeddon", "airgeddon", github.strip(), {"How to Use Airgeddon in Kali Linux": "https://www.systranbox.com/how-to-use-airgeddon-in-kali-linux/", "Airgeddon Wifi Crack in Kali Linux": "https://www.kalilinux.in/2021/03/airgeddon-wifi-crack-kalilinux.html",
+                              "Airgeddon Multi-Use Bash Script to Audit Wireless Networks": "https://xploitlab.com/airgeddon-multi-use-bash-script-to-audit-wireless-networks/", "Airgeddon Tool Installation and Fix All Errors": "https://www.hacknos.com/airgeddon-tool-installation-and-fix-all-errors/"})
+        
+def wifipumpkin3():
+    os.system("clear")
+    github = github_getting_text(
+                "https://wifipumpkin3.github.io/", 'p', 1)
+    template.template("wifipumpkin3", "wifipumpkin3", github.strip(), {
+                              "Wireless Penetration Testing": "https://www.hackingarticles.in/wireless-penetration-testing-wifipumpkin3/", "WiFiPumpkin3 : Powerful Framework For Rogue Access Point Attack": "https://kalilinuxtutorials.com/wifipumpkin3/"})
+        
+def mitmproxy():
+    os.system("clear")
+    github = "mitmproxy is an interactive, SSL/TLS-capable intercepting proxy with a console interface for HTTP/1, HTTP/2, and WebSockets.mitmdump is the command-line version of mitmproxy. Think tcpdump for HTTP.mitmweb is a web-based interface for mitmproxy."
+    template.template("mitmproxy", "mitmproxy", github.strip(), {
+                              "An Introduction to mitmproxy": "https://medium.com/ciandt-techblog/an-introduction-to-mitmproxy-f3654e6bd53b", "mitmproxy docs": "https://docs.mitmproxy.org/stable/", })
+        
+def zaproxy():
+    os.system("clear")
+    github = github_getting_text(
+                "https://github.com/zaproxy/zaproxy", 'p[dir=auto]', 2)
+    template.template("zaproxy", "zaproxy", github.strip(), {
+                              "Overview ZAP": "https://www.zaproxy.org/getting-started/", })
+        
+def bettercap():
+    os.system("clear")
+    github = github_getting_text(
+                "https://www.bettercap.org/intro/", 'p', 0)
+    template.template("bettercap", "bettercap", github.strip(), {"Man in the Middle": "https://www.cybervie.com/blog/easy-and-better-man-in-the-middle-using-bettercap/", "MITM Labs Write-up":
+                              "https://charlesreid1.com/wiki/MITM_Labs/Bettercap_Over_Wifi", "NTLM Capturing": "https://blog.xpnsec.com/bettercap-capturing-ntlm/", "DNS Spoofing": "https://psychovik.medium.com/dns-spoofing-using-bettercap-24a8435f7a03"})
+        
+
+if __name__ == '__main__':
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Vulnerability_Analysis.py` & `cyberonix-3.0.0/cyberonix/main/tools/Vulnerability_Analysis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,108 @@
 #!/usr/bin/python3
 import os
 import requests
-from cyberonix.main.tools import banner,colors,template
+from cyberonix.main.tools import banner, colors, template, information_gathering, WEB_Application_Analysis
 from bs4 import BeautifulSoup
 
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Vulnerability Analysis")
-        list_attacks=["Wpscan","Wireshark","Wapiti","Nmap","Legion","Nikto","go back"]
+        list_attacks = ["Wpscan\t\t(Recommended)", "Wireshark\t\t(Recommended)",
+                        "Wapiti", "Nmap\t\t(Recommended)", "Legion", "Nikto", "Wfuzz", "go back"]
         for i in range(len(list_attacks)):
-                print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option=="0":
+            return
+        if option == "1":
             print("\n[+] Wpscan")
-            os.system("clear")
-            github = "WPScan is a security scanner designed for testing the security of websites built using WordPress. WPScan was developed using the Ruby programming language and then released in the first version in 2019. The WPScan security scanner is primarily intended to be used by WordPress administrators and security teams to assess the security status of their WordPress installations. It is used to scan WordPress websites for known vulnerabilities both in WordPress and commonly used WordPress plugins and themes. The code base for WPScan is licensed under GPLv3"
-            template.template("wpscan","wpscan -h",github.strip(),{'WPScan Intro: How to Scan for WordPress Vulnerabilities':'https://blog.sucuri.net/2021/05/wpscan-how-to-scan-for-wordpress-vulnerabilities.html/','WPScan:WordPress Pentesting Framework':'https://www.hackingarticles.in/wpscanwordpress-pentesting-framework/','How To Use WPScan to Test for Vulnerable Plugins and Themes in Wordpress':"https://www.digitalocean.com/community/tutorials/how-to-use-wpscan-to-test-for-vulnerable-plugins-and-themes-in-wordpress","How to Use wpscan tool in Kali Linux":"https://www.geeksforgeeks.org/how-to-use-wpscan-tool-in-kali-linux/","WPScan Usage Example [Enumeration + Exploit]":"https://www.cyberpunk.rs/wpscan-usage-example"})
-        elif option=="1":
+            wpscan()
+        elif option == "2":
             print("\n[+] Wireshark")
-            os.system("clear")
-            github=github_getting_text("https://github.com/wireshark/wireshark",'p[dir="auto"]',0)
-            template.template("wireshark","wireshark",github.strip(),{'How To Install & Use Wireshark On Kali Linux':'https://infosecscout.com/wireshark-on-kali-linux/','Wireshark Tool Documentation':'https://www.kali.org/tools/wireshark/','Wireshark Training':'https://www.wireshark.org/docs/','Wireshark – Resources':'https://blog.inf.ed.ac.uk/atate/2023/01/14/wireshark-resources/','Kerberos Wireshark Captures: A Windows Login Example':'https://medium.com/@robert.broeckelmann/kerberos-wireshark-captures-a-windows-login-example-151fabf3375a','Wireshark – Packet Capturing and Analyzing':'https://www.geeksforgeeks.org/wireshark-packet-capturing-and-analyzing/','https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/':'https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/'})
-        elif option=="2":
+            wireshark()
+        elif option == "3":
             print("\n[+] Wapiti")
-            os.system("clear")
-            github=github_getting_text("https://github.com/wapiti-scanner/wapiti",'p[dir="auto"]',6)
-            template.template("wapiti","wapiti",github.strip(),{"wapiti free web application vulnerability scanner":"https://pentestit.medium.com/wapiti-free-web-application-vulnerability-scanner-ce7712adf644","Official docs":"https://github.com/wapiti-scanner/wapiti","wapiti tutorial":"https://www.kalilinux.in/2021/01/wapiti-tutorial.html","complete guide to using wapiti web vulnerability scanner to keep your web applications websites secure":"https://linuxsecurity.com/features/complete-guide-to-using-wapiti-web-vulnerability-scanner-to-keep-your-web-applications-websites-secure"})
-        elif option=="3":
+            WEB_Application_Analysis.wapiti()
+        elif option == "4":
             print("\n[+] Nmap")
-            os.system("clear")
-            github = "Nmap (Network Mapper) is a network scanner created by Gordon Lyon (also known by his pseudonym Fyodor Vaskovich). Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses."
-            template.template("nmap","nmap -h",github.strip(),{"Nmap Cheat-Sheet":"https://www.stationx.net/nmap-cheat-sheet/","Official website":"https://nmap.org/ ","Other resources":"https://linux.die.net/man/1/nmap"})            
-        elif option=="4":
-            print("\n[+] Legion")
-            os.system("clear")
-            github=github_getting_text("https://github.com/GoVanguard/legion",'p[class="f4 my-3"]',0)
-            template.template("legion","legion",github.strip(),{'Legion Tool in Kali Linux':'https://www.geeksforgeeks.org/legion-tool-in-kali-linux','Legion -- Test Web Application Vulnerability Automatically':'https://www.kalilinux.in/2020/09/legion-kali-linux.html','How to use Legion application in Kali Linux | Information Gathering':'https://www.youtube.com/watch?v=5UAfXbP5Y0k'})
-        elif option=="5":
+            information_gathering.nmap()
+        elif option == "5":
+            print("\n[+] legion")
+            legion()
+        elif option == "6":
             print("\n[+] Nikto")
-            os.system("clear")
-            github=github_getting_text("https://en.wikipedia.org/wiki/Nikto_(vulnerability_scanner)",'p',1)
-            template.template("nikto","nikto -h",github.strip(),{'What is Nikto and it’s usages ?':'https://www.geeksforgeeks.org/what-is-nikto-and-its-usages/','Nikto: A Practical Website Vulnerability Scanner':'https://securitytrails.com/blog/nikto-website-vulnerability-scanner','Nikto Official Docs':'https://github.com/sullo/nikto/wiki'})
+            nikto()
+        elif option == "7":
+            print("\n[+] Wfuzz")
+            wfuzz()
         else:
             return
 
-def github_getting_text(link,selector,indexvalue):
-    print("Please Wait....\r",end="")
+
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
     URL = link
     try:
         r = requests.get(URL)
         soup = BeautifulSoup(r.content, 'html.parser')
         paras = soup.select(selector)
-        #check index value from test file
+        # check index value from test file
         return paras[indexvalue].text
     except:
         return f"{colors.red}NotLloaded Because No Internet Connection{colors.reset}"
 
+
 def tool_writeups():
     print(f"{colors.options}1) TOOL(About,Installation)")
     print(f"2) Write Ups")
     print(f"3) Go Back..")
     try:
-        ask=input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+        ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
     except KeyboardInterrupt:
-        template.exit_program()
+        return
     return ask
 
-if __name__=='__main__':
+def wfuzz():
+    os.system("clear")
+    github = "Wfuzz is a web application brute force tool used to identify web application vulnerabilities by scanning web content, such as directories and files, for hidden or non-linked content. Wfuzz can be used to test input validation, error handling, and access control mechanisms. It is a command-line tool and allows users to customize requests to send payloads, which makes it very flexible and powerful for web application penetration testing. Wfuzz is written in Python and can be used on Linux, Windows, and macOS. It is open-source and free to use."
+    template.template(
+                "wfuzz", "wfuzz --help", github.strip(), {"How to use Wfuzz to find web application vulnerabilities":
+                                                          "https://www.techtarget.com/searchsecurity/feature/How-to-use-Wfuzz-to-find-web-application-vulnerabilities", }
+            )
+
+
+def wireshark():
+    os.system("clear")
+    github = "Wireshark is a network traffic analyzer, or sniffer, for Linux, macOS, BSD and other Unix and Unixlike operating systems and for Windows. It uses Qt, a graphical user interface library, and libpcap and npcap as packet capture and filtering libraries."
+    template.template("wireshark", "wireshark", github.strip(), {'How To Install & Use Wireshark On Kali Linux': 'https://infosecscout.com/wireshark-on-kali-linux/', 'Wireshark Tool Documentation': 'https://www.kali.org/tools/wireshark/', 'Wireshark Training': 'https://www.wireshark.org/docs/', 'Wireshark – Resources': 'https://blog.inf.ed.ac.uk/atate/2023/01/14/wireshark-resources/',
+                              'Kerberos Wireshark Captures: A Windows Login Example': 'https://medium.com/@robert.broeckelmann/kerberos-wireshark-captures-a-windows-login-example-151fabf3375a', 'Wireshark – Packet Capturing and Analyzing': 'https://www.geeksforgeeks.org/wireshark-packet-capturing-and-analyzing/', 'Wireshark Tutorial: Decrypting HTTPS Traffic': 'https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/'})
+def legion():
+    os.system("clear")
+    github = github_getting_text(
+        "https://github.com/GoVanguard/legion", 'p[class="f4 my-3"]', 0)
+    template.template("legion", "legion", github.strip(), {"Legion: The best all in one network mapping tool": "https://techyrick.com/legion-kali-linux/", "An Overview Of Network Penetration Testing Using Legion Framework": "https://www.c-sharpcorner.com/article/an-overview-of-network-penetration-testing-using-legion-framework/#:~:text=What%20is%20Legion%3F,the%20attacks%20against%20targeted%20devices.",
+                      'Legion Tool in Kali Linux': 'https://www.geeksforgeeks.org/legion-tool-in-kali-linux', 'Legion -- Test Web Application Vulnerability Automatically': 'https://www.kalilinux.in/2020/09/legion-kali-linux.html', 'How to use Legion application in Kali Linux Video Tutorial': 'https://www.youtube.com/watch?v=0v2_UFhq6zQ'})
+
+
+def nikto():
+    os.system("clear")
+    github = github_getting_text(
+        "https://en.wikipedia.org/wiki/Nikto_(vulnerability_scanner)", 'p', 1)
+    template.template("nikto", "nikto -h", github.strip(), {'What is Nikto and it’s usages ?': 'https://www.geeksforgeeks.org/what-is-nikto-and-its-usages/',
+                      'Nikto: A Practical Website Vulnerability Scanner': 'https://securitytrails.com/blog/nikto-website-vulnerability-scanner', 'Nikto Official Docs': 'https://github.com/sullo/nikto/wiki'})
+
+
+def wpscan():
+    os.system("clear")
+    github = "WPScan is a security scanner designed for testing the security of websites built using WordPress. WPScan was developed using the Ruby programming language and then released in the first version in 2019. The WPScan security scanner is primarily intended to be used by WordPress administrators and security teams to assess the security status of their WordPress installations. It is used to scan WordPress websites for known vulnerabilities both in WordPress and commonly used WordPress plugins and themes. The code base for WPScan is licensed under GPLv3"
+    template.template("wpscan", "wpscan -h", github.strip(), {'WPScan Intro: How to Scan for WordPress Vulnerabilities': 'https://blog.sucuri.net/2021/05/wpscan-how-to-scan-for-wordpress-vulnerabilities.html/', 'WPScan:WordPress Pentesting Framework': 'https://www.hackingarticles.in/wpscanwordpress-pentesting-framework/', 'How To Use WPScan to Test for Vulnerable Plugins and Themes in Wordpress':
+                      "https://www.digitalocean.com/community/tutorials/how-to-use-wpscan-to-test-for-vulnerable-plugins-and-themes-in-wordpress", "How to Use wpscan tool in Kali Linux": "https://www.geeksforgeeks.org/how-to-use-wpscan-tool-in-kali-linux/", "WPScan Usage Example [Enumeration + Exploit]": "https://www.cyberpunk.rs/wpscan-usage-example"})
+
+
+if __name__ == '__main__':
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/WEB_Application_Analysis.py` & `cyberonix-3.0.0/cyberonix/main/tools/WEB_Application_Analysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,188 @@
-from cyberonix.main.tools import banner,colors,template,waiting,writeup
-import os,requests
+from cyberonix.main.tools import banner, colors, template, waiting, writeup, Configuration_Management
+import os
+import requests
 import requests
 from bs4 import BeautifulSoup
 
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("WEB Application Analysis")
-        list_attacks=["Burp Suite","Owasp ZAP","Nikto","Wapiti","Nessus","dirb","skipfish","Nuclei","go back"]
+        list_attacks = [" Burp Suite\t\t(Recommended)", " Dirsearch", " Owasp ZAP", " Dirbuster\t\t(Recommended)",
+                        " Nikto", " Wapiti", " Nessus\t\t(Recommended)", " dirb", " Nuclei", "ffuf", "go back"]
         for i in range(len(list_attacks)):
-            print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option=="0":
+            return
+        if option == "1":
             print(f"\n[+] Burp Suite")
-            os.system("clear")
             burp_suite()
-            # github = "Burp Suite is an integrated platform for performing security testing of web applications. Its various tools work seamlessly together to support the entire testing process, from initialmapping and analysis of an application's attack surface, through to finding and exploiting security vulnerabilities. Burp gives you full control, letting you combine advanced manual techniques with state-of-the-art automation, to make your work faster, more effective, and more fun."
-            # template.template("Burp-Suite","burp",github.strip(),{"Top 10 tips for burpsuite":"https://medium.com/r3d-buck3t/top-10-tips-for-burp-suite-72212d22328f","Setting up burbsuite":"https://thexssrat.medium.com/setting-up-burp-suite-b0a6767d3408","Burp Suite: Do I need the professional edition?":"https://thexssrat.medium.com/burp-suite-do-i-need-the-professional-edition-bf8c87ce236e","Burp Suite Extensions to help you Pentest":"https://medium.com/codex/burp-suite-extensions-to-help-you-pentest-97f22a7d7d4d","FIND MORE resources here":"https://medium.com/search?q=burpsuite"},link="https://github.com/hardikhacker/Burp-Suite",method="github")
-        elif option=="1":
+        elif option == "2":
+            print(f"\n[+] Dirsearch")
+            dirsearch()
+        elif option == "3":
             print(f"\n[+] Owasp ZAP")
-            os.system("clear")
-            github = "The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.\nIt is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox. https://www.owasp.org/index.php/ZAP"
-            template.template('zaproxy','zaproxy',github.strip(),{"How to setup OWASP ZAP to scan your web application for security vulnerabilities":"https://www.linkedin.com/pulse/how-setup-owasp-zap-scan-your-web-application-security-botla/","Authenticated Scan using OWASP-ZAP":"https://medium.com/@secureica/authenticated-scan-using-owasp-zap-f0a71dafe41","OWASP ZAP: 6 Key Capabilities and a Quick Tutorial":"https://www.hackerone.com/knowledge-center/owasp-zap-6-key-capabilities-and-quick-tutorial","Initial Setup":"https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/untitled","Setup OWASP ZAP":"https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/setup-owasp-zap"})
-        elif option=="2":
+            owasp_zap()
+        elif option == "4":
+            Configuration_Management.dirbuster()
+        elif option == "5":
             print("\n[+] Nikto")
-            os.system("clear")
-            github=github_getting_text("https://en.wikipedia.org/wiki/Nikto_(vulnerability_scanner)",'p',1)
-            template.template("nikto","nikto -h",github.strip(),{'What is Nikto and it’s usages ?':'https://www.geeksforgeeks.org/what-is-nikto-and-its-usages/','Nikto: A Practical Website Vulnerability Scanner':'https://securitytrails.com/blog/nikto-website-vulnerability-scanner','Nikto Official Docs':'https://github.com/sullo/nikto/wiki'})
-        elif option=="3":
+            nikto()
+        elif option == "6":
             print("\n[+] Wapiti")
-            os.system("clear")
-            github=github_getting_text("https://github.com/wapiti-scanner/wapiti",'p[dir="auto"]',6)
-            template.template("wapiti","wapiti",github.strip(),{"wapiti free web application vulnerability scanner":"https://pentestit.medium.com/wapiti-free-web-application-vulnerability-scanner-ce7712adf644","Official docs":"https://github.com/wapiti-scanner/wapiti","wapiti tutorial":"https://www.kalilinux.in/2021/01/wapiti-tutorial.html","complete guide to using wapiti web vulnerability scanner to keep your web applications websites secure":"https://linuxsecurity.com/features/complete-guide-to-using-wapiti-web-vulnerability-scanner-to-keep-your-web-applications-websites-secure"})
-        elif option=="4":
+            wapiti()
+        elif option == "7":
             print(f"\n[+] Nessus")
-            os.system("clear")
-            github=github_getting_text("https://www.techtarget.com/searchnetworking/definition/Nessus",'section[id="content-body"]',0)
-            template.template("nessus","nessus",github.strip(),{"How To: Run Your First Vulnerability Scan with Nessus":"https://www.tenable.com/blog/how-to-run-your-first-vulnerability-scan-with-nessus","A brief introduction to the Nessus vulnerability scanner":"https://resources.infosecinstitute.com/topic/a-brief-introduction-to-the-nessus-vulnerability-scanner/","Beginner’s Guide to Nessus":"https://www.hackingarticles.in/beginners-guide-to-nessus/","Nessus Ubuntu Installation and Tutorial":"https://linuxhint.com/nessus-ubuntu-installation-tutorial/"},link="https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.4.2-debian9_amd64.deb",method="deb")
-        elif option=="5":
+            nessus()
+        elif option == "8":
             print(f"\n[+] dirb")
-            os.system("clear")
-            github = "DIRB IS a Web Content Scanner. It looks for existing (and/or hidden) Web Objects. It basically works by launching a dictionary basesd attack against a web server and analizing the response"
-            template.template("dirb","dirb",github.strip(),{"Dirb — A web content scanner":"https://medium.com/tech-zoom/dirb-a-web-content-scanner-bc9cba624c86","Footprinting and Reconnaissance with DIRB Tool (For Security Researcher and Bug Bounty Hunters":"https://www.openbugbounty.org/blog/mas00712/footprinting-and-reconnaissance-with-dirb-tool-for-security-researcher-and-bug-bounty-hunters/","Comprehensive Guide on Dirb Tool":"https://www.hackingarticles.in/comprehensive-guide-on-dirb-tool/"})
-        elif option=="6":
-            print(f"\n[+] skipfish")
-            os.system("clear")
-            github = "Skipfish is an active web application security reconnaissance tool. It prepares an interactive sitemap for the targeted site by carrying out a recursive crawl and dictionary-based probes. The resulting map is then annotated with the output from a number of active (but hopefully non-disruptive) security checks. The final report generated by the tool is meant to serve as a foundation for professional web application security assessments."
-            template.template("skipfish","skipfish -h",github.strip(),{"Skipfish in Kali Linux":"https://www.javatpoint.com/skipfish-in-kali-linux","Skipfish – Penetration Testing tool in Kali Linux":"https://www.geeksforgeeks.org/skipfish-penetration-testing-tool-in-kali-linux/","skipfish (1) - Linux Man Pages":"https://www.systutorials.com/docs/linux/man/1-skipfish/","Skipfish – Web Application Security Scanner for XSS, SQL Injection, Shell injection":"https://gbhackers.com/skipfish-web-application-security-scanner/"})
-        elif option=="7":
+            dirb()
+        elif option == "9":
             print(f"\n[+] Nuclei")
-            os.system("clear")
-            github=github_getting_text("https://github.com/projectdiscovery/nuclei",'p[dir="auto"]',3)
-            template.template("nuclei","nuclei -h",github.strip(),{"Nuclei - Automated Vulnerability Scanning Tool":"https://allabouttesting.org/nuclei-automated-vulnerability-scanning-tool/","Nuclei – Fast and Customizable Vulnerability Scanner":"https://www.geeksforgeeks.org/nuclei-fast-and-customizable-vulnerability-scanner/","Gauing+Nuclei for Instant Bounties":"https://infosecwriteups.com/gauing-nuclei-for-instant-bounties-7a8a07979fff ","DevSecOps 101 Part 3: Scanning Live Web Applications with Nuclei":"https://escape.tech/blog/devsecops-part-iii-scanning-live-web-applications"},link="https://github.com/projectdiscovery/nuclei@latest",method="go")
+            nuclei()
+        elif option == "10":
+            print("\n[+] ffuf")
+            ffuf()
         else:
             return
 
-def github_getting_text(link,selector,indexvalue):
-    print(f"Please Wait....\r",end="")
+
+def github_getting_text(link, selector, indexvalue):
+    print(f"Please Wait....\r", end="")
     URL = link
     try:
         r = requests.get(URL)
         soup = BeautifulSoup(r.content, 'html.parser')
         paras = soup.select(selector)
-        #check index value from test file
+        # check index value from test file
         return paras[indexvalue].text
     except:
         return "{colors.red}NotLloaded Because No Internet Connection{colors.reset}"
+
+
+def nikto():
+    os.system("clear")
+    github = github_getting_text(
+                "https://en.wikipedia.org/wiki/Nikto_(vulnerability_scanner)", 'p', 1)
+    template.template("nikto", "nikto ", github.strip(), {'What is Nikto and it’s usages ?': 'https://www.geeksforgeeks.org/what-is-nikto-and-its-usages/',
+                              'Nikto: A Practical Website Vulnerability Scanner': 'https://securitytrails.com/blog/nikto-website-vulnerability-scanner', 'Nikto Official Docs': 'https://github.com/sullo/nikto/wiki'})
+
+
+def nuclei():
+    os.system("clear")
+    github = "Nuclei is a fast vulnerability scanner designed to probe modern applications, infrastructure, cloud platforms, and networks, aiding in the identification and mitigation of exploitable vulnerabilities.At its core, Nuclei uses templates—expressed as straightforward YAML files, that delineate methods for detecting, ranking, and addressing specific security flaws."
+    template.template("nuclei", "nuclei", github.strip(), {"Nuclei - Automated Vulnerability Scanning Tool": "https://allabouttesting.org/nuclei-automated-vulnerability-scanning-tool/", "Nuclei – Fast and Customizable Vulnerability Scanner": "https://www.geeksforgeeks.org/nuclei-fast-and-customizable-vulnerability-scanner/",
+                              "Gauing+Nuclei for Instant Bounties": "https://infosecwriteups.com/gauing-nuclei-for-instant-bounties-7a8a07979fff ", "DevSecOps 101 Part 3: Scanning Live Web Applications with Nuclei": "https://escape.tech/blog/devsecops-part-iii-scanning-live-web-applications"})
+
+def ffuf():
+    os.system("clear")
+    github = "ffuf - Fuzz Faster U Fool.The usage examples below show just the simplest tasks you can accomplish using ffuf."
+    template.template("ffuf", "ffuf", github.strip(), {"How to Fuzz Web Applications using FFuf – Web Security Tutorial": "https://www.freecodecamp.org/news/web-security-fuzz-web-applications-using-ffuf/",
+                                                               "github fuff": "https://github.com/ffuf/ffuf/blob/master/README.md", })
+        
+
+
 def burp_suite():
-        while True:
-            os.system("clear")
-            banner.main()
-            banner.attack("Burp Suite")
-            banner.description("Burp Suite is an integrated platform for performing security testing of web applications. Its various tools work seamlessly together to support the entire testing process, from initialmapping and analysis of an application's attack surface, through to finding and exploiting security vulnerabilities. Burp gives you full control, letting you combine advanced manual techniques with state-of-the-art automation, to make your work faster, more effective, and more fun.")
-            ask=template.tool_writeups("burp"," "," ")
-            if ask=="1":
+    while True:
+        os.system("clear")
+        banner.main()
+        banner.attack("Burp Suite")
+        banner.description("Burp Suite is an integrated platform for performing security testing of web applications. Its various tools work seamlessly together to support the entire testing process, from initialmapping and analysis of an application's attack surface, through to finding and exploiting security vulnerabilities. Burp gives you full control, letting you combine advanced manual techniques with state-of-the-art automation, to make your work faster, more effective, and more fun.")
+        ask = template.tool_writeups("burp", " ", " ")
+        if ask == "1":
+            try:
+                professional = input(
+                    f"{colors.blue}[+] Do You Want It's Professional Version?(Y/N){colors.reset}")
+            except KeyboardInterrupt:
+                return
+            if professional == "y" or professional == "Y" or professional == "Yes" or professional == "yes":
+                # clone repo
+                path = 'Burp-Suite'
+                isExist = os.path.exists(path)
+                if isExist:
+                    print(f"{colors.green}[+] It Is Installed{colors.reset}")
                     try:
-                        professional=input(f"{colors.blue}[+] Do You Want It's Professional Version?(Y/N){colors.reset}")
+                        professional = input(
+                            f"{colors.blue}[+] Do You Want Run It?(Y/N){colors.reset}")
                     except KeyboardInterrupt:
+                        return
+                    if professional == "y" or professional == "Y" or professional == "Yes" or professional == "yes":
+                        print(
+                            f"{colors.yellow}[+] Please Wait....{colors.reset}")
+                        os.system(
+                            "cd Burp-Suite && bash installed.sh > /dev/null 2>&1")
+                else:
+                    os.system(
+                        "git clone https://github.com/hardikhacker/Burp-Suite")
+                    try:
+                        professional = input(
+                            f"{colors.blue}[+] Do You Want Run It?(Y/N){colors.reset}")
+                    except:
                         template.exit_program()
-                    if professional=="y" or professional=="Y" or professional=="Yes" or professional=="yes":
-                        #clone repo
-                        path = 'Burp-Suite'
-                        isExist = os.path.exists(path)
-                        if isExist:
-                            print(f"{colors.green}[+] It Is Installed{colors.reset}")
-                            try:
-                                professional=input(f"{colors.blue}[+] Do You Want Run It?(Y/N){colors.reset}")
-                            except KeyboardInterrupt:
-                                template.exit_program()
-                            if professional=="y" or professional=="Y" or professional=="Yes" or professional=="yes":
-                                print(f"{colors.yellow}[+] Please Wait....{colors.reset}")
-                                os.system("cd Burp-Suite && bash installed.sh > /dev/null 2>&1")
-                        else:
-                            os.system("git clone https://github.com/hardikhacker/Burp-Suite")
-                            try:
-                                professional=input(f"{colors.blue}[+] Do You Want Run It?(Y/N){colors.reset}")
-                            except:
-                                template.exit_program()
-                            if professional=="y" or professional=="Y" or professional=="Yes" or professional=="yes":
-                                print(f"{colors.yellow}[+] Please Wait....{colors.reset}")
-                                os.system("cd Burp-Suite && chmod +x * && ./Kali_Linux_Setup.sh > /dev/null 2>&1")
-                    else:
-                        print(f"{colors.blue}[+] CHECKING OF COMMUNITY VERSION IS INSTALLED OR NOT{colors.reset}")
-                        #check for installation
-                        template.check_installed("burpsuite","burpsuite")
-                        waiting.waiting()
-            elif ask=="2":
-                #first argument for dictionary(key=title,value=url) second argument for banner 
-                writeup.writeup({"Top 10 tips for burpsuite":"https://medium.com/r3d-buck3t/top-10-tips-for-burp-suite-72212d22328f","Setting up burbsuite":"https://thexssrat.medium.com/setting-up-burp-suite-b0a6767d3408","Burp Suite: Do I need the professional edition?":"https://thexssrat.medium.com/burp-suite-do-i-need-the-professional-edition-bf8c87ce236e","Burp Suite Extensions to help you Pentest":"https://medium.com/codex/burp-suite-extensions-to-help-you-pentest-97f22a7d7d4d","FIND MORE resources here":"https://medium.com/search?q=burpsuite"},"Brup Suit writeup.writeup")
+                    if professional == "y" or professional == "Y" or professional == "Yes" or professional == "yes":
+                        print(
+                            f"{colors.yellow}[+] Please Wait....{colors.reset}")
+                        os.system(
+                            "cd Burp-Suite && chmod +x * && ./Kali_Linux_Setup.sh > /dev/null 2>&1")
             else:
-                break
+                print(
+                    f"{colors.blue}[+] CHECKING OF COMMUNITY VERSION IS INSTALLED OR NOT{colors.reset}")
+                # check for installation
+                template.check_installed("burpsuite", "burpsuite")
+                waiting.waiting()
+        elif ask == "2":
+            # first argument for dictionary(key=title,value=url) second argument for banner
+            writeup.writeup({"Setting up Burpsuite Professional": "https://github.com/THECH13F/Burp-Suite/blob/main/Readme.md","Top 10 tips for burpsuite": "https://medium.com/r3d-buck3t/top-10-tips-for-burp-suite-72212d22328f", "Setting up burbsuite": "https://thexssrat.medium.com/setting-up-burp-suite-b0a6767d3408", "Burp Suite: Do I need the professional edition?":
+                            "https://thexssrat.medium.com/burp-suite-do-i-need-the-professional-edition-bf8c87ce236e", "Burp Suite Extensions to help you Pentest": "https://medium.com/codex/burp-suite-extensions-to-help-you-pentest-97f22a7d7d4d", "FIND MORE resources here": "https://medium.com/search?q=burpsuite"}, "Brup Suit writeup.writeup")
+        elif ask == "3":
+            template.uninstall_tool("","burp")
+        else:
+            break
+
+
+def owasp_zap():
+    os.system("clear")
+    github = "The OWASP Zed Attack Proxy (ZAP) is an easy to use integrated penetration testing tool for finding vulnerabilities in web applications.\nIt is designed to be used by people with a wide range of security experience and as such is ideal for developers and functional testers who are new to penetration testing as well as being a useful addition to an experienced pen testers toolbox. https://www.owasp.org/index.php/ZAP"
+    template.template('zaproxy', 'zaproxy', github.strip(), {"How to setup OWASP ZAP to scan your web application for security vulnerabilities": "https://www.linkedin.com/pulse/how-setup-owasp-zap-scan-your-web-application-security-botla/", "Authenticated Scan using OWASP-ZAP in Windows.": "https://medium.com/@secureica/authenticated-scan-using-owasp-zap-f0a71dafe41",
+                      "OWASP ZAP: 6 Key Capabilities and a Quick Tutorial": "https://www.hackerone.com/knowledge-center/owasp-zap-6-key-capabilities-and-quick-tutorial", "Initial Setup": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/untitled", "Setup OWASP ZAP": "https://infosecgirls.gitbook.io/infosecgirls-training/v/appsec/initial-setup-with-owasp-zap/setup-owasp-zap"})
+
+
+def nessus():
+    os.system("clear")
+    version_grab = github_getting_text("https://www.tenable.com/downloads/nessus?loginAttempted=true",
+                                          'div[class="multi-select__single-value css-1uccc91-singleValue"]', 0).strip()
+    version = version_grab.strip().replace(" ", "")
+    github = "Nessus is a platform developed by Tenable that scans for security vulnerabilities in devices, applications, operating systems, cloud services and other network resources.Originally launched as an open source tool in 1998, its enterprise edition became a commercial product in 2005. Nessus now encompasses several products that automate point-in-time vulnerability assessments of a network's attack surface, with the goal of enabling enterprise IT teams to stay ahead of cyber attackers by proactively identifying and fixing vulnerabilities as the tool discovers them, rather than after attackers exploit them.Nessus identifies software flaws, missing patches, malware, denial-of-service vulnerabilities, default passwords and misconfiguration errors, among other potential flaws. When Nessus discovers vulnerabilities, it issues an alert that IT teams can then investigate and determine what -- if any -- further action is required."
+    template.template("nessus", "nessus", github.strip(), {"How To: Run Your First Vulnerability Scan with Nessus": "https://www.tenable.com/blog/how-to-run-your-first-vulnerability-scan-with-nessus", "A brief introduction to the Nessus vulnerability scanner": "https://resources.infosecinstitute.com/topic/a-brief-introduction-to-the-nessus-vulnerability-scanner/",
+                      "Beginner’s Guide to Nessus": "https://www.hackingarticles.in/beginners-guide-to-nessus/", "Nessus Ubuntu Installation and Tutorial": "https://linuxhint.com/nessus-ubuntu-installation-tutorial/"}, link=f"https://www.tenable.com/downloads/api/v2/pages/nessus/files/{version}-debian10_amd64.deb", method="deb")
+
+
+
+def dirb():
+    os.system("clear")
+    github = "DIRB IS a Web Content Scanner. It looks for existing (and/or hidden) Web Objects. It basically works by launching a dictionary basesd attack against a web server and analizing the response"
+    template.template("dirb", "dirb", github.strip(), {"Dirb — A web content scanner": "https://medium.com/tech-zoom/dirb-a-web-content-scanner-bc9cba624c86", "Footprinting and Reconnaissance with DIRB Tool (For Security Researcher and Bug Bounty Hunters":
+                      "https://www.openbugbounty.org/blog/mas00712/footprinting-and-reconnaissance-with-dirb-tool-for-security-researcher-and-bug-bounty-hunters/", "Comprehensive Guide on Dirb Tool": "https://www.hackingarticles.in/comprehensive-guide-on-dirb-tool/"})
+
+
+def dirsearch():
+    os.system("clear")
+    github = "As a feature-rich tool, dirsearch gives users the opportunity to perform a complex web content discovering, with many vectors for the wordlist, high accuracy, impressive performance, advanced connection/request settings, modern brute-force techniques and nice output."
+    template.template("dirsearch", "dirsearch --help ", github.strip(), {"Dirserach helpfile": "https://www.kali.org/tools/dirsearch/",
+                      "Find Hidden Web Directories with Dirsearch ": "https://null-byte.wonderhowto.com/how-to/find-hidden-web-directories-with-dirsearch-0201615/", })
+
+
+def wapiti():
+    os.system("clear")
+    github = github_getting_text("https://wapiti-scanner.github.io/", 'p', 6)
+    template.template("wapiti", "wapiti", github.strip(), {"wapiti free web application vulnerability scanner": "https://pentestit.medium.com/wapiti-free-web-application-vulnerability-scanner-ce7712adf644", "Official docs": "https://github.com/wapiti-scanner/wapiti", "wapiti tutorial":
+                      "https://www.kalilinux.in/2021/01/wapiti-tutorial.html", "complete guide to using wapiti web vulnerability scanner to keep your web applications websites secure": "https://linuxsecurity.com/features/complete-guide-to-using-wapiti-web-vulnerability-scanner-to-keep-your-web-applications-websites-secure"})
+
 
-if __name__ == "__main__": 
+if __name__ == "__main__":
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/Wireless_Hacking.py` & `cyberonix-3.0.0/cyberonix/main/tools/Wireless_Hacking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,92 @@
 from bs4 import BeautifulSoup
-from cyberonix.main.tools import banner,colors,template
+from cyberonix.main.tools import banner, colors, template
 import os
 import requests
 from bs4 import BeautifulSoup
 
+
 def main():
     while True:
         os.system("clear")
         banner.main()
         banner.attack("Wireless Hacking")
-        list_attacks = ["Kismet", "Wifite", "Fern Wifi Cracker",
-                        "Aircrack-ng", "Fluxion", "Wifiphisher", "go back"]
+        list_attacks = ["Kismet\t\t(Recommended)", "Wifite", "Fern Wifi Cracker",
+                        "Aircrack-ng\t\t(Recommended)", "Fluxion", "Wifiphisher\t\t(Recommended)", "go back"]
         for i in range(len(list_attacks)):
-            print(colors.options,f"{i}) {list_attacks[i]}".title(),colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+            option = input(
+                f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
+            return
+        if option == "1":
             print("\n[+] Kismet")
-            github = github_getting_text("https://github.com/kismetwireless/kismet-docs/blob/master/readme/000-intro.md", 'p[dir="auto"]', 0)
-            template.template("kismet","kismet",github.strip(),{"Kismet -- WiFi Sniffer": "https://www.kalilinux.in/2019/02/kismet-wifi-sniffer.html", "Use Kismet to Watch Wi-Fi User Activity": "https://null-byte.wonderhowto.com/how-to/use-kismet-watch-wi-fi-user-activity-through-walls-0182214/",
-                    "HACKING WIFI USING KISMET": "https://www.bookofnetwork.com/hacking-tutorials/Kismet-Wireless", "How To Use Kismet Kali Linux?": "https://www.systranbox.com/how-to-use-kismet-kali-linux/"})
-        elif option == "1":
-            print("\n[+] Wifite")
-            github = github_getting_text("https://www.kali.org/tools/wifite/", 'p', 1)
-            template.template("wifite","wifite -h",github.strip(),{"Wifite walkthrough Part-1": "https://resources.infosecinstitute.com/topic/wifite-walkthrough-part-1/", "Wifite walkthrough Part-2": "https://resources.infosecinstitute.com/topic/wifite-walkthrough-part-2/",
-                    "Wireless pentesting with Wifite": "https://www.hackingarticles.in/wireless-penetration-testing-wifite/", "Wifite - Automated Wifi hacking tool": "https://kalitut.com/wifite-automated-wi-fi-hacking-tool/"})
+            kismet()        
         elif option == "2":
-            print("\n[+] Fern Wifi Cracker")
-            github = github_getting_text("https://github.com/savio-code/fern-wifi-cracker", 'p[dir="auto"]', 0)
-            template.template("fern-wifi-cracker","fern-wifi-cracker",github.strip(),{"What is Fern Wifi Cracker": "https://www.kalilinux.in/2020/09/fern-wifi-cracker.html", "Hacking Wifi networks using Fern Wifi Cracker": "https://www.studocu.com/en-au/document/western-sydney-university/it-product-support-and-services/fern-wifi-cracker-hacking-wifi-networks-using-fern-wifi-cracker-easily/10772514",
-                    "Wireless penetration testing - Fern ": "https://www.hackingarticles.in/wireless-penetration-testing-fern/", "Cracking wifi passwords using Fern": "https://hacking84.rssing.com/chan-13108703/article238.html"})
+            print("\n[+] Wifite")
+            wifite()        
         elif option == "3":
-            print("\n[+] Aircrack-ng")
-            github = github_getting_text("https://www.kali.org/tools/aircrack-ng/", 'p', 32)
-            template.template("aircrack-ng","aircrack-ng --help",github.strip(),{"How to use Aircrack-ng": "https://linuxhint.com/how_to_aircrack_ng/", "Aircrack-ng Practical Demonstration Tutorial": "https://techofide.com/blogs/how-to-use-aircrack-ng-aircrack-ng-tutorial-practical-demonstration/",
-                    "Hacking the wireless network in 5 simple steps": "https://www.hackingloops.com/how-to-use-aircrack-kali/", "Crack WPA/WPA2 WiFi Passwords using Aircrack-ng & Kali Linux": "https://nooblinux.com/crack-wpa-wpa2-wifi-passwords-using-aircrack-ng-kali-linux/"})
+            print("\n[+] Fern Wifi Cracker")
+            fernwificracker()        
         elif option == "4":
-            print("\n[+] Fluxion")
-            github = github_getting_text("https://github.com/FluxionNetwork/fluxion", 'p[dir="auto"]', 1)
-            template.template("fluxion","./fluxion.sh -h",github.strip(),{"Fluxion kali linux tutorial": "https://linuxhint.com/fluxion-kali-linux-tutorial/", "Fluxion - Wifi security auditing tool": "https://www.hackingloops.com/fluxion/", "Fluxion -- Crack WiFi Passwords in Minutes": "https://www.kalilinux.in/2020/07/fluxion-kali-linux-crack-wifi.html",
-                    "Cracking WPA/WPA2 Passwords in Minutes with Fluxion": "https://gbhackers.com/cracking-wpawpa2-passwords-fluxion/amp/", "Wireless Penetration Testing: Fluxion": "https://www.hackingarticles.in/wireless-penetration-testing-fluxion/", "Fluxion in Kali Linux usage": "https://www.cyberpratibha.com/blog/fluxion-wpa-wpa2-hacking/"}, github_install="git clone https://github.com/FluxionNetwork/fluxion.git",method="github",github_check="fluxion")
+            print("\n[+] Aircrack-ng")
+            aircrack_ng()    
         elif option == "5":
+            print("\n[+] Fluxion")
+            fluxion()    
+        elif option == "6":
             print("\n[+] Wifiphisher")
-            github = github_getting_text("https://github.com/wifiphisher/wifiphisher", 'p[dir="auto"]', 2)
-            template.template("wifiphisher","wifiphisher -h",github.strip(),{"WiFi Exploitation with WifiPhisher": "https://www.hackingarticles.in/wifi-exploitation-wifiphisher/", "wifiphisher Description": "https://en.kali.tools/?p=90", "Read Team engagement on Wifi with Wifiphisher": "https://whitehatinstitute.com/conduct-red-team-engagements-on-wifi-with-wifiphisher/", "Wireless Hacking with WifiPhisher": "https://cntemngwa.medium.com/wireless-hacking-with-wifiphisher-d4b857414146", "WifiPhisher – WiFi Crack and Phishing Framework": "https://latesthackingnews.com/2018/10/02/wifiphisher-wifi-crack-and-phishing-framework/", "Wifiphisher Evil Twin Attack": "https://kalitut.com/wifiphisher-evil-twin-attack/"})
-                    
+            wifiphisher()        
         else:
             return
 
 
-def github_getting_text(link,selector,indexvalue):
-    print("Please Wait....\r",end="")
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
     URL = link
     try:
         r = requests.get(URL)
         soup = BeautifulSoup(r.content, 'html.parser')
         paras = soup.select(selector)
-        #check index value from test file
+        # check index value from test file
         return paras[indexvalue].text
     except:
         return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
 
-if __name__=='__main__':
+def kismet():
+    github = github_getting_text(
+                "https://www.kismetwireless.net/docs/readme/intro/kismet/", 'p', 1)
+    template.template("kismet", "kismet", github.strip(), {"Kismet -- WiFi Sniffer": "https://www.kalilinux.in/2019/02/kismet-wifi-sniffer.html", "Use Kismet to Watch Wi-Fi User Activity": "https://null-byte.wonderhowto.com/how-to/use-kismet-watch-wi-fi-user-activity-through-walls-0182214/",
+                                                                   "HACKING WIFI USING KISMET": "https://www.bookofnetwork.com/hacking-tutorials/Kismet-Wireless", "How To Use Kismet Kali Linux?": "https://www.systranbox.com/how-to-use-kismet-kali-linux/"})
+        
+def wifite():
+    github = github_getting_text(
+                "https://www.kali.org/tools/wifite/", 'p', 1)
+    template.template("wifite", "wifite -h", github.strip(), {"Wifite walkthrough Part-1": "https://resources.infosecinstitute.com/topic/wifite-walkthrough-part-1/", "Wifite walkthrough Part-2": "https://resources.infosecinstitute.com/topic/wifite-walkthrough-part-2/",
+                                                                      "Wireless pentesting with Wifite": "https://www.hackingarticles.in/wireless-penetration-testing-wifite/", "Wifite - Automated Wifi hacking tool": "https://kalitut.com/wifite-automated-wi-fi-hacking-tool/"})
+        
+def fernwificracker():
+    github = "Fern Wifi Cracker is a Wireless security auditing and attack software program written using the Python Programming Language and the Python Qt GUI library. The program is able to crack and recover WEP/WPA/WPS keys and also run other network based attacks on wireless or ethernet based networks."
+    template.template("fern-wifi-cracker", "fern-wifi-cracker", github.strip(), {"What is Fern Wifi Cracker": "https://www.kalilinux.in/2020/09/fern-wifi-cracker.html", "Hacking Wifi networks using Fern Wifi Cracker": "https://www.studocu.com/en-au/document/western-sydney-university/it-product-support-and-services/fern-wifi-cracker-hacking-wifi-networks-using-fern-wifi-cracker-easily/10772514",
+                                                                                         "Wireless penetration testing - Fern ": "https://www.hackingarticles.in/wireless-penetration-testing-fern/", "Cracking wifi passwords using Fern": "https://hacking84.rssing.com/chan-13108703/article238.html"})
+        
+def aircrack_ng():
+    github = github_getting_text(
+                "https://www.kali.org/tools/aircrack-ng/", 'p', 32)
+    template.template("aircrack-ng", "aircrack-ng", github.strip(), {"How to use Aircrack-ng": "https://linuxhint.com/how_to_aircrack_ng/", "Aircrack-ng Practical Demonstration Tutorial": "https://techofide.com/blogs/how-to-use-aircrack-ng-aircrack-ng-tutorial-practical-demonstration/",
+                                                                                    "Hacking the wireless network in 5 simple steps": "https://www.hackingloops.com/how-to-use-aircrack-kali/", "Crack WPA/WPA2 WiFi Passwords using Aircrack-ng & Kali Linux": "https://nooblinux.com/crack-wpa-wpa2-wifi-passwords-using-aircrack-ng-kali-linux/"})
+        
+def fluxion():
+    github = github_getting_text(
+                "https://fluxionnetwork.github.io/fluxion/", 'p', 1)
+    template.template("fluxion", "./fluxion.sh", github.strip(), {"Fluxion kali linux tutorial": "https://linuxhint.com/fluxion-kali-linux-tutorial/", "Fluxion - Wifi security auditing tool": "https://www.hackingloops.com/fluxion/", "Fluxion -- Crack WiFi Passwords in Minutes": "https://www.kalilinux.in/2020/07/fluxion-kali-linux-crack-wifi.html",
+                                                                             "Cracking WPA/WPA2 Passwords in Minutes with Fluxion": "https://gbhackers.com/cracking-wpawpa2-passwords-fluxion/amp/", "Wireless Penetration Testing: Fluxion": "https://www.hackingarticles.in/wireless-penetration-testing-fluxion/", "Fluxion in Kali Linux usage": "https://www.cyberpratibha.com/blog/fluxion-wpa-wpa2-hacking/"},method="github", github_install="git clone https://github.com/FluxionNetwork/fluxion.git && cd fluxion", github_check="fluxion")
+        
+def wifiphisher():
+    github = github_getting_text("https://wifiphisher.org/", 'p', 0)
+    template.template("wifiphisher", "wifiphisher -h", github.strip(), {"WiFi Exploitation with WifiPhisher": "https://www.hackingarticles.in/wifi-exploitation-wifiphisher/", "wifiphisher Description": "https://en.kali.tools/?p=90", "Read Team engagement on Wifi with Wifiphisher": "https://whitehatinstitute.com/conduct-red-team-engagements-on-wifi-with-wifiphisher/",
+                              "Wireless Hacking with WifiPhisher": "https://cntemngwa.medium.com/wireless-hacking-with-wifiphisher-d4b857414146", "WifiPhisher – WiFi Crack and Phishing Framework": "https://latesthackingnews.com/2018/10/02/wifiphisher-wifi-crack-and-phishing-framework/", "Wifiphisher Evil Twin Attack": "https://kalitut.com/wifiphisher-evil-twin-attack/"})
+
+
+if __name__ == '__main__':
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/dos.py` & `cyberonix-3.0.0/cyberonix/main/tools/dos.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,104 +14,114 @@
             "GoldenEye",
             "SlowHTTPTest",
             "THC-SSL-DOS",
             "Slowloris",
             "go back",
         ]
         for i in range(len(list_attacks)):
-            print(colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset)
+            print(colors.options, f"{i+1}) {list_attacks[i]}".title(), colors.reset)
         try:
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if option == "0":
+            return
+        if option == "1":
             print("\n[+] GoldenEye")
-            github = github_getting_text(
-                "https://www.kali.org/tools/goldeneye/", "p", 0
-            )
-            template.template(
-                "goldeneye",
-                "goldeneye -h",
-                github.strip(),
-                {
-                    "Goldeneye DDos Tool in Kali Linux": "https://www.geeksforgeeks.org/goldeneye-ddos-tool-in-kali-linux/",
-                    "Golden Eye DDoS Tool: Installation and Tool usage with examples": "https://allabouttesting.org/golden-eye-ddos-tool-installation-and-tool-usage-with-examples/",
-                    "DoS website in Kali Linux using GoldenEye": "https://www.blackmoreops.com/2015/05/18/dos-website-in-kali-linux-using-goldeneye/",
-                    "DoS website with GoldenEye - Layer 7 DoS tool": "https://www.darkmoreops.com/2014/11/22/dos-website-with-goldeneye/",
-                },
-            )  # method=kali
-        elif option == "1":
+            goldeneye()        
+            # method=kali
+        elif option == "2":
             print("\n[+] Slowhttptest")
-            github = github_getting_text(
-                "https://www.kali.org/tools/slowhttptest/", "p", 1
-            )
-            template.template(
-                "slowhttptest",
-                "slowhttptest -h",
+            slowhttptest()        
+            # method is kali
+        elif option == "3":
+            print("\n[+] THC-SSL-DOS")
+            thc_ssl_dos()        
+            # method is kali
+        elif option == "4":
+            print("\n[+] SlowLoris")
+            slowloris()        
+
+        else:
+            return
+
+
+def github_getting_text(link, selector, indexvalue):
+    print("Please Wait....\r", end="")
+    URL = link
+    try:
+        r = requests.get(URL)
+        soup = BeautifulSoup(r.content, "html.parser")
+        paras = soup.select(selector)
+        # check index value from test file
+        return paras[indexvalue].text
+    except:
+        return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
+
+def slowloris():
+    github = "Slowloris is a Low bandwidth  HTTP Denial of Service attack that affects threaded servers"
+    template.template(
+                "Slowloris",
+                "python3 slowloris.py -h",
                 github.strip(),
                 {
-                    'How to perform a DoS attack "Slow HTTP" with SlowHTTPTest': "https://ourcodeworld.com/articles/read/949/how-to-perform-a-dos-attack-slow-http-with-slowhttptest-test-your-server-slowloris-protection-in-kali-linux",
-                    "slowhttptest Usage Example": "https://www.kali.org/tools/slowhttptest/",
-                    "DoS website using slowhttptest in Kali Linux ": "https://www.blackmoreops.com/2015/06/07/attack-website-using-slowhttptest-in-kali-linux/",
-                    "Kali Linux - Stressing Tools": "https://www.tutorialspoint.com/kali_linux/kali_linux_stressing_tools.htm",
-                    "How to perform SlowHTTPtest DOS attack ": "https://support.tetcos.com/support/solutions/articles/14000130254-how-to-perform-slowhttptest-dos-attack-through-netsim-emulator-",
+                    "Slowloris DDOS Attack Tool in Kali Linux": "https://www.geeksforgeeks.org/slowloris-ddos-attack-tool-in-kali-linux/",
+                    "What is Slowloris?": "https://www.imperva.com/learn/ddos/slowloris/",
+                    "Performing a genuine slowloris attack": "https://ourcodeworld.com/articles/read/962/performing-a-genuine-slowloris-attack-slowhttp-of-indefinite-length-in-kali-linux",
                 },
-            )  # method is kali
-        elif option == "2":
-            print("\n[+] THC-SSL-DOS")
-            github = github_getting_text(
+                link="https://github.com/gkbrk/slowloris.git",
+                method="github",
+                github_install="git clone https://github.com/gkbrk/slowloris.git",
+                github_check="slowloris",
+            )
+def thc_ssl_dos():
+    github = github_getting_text(
                 "https://www.kali.org/tools/thc-ssl-dos/", "p", 1
             )
-            github += github_getting_text(
+    github += github_getting_text(
                 "https://www.kali.org/tools/thc-ssl-dos/", "p", 2
             )
-            github += github_getting_text(
+    github += github_getting_text(
                 "https://www.kali.org/tools/thc-ssl-dos/", "p", 3
             )
-            template.template(
+    template.template(
                 "thc-ssl-dos",
                 "thc-ssl-dos -h",
                 github.strip(),
                 {
                     "THC-SSL DoS": "https://www.radware.com/security/ddos-knowledge-center/ddospedia/thc-ssl-dos/",
                     "thc-ssl-dos Usage Example": "https://www.kali.org/tools/thc-ssl-dos/",
                     "THC-SSL-DOS – DoS Tool Against Secure Web-Servers and for Testing SSL-Renegotiation": "https://kalilinuxtutorials.com/thc-ssl-dos/",
                     "The THC SSL DoS Threat": "https://resources.infosecinstitute.com/topic/thc-ssl-dos-threat/",
                 },
-            )  # method is kali
-        elif option == "3":
-            print("\n[+] SlowLoris")
-            github = "Slowloris is a Low bandwidth  HTTP Denial of Service attack that affects threaded servers"
-            template.template(
-                "Slowloris",
-                "python slowloris.py -h",
+            )
+def slowhttptest():
+    github = github_getting_text(
+                "https://www.kali.org/tools/slowhttptest/", "p", 1
+            )
+    template.template(
+                "slowhttptest",
+                "slowhttptest -h",
                 github.strip(),
                 {
-                    "Slowloris DDOS Attack Tool in Kali Linux": "https://www.geeksforgeeks.org/slowloris-ddos-attack-tool-in-kali-linux/",
-                    "What is Slowloris?": "https://www.imperva.com/learn/ddos/slowloris/",
-                    "Performing a genuine slowloris attack": "https://ourcodeworld.com/articles/read/962/performing-a-genuine-slowloris-attack-slowhttp-of-indefinite-length-in-kali-linux",
+                    'How to perform a DoS attack "Slow HTTP" with SlowHTTPTest': "https://ourcodeworld.com/articles/read/949/how-to-perform-a-dos-attack-slow-http-with-slowhttptest-test-your-server-slowloris-protection-in-kali-linux",
+                    "slowhttptest Usage Example": "https://www.kali.org/tools/slowhttptest/",
+                    "DoS website using slowhttptest in Kali Linux ": "https://www.blackmoreops.com/2015/06/07/attack-website-using-slowhttptest-in-kali-linux/",
+                    "Kali Linux - Stressing Tools": "https://www.tutorialspoint.com/kali_linux/kali_linux_stressing_tools.htm",
+                    "How to perform SlowHTTPtest DOS attack ": "https://support.tetcos.com/support/solutions/articles/14000130254-how-to-perform-slowhttptest-dos-attack-through-netsim-emulator-",
                 },
-                link="https://github.com/gkbrk/slowloris.git",
-                method="github",
-                github_install="git clone https://github.com/gkbrk/slowloris.git",
-                github_check="slowloris",
             )
-
-        else:
-            return
-
-
-def github_getting_text(link, selector, indexvalue):
-    print("Please Wait....\r", end="")
-    URL = link
-    try:
-        r = requests.get(URL)
-        soup = BeautifulSoup(r.content, "html.parser")
-        paras = soup.select(selector)
-        # check index value from test file
-        return paras[indexvalue].text
-    except:
-        return f"{colors.red}Not Loaded Because No Internet Connection{colors.reset}"
-
-
+def goldeneye():
+    github = github_getting_text(
+                "https://www.kali.org/tools/goldeneye/", "p", 0
+            )
+    template.template(
+                "goldeneye",
+                "goldeneye -h",
+                github.strip(),
+                {
+                    "Goldeneye DDos Tool in Kali Linux": "https://www.geeksforgeeks.org/goldeneye-ddos-tool-in-kali-linux/",
+                    "Golden Eye DDoS Tool: Installation and Tool usage with examples": "https://allabouttesting.org/golden-eye-ddos-tool-installation-and-tool-usage-with-examples/",
+                    "DoS website in Kali Linux using GoldenEye": "https://en.iguru.gr/odigos-epitheseon-ddos-goldeneye/",
+                    "DoS website with GoldenEye - Layer 7 DoS tool": "https://www.darkmoreops.com/2014/11/22/dos-website-with-goldeneye/",
+                },
+            ) 
 if __name__ == "__main__":
     main()
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/html5.py` & `cyberonix-3.0.0/cyberonix/main/tools/html5.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,52 +13,52 @@
         list_vulns = [
             "WEB Messaging",
             "WEB Storage SQL Injection",
             "CORS Implementation",
             "Go back",
         ]
         for i in range(len(list_vulns)):
-            print(colors.options, f"{i}) {list_vulns[i]}".title(), colors.reset)
+            print(colors.options, f"{i+1}) {list_vulns[i]}".title(), colors.reset)
         try:
             vulns = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
-            template.exit_program()
-        if vulns == "0":
+            return
+        if vulns == "1":
             github = "Web messaging is the ability to send realtime messages from the server to the client browser. It overrides the cross domain communication problem in different domains, protocols or ports"
             template.template(
                 "WEB Messaging",
                 "no-tools",
                 github.strip(),
                 {
                     "HTML5 - Web messaging": "https://www.tutorialspoint.com/html5/html5_web_messaging.htm",
                     "Testing Web Messaging": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/11-Client-side_Testing/11-Testing_Web_Messaging",
                     "Web message manipulation": "https://portswigger.net/web-security/dom-based/web-message-manipulation",
                     "HTML5 Security: Cross Domain Messaging": "https://resources.infosecinstitute.com/topic/html5-security-cross-domain-messaging/",
                     "Testing for DOM XSS using web messages": "https://portswigger.net/burp/documentation/desktop/tools/dom-invader/web-messages",
                 },
             )
 
-        elif vulns == "1":
+        elif vulns == "2":
             github = "SQL injection testing checks if it is possible to inject data into the application so that it executes a user-controlled SQL query in the database. Testers find a SQL injection vulnerability if the application uses user input to create SQL queries without proper input validation. "
             template.template(
                 "WEB Storage SQL Injection",
                 "no-tools",
                 github.strip(),
                 {
                     "Testing Browser Storage": "https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/11-Client_Side_Testing/12-Testing_Browser_Storage",
                     "Testing for SQL Injection": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/07-Input_Validation_Testing/05-Testing_for_SQL_Injection",
                     "Client-side SQL injection": "https://portswigger.net/kb/issues/00200332_client-side-sql-injection-stored-dom-based",
                     "Secure Implementation of HTML5's Web SQL Database": "https://code.google.com/archive/p/html5security/wikis/WebSQLDatabaseSecurity.wiki",
                 },
             )
 
-        elif vulns == "2":
+        elif vulns == "3":
             github = "Cross-origin resource sharing (CORS) is a mechanism that allows restricted resources on a web page to be requested from another domain outside the domain from which the first resource was served."
             template.template(
-                "WEB Storage SQL Injection",
+                "CORS implementation",
                 "no-tools",
                 github.strip(),
                 {
                     "What is Web CORS in HTML5 ?": "https://www.geeksforgeeks.org/what-is-web-cors-in-html5/",
                     "Cross-origin resource sharing (CORS)": "https://portswigger.net/web-security/cors",
                     "Testing Cross Origin Resource Sharing": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/11-Client-side_Testing/07-Testing_Cross_Origin_Resource_Sharing",
                     "CORS Misconfiguration": "https://systemweakness.com/first-bug-bounty-program-found-cors-cross-origin-resource-sharing-misconfiguration-52c1bd3ebfe0",
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/run_on_browser.py` & `cyberonix-3.0.0/cyberonix/main/tools/run_on_browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 def main(URL):
         # print("[+] Opening url")
-        print("[+] Opening Article")
+        print("[+] Opening.....")
         user=os.getlogin()
         if "root" in user:
             os.system(f"firefox {URL} > /dev/null 2>&1" )
         else:
             os.system(f"sudo chown root:root /run/user/{user}/gdm/Xauthority > /dev/null 2>&1")
             os.system(f"sudo chown root:root /home/{user}/.Xauthority > /dev/null 2>&1")
             os.system(f"firefox {URL} > /dev/null 2>&1")
             os.system(f"sudo chown {user}:{user} /run/user/{user}/gdm/Xauthority > /dev/null 2>&1")
-            os.system(f"sudo chown {user}:{user} /home/{user}/.Xauthority > /dev/null 2>&1")
-
+            os.system(f"sudo chown {user}:{user} /home/{user}/.Xauthority > /dev/null 2>&1")
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/template.py` & `cyberonix-3.0.0/cyberonix/main/tools/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cyberonix.main.tools import banner, waiting, writeup, colors, run_on_browser
+from cyberonix.main.tools import banner, waiting, writeup, colors, run_on_browser, Recommended_Tool
 import os
 import subprocess
 import threading
 
 
 class template:
     def __init__(
@@ -20,14 +20,15 @@
         self.command = command
         self.method = method
         self.discription = discription
         self.writeup = writeups
         self.link = link
         self.github_install = github_install
         self.github_check = github_check
+        
         while True:
             os.system("clear")
             banner.main()
             banner.attack(self.name)
             if command!="no-tools":
                 banner.description(self.discription)
             else:
@@ -55,88 +56,151 @@
                             target=run_on_browser.main,
                             args=(self.command,)
                         ).start()
                     elif method == "github":
                         if not os.path.isdir("Tools"):
                             os.system("mkdir Tools")
                         if os.path.exists(f"Tools/{self.github_check}"):
-                            print(f"{colors.green}[+] It Is Installed")
-                            print(f"[+] It Is Installed In Your Kali{colors.reset}")
+                            print(f"{colors.green}[+] Installed")
                             run = input(
                                 f"{colors.blue}[+] Do You Want To Run?(y/n):{colors.reset}"
                             )
                             if run.lower() == "yes" or run.lower() == "y":
-                                os.system(
-                                    f"cd Tools/{self.github_check} && {self.command}"
-                                )
+                               
+                                #os.system(f"cd Tools/{self.github_check} && {self.command}")
+                                Recommended_Tool.recommended(name=name)
+                                
                         else:
                             print(f"{colors.red}[-] Not Installed{colors.reset}")
-                            print(f"{colors.red}[+] It Is Not Installed In Your Kali{colors.reset}")
                             installed = input(
                                 f"{colors.blue}Do You Want To Install The Tool?(y/n):{colors.reset}"
                             )
                             if installed.lower() == "y" or installed.lower() == "yes":
                                 os.system(f"cd Tools && {self.github_install}")
+                                path = check_path(self.github_check)
+                                print(f"\nInstalled folder path : {path}")
                                 run = input(
                                     f"{colors.blue}[+] Do You Want To Run?(y/n):{colors.reset}"
                                 )
                                 if run.lower() == "yes" or run.lower() == "y":
-                                    os.system(
-                                        f"cd Tools/{self.github_check} && {self.command}"
-                                    )
+                                    #os.system(f"cd Tools/{self.github_check} && {self.command}")
+                                    Recommended_Tool.recommended(name=name)
+                                   
                         waiting.waiting()
             elif ask == "2":
                 if self.writeup == "no-writeups":
                     pass
                 else:
                     writeup.writeup(self.writeup, self.name)
+            elif ask == "3":
+                if method == "github":
+                    uninstall_tool(method, self.github_check)
+                else:
+                    uninstall_tool(method,name)
             else:
                 break
+          
 
+def check_path(name):   
+    def find_folder(folder_name, root_folder="/"):
+        for folder, subfolders, files in os.walk(root_folder):
+            if folder_name in subfolders:
+                return os.path.join(folder, folder_name)
+        return "Folder not found"
+    #folder_name = input("Enter the name of the folder you want to find: ")
+    folder_name = name
+    folder_path = find_folder(folder_name)
+    #print("Folder Path:", folder_path)
+    return folder_path
+
+def uninstall_tool(method,name):
+    if method == "kali":
+            run = input(f"\033[1m{colors.red}[+] Do You Want To Uninstall the Tool?(y/n):{colors.reset}")
+            if run.lower() == "y" or run.lower() == "yes":
+	    	        os.system(f"sudo apt remove {name}")
+    elif method == "go" :
+            run = input(f"\033[1m{colors.red}[+] Do You Want To Uninstall the Tool?(y/n):{colors.reset}")
+            if run.lower() == "y" or run.lower() == "yes":
+	    	        os.system(f"rm -rf ~/go/bin/{name}")
+    elif method == "pip":
+            run = input(f"\033[1m{colors.red}[+] Do You Want To Uninstall the Tool?(y/n):{colors.reset}")
+            if run.lower() == "y" or run.lower() == "yes":
+	    	        os.system(f"pip uninstall {name}")
+    elif method == "deb":
+            run = input(f"\033[1m{colors.red}[+] Do You Want To Uninstall the Tool?(y/n):{colors.reset}")
+            if run.lower() == "y" or run.lower() == "yes":
+	    	        os.system(f"sudo dpkg –purge {name}")	 
+    elif method == "github":
+            run = input(f"\033[1m{colors.red}[+] Do You Want To Github Uninstall the Tool?(y/n):{colors.reset}")
+            if run.lower() == "y" or run.lower() == "yes":
+
+                print("Uninstallation...")
+                folder_path = check_path(name)
+                os.system(f'rm -rf {folder_path}')
+                waiting.waiting()
+    elif name == "burp":  
+            print(f"{colors.blue}[+]1. Do You Want Uninstall Professional Version?{colors.reset}")
+            print(f"{colors.blue}[+]2. Do You Want Uninstall COMMUNITY VERSION?{colors.reset}")
+            run = input(f"\033[1m{colors.red}[+] press 1 for Professional Version and 2 for COMMUNITY VERSION : {colors.reset}")
+            if run == "1":
+                print("Uninstallation...")
+                folder_path = check_path("Burp-Suite")
+                os.system(f'rm -rf {folder_path}')
+                waiting.waiting()
+            if run == "2":
+                print("Uninstallation...")
+                os.system("sudo  apt remove burpsuite")
+                waiting.waiting()
 
+def load_banner(name):
+    os.system("clear")
+    banner.main()
+    banner.attack(name)
 def tool_writeups(name,check="no-writeups", tool_check="no-tools"):
     if tool_check != "no-tools":
-        print(f"{colors.options}1) Installation")
+        print(f"{colors.options}1) Launch")
     if check != "no-writeups":
         print(f"2) Write Ups")
-    print(f"3) Go Back..")
+    if check != "uninstall-tool":
+        print(f"3) Uninstall ") 	
+    print(f"4) Go Back..")
     try:
         ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
     except KeyboardInterrupt:
-        exit_program()
+        return
     return ask
 def exit_program():
     os.system("clear")
     banner.main()
     print("\033[38;5;105m", "[+] Thanks visit again".title())
-    exit()
-
-
+    exit() 
+    
 def check_installed(name, run_arg):
     proc = subprocess.Popen(
-        [f"dpkg -s {name} 2>/dev/null"], stdout=subprocess.PIPE, shell=True
+        [f"dpkg -s {name} 2>> {os.path.dirname(__file__)}\\logs.txt "], stdout=subprocess.PIPE, shell=True
     )
     (there, notthere) = proc.communicate()
     if "install ok installed" not in there.decode():
         print(f"\n{colors.red}[+] Not Installed")
-        print(f"{colors.red}[+] It Is Not Installed In Your Kali{colors.reset}")
         try:
             install = input(
             f"{colors.blue}Do You Want To Install The Tool?(y/n):{colors.reset}"
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if install.lower() == "yes" or install.lower() == "y":
             os.system(f"apt install {name} -y")
+            path = check_path(name)
+            print(f"\nInstalled folder path : {path}")
             try:
                 download = input(
                 f"{colors.blue}Do You Want To Run The Tool?(y/n):{colors.reset}"
             )
             except KeyboardInterrupt:
-                exit_program()
+                return
             if (
                 download == "y"
                 or download == "Y"
                 or download == "Yes"
                 or download == "yes"
             ):
                 if run_arg == "kismet":
@@ -147,175 +211,185 @@
                     KURL = "http://localhost:2501"
                     threading.Thread(target=run_on_browser.main, args=(KURL,)).start()
                 elif run_arg == "fern-wifi-cracker":
                     threading.Thread(target=thread_run, args=(run_arg,)).start()
                     print("Fern-wifi-cracker Starting...")
                 else:
                     os.system(f"{run_arg}")
+                    Recommended_Tool.recommended(name=name)
     else:
         print(f"{colors.green}[+] Installed")
-        print(f"[+] It Is Installed In Your Kali{colors.reset}")
         try:
             download = input(
             f"{colors.blue}Do You Want To Run The Tool?(y/n):{colors.reset}"
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if download == "y" or download == "Y" or download == "Yes" or download == "yes":
             # os.system(f"{run_arg}")
             if run_arg == "kismet":
                 threading.Thread(target=thread_run, args=(run_arg,)).start()
                 print(
                     f"[+] {run_arg} is started at address: http://localhost:2501 (or the address of this system) for the Kismet UI"
                 )
                 KURL = "http://localhost:2501"
                 threading.Thread(target=run_on_browser.main, args=(KURL,)).start()
             elif run_arg == "fern-wifi-cracker":
                 threading.Thread(target=thread_run, args=(run_arg,)).start()
                 print("Fern-wifi-cracker Starting...")
             else:
-                os.system(f"{run_arg}")
+                #os.system(f"{run_arg}")
+                load_banner(name=name)
+                Recommended_Tool.recommended(name=name)
 
 
 def thread_run(command):
-    os.system(f"{command} > /dev/null 2>&1")
+    os.system(f"{command} >> {os.path.dirname(__file__)}\\logs.txt  2>&1")
 
 
 def pip_install(name, run_arg):
     proc = subprocess.Popen([f"which {name}"], stdout=subprocess.PIPE, shell=True)
     (there, nothere) = proc.communicate()
     if there:
         print(f"{colors.green}[+] Installed")
-        print(f"[+] It Is Installed In Your Kali{colors.reset}\n")
         try:
             download = input(
-            f"{colors.blue}\nDo You Want To Run The Tool?(y/n): {colors.reset} "
+            f"{colors.blue}Do You Want To Run The Tool?(y/n): {colors.reset} "
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if download.lower() == "y" or download.lower() == "yes":
             os.system(f"{run_arg}")
+            Recommended_Tool.recommended(name=name)
     else:
-        print(f"{colors.red}\n[+] It Is Not Installed In Your Kali{colors.reset}")
+        print(f"{colors.red}[+] Not Installed")
         try:
             download = input(
             f"{colors.blue}[+] Do You Want To Install It?(y/n):{colors.reset} "
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if download.lower() == "y" or download.lower() == "yes":
             os.system(f"pip install {name}")
+            path = check_path(name)
+            print(f"\nInstalled folder path : {path}")
             # os.system("go install github.com/projectdiscovery/katana/cmd/katana@latest")
             # os.system(f'sudo cp ~/go/bin/{name} /usr/bin')
             try:
                 download = input(
                 f"{colors.blue}\nDo You Want To Run The Tool?(y/n): {colors.reset}"
             )
             except KeyboardInterrupt:
-                exit_program()
+                return
             if download.lower() == "y" or download.lower() == "yes":
                 os.system(f"{run_arg}")
+                Recommended_Tool.recommended(name=name)
 
 
 def which_check(name, link, run_arg):
     proc = subprocess.Popen([f"which {name}"], stdout=subprocess.PIPE, shell=True)
     (there, nothere) = proc.communicate()
     if there:
         print(f"{colors.green}[+] Installed")
-        print(f"[+] It Is Installed In Your Kali{colors.reset}\n")
         try:
             download = input(
-            f"{colors.blue}\nDo You Want To Run The Tool?(y/n): {colors.reset} "
+            f"{colors.blue}Do You Want To Run The Tool?(y/n): {colors.reset} "
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if download.lower() == "y" or download.lower() == "yes":
             os.system(f"{run_arg}")
+            Recommended_Tool.recommended(name=name)
     else:
-        print(f"{colors.red}[+] It Is Not Installed In Your Kali{colors.reset}")
+        print(f"{colors.red}[+] Not Installed")
         try:
             download = input(
             f"{colors.blue}[+] Do You Want To Install It?(y/n):{colors.reset} "
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if download.lower() == "y" or download.lower() == "yes":
             os.system(f"go install {link}")
+            path = check_path(name)
+            print(f"\nInstalled folder path : {path}")
             # os.system("go install github.com/projectdiscovery/katana/cmd/katana@latest")
             os.system(f"sudo cp ~/go/bin/{name} /usr/bin")
             try:
                 download = input(
                 f"{colors.blue}\nDo You Want To Run The Tool?(y/n): {colors.reset}"
             )
             except KeyboardInterrupt:
-                exit_program()
+                return
             if download.lower() == "y" or download.lower() == "yes":
                 os.system(f"{run_arg}")
+                Recommended_Tool.recommended(name=name)
 
 
 def deb_install(name, command, link):
     proc = subprocess.Popen(
-        [f"dpkg -s {command} 2>/dev/null"], stdout=subprocess.PIPE, shell=True
+        [f"dpkg -s {command} 2>> {os.path.dirname(__file__)}\\logs.txt "], stdout=subprocess.PIPE, shell=True
     )
     (there, notthere) = proc.communicate()
     if "install ok installed" not in there.decode():
         print(f"{colors.red}[+] Not Installed")
-        print(f"{colors.red}[+] It Is Not Installed In Your Kali{colors.reset}")
         try:
             install = input(
             f"{colors.blue}Do You Want To Install The Tool?(y/n):{colors.reset}"
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if install.lower() == "yes" or install.lower() == "y":
             if not os.path.exists(f"Tools/{link.split('/')[-1]}"):
-                os.system(f"wget {link} -O Tools/{link.split('/')[-1]} 2>/dev/null")
-            os.system(f"dpkg -i Tools/{link.split('/')[-1]} >/dev/null")
+                os.system(f"wget {link} -O Tools/{link.split('/')[-1]} ")
+            os.system(f"dpkg -i Tools/{link.split('/')[-1]} ")
+            path = check_path(name)
+            print(f"\nInstalled folder path : {path}")
             try:
                 install = input(
-                f"{colors.blue}Do you want to run the tool?(y/n):{colors.reset}"
+                f"{colors.blue}Do you want to run the tool?(y/n):{colors.reset}"	
             )
             except KeyboardInterrupt:
-                exit_program()
+                return
             if install.lower() == "y" or install.lower == "yes":
                 if command == "nessus":
                     os.system("systemctl start nessusd.service")
                     print(f"{colors.green}[+] Service Started....")
                     print(
                         f"{colors.blue}[+] YOU CAN CHECK IT'S WRITE UPS FOR MORE INFO{colors.reset}"
                     )
                     try:
                         use = input(
                         f"{colors.blue}[+] Do You Want To Configure Nessus?(y/n):{colors.reset}"
                     )
                     except KeyboardInterrupt:
-                        exit_program()
+                        return
                     if use == "y" or use == "Y" or use == "Yes" or use == "yes":
                         run_on_browser.main("https://localhost:8834/")
                 else:
-                    os.system(f"{command} 2>/dev/null")
+                    os.system(f"{command} 2>> {os.path.dirname(__file__)}\\logs.txt")
+                    Recommended_Tool.recommended(name=name)
     else:
         print(f"{colors.green}[+] Installed")
-        print(f"[+] It Is Installed In Your Kali{colors.reset}")
         try:
             download = input(
             f"{colors.blue}Do You Want To Run The Tool?(y/n):{colors.reset}"
         )
         except KeyboardInterrupt:
-            exit_program()
+            return
         if download.lower() == "y" or download.lower() == "yes":
             if command == "nessus":
                 os.system("systemctl start nessusd.service")
                 print(f"{colors.green}[+] Service Started....")
                 print(
                     f"{colors.blue}[+] YOU CAN CHECK IT'S WRITE UPS FOR MORE INFO{colors.reset}"
                 )
                 try:
                     use = input(
                     f"{colors.blue}[+] Do You Want To Configure Nessus?(y/n):{colors.reset}"
                 )
                 except KeyboardInterrupt:
-                    exit_program()
+                    return
                 if use == "y" or use == "Y" or use == "Yes" or use == "yes":
                     run_on_browser.main("https://localhost:8834/")
             else:
-                os.system(f"{command} 2>/dev/null")
+                os.system(f"{command} 2>> {os.path.dirname(__file__)}\\logs.txt")
+                Recommended_Tool.recommended(name=name)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cyberonix-2.0.9/cyberonix/main/tools/writeup.py` & `cyberonix-3.0.0/cyberonix/main/tools/writeup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,21 @@
         os.system("clear")
         banner.main()
         banner.attack(name.title())
         #convert dict keys in list(type casting)
         key=list(writeup_dist.keys())
         key.append("Go Back")
         for i in range(len(key)):
-            print(colors.options,f"{i}) {key[i]}".title(),colors.reset)
+            
+            print(colors.options,f"{i+1}) {key[i]}".title(),colors.reset)
         try:
-            option = input(f"\n {colors.select}Select An Option -> {colors.reset} ")
+            option =input(f"\n {colors.select}Select An Option -> {colors.reset} ")
+            #option-=1
         except KeyboardInterrupt:
-            template.exit_program()
+            return
         #1-9=int kdsjfhgkjds=int X to type cast safely 
         try:
-            threading.Thread(target=run_on_browser.main, args=(writeup_dist[key[int(option)]],)).start()
+            threading.Thread(target=run_on_browser.main, args=(writeup_dist[key[(int(option))-1]],)).start()
             #a={"a":1,"b":2}
             # print(2)
         except:
             return
```

### Comparing `cyberonix-2.0.9/cyberonix.egg-info/SOURCES.txt` & `cyberonix-3.0.0/cyberonix.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 cyberonix/cyberonix.py
 cyberonix.egg-info/PKG-INFO
 cyberonix.egg-info/SOURCES.txt
 cyberonix.egg-info/dependency_links.txt
 cyberonix.egg-info/entry_points.txt
 cyberonix.egg-info/requires.txt
 cyberonix.egg-info/top_level.txt
-cyberonix/main/Cheat_sheet.py
+cyberonix/main/Bug_Bounty.py
 cyberonix/main/__init__.py
 cyberonix/main/arguments.py
-cyberonix/main/news.py
 cyberonix/main/tool.py
+cyberonix/main/tools/Anonymity.py
 cyberonix/main/tools/Authentication.py
 cyberonix/main/tools/Authorization.py
 cyberonix/main/tools/Configuration_Management.py
 cyberonix/main/tools/Cryptography.py
 cyberonix/main/tools/Exploitation_Tools.py
 cyberonix/main/tools/File_Upload.py
+cyberonix/main/tools/Framework.py
 cyberonix/main/tools/Password_Hacking.py
 cyberonix/main/tools/Pentesting_Bug_Bounty.py
 cyberonix/main/tools/PostExploitationAttacks.py
+cyberonix/main/tools/Recommended_Tool.py
 cyberonix/main/tools/RiskyFuncPayment.py
 cyberonix/main/tools/Secure_Transmission.py
 cyberonix/main/tools/Session_Management.py
 cyberonix/main/tools/Sniffing_and_Spoofing.py
 cyberonix/main/tools/Vulnerability_Analysis.py
 cyberonix/main/tools/WEB_Application_Analysis.py
 cyberonix/main/tools/Wireless_Hacking.py
 cyberonix/main/tools/__init__.py
 cyberonix/main/tools/banner.py
 cyberonix/main/tools/colors.py
 cyberonix/main/tools/data_validation.py
 cyberonix/main/tools/dos.py
+cyberonix/main/tools/forensic.py
 cyberonix/main/tools/html5.py
 cyberonix/main/tools/information_gathering.py
 cyberonix/main/tools/run_on_browser.py
 cyberonix/main/tools/template.py
 cyberonix/main/tools/waiting.py
 cyberonix/main/tools/writeup.py
```

### Comparing `cyberonix-2.0.9/setup.py` & `cyberonix-3.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from setuptools import setup,find_packages 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cyberonix",
-    version="2.0.9",
-    author="Metaxone",
-    author_email="admin@metaxonesolution.com",
+    version="3.0.0",
+    author="Defronix",
+    author_email="hello@defronix.com",
     description="Cyberonix is a complete resource hub for Cyber Security Community.",
-    url='https://github.com/TeamMetaxone/Cyberonix',
+    url='https://github.com/TeamDefronix/Cyberonix',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Security",
     ],
     install_requires=[
         "beautifulsoup4",
         "requests",
         "ipwhois",
         "dnspython==2.3.0",
         "selenium==4.7.2",
+        "netifaces",
     ],
     entry_points={
         'console_scripts': [
             'cyberonix = cyberonix.cyberonix:starting'
         ]
     }
 )
```

