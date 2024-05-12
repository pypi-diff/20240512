# Comparing `tmp/schubmult-1.3.6.tar.gz` & `tmp/schubmult-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.6.tar", last modified: Fri May  3 18:01:59 2024, max compression
+gzip compressed data, was "schubmult-1.3.7.tar", last modified: Sun May 12 18:39:23 2024, max compression
```

## Comparing `schubmult-1.3.6.tar` & `schubmult-1.3.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.894000 schubmult-1.3.6/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5235 2024-05-03 18:01:59.846000 schubmult-1.3.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4853 2024-04-15 14:05:16.000000 schubmult-1.3.6/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:57.642000 schubmult-1.3.6/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.6/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16320 2024-05-01 14:26:35.000000 schubmult-1.3.6/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.350000 schubmult-1.3.6/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.6/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.6/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.6/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.627000 schubmult-1.3.6/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.6/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.6/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.6/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.941000 schubmult-1.3.6/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.6/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.6/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     9034 2024-05-01 11:44:33.000000 schubmult-1.3.6/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.203000 schubmult-1.3.6/schubmult/schubmult_q_double/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.6/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.6/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.6/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.477000 schubmult-1.3.6/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.6/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.6/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     8098 2024-05-03 15:03:11.000000 schubmult-1.3.6/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:59.781000 schubmult-1.3.6/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.6/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.6/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.6/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 18:01:58.069000 schubmult-1.3.6/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5235 2024-05-03 18:01:55.000000 schubmult-1.3.6/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-03 18:01:55.000000 schubmult-1.3.6/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-03 18:01:56.000000 schubmult-1.3.6/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-03 18:01:59.878000 schubmult-1.3.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-03 18:01:06.000000 schubmult-1.3.6/setup.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.882000 schubmult-1.3.7/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.7/LICENSE
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     5681 2024-05-12 18:39:23.831000 schubmult-1.3.7/PKG-INFO
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     5299 2024-05-12 18:38:20.000000 schubmult-1.3.7/README.md
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:21.540000 schubmult-1.3.7/schubmult/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2023-09-24 17:08:26.000000 schubmult-1.3.7/schubmult/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    17334 2024-05-12 18:35:24.000000 schubmult-1.3.7/schubmult/perm_lib.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:22.269000 schubmult-1.3.7/schubmult/schubmult_double/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       41 2023-09-25 01:39:08.000000 schubmult-1.3.7/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       97 2023-09-26 17:55:50.000000 schubmult-1.3.7/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.7/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:22.570000 schubmult-1.3.7/schubmult/schubmult_py/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       36 2023-09-25 01:39:03.000000 schubmult-1.3.7/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       94 2023-09-26 17:55:38.000000 schubmult-1.3.7/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.7/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:22.859000 schubmult-1.3.7/schubmult/schubmult_q/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       36 2024-04-03 15:35:41.000000 schubmult-1.3.7/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       92 2024-04-03 15:28:43.000000 schubmult-1.3.7/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     9034 2024-05-01 11:44:33.000000 schubmult-1.3.7/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.144000 schubmult-1.3.7/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       33 2024-04-12 18:50:20.000000 schubmult-1.3.7/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       99 2024-04-12 18:49:31.000000 schubmult-1.3.7/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.7/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.456000 schubmult-1.3.7/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       29 2024-04-12 18:49:56.000000 schubmult-1.3.7/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       95 2024-04-12 18:49:43.000000 schubmult-1.3.7/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     9952 2024-05-12 18:35:10.000000 schubmult-1.3.7/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:23.756000 schubmult-1.3.7/schubmult/schubmult_yz/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       27 2023-09-25 01:38:28.000000 schubmult-1.3.7/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       93 2023-09-26 17:55:32.000000 schubmult-1.3.7/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.7/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        0 2024-05-12 18:39:21.962000 schubmult-1.3.7/schubmult.egg-info/
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     5681 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)      978 2024-05-12 18:39:20.000000 schubmult-1.3.7/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)        1 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)      353 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       83 2024-05-12 18:39:19.000000 schubmult-1.3.7/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       10 2024-05-12 18:39:20.000000 schubmult-1.3.7/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)       79 2024-05-12 18:39:23.866000 schubmult-1.3.7/setup.cfg
+-rwxrwxrwx   0 matthematics  (1000) matthematics  (1000)     1243 2024-05-12 18:36:25.000000 schubmult-1.3.7/setup.py
```

### Comparing `schubmult-1.3.6/LICENSE` & `schubmult-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/PKG-INFO` & `schubmult-1.3.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.6
+Version: 1.3.7
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -46,15 +46,18 @@
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
 schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
