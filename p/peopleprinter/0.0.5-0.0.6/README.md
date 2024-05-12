# Comparing `tmp/peopleprinter-0.0.5.tar.gz` & `tmp/peopleprinter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopleprinter-0.0.5.tar", last modified: Wed Mar 27 13:43:38 2024, max compression
+gzip compressed data, was "peopleprinter-0.0.6.tar", last modified: Sun May 12 16:01:04 2024, max compression
```

## Comparing `peopleprinter-0.0.5.tar` & `peopleprinter-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.839679 peopleprinter-0.0.5/
--rw-rw-rw-   0        0        0      498 2024-03-27 13:43:38.838683 peopleprinter-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.797793 peopleprinter-0.0.5/peopleprinter/
--rw-rw-rw-   0        0        0       66 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/__init__.py
--rw-rw-rw-   0        0        0     1803 2024-03-19 13:24:03.000000 peopleprinter-0.0.5/peopleprinter/main.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.811753 peopleprinter-0.0.5/peopleprinter/manufacturers/
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.815743 peopleprinter-0.0.5/peopleprinter/manufacturers/HP/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/HP/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/HP/major_hp.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.825715 peopleprinter-0.0.5/peopleprinter/manufacturers/KYOCERA/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/KYOCERA/__init__.py
--rw-rw-rw-   0        0        0     3736 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
--rw-rw-rw-   0        0        0     2413 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/KYOCERA/major_kyocera.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.828708 peopleprinter-0.0.5/peopleprinter/manufacturers/PANTUM/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/PANTUM/__init__.py
--rw-rw-rw-   0        0        0     1018 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/PANTUM/major_pantum.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.832708 peopleprinter-0.0.5/peopleprinter/manufacturers/Xerox/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/Xerox/__init__.py
--rw-rw-rw-   0        0        0     3050 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/Xerox/major_xerox.py
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/manufacturers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.834692 peopleprinter-0.0.5/peopleprinter/src/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.5/peopleprinter/src/__init__.py
--rw-rw-rw-   0        0        0     2335 2024-03-19 13:26:52.000000 peopleprinter-0.0.5/peopleprinter/sub_main.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:43:38.836687 peopleprinter-0.0.5/peopleprinter.egg-info/
--rw-rw-rw-   0        0        0      498 2024-03-27 13:43:38.000000 peopleprinter-0.0.5/peopleprinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2024-03-27 13:43:38.000000 peopleprinter-0.0.5/peopleprinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 13:43:38.000000 peopleprinter-0.0.5/peopleprinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-27 13:43:38.000000 peopleprinter-0.0.5/peopleprinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      575 2024-03-27 13:43:10.000000 peopleprinter-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 13:43:38.839679 peopleprinter-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.269326 peopleprinter-0.0.6/
+-rw-rw-rw-   0        0        0      498 2024-05-12 16:01:04.268328 peopleprinter-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.237410 peopleprinter-0.0.6/peopleprinter/
+-rw-rw-rw-   0        0        0       67 2024-05-12 15:38:05.000000 peopleprinter-0.0.6/peopleprinter/__init__.py
+-rw-rw-rw-   0        0        0     1794 2024-05-12 15:38:21.000000 peopleprinter-0.0.6/peopleprinter/main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.255390 peopleprinter-0.0.6/peopleprinter/manufacturers/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.256360 peopleprinter-0.0.6/peopleprinter/manufacturers/HP/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/HP/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/HP/major_hp.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.261346 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/__init__.py
+-rw-rw-rw-   0        0        0     3736 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
+-rw-rw-rw-   0        0        0     2413 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/major_kyocera.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.263342 peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/__init__.py
+-rw-rw-rw-   0        0        0     1018 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/major_pantum.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.265337 peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/__init__.py
+-rw-rw-rw-   0        0        0     3050 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/major_xerox.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.266333 peopleprinter-0.0.6/peopleprinter/src/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/src/__init__.py
+-rw-rw-rw-   0        0        0     2336 2024-05-12 15:38:21.000000 peopleprinter-0.0.6/peopleprinter/sub_main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.267330 peopleprinter-0.0.6/peopleprinter.egg-info/
+-rw-rw-rw-   0        0        0      498 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-12 15:55:36.000000 peopleprinter-0.0.6/peopleprinter.egg-info/upload.txt
+-rw-rw-rw-   0        0        0      575 2024-05-12 15:58:15.000000 peopleprinter-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:01:04.269326 peopleprinter-0.0.6/setup.cfg
```

### Comparing `peopleprinter-0.0.5/peopleprinter/main.py` & `peopleprinter-0.0.6/peopleprinter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .sub_main import InitPrinter
-from .manufacturers.KYOCERA.major_kyocera import KyoceraMajor
-from .manufacturers.HP.major_hp import HPMajor
-from .manufacturers.PANTUM.major_pantum import PantumMajor
-from .manufacturers.Xerox.major_xerox import XeroxMajor
+from sub_main import InitPrinter
+from manufacturers.KYOCERA.major_kyocera import KyoceraMajor
+from manufacturers.HP.major_hp import HPMajor
+from manufacturers.PANTUM.major_pantum import PantumMajor
+from manufacturers.Xerox.major_xerox import XeroxMajor
 
 
 class PeoplePrinter(InitPrinter):
     def __init__(self, ip_address):
         super().__init__(ip_address)
 
     def info(self):
