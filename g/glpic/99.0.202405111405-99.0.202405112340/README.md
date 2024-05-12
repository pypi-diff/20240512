# Comparing `tmp/glpic-99.0.202405111405.tar.gz` & `tmp/glpic-99.0.202405112340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405111405.tar", last modified: Sat May 11 14:05:59 2024, max compression
+gzip compressed data, was "glpic-99.0.202405112340.tar", last modified: Sat May 11 23:40:55 2024, max compression
```

## Comparing `glpic-99.0.202405111405.tar` & `glpic-99.0.202405112340.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:05:59.388721 glpic-99.0.202405111405/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 14:05:59.388721 glpic-99.0.202405111405/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 14:05:45.000000 glpic-99.0.202405111405/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:05:59.384721 glpic-99.0.202405111405/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-11 14:05:45.000000 glpic-99.0.202405111405/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-11 14:05:45.000000 glpic-99.0.202405111405/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:05:59.388721 glpic-99.0.202405111405/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:05:59.388721 glpic-99.0.202405111405/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-11 14:05:59.000000 glpic-99.0.202405111405/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:40:55.876735 glpic-99.0.202405112340/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 23:40:55.876735 glpic-99.0.202405112340/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 23:40:43.000000 glpic-99.0.202405112340/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:40:55.876735 glpic-99.0.202405112340/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-05-11 23:40:43.000000 glpic-99.0.202405112340/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-11 23:40:43.000000 glpic-99.0.202405112340/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:40:55.876735 glpic-99.0.202405112340/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:40:55.876735 glpic-99.0.202405112340/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-11 23:40:55.000000 glpic-99.0.202405112340/setup.py
```

### Comparing `glpic-99.0.202405111405/README.md` & `glpic-99.0.202405112340/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405111405/glpic/__init__.py` & `glpic-99.0.202405112340/glpic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         url = f'{self.base_url}/search/Computer?{search_data}&uid_cols'
         if overrides.get('uid', False):
             url += '&forcedisplay[0]=2'
         computers = _get(url, headers=self.headers)
         return computers['data'] if 'data' in computers else []
 
     def info_reservation(self, reservation):
-        return _get(f'{self.base_url}/Reservation/{reservation}', headers=self.headers)
+        return _get(f'{self.base_url}/ReservationItem/{reservation}', headers=self.headers)
 
     def list_reservations(self, overrides={}):
         user = overrides.get('user') or self.user
         response = _get(f'{self.base_url}/Reservation', headers=self.headers)
         user_id = self.get_user(user)['id']
         return [r for r in response if r['users_id'] == user_id]
 
@@ -202,20 +202,21 @@
     def create_reservation(self, computer, overrides):
         overrides['begin'] = parse(str(datetime.now())).strftime('%Y-%m-%d %H:%M:%S')
         if 'end' not in overrides:
             overrides['end'] = date.today() + timedelta(days=30)
         user = overrides.get('user', self.user)
         if 'users_id' not in overrides:
             user_id = self.get_user(user)['id']
-            overrides['users_id'] = str(user_id)
+            overrides['users_id'] = user_id
         overrides['end'] = parse(str(overrides['end'])).strftime('%Y-%m-%d 00:00:00')
         if 'comment' not in overrides:
             overrides['comment'] = f'reservation for {user}'
-        reservation_id = self.info_computer({'computer': computer, 'uid': True})[0]['Computer.id']
-        overrides['reservationitems_id'] = str(reservation_id)
+        computer_id = self.info_computer({'computer': computer, 'uid': True})[0]['Computer.id']
+        reservationitem_id = self.get_reservation_item_id(computer_id)
+        overrides['reservationitems_id'] = reservationitem_id
         valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys())
         wrong_keys = [key for key in overrides if key not in valid_keys]
         if wrong_keys:
             error(f"Ignoring keys {','.join(wrong_keys)}")
             for key in wrong_keys:
                 del overrides[key]
         if not overrides:
@@ -256,7 +257,14 @@
         data = {'input': overrides}
         if self.debug:
             base_curl = curl_base(self.headers)
             msg = f"{base_curl} -X PUT -Lk {self.base_url}/Reservation/{reservation} -d '{json.dumps(data)}'"
             print(msg)
         result = _put(f'{self.base_url}/Reservation/{reservation}', self.headers, data)
         return result
+
+    def get_reservation_item_id(self, computer_id):
+        url = f'{self.base_url}/ReservationItem?uid_cols'
+        reservation_items = _get(url, headers=self.headers)
+        for entry in reservation_items:
+            if entry['itemtype'] == 'Computer' and entry['items_id'] == computer_id:
+                return entry['id']
```

### Comparing `glpic-99.0.202405111405/glpic/cli.py` & `glpic-99.0.202405112340/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405111405/setup.py` & `glpic-99.0.202405112340/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405111405',
+    version='99.0.202405112340',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```
