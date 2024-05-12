# Comparing `tmp/peopleprinter-0.0.6.tar.gz` & `tmp/peopleprinter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopleprinter-0.0.6.tar", last modified: Sun May 12 16:01:04 2024, max compression
+gzip compressed data, was "peopleprinter-0.0.7.tar", last modified: Sun May 12 16:25:45 2024, max compression
```

## Comparing `peopleprinter-0.0.6.tar` & `peopleprinter-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.269326 peopleprinter-0.0.6/
--rw-rw-rw-   0        0        0      498 2024-05-12 16:01:04.268328 peopleprinter-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.237410 peopleprinter-0.0.6/peopleprinter/
--rw-rw-rw-   0        0        0       67 2024-05-12 15:38:05.000000 peopleprinter-0.0.6/peopleprinter/__init__.py
--rw-rw-rw-   0        0        0     1794 2024-05-12 15:38:21.000000 peopleprinter-0.0.6/peopleprinter/main.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.255390 peopleprinter-0.0.6/peopleprinter/manufacturers/
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.256360 peopleprinter-0.0.6/peopleprinter/manufacturers/HP/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/HP/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/HP/major_hp.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.261346 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/__init__.py
--rw-rw-rw-   0        0        0     3736 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
--rw-rw-rw-   0        0        0     2413 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/major_kyocera.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.263342 peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/__init__.py
--rw-rw-rw-   0        0        0     1018 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/major_pantum.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.265337 peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/__init__.py
--rw-rw-rw-   0        0        0     3050 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/major_xerox.py
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/manufacturers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.266333 peopleprinter-0.0.6/peopleprinter/src/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.6/peopleprinter/src/__init__.py
--rw-rw-rw-   0        0        0     2336 2024-05-12 15:38:21.000000 peopleprinter-0.0.6/peopleprinter/sub_main.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:01:04.267330 peopleprinter-0.0.6/peopleprinter.egg-info/
--rw-rw-rw-   0        0        0      498 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 16:01:04.000000 peopleprinter-0.0.6/peopleprinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-12 15:55:36.000000 peopleprinter-0.0.6/peopleprinter.egg-info/upload.txt
--rw-rw-rw-   0        0        0      575 2024-05-12 15:58:15.000000 peopleprinter-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 16:01:04.269326 peopleprinter-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.686225 peopleprinter-0.0.7/
+-rw-rw-rw-   0        0        0      498 2024-05-12 16:25:45.684227 peopleprinter-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.638351 peopleprinter-0.0.7/peopleprinter/
+-rw-rw-rw-   0        0        0       67 2024-05-12 15:38:05.000000 peopleprinter-0.0.7/peopleprinter/__init__.py
+-rw-rw-rw-   0        0        0     1806 2024-05-12 16:20:11.000000 peopleprinter-0.0.7/peopleprinter/main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.662287 peopleprinter-0.0.7/peopleprinter/manufacturers/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.663284 peopleprinter-0.0.7/peopleprinter/manufacturers/HP/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/HP/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/HP/major_hp.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.666276 peopleprinter-0.0.7/peopleprinter/manufacturers/KYOCERA/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/KYOCERA/__init__.py
+-rw-rw-rw-   0        0        0     3736 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
+-rw-rw-rw-   0        0        0     2413 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/KYOCERA/major_kyocera.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.668270 peopleprinter-0.0.7/peopleprinter/manufacturers/PANTUM/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/PANTUM/__init__.py
+-rw-rw-rw-   0        0        0     1018 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/PANTUM/major_pantum.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.671271 peopleprinter-0.0.7/peopleprinter/manufacturers/Xerox/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/Xerox/__init__.py
+-rw-rw-rw-   0        0        0     3050 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/Xerox/major_xerox.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/manufacturers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.680244 peopleprinter-0.0.7/peopleprinter/src/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:14:55.000000 peopleprinter-0.0.7/peopleprinter/src/__init__.py
+-rw-rw-rw-   0        0        0     2334 2024-05-12 16:24:07.000000 peopleprinter-0.0.7/peopleprinter/sub_main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:25:45.682233 peopleprinter-0.0.7/peopleprinter.egg-info/
+-rw-rw-rw-   0        0        0      498 2024-05-12 16:25:45.000000 peopleprinter-0.0.7/peopleprinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-05-12 16:25:45.000000 peopleprinter-0.0.7/peopleprinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:25:45.000000 peopleprinter-0.0.7/peopleprinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 16:25:45.000000 peopleprinter-0.0.7/peopleprinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      575 2024-05-12 16:25:20.000000 peopleprinter-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:25:45.687220 peopleprinter-0.0.7/setup.cfg
```

### Comparing `peopleprinter-0.0.6/peopleprinter/main.py` & `peopleprinter-0.0.7/peopleprinter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 
 if __name__ == "__main__":
     ip = '10.12.21.87'
     printer = PeoplePrinter(ip)
     print(printer.info())
 
 
