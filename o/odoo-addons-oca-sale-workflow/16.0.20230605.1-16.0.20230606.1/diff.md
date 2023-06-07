# Comparing `tmp/odoo_addons_oca_sale_workflow-16.0.20230605.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_sale_workflow-16.0.20230606.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1685 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2339 b- defN 23-Jun-06 04:59 odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 04:59 odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-06 04:59 odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      425 b- defN 23-Jun-06 04:59 odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/RECORD
-4 files, 2857 bytes uncompressed, 847 bytes compressed:  70.4%
+Zip file size: 1701 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2487 b- defN 23-Jun-07 05:01 odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 05:01 odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-07 05:01 odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      425 b- defN 23-Jun-07 05:01 odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/RECORD
+4 files, 3005 bytes uncompressed, 863 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/METADATA
+Filename: odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/WHEEL
+Filename: odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/RECORD
+Filename: odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_sale_workflow-16.0.20230605.1.dist-info/METADATA` & `odoo_addons_oca_sale_workflow-16.0.20230606.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-sale-workflow
-Version: 16.0.20230605.1
+Version: 16.0.20230606.1
 Summary: Meta package for oca-sale-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -15,23 +15,25 @@
 Requires-Dist: odoo-addon-sale-automatic-workflow-job (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-automatic-workflow-payment-mode (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-cancel-reason (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-commercial-partner (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-company-currency (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-elaboration (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-exception (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-sale-force-invoiced (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-invoice-policy (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-archive (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-general-discount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-invoice-amount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-line-menu (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-line-price-history (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-lot-generator (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-lot-selection (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-product-availability-inline (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-sale-order-product-recommendation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-qty-change-no-recompute (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-revision (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-type (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-partner-incoterm (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-partner-selectable-option (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-stock-picking-blocking (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-tier-validation (<16.1dev,>=16.0dev)
```

