# Comparing `tmp/azubiheftapi-0.0.94.tar.gz` & `tmp/azubiheftapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azubiheftapi-0.0.94.tar", last modified: Fri Apr 26 19:18:53 2024, max compression
+gzip compressed data, was "azubiheftapi-1.0.0.tar", last modified: Sat May 11 22:25:29 2024, max compression
```

## Comparing `azubiheftapi-0.0.94.tar` & `azubiheftapi-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/azubiheftApi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/azubiheftApi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17838 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/azubiheftApi/azubiheftApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/azubiheftApi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/azubiheftApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 19:18:53.000000 azubiheftapi-0.0.94/azubiheftApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:18:53.308330 azubiheftapi-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-26 19:18:40.000000 azubiheftapi-0.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:29.145763 azubiheftapi-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-11 22:25:29.145763 azubiheftapi-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:29.145763 azubiheftapi-1.0.0/azubiheftApi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/azubiheftApi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16142 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/azubiheftApi/azubiheftApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/azubiheftApi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:29.145763 azubiheftapi-1.0.0/azubiheftApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-11 22:25:29.000000 azubiheftapi-1.0.0/azubiheftApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 22:25:29.000000 azubiheftapi-1.0.0/azubiheftApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:25:29.000000 azubiheftapi-1.0.0/azubiheftApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 22:25:29.000000 azubiheftapi-1.0.0/azubiheftApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 22:25:29.000000 azubiheftapi-1.0.0/azubiheftApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:25:29.145763 azubiheftapi-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:29.145763 azubiheftapi-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-11 22:25:22.000000 azubiheftapi-1.0.0/tests/test.py
```

### Comparing `azubiheftapi-0.0.94/LICENSE` & `azubiheftapi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azubiheftapi-0.0.94/PKG-INFO` & `azubiheftapi-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azubiheftApi
-Version: 0.0.94
+Version: 1.0.0
 Summary: Azubiheft.de custom api
 Home-page: https://github.com/leonkohli/azubiheft-api
 Author: Leon Kohlhaussen
 Author-email: kohli.leon@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -61,14 +61,15 @@
 # Delete an existing subject by ID
 azubiheft.delete_subject("subjectId")
 
 # Fetch a report by date
 report = azubiheft.getReport(datetime(2023, 10, 19))
 print(report)
 
+
 # Get a week's report ID
 week_id = azubiheft.getReportWeekId(datetime.now())
 print(week_id)
 
 # Write a new report entry
 azubiheft.writeReport(datetime(2023, 10, 19), "Hello World", "2:00", 1)
 # its also possible to format the text using \n or just like this
@@ -78,14 +79,18 @@
 # """
 
 # Fetch the report again to see changes
 report = azubiheft.getReport(datetime(2023, 10, 19), include_formatting=True)  #  include_formatting=True to include formatting
 print(report)
 
 
+# delete a report entry
+azubiheft.deleteReport(datetime(2023, 10, 19))
+
+
 # Log out from the session
 azubiheft.logout()
 
 # Check login status (should be False after logging out)
 print(azubiheft.isLoggedIn())
```

### Comparing `azubiheftapi-0.0.94/README.md` & `azubiheftapi-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 # Delete an existing subject by ID
 azubiheft.delete_subject("subjectId")
 
 # Fetch a report by date
 report = azubiheft.getReport(datetime(2023, 10, 19))
 print(report)
 
+
 # Get a week's report ID
 week_id = azubiheft.getReportWeekId(datetime.now())
 print(week_id)
 
 # Write a new report entry
 azubiheft.writeReport(datetime(2023, 10, 19), "Hello World", "2:00", 1)
 # its also possible to format the text using \n or just like this
@@ -60,14 +61,18 @@
 # """
 
 # Fetch the report again to see changes
 report = azubiheft.getReport(datetime(2023, 10, 19), include_formatting=True)  #  include_formatting=True to include formatting
 print(report)
 
 
