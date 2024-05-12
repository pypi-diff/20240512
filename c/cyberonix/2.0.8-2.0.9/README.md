# Comparing `tmp/cyberonix-2.0.8.tar.gz` & `tmp/cyberonix-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberonix-2.0.8.tar", last modified: Wed Mar  8 18:31:44 2023, max compression
+gzip compressed data, was "cyberonix-2.0.9.tar", last modified: Thu Mar  9 16:27:11 2023, max compression
```

## Comparing `cyberonix-2.0.8.tar` & `cyberonix-2.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 18:31:44.117724 cyberonix-2.0.8/
--rw-r--r--   0 root         (0) root         (0)    16291 2023-03-08 18:31:44.117724 cyberonix-2.0.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    15521 2023-03-08 18:30:52.000000 cyberonix-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 18:31:44.109724 cyberonix-2.0.8/cyberonix/
--rwxr-xr-x   0 root         (0) root         (0)       44 2023-02-28 17:25:39.000000 cyberonix-2.0.8/cyberonix/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10466 2023-03-08 18:16:23.000000 cyberonix-2.0.8/cyberonix/cyberonix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 18:31:44.113724 cyberonix-2.0.8/cyberonix/main/
--rw-r--r--   0 root         (0) root         (0)     3404 2023-03-08 14:10:28.000000 cyberonix-2.0.8/cyberonix/main/Cheat_sheet.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-04 16:50:35.000000 cyberonix-2.0.8/cyberonix/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18118 2023-03-08 16:36:27.000000 cyberonix-2.0.8/cyberonix/main/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-03-08 14:09:58.000000 cyberonix-2.0.8/cyberonix/main/news.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-03-08 14:08:38.000000 cyberonix-2.0.8/cyberonix/main/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 18:31:44.117724 cyberonix-2.0.8/cyberonix/main/tools/
--rw-r--r--   0 root         (0) root         (0)     7895 2023-03-07 18:37:06.000000 cyberonix-2.0.8/cyberonix/main/tools/Authentication.py
--rw-r--r--   0 root         (0) root         (0)    22162 2023-03-07 18:37:18.000000 cyberonix-2.0.8/cyberonix/main/tools/Authorization.py
--rw-r--r--   0 root         (0) root         (0)    20829 2023-03-07 18:37:31.000000 cyberonix-2.0.8/cyberonix/main/tools/Configuration_Management.py
--rw-r--r--   0 root         (0) root         (0)     8774 2023-03-06 20:27:23.000000 cyberonix-2.0.8/cyberonix/main/tools/Cryptography.py
--rw-r--r--   0 root         (0) root         (0)    10616 2023-03-07 18:38:18.000000 cyberonix-2.0.8/cyberonix/main/tools/Exploitation_Tools.py
--rw-r--r--   0 root         (0) root         (0)     5421 2023-03-07 18:38:29.000000 cyberonix-2.0.8/cyberonix/main/tools/File_Upload.py
--rw-r--r--   0 root         (0) root         (0)    30574 2023-03-06 20:53:01.000000 cyberonix-2.0.8/cyberonix/main/tools/Password_Hacking.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-03-07 18:39:05.000000 cyberonix-2.0.8/cyberonix/main/tools/Pentesting_Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)    21205 2023-03-07 18:31:17.000000 cyberonix-2.0.8/cyberonix/main/tools/PostExploitationAttacks.py
--rw-r--r--   0 root         (0) root         (0)    16842 2023-03-07 18:39:27.000000 cyberonix-2.0.8/cyberonix/main/tools/RiskyFuncPayment.py
--rw-r--r--   0 root         (0) root         (0)     5236 2023-03-07 18:39:39.000000 cyberonix-2.0.8/cyberonix/main/tools/Secure_Transmission.py
--rw-r--r--   0 root         (0) root         (0)    18659 2023-03-07 18:39:51.000000 cyberonix-2.0.8/cyberonix/main/tools/Session_Management.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-03-07 18:40:00.000000 cyberonix-2.0.8/cyberonix/main/tools/Sniffing_and_Spoofing.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-03-07 18:40:13.000000 cyberonix-2.0.8/cyberonix/main/tools/Vulnerability_Analysis.py
--rw-r--r--   0 root         (0) root         (0)    12318 2023-03-07 18:40:24.000000 cyberonix-2.0.8/cyberonix/main/tools/WEB_Application_Analysis.py
--rw-r--r--   0 root         (0) root         (0)     6003 2023-03-07 19:21:36.000000 cyberonix-2.0.8/cyberonix/main/tools/Wireless_Hacking.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-04 16:50:35.000000 cyberonix-2.0.8/cyberonix/main/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-03-04 16:50:35.000000 cyberonix-2.0.8/cyberonix/main/tools/banner.py
--rw-r--r--   0 root         (0) root         (0)      207 2023-03-04 16:50:35.000000 cyberonix-2.0.8/cyberonix/main/tools/colors.py
--rw-r--r--   0 root         (0) root         (0)    31538 2023-03-07 18:37:56.000000 cyberonix-2.0.8/cyberonix/main/tools/data_validation.py
--rw-r--r--   0 root         (0) root         (0)     5628 2023-03-07 18:38:08.000000 cyberonix-2.0.8/cyberonix/main/tools/dos.py
--rw-r--r--   0 root         (0) root         (0)     5273 2023-03-07 19:22:11.000000 cyberonix-2.0.8/cyberonix/main/tools/html5.py
--rw-r--r--   0 root         (0) root         (0)    10451 2023-03-07 18:38:49.000000 cyberonix-2.0.8/cyberonix/main/tools/information_gathering.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-03-04 16:50:35.000000 cyberonix-2.0.8/cyberonix/main/tools/run_on_browser.py
--rw-r--r--   0 root         (0) root         (0)    13359 2023-03-06 21:13:59.000000 cyberonix-2.0.8/cyberonix/main/tools/template.py
--rw-r--r--   0 root         (0) root         (0)       78 2023-03-04 16:50:35.000000 cyberonix-2.0.8/cyberonix/main/tools/waiting.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-03-06 21:27:44.000000 cyberonix-2.0.8/cyberonix/main/tools/writeup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 18:31:44.109724 cyberonix-2.0.8/cyberonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16291 2023-03-08 18:31:44.000000 cyberonix-2.0.8/cyberonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-08 18:31:44.000000 cyberonix-2.0.8/cyberonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 18:31:44.000000 cyberonix-2.0.8/cyberonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-08 18:31:44.000000 cyberonix-2.0.8/cyberonix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-03-08 18:31:44.000000 cyberonix-2.0.8/cyberonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-08 18:31:44.000000 cyberonix-2.0.8/cyberonix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-08 18:31:44.117724 cyberonix-2.0.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1290 2023-03-08 18:31:34.000000 cyberonix-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.798401 cyberonix-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)    16291 2023-03-09 16:27:11.798401 cyberonix-2.0.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    15521 2023-03-08 18:30:52.000000 cyberonix-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.790401 cyberonix-2.0.9/cyberonix/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2023-02-28 17:25:39.000000 cyberonix-2.0.9/cyberonix/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10466 2023-03-08 18:16:23.000000 cyberonix-2.0.9/cyberonix/cyberonix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.794401 cyberonix-2.0.9/cyberonix/main/
+-rw-r--r--   0 root         (0) root         (0)     3354 2023-03-09 15:11:27.000000 cyberonix-2.0.9/cyberonix/main/Cheat_sheet.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18118 2023-03-08 16:36:27.000000 cyberonix-2.0.9/cyberonix/main/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2023-03-08 14:09:58.000000 cyberonix-2.0.9/cyberonix/main/news.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-03-08 14:08:38.000000 cyberonix-2.0.9/cyberonix/main/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.798401 cyberonix-2.0.9/cyberonix/main/tools/
+-rw-r--r--   0 root         (0) root         (0)     7895 2023-03-07 18:37:06.000000 cyberonix-2.0.9/cyberonix/main/tools/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)    22162 2023-03-09 15:37:30.000000 cyberonix-2.0.9/cyberonix/main/tools/Authorization.py
+-rw-r--r--   0 root         (0) root         (0)    20825 2023-03-09 15:38:06.000000 cyberonix-2.0.9/cyberonix/main/tools/Configuration_Management.py
+-rw-r--r--   0 root         (0) root         (0)     8774 2023-03-06 20:27:23.000000 cyberonix-2.0.9/cyberonix/main/tools/Cryptography.py
+-rw-r--r--   0 root         (0) root         (0)    10616 2023-03-07 18:38:18.000000 cyberonix-2.0.9/cyberonix/main/tools/Exploitation_Tools.py
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-03-07 18:38:29.000000 cyberonix-2.0.9/cyberonix/main/tools/File_Upload.py
+-rw-r--r--   0 root         (0) root         (0)    30502 2023-03-09 16:12:02.000000 cyberonix-2.0.9/cyberonix/main/tools/Password_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-03-07 18:39:05.000000 cyberonix-2.0.9/cyberonix/main/tools/Pentesting_Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)    21205 2023-03-07 18:31:17.000000 cyberonix-2.0.9/cyberonix/main/tools/PostExploitationAttacks.py
+-rw-r--r--   0 root         (0) root         (0)    16842 2023-03-07 18:39:27.000000 cyberonix-2.0.9/cyberonix/main/tools/RiskyFuncPayment.py
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-03-07 18:39:39.000000 cyberonix-2.0.9/cyberonix/main/tools/Secure_Transmission.py
+-rw-r--r--   0 root         (0) root         (0)    18659 2023-03-07 18:39:51.000000 cyberonix-2.0.9/cyberonix/main/tools/Session_Management.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-03-07 18:40:00.000000 cyberonix-2.0.9/cyberonix/main/tools/Sniffing_and_Spoofing.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-03-09 16:21:18.000000 cyberonix-2.0.9/cyberonix/main/tools/Vulnerability_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)    12318 2023-03-09 16:21:10.000000 cyberonix-2.0.9/cyberonix/main/tools/WEB_Application_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6003 2023-03-07 19:21:36.000000 cyberonix-2.0.9/cyberonix/main/tools/Wireless_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/banner.py
+-rw-r--r--   0 root         (0) root         (0)      207 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    31538 2023-03-09 15:47:26.000000 cyberonix-2.0.9/cyberonix/main/tools/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2023-03-07 18:38:08.000000 cyberonix-2.0.9/cyberonix/main/tools/dos.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2023-03-07 19:22:11.000000 cyberonix-2.0.9/cyberonix/main/tools/html5.py
+-rw-r--r--   0 root         (0) root         (0)    10451 2023-03-09 15:51:45.000000 cyberonix-2.0.9/cyberonix/main/tools/information_gathering.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/run_on_browser.py
+-rw-r--r--   0 root         (0) root         (0)    13411 2023-03-09 15:33:04.000000 cyberonix-2.0.9/cyberonix/main/tools/template.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-03-04 16:50:35.000000 cyberonix-2.0.9/cyberonix/main/tools/waiting.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-03-06 21:27:44.000000 cyberonix-2.0.9/cyberonix/main/tools/writeup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 16:27:11.790401 cyberonix-2.0.9/cyberonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16291 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-03-09 16:27:11.000000 cyberonix-2.0.9/cyberonix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 16:27:11.798401 cyberonix-2.0.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1274 2023-03-09 16:22:59.000000 cyberonix-2.0.9/setup.py
```

### Comparing `cyberonix-2.0.8/PKG-INFO` & `cyberonix-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 2.0.8
+Version: 2.0.9
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamMetaxone/Cyberonix
 Author: Metaxone
 Author-email: admin@metaxonesolution.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 2.0.8 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 2.0.9 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamMetaxone/Cyberonix Author: Metaxone Author-email:
 admin@metaxonesolution.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-2.0.8/README.md` & `cyberonix-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/cyberonix.py` & `cyberonix-2.0.9/cyberonix/cyberonix.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/Cheat_sheet.py` & `cyberonix-2.0.9/cyberonix/main/Cheat_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,14 @@
     if inspect.stack()[1].function != "main":
         if not main.called:
               main.called=True
               start()
     else:
         start()
 def start():  
