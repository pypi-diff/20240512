# Comparing `tmp/persiantools-4.0.0.tar.gz` & `tmp/persiantools-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persiantools-4.0.0.tar", last modified: Sun Mar 24 15:58:11 2024, max compression
+gzip compressed data, was "persiantools-4.0.2.tar", last modified: Sun May 12 16:16:21 2024, max compression
```

## Comparing `persiantools-4.0.0.tar` & `persiantools-4.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:58:11.175681 persiantools-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-24 15:58:06.000000 persiantools-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-24 15:58:06.000000 persiantools-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-03-24 15:58:11.175681 persiantools-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-03-24 15:58:06.000000 persiantools-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:58:11.171681 persiantools-4.0.0/persiantools/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-24 15:58:06.000000 persiantools-4.0.0/persiantools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-24 15:58:06.000000 persiantools-4.0.0/persiantools/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-24 15:58:06.000000 persiantools-4.0.0/persiantools/digits.py
--rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-03-24 15:58:06.000000 persiantools-4.0.0/persiantools/jdatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-24 15:58:06.000000 persiantools-4.0.0/persiantools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:58:11.175681 persiantools-4.0.0/persiantools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-03-24 15:58:11.000000 persiantools-4.0.0/persiantools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-24 15:58:11.000000 persiantools-4.0.0/persiantools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 15:58:11.000000 persiantools-4.0.0/persiantools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 15:58:11.000000 persiantools-4.0.0/persiantools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 15:58:11.000000 persiantools-4.0.0/persiantools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-24 15:58:11.000000 persiantools-4.0.0/persiantools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-24 15:58:06.000000 persiantools-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 15:58:11.175681 persiantools-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-24 15:58:06.000000 persiantools-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 15:58:11.175681 persiantools-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-24 15:58:06.000000 persiantools-4.0.0/tests/test_characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-03-24 15:58:06.000000 persiantools-4.0.0/tests/test_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-03-24 15:58:06.000000 persiantools-4.0.0/tests/test_jalalidate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-03-24 15:58:06.000000 persiantools-4.0.0/tests/test_jalalidatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-24 15:58:06.000000 persiantools-4.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:16:21.697750 persiantools-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-12 16:16:16.000000 persiantools-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 16:16:16.000000 persiantools-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-12 16:16:21.697750 persiantools-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-12 16:16:16.000000 persiantools-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:16:21.697750 persiantools-4.0.2/persiantools/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-12 16:16:16.000000 persiantools-4.0.2/persiantools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-12 16:16:16.000000 persiantools-4.0.2/persiantools/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-12 16:16:16.000000 persiantools-4.0.2/persiantools/digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39541 2024-05-12 16:16:16.000000 persiantools-4.0.2/persiantools/jdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-12 16:16:16.000000 persiantools-4.0.2/persiantools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:16:21.697750 persiantools-4.0.2/persiantools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-12 16:16:21.000000 persiantools-4.0.2/persiantools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-12 16:16:21.000000 persiantools-4.0.2/persiantools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:16:21.000000 persiantools-4.0.2/persiantools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:16:21.000000 persiantools-4.0.2/persiantools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-12 16:16:21.000000 persiantools-4.0.2/persiantools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 16:16:21.000000 persiantools-4.0.2/persiantools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-12 16:16:16.000000 persiantools-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:16:21.697750 persiantools-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-12 16:16:16.000000 persiantools-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:16:21.697750 persiantools-4.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-12 16:16:16.000000 persiantools-4.0.2/tests/test_characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-12 16:16:16.000000 persiantools-4.0.2/tests/test_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-05-12 16:16:16.000000 persiantools-4.0.2/tests/test_jalalidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-05-12 16:16:16.000000 persiantools-4.0.2/tests/test_jalalidatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-12 16:16:16.000000 persiantools-4.0.2/tests/test_utils.py
```

### Comparing `persiantools-4.0.0/LICENSE` & `persiantools-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/PKG-INFO` & `persiantools-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persiantools
-Version: 4.0.0
+Version: 4.0.2
 Summary: Jalali date and datetime with other tools
 Home-page: https://github.com/majiidd/persiantools
 Author: Majid Hajiloo
 Author-email: majid.hajiloo@gmail.com
 License: MIT
 Keywords: jalali shamsi persian digits characters converter jalalidate jalalidatetime date datetime jdate jdatetime farsi
 Classifier: Intended Audience :: Developers
