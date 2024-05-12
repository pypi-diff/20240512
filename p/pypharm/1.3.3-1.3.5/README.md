# Comparing `tmp/pypharm-1.3.3.tar.gz` & `tmp/pypharm-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypharm-1.3.3.tar", last modified: Sun Apr  7 19:42:46 2024, max compression
+gzip compressed data, was "pypharm-1.3.5.tar", last modified: Sun May 12 19:39:41 2024, max compression
```

## Comparing `pypharm-1.3.3.tar` & `pypharm-1.3.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:46.305100 pypharm-1.3.3/
--rw-rw-rw-   0        0        0    14758 2024-04-07 19:42:46.305100 pypharm-1.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:46.300100 pypharm-1.3.3/PyPharm/
--rw-rw-rw-   0        0        0       90 2023-11-25 15:50:04.000000 pypharm-1.3.3/PyPharm/__init__.py
--rw-rw-rw-   0        0        0    20452 2024-03-13 19:09:03.000000 pypharm-1.3.3/PyPharm/country_optimization.py
--rw-rw-rw-   0        0        0    13156 2023-10-22 19:22:41.000000 pypharm-1.3.3/PyPharm/country_optimization_v2.py
--rw-rw-rw-   0        0        0    32080 2024-04-07 19:29:54.000000 pypharm-1.3.3/PyPharm/models.py
--rw-rw-rw-   0        0        0    14238 2024-03-13 20:07:04.000000 pypharm-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 19:42:46.304101 pypharm-1.3.3/pypharm.egg-info/
--rw-rw-rw-   0        0        0    14758 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 19:42:46.306100 pypharm-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      827 2024-04-07 19:42:07.000000 pypharm-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 19:39:41.226277 pypharm-1.3.5/
+-rw-rw-rw-   0        0        0    18008 2024-05-12 19:39:41.226277 pypharm-1.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 19:39:41.222291 pypharm-1.3.5/PyPharm/
+-rw-rw-rw-   0        0        0       90 2023-11-25 15:50:04.000000 pypharm-1.3.5/PyPharm/__init__.py
+-rw-rw-rw-   0        0        0    19664 2024-05-11 20:28:45.000000 pypharm-1.3.5/PyPharm/country_optimization.py
+-rw-rw-rw-   0        0        0    13156 2023-10-22 19:22:41.000000 pypharm-1.3.5/PyPharm/country_optimization_v2.py
+-rw-rw-rw-   0        0        0    17034 2024-05-06 20:34:35.000000 pypharm-1.3.5/PyPharm/country_optimization_v3.py
+-rw-rw-rw-   0        0        0     5036 2024-05-12 19:26:32.000000 pypharm-1.3.5/PyPharm/genetic_optimization.py
+-rw-rw-rw-   0        0        0     4449 2024-05-02 22:48:40.000000 pypharm-1.3.5/PyPharm/gold_digger_optimization.py
+-rw-rw-rw-   0        0        0    33066 2024-05-11 20:28:45.000000 pypharm-1.3.5/PyPharm/models.py
+-rw-rw-rw-   0        0        0    17488 2024-05-12 19:38:56.000000 pypharm-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 19:39:41.225281 pypharm-1.3.5/pypharm.egg-info/
+-rw-rw-rw-   0        0        0    18008 2024-05-12 19:39:41.000000 pypharm-1.3.5/pypharm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-05-12 19:39:41.000000 pypharm-1.3.5/pypharm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 19:39:41.000000 pypharm-1.3.5/pypharm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-12 19:39:41.000000 pypharm-1.3.5/pypharm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 19:39:41.000000 pypharm-1.3.5/pypharm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 19:39:41.227274 pypharm-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      826 2024-05-12 19:26:32.000000 pypharm-1.3.5/setup.py
```

### Comparing `pypharm-1.3.3/PKG-INFO` & `pypharm-1.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pypharm
-Version: 1.3.3
-Summary: Module for solving pharmacokinetic problems
-Home-page: https://github.com/Krash13/PyPharm
-Author: Krash13
-Author-email: krasheninnikov.r.s@muctr.ru
-License: UNKNOWN
-Keywords: pharmacokinetics compartment-model
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 PyPharm  
 ----------  
   **1) Установка пакета**
   
 ```  
 pip install pypharm  
 ```  
