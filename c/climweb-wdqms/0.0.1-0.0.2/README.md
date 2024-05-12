# Comparing `tmp/climweb_wdqms-0.0.1.tar.gz` & `tmp/climweb_wdqms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climweb_wdqms-0.0.1.tar", last modified: Sat May 11 20:02:53 2024, max compression
+gzip compressed data, was "climweb_wdqms-0.0.2.tar", last modified: Sun May 12 01:27:23 2024, max compression
```

## Comparing `climweb_wdqms-0.0.1.tar` & `climweb_wdqms-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:53.292660 climweb_wdqms-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 20:02:53.292660 climweb_wdqms-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:53.292660 climweb_wdqms-0.0.1/climweb_wdqms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 20:02:53.000000 climweb_wdqms-0.0.1/climweb_wdqms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-11 20:02:53.000000 climweb_wdqms-0.0.1/climweb_wdqms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 20:02:53.000000 climweb_wdqms-0.0.1/climweb_wdqms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-11 20:02:53.000000 climweb_wdqms-0.0.1/climweb_wdqms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 20:02:53.000000 climweb_wdqms-0.0.1/climweb_wdqms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:53.288660 climweb_wdqms-0.0.1/climwebwdqms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:53.288660 climweb_wdqms-0.0.1/climwebwdqms/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:53.288660 climweb_wdqms-0.0.1/climwebwdqms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/management/commands/fetch_transmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:53.292660 climweb_wdqms-0.0.1/climwebwdqms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/climwebwdqms/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-11 20:02:49.000000 climweb_wdqms-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-11 20:02:53.292660 climweb_wdqms-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/management/commands/fetch_transmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/climweb_wdqms/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:27:23.854836 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-12 01:27:23.000000 climweb_wdqms-0.0.2/climweb_wdqms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 01:27:17.000000 climweb_wdqms-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-12 01:27:23.858836 climweb_wdqms-0.0.2/setup.cfg
```

### Comparing `climweb_wdqms-0.0.1/PKG-INFO` & `climweb_wdqms-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.1
+Version: 0.0.2
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.1/climweb_wdqms.egg-info/PKG-INFO` & `climweb_wdqms-0.0.2/climweb_wdqms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.1
+Version: 0.0.2
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.1/climweb_wdqms.egg-info/SOURCES.txt` & `climweb_wdqms-0.0.2/climweb_wdqms.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 MANIFEST.in
 pyproject.toml
 setup.cfg
+climweb_wdqms/__init__.py
+climweb_wdqms/admin.py
+climweb_wdqms/apps.py
+climweb_wdqms/models.py
+climweb_wdqms/serializers.py
+climweb_wdqms/tests.py
+climweb_wdqms/urls.py
+climweb_wdqms/views.py
 climweb_wdqms.egg-info/PKG-INFO
 climweb_wdqms.egg-info/SOURCES.txt
 climweb_wdqms.egg-info/dependency_links.txt
 climweb_wdqms.egg-info/requires.txt
 climweb_wdqms.egg-info/top_level.txt
-climwebwdqms/__init__.py
-climwebwdqms/admin.py
-climwebwdqms/apps.py
-climwebwdqms/models.py
-climwebwdqms/serializers.py
-climwebwdqms/tests.py
-climwebwdqms/urls.py
-climwebwdqms/views.py
-climwebwdqms/management/__init__.py
-climwebwdqms/management/commands/__init__.py
-climwebwdqms/management/commands/fetch_transmissions.py
-climwebwdqms/migrations/0001_initial.py
-climwebwdqms/migrations/__init__.py
+climweb_wdqms/management/__init__.py
+climweb_wdqms/management/commands/__init__.py
+climweb_wdqms/management/commands/fetch_transmissions.py
+climweb_wdqms/migrations/0001_initial.py
+climweb_wdqms/migrations/__init__.py
```

### Comparing `climweb_wdqms-0.0.1/climwebwdqms/management/commands/fetch_transmissions.py` & `climweb_wdqms-0.0.2/climweb_wdqms/management/commands/fetch_transmissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime, timedelta
 from django.contrib.gis.geos import Point
 import pandas as pd
 import numpy as np
 
 import requests
 from django.core.management.base import BaseCommand
-from climwebwdqms.models import Station, Transmission
+from climweb_wdqms.models import Station, Transmission
 from adminboundarymanager.models import Country
 
 logger = logging.getLogger(__name__)
 
 # Define the base URL for the WDQMS csv download
 BASE_URL = "https://wdqms.wmo.int/wdqmsapi/v1/download/synop/six_hour/availability"
 
