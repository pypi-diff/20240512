# Comparing `tmp/opsys-spectrometer-0.0.1.tar.gz` & `tmp/opsys-spectrometer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Z:\opt\atlassian\pipelines\agent\build\dist\.tmp-tpphmtq_\opsys-spectrometer-0.0.1.tar", last modified: Thu May  2 17:22:53 2024, max compression
+gzip compressed data, was "Z:\opt\atlassian\pipelines\agent\build\dist\.tmp-1cnagpra\opsys-spectrometer-0.0.2.tar", last modified: Sun May 12 10:43:30 2024, max compression
```

## Comparing `opsys-spectrometer-0.0.1.tar` & `opsys-spectrometer-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      376 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1834 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer/
--rw-rw-rw-   0        0        0      118 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/opsys_spectrometer/__init__.py
--rw-rw-rw-   0        0        0   392192 2024-05-02 17:22:35.000000 opsys-spectrometer-0.0.1/opsys_spectrometer/avaspecx64.dll
--rw-rw-rw-   0        0        0      412 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/opsys_spectrometer/spectrometer_abstract.py
--rw-rw-rw-   0        0        0     4356 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/opsys_spectrometer/spectrometer_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/
--rw-rw-rw-   0        0        0      376 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-02 17:22:52.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      610 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1095 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:53.000000 opsys-spectrometer-0.0.1/test/
--rw-rw-rw-   0        0        0       78 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0     2411 2024-05-02 17:22:34.000000 opsys-spectrometer-0.0.1/test/test_spectrometer.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      376 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1834 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/
+-rw-rw-rw-   0        0        0      118 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/__init__.py
+-rw-rw-rw-   0        0        0   392192 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/avaspecx64.dll
+-rw-rw-rw-   0        0        0      551 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_abstract.py
+-rw-rw-rw-   0        0        0     4603 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/
+-rw-rw-rw-   0        0        0      376 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 10:43:29.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      610 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/test/
+-rw-rw-rw-   0        0        0       78 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0     2686 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/test/test_spectrometer.py
```

### Comparing `opsys-spectrometer-0.0.1/LICENSE` & `opsys-spectrometer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.1/README.md` & `opsys-spectrometer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.1/opsys_spectrometer/avaspecx64.dll` & `opsys-spectrometer-0.0.2/opsys_spectrometer/avaspecx64.dll`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.1/opsys_spectrometer/spectrometer_controller.py` & `opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,39 +56,42 @@
     def get_peak_value(self):
         """
         Get max measured value
 
         Returns:
             float: max measured value
         """
-        return max(self.data)
+        peak = max(self.data)
+            
+        return round(peak, 3)
     
     def get_fwhm(self):
         """
         Get Full Width at Half Max value,
         for given x and y values
 
         Returns:
             float: calculated width value
         """
         # get wavelengths (x-axis values)
-        x = self.get_lambda()
+        self.lambda_value = self.get_lambda()
+        x = self.lambda_value
         y = self.data
         
         difference = max(y) - min(y)
         HM = difference / 2
         pos_extremum = y.argmax()
 
         nearest_above = (np.abs(y[pos_extremum:-1] - HM)).argmin()
         nearest_below = (np.abs(y[0:pos_extremum] - HM)).argmin()
 
         width = (np.mean(x[nearest_above + pos_extremum]) - 
                  np.mean(x[nearest_below]))
 
-        return width
+        return round(width, 3)
     
     def get_dll_version(self):
         """
         Get DLL/SDK version
 
         Returns:
             str: DLL/SDK version
@@ -140,12 +143,18 @@
     
     def get_num_pixels(self):
         """
         Returns the number of pixels of a spectrometer
         """
         return self._spectrometer.get_num_pixels()
     
+    def stop_measurement(self):
+        """
+        Stop wavelength measurement
+        """
+        self._spectrometer.stop_measure()
+    
     def disconnect(self):
         """
         Disconnect from the spectrometer
         """
         self._spectrometer.disconnect()
```

### Comparing `opsys-spectrometer-0.0.1/opsys_spectrometer.egg-info/requires.txt` & `opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.1/setup.py` & `opsys-spectrometer-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     if fname.exists():
         with open(fname, 'r') as f:
             targets = f.read().splitlines()
     return targets
 
 
 setuptools.setup(name='opsys-spectrometer',
-                 version='0.0.1',
+                 version='0.0.2',
                  description='python package for wavelength measuring devices',
                  url='https://bitbucket.org/opsys_tech/opsys-spectrometer/src/master/',
                  download_url='https://bitbucket.org/opsys_tech/opsys-spectrometer/src/master/',
                  author='dmitry.borovensky',
                  install_requires=get_install_requirements(),
                  author_email='dmitry.borovensky@opsys-tech.com',
                  packages=setuptools.find_packages(),
```

### Comparing `opsys-spectrometer-0.0.1/test/test_spectrometer.py` & `opsys-spectrometer-0.0.2/test/test_spectrometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,12 +54,18 @@
         
     @ patch.object(SpectrometerController, 'get_num_pixels')
     def test_get_num_pixels(self, spectro_mock: MagicMock):
         spectrometer = SpectrometerController()
         spectrometer.get_num_pixels()
         spectro_mock.assert_called_once_with()
         
+    @ patch.object(SpectrometerController, 'stop_measurement')
+    def test_stop_measurement(self, spectro_mock: MagicMock):
+        spectrometer = SpectrometerController()
+        spectrometer.stop_measurement()
+        spectro_mock.assert_called_once_with()
+        
     @ patch.object(SpectrometerController, 'disconnect')
     def test_disconnect(self, spectro_mock: MagicMock):
         spectrometer = SpectrometerController()
         spectrometer.disconnect()
         spectro_mock.assert_called_once_with()
```