-    if not main.called:
-        main.called=True
-
         os.system("clear")
         banner.main()
         banner.attack("Cheat Sheet")
         cheat({"Nmap cheatsheet" : "https://www.tutorialspoint.com/nmap-cheat-sheet","Maltego cheatsheet" : "https://static.maltego.com/cdn/case%20studies/building-integrations-for-maltego-cheat-sheet.pdf","Hping3 cheatsheet" : "https://cyberwar.nl/d/cheatsheets/hping3_cheatsheet_v1.0-ENG.pdf","Netdiscover cheatsheet" : "https://linuxcommandlibrary.com/man/netdiscover","Wafw00f cheatsheet" : "https://cheatsheet.haax.fr/web-pentest/applicative-scans/web_application_firewall/", "Metasploit-Framework cheatsheet" : "https://cdn.comparitech.com/wp-content/uploads/2019/06/Metasploit-Cheat-Sheet-1.webp", "Wireshark cheatsheet" : "https://www.stationx.net/wireshark-cheat-sheet/", "Bettercap cheatsheet" : "https://www.bettercap.org/usage/interactive/", "Tcpdump cheatsheet" : "https://cdn.comparitech.com/wp-content/uploads/2019/06/tcpdump-cheat-sheet-1.pdf", "Scapy cheatsheet" : "https://wiki.sans.blue/Tools/pdfs/ScapyCheatSheet_v0.2.pdf", "Responder cheatsheet" : "https://www.ivoidwarranties.tech/posts/pentesting-tuts/responder/cheatsheet/", "Airgeddon cheatsheet" : "https://liodeus.github.io/2020/10/29/OSWP-personal-cheatsheet.html#airgeddon", "Wpscan cheatsheet" : "https://linuxcommandlibrary.com/man/wpscan","Wapiti cheatsheet" : "https://wapiti.limsi.fr/manual.html","Legion cheatsheet" : "https://theory.stanford.edu/~aiken/LegionRetreat21/slides/Tools.pdf","Nikto cheatsheet" : "https://cdn.comparitech.com/wp-content/uploads/2019/07/NIkto-Cheat-Sheet.pdf", "Burp Suite cheatsheet" : "https://portswigger.net/burp/documentation/desktop","Owasp ZAP cheatsheet" : "https://www.zaproxy.org/docs/desktop/cmdline/","Nessus cheatsheet" : "https://limberduck.github.io/nessus-cheat-sheet/nessus-cheat-sheet.pdf","dirb cheatsheet" : "https://man7.org/linux/man-pages/man1/dir.1.html","skipfish cheatsheet" : "https://linux.die.net/man/1/skipfish","Nuclei cheatsheet" : "https://cheatsheet.haax.fr/web-pentest/tools/nuclei/", "Wifite cheatsheet" : "https://cheatography.com/socket23/cheat-sheets/wifite/", "Aircrack-ng cheatsheet" : "https://www.cyberfella.co.uk/rhel/aircrack-ng-suite.pdf"}, "cheatSheet")
 
 def exit_program():
         os.system("clear")
