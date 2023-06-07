# Comparing `tmp/tdnpathviz-0.1.2.6-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 379221 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 08:36 tdnpathviz/__init__.py
+Zip file size: 381405 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 09:19 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat    13558 b- defN 23-Jun-07 08:44 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat    24150 b- defN 23-Jun-07 09:24 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      266 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 08:47 tdnpathviz-0.1.2.6.dist-info/RECORD
-9 files, 2195190 bytes uncompressed, 377971 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      724 b- defN 23-Jun-07 09:29 tdnpathviz-0.1.2.7.dist-info/RECORD
+9 files, 2205831 bytes uncompressed, 380155 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.6.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.7.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.6.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.6.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.6.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.6'
+__version__ = '0.1.2.7'
```

## tdnpathviz/visualizations.py

```diff
@@ -1,11 +1,15 @@
 import plotly.graph_objects as go
 import random
 import teradataml as tdml
-
+import io
+from IPython.display import Image
+import imageio
+import matplotlib.pyplot as plt
+import seaborn as sns
 
 import random  # Importing the random module for random number generation
 
 def colors(n, alpha=0.8, random_seed=124):
     """
     Generates a list of n colors in the form of RGBA strings.
 
@@ -328,8 +332,313 @@
     --ORDER BY "path","index"
     ) CC
     GROUP BY 1,2,3,4,5
     """
     tdml.get_context().execute(query)
     print(f'npath view created : {graph_aggregated_npath_view}')
 