+# delete a report entry
+azubiheft.deleteReport(datetime(2023, 10, 19))
+
+
 # Log out from the session
 azubiheft.logout()
 
 # Check login status (should be False after logging out)
 print(azubiheft.isLoggedIn())
```

### Comparing `azubiheftapi-0.0.94/azubiheftApi/azubiheftApi.py` & `azubiheftapi-1.0.0/azubiheftApi/azubiheftApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,119 @@
 #!/usr/bin/python3
 # azubiheft.com web-api
 
 import requests
 from bs4 import BeautifulSoup, NavigableString
 from datetime import datetime, timedelta
-from .errors import AuthError, ValueTooLargeError, NotLoggedInError
-import time
-from typing import List
+from typing import List, Optional, Dict
 import urllib.parse
 import re
+import logging
+import time
+
+from .errors import AuthError, ValueTooLargeError, NotLoggedInError
 
+# Configure the logging
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
 
 class Entry:
     def __init__(self, date: datetime, message: str, time_spent: str, entry_type: int):
         self.date = date
         self.message = message
         self.time_spent = time_spent
         self.type = entry_type
 
-
 class Session:
+    BASE_URL = "https://www.azubiheft.de"
+
     def __init__(self):
         """Initializes the Azubiheft session."""
-        self.session: requests.sessions.Session = None
+        self.session: Optional[requests.sessions.Session] = None
 
     def login(self, username: str, password: str) -> None:
-        """Logs in the user.
-        - Parameters:
-            username: Username of the user.
-            password: Password of the user.
-        """
+        """Log in the user with the provided username and password."""
         if self.isLoggedIn():
-            raise AuthError("already logged in. Logout first")
+            raise AuthError("Already logged in. Logout first.")
 
         self.session = requests.session()
+        login_page_html = self.session.get(
+            urllib.parse.urljoin(self.BASE_URL, "/Login.aspx")
+        )
+        soup = BeautifulSoup(login_page_html.text, "html.parser")
 
-        loginPageHtml = self.session.get("https://www.azubiheft.de/Login.aspx")
-
-        soup = BeautifulSoup(loginPageHtml.text, "html.parser")
-
-        viewstate = soup.find(id="__VIEWSTATE")["value"]
-        viewstategenerator = soup.find(id="__VIEWSTATEGENERATOR")["value"]
-        eventvalidation = soup.find(id="__EVENTVALIDATION")["value"]
+        tokens = self._extract_form_tokens(soup)
 
-        headers = {"content-type": "application/x-www-form-urlencoded"}
+        headers = {"Content-Type": "application/x-www-form-urlencoded"}
         formData = {
-            "__VIEWSTATE": viewstate,
-            "__VIEWSTATEGENERATOR": viewstategenerator,
-            "__EVENTVALIDATION": eventvalidation,
+            "__VIEWSTATE": tokens["__VIEWSTATE"],
+            "__VIEWSTATEGENERATOR": tokens["__VIEWSTATEGENERATOR"],
+            "__EVENTVALIDATION": tokens["__EVENTVALIDATION"],
             "ctl00$ContentPlaceHolder1$txt_Benutzername": username,
             "ctl00$ContentPlaceHolder1$txt_Passwort": password,
             "ctl00$ContentPlaceHolder1$chk_Persistent": "on",
             "ctl00$ContentPlaceHolder1$cmd_Login": "Anmelden",
             "ctl00$ContentPlaceHolder1$HiddenField_isMobile": "false",
         }
 
         self.session.post(
-            "https://www.azubiheft.de/Login.aspx", headers=headers, data=formData
+            urllib.parse.urljoin(self.BASE_URL, "/Login.aspx"),
+            headers=headers,
+            data=formData,
         )
+
         if not self.isLoggedIn():
-            raise AuthError("login failed")
+            raise AuthError("Login failed.")
 
     def logout(self) -> None:
