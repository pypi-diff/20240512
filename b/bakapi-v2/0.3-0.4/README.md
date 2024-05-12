# Comparing `tmp/bakapi_v2-0.3.tar.gz` & `tmp/bakapi_v2-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakapi_v2-0.3.tar", last modified: Wed May  8 07:53:08 2024, max compression
+gzip compressed data, was "bakapi_v2-0.4.tar", last modified: Sun May 12 19:00:27 2024, max compression
```

## Comparing `bakapi_v2-0.3.tar` & `bakapi_v2-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:53:08.651543 bakapi_v2-0.3/
--rw-rw-rw-   0        0        0     1120 2024-05-06 20:21:19.000000 bakapi_v2-0.3/LICENSE
--rw-rw-rw-   0        0        0     3528 2024-05-08 07:53:08.649543 bakapi_v2-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2675 2024-05-08 07:51:51.000000 bakapi_v2-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:53:08.647542 bakapi_v2-0.3/bakapi_v2.egg-info/
--rw-rw-rw-   0        0        0     3528 2024-05-08 07:53:08.000000 bakapi_v2-0.3/bakapi_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-08 07:53:08.000000 bakapi_v2-0.3/bakapi_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:53:08.000000 bakapi_v2-0.3/bakapi_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 07:53:08.000000 bakapi_v2-0.3/bakapi_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 07:53:08.000000 bakapi_v2-0.3/bakapi_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7300 2024-05-07 17:51:08.000000 bakapi_v2-0.3/bakapiv2.py
--rw-rw-rw-   0        0        0       42 2024-05-08 07:53:08.652542 bakapi_v2-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1265 2024-05-08 07:52:03.000000 bakapi_v2-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:00:27.808467 bakapi_v2-0.4/
+-rw-rw-rw-   0        0        0     1120 2024-05-06 20:21:19.000000 bakapi_v2-0.4/LICENSE
+-rw-rw-rw-   0        0        0     2622 2024-05-12 19:00:27.805467 bakapi_v2-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1769 2024-05-12 18:55:54.000000 bakapi_v2-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 19:00:27.803467 bakapi_v2-0.4/bakapi_v2.egg-info/
+-rw-rw-rw-   0        0        0     2622 2024-05-12 19:00:27.000000 bakapi_v2-0.4/bakapi_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-12 19:00:27.000000 bakapi_v2-0.4/bakapi_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 19:00:27.000000 bakapi_v2-0.4/bakapi_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 19:00:27.000000 bakapi_v2-0.4/bakapi_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 19:00:27.000000 bakapi_v2-0.4/bakapi_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7897 2024-05-12 18:47:18.000000 bakapi_v2-0.4/bakapiv2.py
+-rw-rw-rw-   0        0        0       42 2024-05-12 19:00:27.808467 bakapi_v2-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2024-05-12 18:57:53.000000 bakapi_v2-0.4/setup.py
```

### Comparing `bakapi_v2-0.3/LICENSE` & `bakapi_v2-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bakapi_v2-0.3/PKG-INFO` & `bakapi_v2-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakapi-v2
-Version: 0.3
+Version: 0.4
 Summary: Klient k API Bakalářů v jazyce Python.
 Home-page: https://github.com/MortikCZ/bakapi-v2
 Author: Lukáš S., mwolfik
 Project-URL: Documentation, https://github.com/MortikCZ/bakapi-v2/blob/main/README.md
 Project-URL: Source Code, https://github.com/MortikCZ/bakapi-v2/blob/main/bakapi-v2.py
 Project-URL: License, https://github.com/MortikCZ/bakapi-v2/blob/main/LICENSE
 Project-URL: Issues, https://github.com/MortikCZ/bakapi-v2/issues