-    return
+    return
+
+
+
+
+
+def scatter_plot(tddf, x_col, y_col, **kwargs):
+    """
+    This function generates a scatter plot based on the given parameters.
+    This function used TD_PLOT so requires Teradata 17.20 or later versions.
+
+    Parameters
+    ----------
+    tddf : teradata DataFrame
+        The DataFrame from which the plot will be generated.
+    x_col : str
+        The column of the DataFrame to use as the x-axis.
+    y_col : str
+        The column of the DataFrame to use as the y-axis.
+    **kwargs :
+        Additional optional parameters can be set as follows:
+
+        width : int, optional
+            The width of the plot, defaults to 600.
+        height : int, optional
+            The height of the plot, defaults to 600.
+        row_axis_type : str, optional
+            The type of axis, defaults to 'SEQUENCE'.
+        series_id : str or list, optional
+            The id(s) of the series, defaults to None.
+        color : str, optional
+            The color of the marker, defaults to 'b'.
+        marker : str, optional
+            The shape of the marker, defaults to 'o'.
+        markersize : int, optional
+            The size of the marker, defaults to 3.
+        noplot : bool, optional
+            If True, the plot will not be displayed, defaults to False.
+        title : str, optional
+            The title of the plot, defaults to '{y_col} Vs. {x_col}'.
+
+    Returns
+    -------
+    Image
+        either the image read from the stream or the Image object object containing the scatter plot (depending on the "no_plot" option).
+    """
+
+    # Fetch keyword arguments with default values
+    width = kwargs.get('width', 600)
+    height = kwargs.get('height', 600)
+    row_axis_type = kwargs.get('row_axis_type', 'SEQUENCE')
+    series_id = kwargs.get('series_id', None)
+    color = kwargs.get('color', 'b')
+    marker = kwargs.get('marker', 'o')
+    markersize = kwargs.get('markersize', 3)
+    noplot = kwargs.get('noplot', False)
+    title = kwargs.get('title', f'{y_col} Vs. {x_col}')
+
+    # If no series id is provided, a default one is created
+    if series_id is None:
+        tddf = tddf.assign(series_id=1)
+        series_id = 'series_id'
+
+    n = 1
+    # If series_id is a list, its length is stored and it's joined into a comma-separated string
+    if type(series_id) == list:
+        n = len(series_id)
+        series_id = ','.join(series_id)
+
+    # This line is specific to teradata DataFrame structure,
+    # it aims to be sure the name of the temporary view is available
+    tddf._DataFrame__execute_node_and_set_table_name(tddf._nodeid, tddf._metaexpr)
+
+    # SQL query to be executed using TD_PLOT
+    query = f"""
+    EXECUTE FUNCTION
+        TD_PLOT(
+            SERIES_SPEC(
+            TABLE_NAME({tddf._table_name}),
+            ROW_AXIS({row_axis_type}({x_col})),
+            SERIES_ID({series_id}),
+            PAYLOAD (
+                FIELDS({y_col}),
+                CONTENT(REAL)
+            )
+        ),
+        FUNC_PARAMS(
+        TITLE('{title}'),
+        PLOTS[(
+        TYPE('scatter'),
+        MARKER('{marker}'),
+        MARKERSIZE({markersize})
+        --COLOR('{color}')
+        )],
+        WIDTH({width}),
+        HEIGHT({height})
+        )
+        );
+    """
+
+    # If enabled, print the SQL query
+    if tdml.display.print_sqlmr_query:
+        print(query)
+
+    # Execute the query and fetch the result
+    res = tdml.get_context().execute(query).fetchall()
+
+    stream_str = io.BytesIO(res[0][1 + n])
+
+    # Return either the image read from the stream or the Image object
+    if noplot:
+        return imageio.imread(stream_str.getvalue())
+    else:
+        return Image(stream_str.getvalue())
+
+
+def pair_plot(tddf, **kwargs):
+    """
+    This function generates a pair plot based on the given parameters.
+    This function used TD_PLOT so requires Teradata 17.20 or later versions.
+
+    Parameters
+    ----------
+    tddf : teradata DataFrame
+        The DataFrame from which the plot will be generated.
+    **kwargs :
+        Additional optional parameters can be set as follows:
+
+        width : int, optional
+            The width of the plot, defaults to 600.
+        height : int, optional
+            The height of the plot, defaults to 600.
+        row_axis_type : str, optional
+            The type of axis, defaults to 'SEQUENCE'.
+        series_id : str or list, optional
+            The id(s) of the series, defaults to None.
+        color : str, optional
+            The color of the marker, defaults to 'b'.
+        marker : str, optional
+            The shape of the marker, defaults to 'o'.
+        noplot : bool, optional
+            If True, the plot will not be displayed, defaults to False.
+        title : str, optional
+            The title of the plot, defaults to 'pairplot'.
+        markersize : int, optional
+            The size of the marker, defaults to 3.
+
+    Returns
+    -------
+    Image
+        An Image object containing the pair plot.
+    """
+
+    # Fetch keyword arguments with default values
+    width = kwargs.get('width', 600)
+    height = kwargs.get('height', 600)
+    row_axis_type = kwargs.get('row_axis_type', 'SEQUENCE')
+    series_id = kwargs.get('series_id', None)
+    color = kwargs.get('color', 'b')
+    marker = kwargs.get('marker', 'o')
+    noplot = kwargs.get('noplot', False)
+    title = kwargs.get('title', 'pairplot')
+    markersize = kwargs.get('markersize', 3)
+
+    # If no series id is provided, a default one is created
+    if series_id is None:
+        tddf = tddf.assign(series_id=1)
+        series_id = 'series_id'
+
+    n = 1
+    # If series_id is a list, its length is stored and it's joined into a comma-separated string
+    if type(series_id) == list:
+        n = len(series_id)
+        series_id = ','.join(series_id)
+
+    # This line is specific to teradata DataFrame structure,
+    # it aims to be sure the name of the temporary view is available
+    tddf._DataFrame__execute_node_and_set_table_name(tddf._nodeid, tddf._metaexpr)
+
+    # Determine which columns to include in the plot
+    if type(series_id) == list:
+        columns = [c for c in list(tddf.columns) if c not in series_id]
+    else:
+        columns = [c for c in list(tddf.columns) if c not in [series_id]]
+
+    series_blocks = []
+    plot_blocks = []
+    counter = 0
+
+    # For each pair of columns, add a block to the series_blocks and plot_blocks lists
+    for i, c_row in enumerate(columns):
+        for j, c_col in enumerate(columns):
+            if i < j:
+                counter += 1
+                # Series block for the SQL query
+                series_block = f"""
+                SERIES_SPEC(
+                TABLE_NAME({tddf._table_name}),
+                ROW_AXIS({row_axis_type}({c_row})),
+                SERIES_ID({series_id}),
+                PAYLOAD (
+                    FIELDS({c_col}),
+                    CONTENT(REAL)
+                ))"""
+                series_blocks.append(series_block)
+
+                # Plot block for the SQL query
+                plot_block = f"""
+                (
+                    ID({counter}),
+                    CELL({i + 1},{j}),
+                    TYPE('scatter'),
+                    MARKER('{marker}'),
+                    MARKERSIZE({markersize})
+                    --COLOR('{color}')
+                    )
+                """
+                plot_blocks.append(plot_block)
+
+    series_blocks = ',\n'.join(series_blocks)
+    plot_blocks = ',\n'.join(plot_blocks)
+
+    # SQL query to be executed
+    query = f"""
+    EXECUTE FUNCTION
+        TD_PLOT(
+            {series_blocks}
+        ,
+        FUNC_PARAMS(
+        LAYOUT({len(columns) - 1},{len(columns) - 1}),
+        TITLE('{title}'),
+        WIDTH({width}),
+        HEIGHT({height}),
+        PLOTS[
+            {plot_blocks}
+        ]
+        )
+        );
+    """
+
+    # If enabled, print the SQL query
+    if tdml.display.print_sqlmr_query:
+        print(query)
+
+    # Execute the query and fetch the result
+    res = tdml.get_context().execute(query).fetchall()
+
+    stream_str = io.BytesIO(res[0][1 + n])
+
+    # Return either the image read from the stream or the Image object
+    if noplot:
+        return imageio.imread(stream_str.getvalue())
+    else:
+        return Image(stream_str.getvalue())
+
+
+def plot_correlation_heatmap(tddf, **kwargs):
+    """
+    This function calculates the correlation matrix of a DataFrame and plots a heatmap of it.
+    It requires Vantage Analytic Library installed with the rights to execute its functions.
+
+    Parameters
+    ----------
+    tddf : teradata DataFrame
+        The DataFrame for which the correlation matrix will be calculated and plotted.
+    **kwargs :
+        Additional optional parameters can be set as follows:
+
+        ax : matplotlib axis, optional
+            The axis on which the plot will be displayed. If none is given, the current axis will be used. Defaults to None.
+        no_plot : bool, optional
+            If True, the plot will not be displayed, and the function will return the correlation matrix. Defaults to False.
+        title : str, optional
+            The title of the plot, defaults to an empty string.
+
+    Returns
+    -------
+    DataFrame or None
+        If no_plot is True, a DataFrame containing the correlation matrix is returned.
+        Otherwise, None is returned, and a heatmap of the correlation matrix is plotted.
+    """
+
+    # Fetch keyword arguments with default values
+    ax = kwargs.get('ax', None)
+    no_plot = kwargs.get('no_plot', False)
+    title = kwargs.get('title', '')
+
+    # compute the correlation matrix in-db
+    obj = tdml.valib.Matrix(data=tddf,
+                       columns=list(tddf.columns),
+                       type="COR")
+
+    # download the result
+    val_corr_matrix = obj.result.to_pandas().reset_index().drop('rownum', axis=1).set_index('rowname').loc[
+                      list(tddf.columns), :]
+
+    # plot the heatmap
+    if no_plot:
+        return val_corr_matrix
+    else:
+        if ax != None:
+            sns.heatmap(val_corr_matrix, annot=True, cmap='coolwarm', ax=ax)
+            ax.set_title(title)
+        else:
+            sns.heatmap(val_corr_matrix, annot=True, cmap='coolwarm')
+            plt.title(title)
```

## Comparing `tdnpathviz-0.1.2.6.dist-info/RECORD` & `tdnpathviz-0.1.2.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tdnpathviz/__init__.py,sha256=YiBCz8xwaogZDfIC0Z5S9EmhIrnSlxGqGaSYi-ZHwCs,23
+tdnpathviz/__init__.py,sha256=9BmWlJ9mets8moEWokf_dhefUjU7G7N4DCcife5EY_M,23
 tdnpathviz/datasets.py,sha256=XASLSjLtaHMZq-uPArgCLjbGapxDI2CJ2i0gSu9KW8M,991
 tdnpathviz/utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tdnpathviz/visualizations.py,sha256=jJAZCnCTb27JKr1zObmXANE7H-dxOOKvIJ6t5lUj9zM,13558
+tdnpathviz/visualizations.py,sha256=QjBfDx46EZFCYMR_rYRO4ClCkkOVUkyCM1h2oRKsEjc,24150
 tdnpathviz/data/train_dataset.csv,sha256=ko9f4sY4Cglvfii921mOnb01gAqP_EOhgKe12UdX9Pg,2179525
-tdnpathviz-0.1.2.6.dist-info/METADATA,sha256=vkFBMkEcBRQohGWSIDyx-QLKyDjMckyyW8teDw8MFic,266
-tdnpathviz-0.1.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tdnpathviz-0.1.2.6.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
-tdnpathviz-0.1.2.6.dist-info/RECORD,,
+tdnpathviz-0.1.2.7.dist-info/METADATA,sha256=eNTaX4OBb-23Ni2dpkJVOEhuWIFC7GPau-xgkYo9sD8,315
+tdnpathviz-0.1.2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tdnpathviz-0.1.2.7.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
+tdnpathviz-0.1.2.7.dist-info/RECORD,,
```

