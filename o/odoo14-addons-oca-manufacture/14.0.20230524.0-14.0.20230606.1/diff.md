# Comparing `tmp/odoo14_addons_oca_manufacture-14.0.20230524.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_manufacture-14.0.20230606.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1868 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2955 b- defN 23-May-25 04:12 odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 04:12 odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-25 04:12 odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      425 b- defN 23-May-25 04:12 odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/RECORD
-4 files, 3473 bytes uncompressed, 1030 bytes compressed:  70.3%
+Zip file size: 1878 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3059 b- defN 23-Jun-07 04:14 odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 04:14 odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-07 04:14 odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      425 b- defN 23-Jun-07 04:14 odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/RECORD
+4 files, 3577 bytes uncompressed, 1040 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/METADATA
+Filename: odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/RECORD
+Filename: odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_manufacture-14.0.20230524.0.dist-info/METADATA` & `odoo14_addons_oca_manufacture-14.0.20230606.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-manufacture
-Version: 14.0.20230524.0
+Version: 14.0.20230606.1
 Summary: Meta package for oca-manufacture Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -15,14 +15,15 @@
 Requires-Dist: odoo14-addon-mrp-analytic-cost
 Requires-Dist: odoo14-addon-mrp-attachment-mgmt
 Requires-Dist: odoo14-addon-mrp-bom-attribute-match
 Requires-Dist: odoo14-addon-mrp-bom-component-menu
 Requires-Dist: odoo14-addon-mrp-bom-hierarchy
 Requires-Dist: odoo14-addon-mrp-bom-line-sequence
 Requires-Dist: odoo14-addon-mrp-bom-location
+Requires-Dist: odoo14-addon-mrp-bom-note
 Requires-Dist: odoo14-addon-mrp-bom-responsible
 Requires-Dist: odoo14-addon-mrp-bom-tracking
 Requires-Dist: odoo14-addon-mrp-component-operation
 Requires-Dist: odoo14-addon-mrp-component-operation-scrap-reason
 Requires-Dist: odoo14-addon-mrp-lot-on-hand-first
 Requires-Dist: odoo14-addon-mrp-multi-level
 Requires-Dist: odoo14-addon-mrp-multi-level-estimate
@@ -51,14 +52,15 @@
 Requires-Dist: odoo14-addon-product-mrp-info
 Requires-Dist: odoo14-addon-quality-control-mrp-oca
 Requires-Dist: odoo14-addon-quality-control-oca
 Requires-Dist: odoo14-addon-quality-control-stock-oca
 Requires-Dist: odoo14-addon-repair-discount
 Requires-Dist: odoo14-addon-repair-picking-after-done
 Requires-Dist: odoo14-addon-repair-refurbish
+Requires-Dist: odoo14-addon-repair-refurbish-repair-stock-move
 Requires-Dist: odoo14-addon-repair-stock-move
 Requires-Dist: odoo14-addon-repair-type
 Requires-Dist: odoo14-addon-stock-picking-product-kit-helper
 Requires-Dist: odoo14-addon-stock-whole-kit-constraint
 
 UNKNOWN
```