@@ -46,23 +46,26 @@
         with open(file_name, 'wb') as f:
             f.write(response.content)
 
         print(f"DOWNLOAD: {file_name} downloaded successfully.")
         
         # Load the CSV data into a DataFrame
         df = pd.read_csv(file_name)
-        # Group by 'name' and select the row with the highest 'received rate'
-        max_rate_indices = df.groupby('wigosid')['#received'].idxmax()
-        df_filtered = df.loc[max_rate_indices]
-        df_filtered = df_filtered[df_filtered['country code'] == country_code]
+       
+        df_filtered = df[df['country code'] == country_code]
 
+        # Assuming df_filtered is your DataFrame
+        df_filtered = df_filtered.copy()
         df_filtered['received_rate'] = (df_filtered['#received'] / df_filtered['#expected']) * 100
+         # Group by 'name' and select the row with the highest 'received rate'
+        max_rate_indices = df_filtered.groupby('wigosid')['received_rate'].idxmax()
+        df_filtered = df_filtered.loc[max_rate_indices]
         df_filtered.replace([np.inf, -np.inf], 0, inplace=True)
 
-        os.remove(file_name)
+        # os.remove(file_name)
         return df_filtered
 
     else:
         print("Failed to retrieve data. Status code:", response.status_code)
 
 def generate_date_range(start_date, end_date):
     dates = []
@@ -70,22 +73,16 @@
     while current_date <= datetime.strptime(end_date, "%Y-%m-%d"):
         dates.append(current_date.strftime('%Y-%m-%d'))
         current_date += timedelta(days=1)
     return dates
 
 
 def ingest_transmission_rates(start_date, end_date,variable, periods, centers, country_code):
-    # start_date = "2024-01-01" # TODO: USER DEFINED
-    # end_date = "2024-05-01" # TODO: USER DEFINED
     dates = generate_date_range(start_date, end_date)
-    # periods = ["00", "06", "12", "18"] # TODO: USER DEFINED
-    # variable = "pressure" # TODO: USER DEFINED
-    # centers = ["DWD", "ECMWF", "JMA", "NCEP"] # TODO: USER DEFINED
     baseline = "OSCAR" 
-    # country_code = "KEN" # TODO: USER DEFINED
 
     for date in dates:
         for period in periods:
             trans_rates = download_transmission_rate_csv(date, period, variable, centers, baseline, country_code)
 
             print(f"INGEST: Starting data ingestion for {date}-{period}")
 