@@ -30,44 +30,26 @@
 
 Tento projekt používá kód z nasledujícího repozitáře:
 [bakapi](https://github.com/mvolfik/bakapi), autor: [mvolfik](https://github.com/mvolfik)
 
 ## Instalace
 Instalace je možná pomocí `pip` příkazu:
 ```bash
-pip install bakapiv2
-py -m pip install bakapiv2
+pip install bakapi-v2
+py -m pip install bakapi-v2
 ```
 ## Changelog
+### 0.4
+- Přidána funkce `get_timetable`, `get_timetable_actual`, `get_substitutions`, `get_subjects_info`, `get_subject_themes`, `get_marks_final`, `get_marks_measures` a `get_marks`.
+- Oprava chyb v dokumentaci
+- Oprava chyb v kódu
+- Dokumentace API klienta je dostupná v souboru [`API_docs.md`](https://github.com/MortikCZ/bakapi-v2/blob/main/API_docs.md).
 ### 0.3 
 - Oprava PyPi balíčku
 ### 0.2
 - Přidána funkce `get_api_info`, `get_absence`, `get_gdpr_info`, `get_marks`, `get_events`, `get_my_events` a `get_public_events`.
 - Nově je možné instalovat balíček pomocí `pip` příkazu.
 ### 0.1
 - První release 
 
 ## Dokumentace
-API klient je navržen pro komunikaci s API Bakalářů pomocí jazyka Python. Poskytuje sadu funkcí pro získávání dat z API a jejich manipulaci.
-
-### Funkce API klienta:
-- `get_student_info`: Tato funkce slouží k získání informací o studentovi.
-- `get_subjects`: Tato funkce vrátí seznam předmětů a informace o nich..
-- `get_timetable_actual`: Tato funkce vrátí rozvrh studenta.
-- `get_homework`: Tato funkce vrátí seznam domácích úkolů.
-- `get_absence`: Tato funkce vrátí seznam absencí studenta.
-- `get_marks`: Tato funkce vrátí seznam známek studenta.
-- `get_events`: Tato funkce vrátí seznam událostí.
-- `get_my_events`: Tato funkce vrátí seznam událostí studenta.
-- `get_public_events`: Tato funkce vrátí seznam veřejných událostí.
-- `get_gdpr_info`: Tato funkce vrátí informace o GDPR.
-- `get_api_info`: Tato funkce vrátí informace o API.
-
-Pro použití API klienta je nejprve nutné provést inicializaci objektu klienta a přihlášení pomocí přihlašovacích údajů studenta. Poté je možné volat jednotlivé funkce pro získání a manipulaci s daty z API.
-
-Proměnné potřebné pro přihlášení:
-- `username`: Uživatelské jméno
-- `password`: Heslo
-- `url`: URL adresa Bakalářů (musí odkazovat na přihlašovací stránku).
-
-##
-Kompletní dokumentaci k API Bakalářů a seznam Endpointů naleznete [zde](https://github.com/bakalari-api/bakalari-api-v3).
+Dokumentace k tomuto projektu je dostupná v souboru [`API_docs.md`](https://github.com/MortikCZ/bakapi-v2/blob/main/API_docs.md) v kořenovém adresáři tohoto repozitáře.
```

### Comparing `bakapi_v2-0.3/bakapi_v2.egg-info/PKG-INFO` & `bakapi_v2-0.4/bakapi_v2.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakapi-v2
-Version: 0.3
+Version: 0.4
 Summary: Klient k API Bakalářů v jazyce Python.
 Home-page: https://github.com/MortikCZ/bakapi-v2
 Author: Lukáš S., mwolfik
 Project-URL: Documentation, https://github.com/MortikCZ/bakapi-v2/blob/main/README.md
 Project-URL: Source Code, https://github.com/MortikCZ/bakapi-v2/blob/main/bakapi-v2.py
 Project-URL: License, https://github.com/MortikCZ/bakapi-v2/blob/main/LICENSE
 Project-URL: Issues, https://github.com/MortikCZ/bakapi-v2/issues
@@ -30,44 +30,26 @@
 
 Tento projekt používá kód z nasledujícího repozitáře:
 [bakapi](https://github.com/mvolfik/bakapi), autor: [mvolfik](https://github.com/mvolfik)
 
 ## Instalace
 Instalace je možná pomocí `pip` příkazu:
 ```bash
-pip install bakapiv2
-py -m pip install bakapiv2
+pip install bakapi-v2
+py -m pip install bakapi-v2
 ```
 ## Changelog
+### 0.4
+- Přidána funkce `get_timetable`, `get_timetable_actual`, `get_substitutions`, `get_subjects_info`, `get_subject_themes`, `get_marks_final`, `get_marks_measures` a `get_marks`.
+- Oprava chyb v dokumentaci
+- Oprava chyb v kódu
+- Dokumentace API klienta je dostupná v souboru [`API_docs.md`](https://github.com/MortikCZ/bakapi-v2/blob/main/API_docs.md).
 ### 0.3 
 - Oprava PyPi balíčku
 ### 0.2
 - Přidána funkce `get_api_info`, `get_absence`, `get_gdpr_info`, `get_marks`, `get_events`, `get_my_events` a `get_public_events`.
 - Nově je možné instalovat balíček pomocí `pip` příkazu.
 ### 0.1
 - První release 
 
 ## Dokumentace
-API klient je navržen pro komunikaci s API Bakalářů pomocí jazyka Python. Poskytuje sadu funkcí pro získávání dat z API a jejich manipulaci.
-
-### Funkce API klienta:
-- `get_student_info`: Tato funkce slouží k získání informací o studentovi.
-- `get_subjects`: Tato funkce vrátí seznam předmětů a informace o nich..
-- `get_timetable_actual`: Tato funkce vrátí rozvrh studenta.
-- `get_homework`: Tato funkce vrátí seznam domácích úkolů.
-- `get_absence`: Tato funkce vrátí seznam absencí studenta.
-- `get_marks`: Tato funkce vrátí seznam známek studenta.
-- `get_events`: Tato funkce vrátí seznam událostí.
-- `get_my_events`: Tato funkce vrátí seznam událostí studenta.
-- `get_public_events`: Tato funkce vrátí seznam veřejných událostí.
-- `get_gdpr_info`: Tato funkce vrátí informace o GDPR.
-- `get_api_info`: Tato funkce vrátí informace o API.
-
-Pro použití API klienta je nejprve nutné provést inicializaci objektu klienta a přihlášení pomocí přihlašovacích údajů studenta. Poté je možné volat jednotlivé funkce pro získání a manipulaci s daty z API.
-
-Proměnné potřebné pro přihlášení:
-- `username`: Uživatelské jméno
-- `password`: Heslo
-- `url`: URL adresa Bakalářů (musí odkazovat na přihlašovací stránku).
-
-##
-Kompletní dokumentaci k API Bakalářů a seznam Endpointů naleznete [zde](https://github.com/bakalari-api/bakalari-api-v3).
+Dokumentace k tomuto projektu je dostupná v souboru [`API_docs.md`](https://github.com/MortikCZ/bakapi-v2/blob/main/API_docs.md) v kořenovém adresáři tohoto repozitáře.
```

### Comparing `bakapi_v2-0.3/bakapiv2.py` & `bakapi_v2-0.4/bakapiv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,64 +143,72 @@
         if "error" in d:
             e = d["error"]
             if e == "invalid_grant":
                 raise InvalidCredentials
             else:
                 raise BakaAPIException
 
-        # retry with refreshed token if needed, but prevent infinite loops in case the
-        # the cause was something else
         if (
             d == {"Message": "Authorization has been denied for this request."}
             and not is_retry
         ):
             warnings.warn("Got authorization error, refreshing token and retrying")
             self.use_refresh_token()
             return self.query_api(endpoint, method, is_retry=True, **kwargs)
 
         return d
 
     def get_user_info(self):
         return self.query_api("api/3/user")
 
-    def get_homework(
-        self,
-        since: Union[datetime, date, str] = None,
-        to: Union[datetime, date, str] = None,
+    def get_homework_count(
+            self,
     ):
-        if type(since) in (date, datetime):
-            since = since.strftime("%Y-%m-%d")
-        if type(to) in (date, datetime):
-            to = to.strftime("%Y-%m-%d")
-        params = {}
-        if since:
-            params["from"] = since
-        if to:
-            params["to"] = to
-        return self.query_api("api/3/homework", params=params)
-
+        
+        return self.query_api("api/3/homeworks/count-actual")
+    
+    def get_timetable_perm(
+            self,
+    ):
+        return self.query_api("api/3/timetable/permanent")
+        
     def get_timetable_actual(
         self,
-        since: Union[datetime, date, str] = None,
-        to: Union[datetime, date, str] = None,
+        date: Union[datetime, date, str] = None,
+    ):
+        if type(date) in (date, datetime):
+            date = date.strftime("%Y-%m-%d")
+    
+        params = {"date": date}
+    
+        return self.query_api("api/3/timetable/actual", params=params)
+    
+    def get_substitutions(
+            self,
+            since: Union[datetime, date, str] = None,
     ):
         if type(since) in (date, datetime):
             since = since.strftime("%Y-%m-%d")
-        if type(to) in (date, datetime):
-            to = to.strftime("%Y-%m-%d")
 
-        params = {"from": since, "to": to}
-        
-        return self.query_api("api/3/timetable/actual", params=params)
+        params = {"from": since}
+
+        return self.query_api("api/3/substitutions", params=params)
 
     def get_subjects_info(
             self
             ):
         return self.query_api("api/3/subjects")
     
+    def get_subject_themes(
+            self,
+            subject_id
+    ):
+        endpoint = f"api/3/subjects/themes/{subject_id}"
+        return self.query_api(endpoint)
+    
     def get_api_info(
             self
     ):
         return self.query_api("api")
     
     def get_absence(
             self
@@ -210,33 +218,56 @@
     def get_gdpr_info(
             self
     ):
         return self.query_api("api/3/gdpr/commissioners")
     
     def get_marks(
         self,
-        since: Union[datetime, date, str] = None,
-        to: Union[datetime, date, str] = None,
     ):
-        if type(since) in (date, datetime):
-            since = since.strftime("%Y-%m-%d")
-        if type(to) in (date, datetime):
-            to = to.strftime("%Y-%m-%d")
-        
-        params = {"from": since, "to": to}
+        return self.query_api("api/3/marks")
+    
+    def get_marks_final(
+            self
+    ):
+        return self.query_api("api/3/marks/final")
+    
+    def get_marks_measures(
+            self,
+    ):
         
-        return self.query_api("api/3/marks", params=params)
+        return self.query_api("api/3/marks/measures")
     
     def get_events(
-            self
+            self,
+            since: Union[datetime, date, str] = None,
     ):
-        return self.query_api("api/3/events")
+        if type(since) in (date, datetime):
+            since = since.strftime("%Y-%m-%d")
+        params = {}
+        if since:
+            params["from"] = since
+            return self.query_api("api/3/events/my", params=params)
     
     def get_my_events(
-            self
+            self,
+            since: Union[datetime, date, str] = None,
     ):
-        return self.query_api("api/3/events/my")
+        if type(since) in (date, datetime):
+            since = since.strftime("%Y-%m-%d")
+        params = {}
+        if since:
+            params["from"] = since
+            return self.query_api("api/3/events/my", params=params)
     
     def get_public_events(
-            self
+            self,
+            since: Union[datetime, date, str] = None,
     ):
-        return self.query_api("api/3/events/public")
+        if type(since) in (date, datetime):
+            since = since.strftime("%Y-%m-%d")
+        params = {}
+        if since:
+            params["from"] = since
+            return self.query_api("api/3/events/my", params=params)
+
+
+
```

### Comparing `bakapi_v2-0.3/setup.py` & `bakapi_v2-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bakapi-v2',
-    version='0.3',
+    version='0.4',
     url='https://github.com/MortikCZ/bakapi-v2',
     project_urls = {
         "Documentation": "https://github.com/MortikCZ/bakapi-v2/blob/main/README.md",
         "Source Code": "https://github.com/MortikCZ/bakapi-v2/blob/main/bakapi-v2.py",
         "License": "https://github.com/MortikCZ/bakapi-v2/blob/main/LICENSE",
         "Issues"    : "https://github.com/MortikCZ/bakapi-v2/issues"
     },
```

