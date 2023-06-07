# Comparing `tmp/tdnpathviz-0.1.2.7-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 381405 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 09:19 tdnpathviz/__init__.py
+Zip file size: 381451 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 12:54 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat    24150 b- defN 23-Jun-07 09:24 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat    24197 b- defN 23-Jun-07 12:52 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/RECORD
-9 files, 2205831 bytes uncompressed, 380155 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 12:54 tdnpathviz-0.1.2.8.dist-info/RECORD
+9 files, 2205878 bytes uncompressed, 380201 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.7.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.8.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.7.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.7.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.7.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.7'
+__version__ = '0.1.2.8'
```

## tdnpathviz/visualizations.py

```diff
@@ -108,43 +108,45 @@
         FROM {df_agg._table_name} A
         QUALIFY id < {nb_paths}+1"""
 
     df_selection = tdml.DataFrame.from_query(query)
 
     if justify == 'left':
         justify_query = 'AAA.id_end_temp AS id_end'
+        ascending     = ''
     elif justify == 'right':
-        justify_query = '''AAA.id_end_temp + max_max_path_length - max_path_length as id_end'''
+        justify_query = '''AAA.id_end_temp as id_end'''
+        ascending     = ' DESC'
 
     query2 = f"""
     sel
         CC.id
-    ,	CC.node_source
+    ,   CC.node_source
     ,	CC.node_target
     ,	CC.beg
     ,	CC."end"
     ,	sum(CC.weight) as weight
     FROM 
     (
     sel
         B.*
-    ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."path",B."index") as id_beg
+    ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."index") as id_beg
     ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(200))) as node_source
     ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(200))) as node_target
     FROM 
     (
         SEL
             AAA.*
         ,   {justify_query}
         ,   MAX(AAA.id_end_temp) OVER (PARTITION BY AAA."path") AS max_path_length
         ,   MAX(AAA.id_end_temp) OVER (PARTITION BY 1) AS max_max_path_length
         FROM (
             sel 
                 A.*
-            ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end_temp
+            ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."index" {ascending}) as id_end_temp
             from (
                 SELECT
         
                     lag(AA.token,1) IGNORE NULLS OVER (PARTITION BY AA.outkey ORDER BY AA.tokennum) as "beg"
                 ,	AA.token as "end"
                 ,	AA.outkey as "path"
                 ,	B.weight
@@ -172,15 +174,15 @@
     if print_query:
         print(query2)
 
     df_ready = tdml.DataFrame.from_query(query2)
 
     df_ready_local = df_ready.to_pandas()
 
-    df_ready_local = df_ready_local.sort_values(by='id')
+    df_ready_local = df_ready_local.sort_values(by=['id','node_source','node_target'])
 
     labs = dict()
     labels = list(set(df_ready_local.node_source.tolist() + df_ready_local.node_target.tolist()))
 
     for i, label in enumerate(labels):
         labs[label] = i
```