-        """Logs out the user."""
+        """Log out the current user."""
         if not self.session:
-            raise NotLoggedInError("not logged in. Login first")
-        self.session.get("https://www.azubiheft.de/Azubi/Abmelden.aspx")
-        if not self.isLoggedIn():
-            self.session = None
+            raise NotLoggedInError("Not logged in. Login first.")
+        self.session.get(urllib.parse.urljoin(self.BASE_URL, "/Azubi/Abmelden.aspx"))
+        self.session = None
 
     def isLoggedIn(self) -> bool:
-        """Checks if the user is logged in.
-        - Returns:
-            True if the user is logged in, False otherwise.
-        """
+        """Check if the user is currently logged in."""
         if not self.session:
             return False
 
-        indexHtml = self.session.get("https://www.azubiheft.de/Azubi/Default.aspx").text
-        soup = BeautifulSoup(indexHtml, "html.parser")
-        viewstate = soup.find(id="Abmelden")
-        if viewstate:
-            return True
+        index_html = self.session.get(
+            urllib.parse.urljoin(self.BASE_URL, "/Azubi/Default.aspx")
+        ).text
+        soup = BeautifulSoup(index_html, "html.parser")
+        return bool(soup.find(id="Abmelden"))
 
-        return False
-
-    def _fetch_setup_page_tokens(self):
-        """
-        Fetches the setup page and extracts necessary tokens.
-        Returns a dictionary with '__VIEWSTATE', '__VIEWSTATEGENERATOR', and '__EVENTVALIDATION'.
-        """
+    def _fetch_setup_page_tokens(self) -> Dict[str, str]:
+        """Fetch the setup page and extract necessary tokens."""
         setup_page = self.session.get(
-            "https://www.azubiheft.de/Azubi/SetupSchulfach.aspx"
+            urllib.parse.urljoin(self.BASE_URL, "/Azubi/SetupSchulfach.aspx")
         )
         soup = BeautifulSoup(setup_page.text, "html.parser")
+        return self._extract_form_tokens(soup)
 
-        tokens = {
-            "__VIEWSTATE": soup.find(id="__VIEWSTATE")["value"],
-            "__VIEWSTATEGENERATOR": soup.find(id="__VIEWSTATEGENERATOR")["value"],
-            "__EVENTVALIDATION": soup.find(id="__EVENTVALIDATION")["value"],
+    def _extract_form_tokens(self, soup: BeautifulSoup) -> Dict[str, str]:
+        """Extract __VIEWSTATE, __VIEWSTATEGENERATOR, and __EVENTVALIDATION tokens from BeautifulSoup object."""
+        viewstate = soup.find(id="__VIEWSTATE")
+        viewstategenerator = soup.find(id="__VIEWSTATEGENERATOR")
+        eventvalidation = soup.find(id="__EVENTVALIDATION")
+        return {
+            "__VIEWSTATE": viewstate["value"] if viewstate else "",
+            "__VIEWSTATEGENERATOR": (
+                viewstategenerator["value"] if viewstategenerator else ""
+            ),
+            "__EVENTVALIDATION": eventvalidation["value"] if eventvalidation else "",
         }
-        return tokens
 
     def _prepare_subjects_payload(
-        self, subjects, new_subject=None, delete_subject_id=None
-    ):
-        """
-        Prepares payload for subject manipulation.
-        - Parameters:
-            subjects: List of current subjects.
-            new_subject: New subject to be added (optional).
-            delete_subject_id: ID of subject to be deleted (optional).
-        """
+        self,
+        subjects: List[Dict[str, str]],
+        new_subject: Optional[str] = None,
+        delete_subject_id: Optional[str] = None,
+    ) -> Dict[str, str]:
+        """Prepare payload for subject manipulation."""
         payload = {}
         for subject in subjects:
             if delete_subject_id and subject["id"] == delete_subject_id:
                 continue
             payload[f'ctl00$ContentPlaceHolder1$txt{subject["id"]}'] = subject["name"]
 
         if new_subject:
@@ -152,327 +150,280 @@
 
         if response.status_code != 200:
             print("Failed to add subject. Response code:", response.status_code)
         else:
             print("Subject added successfully.")
 
     def delete_subject(self, subject_id: str) -> None:
-        """Deletes a subject from the list of subjects.
-        - Parameters:
-            subject_id: ID of the subject to be deleted.
-        """
+        """Delete a subject from the list of subjects."""
         if not self.isLoggedIn():
-            raise NotLoggedInError("not logged in. Login first")
+            raise NotLoggedInError("Not logged in. Login first.")
 
         tokens = self._fetch_setup_page_tokens()
         current_subjects = self.getSubjects()
 
-        # Constructing the payload
         payload = {
             "__VIEWSTATE": tokens["__VIEWSTATE"],
             "__VIEWSTATEGENERATOR": tokens["__VIEWSTATEGENERATOR"],
             "__EVENTVALIDATION": tokens["__EVENTVALIDATION"],
-            "ctl00$ContentPlaceHolder1$HiddenLöschIDs": ","
-            + subject_id,  # Add leading comma
+            "ctl00$ContentPlaceHolder1$HiddenLöschIDs": "," + subject_id,
             **{
                 f'ctl00$ContentPlaceHolder1$txt{subj["id"]}': subj["name"]
                 for subj in current_subjects
                 if subj["id"] != subject_id
             },
             "ctl00$ContentPlaceHolder1$cmd_Save": "Speichern",
         }
 
-        # Sending the request
         response = self.session.post(
-            "https://www.azubiheft.de/Azubi/SetupSchulfach.aspx", data=payload
+            urllib.parse.urljoin(self.BASE_URL, "/Azubi/SetupSchulfach.aspx"),
+            data=payload,
         )
 
         if response.status_code != 200:
-            print("Failed to delete subject. Response code:", response.status_code)
+            logger.error(
+                f"Failed to delete subject. Response code: {response.status_code}"
+            )
         else:
-            print("Subject deleted successfully.")
+            logger.info("Subject deleted successfully.")
 
     def getReportWeekId(self, date: datetime) -> str:
-        """Gets the week ID for a given date.
-        - Parameters:
-            date: Date for which the week ID should be retrieved.
-        - Returns:
-            Week ID for the given date.
-        """
-        if self.isLoggedIn():
-            url = "https://www.azubiheft.de/Azubi/Ausbildungsnachweise.aspx"
-            overviewHtml = self.session.get(url).text
-            soup = BeautifulSoup(overviewHtml, "html.parser")
-            weekDivs = soup.find_all("div", class_="mo NBox")
-
-            # Calculate the calendar week number
-            calendar_week = date.isocalendar()[1]
-            year = date.isocalendar()[0]
-
-            for div in weekDivs:
-                kwDiv = div.find("div", class_="sKW")
-                yearDiv = div.find("div", class_="KW").find_all("div")[2]
-
-                if kwDiv and yearDiv:
-                    kw = int(kwDiv.get_text(strip=True))
-                    kwYear = int(yearDiv.get_text(strip=True))
-
-                    if kw == calendar_week and kwYear == year:
-                        weekId = div["onclick"].split("'")[1].split("=")[1]
-                        return weekId
+        """Get the week ID for a given date."""
+        if not self.isLoggedIn():
+            raise NotLoggedInError("Not logged in. Login first.")
 