@@ -108,23 +105,27 @@
             # Create or update transmissions
             transmissions_to_create = []
             for _, row in trans_rates.iterrows():
 
                 if Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).exists():
                     transmission_data = {
                         'received_rate':row['received_rate'],
+                        'received':row['#received'],
+                        'expected':row['#expected'],
                     }
                     Transmission.objects.filter(station=row['wigosid'], variable=row['variable'], received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')).update(**transmission_data)
 
                 else:
                     station = Station.objects.get(wigos_id=row['wigosid'])
                     transmissions_to_create.append(Transmission(
                         station=station,
                         variable=row['variable'],
                         received_rate=row['received_rate'],
+                        received=row['#received'],
+                        expected=row['#expected'],
                         received_date=datetime.strptime(row['date'],'%Y-%m-%d %H:%M:%S%z')
                     ))
 
             # Bulk create new transmissions
             Transmission.objects.bulk_create(transmissions_to_create, ignore_conflicts=True)
             
             print(f"INGEST: Completed ingestion for {date}-{period}")
@@ -168,45 +169,51 @@
                 self.stderr.write(self.style.ERROR(f"Invalid format for 'start_date'. Use YYYY-MM-DD format."))
                 return  # Exit the command
 
         if end_date:  
             if not date_pattern.match(end_date):
                 self.stderr.write(self.style.ERROR(f"Invalid format for 'end_date'. Use YYYY-MM-DD format."))
                 return  # Exit the command
+            
+        if datetime.strptime(start_date, "%Y-%m-%d") > datetime.strptime(end_date, "%Y-%m-%d"):
+            self.stderr.write(self.style.ERROR(f"'Start date' cannot come earlier than 'End date'"))
+            return  # Exit the command
+
 
         if variable:
             if variable not in variables_ls:
                 self.stderr.write(self.style.ERROR(f"Allowed variables include pressure,temperature, humidity, meridional_wind, zonal_wind"))
                 return  # Exit the command
 
             # Split the value by comma and append to list_arg
-        print(periods)
         if periods:
             for period in periods:
                 if period not in period_ls:
                     self.stderr.write(self.style.ERROR(f"'{period}' is not a valid option. Choices are 00 06 12 18"))
                     return  # Exit the command
             
         if centers:
             for center in centers:
                 if center.upper() not in center_ls:
                     self.stderr.write(self.style.ERROR(f"'{center}' is not a valid option. Choices are DWD ECMWF JMA NCEP"))
                     return  # Exit the command
+                
+            
 
 
         if start_date and end_date and variable and centers and periods:
             for country in Country.objects.all():
-                # loop through all countries in boundary manager for data fetching and ingestion
-                self.stdout.write(f"FETCH: Requesting data for {country.country.name}")
+                if Country.objects.count() > 0:
+                    # loop through all countries in boundary manager for data fetching and ingestion
+                    self.stdout.write(f"FETCH: Requesting data for {country.country.name}")
+
+                    ingest_transmission_rates(start_date, end_date, variable, periods, centers, country.country.alpha3)
+                else:
+                    self.stderr.write(self.style.ERROR(f"Please select atleast one country in admin boundary settings first"))
 
-                ingest_transmission_rates(start_date, end_date, variable, periods, centers, country.country.alpha3)
-        
-        # else:
-        #     self.stderr.write(self.style.ERROR("Missing arguements for start_date, end_date, centers, variables, periods"))
-        #     return
```

### Comparing `climweb_wdqms-0.0.1/climwebwdqms/migrations/0001_initial.py` & `climweb_wdqms-0.0.2/climweb_wdqms/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.11 on 2024-05-10 00:03
+# Generated by Django 4.2.11 on 2024-05-12 00:08
 
 import django.contrib.gis.db.models.fields
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
@@ -27,17 +27,19 @@
             },
         ),
         migrations.CreateModel(
             name='Transmission',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('variable', models.CharField(max_length=50, verbose_name='Transmission Variable')),
-                ('received_rate', models.DecimalField(decimal_places=2, max_digits=5, verbose_name='Percentage received')),
+                ('received', models.IntegerField(null=True, verbose_name='Transmissions received')),
+                ('expected', models.IntegerField(null=True, verbose_name='Transmissions expected')),
+                ('received_rate', models.DecimalField(decimal_places=2, max_digits=5, verbose_name='Transmission Rate')),
                 ('received_date', models.DateTimeField(verbose_name='Date Time Received')),
-                ('station', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='climwebwdqms.station')),
+                ('station', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='climweb_wdqms.station')),
             ],
             options={
                 'verbose_name': 'Transmission',
                 'verbose_name_plural': 'Transmissions',
             },
         ),
     ]
```

### Comparing `climweb_wdqms-0.0.1/climwebwdqms/models.py` & `climweb_wdqms-0.0.2/climweb_wdqms/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     
         
 # Create your models here.
 class Transmission(models.Model):
 
     station = models.ForeignKey("Station", on_delete=models.CASCADE)
     variable = models.CharField(_("Transmission Variable"), max_length=50 )
-    received_rate = models.DecimalField(_("Percentage received"), max_digits=5, decimal_places=2)
+    received = models.IntegerField(_("Transmissions received"), null=True)
+    expected = models.IntegerField(_("Transmissions expected"), null=True)
+    received_rate = models.DecimalField(_("Transmission Rate"), max_digits=5, decimal_places=2)
     received_date = models.DateTimeField(_("Date Time Received"), auto_now=False, auto_now_add=False)
 
 
         
     class Meta:
         verbose_name = _("Transmission")
         verbose_name_plural = _("Transmissions")
```

### Comparing `climweb_wdqms-0.0.1/climwebwdqms/serializers.py` & `climweb_wdqms-0.0.2/climweb_wdqms/serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rest_framework import serializers
 
-from climwebwdqms.models import Transmission, Station
+from climweb_wdqms.models import Transmission, Station
 
 
 class StationSerializer(serializers.ModelSerializer):
     geom = serializers.SerializerMethodField()
 
     class Meta:
         model = Station
@@ -12,9 +12,9 @@
 
     def get_geom(self, obj):
         return obj.geom
 
 class TransmissionSerializer(serializers.ModelSerializer):
     class Meta:
         model = Transmission
-        fields = ["received_date", "station", "variable", "received_rate"]
+        fields = ["received_date", "station", "variable", "received_rate", "recieved", "expected"]
```

### Comparing `climweb_wdqms-0.0.1/climwebwdqms/urls.py` & `climweb_wdqms-0.0.2/climweb_wdqms/urls.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.1/climwebwdqms/views.py` & `climweb_wdqms-0.0.2/climweb_wdqms/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 from django.shortcuts import render
+import pytz
+
 from rest_framework.generics import ListAPIView