```

### Comparing `persiantools-4.0.0/README.md` & `persiantools-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/persiantools/__init__.py` & `persiantools-4.0.2/persiantools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 #    / __ \/ _ \/ ___/ ___/ / __ `/ __ \/ __/ __ \/ __ \/ / ___/
 #   / /_/ /  __/ /  (__  ) / /_/ / / / / /_/ /_/ / /_/ / (__  )
 #  / .___/\___/_/  /____/_/\__,_/_/ /_/\__/\____/\____/_/____/
 # /_/
 
 __title__ = "persiantools"
 __url__ = "https://github.com/majiidd/persiantools"
-__version__ = "4.0.0"
+__version__ = "4.0.2"
 __build__ = __version__
 __author__ = "Majid Hajiloo"
 __author_email__ = "majid.hajiloo@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2016-2024 Majid Hajiloo"
```

### Comparing `persiantools-4.0.0/persiantools/characters.py` & `persiantools-4.0.2/persiantools/characters.py`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/persiantools/digits.py` & `persiantools-4.0.2/persiantools/digits.py`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/persiantools/jdatetime.py` & `persiantools-4.0.2/persiantools/jdatetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,71 +261,62 @@
             jalali_month = 7 + days // 30
             jalali_day = 1 + (days % 30)
 
         return cls(jalali_year, jalali_month, jalali_day)
 
     def to_gregorian(self):
         """based on jdf.scr.ir"""
+        year = self.year + 1595
         month = self.month
         day = self.day
-        year = self.year
 
