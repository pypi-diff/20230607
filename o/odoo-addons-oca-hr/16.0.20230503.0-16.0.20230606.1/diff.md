# Comparing `tmp/odoo_addons_oca_hr-16.0.20230503.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_hr-16.0.20230606.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1396 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1067 b- defN 23-May-03 04:18 odoo_addons_oca_hr-16.0.20230503.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 04:18 odoo_addons_oca_hr-16.0.20230503.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 04:18 odoo_addons_oca_hr-16.0.20230503.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      381 b- defN 23-May-03 04:18 odoo_addons_oca_hr-16.0.20230503.0.dist-info/RECORD
-4 files, 1541 bytes uncompressed, 646 bytes compressed:  58.1%
+Zip file size: 1420 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1208 b- defN 23-Jun-07 03:30 odoo_addons_oca_hr-16.0.20230606.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 03:30 odoo_addons_oca_hr-16.0.20230606.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-07 03:30 odoo_addons_oca_hr-16.0.20230606.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      381 b- defN 23-Jun-07 03:30 odoo_addons_oca_hr-16.0.20230606.1.dist-info/RECORD
+4 files, 1682 bytes uncompressed, 670 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_hr-16.0.20230503.0.dist-info/METADATA
+Filename: odoo_addons_oca_hr-16.0.20230606.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_hr-16.0.20230503.0.dist-info/WHEEL
+Filename: odoo_addons_oca_hr-16.0.20230606.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_hr-16.0.20230503.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_hr-16.0.20230606.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_hr-16.0.20230503.0.dist-info/RECORD
+Filename: odoo_addons_oca_hr-16.0.20230606.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_hr-16.0.20230503.0.dist-info/METADATA` & `odoo_addons_oca_hr-16.0.20230606.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-hr
-Version: 16.0.20230503.0
+Version: 16.0.20230606.1
 Summary: Meta package for oca-hr Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-hr-course (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-age (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-hr-employee-birthday-mail (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-digitized-signature (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-firstname (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-lastnames (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-medical-examination (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-partner-external (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-phone-extension (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-relative (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-employee-ssn (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-hr-holidays-settings (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-personal-equipment-request (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