-
+Since version 1.3.7, schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
+```
+schubmult_q_yz -nil-hecke 6 -code 2 2 --display-positive
+```
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
 New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
```

### Comparing `schubmult-1.3.6/README.md` & `schubmult-1.3.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
 schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
-
+Since version 1.3.7, schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
+```
+schubmult_q_yz -nil-hecke 6 -code 2 2 --display-positive
+```
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
 New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
```

### Comparing `schubmult-1.3.6/schubmult/perm_lib.py` & `schubmult-1.3.7/schubmult/perm_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,14 +177,40 @@
 						#print(f"{ct=} {i=} {j=} {k=} {last_j=} {pp=} {up_perm2=} {new_perm_add=} {new_val=}")
 						perm_list += [(new_perm_add,new_val,j)]
 						total_list+=[(new_perm_add,pp+1,new_val)]
 		up_perm_list = perm_list
 	#print(f"{total_list=}")
 	return total_list
 
+def elem_sym_perms_q_op(orig_perm,p,k,n):	
+	total_list = [(orig_perm,0,1)]
+	up_perm_list = [(orig_perm,1,k)]
+	for pp in range(p):
+		perm_list = []
+		for up_perm, val, last_j in up_perm_list:
+			up_perm2 = [*up_perm]
+			if len(up_perm) < n :
+				up_perm2 += [i+1 for i in range(len(up_perm2),n)]
+			pos_list = [i for i in range(k) if (i>=len(orig_perm) and up_perm2[i]==i+1) or (i<len(orig_perm) and up_perm2[i] == orig_perm[i])]
+			for j in range(last_j,n):
+				for i in pos_list:
+					ct = count_bruhat(up_perm2,i,j)
+					#print(f"{up_perm2=} {ct=} {i=} {j=} {k=} {pp=}")
+					if ct == -1 or ct == 2*(j-i)-1:
+						new_perm = [*up_perm2]
+						new_perm[i],new_perm[j] = new_perm[j],new_perm[i]
+						new_perm_add = tuple(permtrim(new_perm))
+						new_val = val
+						if ct>0:
+							new_val *= np.prod([q_var[index] for index in range(i+1,j+1)])
+						perm_list += [(new_perm_add,new_val,j)]
+						total_list+=[(new_perm_add,pp+1,new_val)]
+		up_perm_list = perm_list
+	return total_list
+
 
 # perms and inversion diff
 def kdown_perms(perm,monoperm,p,k):	
 	inv_m = inv(monoperm)
 	inv_p = inv(perm)
 	full_perm_list = []
```

### Comparing `schubmult-1.3.6/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.7/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.7/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.7/schubmult/schubmult_q/schubmult_q.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.3.7/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.3.7/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,57 @@
 from schubmult.perm_lib import *
 from schubmult.schubmult_yz import compute_positive_rep, posify
 from symengine import *
 import sys
 
-
-#q_var = symarray("q",100)
-
 var2 = symarray("y",100)
 var3 = symarray("z",100)
 
-	
+var_x = symarray("x",100)
+
+def nil_hecke(perm_dict,v,n,var2=var2,var3=var3):
+	th = strict_theta(inverse(v))
+	mu = permtrim(uncode(th))
+	vmu = permtrim(mulperm([*v],mu))
+	inv_vmu = inv(vmu)
+	inv_mu = inv(mu)
+	ret_dict = {}
+	vpaths = [([(vmu,0)],1)]
+	while th[-1] == 0:
+		th.pop()
+	thL = len(th)
+	vpathdicts = compute_vpathdicts(th,vmu,True)
+	for u,val in perm_dict.items():
+		inv_u = inv(u)
+		vpathsums = {u: {(1,2): val}}
+		for index in range(thL):			
+			mx_th = 0
+			for vp in vpathdicts[index]:
+				for v2,vdiff,s in vpathdicts[index][vp]:
+					if th[index]-vdiff > mx_th:
+						mx_th = th[index] - vdiff					
+			newpathsums = {}
+			for up in vpathsums:
+				inv_up = inv(up)
+				newperms = elem_sym_perms_q_op(up,mx_th,th[index],n)
+				for up2, udiff,mul_val in newperms:
+					if up2 not in newpathsums:
+						newpathsums[up2]={}
+					for v in vpathdicts[index]:
+						sumval = vpathsums[up].get(v,zero)*mul_val
+						if sumval == 0:
+							continue
+						for v2,vdiff,s in vpathdicts[index][v]:
+							#print(f"{code(up2)=} {elem_sym_func_q(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)=} {mul_val=} {sumval=}")							
+							newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*elem_sym_func_q(th[index],index+1,up2,up,v,v2,udiff,vdiff,var2,var3)
+			vpathsums = newpathsums
+		toget = tuple(vmu)
+		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
+	return ret_dict
 
