# Comparing `tmp/odoo13_addons_oca_manufacture-13.0.20220705.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_manufacture-13.0.20230606.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1665 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1744 b- defN 22-Jul-06 03:49 odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-06 03:49 odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Jul-06 03:49 odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      425 b- defN 22-Jul-06 03:49 odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/RECORD
-4 files, 2262 bytes uncompressed, 827 bytes compressed:  63.4%
+Zip file size: 1677 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1799 b- defN 23-Jun-07 04:13 odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 04:13 odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-07 04:13 odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      425 b- defN 23-Jun-07 04:13 odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/RECORD
+4 files, 2317 bytes uncompressed, 839 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/METADATA
+Filename: odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/RECORD
+Filename: odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_manufacture-13.0.20220705.0.dist-info/METADATA` & `odoo13_addons_oca_manufacture-13.0.20230606.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-manufacture
-Version: 13.0.20220705.0
+Version: 13.0.20230606.0
 Summary: Meta package for oca-manufacture Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
@@ -24,14 +24,15 @@
 Requires-Dist: odoo13-addon-mrp-production-putaway-strategy
 Requires-Dist: odoo13-addon-mrp-production-request
 Requires-Dist: odoo13-addon-mrp-sale-info
 Requires-Dist: odoo13-addon-mrp-stock-orderpoint-manual-procurement
 Requires-Dist: odoo13-addon-mrp-unbuild-tracked-raw-material
 Requires-Dist: odoo13-addon-mrp-warehouse-calendar
 Requires-Dist: odoo13-addon-mrp-workorder-sequence
+Requires-Dist: odoo13-addon-product-cost-rollup-to-bom
 Requires-Dist: odoo13-addon-product-mrp-info
 Requires-Dist: odoo13-addon-product-quick-bom
 Requires-Dist: odoo13-addon-quality-control-mrp-oca
 Requires-Dist: odoo13-addon-quality-control-oca
 Requires-Dist: odoo13-addon-quality-control-stock-oca
 Requires-Dist: odoo13-addon-repair-refurbish
 Requires-Dist: odoo13-addon-stock-picking-product-kit-helper
```