@@ -135,14 +119,83 @@
 	printing=True,
 )
 ```
 
 При оптимизации, вектор неизвестных это
 x = [configuration_matrix (неизвестные), outputs(неизвестные), volumes(неизвестные)]
 
+Кроме того, вы можете использовать генетический алгоритм:
+```python
+model.optimize(
+    method='GA',
+    x_min=[0.00001, 0.001, 0.01, 1, 1],
+    x_max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+	n=100,
+    child_percent=0.3,
+    mutation_chance=0.5,
+    max_mutation=5,
+    t_max=300,
+    max_step=0.5,
+    printing=True,
+)
+```
+
+Вы даже можете использовать свой собственный алгоритм, если это необходимо
+
+```python
+# CountriesAlgorithm - ваш класс алгоритма
+# start - функция запуска алгоритма
+# важно, чтобы ваша функция запуска возвращала numpy.array
+
+model.optimize(
+    user_method=CountriesAlgorithm,
+    method_is_func=False,
+    optimization_func_name='start',
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], #ваши настроечные параметры
+    Xmax=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0.2, 0.4],
+    tmax=200,
+    max_step=0.5,
+    printing=True
+)
+```
+
+или
+
+```python
+# my_alg - ваша функция алгоритма, важно, чтобы она принимала только целевую функцию 
+
+model.optimize(
+    user_method=my_alg,
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], #ваши настроечные параметры
+    Xmax=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0.2, 0.4],
+    tmax=200,
+    max_step=0.5,
+    printing=True
+)
+```
+
 **4) Модель MagicCompartmentModel** 
 
 Данная модель необходима нам для тех случаев, 
 когда мы не знаем как именно стоит переводить входные
 единицы измерения в выходные.
 
 В модель добавляется 2 дополнительных параметра:
@@ -341,14 +394,85 @@
 printing=True,
 )
 ```
 
 When optimizing, the vector of unknowns is
 x = [configuration_matrix (unknown), outputs(unknown), volumes(unknown)]
 
+In addition, you can use a genetic algorithm:
+
+```python 
+
+model.optimize(
+    method='GA',
+    x_min=[0.00001, 0.001, 0.01, 1, 1],
+    x_max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    n=100,
+    percentage of descendants=0.3,
+    the probability of mutation =0.5,
+    max_mutation=5,
+    t_max=300,
+    max_step=0.5,
+    print=True,
+)
+```
+
+You can even use your own algorithm if necessary.
+
+```python
+# Countryalgorithm - your class is an algorithm
+# start - start the algorithm
+# it is important that your application aroused the interest of numpy.array
+
+model.optimize(
+    user_method=country Countryalgorithm,
+    method_is_func=False,
+    optimization_func_name='start',
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], # your desktop settings
+    Xmax Max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0,2, 0,4],
+    tmax=200,
+    max_step=0.5,
+    print=True
+)
+```
+
+or
+
+```python
+# my_alg is your algorithm function, it is important that it accepts only the target function
+
+model.optimize(
+    custom method=my_alg,
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], # your desktop settings
+    Xmax Max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0,2, 0,4],
+    tmax=200,
+    max_step=0.5,
+    print=True
+)
+```
+
 **4) The MagicCompartmentModel model**
 
 We need this model for those cases
 when we do not know exactly how to convert input
 units of measurement into output units.
 
 2 additional parameters are added to the model:
@@ -417,9 +541,8 @@
 from multiprocessing import shared_memory
 
 c = shared_memory.ShareableList(name='<your model.memory_name>')
 print(c)
 # ShareableList([4, 3.5192100752465563, 1.4158559227257506, 1.7264077213115414, 0.008336751860551, 0.2549196311342251, 0.5160375718404234, 6.915499993374695, 2.944744649331201, 0.5, 1.907294741996761], name='wnsm_0c50aa90')
 ```
 
-The data is stored in list format [current_iteration, x0, ... , xn, f], works only for the country_optimization algorithm.
-
+The data is stored in list format [current_iteration, x0, ... , xn, f], works only for the country_optimization algorithm.
```

