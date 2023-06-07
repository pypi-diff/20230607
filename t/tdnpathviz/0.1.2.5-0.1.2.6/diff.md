# Comparing `tmp/tdnpathviz-0.1.2.5-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 379078 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-30 10:18 tdnpathviz/__init__.py
+Zip file size: 379221 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 08:36 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat    12050 b- defN 23-May-30 10:34 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat    13558 b- defN 23-Jun-07 08:44 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      266 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      724 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/RECORD
-9 files, 2193682 bytes uncompressed, 377828 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      266 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/RECORD
+9 files, 2195190 bytes uncompressed, 377971 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.5.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.6.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.5.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.5.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.5.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.5'
+__version__ = '0.1.2.6'
```

## tdnpathviz/visualizations.py

```diff
@@ -43,15 +43,15 @@
         ret.append("rgba(" + str(r) + "," + str(g) + "," + str(b) + "," + str(alpha) + ")")
 
     return ret  # Return the list of generated colors
 
 
 
 def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15, print_query=False,
-                          font_size=10, width=1200, height=800, weight_column = None, weight_agg = 'count'):
+                          font_size=10, width=1200, height=800, weight_column = None, weight_agg = 'count', justify='left'):
     """
         Plots the first main paths based on a given output of the teradataml NPATH function or the teradataml dataframe of its result field.
 
         Parameters:
         - myPathAnalysis (DataFrame or tdml.dataframe.dataframe.DataFrame): The input DataFrame containing path analysis data.
         - path_column (str, optional): The column name representing the path. Defaults to 'mypath'.
         - id_column (str or list, optional): The column name(s) representing the unique identifier(s). Defaults to 'travelid'.
@@ -61,14 +61,15 @@
         - width (int, optional): define the width of the figure. Defaults is 1200.
         - height (int, optional): define the height of the figure. Defaults is 800.
         - weight_column (str, optional): define the column to aggregate. If None, just count the number of pathes.
           Default is None.
         - weight_agg (str, optional): when weight_column is not None, then the weight is the result of the aggregation
           defined by weight_agg on the weight_column. Permitted values are 'count', 'avg', 'max', 'min', 'sum'.
           Default is 'count'.
+        - justify (str, optional): define if you want to justify 'right' or 'left' the output sankey. Defaults is 'left'.
 
         Returns:
         - None (it display an interactive Sankey plot)
     """
     if type(id_column) != list:
         id_column = [id_column]
 
@@ -101,14 +102,19 @@
         ,	REGEXP_REPLACE(lower(A.{path_column}),'\\[|\\]', '') as str
         ,	{weight_agg}_{weight_column} as weight
         FROM {df_agg._table_name} A
         QUALIFY id < {nb_paths}+1"""
 
     df_selection = tdml.DataFrame.from_query(query)
 
+    if justify == 'left':
+        justify_query = 'AAA.id_end_temp AS id_end'
+    elif justify == 'right':
+        justify_query = '''AAA.id_end_temp + max_max_path_length - max_path_length as id_end'''
+
     query2 = f"""
     sel
         CC.id
     ,	CC.node_source
     ,	CC.node_target
     ,	CC.beg
     ,	CC."end"
