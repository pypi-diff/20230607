# Comparing `tmp/odoo14_addon_metadata-14.0.0.0.1-py3-none-any.whl.zip` & `tmp/odoo14_addon_metadata-14.0.1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 2618 bytes, number of entries: 8
--rw-r--r--  2.0 unx       21 b- defN 23-May-02 14:44 odoo/addons/metadata/__init__.py
--rw-r--r--  2.0 unx      379 b- defN 23-May-05 10:33 odoo/addons/metadata/__manifest__.py
--rw-r--r--  2.0 unx       28 b- defN 23-May-02 14:44 odoo/addons/metadata/models/__init__.py
--rw-r--r--  2.0 unx      322 b- defN 23-May-02 14:44 odoo/addons/metadata/models/metadata_line.py
--rw-r--r--  2.0 unx      455 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      745 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD
-8 files, 2047 bytes uncompressed, 1278 bytes compressed:  37.6%
+Zip file size: 2966 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       21 b- defN 23-May-03 12:56 odoo/addons/metadata/__init__.py
+-rw-r--r--  2.0 unx      423 b- defN 23-Jun-07 18:27 odoo/addons/metadata/__manifest__.py
+-rw-r--r--  2.0 unx       28 b- defN 23-May-03 12:56 odoo/addons/metadata/models/__init__.py
+-rw-r--r--  2.0 unx      322 b- defN 23-May-03 12:56 odoo/addons/metadata/models/metadata_line.py
+-rwxr-xr-x  2.0 unx      148 b- defN 23-Jun-07 18:27 odoo/addons/metadata/security/ir.model.access.csv
+-rw-r--r--  2.0 unx      456 b- defN 23-Jun-07 18:29 odoo14_addon_metadata-14.0.1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 18:29 odoo14_addon_metadata-14.0.1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-07 18:29 odoo14_addon_metadata-14.0.1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      850 b- defN 23-Jun-07 18:29 odoo14_addon_metadata-14.0.1.0.0.dist-info/RECORD
+9 files, 2345 bytes uncompressed, 1452 bytes compressed:  38.1%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: odoo/addons/metadata/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/metadata/models/metadata_line.py
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/METADATA
+Filename: odoo/addons/metadata/security/ir.model.access.csv
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/WHEEL
+Filename: odoo14_addon_metadata-14.0.1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/top_level.txt
+Filename: odoo14_addon_metadata-14.0.1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD
+Filename: odoo14_addon_metadata-14.0.1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo14_addon_metadata-14.0.1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/metadata/__manifest__.py

```diff
@@ -5,16 +5,18 @@
     'summary': """
         Save custom metadata on any model""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'server',
-    'version': '14.0.0.0.1',
+    'version': '14.0.1.0.0',
     "license": "AGPL-3",
 
     # any module necessary for this one to work correctly
     'depends': ['base'],
 
     # always loaded
-    'data': [],
+    'data': [
+        'security/ir.model.access.csv'
+    ],
 }
```

## Comparing `odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD` & `odoo14_addon_metadata-14.0.1.0.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 odoo/addons/metadata/__init__.py,sha256=X9EJGOE2GtZbS0G82PtSXmWSZ_R8jEM0rlJTDliQjp4,21
-odoo/addons/metadata/__manifest__.py,sha256=c6Y1k08idM6gNnfA_sO4iFxx5sYSXZTfNRi1MdnP6to,379
+odoo/addons/metadata/__manifest__.py,sha256=PU87FN4dqRn-kNi56jHwsm5hExVvoZbv-ULI-BlUbXM,423
 odoo/addons/metadata/models/__init__.py,sha256=vG7B0tIxGzuSl710Vo4Xv5mrrcfmJpVaAleEZBmvDFs,28
 odoo/addons/metadata/models/metadata_line.py,sha256=127tiwAUtC_hYIyiwGJsRBXCQdfY6TGKk4n0VQr7kC4,322
-odoo14_addon_metadata-14.0.0.0.1.dist-info/METADATA,sha256=pRDthMpRgNvnL2_vSWhCsL0XjqmM194rVI9WlEx9ISE,455
-odoo14_addon_metadata-14.0.0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo14_addon_metadata-14.0.0.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD,,
+odoo/addons/metadata/security/ir.model.access.csv,sha256=sYhtFcXXvIUjFYW7403-D0sbbbmLXyVem5uQx7pUIK8,148
+odoo14_addon_metadata-14.0.1.0.0.dist-info/METADATA,sha256=C45FVqBVE9sy0IyhzIJK5WLxOayizFsUp005dGez26A,456
+odoo14_addon_metadata-14.0.1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo14_addon_metadata-14.0.1.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_metadata-14.0.1.0.0.dist-info/RECORD,,
```