```

### Comparing `cyberonix-2.0.8/cyberonix/main/arguments.py` & `cyberonix-2.0.9/cyberonix/main/arguments.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/news.py` & `cyberonix-2.0.9/cyberonix/main/news.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tool.py` & `cyberonix-2.0.9/cyberonix/main/tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Authentication.py` & `cyberonix-2.0.9/cyberonix/main/tools/Authentication.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Authorization.py` & `cyberonix-2.0.9/cyberonix/main/tools/Authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,19 +194,19 @@
                         },
                     )
                 elif option == "9":
                     os.system("clear")
                     github = "The PenTesters Framework (PTF) is a Python script designed for Debian/Ubuntu/ArchLinux based distributions to create a similar and familiar distribution for Penetration Testing. PTF attempts to install all of your penetration testing tools (latest and greatest), compile them, build them, and make it so that you can install/update your distribution on any machine. Everything is organized in a fashion that is cohesive to the Penetration Testing Execution Standard (PTES) and eliminates a lot of things that are hardly used"
                     template.template(
                         "Penetration Testers Framework (PTF)",
-                        "chmod +x ptf && ./ptf",
+                        "./ptf",
                         github.strip(),
                         "no-writeups",
                         method="github",
-                        github_install="git clone https://github.com/trustedsec/ptf.git",
+                        github_install="git clone https://github.com/trustedsec/ptf.git && chmod +x ptf",
                         github_check="ptf",
                     )
                 else:
                     break
 
         elif option == "1":
             os.system("clear")
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Configuration_Management.py` & `cyberonix-2.0.9/cyberonix/main/tools/Configuration_Management.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                     " HTTPie",
                     " Metasploit",
                     "SecurityHeaders",
                     "SQLmap",
                     "TruffleHog",
                     "Gitleaks",
                     "SecretFinder",
+                    "Go Back"
                 ]
                 for i in range(len(list_attacks)):
                     print(
                         colors.options, f"{i}) {list_attacks[i]}".title(), colors.reset
                     )
                 try:
                     option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
@@ -140,15 +141,15 @@
                         },
                     )
                 elif option == "8":
                     print("\n[+] HTTPie")
                     os.system("clear")
                     github = "HTTPie is a command-line tool used to send HTTP requests and receive responses from a server. It is designed to be user-friendly and intuitive, with a simple syntax and easy-to-read output. HTTPie can be used to test and debug APIs, as well as interact with web services and applications. It supports various HTTP methods, data formats, and authentication methods, and can be customized with various options and configurations to suit specific use cases."
                     template.template(
-                        "HTTPie", "httpie -h", github.strip(), "no-writeups"
+                        "httpie", "httpie -h", github.strip(), "no-writeups"
                     )
                 elif option == "9":
                     print("\n[+] Metasploit")
                     os.system("clear")
                     github = "The Metasploit Framework is an open-source tool for developing and executing exploit code against a remote target machine. It can be used to test the security of a computer system by finding and exploiting vulnerabilities. The framework includes a large collection of exploit modules, as well as various tools for payload generation, post-exploitation, and more. It can be used by security professionals for penetration testing, as well as by attackers for malicious purposes."
                     template.template(
                         "metasploit-framework",
@@ -158,22 +159,22 @@
                     )
                 elif option == "10":
                     print("\n[+] SecurityHeaders")
                     os.system("clear")
                     github = """SecurityHeaders is a configuration management tool that focuses on securing web applications by helping administrators configure appropriate HTTP security headers. HTTP security headers are additional response headers that can be sent by a web server to a client's browser to instruct it to follow certain security-related behaviors. For example, the "Content-Security-Policy" header can be used to restrict the types of content that a web page can load, helping to prevent cross-site scripting (XSS) attacks."""
                     template.template(
                         "securityheaders",
-                        "pip install -r requirements.txt > /dev/null 2>&1 && python3 securityheaders.py -h",
+                        "python3 securityheaders.py -h",
                         github.strip(),
                         {
                             "Website": "https://securityheaders.com/",
                             "Securityheaders usage": "https://github.com/koenbuyens/securityheaders",
                         },
                         method="github",
-                        github_install="git clone https://github.com/koenbuyens/securityheaders.git",
+                        github_install="git clone https://github.com/koenbuyens/securityheaders.git && pip install -r requirements.txt",
                         github_check="securityheaders",
                     )
                 elif option == "11":
                     print("\n[+] Sqlmap")
                     os.system("clear")
                     github = github_getting_text("https://sqlmap.org/", "p", 0)
                     template.template(
@@ -207,21 +208,21 @@
                     )
                 elif option == "14":
                     print("\n[+] SecretFinder")
                     os.system("clear")
                     github = "SecretFinder is an open-source tool used to scan web applications for sensitive information and secrets, such as API keys, passwords, and tokens. It is designed to identify potential security vulnerabilities that could be exploited by attackers, and can be used in bug bounty hunting and vulnerability assessments. SecretFinder uses a combination of static analysis and dynamic analysis techniques to discover secrets, and can be customized with various options and configurations to suit specific use cases. It generates a report of its findings, which can be used to remediate identified vulnerabilities and improve the overall security of the web application. SecretFinder is a powerful and efficient tool that can help security professionals and developers identify potential security risks in their web applications."
                     template.template(
                         "secretFinder",
-                        "pip install -r requirements.txt > /dev/null 2>&1 && python3 SecretFinder.py -h",
+                        "python3 SecretFinder.py -h",
                         github.strip(),
                         {
                             "SecretFinder demo": "https://www.briskinfosec.com/tooloftheday/toolofthedaydetail/SecretFinder",
                         },
                         method="github",
-                        github_install="git clone https://github.com/m4ll0k/SecretFinder.git",
+                        github_install="git clone https://github.com/m4ll0k/SecretFinder.git && pip install -r requirements.txt",
                         github_check="SecretFinder",
                     )
                 else:
                     break
 
         elif option == "1":
             print("\n[+] Write-UPS")
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Cryptography.py` & `cyberonix-2.0.9/cyberonix/main/tools/Cryptography.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Exploitation_Tools.py` & `cyberonix-2.0.9/cyberonix/main/tools/Exploitation_Tools.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/File_Upload.py` & `cyberonix-2.0.9/cyberonix/main/tools/File_Upload.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Password_Hacking.py` & `cyberonix-2.0.9/cyberonix/main/tools/Password_Hacking.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,25 @@
                     print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     template.exit_program()
                 if ask == "0":
                     github = "Hashcat is an open-source password cracking tool that can perform dictionary, brute force and combination attacks, it uses the power of GPUs to accelerate the cracking process, supports a wide variety of hashing algorithms and it can run on Windows, Linux and macOS. It's widely used for password recovery, security testing and penetration testing."
