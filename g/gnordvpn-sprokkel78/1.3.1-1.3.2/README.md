# Comparing `tmp/gnordvpn_sprokkel78-1.3.1.tar.gz` & `tmp/gnordvpn_sprokkel78-1.3.2.tar.gz`

## Comparing `gnordvpn_sprokkel78-1.3.1.tar` & `gnordvpn_sprokkel78-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/.DS_Store
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/MANIFEST.in
--rw-r--r--   0        0        0     7371 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/CHANGELOG.txt
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/LICENSE
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/__init__.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.css
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.desktop
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.png
--rw-r--r--   0        0        0    97881 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.py
--rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.svg
--rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/install.sh
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/uninstall.sh
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_allowlist.png
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_help.png
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_menu.png
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_meshnet.png
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_pause.png
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_peers.png
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_play.png
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_settings.png
--rw-r--r--   0        0        0    70827 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-1.png
--rw-r--r--   0        0        0    57303 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-2.png
--rw-r--r--   0        0        0    84859 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-3.png
--rw-r--r--   0        0        0    87941 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-4.png
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/LICENSE
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/MANIFEST.in
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/CHANGELOG.txt
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/LICENSE
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/__init__.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.css
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.desktop
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.png
+-rw-r--r--   0        0        0    97836 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.py
+-rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.svg
+-rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/install.sh
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/uninstall.sh
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_allowlist.png
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_help.png
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_menu.png
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_meshnet.png
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_pause.png
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_peers.png
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_play.png
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_settings.png
+-rw-r--r--   0        0        0    70827 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-1.png
+-rw-r--r--   0        0        0    57303 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-2.png
+-rw-r--r--   0        0        0    84859 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-3.png
+-rw-r--r--   0        0        0    87941 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-4.png
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/README.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 gnordvpn_sprokkel78-1.3.2/PKG-INFO
```

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/CHANGELOG.txt` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/CHANGELOG.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 ------------
 Pressing CTRL-q will quit the application.
 Pressing CTRL-m will minimize the application.
 
 CHANGELOG
 ---------
 
+# gnordvpn-sprokkel 1.3.2
+- fix for nordvpn version 3.18.1
+
 # gnordvpn-sprokkel78 1.3.1
 - this version is compatible with nordvpn client version 3.17.2 and up.
 - fix for the ubuntu dock application icon after doing a system wide installation.
   the new .desktop file is named /usr/share/applications/com.sprokkel78.gnordvpn.desktop,
 - code cleanup after setting the application id to com.sprokkel78.gnordvpn.
 - added peer nicknames to peer permissions view.
 - fix for show_devices output after changing to another menu item.
```

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/LICENSE` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/LICENSE`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/README.md` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 gnordvpn-sprokkel78
 
 A graphical user interface in PyGTK for using the nordvpn client binary on Ubuntu and other Linux distro's. 
 It requires Python3.10 or higher, Pip, Venv and the PyGTK apps, it also relies on gnome-terminal for accepting
-and sending files. Developed and tested on Ubuntu 23.10. 
-
-Installation on Ubuntu 23.10
-
-1. $sudo apt install python3 python3-dev python3-pip python3-venv
-2. $sudo apt install python3-gi python3-gi-cairo gir1.2-gtk-3.0
-3. $sudo apt install gnome-terminal
-4. $python3 -m venv --system-site-packages /home/USERNAME/Python3
-5. $cd /home/USERNAME/Python3/bin
-6. $./pip install gnordvpn-sprokkel78
-7. $cd /home/USERNAME/Python3/lib/python3.11/site-packages/gnordvpn_sprokkel78
-8. $/home/USERNAME/Python3/bin/python3 ./gnordvpn.py
+and sending files. Developed and tested on Ubuntu 24.04. 
 
 Note: You must start gnordvpn.py from its own directory or it will not find the css file.
 Note: check CHANGELOG.txt for additional notes and changes.
 
 Added 'install.sh' script for system-wide installation.
 - The startup shell script will be /usr/bin/gnordvpn
 - The application is installed in /usr/share/gnordvpn-sprokkel78
```

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.py` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 gi.require_version('Gtk', '3.0')
 from gi.repository import Gtk, GLib, Gdk
 from threading import Thread
 from time import sleep
 
 
-# VERSION = 1.3.1
-ver = "1.3.1"
+# VERSION = 1.3.2
+ver = "1.3.2"
 
 
 # TODO
 
 
 # GLOBAL VARIABLES
 pause = 0