-from climwebwdqms.models import Transmission, Station
+from climweb_wdqms.models import Transmission, Station
 from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework.permissions import BasePermission, IsAuthenticated, SAFE_METHODS
-from climwebwdqms.serializers import TransmissionSerializer, StationSerializer
-from datetime import date, timedelta, datetime
-from dateutil import parser
+from climweb_wdqms.serializers import StationSerializer
+from datetime import datetime
 from rest_framework.views import APIView
 from rest_framework.response import Response
-from django.db.models.functions import TruncMonth
-from django.db.models import Count
 from django.db.models.functions import ExtractHour,ExtractMonth,ExtractYear
 from django.db.models import Avg
 
+
+def validate_params(query_params, supported_params):
+    # Check for unsupported parameters
+    error_message = None
+    unsupported_params = [param for param in query_params.keys() if param not in supported_params]
+    
+    # If there are unsupported parameters, return an error response
+    if unsupported_params:
+        error_message = {'error': f'Unsupported parameter(s): {", ".join(unsupported_params)}. Only Supports {", ".join(supported_params)}'}
+        # return Response(error_message, status=400)  # Return a 400 Bad Request response
+    
+
+    # Check if the 'param' parameter is present in the request
+    for q in supported_params:
+        if q not in query_params:
+            error_message = {'error': f'Parameter "{q}" is required.'}
+            # return Response(error_message, status=400)  # Return a 400 Bad Request response
+
+
+    return error_message
+
 class ReadOnly(BasePermission):
     def has_permission(self, request, view):
         return request.method in SAFE_METHODS
     
 
 class StationListView(ListAPIView):
     queryset = Station.objects.all()
@@ -32,74 +52,92 @@
     
 # Create your views here.
 class SynopTransmissionView(APIView):
     filter_backends = [DjangoFilterBackend]
     filterset_fields = ["received_date", "station", "variable"]
     permission_classes = [IsAuthenticated | ReadOnly]
 
+    
+
     def get(self, request):
+        
         queryset = Transmission.objects.all()
+        supported_params = ['station', 'frequency', 'received_date', 'variable']
+        query_params = request.query_params
+        
+        validate = validate_params(query_params, supported_params)
+
+        if validate:
+            return Response(validate, status=400)  # Return a 400 Bad Request response
 
         # query parameters 
         station = request.query_params.get('station', None)
         frequency = request.query_params.get('frequency', None)
         received_date = request.query_params.get('received_date', queryset.order_by('received_date').values_list('received_date').last()[0].strftime("%Y-%m-%dT%H:%M:%SZ"))
-        
         variable = request.query_params.get('variable', 'pressure')
-        frequency = request.query_params.get('frequency', None)
 
         result = []
 
         if station:
             queryset = queryset.filter(station = station)
 
         if received_date:
-            received_date = datetime.strptime(f"{received_date}", "%Y-%m-%dT%H:%M:%SZ")
+            received_date = datetime.strptime(f"{received_date}T00:00:00Z", "%Y-%m-%dT%H:%M:%SZ").replace(tzinfo=pytz.UTC)
 
             # check the frequencies 
             if frequency == 'monthly_synop':
                 queryset = queryset.filter(received_date__month = received_date.month, variable=variable).order_by('received_date__hour')
             
             elif frequency == 'daily_synop':
-                queryset = queryset.filter(received_date__day=received_date.day, variable=variable).order_by('received_date__hour')
+                queryset = queryset.filter(received_date__date=received_date.date(), variable=variable).order_by('received_date__hour')
             elif frequency == 'yearly_synop':
                 queryset = queryset.filter(received_date__year = received_date.year, variable=variable).order_by('received_date__hour')
 
         # Extract the hour from the received_date and annotate the queryset
         queryset = queryset.annotate(
             synop_hour=ExtractHour('received_date')
         )
 
         # Aggregate the queryset to calculate the average received_rate for each synoptic hour
         queryset = queryset.values('synop_hour').annotate(
-            avg_received_rate=Avg('received_rate')
+            avg_received_rate=Avg('received_rate'),
+            avg_received=Avg('received'),
+            avg_expected=Avg('expected'),
         )
 
         # Format the result
         result = [
             {
                 'synop_hour': str(hour).zfill(2),  # Format hour to have leading zero if needed
-                'avg_received_rate': round(avg_rate, 0) if avg_rate else None  # Round to 2 decimal places
+                'avg_received_rate': round(avg_rate, 0), # Round to 0 decimal places
+                'avg_received': round(avg_received, 0),  # Round to 0 decimal places
+                'avg_expected': round(avg_expected, 0)  # Round to 0 decimal places
             }
-            for hour, avg_rate in queryset.values_list('synop_hour', 'avg_received_rate')
+            for hour, avg_rate, avg_received, avg_expected in queryset.values_list('synop_hour', 'avg_received_rate','avg_received', 'avg_expected' )
         ] 
             
         # Return response
         return Response(result)
 
 
 class MonthlyTransmissionView(APIView):
 
     def get(self, request):
 
         queryset = Transmission.objects.all()
         result = []
 
         latest_year =  queryset.values_list('received_date__year').order_by('received_date__year').last()