### Comparing `pypharm-1.3.3/PyPharm/country_optimization.py` & `pypharm-1.3.5/PyPharm/country_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import random
 import numpy as np
 from operator import attrgetter
 from math import ceil, cos, sin
-from multiprocessing import shared_memory
 
 
 class Individual:
 
     def __init__(self, x, function):
         self.x = x
         self.f = function(self.x)
@@ -465,39 +464,7 @@
             if self.memory_list is not None:
                 self.memory_list[0] = ti
                 for i in range(len(result.x)):
                     self.memory_list[i + 1] = float(result.x[i])
                 self.memory_list[-1] = float(result.f)
         return (result.x, result.f, False, ti)
 
-
-
-# def func(x):
-#     s = 0
-#     for i in range(len(x) - 1):
-#         s += -x[i] * np.sin(abs(x[i] - x[i+1] - 47) ** 0.5) - (x[i+1] + 47) * np.sin(abs(x[i+1] + x[i] / 2 + 47) ** 0.5)
-#     return s
-#
-# k = 0
-# for i in range(100):
-#     CA = CountriesAlgorithm(
-#         f=func,
-#         Xmin=[-512 for i in range(3)],
-#         Xmax=[512 for i in range(3)],
-#         M=100,
-#         N=15,
-#         n=[1, 10],
-#         p=[0.00001, 2.5],
-#         m=[1, 8],
-#         k=8,
-#         l=3,
-#         ep=[0.2, 0.4],
-#         tmax=300,
-#         printing=False,
-#         teoretic_y=-1888.3213909
-#     )
-#     r = CA.start()
-#     print(i, r[2], r[0], r[1])
-#     if r[2]:
-#         k += 1
-#
-# print(k/100)
```

### Comparing `pypharm-1.3.3/PyPharm/country_optimization_v2.py` & `pypharm-1.3.5/PyPharm/country_optimization_v2.py`

 * *Files identical despite different names*

### Comparing `pypharm-1.3.3/PyPharm/models.py` & `pypharm-1.3.5/PyPharm/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 from scipy.integrate import solve_ivp, RK45
 from scipy.integrate import simps
 from scipy.optimize import minimize
 from .country_optimization import CountriesAlgorithm
 from .country_optimization_v2 import CountriesAlgorithm_v2
+from .genetic_optimization import GeneticAlgorithm
 from numba import njit
 import matplotlib.pyplot as plt
 
 
 class BaseCompartmentModel:
 
     configuration_matrix_target = None
@@ -212,50 +213,64 @@
             self.d = d
             self.compartment_number = compartment_number
             self.c0 = None
         else:
             self.c0 = np.array(c0)
         self.w = np.ones(self.teoretic_y.shape) if w is None else np.array(w)
 
-    def optimize(self, method=None, max_step=0.01, metric='R2', **kwargs):
+    def optimize(self, method=None, user_method=None, method_is_func=True,
+                 optimization_func_name='__call__', max_step=0.01, metric='R2', **kwargs):
         """
         Функция оптимизации модели
 
         Args:
             method: Метод оптимизации, любой доступный minimize + 'country_optimization' и 'country_optimization_v2'
             max_step: Максимальный шаг при решении СДУ
             **kwargs: Дополнительные именованные аргументы
 
         Returns:
             None
         """
         self._optim = True
         f = lambda x: self._target_function(x, max_step=max_step, metric=metric)
-        if method == 'country_optimization':
-            CA = CountriesAlgorithm(
-                f=f,
-                memory_list=getattr(self, 'memory', None),
-                **kwargs
-            )
-            CA.start()
-            x = CA.countries[0].population[0].x
-        elif method == 'country_optimization_v2':
-            CA = CountriesAlgorithm_v2(
-                f=f,
-                **kwargs
-            )
-            CA.start()
-            x = CA.countries[0].population[0].x
+        if user_method is not None:
+            if method_is_func:
+                x = user_method(f, **kwargs)
+            else:
+                optimization_obj = user_method(f, **kwargs)
+                x = getattr(optimization_obj, optimization_func_name)()
         else:
-            res = minimize(
-                fun=f,
-                method=method,
-                **kwargs
-            )
-            x = res.x
+            if method == 'country_optimization':
+                CA = CountriesAlgorithm(
+                    f=f,
+                    memory_list=getattr(self, 'memory', None),
+                    **kwargs
+                )
+                CA.start()
+                x = CA.countries[0].population[0].x
+            elif method == 'country_optimization_v2':
+                CA = CountriesAlgorithm_v2(
+                    f=f,
+                    **kwargs
+                )
+                CA.start()
+                x = CA.countries[0].population[0].x
+            elif method == 'GA':
+                CA = GeneticAlgorithm(
+                    f=f,
+                    **kwargs
+                )
+                x = CA.start()
+            else:
+                res = minimize(
+                    fun=f,
+                    method=method,
+                    **kwargs
+                )
+                x = res.x
         if self.configuration_matrix_target:
             self.configuration_matrix[self.configuration_matrix_target] = x[:self.configuration_matrix_target_count]
         if self.outputs_target:
             self.outputs[self.outputs_target] = x[
                                                 self.configuration_matrix_target_count:self.configuration_matrix_target_count + self.outputs_target_count]
         if self.volumes_target:
             self.volumes[self.volumes_target] = x[self.configuration_matrix_target_count + self.outputs_target_count:self.configuration_matrix_target_count + self.outputs_target_count + self.volumes_target_count]
@@ -322,16 +337,17 @@
         return res
 
     def load_data_from_list(self, x):
         super().load_data_from_list(x)
         if self.need_magic_optimization:
             self.magic_coefficient = x[-1]
         
-    def optimize(self, method=None, max_step=0.01, **kwargs):
-        x = super().optimize(method, max_step, **kwargs)
+    def optimize(self, method=None, user_method=None, method_is_func=True,
+                 optimization_func_name='__call__', max_step=0.01, **kwargs):
+        x = super().optimize(method, user_method, method_is_func, optimization_func_name, max_step, **kwargs)
         if self.need_magic_optimization:
             self.magic_coefficient = x[-1]
             self.need_magic_optimization = False
         return x
 
 
 class ReleaseCompartmentModel(BaseCompartmentModel):
@@ -588,16 +604,17 @@
             assert all([d, compartment_number is not None]), "Need to set d and compartment_number"
             self.d = d
             self.c0 = None
         else:
             self.c0 = np.array(c0)
         self.w = np.ones(self.teoretic_y.shape) if w is None else np.array(w)
 
-    def optimize(self, method=None, max_step=0.01, **kwargs):
-        x = super().optimize(method, max_step, **kwargs)
+    def optimize(self, method=None, user_method=None, method_is_func=True,
+                 optimization_func_name='__call__', max_step=0.01, **kwargs):
+        x = super().optimize(method, user_method, method_is_func, optimization_func_name, max_step, **kwargs)
         s = self.configuration_matrix_target_count + self.outputs_target_count + self.volumes_target_count
         if self.release_parameters_target:
             self.release_parameters[self.release_parameters_target] = x[s:s + self.release_parameters_target_count]
         if self.need_v_release_optimization:
             self.v_release = x[s:s + self.release_parameters_target_count + 1]
             self.need_v_release_optimization = False
         if self.with_accumulate:
```

### Comparing `pypharm-1.3.3/README.md` & `pypharm-1.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pypharm
+Version: 1.3.5
+Summary: Module for solving pharmacokinetic problems
+Home-page: https://github.com/Krash13/PyPharm
+Author: Krash13
+Author-email: krasheninnikov.r.s@muctr.ru
+License: UNKNOWN
+Keywords: pharmacokinetics compartment-model
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 PyPharm  
 ----------  
   **1) Установка пакета**
   
 ```  
 pip install pypharm  
 ```  