@@ -2919,17 +2919,15 @@
         sb = Gtk.Statusbar()
         sb.show()
         box99c.pack_start(sb, True, True, 0)
         result = subprocess.Popen("/usr/bin/nordvpn version", shell=True,
                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
         rc = result.wait()
         out, err = result.communicate()
-        line = out.split('\n')
-        line[3].strip()
-        push = " " + line[3]
+        push = " " + str(out).strip()
         sb.push(0, push)
 
         win.present()
 
 
 # START A THREAD THAT GETS THE NORDVPN STATUS EVERY 4 SECONDS
 thread = Thread(target=Get_Nordvpn_Status)
@@ -2947,8 +2945,8 @@
 
 # START THE APPLICATION
 def main():
     app = MyApplication()
     app.run(None)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/gnordvpn.svg` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/gnordvpn.svg`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/install.sh` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/install.sh`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_allowlist.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_allowlist.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_help.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_help.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_menu.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_menu.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_meshnet.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_meshnet.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_pause.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_pause.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_peers.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_peers.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_play.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_play.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/images/b_settings.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/images/b_settings.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-1.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-1.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-2.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-2.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-3.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-3.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/src/gnordvpn_sprokkel78/screenshots/gnordvpn-4.png` & `gnordvpn_sprokkel78-1.3.2/src/gnordvpn_sprokkel78/screenshots/gnordvpn-4.png`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/LICENSE` & `gnordvpn_sprokkel78-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gnordvpn_sprokkel78-1.3.1/README.md` & `gnordvpn_sprokkel78-1.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 gnordvpn-sprokkel78
 
 A graphical user interface in PyGTK for using the nordvpn client binary on Ubuntu and other Linux distro's. 
 It requires Python3.10 or higher, Pip, Venv and the PyGTK apps, it also relies on gnome-terminal for accepting
-and sending files. Developed and tested on Ubuntu 23.10. 
-
-Installation on Ubuntu 23.10
-
-1. $sudo apt install python3 python3-dev python3-pip python3-venv
-2. $sudo apt install python3-gi python3-gi-cairo gir1.2-gtk-3.0
-3. $sudo apt install gnome-terminal
-4. $python3 -m venv --system-site-packages /home/USERNAME/Python3
-5. $cd /home/USERNAME/Python3/bin
-6. $./pip install gnordvpn-sprokkel78
-7. $cd /home/USERNAME/Python3/lib/python3.11/site-packages/gnordvpn_sprokkel78
-8. $/home/USERNAME/Python3/bin/python3 ./gnordvpn.py
+and sending files. Developed and tested on Ubuntu 24.04. 
 
 Note: You must start gnordvpn.py from its own directory or it will not find the css file.
 Note: check CHANGELOG.txt for additional notes and changes.
 
 Added 'install.sh' script for system-wide installation.
 - The startup shell script will be /usr/bin/gnordvpn
 - The application is installed in /usr/share/gnordvpn-sprokkel78
```

### Comparing `gnordvpn_sprokkel78-1.3.1/pyproject.toml` & `gnordvpn_sprokkel78-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gnordvpn_sprokkel78"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Sprokkel78", email="sprokkel78.bart@gmail.com" },
 ]
 description = "A graphical user interface in pygtk for using the nordvpn client binary on ubuntu and other linux distro's."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `gnordvpn_sprokkel78-1.3.1/PKG-INFO` & `gnordvpn_sprokkel78-1.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gnordvpn_sprokkel78
-Version: 1.3.1
+Version: 1.3.2
 Summary: A graphical user interface in pygtk for using the nordvpn client binary on ubuntu and other linux distro's.
 Author-email: Sprokkel78 <sprokkel78.bart@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 gnordvpn-sprokkel78
 
 A graphical user interface in PyGTK for using the nordvpn client binary on Ubuntu and other Linux distro's. 
 It requires Python3.10 or higher, Pip, Venv and the PyGTK apps, it also relies on gnome-terminal for accepting
-and sending files. Developed and tested on Ubuntu 23.10. 
-
-Installation on Ubuntu 23.10
-
-1. $sudo apt install python3 python3-dev python3-pip python3-venv
-2. $sudo apt install python3-gi python3-gi-cairo gir1.2-gtk-3.0
-3. $sudo apt install gnome-terminal
-4. $python3 -m venv --system-site-packages /home/USERNAME/Python3
-5. $cd /home/USERNAME/Python3/bin
-6. $./pip install gnordvpn-sprokkel78
-7. $cd /home/USERNAME/Python3/lib/python3.11/site-packages/gnordvpn_sprokkel78
-8. $/home/USERNAME/Python3/bin/python3 ./gnordvpn.py
+and sending files. Developed and tested on Ubuntu 24.04. 
 
 Note: You must start gnordvpn.py from its own directory or it will not find the css file.
 Note: check CHANGELOG.txt for additional notes and changes.
 
 Added 'install.sh' script for system-wide installation.
 - The startup shell script will be /usr/bin/gnordvpn
 - The application is installed in /usr/share/gnordvpn-sprokkel78
```

