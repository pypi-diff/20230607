# Comparing `tmp/sfpl-1.5.3-py3-none-any.whl.zip` & `tmp/sfpl-1.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11585 bytes, number of entries: 8
+Zip file size: 11274 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      781 b- defN 23-Jun-06 22:54 sfpl/__init__.py
 -rw-r--r--  2.0 unx     2215 b- defN 23-Jun-06 22:54 sfpl/exceptions.py
--rw-r--r--  2.0 unx    31573 b- defN 23-Jun-06 23:00 sfpl/sfpl.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jun-06 23:04 sfpl-1.5.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4212 b- defN 23-Jun-06 23:04 sfpl-1.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 23:04 sfpl-1.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-06 23:04 sfpl-1.5.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-06 23:04 sfpl-1.5.3.dist-info/RECORD
-8 files, 40536 bytes uncompressed, 10569 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx    29997 b- defN 23-Jun-07 03:18 sfpl/sfpl.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     4212 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-07 03:18 sfpl-1.5.4.dist-info/RECORD
+8 files, 38960 bytes uncompressed, 10258 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: sfpl/exceptions.py
 Comment: 
 
 Filename: sfpl/sfpl.py
 Comment: 
 
-Filename: sfpl-1.5.3.dist-info/LICENSE.md
+Filename: sfpl-1.5.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: sfpl-1.5.3.dist-info/METADATA
+Filename: sfpl-1.5.4.dist-info/METADATA
 Comment: 
 
-Filename: sfpl-1.5.3.dist-info/WHEEL
+Filename: sfpl-1.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: sfpl-1.5.3.dist-info/top_level.txt
+Filename: sfpl-1.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sfpl-1.5.3.dist-info/RECORD
+Filename: sfpl-1.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sfpl/sfpl.py