-            raise ValueError("No report found for the specified week")
-        else:
-            raise NotLoggedInError("not logged in. Login first")
+        url = urllib.parse.urljoin(self.BASE_URL, "/Azubi/Ausbildungsnachweise.aspx")
+        overview_html = self.session.get(url).text
+        soup = BeautifulSoup(overview_html, "html.parser")
+        week_divs = soup.find_all("div", class_="mo NBox")
+
+        calendar_week = date.isocalendar()[1]
+        year = date.isocalendar()[0]
+
+        for div in week_divs:
+            kw_div = None
+            year_div = None
+            if "onclick" in div.attrs:
+                kw_div = div.find("div", class_="sKW")
+                year_div_elements = div.find("div", class_="KW").find_all("div")
+                if len(year_div_elements) > 2:
+                    year_div = year_div_elements[2]
+
+            if kw_div and year_div:
+                kw = int(kw_div.get_text(strip=True))
+                kw_year = int(year_div.get_text(strip=True))
+
+                if kw == calendar_week and kw_year == year:
+                    week_id = div["onclick"].split("'")[1].split("=")[1]
+                    return week_id
 
-    def getSubjects(self) -> list:
-        """Gets the list of subjects.
-        - Returns:
-            List of subjects.
-        """
-        if self.isLoggedIn():
-            staticSubjects = [
-                {"id": 1, "name": "Betrieb"},
-                {"id": 2, "name": "Schule"},
-                {"id": 3, "name": "ÜBA"},
-                {"id": 4, "name": "Urlaub"},
-                {"id": 5, "name": "Feiertag"},
-                {"id": 6, "name": "Arbeitsunfähig"},
-                {"id": 7, "name": "Frei"},
-            ]
-            subjectSetupHtml = self.session.get(
-                "https://www.azubiheft.de/Azubi/SetupSchulfach.aspx"
-            ).text
-            soup = BeautifulSoup(subjectSetupHtml, "html.parser")
-            subjectElements = soup.find(id="divSchulfach").find_all("input")
-
-            subjects = []
-            for subjectElement in subjectElements:
-                subject = {
-                    "id": subjectElement["data-default"],
-                    "name": subjectElement["value"],
-                }
-                subjects.append(subject)
+        raise ValueError("No report found for the specified week.")
 
-            return staticSubjects + subjects
+    def getSubjects(self) -> List[Dict[str, str]]:
+        """Get the complete list of subjects, including both static and user-defined subjects."""
+        if not self.isLoggedIn():
+            raise NotLoggedInError("Not logged in. Login first.")
 
-        else:
-            raise NotLoggedInError("not logged in. Login first")
-        
-    def get_art_id_from_text(self, subject_name: str) -> str:
-        subjects = self.getSubjects()  # Retrieve all subjects
+        static_subjects = [
+            {"id": "1", "name": "Betrieb"},
+            {"id": "2", "name": "Schule"},
+            {"id": "3", "name": "ÜBA"},
+            {"id": "4", "name": "Urlaub"},
+            {"id": "5", "name": "Feiertag"},
+            {"id": "6", "name": "Arbeitsunfähig"},
+            {"id": "7", "name": "Frei"},
+        ]
+
+        subject_setup_html = self.session.get(
+            urllib.parse.urljoin(self.BASE_URL, "/Azubi/SetupSchulfach.aspx")
+        ).text
+        soup = BeautifulSoup(subject_setup_html, "html.parser")
+        subject_elements = soup.find(id="divSchulfach").find_all("input")
+
+        dynamic_subjects = [
+            {
+                "id": subject_element.get("data-default"),
+                "name": subject_element.get("value"),
+            }
+            for subject_element in subject_elements
+        ]
+
+        return static_subjects + dynamic_subjects
+
+    def get_art_id_from_text(self, subject_name: str) -> Optional[str]:
+        """Get the subject ID from its name."""
+        subjects = self.getSubjects()
         for subject in subjects:
             if subject_name in subject['name']:
                 return subject['id']
-        return None  # Return None if no match found
+        return None
 
     def writeReports(self, entries: List[Entry]) -> None:
-        """Writes a list of reports to the Azubiheft.
-        - Parameters:
-            entries: List of reports to be written.
-        """
+        """Write a list of reports to the Azubiheft."""
         if not self.isLoggedIn():