-                    template.template("Hashcat", "hashcat -h", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/","How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
+                    template.template("hashcat", "hashcat -h", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/","How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
                 elif ask == "1":
                     github = "John the Ripper is a free and open-source password cracking software tool. It can be run on a variety of operating systems, including Windows, macOS, and Linux. It uses a combination of wordlists and rules to try and guess the password for a given hash or file, and can support a variety of different hash types, including those used for Unix and Windows passwords. John the Ripper is commonly used by security professionals and system administrators to audit the security of their systems and detect weak or easily guessable passwords."
-                    template.template("John The Ripper", "john", github.strip(), {"Open-wall John": "https://www.openwall.com/john/","Password Cracking With John The Ripper": "https://www.section.io/engineering-education/password-cracking-with-john-the-ripper/","Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
+                    template.template("john", "john", github.strip(), {"Open-wall John": "https://www.openwall.com/john/","Password Cracking With John The Ripper": "https://www.section.io/engineering-education/password-cracking-with-john-the-ripper/","Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
                 elif ask == "2":
                     github = "Hydra is a password cracking tool that performs brute-force and dictionary attacks on network protocols such as Telnet, FTP, HTTP, and SSH. It is used to test the security of remote systems by attempting to log in with multiple username and password combinations. It can run on multiple operating systems and is commonly used by security professionals and penetration testers."
-                    template.template("Hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool","Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
+                    template.template("hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool","Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
 
                 elif ask == "3":
                     github = "Johnny is a GUI (Graphical User Interface) for the John the Ripper password cracking tool. It provides a user-friendly interface for managing and running John the Ripper's cracking tasks, rather than using command line commands. It is designed to make the process of cracking passwords more efficient and user-friendly. It can run on Windows, Linux and MacOS."
-                    template.template("Johnny", "johnny", github.strip(), {"How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca","Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
+                    template.template("johnny", "johnny", github.strip(), {"How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca","Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
                 elif ask == "4":
                     github = "CrackStation is a website that provides a service to check if a given password has been previously compromised in a data breach. It uses a precomputed hash database of billions of real-world passwords to check if a given password is in the list. It's designed to help users and organizations check the security of their passwords and identify weak or easily guessable passwords that should be changed."
                     template.template("CrackStation", "https://crackstation.net/",github.strip(), {"Salted Password Hashing - Doing it Right": "https://crackstation.net/hashing-security.htm","CrackStation's Password Cracking Dictionary": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm","Wordlist Download": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm"},method="browser")
                 elif ask == "5":
                     github = "Cyber Chef is a web-based tool developed by the US Cyber Command, that allows users to perform digital forensic and incident response tasks, such as data carving, decoding, and exfiltration using pre-built 'recipes' or custom workflows using a visual, drag-and-drop interface. It can process various types of data and run on different platforms. It is generally used by security professionals to quickly process large amounts of data, extract useful information and identify potential malicious activity."
                     template.template("CyberChef", "https://gchq.github.io/CyberChef/", github.strip(), {"CyberChef - A must have security tool": "https://www.youtube.com/watch?v=rT_CjwKN380","CyberChef – Data decoding made easy": "https://www.csnp.org/post/cyberchef-data-decoding-made-easy"},method="browser")
                 else:
@@ -58,30 +58,30 @@
                     print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     template.exit_program()
                 if ask == "0":
                     github = "Hashcat is an open-source password cracking tool that can perform dictionary, brute force and combination attacks, it uses the power of GPUs to accelerate the cracking process, supports a wide variety of hashing algorithms and it can run on Windows, Linux and macOS. It's widely used for password recovery, security testing and penetration testing."
-                    template.template("Hashcat", "hashcat", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/","How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
+                    template.template("hashcat", "hashcat", github.strip(), {"Hashcat tutorial for beginners": "https://resources.infosecinstitute.com/topic/hashcat-tutorial-beginners/","How to Crack Passwords Using Hashcat Tool?": "https://geekflare.com/password-cracking-with-hashcat/"})
                 elif ask == "1":
                     github = "John the Ripper is a free and open-source password cracking software tool. It can be run on a variety of operating systems, including Windows, macOS, and Linux. It uses a combination of wordlists and rules to try and guess the password for a given hash or file, and can support a variety of different hash types, including those used for Unix and Windows passwords. John the Ripper is commonly used by security professionals and system administrators to audit the security of their systems and detect weak or easily guessable passwords."
-                    template.template("John The Ripper", "john", github.strip(), {"Open-wall John": "https://www.openwall.com/john/","Password Cracking With John The Ripper": "https://www.section.io/engineering-education/password-cracking-with-john-the-ripper/","Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
+                    template.template("john", "john", github.strip(), {"Open-wall John": "https://www.openwall.com/john/","Password Cracking With John The Ripper": "https://www.section.io/engineering-education/password-cracking-with-john-the-ripper/","Tips and Tutorials of John": "https://www.varonis.com/blog/john-the-ripper"})
                 elif ask == "2":
                     github = "Hydra is a password cracking tool that performs brute-force and dictionary attacks on network protocols such as Telnet, FTP, HTTP, and SSH. It is used to test the security of remote systems by attempting to log in with multiple username and password combinations. It can run on multiple operating systems and is commonly used by security professionals and penetration testers."
-                    template.template("Hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool","Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
+                    template.template("hydra", "hydra", github.strip(), {"How to use the hydra for password cracking": "https://www.techtarget.com/searchsecurity/tutorial/How-to-use-the-Hydra-password-cracking-tool","Hydra Tool For Brute- force attack": "https://systemweakness.com/hydra-tool-for-brute-force-attack-72653db7abe9?gi=efe05fea34af"})
                 elif ask == "3":
                     github = "Medusa is a password cracking tool that is used to perform brute-force attacks on login credentials. It is a command-line tool that can be used to test the security of login systems by trying a large number of possible username and password combinations. Medusa is capable of testing various protocols such as HTTP, HTTPS, FTP, SSH, and more. It is mainly used by penetration testers and security professionals to identify weak passwords in a network and help improve the overall security of an organization. However, like other password cracking tools, it can also be used by malicious actors for illegal activities."
-                    template.template("Medusa", "medusa", github.strip(), {"A Detailed Guide on Medusa": "https://www.hackingarticles.in/a-detailed-guide-on-medusa/","Bruteforce Password Cracking with Medusa": "https://www.yeahhub.com/bruteforce-password-cracking-medusa-kali-linux/"})
+                    template.template("medusa", "medusa", github.strip(), {"A Detailed Guide on Medusa": "https://www.hackingarticles.in/a-detailed-guide-on-medusa/","Bruteforce Password Cracking with Medusa": "https://www.yeahhub.com/bruteforce-password-cracking-medusa-kali-linux/"})
                 elif ask == "4":
                     github = "Ncrack is a network authentication cracking tool. It is designed to perform efficient brute-force and dictionary attacks against a variety of different network protocols, including Telnet, FTP, HTTP, HTTPS, SMB, and RDP. It can be used to test the security of networks and remote systems by attempting to log in with a large number of different username and password combinations.Ncrack is similar to other password cracking tools such as John the Ripper and Hydra, but it is specifically designed to work with network protocols. It can run on Windows, Linux, and macOS and is often used by security professionals and penetration testers to test the security of networks and web applications"
                     template.template("ncrack", "ncrack", github.strip(), {"Comprehensive Guide on Ncrack – A Brute Forcing Tool": "https://www.hackingarticles.in/comprehensive-guide-on-ncrack-a-brute-forcing-tool/","Ncrack – Network Authentication and Password Cracking Tool": "https://secnhack.in/ncrack-network-authentication-and-password-cracking-tool/"})
                 elif ask == "5":
                     github = "Johnny is a GUI (Graphical User Interface) for the John the Ripper password cracking tool. It provides a user-friendly interface for managing and running John the Ripper's cracking tasks, rather than using command line commands. It is designed to make the process of cracking passwords more efficient and user-friendly. It can run on Windows, Linux and MacOS."
-                    template.template("Johnny", "johnny", github.strip(), {"How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca","Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
+                    template.template("johnny", "johnny", github.strip(), {"How to use the Johnny GUI for password cracking": "https://andregodinho1.medium.com/how-to-use-johnny-an-advanced-password-cracker-recovery-gui-soft-61736c8cb1ca","Password cracking with Johnny": "https://www.youtube.com/watch?v=Wrg6XZu6Luw"})
                 elif ask == "6":
                     github = "CrackStation is a website that provides a service to check if a given password has been previously compromised in a data breach. It uses a precomputed hash database of billions of real-world passwords to check if a given password is in the list. It's designed to help users and organizations check the security of their passwords and identify weak or easily guessable passwords that should be changed."
                     template.template("CrackStation", "https://crackstation.net/",github.strip(), {"Salted Password Hashing - Doing it Right": "https://crackstation.net/hashing-security.htm","CrackStation's Password Cracking Dictionary": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm","Wordlist Download": "https://crackstation.net/crackstation-wordlist-password-cracking-dictionary.htm"},method="browser")
                 elif ask == "7":
                     github = "Cyber Chef is a web-based tool developed by the US Cyber Command, that allows users to perform digital forensic and incident response tasks, such as data carving, decoding, and exfiltration using pre-built 'recipes' or custom workflows using a visual, drag-and-drop interface. It can process various types of data and run on different platforms. It is generally used by security professionals to quickly process large amounts of data, extract useful information and identify potential malicious activity."
                     template.template("CyberChef", "https://gchq.github.io/CyberChef/", github.strip(), {"CyberChef - A must have security tool": "https://www.youtube.com/watch?v=rT_CjwKN380","CyberChef – Data decoding made easy": "https://www.csnp.org/post/cyberchef-data-decoding-made-easy"},method="browser")
                 else:
@@ -120,18 +120,18 @@
                     print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     template.exit_program()
                 if ask == "0":
                     github = "Crunch is a wordlist generator tool that can be used to generate a list of all possible combinations of characters for a given set of parameters. It can be used to generate a wordlist for password cracking, testing password policies and other security related tasks. It is a simple command line tool that can be used to generate wordlists with different character sets, lengths, patterns and other parameters. It can also use a standard or a custom character set to generate the wordlist and can be used to generate a wordlist of any size."
-                    template.template("Crunch", "crunch", github.strip(), {"Create Wordlist Using Crunch": "https://null-byte.wonderhowto.com/how-to/tutorial-create-wordlists-with-crunch-0165931/","Crunch Password List Generation": "https://www.hackingtutorials.org/general-tutorials/crunch-password-list-generation/","Complete Guide on Crunch Tool": "https://secnhack.in/complete-guide-on-crunch-tool/"})
+                    template.template("crunch", "crunch", github.strip(), {"Create Wordlist Using Crunch": "https://null-byte.wonderhowto.com/how-to/tutorial-create-wordlists-with-crunch-0165931/","Crunch Password List Generation": "https://www.hackingtutorials.org/general-tutorials/crunch-password-list-generation/","Complete Guide on Crunch Tool": "https://secnhack.in/complete-guide-on-crunch-tool/"})
                 elif ask == "1":
                     github = "CUPP (Common User Passwords Profiler) is a tool that generates a custom wordlist based on personal information about a target. It can be used to generate a wordlist based on information such as the target's name, birthdate, address, and other personal details. CUPP can be used to perform a dictionary attack on a password hash, trying all the generated words as passwords, in order to crack the password. CUPP is written in Python and it's open source."
-                    template.template("Cupp", "cupp", github.strip(), {"Cybrary CUPP Tool": "https://www.cybrary.it/blog/0p3n/using-cupp-tool-generate-powerful-password-lists/","How To Create Password List Using CUPP Tool": "https://programmercave0.github.io/blog/2019/10/10/How-to-create-Password-list-using-CUPP-tool-on-ubuntu","CUPP Tool Password Generator)": "https://www.geeksforgeeks.org/cupp-common-user-passwords-profiler/"})
+                    template.template("cupp", "cupp", github.strip(), {"Cybrary CUPP Tool": "https://www.cybrary.it/blog/0p3n/using-cupp-tool-generate-powerful-password-lists/","How To Create Password List Using CUPP Tool": "https://programmercave0.github.io/blog/2019/10/10/How-to-create-Password-list-using-CUPP-tool-on-ubuntu","CUPP Tool Password Generator)": "https://www.geeksforgeeks.org/cupp-common-user-passwords-profiler/"})
                 elif ask == "2":
                     github = "Bopscrk (Before Outset Password Cracking is a tool to generate smart and powerful wordlists for targeted attacks. It is part of Black Arch Linux for as long as we can remember. It introduces personal information related to the target and combines every word and transforms it into possible passwords. It also contains a lyric pass module which allows it to search lyrics related to the favourite artist of the target and then include them into the wordlists."
                     template.template("bopscrk", "bopscrk -i", github.strip(), {"Create Wordlist Like Pro by Zsecurity": "https://zsecurity.org/create-password-wordlists-like-a-pro-2/","Wordlist For Pentester": "https://www.hackingarticles.in/wordlists-for-pentester/"},method="pip")
                 else:
                     break
 
         elif option == "4":
@@ -149,27 +149,27 @@
                     template.exit_program()
                 if ask == "0":
                     github = "The Social Engineering Toolkit (SET) is an open-source penetration testing framework that is used to perform various social engineering attacks. It is designed to be used for the purposes of penetration testing and vulnerability assessments, and it can be used to perform attacks such as phishing, website attacks, and other forms of social engineering. The toolkit is written in Python and is available for Windows, Linux, and Mac OS X. It can be used to test the security of an organization's employees and to evaluate the effectiveness of security awareness training programs."
                     template.template("set", "setoolkit", github.strip(), {"Phishing using SET": "https://www.golinuxcloud.com/social-engineering-toolkit-phishing/","Phishing using SET by Hengky Sanjaya": "https://medium.com/hengky-sanjaya-blog/social-engineering-toolkit-set-23be8b66aa18"})
 
                 elif ask == "1":
                     github = "HiddenEye is a modern phishing tool with advanced functionality. It is written in Python and can be run on Windows, Linux, and Mac OS X. It allows you to perform various phishing attacks."
-                    template.template("HiddenEye","pip install -r requirements.txt >/dev/null 2>&1 && python HiddenEye.py",github.strip(), {"HiddenEye by JohnJHacking": "https://johnjhacking.com/blog/hiddeneye/", "HiddenEye by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/", "HiddenEye by Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"},method="github",github_install="git clone https://github.com/Morsmalleo/HiddenEye",github_check="HiddenEye")
+                    template.template("HiddenEye","python HiddenEye.py",github.strip(), {"HiddenEye by JohnJHacking": "https://johnjhacking.com/blog/hiddeneye/", "HiddenEye by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/", "HiddenEye by Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"},method="github",github_install="git clone https://github.com/Morsmalleo/HiddenEye && pip install -r requirements.txt",github_check="HiddenEye")
                 elif ask == "2":
                     github = "It is a Phishing tool that has latest and updated login pages, Mask URL support, Beginners Friendly, Multiple tunneling options"
-                    template.template("r3bu5", "chmod +x r3bu5.sh && ./r3bu5.sh", github.strip(), {"Github Repo of r3bu5": " https://github.com/k46-db0y/r3bu5"}, method="github",github_install="git clone https://github.com/k46-db0y/r3bu5",github_check="r3bu5")
+                    template.template("r3bu5", "./r3bu5.sh", github.strip(), {"Github Repo of r3bu5": " https://github.com/k46-db0y/r3bu5"}, method="github",github_install="git clone https://github.com/k46-db0y/r3bu5 && chmod +x r3bu5.sh",github_check="r3bu5")
                 elif ask == "3":
                     github = "Zphisher is an open-source phishing tool that automates the process of creating and deploying phishing pages. It allows users to easily create phishing pages for various popular websites, such as Google, Facebook, and LinkedIn, and can be used to perform phishing attacks on targeted individuals or organizations. It can also be used to test the security awareness of an organization's employees. Zphisher is written in Shell Script and it's available for Linux and Termux."
                     template.template("zphisher", "chmod +x zphisher.sh && ./zphisher.sh", github.strip(), {"Zphisher phishing tool by reconshell": "https://reconshell.com/zphisher-an-automated-phishing-tool/","Zphisher phishing tool by vulners": "https://vulners.com/kitploit/KITPLOIT:1994086289094110137"},method="github", github_install="git clone https://github.com/htr-tech/zphisher",github_check="zphisher")
                 elif ask == "4":
                     github = "Shellphish is a tool used for phishing attacks, specifically for the purpose of stealing login credentials. It automates the process of creating phishing pages for various websites, such as social media platforms and email services. The tool is typically used by ethical hackers and penetration testers to test the security of a system, but can also be used by malicious actors for illegal activities."
-                    template.template("ShellPhish", "chmod +x shellphish.sh && ./shellphish.sh", github.strip(),{"Shellphish Tool writeup.writeup": "https://www.kalilinux.in/2019/04/shellphish-phishing-page-creator.html"},method="github",github_install="git clone https://github.com/AbirHasan2005/ShellPhish",github_check="ShellPhish")
+                    template.template("ShellPhish", "./shellphish.sh", github.strip(),{"Shellphish Tool writeup.writeup": "https://www.kalilinux.in/2019/04/shellphish-phishing-page-creator.html"},method="github",github_install="git clone https://github.com/AbirHasan2005/ShellPhish && chmod +x shellphish.sh",github_check="ShellPhish")
                 elif ask == "5":
                     github = "Gophish is an open-source tool for conducting phishing campaigns. It allows users to create, send and track phishing campaigns, including the ability to create custom phishing templates and landing pages, as well as track user interactions with the phishing emails. Gophish is often used by penetration testers and security professionals to test the security of an organization's email system and educate employees on how to spot and avoid phishing attempts. However, like other phishing tools, it can also be used by malicious actors for illegal activities."
-                    template.template("Gophish","unzip gophish-v0.12.1-linux-64bit.zip > /dev/null 2>&1 && chmod +x gophish && ./gophish &",github.strip(), {"Create phishing campaign gophish": "https://www.golinuxcloud.com/create-phishing-campaign-gophish/","Phishing attack using gophish": "https://www.techrepublic.com/article/how-to-run-a-phishing-attack-simulation-with-gophish/"},method="github",github_install="mkdir Gophish && wget https://github.com/gophish/gophish/releases/download/v0.12.1/gophish-v0.12.1-linux-64bit.zip",github_check="Gophish")
+                    template.template("Gophish","./gophish &",github.strip(), {"Create phishing campaign gophish": "https://www.golinuxcloud.com/create-phishing-campaign-gophish/","Phishing attack using gophish": "https://www.techrepublic.com/article/how-to-run-a-phishing-attack-simulation-with-gophish/"},method="github",github_install="mkdir Gophish && wget https://github.com/gophish/gophish/releases/download/v0.12.1/gophish-v0.12.1-linux-64bit.zip && unzip gophish-v0.12.1-linux-64bit.zip && chmod +x gophish",github_check="Gophish")
                 else:
                     break
 
         elif option == "5":
             while True:
                 os.system("clear")
                 banner.main()
@@ -180,15 +180,15 @@
                     print(colors.options, f"{i}) {list_root_attacks[i]}".title(), colors.reset)
                 try:
                     ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
                 except KeyboardInterrupt:
                     template.exit_program()
                 if ask == "0":
                     github = "zLogger is a Remote persistent keylogger it is written in python, and can generate executables that run on Windows and Linux, once executed on a system it’ll run the background, record every key-strike and report to the email specified when the keylogger was generated."
-                    template.template("ZLogger","python zlogger.py -h" ,github.strip(), {"ZLogger Tool in Medium": "https://medium.com/purple-team/make-a-keylogger-using-the-zlogger-tool-9945bc87922","ZLogger by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/","ZLogger in Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"},method="github", github_install="git clone https://github.com/z00z/ZLogger && pip install pynput > /dev/null 2>&1 && chmod +x *",github_check="ZLogger")
+                    template.template("ZLogger","python zlogger.py -h" ,github.strip(), {"ZLogger Tool in Medium": "https://medium.com/purple-team/make-a-keylogger-using-the-zlogger-tool-9945bc87922","ZLogger by Zsecurity": "https://zsecurity.org/hiddeneye-with-ngrok-all-in-one-phishing-solution/","ZLogger in Null-Byte": "https://null-byte.wonderhowto.com/forum/phish-with-hiddeneye-tool-with-advanced-feature-0323221/"},method="github", github_install="git clone https://github.com/z00z/ZLogger && pip install pynput && chmod +x *",github_check="ZLogger")
                 else:
                     break
         else:
             return
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Pentesting_Bug_Bounty.py` & `cyberonix-2.0.9/cyberonix/main/tools/Pentesting_Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/PostExploitationAttacks.py` & `cyberonix-2.0.9/cyberonix/main/tools/PostExploitationAttacks.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/RiskyFuncPayment.py` & `cyberonix-2.0.9/cyberonix/main/tools/RiskyFuncPayment.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Secure_Transmission.py` & `cyberonix-2.0.9/cyberonix/main/tools/Secure_Transmission.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Session_Management.py` & `cyberonix-2.0.9/cyberonix/main/tools/Session_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Sniffing_and_Spoofing.py` & `cyberonix-2.0.9/cyberonix/main/tools/Sniffing_and_Spoofing.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Vulnerability_Analysis.py` & `cyberonix-2.0.9/cyberonix/main/tools/Vulnerability_Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
             option = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
         except KeyboardInterrupt:
             template.exit_program()
         if option=="0":
             print("\n[+] Wpscan")
             os.system("clear")
             github = "WPScan is a security scanner designed for testing the security of websites built using WordPress. WPScan was developed using the Ruby programming language and then released in the first version in 2019. The WPScan security scanner is primarily intended to be used by WordPress administrators and security teams to assess the security status of their WordPress installations. It is used to scan WordPress websites for known vulnerabilities both in WordPress and commonly used WordPress plugins and themes. The code base for WPScan is licensed under GPLv3"
-            template.template("Wpscan","wpscan -h",github.strip(),{'WPScan Intro: How to Scan for WordPress Vulnerabilities':'https://blog.sucuri.net/2021/05/wpscan-how-to-scan-for-wordpress-vulnerabilities.html/','WPScan:WordPress Pentesting Framework':'https://www.hackingarticles.in/wpscanwordpress-pentesting-framework/','How To Use WPScan to Test for Vulnerable Plugins and Themes in Wordpress':"https://www.digitalocean.com/community/tutorials/how-to-use-wpscan-to-test-for-vulnerable-plugins-and-themes-in-wordpress","How to Use wpscan tool in Kali Linux":"https://www.geeksforgeeks.org/how-to-use-wpscan-tool-in-kali-linux/","WPScan Usage Example [Enumeration + Exploit]":"https://www.cyberpunk.rs/wpscan-usage-example"})
+            template.template("wpscan","wpscan -h",github.strip(),{'WPScan Intro: How to Scan for WordPress Vulnerabilities':'https://blog.sucuri.net/2021/05/wpscan-how-to-scan-for-wordpress-vulnerabilities.html/','WPScan:WordPress Pentesting Framework':'https://www.hackingarticles.in/wpscanwordpress-pentesting-framework/','How To Use WPScan to Test for Vulnerable Plugins and Themes in Wordpress':"https://www.digitalocean.com/community/tutorials/how-to-use-wpscan-to-test-for-vulnerable-plugins-and-themes-in-wordpress","How to Use wpscan tool in Kali Linux":"https://www.geeksforgeeks.org/how-to-use-wpscan-tool-in-kali-linux/","WPScan Usage Example [Enumeration + Exploit]":"https://www.cyberpunk.rs/wpscan-usage-example"})
         elif option=="1":
             print("\n[+] Wireshark")
             os.system("clear")
             github=github_getting_text("https://github.com/wireshark/wireshark",'p[dir="auto"]',0)
-            template.template("Wireshark","wireshark",github.strip(),{'How To Install & Use Wireshark On Kali Linux':'https://infosecscout.com/wireshark-on-kali-linux/','Wireshark Tool Documentation':'https://www.kali.org/tools/wireshark/','Wireshark Training':'https://www.wireshark.org/docs/','Wireshark – Resources':'https://blog.inf.ed.ac.uk/atate/2023/01/14/wireshark-resources/','Kerberos Wireshark Captures: A Windows Login Example':'https://medium.com/@robert.broeckelmann/kerberos-wireshark-captures-a-windows-login-example-151fabf3375a','Wireshark – Packet Capturing and Analyzing':'https://www.geeksforgeeks.org/wireshark-packet-capturing-and-analyzing/','https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/':'https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/'})
+            template.template("wireshark","wireshark",github.strip(),{'How To Install & Use Wireshark On Kali Linux':'https://infosecscout.com/wireshark-on-kali-linux/','Wireshark Tool Documentation':'https://www.kali.org/tools/wireshark/','Wireshark Training':'https://www.wireshark.org/docs/','Wireshark – Resources':'https://blog.inf.ed.ac.uk/atate/2023/01/14/wireshark-resources/','Kerberos Wireshark Captures: A Windows Login Example':'https://medium.com/@robert.broeckelmann/kerberos-wireshark-captures-a-windows-login-example-151fabf3375a','Wireshark – Packet Capturing and Analyzing':'https://www.geeksforgeeks.org/wireshark-packet-capturing-and-analyzing/','https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/':'https://unit42.paloaltonetworks.com/wireshark-tutorial-decrypting-https-traffic/'})
         elif option=="2":
             print("\n[+] Wapiti")
             os.system("clear")
             github=github_getting_text("https://github.com/wapiti-scanner/wapiti",'p[dir="auto"]',6)
             template.template("wapiti","wapiti",github.strip(),{"wapiti free web application vulnerability scanner":"https://pentestit.medium.com/wapiti-free-web-application-vulnerability-scanner-ce7712adf644","Official docs":"https://github.com/wapiti-scanner/wapiti","wapiti tutorial":"https://www.kalilinux.in/2021/01/wapiti-tutorial.html","complete guide to using wapiti web vulnerability scanner to keep your web applications websites secure":"https://linuxsecurity.com/features/complete-guide-to-using-wapiti-web-vulnerability-scanner-to-keep-your-web-applications-websites-secure"})
         elif option=="3":
             print("\n[+] Nmap")
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/WEB_Application_Analysis.py` & `cyberonix-2.0.9/cyberonix/main/tools/WEB_Application_Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             os.system("clear")
             github=github_getting_text("https://github.com/wapiti-scanner/wapiti",'p[dir="auto"]',6)
             template.template("wapiti","wapiti",github.strip(),{"wapiti free web application vulnerability scanner":"https://pentestit.medium.com/wapiti-free-web-application-vulnerability-scanner-ce7712adf644","Official docs":"https://github.com/wapiti-scanner/wapiti","wapiti tutorial":"https://www.kalilinux.in/2021/01/wapiti-tutorial.html","complete guide to using wapiti web vulnerability scanner to keep your web applications websites secure":"https://linuxsecurity.com/features/complete-guide-to-using-wapiti-web-vulnerability-scanner-to-keep-your-web-applications-websites-secure"})
         elif option=="4":
             print(f"\n[+] Nessus")
             os.system("clear")
             github=github_getting_text("https://www.techtarget.com/searchnetworking/definition/Nessus",'section[id="content-body"]',0)
-            template.template("Nessus","nessus",github.strip(),{"How To: Run Your First Vulnerability Scan with Nessus":"https://www.tenable.com/blog/how-to-run-your-first-vulnerability-scan-with-nessus","A brief introduction to the Nessus vulnerability scanner":"https://resources.infosecinstitute.com/topic/a-brief-introduction-to-the-nessus-vulnerability-scanner/","Beginner’s Guide to Nessus":"https://www.hackingarticles.in/beginners-guide-to-nessus/","Nessus Ubuntu Installation and Tutorial":"https://linuxhint.com/nessus-ubuntu-installation-tutorial/"},link="https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.4.2-debian9_amd64.deb",method="deb")
+            template.template("nessus","nessus",github.strip(),{"How To: Run Your First Vulnerability Scan with Nessus":"https://www.tenable.com/blog/how-to-run-your-first-vulnerability-scan-with-nessus","A brief introduction to the Nessus vulnerability scanner":"https://resources.infosecinstitute.com/topic/a-brief-introduction-to-the-nessus-vulnerability-scanner/","Beginner’s Guide to Nessus":"https://www.hackingarticles.in/beginners-guide-to-nessus/","Nessus Ubuntu Installation and Tutorial":"https://linuxhint.com/nessus-ubuntu-installation-tutorial/"},link="https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.4.2-debian9_amd64.deb",method="deb")
         elif option=="5":
             print(f"\n[+] dirb")
             os.system("clear")
             github = "DIRB IS a Web Content Scanner. It looks for existing (and/or hidden) Web Objects. It basically works by launching a dictionary basesd attack against a web server and analizing the response"
             template.template("dirb","dirb",github.strip(),{"Dirb — A web content scanner":"https://medium.com/tech-zoom/dirb-a-web-content-scanner-bc9cba624c86","Footprinting and Reconnaissance with DIRB Tool (For Security Researcher and Bug Bounty Hunters":"https://www.openbugbounty.org/blog/mas00712/footprinting-and-reconnaissance-with-dirb-tool-for-security-researcher-and-bug-bounty-hunters/","Comprehensive Guide on Dirb Tool":"https://www.hackingarticles.in/comprehensive-guide-on-dirb-tool/"})
         elif option=="6":
             print(f"\n[+] skipfish")
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/Wireless_Hacking.py` & `cyberonix-2.0.9/cyberonix/main/tools/Wireless_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/banner.py` & `cyberonix-2.0.9/cyberonix/main/tools/banner.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/data_validation.py` & `cyberonix-2.0.9/cyberonix/main/tools/data_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                             )
                         elif option == "2":
                             print("\n[+] Xsser")
                             github = github_getting_text(
                                 "https://www.kali.org/tools/xsser/", "p", 3
                             )
                             template.template(
-                                "Xsser",
+                                "xsser",
                                 "xsser -h",
                                 github.strip(),
                                 {
                                     "Detecting and Exploiting XSS Injections using XSSer Tool": "https://securityxploded.com/detecting-exploiting-xss-using-xsser-tool.php",
                                     "XSSer - Detect and Exploit XSS vulnerabilities": "https://gbhackers.com/xsser-automated-framework-detectexploit-report-xss-vulnerabilities/",
                                     "XSSer- Cross Site Scripting Penetration Tool": "https://www.ehacking.net/2011/02/xsser-cross-site-scripting-penetration.html",
                                 },
@@ -204,15 +204,15 @@
                         option = input(
                             f"\n {colors.select}Select an Option ->{colors.reset} "
                         )
                         if option == "0":
                             print("\n[+] SQLMap")
                             github = github_getting_text("https://sqlmap.org/", "p", 0)
                             template.template(
-                                "Sqlmap",
+                                "sqlmap",
                                 "sqlmap -h",
                                 github.strip(),
                                 {
                                     "What is SQL Injection? How to do it with sqlmap?": "https://medium.com/@feat7/what-is-sql-injection-how-to-do-it-with-sqlmap-1e630e8220b7",
                                     "SQL injection using Sqlmap": "https://auntoracharja.medium.com/sql-injection-using-sqlmap-44aa84f7779",
                                     "SQLmap Full Guide For Beginners": "https://systemweakness.com/sqlmap-full-guide-for-beginners-920934cdedac",
                                     "How to use SQLMAP to test a website for SQL Injection vulnerability": "https://www.geeksforgeeks.org/use-sqlmap-test-website-sql-injection-vulnerability/",
@@ -269,15 +269,15 @@
                             print("\n[+] Commix")
                             github = github_getting_text(
                                 "https://github.com/commixproject/commix",
                                 "p[dir=auto]",
                                 3,
                             )
                             template.template(
-                                "Commix",
+                                "commix",
                                 "python commix.py -h",
                                 github.strip(),
                                 {
                                     "Commix-Command Injection Exploiter (Beginner’s Guide)": "https://www.hackingarticles.in/commix-command-injection-exploiter-beginners-guide/",
                                     "Commix – OS Command Injection and Exploitation Tool": "https://www.geeksforgeeks.org/commix-os-command-injection-and-exploitation-tool/",
                                     "Commix - Automate Exploiting Command Injection Flaws in Web Applications": "https://null-byte.wonderhowto.com/how-to/use-commix-automate-exploiting-command-injection-flaws-web-applications-0189044/",
                                     "Commix : Detecting & Exploiting Command Injection Flaws.": "https://www.blackhat.com/docs/eu-15/materials/eu-15-Stasinopoulos-Commix-Detecting-And-Exploiting-Command-Injection-Flaws.pdf",
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/dos.py` & `cyberonix-2.0.9/cyberonix/main/tools/dos.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/html5.py` & `cyberonix-2.0.9/cyberonix/main/tools/html5.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/information_gathering.py` & `cyberonix-2.0.9/cyberonix/main/tools/information_gathering.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,52 +29,52 @@
             template.exit_program()
         if option == "0":
             print("\n[+] Nmap")
             os.system("clear")
             # name,command,discription,writeup,link=True,method="kali",github_install="",github_check=True
             github = "Nmap (Network Mapper) is a network scanner created by Gordon Lyon (also known by his pseudonym Fyodor Vaskovich). Nmap is used to discover hosts and services on a computer network by sending packets and analyzing the responses. "
             template.template(
-                "Nmap",
+                "nmap",
                 "nmap -h",
                 github.strip(),
                 {
                     "Nmap Cheat-Sheet": "https://www.stationx.net/nmap-cheat-sheet/",
                     "Official website": "https://nmap.org/ ",
                     "Other resources": "https://linux.die.net/man/1/nmap",
                 },
             )
         elif option == "1":
             print("\n[+] Maltego")
             os.system("clear")
             github = "Maltego is software used for open-source intelligence and forensics, developed by Paterva from Pretoria, South Africa. Maltego focuses on providing a library of transforms for discovery of data from open sources, and visualizing that information in a graph format, suitable for link analysis and data mining"
             template.template(
-                "Maltego",
+                "maltego",
                 "maltego",
                 github.strip(),
                 {
                     "Official website": "https://www.maltego.com/ ",
                     "How to use it": "https://www.geeksforgeeks.org/maltego-tool-in-kali-linux/ ",
                     "Other resources": "https://www.cyberpratibha.com/information-gathering-with-maltego/ ",
                 },
             )
         elif option == "2":
             print("\n[+] Dracnmap")
             os.system("clear")
             github = "Dracnmap is an open source program which is using to exploit the network and gathering information with nmap help. Nmap command comes with lots of options that can make the utility more robust and difficult to follow for new users. Hence Dracnmap is designed to perform fast scaning with the utilizing script engine of nmap and nmap can perform various automatic scanning techniques with the advanced commands."
             template.template(
                 "Dracnmap",
-                "chmod +x dracnmap-v2.2.sh && ./dracnmap-v2.2.sh",
+                "./dracnmap-v2.2.sh",
                 github.strip(),
                 {
                     "Github website": "https://github.com/Screetsec/Dracnmap",
                     "How to use": "https://www.geeksforgeeks.org/dracnmap-information-gathering-and-network-exploitation-tool/ ",
                     "Other resources": "https://www.hacking.land/2016/10/dracnmap-exploit-network-and-gathering.html?utm_source=dlvr.it&utm_medium=facebook&m=1 ",
                 },
                 method="github",
-                github_install="git clone https://github.com/Screetsec/Dracnmap.git",
+                github_install="git clone https://github.com/Screetsec/Dracnmap.git && chmod +x dracnmap-v2.2.sh",
                 github_check="Dracnmap",
             )
         elif option == "3":
             print("\n[+] RED_HAWK")
             os.system("clear")
             github = "Red Hawk is a free and open-source tool available on GitHub. Red Hawk is used to scanning websites for information gathering and finding vulnerabilities. Red Hawk is written in PHP. It uses PHP script to do reconnaissance. Red Hawk is so powerful that it can detect content management system while scanning, it can detect IP address, it can detect webserver record, it can detect Cloudflare information, and can detect robots.txt. Red Hawk can detect WordPress, Drupal, Joomla, and Magento CMS. Red Hawk looks for error-based SQL injections, WordPress sensitive files, and WordPress version-related vulnerabilities. RedHawk uses different modules for doing all the scannings."
             template.template(
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/run_on_browser.py` & `cyberonix-2.0.9/cyberonix/main/tools/run_on_browser.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/template.py` & `cyberonix-2.0.9/cyberonix/main/tools/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                             target=run_on_browser.main,
                             args=(self.command,)
                         ).start()
                     elif method == "github":
                         if not os.path.isdir("Tools"):
                             os.system("mkdir Tools")
                         if os.path.exists(f"Tools/{self.github_check}"):
-                            print(f"{colors.green}[+] It Is Installed{colors.reset}")
+                            print(f"{colors.green}[+] It Is Installed")
                             print(f"[+] It Is Installed In Your Kali{colors.reset}")
                             run = input(
                                 f"{colors.blue}[+] Do You Want To Run?(y/n):{colors.reset}"
                             )
                             if run.lower() == "yes" or run.lower() == "y":
                                 os.system(
                                     f"cd Tools/{self.github_check} && {self.command}"
@@ -95,15 +95,18 @@
 
 def tool_writeups(name,check="no-writeups", tool_check="no-tools"):
     if tool_check != "no-tools":
         print(f"{colors.options}1) Installation")
     if check != "no-writeups":
         print(f"2) Write Ups")
     print(f"3) Go Back..")
-    ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+    try:
+        ask = input(f"\n {colors.select}Select An Option ->{colors.reset}  ")
+    except KeyboardInterrupt:
+        exit_program()
     return ask
 def exit_program():
     os.system("clear")
     banner.main()
     print("\033[38;5;105m", "[+] Thanks visit again".title())
     exit()
```

### Comparing `cyberonix-2.0.8/cyberonix/main/tools/writeup.py` & `cyberonix-2.0.9/cyberonix/main/tools/writeup.py`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/cyberonix.egg-info/PKG-INFO` & `cyberonix-2.0.9/cyberonix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 2.0.8
+Version: 2.0.9
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamMetaxone/Cyberonix
 Author: Metaxone
 Author-email: admin@metaxonesolution.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 2.0.8 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 2.0.9 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamMetaxone/Cyberonix Author: Metaxone Author-email:
 admin@metaxonesolution.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `cyberonix-2.0.8/cyberonix.egg-info/SOURCES.txt` & `cyberonix-2.0.9/cyberonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberonix-2.0.8/setup.py` & `cyberonix-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cyberonix",
-    version="2.0.8",
+    version="2.0.9",
     author="Metaxone",
     author_email="admin@metaxonesolution.com",
     description="Cyberonix is a complete resource hub for Cyber Security Community.",
     url='https://github.com/TeamMetaxone/Cyberonix',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
@@ -22,16 +22,16 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Security",
     ],
     install_requires=[
-        "beautifulsoup4==4.11.1",
-        "requests==2.28.1",
+        "beautifulsoup4",
+        "requests",
         "ipwhois",
         "dnspython==2.3.0",
         "selenium==4.7.2",
     ],
     entry_points={
         'console_scripts': [
             'cyberonix = cyberonix.cyberonix:starting'
```