@@ -119,14 +135,83 @@
 	printing=True,
 )
 ```
 
 При оптимизации, вектор неизвестных это
 x = [configuration_matrix (неизвестные), outputs(неизвестные), volumes(неизвестные)]
 
+Кроме того, вы можете использовать генетический алгоритм:
+```python
+model.optimize(
+    method='GA',
+    x_min=[0.00001, 0.001, 0.01, 1, 1],
+    x_max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+	n=100,
+    child_percent=0.3,
+    mutation_chance=0.5,
+    max_mutation=5,
+    t_max=300,
+    max_step=0.5,
+    printing=True,
+)
+```
+
+Вы даже можете использовать свой собственный алгоритм, если это необходимо
+
+```python
+# CountriesAlgorithm - ваш класс алгоритма
+# start - функция запуска алгоритма
+# важно, чтобы ваша функция запуска возвращала numpy.array
+
+model.optimize(
+    user_method=CountriesAlgorithm,
+    method_is_func=False,
+    optimization_func_name='start',
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], #ваши настроечные параметры
+    Xmax=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0.2, 0.4],
+    tmax=200,
+    max_step=0.5,
+    printing=True
+)
+```
+
+или
+
+```python
+# my_alg - ваша функция алгоритма, важно, чтобы она принимала только целевую функцию 
+
+model.optimize(
+    user_method=my_alg,
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], #ваши настроечные параметры
+    Xmax=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0.2, 0.4],
+    tmax=200,
+    max_step=0.5,
+    printing=True
+)
+```
+
 **4) Модель MagicCompartmentModel** 
 
 Данная модель необходима нам для тех случаев, 
 когда мы не знаем как именно стоит переводить входные
 единицы измерения в выходные.
 
 В модель добавляется 2 дополнительных параметра:
@@ -325,14 +410,85 @@
 printing=True,
 )
 ```
 
 When optimizing, the vector of unknowns is
 x = [configuration_matrix (unknown), outputs(unknown), volumes(unknown)]
 
+In addition, you can use a genetic algorithm:
+
+```python 
+
+model.optimize(
+    method='GA',
+    x_min=[0.00001, 0.001, 0.01, 1, 1],
+    x_max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    n=100,
+    percentage of descendants=0.3,
+    the probability of mutation =0.5,
+    max_mutation=5,
+    t_max=300,
+    max_step=0.5,
+    print=True,
+)
+```
+
+You can even use your own algorithm if necessary.
+
+```python
+# Countryalgorithm - your class is an algorithm
+# start - start the algorithm
+# it is important that your application aroused the interest of numpy.array
+
+model.optimize(
+    user_method=country Countryalgorithm,
+    method_is_func=False,
+    optimization_func_name='start',
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], # your desktop settings
+    Xmax Max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0,2, 0,4],
+    tmax=200,
+    max_step=0.5,
+    print=True
+)
+```
+
+or
+
+```python
+# my_alg is your algorithm function, it is important that it accepts only the target function
+
+model.optimize(
+    custom method=my_alg,
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], # your desktop settings
+    Xmax Max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0,2, 0,4],
+    tmax=200,
+    max_step=0.5,
+    print=True
+)
+```
+
 **4) The MagicCompartmentModel model**
 
 We need this model for those cases
 when we do not know exactly how to convert input
 units of measurement into output units.
 
 2 additional parameters are added to the model:
@@ -401,8 +557,9 @@
 from multiprocessing import shared_memory
 
 c = shared_memory.ShareableList(name='<your model.memory_name>')
 print(c)
 # ShareableList([4, 3.5192100752465563, 1.4158559227257506, 1.7264077213115414, 0.008336751860551, 0.2549196311342251, 0.5160375718404234, 6.915499993374695, 2.944744649331201, 0.5, 1.907294741996761], name='wnsm_0c50aa90')
 ```
 
-The data is stored in list format [current_iteration, x0, ... , xn, f], works only for the country_optimization algorithm.
+The data is stored in list format [current_iteration, x0, ... , xn, f], works only for the country_optimization algorithm.
+
```

### Comparing `pypharm-1.3.3/pypharm.egg-info/PKG-INFO` & `pypharm-1.3.5/pypharm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypharm
-Version: 1.3.3
+Version: 1.3.5
 Summary: Module for solving pharmacokinetic problems
 Home-page: https://github.com/Krash13/PyPharm
 Author: Krash13
 Author-email: krasheninnikov.r.s@muctr.ru
 License: UNKNOWN
 Keywords: pharmacokinetics compartment-model
 Platform: UNKNOWN