@@ -18,15 +18,14 @@
             x = PantumMajor
         elif self.prod == 'XEROX':
             x = XeroxMajor
         else:
             return 'Производитель неизвестен'
         return self.work(x(self.ip_address))
 
-
     # Принимает определенный класс производителя принтера
     def work(self, printer):
         return {
                 'ip_address': self.ip_address,
                 'mac_address': printer.mac(),
                 'host_name': printer.host_name(),
                 'prod': self.prod,
@@ -34,15 +33,15 @@
                 'locate': self.locate,
                 'toner_lvl': printer.toner(),
                 'prints_count': printer.prints_count()
                 }
 
 
 if __name__ == "__main__":
-    ip = '192.168.2.184'
+    ip = '10.12.21.87'
     printer = PeoplePrinter(ip)
     print(printer.info())
 
 
 # Возвращает словарь со всей инфой
 # {'ip_address': '192.168.1.39', 'mac_address': '00:17:C8:A0:4D:89', 'host_name': 'NetPRN1-AMBRA', 'prod': 'KYOCERA', 'model': 'ECOSYS M2735dn', 'locate': 'Olimp', 'toner_lvl': 75, 'prints_count': 24109}
 # получаем данные по ключу printer.full_info()['mac_address']
```

### Comparing `peopleprinter-0.0.5/peopleprinter/manufacturers/HP/major_hp.py` & `peopleprinter-0.0.6/peopleprinter/manufacturers/HP/major_hp.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.5/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py` & `peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.5/peopleprinter/manufacturers/KYOCERA/major_kyocera.py` & `peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/major_kyocera.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.5/peopleprinter/manufacturers/PANTUM/major_pantum.py` & `peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/major_pantum.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.5/peopleprinter/manufacturers/Xerox/major_xerox.py` & `peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/major_xerox.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.5/peopleprinter/sub_main.py` & `peopleprinter-0.0.6/peopleprinter/sub_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         return prod
 
     def init_info(self):
         return self.ip_address, self.prod, self.locate
 
 
 if __name__ == "__main__":
-    ip = '10.12.11.36'
+    ip = '192.168.1.39'
     printer = InitPrinter(ip)
     print(printer.init_info())
```

### Comparing `peopleprinter-0.0.5/peopleprinter.egg-info/SOURCES.txt` & `peopleprinter-0.0.6/peopleprinter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 peopleprinter/__init__.py
 peopleprinter/main.py
 peopleprinter/sub_main.py
 peopleprinter.egg-info/PKG-INFO
 peopleprinter.egg-info/SOURCES.txt
 peopleprinter.egg-info/dependency_links.txt
 peopleprinter.egg-info/top_level.txt
+peopleprinter.egg-info/upload.txt
 peopleprinter/manufacturers/__init__.py
 peopleprinter/manufacturers/HP/__init__.py
 peopleprinter/manufacturers/HP/major_hp.py
 peopleprinter/manufacturers/KYOCERA/__init__.py
 peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
 peopleprinter/manufacturers/KYOCERA/major_kyocera.py
 peopleprinter/manufacturers/PANTUM/__init__.py
```

### Comparing `peopleprinter-0.0.5/pyproject.toml` & `peopleprinter-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["bs4", "requests", "re"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peopleprinter"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Guazah", email="guazah@gmail.com" },
 ]
 description = "Parsing printers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