```diff
@@ -715,65 +715,84 @@
 
 
 class Branch:
     """A library branch.
 
     Attributes:
         name (str): The name of the library branch.
-        _id (str): SFPL's ID for the library branch.
     """
+    BRANCHES = (
+        'anza',
+        'bayview',
+        'bernal heights',
+        'chinatown',
+        'eureka valley',
+        'excelsior',
+        'glen park',
+        'golden gate valley',
+        'ingleside',
+        'main library',
+        'marina',
+        'merced',
+        'mission',
+        'mission bay',
+        'noe valley',
+        'north beach',
+        'ocean view',
+        'ortega',
+        'park',
+        'parkside',
+        'portola',
+        'potrero',
+        'presidio',
+        'richmond',
+        'sunset',
+        'visitacion valley',
+        'west portal',
+        'western addition',
+    )
 
     def __init__(self, name):
         """
         Args:
             name (str): Name of library branch to match.
 
         Raises:
             NoBranchFound: No matches for the given name were found.
         """
-        branches = {'ANZA BRANCH': '44563120', 'BAYVIEW BRANCH': '44563121', 'BERNAL HEIGHTS BRANCH': '44563122',
-                    'CHINATOWN BRANCH': '44563123', "CHINATOWN CHILDREN'S": '44563124', 'EUREKA VALLEY BRANCH': '44563125',
-                    'EXCELSIOR BRANCH': '44563126', 'GLEN PARK BRANCH': '44563127', 'GOLDEN GATE VALLEY BRANCH': '44563128',
-                    'INGLESIDE BRANCH': '44563130', 'MAIN': '44563151', 'MARINA BRANCH': '44563131', 'MERCED BRANCH': '44563132',
-                    'MISSION': '44563133', 'MISSION BAY BRANCH': '44563134', 'NOE VALLEY': '44563135', 'NORTH BEACH BRANCH': '44563136',
-                    'OCEAN VIEW BRANCH': '44563137', 'ORTEGA BRANCH': '44563138', 'PARK BRANCH': '44563139', 'PARKSIDE BRANCH': '44563140',
-                    'PORTOLA BRANCH': '44563141', 'POTRERO BRANCH': '44563142', 'PRESIDIO BRANCH': '44563143', 'RICHMOND BRANCH': '44563144',
-                    "RICHMOND CHILDREN'S": '44563145', 'SUNSET BRANCH': '44563146', "SUNSET CHILDREN'S": '44563147',
-                    'VISITACION VALLEY BRANCH': '44563148', 'WESTERN ADDITION BRANCH': '44563150', 'WEST PORTAL BRANCH': '44563149'}
-
-        for branch in branches:
+        for branch in Branch.BRANCHES:
             if name.lower() in branch.lower():
                 self.name = branch
-                self._id = branches[self.name]
                 break
 
         else:
             raise exceptions.NoBranchFound(name)
 
     def getHours(self):
         """Get the operating hours of the library.
 
         Returns:
             dict: A dictionary mapping days of the week to operating hours.
         """
-        locations = {'ANZA BRANCH': '0100000301', 'BAYVIEW BRANCH': '0100000401', 'BERNAL HEIGHTS BRANCH': '0100002201',
-                     'CHINATOWN BRANCH': '0100000501', "CHINATOWN CHILDREN'S": '0100000501', 'EUREKA VALLEY BRANCH': '0100002301',
-                     'EXCELSIOR BRANCH': '0100000601', 'GLEN PARK BRANCH': '0100000701', 'GOLDEN GATE VALLEY BRANCH': '0100000801',
-                     'INGLESIDE BRANCH': '0100000901', 'MAIN': '0100000101', 'MARINA BRANCH': '0100001001',
-                     'MERCED BRANCH': '0100001101', 'MISSION': '0100000201', 'MISSION BAY BRANCH': '0100001201', 'NOE VALLEY': '0100001301',
-                     'NORTH BEACH BRANCH': '0100001401', 'OCEAN VIEW BRANCH': '0100001501', 'ORTEGA BRANCH': '0100001601',
-                     'PARK BRANCH': '0100001701', 'PARKSIDE BRANCH': '0100002401', 'PORTOLA BRANCH': '0100002701',
-                     'POTRERO BRANCH': '0100002501', 'PRESIDIO BRANCH': '0100002801', 'RICHMOND BRANCH': '0100002601',
-                     "RICHMOND CHILDREN'S": '0100002601', 'SUNSET BRANCH': '0100001801', "SUNSET CHILDREN'S": '0100001801',
-                     'VISITACION VALLEY BRANCH': '0100001901', 'WESTERN ADDITION BRANCH': '0100002101', 'WEST PORTAL BRANCH': '0100002001'}
-
-        schedhule = BeautifulSoup(requests.get('https://sfpl.org/index.php?pg={}'.format(
-            locations[self.name])).text, 'lxml')
+        branch = (
+            self.name
+                .replace(' ', '-')
+                .lower()
+        )
+        response = requests.get(f'https://sfpl.org/locations/{branch}')
+        response.raise_for_status()
+        soup = BeautifulSoup(response.text, 'lxml')
+        result = {}
+
+        for day in soup.select('.office-hours__item'):
+            day_of_week = day.select_one('.office-hours__item-label').text.strip()
+            hours = day.select_one('.office-hours__item-slots').text.strip()
+            result[day_of_week] = hours
 
-        return {k: v for (k, v) in zip([d.text for d in schedhule('abbr')], [h.text for h in schedhule('dd')[0:7]])}
+        return result
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return self.name
```

## Comparing `sfpl-1.5.3.dist-info/LICENSE.md` & `sfpl-1.5.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `sfpl-1.5.3.dist-info/METADATA` & `sfpl-1.5.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfpl
-Version: 1.5.3
+Version: 1.5.4
 Summary: Unofficial Python API for SFPL
 Home-page: https://github.com/kajchang/sfpl-scraper
 Author: Kai Chang
 Author-email: kaijchang@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

