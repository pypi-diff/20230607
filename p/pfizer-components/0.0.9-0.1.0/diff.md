# Comparing `tmp/pfizer_components-0.0.9-py3-none-any.whl.zip` & `tmp/pfizer_components-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 29658 bytes, number of entries: 15
+Zip file size: 29676 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     5539 b- defN 23-Jun-07 10:59 pfizer_components/Accordion.py
 -rw-rw-rw-  2.0 fat     3222 b- defN 23-Jun-07 10:59 pfizer_components/Breadcrumb.py
 -rw-rw-rw-  2.0 fat    56916 b- defN 23-Jun-07 10:59 pfizer_components/Cards.py
 -rw-rw-rw-  2.0 fat     4720 b- defN 23-Jun-07 10:59 pfizer_components/Carousel.py
 -rw-rw-rw-  2.0 fat    29164 b- defN 23-Jun-07 10:59 pfizer_components/Components.py
 -rw-rw-rw-  2.0 fat    16122 b- defN 23-Jun-07 10:58 pfizer_components/Graph.py
 -rw-rw-rw-  2.0 fat     8653 b- defN 23-Jun-07 10:46 pfizer_components/Navigation.py
 -rw-rw-rw-  2.0 fat     6951 b- defN 23-Jun-07 10:58 pfizer_components/Toast.py
 -rw-rw-rw-  2.0 fat     2680 b- defN 23-Jun-07 10:59 pfizer_components/Usage_css.py
 -rw-rw-rw-  2.0 fat     2706 b- defN 23-Jun-07 10:59 pfizer_components/Usage_python.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-Jun-07 10:59 pfizer_components/__init__.py
--rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-07 11:10 pfizer_components-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 11:10 pfizer_components-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       29 b- defN 23-Jun-07 11:10 pfizer_components-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1288 b- defN 23-Jun-07 11:10 pfizer_components-0.0.9.dist-info/RECORD
-15 files, 138707 bytes uncompressed, 27516 bytes compressed:  80.2%
+-rw-rw-rw-  2.0 fat      366 b- defN 23-Jun-07 11:24 pfizer_components/__init__.py
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Jun-07 11:30 pfizer_components-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 11:30 pfizer_components-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       29 b- defN 23-Jun-07 11:30 pfizer_components-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1288 b- defN 23-Jun-07 11:30 pfizer_components-0.1.0.dist-info/RECORD
+15 files, 138829 bytes uncompressed, 27534 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: pfizer_components/Usage_python.py
 Comment: 
 
 Filename: pfizer_components/__init__.py
 Comment: 
 
-Filename: pfizer_components-0.0.9.dist-info/METADATA
+Filename: pfizer_components-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pfizer_components-0.0.9.dist-info/WHEEL
+Filename: pfizer_components-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pfizer_components-0.0.9.dist-info/top_level.txt
+Filename: pfizer_components-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pfizer_components-0.0.9.dist-info/RECORD
+Filename: pfizer_components-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pfizer_components/__init__.py

```diff
@@ -1,5 +1,8 @@
 from pfizer_components.Components import Button, Checkbox, Dropdown, Input
 from pfizer_components.Cards import *
 from pfizer_components.Carousel import *
 from pfizer_components.Accordion import *
 from pfizer_components.Breadcrumb import *
+from pfizer_components.Toast import *
+from pfizer_components.Navigation import *
+from pfizer_components.Graph import *
```

## Comparing `pfizer_components-0.0.9.dist-info/RECORD` & `pfizer_components-0.1.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 pfizer_components/Carousel.py,sha256=HyEsHuAO9J_alJJo70HkbOzWoyFVUi_1-DDGT0r1A3w,4720
 pfizer_components/Components.py,sha256=vm3RaqWyEd0NLgcwreSPocjpqQMBu1As95nY2XnQin0,29164
 pfizer_components/Graph.py,sha256=gspV9nvbQAOcTyEj43WwqGnfehS7ZdeRj2O9Adhrn8U,16122
 pfizer_components/Navigation.py,sha256=LvRAz3PaXo4HA-KRHTrnUHLxcb5aNkU2O9vnRYpjjP8,8653
 pfizer_components/Toast.py,sha256=DXCNz3tcod6Q3NfS3L3BFa_1kTNdJVKzTskP9KBUoPs,6951
 pfizer_components/Usage_css.py,sha256=-F23a74K7TPNbcHrQVKWPBoJJzpAmNSboamRAu8AQiI,2680
 pfizer_components/Usage_python.py,sha256=GQmhYxMhv-VkaI0ej6VMdjg2PSoopzaRbC4BfHE83jk,2706
-pfizer_components/__init__.py,sha256=DUVYuQ8UKGppmrooYS0h0gT-4MGlh1v-HfpjbBwRojE,244
-pfizer_components-0.0.9.dist-info/METADATA,sha256=NK0shAIYE-Oww9HO37vxIy9Um5LwUGjxiMnntqxINkc,381
-pfizer_components-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pfizer_components-0.0.9.dist-info/top_level.txt,sha256=aTa_jkDnegljBrbkpUpV-7BZlC0JlnD5B1ch3nmeXIY,29
-pfizer_components-0.0.9.dist-info/RECORD,,
+pfizer_components/__init__.py,sha256=BmghHDd1vexRUSYE0ya8WG34n5b5lsXwvIW8Ptz2WsQ,366
+pfizer_components-0.1.0.dist-info/METADATA,sha256=nnqmkDWpvTgY4QAaKbcE7Wanc06uRgttf82f9bspA6s,381
+pfizer_components-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pfizer_components-0.1.0.dist-info/top_level.txt,sha256=aTa_jkDnegljBrbkpUpV-7BZlC0JlnD5B1ch3nmeXIY,29
+pfizer_components-0.1.0.dist-info/RECORD,,
```

