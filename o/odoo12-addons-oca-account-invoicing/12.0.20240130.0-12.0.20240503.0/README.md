# Comparing `tmp/odoo12_addons_oca_account_invoicing-12.0.20240130.0-py3-none-any.whl.zip` & `tmp/odoo12_addons_oca_account_invoicing-12.0.20240503.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2008 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4259 b- defN 24-Jan-31 02:51 odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-31 02:51 odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Jan-31 02:51 odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      449 b- defN 24-Jan-31 02:51 odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/RECORD
-4 files, 4801 bytes uncompressed, 1122 bytes compressed:  76.6%
+Zip file size: 2019 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4322 b- defN 24-May-04 02:45 odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-04 02:45 odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-04 02:45 odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      449 b- defN 24-May-04 02:45 odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/RECORD
+4 files, 4864 bytes uncompressed, 1133 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/METADATA
+Filename: odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/WHEEL
+Filename: odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/top_level.txt
+Filename: odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/RECORD
+Filename: odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo12_addons_oca_account_invoicing-12.0.20240130.0.dist-info/METADATA` & `odoo12_addons_oca_account_invoicing-12.0.20240503.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addons-oca-account-invoicing
-Version: 12.0.20240130.0
+Version: 12.0.20240503.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
@@ -21,14 +21,15 @@
 Requires-Dist: odoo12-addon-account-invoice-confirm-popup
 Requires-Dist: odoo12-addon-account-invoice-date-due
 Requires-Dist: odoo12-addon-account-invoice-default-code-column
 Requires-Dist: odoo12-addon-account-invoice-fiscal-position-update
 Requires-Dist: odoo12-addon-account-invoice-fix-tax-rounding
 Requires-Dist: odoo12-addon-account-invoice-fixed-discount
 Requires-Dist: odoo12-addon-account-invoice-force-number
+Requires-Dist: odoo12-addon-account-invoice-line-complimentary
 Requires-Dist: odoo12-addon-account-invoice-line-default-account
 Requires-Dist: odoo12-addon-account-invoice-line-description
 Requires-Dist: odoo12-addon-account-invoice-line-sequence
 Requires-Dist: odoo12-addon-account-invoice-mass-sending
 Requires-Dist: odoo12-addon-account-invoice-merge
 Requires-Dist: odoo12-addon-account-invoice-pricelist
 Requires-Dist: odoo12-addon-account-invoice-pricelist-sale
```

