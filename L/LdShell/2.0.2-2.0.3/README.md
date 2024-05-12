# Comparing `tmp/LdShell-2.0.2.tar.gz` & `tmp/LdShell-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LdShell-2.0.2.tar", last modified: Tue Apr  2 07:28:56 2024, max compression
+gzip compressed data, was "LdShell-2.0.3.tar", last modified: Sun May 12 02:02:40 2024, max compression
```

## Comparing `LdShell-2.0.2.tar` & `LdShell-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:28:56.328245 LdShell-2.0.2/
--rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-2.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-02 07:28:56.321134 LdShell-2.0.2/LdShell/
--rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-2.0.2/LdShell/__init__.py
--rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-2.0.2/LdShell/__version__.py
--rw-rw-rw-   0        0        0     8303 2024-04-02 07:27:05.000000 LdShell-2.0.2/LdShell/core.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:28:56.326291 LdShell-2.0.2/LdShell.egg-info/
--rw-rw-rw-   0        0        0     3038 2024-04-02 07:28:56.000000 LdShell-2.0.2/LdShell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-02 07:28:56.000000 LdShell-2.0.2/LdShell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:28:56.000000 LdShell-2.0.2/LdShell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 07:28:56.000000 LdShell-2.0.2/LdShell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3038 2024-04-02 07:28:56.327269 LdShell-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 07:28:56.328245 LdShell-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3767 2024-04-02 07:28:44.000000 LdShell-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:02:40.753208 LdShell-2.0.3/
+-rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-2.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-12 02:02:40.749641 LdShell-2.0.3/LdShell/
+-rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-2.0.3/LdShell/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-2.0.3/LdShell/__version__.py
+-rw-rw-rw-   0        0        0     8841 2024-05-12 01:56:40.000000 LdShell-2.0.3/LdShell/core.py
+-rw-rw-rw-   0        0        0      250 2024-05-12 01:54:35.000000 LdShell-2.0.3/LdShell/test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:02:40.752039 LdShell-2.0.3/LdShell.egg-info/
+-rw-rw-rw-   0        0        0     3038 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 02:02:40.000000 LdShell-2.0.3/LdShell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3038 2024-05-12 02:02:40.753208 LdShell-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:02:40.753208 LdShell-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3767 2024-05-12 01:59:58.000000 LdShell-2.0.3/setup.py
```

### Comparing `LdShell-2.0.2/LICENSE` & `LdShell-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LdShell-2.0.2/LdShell/core.py` & `LdShell-2.0.3/LdShell/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
         adb=11       #ADB命令
         shell=12     #Shell命令
         text=13
         content=14
         child=15
         Tap=16
         Checked=17
+        LongCLick=18
+        ListText=19
+        ListLocal=20
+        ALL=21
 class InitLdPlayer :
      index=0
      _debug=False
      def __init__(self, index=None,debug=False):
           InitLdPlayer.index=index
           InitLdPlayer._debug=debug
     
@@ -111,14 +115,18 @@
                 pass
         return "";
 
     # 下面定义了一个CLick方法
     def Click(self):
         return self.IniPost(LdType.Click)
 
+    # 下面定义了一个LongCLick方法
+    def LongCLick(self):
+        return self.IniPost(LdType.LongCLick)
+    
     # 下面定义了一个Input方法
     def Input(self,txt):
         self.input_text=txt
         return self.IniPost(LdType.Input)
 
     # 下面定义了一个Exists方法
     def Exists(self):
@@ -176,24 +184,36 @@
     def Shell(self,shell):
         self.input_text=shell
         return self.IniPost(LdType.shell)
     
     # 下面定义了一个 Text 方法
     def Text(self):
         return self.InistrPost(LdType.text)
+
+    # 下面定义了一个 ALL 方法
+    def ALL(self):
+        return self.InistrPost(LdType.ALL)
+    
+    # 下面定义了一个 ListText 方法
+    def ListText(self):
+        return self.InistrPost(LdType.ListText)
+    
+    # 下面定义了一个 ListLocal 方法
+    def ListLocal(self):
+        return self.InistrPost(LdType.ListLocal)
     
     # 下面定义了一个 Content 方法
     def Content(self):
         return self.InistrPost(LdType.content)
 
     # 下面定义了一个 Child 方法
     def Child(self):
         return self.InistrPost(LdType.child)
     
-    # 下面定义了一个 Content 方法
+    # 下面定义了一个 Tap 方法
     def Tap(self,xy):
         self.input_text=xy
         return self.IniPost(LdType.Tap)
 
 
     # 下面定义了一个 Back 方法
     def Back(self):
@@ -217,15 +237,14 @@
         return self.IniPost(LdType.shell)
     
     # 下面定义了一个 BackSpage 方法
     def BackSpage(self):
         self.input_text="input keyevent 67"
         return self.IniPost(LdType.shell)
         
-
     # 读取INI文件
     def ReadINI(self,node='Main',key='about',enc='gbk'):
         try:
             IniPath = os.path.dirname(os.path.abspath(sys.argv[0]))+"\\system.ini"
             config = ConfigObj(IniPath,encoding=enc)
             _value=config[node][key]
             return _value
```

### Comparing `LdShell-2.0.2/LdShell.egg-info/PKG-INFO` & `LdShell-2.0.3/LdShell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 2.0.2
+Version: 2.0.3
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-2.0.2/PKG-INFO` & `LdShell-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 2.0.2
+Version: 2.0.3
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-2.0.2/README.md` & `LdShell-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `LdShell-2.0.2/setup.py` & `LdShell-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LdShell'
 DESCRIPTION = 'My short description for my project.'
 URL="http://www.google.com/"
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