@@ -135,14 +135,83 @@
 	printing=True,
 )
 ```
 
 При оптимизации, вектор неизвестных это
 x = [configuration_matrix (неизвестные), outputs(неизвестные), volumes(неизвестные)]
 
+Кроме того, вы можете использовать генетический алгоритм:
+```python
+model.optimize(
+    method='GA',
+    x_min=[0.00001, 0.001, 0.01, 1, 1],
+    x_max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+	n=100,
+    child_percent=0.3,
+    mutation_chance=0.5,
+    max_mutation=5,
+    t_max=300,
+    max_step=0.5,
+    printing=True,
+)
+```
+
+Вы даже можете использовать свой собственный алгоритм, если это необходимо
+
+```python
+# CountriesAlgorithm - ваш класс алгоритма
+# start - функция запуска алгоритма
+# важно, чтобы ваша функция запуска возвращала numpy.array
+
+model.optimize(
+    user_method=CountriesAlgorithm,
+    method_is_func=False,
+    optimization_func_name='start',
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], #ваши настроечные параметры
+    Xmax=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0.2, 0.4],
+    tmax=200,
+    max_step=0.5,
+    printing=True
+)
+```
+
+или
+
+```python
+# my_alg - ваша функция алгоритма, важно, чтобы она принимала только целевую функцию 
+
+model.optimize(
+    user_method=my_alg,
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], #ваши настроечные параметры
+    Xmax=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0.2, 0.4],
+    tmax=200,
+    max_step=0.5,
+    printing=True
+)
+```
+
 **4) Модель MagicCompartmentModel** 
 
 Данная модель необходима нам для тех случаев, 
 когда мы не знаем как именно стоит переводить входные
 единицы измерения в выходные.
 
 В модель добавляется 2 дополнительных параметра:
@@ -341,14 +410,85 @@
 printing=True,
 )
 ```
 
 When optimizing, the vector of unknowns is
 x = [configuration_matrix (unknown), outputs(unknown), volumes(unknown)]
 
+In addition, you can use a genetic algorithm:
+
+```python 
+
+model.optimize(
+    method='GA',
+    x_min=[0.00001, 0.001, 0.01, 1, 1],
+    x_max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    n=100,
+    percentage of descendants=0.3,
+    the probability of mutation =0.5,
+    max_mutation=5,
+    t_max=300,
+    max_step=0.5,
+    print=True,
+)
+```
+
+You can even use your own algorithm if necessary.
+
+```python
+# Countryalgorithm - your class is an algorithm
+# start - start the algorithm
+# it is important that your application aroused the interest of numpy.array
+
+model.optimize(
+    user_method=country Countryalgorithm,
+    method_is_func=False,
+    optimization_func_name='start',
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], # your desktop settings
+    Xmax Max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0,2, 0,4],
+    tmax=200,
+    max_step=0.5,
+    print=True
+)
+```
+
+or
+
+```python
+# my_alg is your algorithm function, it is important that it accepts only the target function
+
+model.optimize(
+    custom method=my_alg,
+    Xmin=[0.00001, 0.001, 0.01, 1, 1], # your desktop settings
+    Xmax Max=[1, 2, 1, 10, 3],
+    genes=[16, 17, 16, 20, 16],
+    M=20,
+    N=25,
+    n=[1, 10],
+    max_mutation=8,
+    m=[1, 8],
+    k=8,
+    l=3,
+    ep=[0,2, 0,4],
+    tmax=200,
+    max_step=0.5,
+    print=True
+)
+```
+
 **4) The MagicCompartmentModel model**
 
 We need this model for those cases
 when we do not know exactly how to convert input
 units of measurement into output units.
 
 2 additional parameters are added to the model:
```

### Comparing `pypharm-1.3.3/setup.py` & `pypharm-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r', encoding="utf-8") as f:
     return f.read()
 
 setup(
   name='pypharm',
-  version='1.3.3',
+  version='1.3.5',
   author='Krash13',
   author_email='krasheninnikov.r.s@muctr.ru',
   description='Module for solving pharmacokinetic problems',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Krash13/PyPharm',
   packages=find_packages(),
-  install_requires=['numpy>=1.22.1', 'scipy>=1.8.0', 'numba>=0.58.1', 'matplotlib>=3.5.1 '],
+  install_requires=['numpy>=1.22.1', 'scipy>=1.8.0', 'numba>=0.58.1', 'matplotlib>=3.5.1'],
   classifiers=[
     'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent'
   ],
   keywords='pharmacokinetics compartment-model',
   project_urls={
```

