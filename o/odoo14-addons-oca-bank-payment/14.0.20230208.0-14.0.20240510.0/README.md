# Comparing `tmp/odoo14_addons_oca_bank_payment-14.0.20230208.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_bank_payment-14.0.20240510.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1555 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1490 b- defN 23-Feb-09 03:19 odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-09 03:19 odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-09 03:19 odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      429 b- defN 23-Feb-09 03:19 odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/RECORD
-4 files, 2012 bytes uncompressed, 709 bytes compressed:  64.8%
+Zip file size: 1566 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-12 03:01 odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 03:01 odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-12 03:01 odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      429 b- defN 24-May-12 03:01 odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/RECORD
+4 files, 2073 bytes uncompressed, 720 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/METADATA
+Filename: odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/RECORD
+Filename: odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_bank_payment-14.0.20230208.0.dist-info/METADATA` & `odoo14_addons_oca_bank_payment-14.0.20240510.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-bank-payment
-Version: 14.0.20230208.0
+Version: 14.0.20240510.0
 Summary: Meta package for oca-bank-payment Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -15,14 +15,15 @@
 Requires-Dist: odoo14-addon-account-banking-sepa-credit-transfer
 Requires-Dist: odoo14-addon-account-banking-sepa-direct-debit
 Requires-Dist: odoo14-addon-account-invoice-select-for-payment
 Requires-Dist: odoo14-addon-account-payment-mode
 Requires-Dist: odoo14-addon-account-payment-mode-default-account
 Requires-Dist: odoo14-addon-account-payment-order
 Requires-Dist: odoo14-addon-account-payment-order-grouped-output
+Requires-Dist: odoo14-addon-account-payment-order-lock-draft
 Requires-Dist: odoo14-addon-account-payment-order-notification
 Requires-Dist: odoo14-addon-account-payment-order-return
 Requires-Dist: odoo14-addon-account-payment-order-sequence-payment-mode
 Requires-Dist: odoo14-addon-account-payment-order-tier-validation
 Requires-Dist: odoo14-addon-account-payment-order-vendor-email
 Requires-Dist: odoo14-addon-account-payment-partner
 Requires-Dist: odoo14-addon-account-payment-purchase
```