-# Возвращает словарь со всей инфой
-# {'ip_address': '192.168.1.39', 'mac_address': '00:17:C8:A0:4D:89', 'host_name': 'NetPRN1-AMBRA', 'prod': 'KYOCERA', 'model': 'ECOSYS M2735dn', 'locate': 'Olimp', 'toner_lvl': 75, 'prints_count': 24109}
-# получаем данные по ключу printer.full_info()['mac_address']
+    # Возвращает словарь со всей инфой
+    # {'ip_address': '192.168.1.39', 'mac_address': '00:17:C8:A0:4D:89', 'host_name': 'NetPRN1-AMBRA', 'prod': 'KYOCERA', 'model': 'ECOSYS M2735dn', 'locate': 'Olimp', 'toner_lvl': 75, 'prints_count': 24109}
+    # получаем данные по ключу printer.full_info()['mac_address']
```

### Comparing `peopleprinter-0.0.6/peopleprinter/manufacturers/HP/major_hp.py` & `peopleprinter-0.0.7/peopleprinter/manufacturers/HP/major_hp.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py` & `peopleprinter-0.0.7/peopleprinter/manufacturers/KYOCERA/kyocera_3040.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.6/peopleprinter/manufacturers/KYOCERA/major_kyocera.py` & `peopleprinter-0.0.7/peopleprinter/manufacturers/KYOCERA/major_kyocera.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.6/peopleprinter/manufacturers/PANTUM/major_pantum.py` & `peopleprinter-0.0.7/peopleprinter/manufacturers/PANTUM/major_pantum.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.6/peopleprinter/manufacturers/Xerox/major_xerox.py` & `peopleprinter-0.0.7/peopleprinter/manufacturers/Xerox/major_xerox.py`

 * *Files identical despite different names*

### Comparing `peopleprinter-0.0.6/peopleprinter/sub_main.py` & `peopleprinter-0.0.7/peopleprinter/sub_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         self.ip_address = ip_address
         self.main_page = self.__get_main_page_printer()
         self.locate = self.find_locate(ip_address)
         self.prod = self.get_prod_printer()
 
     @staticmethod
     def find_locate(ip_address):
-        f = re.findall(r"\d*.\d*.(\d*1)\d.\d*", ip_address)[0]
+        f = re.findall(r"\d*.\d*.(\d*)\d.\d*", ip_address)[0]
         if f == '1':
             locate = 'Olimp'
         elif f == '2':
-            locate = 'Summarinn'
+            locate = 'Sunmarinn'
         elif f == '4':
             locate = 'Aurum'
         else:
             locate = 'Неизвестно'
         return locate
 
     def __get_main_page_printer(self):
@@ -58,10 +58,10 @@
         return prod
 
     def init_info(self):
         return self.ip_address, self.prod, self.locate
 
 
 if __name__ == "__main__":
-    ip = '192.168.1.39'
+    ip = '10.12.11.87'
     printer = InitPrinter(ip)
     print(printer.init_info())
```

### Comparing `peopleprinter-0.0.6/peopleprinter.egg-info/SOURCES.txt` & `peopleprinter-0.0.7/peopleprinter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 peopleprinter/__init__.py
 peopleprinter/main.py
 peopleprinter/sub_main.py
 peopleprinter.egg-info/PKG-INFO
 peopleprinter.egg-info/SOURCES.txt
 peopleprinter.egg-info/dependency_links.txt
 peopleprinter.egg-info/top_level.txt
-peopleprinter.egg-info/upload.txt
 peopleprinter/manufacturers/__init__.py
 peopleprinter/manufacturers/HP/__init__.py
 peopleprinter/manufacturers/HP/major_hp.py
 peopleprinter/manufacturers/KYOCERA/__init__.py
 peopleprinter/manufacturers/KYOCERA/kyocera_3040.py
 peopleprinter/manufacturers/KYOCERA/major_kyocera.py
 peopleprinter/manufacturers/PANTUM/__init__.py
```

### Comparing `peopleprinter-0.0.6/pyproject.toml` & `peopleprinter-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["bs4", "requests", "re"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peopleprinter"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Guazah", email="guazah@gmail.com" },
 ]
 description = "Parsing printers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