@@ -118,38 +124,45 @@
     sel
         B.*
     ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."path",B."index") as id_beg
     ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(200))) as node_source
     ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(200))) as node_target
     FROM 
     (
-        sel 
-            A.*
-        ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end
-        from (
-        SELECT
-
-            lag(AA.token,1) IGNORE NULLS OVER (PARTITION BY AA.outkey ORDER BY AA.tokennum) as "beg"
-        ,	AA.token as "end"
-        ,	AA.outkey as "path"
-        ,	B.weight
-        ,	AA.tokennum as "index"
-        ,   B.id
+        SEL
+            AAA.*
+        ,   {justify_query}
+        ,   MAX(AAA.id_end_temp) OVER (PARTITION BY AAA."path") AS max_path_length
+        ,   MAX(AAA.id_end_temp) OVER (PARTITION BY 1) AS max_max_path_length
         FROM (
-
-        SELECT 
-            d.*
-        FROM TABLE (strtok_split_to_table({df_selection._table_name}.id, {df_selection._table_name}.str, ',')
-        RETURNS (outkey integer, tokennum integer, token varchar(200)character set unicode) ) as d 
-
-        ) AA
-        ,{df_selection._table_name} B
-        WHERE AA.outkey = B.id
-        QUALIFY beg IS NOT NULL
-    ) A
+            sel 
+                A.*
+            ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end_temp
+            from (
+                SELECT
+        
+                    lag(AA.token,1) IGNORE NULLS OVER (PARTITION BY AA.outkey ORDER BY AA.tokennum) as "beg"
+                ,	AA.token as "end"
+                ,	AA.outkey as "path"
+                ,	B.weight
+                ,	AA.tokennum as "index"
+                ,   B.id
+                FROM (
+        
+                    SELECT 
+                        d.*
+                    FROM TABLE (strtok_split_to_table({df_selection._table_name}.id, {df_selection._table_name}.str, ',')
+                    RETURNS (outkey integer, tokennum integer, token varchar(200)character set unicode) ) as d 
+            
+                    ) AA
+                ,{df_selection._table_name} B
+                WHERE AA.outkey = B.id
+                QUALIFY beg IS NOT NULL
+            ) A
+        ) AAA
     ) B
     --ORDER BY "path","index"
     ) CC
     GROUP BY 1,2,3,4,5
     """
 
     if print_query:
@@ -191,24 +204,25 @@
                       height=height)
     fig.show()
 
     return
 
 def create_all_pathes_views(myPathAnalysis, root_name = 'mytest',
                             schema = tdml.get_context().execute('SELECT DATABASE').fetchall()[0][0],
-                            path_column='mypath', id_column='travelid'):
+                            path_column='mypath', id_column='travelid', justify = 'left'):
     """
         Creates multiple views related to the given myPathAnalysis DataFrame.
 
         Parameters:
         - myPathAnalysis (DataFrame or tdml.dataframe.dataframe.DataFrame): The input DataFrame containing path analysis data.
         - root_name (str, optional): The root name to be used for naming the created views. Defaults to 'mytest'.
         - schema (str, optional): The schema to create the views in. Defaults to the current database schema.
         - path_column (str, optional): The column name representing the path. Defaults to 'mypath'.
         - id_column (str or list, optional): The column name(s) representing the unique identifier(s). Defaults to 'travelid'.
+        - justify (str, optional): define if you want to justify 'right' or 'left' the output sankey. Defaults is 'left'.
 
         Returns:
         - None
     """
 
     if type(id_column) != list:
         id_column = [id_column]
@@ -251,14 +265,20 @@
         row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column[0]} DESC) as id
     ,	REGEXP_REPLACE(lower(A.{path_column}),'\[|\]', '') as str
     ,	count_{id_column[0]} as weight
     FROM {aggregated_npath_view} A"""
     tdml.get_context().execute(query)
     print(f'clean aggregated npath view created : {clean_aggregated_npath_view}')
 