-	
 
 	
 def schubmult(perm_dict,v,var2=var2,var3=var3):
 	th = strict_theta(inverse(v))
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	inv_vmu = inv(vmu)
@@ -146,62 +182,79 @@
 			
 		ret[q_part] = ret.get(q_part,0) + yz_part
 	return ret
 
 var2_t = tuple(var2.tolist())
 var3_t = tuple(var3.tolist())	
 
+def print_usage():
+	print("**** schubmult_q_yz ****")
+	print("Purpose: Compute Molev-Sagan coefficients of quantum double Schubert polynomials")
+	print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
+	print("       *** Computes products")
+	print("Alternative usage: schubmult_q_yz -nil-hecke n <-code> <--display-positive> perm")
+	print("       *** Computes nil-Hecke representation of quantum double Schubert polynomial, limiting to the group S_n")
+
 def main():
 	global var2
 	try:
 		sys.setrecursionlimit(1000000)
 	
 		perms=[]
 		curperm = []
 		
 		pr = True
 		display_positive = False
 		ascode = False
 		coprod = False
+		nilhecke = False
 		check = True
 		msg = False
+		just_nil = False
+		
+		nil_N = 0
+		
 		try:
 			for s in sys.argv[1:]:
+				if just_nil:
+					just_nil = False
+					nil_N = int(s)
+					continue
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
 				if s == "-nocheck":
 					check = False
 					continue
 				if s == "--display-positive":
 					display_positive = True
 					continue
 				if s == "--optimizer-message":
 					msg = True
 					continue
+				if s == "-nil-hecke":
+					nilhecke = True
+					just_nil = True
+					continue
 				if s == "--version":
 					print(f"Python version {sys.version}")
 					exit(0)
 				if s == "-code":
 					ascode = True
 					continue
-				if s == "--usage":
-					print("**** schubmult_q_yz ****")
-					print("Purpose: Compute Molev-Sagan coefficients of quantum double Schubert polynomials")
-					print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
+				if s == "--usage" or s == "--help":
+					print_usage()
 					exit(0)
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
-			print("**** schubmult_q_yz ****")
-			print("Purpose: Compute Molev-Sagan coefficients of quantum double Schubert polynomials")
-			print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
+			print_usage()
 			exit(1)
 				
 		perms += [curperm]
 		
 		
 		if ascode:
 			for i in range(len(perms)):
@@ -209,17 +262,22 @@
 		else:
 			for i in range(len(perms)):
 				perms[i] = tuple(permtrim([*perms[i]]))
 		
 		size = 0
 		L = len(perms)
 		
-		coeff_dict = {perms[0]: 1}
-		for perm in perms[1:]:
-			coeff_dict = schubmult(coeff_dict,perm)
+		if nilhecke:
+			coeff_dict = nil_hecke({(1,2): 1},perms[0],nil_N)			
+			rep = ("y","x")
+		else:
+			coeff_dict = {perms[0]: 1}
+			for perm in perms[1:]:
+				coeff_dict = schubmult(coeff_dict,perm)
+			rep = ("","")
 		
 		if pr:
 			if ascode:
 				width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			else:
 				width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			
@@ -265,15 +323,15 @@
 										exit(1)
 							if check and expand(val - val2)!=0:
 								print(f"error: value not equal; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
 								exit(1)
 							val = val2
 					if val!=0:
 						if ascode:
-							print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ')}")	
+							print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 						else:
-							print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ')}")	
+							print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 	except BrokenPipeError:
 		pass
 		
 if __name__ == "__main__":
 	main()
```

### Comparing `schubmult-1.3.6/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.7/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.7/schubmult.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.6
+Version: 1.3.7
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -46,15 +46,18 @@
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
 schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
-
+Since version 1.3.7, schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
+```
+schubmult_q_yz -nil-hecke 6 -code 2 2 --display-positive
+```
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
 New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
```

### Comparing `schubmult-1.3.6/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.7/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.6/setup.py` & `schubmult-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.6",
+    version="1.3.7",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

