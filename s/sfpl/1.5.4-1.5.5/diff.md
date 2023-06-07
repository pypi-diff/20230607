# Comparing `tmp/sfpl-1.5.4-py3-none-any.whl.zip` & `tmp/sfpl-1.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11274 bytes, number of entries: 8
+Zip file size: 11427 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      781 b- defN 23-Jun-06 22:54 sfpl/__init__.py
 -rw-r--r--  2.0 unx     2215 b- defN 23-Jun-06 22:54 sfpl/exceptions.py
--rw-r--r--  2.0 unx    29997 b- defN 23-Jun-07 03:18 sfpl/sfpl.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4212 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/RECORD
-8 files, 38960 bytes uncompressed, 10258 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx    30612 b- defN 23-Jun-07 03:39 sfpl/sfpl.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     4212 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-07 03:42 sfpl-1.5.5.dist-info/RECORD
+8 files, 39575 bytes uncompressed, 10411 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: sfpl/exceptions.py
 Comment: 
 
 Filename: sfpl/sfpl.py
 Comment: 
 
-Filename: sfpl-1.5.4.dist-info/LICENSE.md
+Filename: sfpl-1.5.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: sfpl-1.5.4.dist-info/METADATA
+Filename: sfpl-1.5.5.dist-info/METADATA
 Comment: 
 
-Filename: sfpl-1.5.4.dist-info/WHEEL
+Filename: sfpl-1.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: sfpl-1.5.4.dist-info/top_level.txt
+Filename: sfpl-1.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sfpl-1.5.4.dist-info/RECORD
+Filename: sfpl-1.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sfpl/sfpl.py

```diff
@@ -715,70 +715,76 @@
 
 
 class Branch:
     """A library branch.
 
     Attributes:
         name (str): The name of the library branch.
+        _id (str): SFPL's ID for the library branch.
     """
-    BRANCHES = (
-        'anza',
-        'bayview',
-        'bernal heights',
-        'chinatown',
-        'eureka valley',
-        'excelsior',
-        'glen park',
-        'golden gate valley',
-        'ingleside',
-        'main library',
-        'marina',
-        'merced',
-        'mission',
-        'mission bay',
-        'noe valley',
-        'north beach',
-        'ocean view',
-        'ortega',
-        'park',
-        'parkside',
-        'portola',
-        'potrero',
-        'presidio',
-        'richmond',
-        'sunset',
-        'visitacion valley',
-        'west portal',
-        'western addition',
-    )
+    BRANCHES = {
+        'anza': '44563120',
+        'bayview': '44563121',
+        'bernal heights': '44563122',
+        'chinatown': '44563123',
+        "chinatown children's": '44563124',
+        'eureka valley': '44563125',
+        'excelsior': '44563126',
+        'glen park': '44563127',
+        'golden gate valley': '44563128',
+        'ingleside': '44563130',
+        'main library': '44563151',
+        'marina': '44563131',
+        'merced': '44563132',
+        'mission': '44563133',
+        'mission bay': '44563134',
+        'noe valley': '44563135',
+        'north beach': '44563136',
+        'ocean view': '44563137',
+        'ortega': '44563138',
+        'park': '44563139',
+        'parkside': '44563140',
+        'portola': '44563141',
+        'potrero': '44563142',
+        'presidio': '44563143',
+        'richmond': '44563144',
+        "richmond children's": '44563145',
+        'sunset': '44563146',
+        "sunset children's": '44563147',
+        'visitacion valley': '44563148',
+        'west portal': '44563149',
+        'western addition': '44563150',
+    }
 
     def __init__(self, name):
         """
         Args:
             name (str): Name of library branch to match.
 
         Raises:
             NoBranchFound: No matches for the given name were found.
         """
         for branch in Branch.BRANCHES:
             if name.lower() in branch.lower():
                 self.name = branch
+                self._id = Branch.BRANCHES[self.name]
                 break
 
         else:
             raise exceptions.NoBranchFound(name)
 
     def getHours(self):
         """Get the operating hours of the library.
 
         Returns:
             dict: A dictionary mapping days of the week to operating hours.
         """
         branch = (
             self.name
+                .replace(" children's", '')
                 .replace(' ', '-')
                 .lower()
         )
         response = requests.get(f'https://sfpl.org/locations/{branch}')
         response.raise_for_status()
         soup = BeautifulSoup(response.text, 'lxml')
         result = {}
```

## Comparing `sfpl-1.5.4.dist-info/LICENSE.md` & `sfpl-1.5.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `sfpl-1.5.4.dist-info/METADATA` & `sfpl-1.5.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfpl
-Version: 1.5.4
+Version: 1.5.5
 Summary: Unofficial Python API for SFPL
 Home-page: https://github.com/kajchang/sfpl-scraper
 Author: Kai Chang
 Author-email: kaijchang@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