+    if justify == 'left':
+        justify_query = 'AAA.id_end_temp AS id_end'
+    elif justify == 'right':
+        justify_query = '''AAA.id_end_temp + max_max_path_length - max_path_length as id_end'''
+
+
     # Create the graph view of the aggregated npath view
     graph_aggregated_npath_view =  f"{schema}.{root_name}_GRAPH_NPATH_VIEW_AGG"
     query = f"""
     REPLACE VIEW {graph_aggregated_npath_view} AS
     SELECT
         CC.id
     ,	CC.node_source
@@ -271,36 +291,43 @@
     sel
         B.*
     ,	LAG(id_end,1,0) OVER (PARTITION BY B."path" ORDER BY B."path",B."index") as id_beg
     ,	B."beg" || '_' || TRIM(CAST(id_beg AS VARCHAR(10))) as node_source
     ,	B."end" || '_' || TRIM(CAST(id_end AS VARCHAR(10))) as node_target
     FROM 
         (
-        sel 
-            A.*
-        ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end
-        from (
-            SELECT
-    
-                lag(AA.token,1) IGNORE NULLS OVER (PARTITION BY AA.outkey ORDER BY AA.tokennum) as "beg"
-            ,	AA.token as "end"
-            ,	AA.outkey as "path"
-            ,	B.weight
-            ,	AA.tokennum as "index"
-            ,   B.id
-            FROM (
-                SELECT 
-                    d.*
-                FROM TABLE (strtok_split_to_table({clean_aggregated_npath_view}.id, {clean_aggregated_npath_view}.str, ',')
-                RETURNS (outkey integer, tokennum integer, token varchar(20)character set unicode) ) as d 
-            ) AA
-            ,   {clean_aggregated_npath_view} B
-            WHERE AA.outkey = B.id
-            QUALIFY beg IS NOT NULL
-        ) A
+        SEL
+            AAA.*
+        ,   {justify_query}
+        ,   MAX(AAA.id_end_temp) OVER (PARTITION BY AAA."path") AS max_path_length
+        ,   MAX(AAA.id_end_temp) OVER (PARTITION BY 1) AS max_max_path_length
+        FROM (
+            sel 
+                A.*
+            ,	row_number() OVER (PARTITION BY A."path" ORDER BY A."path",A."index") as id_end_temp
+            from (
+                SELECT
+        
+                    lag(AA.token,1) IGNORE NULLS OVER (PARTITION BY AA.outkey ORDER BY AA.tokennum) as "beg"
+                ,	AA.token as "end"
+                ,	AA.outkey as "path"
+                ,	B.weight
+                ,	AA.tokennum as "index"
+                ,   B.id
+                FROM (
+                    SELECT 
+                        d.*
+                    FROM TABLE (strtok_split_to_table({clean_aggregated_npath_view}.id, {clean_aggregated_npath_view}.str, ',')
+                    RETURNS (outkey integer, tokennum integer, token varchar(20)character set unicode) ) as d 
+                ) AA
+                ,   {clean_aggregated_npath_view} B
+                WHERE AA.outkey = B.id
+                QUALIFY beg IS NOT NULL
+            ) A
+        ) AAA
        ) B
     --ORDER BY "path","index"
     ) CC
     GROUP BY 1,2,3,4,5
     """
     tdml.get_context().execute(query)
     print(f'npath view created : {graph_aggregated_npath_view}')
```

## Comparing `tdnpathviz-0.1.2.5.dist-info/RECORD` & `tdnpathviz-0.1.2.6.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tdnpathviz/__init__.py,sha256=IxHn7mJsooF4Nc95xzZMmWnoxCVB5QRVByOksR-DxZQ,23
+tdnpathviz/__init__.py,sha256=YiBCz8xwaogZDfIC0Z5S9EmhIrnSlxGqGaSYi-ZHwCs,23
 tdnpathviz/datasets.py,sha256=XASLSjLtaHMZq-uPArgCLjbGapxDI2CJ2i0gSu9KW8M,991
 tdnpathviz/utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tdnpathviz/visualizations.py,sha256=XPtiDY1augAyu-KtGOsu9lJwNAMjp94ysqtqX8l3QAE,12050
+tdnpathviz/visualizations.py,sha256=jJAZCnCTb27JKr1zObmXANE7H-dxOOKvIJ6t5lUj9zM,13558
 tdnpathviz/data/train_dataset.csv,sha256=ko9f4sY4Cglvfii921mOnb01gAqP_EOhgKe12UdX9Pg,2179525
-tdnpathviz-0.1.2.5.dist-info/METADATA,sha256=DzY3lqk-FU8J1j6aGJS7yOTuYaJ7YEgDNfjjPAnYkyc,266
-tdnpathviz-0.1.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tdnpathviz-0.1.2.5.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
-tdnpathviz-0.1.2.5.dist-info/RECORD,,
+tdnpathviz-0.1.2.6.dist-info/METADATA,sha256=vkFBMkEcBRQohGWSIDyx-QLKyDjMckyyW8teDw8MFic,266
+tdnpathviz-0.1.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tdnpathviz-0.1.2.6.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
+tdnpathviz-0.1.2.6.dist-info/RECORD,,
```