-        # Determine the Gregorian year
-        gregorian_year = 621 if year <= 979 else 1600
-        year -= 0 if year <= 979 else 979
-
-        # Calculate the number of days
-        days_in_month = (month - 1) * 31 if month < 7 else ((month - 7) * 30) + 186
-        days = (365 * year) + (year // 33) * 8 + ((year % 33) + 3) // 4
-        days += 78 + day + days_in_month
+        # Calculate the total number of days
+        days = -355668 + (365 * year) + ((year // 33) * 8) + (((year % 33) + 3) // 4) + day
+        if month < 7:
+            days += (month - 1) * 31
+        else:
+            days += ((month - 7) * 30) + 186
 
-        gregorian_year += 400 * (days // 146097)
+        # Determine the Gregorian year
+        gregorian_year = 400 * (days // 146097)
         days %= 146097
 
         if days > 36524:
             days -= 1
             gregorian_year += 100 * (days // 36524)
             days %= 36524
-
             if days >= 365:
                 days += 1
 
         gregorian_year += 4 * (days // 1461)
         days %= 1461
-        gregorian_year += (days - 1) // 365
-
         if days > 365:
+            gregorian_year += (days - 1) // 365
             days = (days - 1) % 365
 
         gregorian_day = days + 1
 
+        # Handle leap years for February day count adjustment
+        if (gregorian_year % 4 == 0 and gregorian_year % 100 != 0) or (gregorian_year % 400 == 0):
+            feb_days = 29
+        else:
+            feb_days = 28
+
         # Days in each month of the Gregorian calendar
-        gregorian_days_in_month = [
-            0,
-            31,
-            29 if (gregorian_year % 4 == 0 and gregorian_year % 100 != 0) or gregorian_year % 400 == 0 else 28,
-            31,
-            30,
-            31,
-            30,
-            31,
-            31,
-            30,
-            31,
-            30,
-            31,
-        ]
+        gregorian_days_in_month = [0, 31, feb_days, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
         # Determine the Gregorian month
-        for _gregorian_month, g in enumerate(gregorian_days_in_month):
-            if gregorian_day <= g:
+        gregorian_month = 1
+        for days_in_month in gregorian_days_in_month[1:]:
+            if gregorian_day <= days_in_month:
                 break
-            gregorian_day -= g
+            gregorian_day -= days_in_month
+            gregorian_month += 1
 
-        return date(gregorian_year, _gregorian_month, gregorian_day)
+        return date(gregorian_year, gregorian_month, gregorian_day)
 
     @classmethod
     def today(cls):
         return cls(date.today())
 
     def timetuple(self):
         "Return local time tuple compatible with time.localtime()."
```

### Comparing `persiantools-4.0.0/persiantools.egg-info/PKG-INFO` & `persiantools-4.0.2/persiantools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persiantools
-Version: 4.0.0
+Version: 4.0.2
 Summary: Jalali date and datetime with other tools
 Home-page: https://github.com/majiidd/persiantools
 Author: Majid Hajiloo
 Author-email: majid.hajiloo@gmail.com
 License: MIT
 Keywords: jalali shamsi persian digits characters converter jalalidate jalalidatetime date datetime jdate jdatetime farsi
 Classifier: Intended Audience :: Developers
```

### Comparing `persiantools-4.0.0/setup.py` & `persiantools-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/tests/test_characters.py` & `persiantools-4.0.2/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/tests/test_digits.py` & `persiantools-4.0.2/tests/test_digits.py`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/tests/test_jalalidate.py` & `persiantools-4.0.2/tests/test_jalalidate.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,20 @@
         self.assertEqual(JalaliDate(1400, 6, 31).to_gregorian(), date(2021, 9, 22))
         self.assertEqual(JalaliDate(1396, 7, 27).to_gregorian(), date(2017, 10, 19))
         self.assertEqual(JalaliDate(1397, 11, 29).to_gregorian(), date(2019, 2, 18))
         self.assertEqual(JalaliDate(1399, 11, 23).to_gregorian(), date(2021, 2, 11))
         self.assertEqual(JalaliDate(1400, 4, 25).to_gregorian(), date(2021, 7, 16))
         self.assertEqual(JalaliDate(1400, 12, 20).to_gregorian(), date(2022, 3, 11))
         self.assertEqual(JalaliDate(1403, 1, 5).to_gregorian(), date(2024, 3, 24))
+        self.assertEqual(JalaliDate(1390, 10, 11).to_gregorian(), date(2012, 1, 1))
+        self.assertEqual(JalaliDate(1398, 10, 11).to_gregorian(), date(2020, 1, 1))
+        self.assertEqual(JalaliDate(1402, 10, 11).to_gregorian(), date(2024, 1, 1))
+        self.assertEqual(JalaliDate(1402, 10, 10).to_gregorian(), date(2023, 12, 31))
+        self.assertEqual(JalaliDate(1403, 10, 11).to_gregorian(), date(2024, 12, 31))
+        self.assertEqual(JalaliDate(1403, 2, 23).to_gregorian(), date(2024, 5, 12))
 
         self.assertEqual(JalaliDate.today().to_gregorian(), date.today())
 
     def test_gregorian_to_shamsi(self):
         self.assertEqual(JalaliDate(date(1988, 5, 4)), JalaliDate(1367, 2, 14))
         self.assertEqual(JalaliDate(date(2122, 1, 31)), JalaliDate(1500, 11, 11))
         self.assertEqual(JalaliDate(date(2017, 3, 20)), JalaliDate(1395, 12, 30))
@@ -36,14 +42,21 @@
         self.assertEqual(JalaliDate.to_jalali(1990, 9, 23), JalaliDate(1369, 7, 1))
         self.assertEqual(JalaliDate.to_jalali(1990, 9, 23), JalaliDate(1369, 7, 1))
         self.assertEqual(JalaliDate.to_jalali(2013, 9, 16), JalaliDate(1392, 6, 25))
         self.assertEqual(JalaliDate.to_jalali(2018, 3, 20), JalaliDate(1396, 12, 29))
         self.assertEqual(JalaliDate.to_jalali(2021, 2, 11), JalaliDate(1399, 11, 23))
         self.assertEqual(JalaliDate.to_jalali(2021, 7, 16), JalaliDate(1400, 4, 25))
         self.assertEqual(JalaliDate.to_jalali(2024, 3, 24), JalaliDate(1403, 1, 5))
+        self.assertEqual(JalaliDate.to_jalali(2012, 1, 1), JalaliDate(1390, 10, 11))
+        self.assertEqual(JalaliDate.to_jalali(2020, 1, 1), JalaliDate(1398, 10, 11))
+        self.assertEqual(JalaliDate.to_jalali(2024, 1, 1), JalaliDate(1402, 10, 11))
+        self.assertEqual(JalaliDate.to_jalali(2024, 1, 1), JalaliDate(1402, 10, 11))
+        self.assertEqual(JalaliDate.to_jalali(2023, 12, 31), JalaliDate(1402, 10, 10))
+        self.assertEqual(JalaliDate.to_jalali(2024, 12, 31), JalaliDate(1403, 10, 11))
+        self.assertEqual(JalaliDate.to_jalali(2024, 5, 12), JalaliDate(1403, 2, 23))
 
         self.assertEqual(JalaliDate(date.today()), JalaliDate.today())
 
     def test_checkdate(self):
         self.assertEqual(JalaliDate.check_date(1367, 2, 14), True)
         self.assertEqual(JalaliDate.check_date(1395, 12, 30), True)
         self.assertEqual(JalaliDate.check_date(1394, 12, 30), False)
```

### Comparing `persiantools-4.0.0/tests/test_jalalidatetime.py` & `persiantools-4.0.2/tests/test_jalalidatetime.py`

 * *Files identical despite different names*

### Comparing `persiantools-4.0.0/tests/test_utils.py` & `persiantools-4.0.2/tests/test_utils.py`

 * *Files identical despite different names*