-            raise NotLoggedInError("not logged in. Login first")
+            raise NotLoggedInError("Not logged in. Login first.")
 
         headers = {
             "x-my-ajax-request": "ajax",
-            "Origin": "https://www.azubiheft.de",
-            "Referer": "https://www.azubiheft.de/",
+            "Origin": self.BASE_URL,
+            "Referer": self.BASE_URL,
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "Pragma": "no-cache",
             "Cache-Control": "no-cache",
         }
 
         for entry in entries:
             date_str = TimeHelper.dateTimeToString(entry.date)
             week_number = self.getReportWeekId(entry.date)
-            url = f"https://www.azubiheft.de/Azubi/XMLHttpRequest.ashx?Datum={date_str}&BrNr={week_number}&BrSt=1&BrVorh=Yes&T={TimeHelper.getActualTimestamp()}"
+            url = f"{self.BASE_URL}/Azubi/XMLHttpRequest.ashx?Datum={date_str}&BrNr={week_number}&BrSt=1&BrVorh=Yes&T={TimeHelper.getActualTimestamp()}"
 
-            # Convert line breaks in the message to <div> tags for HTML formatting
             formatted_message = (
                 "<div>" + "</div><div>".join(entry.message.split("\n")) + "</div>"
             )
-            # URL-encode the formatted HTML
             encoded_message = urllib.parse.quote(formatted_message)
 
             formData = {
                 "disablePaste": "0",
                 "Seq": "0",
                 "Art_ID": str(entry.type),
                 "Abt_ID": "0",
                 "Dauer": entry.time_spent,
-                "Inhalt": encoded_message,  # Use the URL-encoded HTML message
+                "Inhalt": encoded_message,
                 "jsVer": "12",
             }
 
             response = self.session.post(url, headers=headers, data=formData)
             if response.status_code != 200:
-                print(
+                logger.error(
                     f"Failed to add entry for date {date_str}. Response code: {response.status_code}"
                 )
+            else:
+                logger.info(f"Entry added successfully for date {date_str}.")
 
     def writeReport(
         self, date: datetime, message: str, time_spent: str, entry_type: int
     ) -> None:
-        """Writes a report to the Azubiheft.
-        - Parameters:
-            date: Date of the report.
-            message: Message of the report.
-            time_spent: Time spent on the report.
-            entry_type: Type of the report.
-        """
+        """Write a single report to the Azubiheft."""
         if time_spent.strip() != "00:00":
             entry = Entry(date, message, time_spent, entry_type)
             self.writeReports([entry])
-            
-    def getReport(self, date: datetime, include_formatting: bool = False):
+
+    def getReport(
+        self, date: datetime, include_formatting: bool = False
+    ) -> List[Dict[str, str]]:
+        """Retrieve a report for a given date, optionally including HTML formatting."""
         if not self.isLoggedIn():
-            raise NotLoggedInError("not logged in. Login first")
+            raise NotLoggedInError("Not logged in. Login first.")
 
-        url = (
-            "https://www.azubiheft.de/Azubi/Tagesbericht.aspx?Datum="
-            + TimeHelper.dateTimeToString(date)
-        )
-        reportHtml = self.session.get(url).text
-        soup = BeautifulSoup(reportHtml, "html.parser")
+        url = f"{self.BASE_URL}/Azubi/Tagesbericht.aspx?Datum={TimeHelper.dateTimeToString(date)}"
+        report_html = self.session.get(url).text
+        soup = BeautifulSoup(report_html, "html.parser")
 
         reports = []
-
-        # Find all report entries
         entries = soup.find_all("div", class_="d0 mo")
+
         for entry in entries:
-            # Extract the duration and type of activity
             duration = entry.find("div", class_="row2 d4").get_text(strip=True)
             if duration.strip() == "00:00":
                 continue
             activity_type = (
                 entry.find("div", class_="row1 d3")
                 .get_text(strip=True)
                 .replace("Art: ", "")
             )
-            seq = entry.get("data-seq")  # Extract the sequence number
+            seq = entry.get("data-seq")
 
-            # Extract and format the report text
             report_text_div = entry.find("div", class_="row7 d5")
             if include_formatting:
-                # Replace <br> tags with newline characters
-                for br in report_text_div.find_all("br"):
-                    br.replace_with("\n")
-
-                # Convert <div> tags to newline characters while preserving whitespace
-                report_text_parts = []
-                for element in report_text_div.contents:
-                    if isinstance(element, NavigableString):
-                        report_text_parts.append(str(element))
-                    elif element.name == "div":
-                        report_text_parts.append("\n" + element.get_text(strip=False))
-
-                report_text = "".join(report_text_parts)
-                report_text = re.sub(r"\n+", "\n", report_text.strip())
+                report_text = "".join(
+                    str(e)
+                    for e in report_text_div.contents
+                    if isinstance(e, NavigableString) or e.name == "div"
+                )
+                report_text = re.sub(r"<br\s*/?>", "\n", report_text)
             else:
-                # Concatenate all text without formatting
                 report_text = " ".join(report_text_div.stripped_strings)
 
             reports.append(
                 {
                     "seq": seq,
                     "type": activity_type,
                     "duration": duration,
                     "text": report_text,
                 }
             )
 
-        if len(reports) == 0:
-            print("No Reports")
-        else:
-            return reports
-        
-    def deleteReport(self, date: datetime, entry_number: int = None) -> None:
+        if not reports:
+            logger.info("No reports found for the given date.")
+        return reports
+
+    def deleteReport(self, date: datetime, entry_number: Optional[int] = None) -> None:
+        """Delete one or all reports for a given date."""
         if not self.isLoggedIn():
-            raise NotLoggedInError("not logged in. Login first")
+            raise NotLoggedInError("Not logged in. Login first.")
 
-        # Retrieve the report for the specified date
         report_entries = self.getReport(date)
         if not report_entries:
-            print("No report entries found for this date.")
+            logger.info("No report entries found for this date.")
             return
 
-        if entry_number is None:
-            # Display report entries and ask user which to delete
-            for i, entry in enumerate(report_entries, 1):
-                print(
-                    f"{i}. {entry['type']} - {entry['text']} - {entry['duration']}")
-            print("all. Delete all entries")
-            choice = input(
-                "Select the number of the entry to delete (or 'all' to delete everything): ")
-        else:
-            choice = str(entry_number)
-
-        if choice.isdigit():
-            choice = int(choice) - 1
-            if choice < 0 or choice >= len(report_entries):
-                print("Invalid entry number.")
-                return
-            entries_to_delete = [report_entries[choice]]
-        elif choice == "all":
-            entries_to_delete = report_entries
-        else:
-            print("Invalid choice.")
-            return
-
-        # Retrieve the week number for the specified date
         week_number = self.getReportWeekId(date)
 
         headers = {
-            'x-my-ajax-request': 'ajax',
-            'Origin': 'https://www.azubiheft.de',
-            'Referer': 'https://www.azubiheft.de/',
-            'Sec-Fetch-Dest': 'empty',
-            'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Site': 'same-origin',
-            'Pragma': 'no-cache',
-            'Cache-Control': 'no-cache',
+            "x-my-ajax-request": "ajax",
+            "Origin": self.BASE_URL,
+            "Referer": self.BASE_URL,
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "Pragma": "no-cache",
+            "Cache-Control": "no-cache",
         }
 
-        # Loop through and delete each selected entry
+        entries_to_delete = (
+            report_entries
+            if entry_number is None or entry_number == "all"
+            else [report_entries[entry_number - 1]]
+        )
+
         for entry in entries_to_delete:
             formData = {
                 'disablePaste': '0',
                 'Seq': f"-{entry['seq']}",
                 'Art_ID': self.get_art_id_from_text(entry['type']),
                 'Abt_ID': '0',
                 'Dauer': entry['duration'],
                 'Inhalt': entry['text'],
                 'jsVer': '12'
             }
 
-            url = f"https://www.azubiheft.de/Azubi/XMLHttpRequest.ashx?Datum={TimeHelper.dateTimeToString(
-                date)}&BrNr={week_number}&BrSt=1&BrVorh=Yes&T={TimeHelper.getActualTimestamp()}"
+            url = f"{self.BASE_URL}/Azubi/XMLHttpRequest.ashx?Datum={TimeHelper.dateTimeToString(date)}&BrNr={week_number}&BrSt=1&BrVorh=Yes&T={TimeHelper.getActualTimestamp()}"
 
             response = self.session.post(url, headers=headers, data=formData)
             if response.status_code != 200:
-                print(f"Failed to delete entry: {
-                      entry['text']}. Response code: {response.status_code}")
+                logger.error(
+                    f"Failed to delete entry: {entry['text']}. Response code: {response.status_code}"
+                )
             else:
-                print(f"Entry deleted successfully: {entry['text']}")
-
+                logger.info(f"Entry deleted successfully: {entry['text']}")
 
 
 class TimeHelper:
     @staticmethod
     def dateTimeToString(date: datetime) -> str:
+        """Convert a datetime object to a string in the format YYYYMMDD."""
         return date.strftime("%Y%m%d")
 
     @staticmethod
     def getActualTimestamp() -> str:
+        """Get the current time as a string timestamp."""
         return str(int(time.time()))
 
     @staticmethod
-    def timeDeltaToString(time: timedelta) -> str:
-        maxTime = timedelta(hours=19, minutes=59)
-        if time < maxTime:
-            formatted = ":".join(str(time).split(":")[:2])
-            return formatted
-        else:
-            raise ValueTooLargeError("Max time is " + str(maxTime))
+    def timeDeltaToString(time_delta: timedelta) -> str:
+        """Convert a timedelta object to a string, ensuring it's less than 19:59."""
+        max_time = timedelta(hours=19, minutes=59)
+        if time_delta > max_time:
+            raise ValueTooLargeError(f"Max time is {max_time}")
+        return str(time_delta)[:-3]
```

### Comparing `azubiheftapi-0.0.94/azubiheftApi.egg-info/PKG-INFO` & `azubiheftapi-1.0.0/azubiheftApi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azubiheftApi
-Version: 0.0.94
+Version: 1.0.0
 Summary: Azubiheft.de custom api
 Home-page: https://github.com/leonkohli/azubiheft-api
 Author: Leon Kohlhaussen
 Author-email: kohli.leon@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -61,14 +61,15 @@
 # Delete an existing subject by ID
 azubiheft.delete_subject("subjectId")
 
 # Fetch a report by date
 report = azubiheft.getReport(datetime(2023, 10, 19))
 print(report)
 
+
 # Get a week's report ID
 week_id = azubiheft.getReportWeekId(datetime.now())
 print(week_id)
 
 # Write a new report entry
 azubiheft.writeReport(datetime(2023, 10, 19), "Hello World", "2:00", 1)
 # its also possible to format the text using \n or just like this
@@ -78,14 +79,18 @@
 # """
 
 # Fetch the report again to see changes
 report = azubiheft.getReport(datetime(2023, 10, 19), include_formatting=True)  #  include_formatting=True to include formatting
 print(report)
 
 
+# delete a report entry
+azubiheft.deleteReport(datetime(2023, 10, 19))
+
+
 # Log out from the session
 azubiheft.logout()
 
 # Check login status (should be False after logging out)
 print(azubiheft.isLoggedIn())
```

### Comparing `azubiheftapi-0.0.94/setup.py` & `azubiheftapi-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="azubiheftApi",
-    version="0.0.94",
+    version="1.0.0",
     author="Leon Kohlhaussen",
     author_email="kohli.leon@gmail.com",
     description="Azubiheft.de custom api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leonkohli/azubiheft-api",
     packages=setuptools.find_packages(),
```