+        supported_params = ['station', 'year', 'variable']
 
+        validate = validate_params(request.query_params, supported_params)
+
+        if validate:
+            return Response(validate, status=400)  # Return a 400 Bad Request response
+        
         # query params 
         station = request.query_params.get('station', None)
         year = request.query_params.get('year', latest_year[0] if len(latest_year) else None)
         variable = request.query_params.get('variable', 'pressure')
 
         if station:
             queryset = queryset.filter(station = station)
@@ -107,81 +145,78 @@
         # Extract the month from the received_date and annotate the queryset
         queryset = queryset.filter(variable=variable, received_date__year=year).annotate(
             month=ExtractMonth('received_date')
         )
 
         # Aggregate the queryset to calculate the average received_rate for each month
         monthly_averages = queryset.values('month').order_by('received_date__month').annotate(
-            avg_received_rate=Avg('received_rate')
+            avg_received_rate=Avg('received_rate'),
+            avg_received=Avg('received'),
+            avg_expected=Avg('expected'),
         )
 
         # Map month numbers to month names
         MONTH_NAMES = {
             1: 'January', 2: 'February', 3: 'March', 4: 'April',
             5: 'May', 6: 'June', 7: 'July', 8: 'August',
             9: 'September', 10: 'October', 11: 'November', 12: 'December'
         }
         # Format the result
         result = [
             {
                 'month': MONTH_NAMES[month],
-                'avg_received_rate': round(avg_rate, 2) if avg_rate else None  # Round to 2 decimal places
+                'avg_received_rate': round(avg_rate, 0),  # Round to 0 decimal places
+                'avg_received': round(avg_received, 0),  # Round to 0 decimal places
+                'avg_expected': round(avg_expected, 0)  # Round to 0 decimal places
             }
-            for month, avg_rate in monthly_averages.values_list('month', 'avg_received_rate')
+            for month, avg_rate, avg_received, avg_expected in monthly_averages.values_list('month', 'avg_received_rate','avg_received', 'avg_expected')
         ]
 
         return Response(result)
 
 
 class YearlyTransmissionView(APIView):
 
     def get(self, request):
 
         queryset = Transmission.objects.all()
         result = []
 
+        supported_params = ['station', 'variable']
+
+        validate = validate_params(request.query_params, supported_params)
+
+        if validate:
+            return Response(validate, status=400)  # Return a 400 Bad Request response
+
         # query params 
         station = request.query_params.get('station', None)
         variable = request.query_params.get('variable', 'pressure')
+        
 
         if station:
             queryset = queryset.filter(station = station)
 
         # Extract the month from the received_date and annotate the queryset
         queryset = queryset.annotate(
             year=ExtractYear('received_date')
         )
 
         # Aggregate the queryset to calculate the average received_rate for each month
         yearly_averages = queryset.values('year').order_by('received_date__year').annotate(
-            avg_received_rate=Avg('received_rate')
+            avg_received_rate=Avg('received_rate'),
+            avg_received=Avg('received'),
+            avg_expected=Avg('expected'),
         )
 
         # Format the result
         result = [
             {
                 'year': year,
-                'avg_received_rate': round(avg_rate, 2) if avg_rate else None  # Round to 2 decimal places
+                'avg_received_rate': round(avg_rate, 0),  # Round to 0 decimal places
+                'avg_received': round(avg_received, 0), # Round to 0 decimal places
+                'avg_expected': round(avg_expected, 0)  # Round to 0 decimal places
             }
-            for year, avg_rate in yearly_averages.values_list('year', 'avg_received_rate')
+            for year, avg_rate, avg_received, avg_expected in yearly_averages.values_list('year', 'avg_received_rate','avg_received', 'avg_expected')
         ]
 
         return Response(result)
-
-
-
-
-        
-
-
-
-
-
-
-
-
-
-        return Response(result)
-
-
-
-
```

### Comparing `climweb_wdqms-0.0.1/setup.cfg` & `climweb_wdqms-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climweb-wdqms
-version = 0.0.1
+version = 0.0.2
 description = National level WDQMS Summary tool
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/climweb-wdqms
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

