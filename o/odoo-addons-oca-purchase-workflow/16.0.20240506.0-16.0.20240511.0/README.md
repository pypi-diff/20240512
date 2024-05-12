# Comparing `tmp/odoo_addons_oca_purchase_workflow-16.0.20240506.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_purchase_workflow-16.0.20240511.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2048 bytes, number of entries: 4
--rw-r--r--  2.0 unx     5183 b- defN 24-May-07 06:10 odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 06:10 odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-07 06:10 odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 24-May-07 06:10 odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/RECORD
-4 files, 5717 bytes uncompressed, 1178 bytes compressed:  79.4%
+Zip file size: 2062 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     5331 b- defN 24-May-12 05:55 odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 05:55 odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-12 05:55 odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 24-May-12 05:55 odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/RECORD
+4 files, 5865 bytes uncompressed, 1192 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/METADATA
+Filename: odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/WHEEL
+Filename: odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/RECORD
+Filename: odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_purchase_workflow-16.0.20240506.0.dist-info/METADATA` & `odoo_addons_oca_purchase_workflow-16.0.20240511.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-purchase-workflow
-Version: 16.0.20240506.0
+Version: 16.0.20240511.0
 Summary: Meta package for oca-purchase-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -45,19 +45,21 @@
 Requires-Dist: odoo-addon-purchase-order-no-zero-price <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-owner <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-price-recalculation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-product-attachment-mgmt <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-product-recommendation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-purchase-manager <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-qty-change-no-recompute <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-purchase-order-supplier-return <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-supplierinfo-update <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-type-dashboard <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-uninvoiced-amount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-order-weight-volume <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-purchase-packaging-default <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-packaging-level-qty <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-partner-incoterm <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-partner-selectable-option <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-product-packaging-container-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-reception-status <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-reorder-control <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-request <16.1dev,>=16.0dev
```

