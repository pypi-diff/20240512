# Comparing `tmp/odoo_addons_oca_timesheet-16.0.20240412.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_timesheet-16.0.20240510.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1525 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1597 b- defN 24-Apr-13 06:43 odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 06:43 odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-13 06:43 odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      409 b- defN 24-Apr-13 06:43 odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/RECORD
-4 files, 2099 bytes uncompressed, 719 bytes compressed:  65.7%
+Zip file size: 1542 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1745 b- defN 24-May-12 06:55 odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 06:55 odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-12 06:55 odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      409 b- defN 24-May-12 06:55 odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/RECORD
+4 files, 2247 bytes uncompressed, 736 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/METADATA
+Filename: odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/WHEEL
+Filename: odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/RECORD
+Filename: odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_timesheet-16.0.20240412.0.dist-info/METADATA` & `odoo_addons_oca_timesheet-16.0.20240510.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-timesheet
-Version: 16.0.20240412.0
+Version: 16.0.20240510.1
 Summary: Meta package for oca-timesheet Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-crm-timesheet <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-employee-cost-history <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-begin-end <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-employee-analytic-tag <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-name-customer <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-report <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-sheet <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-hr-timesheet-sheet-attendance <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-sheet-autodraft <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-sheet-policy-project-manager <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-task-domain <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-task-required <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-task-stage <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-hr-timesheet-time-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-project-task-analytic-propagation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-project-task-stage-allow-timesheet <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-sale-timesheet-invoice-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-timesheet-line-exclude <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-timesheet-rounded <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-timesheet-task-exclude <16.1dev,>=16.0dev
 
 UNKNOWN
```

