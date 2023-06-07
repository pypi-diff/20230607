# Comparing `tmp/raphtory-0.3.2-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.4.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2928225 bytes, number of entries: 7
--rw-r--r--  4.6 unx     9737 b- defN 23-May-26 16:14 raphtory-0.3.2.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-May-26 16:14 raphtory-0.3.2.dist-info/WHEEL
--rw-r--r--  4.6 unx     2052 b- defN 23-May-26 16:14 raphtory/nullmodels.py
--rw-r--r--  4.6 unx     7552 b- defN 23-May-26 16:14 raphtory/vis.py
--rw-r--r--  4.6 unx      537 b- defN 23-May-26 16:14 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  8371200 b- defN 23-May-26 16:14 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      532 b- defN 23-May-26 16:14 raphtory-0.3.2.dist-info/RECORD
-7 files, 8391704 bytes uncompressed, 2927297 bytes compressed:  65.1%
+Zip file size: 6275234 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     9622 b- defN 23-Jun-07 19:27 raphtory-0.4.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      134 b- defN 23-Jun-07 19:27 raphtory-0.4.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      522 b- defN 23-Jun-07 19:27 raphtory/__init__.py
+-rw-r--r--  4.6 unx     7399 b- defN 23-Jun-07 19:27 raphtory/vis.py
+-rw-r--r--  4.6 unx     1994 b- defN 23-Jun-07 19:27 raphtory/nullmodels.py
+-rwxr-xr-x  4.6 unx 19520856 b- defN 23-Jun-07 19:27 raphtory/raphtory.pypy39-pp73-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      547 b- defN 23-Jun-07 19:27 raphtory-0.4.0.dist-info/RECORD
+7 files, 19541074 bytes uncompressed, 6274280 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.3.2.dist-info/METADATA
+Filename: raphtory-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.3.2.dist-info/WHEEL
+Filename: raphtory-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: raphtory/nullmodels.py
+Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/vis.py
 Comment: 
 
-Filename: raphtory/__init__.py
+Filename: raphtory/nullmodels.py
 Comment: 
 
-Filename: raphtory/raphtory.cp39-win_amd64.pyd
+Filename: raphtory/raphtory.pypy39-pp73-x86_64-linux-gnu.so
 Comment: 
 
-Filename: raphtory-0.3.2.dist-info/RECORD
+Filename: raphtory-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## raphtory/nullmodels.py

 * *Ordering differences only*

```diff
@@ -1,59 +1,59 @@
-"""
-Generate null models for a graph.
-"""
-
-import pandas as pd
-
-def shuffle_column(graph_df:pd.DataFrame, col_number=None, col_name=None, inplace=False):
-    """
-    returns a dataframe with a given column shuffled
-    """
-    assert col_number is not None or col_name is not None, f"No column number or name provided."
-    assert not (col_name is not None and col_number is not None), f"Cannot have both a column number and a column name."
-
-    if inplace:
-        df = graph_df
-    else:
-        df = graph_df.copy()
-
-    no_events = len(df)
-
-    if col_number is not None:
-        col = df[[col_number]].sample(n=no_events)
-        col.reset_index(inplace=True,drop=True)
-        df[[col_number]] = col
-    if col_name is not None:
-        col = df[col_name].sample(n=no_events)
-        col.reset_index(inplace=True,drop=True)
-    
-    return df
-
-def shuffle_multiple_columns(graph_df:pd.DataFrame, col_numbers:list=None, col_names:list=None, inplace=False):
-    """
-    returns a dataframe with a given columns shuffled.
-    """
-    assert col_numbers is not None or col_names is not None, f"No column numbers or names provided."
-    assert not (col_names is not None and col_numbers is not None), f"Cannot have both column numbers and column names."
-
-    if col_numbers is not None:
-        for n in col_numbers:
-            df = shuffle_column(graph_df, col_number=n, inplace=inplace)
-    if col_names is not None:
-        for name in col_names:
-            df = shuffle_column(graph_df, col_name=name)
-    
-    return df
-    
-def permuted_timestamps_model(graph_df:pd.DataFrame, time_col:int=None, time_name:str=None, inplace=False, sorted=False):
-    """
-    returns a dataframe with the time column shuffled
-    """
-    shuffled_df = shuffle_column(graph_df, time_col, time_name, inplace)
-
-    if sorted:
-        shuffled_df.sort_values(by=time_name if time_name else shuffled_df.columns[time_col], inplace=True)
-    
-    if inplace:
-        return
-    else:
+"""
+Generate null models for a graph.
+"""
+
+import pandas as pd
+
+def shuffle_column(graph_df:pd.DataFrame, col_number=None, col_name=None, inplace=False):
+    """
+    returns a dataframe with a given column shuffled
+    """
+    assert col_number is not None or col_name is not None, f"No column number or name provided."
+    assert not (col_name is not None and col_number is not None), f"Cannot have both a column number and a column name."
+
+    if inplace:
+        df = graph_df
+    else:
+        df = graph_df.copy()
+
+    no_events = len(df)
+
+    if col_number is not None:
+        col = df[[col_number]].sample(n=no_events)
+        col.reset_index(inplace=True,drop=True)
+        df[[col_number]] = col
+    if col_name is not None:
+        col = df[col_name].sample(n=no_events)
+        col.reset_index(inplace=True,drop=True)
+    
+    return df
+
+def shuffle_multiple_columns(graph_df:pd.DataFrame, col_numbers:list=None, col_names:list=None, inplace=False):
+    """
+    returns a dataframe with a given columns shuffled.
+    """
+    assert col_numbers is not None or col_names is not None, f"No column numbers or names provided."
+    assert not (col_names is not None and col_numbers is not None), f"Cannot have both column numbers and column names."
+
+    if col_numbers is not None:
+        for n in col_numbers:
+            df = shuffle_column(graph_df, col_number=n, inplace=inplace)
+    if col_names is not None:
+        for name in col_names:
+            df = shuffle_column(graph_df, col_name=name)
+    
+    return df
+    
+def permuted_timestamps_model(graph_df:pd.DataFrame, time_col:int=None, time_name:str=None, inplace=False, sorted=False):
+    """
+    returns a dataframe with the time column shuffled
+    """
+    shuffled_df = shuffle_column(graph_df, time_col, time_name, inplace)
+
+    if sorted:
+        shuffled_df.sort_values(by=time_name if time_name else shuffled_df.columns[time_col], inplace=True)
+    
+    if inplace:
+        return
+    else:
         return shuffled_df
```

## raphtory/vis.py

 * *Ordering differences only*

```diff
@@ -1,153 +1,153 @@
-"""
-Generate a visualisation using matplotlib or pyvis from Raphtory graphs.
-"""
-from pyvis.network import Network
-import networkx as nx
-
-r"""Draw a graph with Pyvis.
-
-.. note::
-
-    Pyvis is a required dependency.
-    If you intend to use this function make sure that
-    you install Pyvis with ``pip install pyvis``
-
-:param graph: A Raphtory graph.
-:param str height: A string defining the height of the graph. By default ``800px`` is set.
-:param str width: A string defining the width of the graph.  By default ``800px`` is set.
-:param str bg_color: A string defining the colour of the graph background. It must be a HTML color code. By default ``#white`` (white) is set.
-:param str font_color: A string defining the colour of the graph font. By default ``"black"`` is set.
-:param str edge_color: A string defining the colour of the edges in the graph. By default ``#000000`` (black) is set.
-:param str shape: An optional string defining what the node looks like. 
-    There are two types of nodes. One type has the label inside of it and the other type has the label underneath it. 
-    The types with the label inside of it are: ellipse, circle, database, box, text. 
-    The ones with the label outside of it are: image, circularImage, diamond, dot, star, triangle, triangleDown, square and icon.
-    By default ``"dot"`` is set.
-:param str node_image: An optional string defining the url of a custom node image. By default an image of a circle is set.
-:param str edge_weight: An optional string defining the name of the property where edge weight is set on your Raphtory graph. By default ``1`` is set.
-:param str edge_label: An optional string defining the name of the property where edge label is set on your Raphtory graph. By default, an empty string as the label is set.
-:param bool notebook: A boolean that is set to True if using jupyter notebook. By default this is set to True.
-
-
-:returns: A pyvis visualisation in static HTML format that is interactive with toggles menu.
-:rtype: IFrame(name, width=self.width, height=self.height)
-
-For Example:
-
-.. jupyter-execute::
-
-    from raphtory import Graph
-    from raphtory import vis
-
-    g = Graph()
-    g.add_vertex(1, src, properties={"image": "image.png"})
-    g.add_edge(1, 1, 2, {"title": "edge", "weight": 1})
-    g.add_edge(1, 2, 1, {"title": "edge", "weight": 3})
-
-    vis.to_pyvis(graph=g, edge_color="#FF0000", edge_weight= "weight", shape="image", node_image="image", edge_label="title")
-
-"""
-
-def to_pyvis(
-            graph,
-            height="800px",
-            width="800px",
-            bg_color="#white",
-            font_color="black",
-            edge_color="#000000",
-            shape=None,
-            node_image=None,
-            edge_weight=None,
-            edge_label=None,
-            notebook=True,
-        ):
-    """
-    Returns a dynamic visualisation in static HTML format from a Raphtory graph.
-    """
-    visGraph = Network(height=height, width=width, bgcolor=bg_color, font_color=font_color, notebook=notebook)
-   
-    for v in graph.vertices():
-        image = v.property(node_image) if node_image != None else "https://cdn-icons-png.flaticon.com/512/7584/7584620.png"
-        shape = shape if shape != None else "dot"
-        visGraph.add_node(v.id(), label= v.name(), shape=shape, image=image)
-
-    for e in graph.edges():
-        weight = e.property(edge_weight) if edge_weight != None else 1
-        label = e.property(edge_label) if edge_label != None else ""
-        visGraph.add_edge(e.src().id(), e.dst().id(), value=weight, color=edge_color, title=label)
-       
-    visGraph.show_buttons(filter_=['physics'])
-    visGraph.show('nx.html')
-    return visGraph
-    
-r"""Draw a graph with NetworkX.
-
-.. note::
-
-    Network X is a required dependency.
-    If you intend to use this function make sure that
-    you install Network X with ``pip install networkx``
-
-:param graph: A Raphtory graph.
-:param float k: A float defining optimal distance between nodes. If None the distance is set to 1/sqrt(n) where n is the number of nodes. Increase this value to move nodes farther apart.
-:param int iterations: An integer defining the maximum number of iterations taken to generate the optimum spring layout. Increasing this number will increase the computational time to generate the layout.  By default ``50`` is set.
-:param scalar or array node_size: A scalar defining the size of nodes. By default ``300`` is set.
-:param color or array of colors node_color: Node color. Can be a single color or a sequence of colors with the same length as nodelist. Color can be string or rgb (or rgba) tuple of floats from 0-1. If numeric values are specified they will be mapped to colors using the cmap and vmin,vmax parameters. See matplotlib.scatter for more details. By default ``"#1f78b4"`` (blue) is set.
-:param color or array of colors edge_color: Edge color. Can be a single color or a sequence of colors with the same length as edgelist. Color can be string or rgb (or rgba) tuple of floats from 0-1. If numeric values are specified they will be mapped to colors using the edge_cmap and edge_vmin,edge_vmax parameters. By default ``'k'`` (black) is set.
-:param bool arrows: If None, directed graphs draw arrowheads with FancyArrowPatch, while undirected graphs draw edges via LineCollection for speed. If True, draw arrowheads with FancyArrowPatches (bendable and stylish). If False, draw edges using LineCollection (linear and fast).
-    Note: Arrowheads will be the same color as edges. Default is None.
-:param str arrow_style: Style of the edges, defaults to ``‘-|>’``.
-
-:returns: A networkx visualisation that appears in the notebook output.
-:rtype:  matplotlib.collections.PathCollection and matplotlib.collections.LineCollection or a list of matplotlib.patches.FancyArrowPatch.
-        `PathCollection` of the nodes.  
-        If ``arrows=True``, a list of FancyArrowPatches is returned.
-        If ``arrows=False``, a LineCollection is returned.
-        If ``arrows=None`` (the default), then a LineCollection is returned if
-        `G` is undirected, otherwise returns a list of FancyArrowPatches.
-
-For Example:
-
-.. jupyter-execute::
-
-    from raphtory import Graph
-    from raphtory import vis
-
-    g = Graph()
-    g.add_vertex(1, src, properties={"image": "image.png"})
-    g.add_edge(1, 1, 2, {"title": "edge", "weight": 1})
-    g.add_edge(1, 2, 1, {"title": "edge", "weight": 3})
-
-    vis.to_networkx(graph=g, k=0.15, iterations=100, node_size=500, node_color='red', edge_color='blue', arrows=True)
-
-"""
-def to_networkx(
-                graph,
-                k=None,
-                iterations=50,
-                node_size=300,
-                node_color='#1f78b4',
-                edge_color='k',
-                arrows=None,
-                arrow_style= "-|>"
-                ):
-    """
-    Returns a Network X graph visualiation from a Raphtory graph.
-    """
-    
-    networkXGraph = nx.MultiDiGraph()
-
-    networkXGraph.add_nodes_from(list(graph.vertices().id()))
-
-    edges = []
-    for e in graph.edges():
-        edges.append((e.src().id(), e.dst().id()))
-    
-    networkXGraph.add_edges_from(edges)
-    pos = nx.spring_layout(networkXGraph, k=k, iterations=iterations)
-
-    nx.draw_networkx_nodes(networkXGraph, pos, node_size=node_size, node_color=node_color)
-    nx.draw_networkx_edges(networkXGraph, pos, edge_color=edge_color, arrows=arrows, arrowstyle=arrow_style)
-
-
-
+"""
+Generate a visualisation using matplotlib or pyvis from Raphtory graphs.
+"""
+from pyvis.network import Network
+import networkx as nx
+
+r"""Draw a graph with Pyvis.
+
+.. note::
+
+    Pyvis is a required dependency.
+    If you intend to use this function make sure that
+    you install Pyvis with ``pip install pyvis``
+
+:param graph: A Raphtory graph.
+:param str height: A string defining the height of the graph. By default ``800px`` is set.
+:param str width: A string defining the width of the graph.  By default ``800px`` is set.
+:param str bg_color: A string defining the colour of the graph background. It must be a HTML color code. By default ``#white`` (white) is set.
+:param str font_color: A string defining the colour of the graph font. By default ``"black"`` is set.
+:param str edge_color: A string defining the colour of the edges in the graph. By default ``#000000`` (black) is set.
+:param str shape: An optional string defining what the node looks like. 
+    There are two types of nodes. One type has the label inside of it and the other type has the label underneath it. 
+    The types with the label inside of it are: ellipse, circle, database, box, text. 
+    The ones with the label outside of it are: image, circularImage, diamond, dot, star, triangle, triangleDown, square and icon.
+    By default ``"dot"`` is set.
+:param str node_image: An optional string defining the url of a custom node image. By default an image of a circle is set.
+:param str edge_weight: An optional string defining the name of the property where edge weight is set on your Raphtory graph. By default ``1`` is set.
+:param str edge_label: An optional string defining the name of the property where edge label is set on your Raphtory graph. By default, an empty string as the label is set.
+:param bool notebook: A boolean that is set to True if using jupyter notebook. By default this is set to True.
+
+
+:returns: A pyvis visualisation in static HTML format that is interactive with toggles menu.
+:rtype: IFrame(name, width=self.width, height=self.height)
+
+For Example:
+
+.. jupyter-execute::
+
+    from raphtory import Graph
+    from raphtory import vis
+
+    g = Graph()
+    g.add_vertex(1, src, properties={"image": "image.png"})
+    g.add_edge(1, 1, 2, {"title": "edge", "weight": 1})
+    g.add_edge(1, 2, 1, {"title": "edge", "weight": 3})
+
+    vis.to_pyvis(graph=g, edge_color="#FF0000", edge_weight= "weight", shape="image", node_image="image", edge_label="title")
+
+"""
+
+def to_pyvis(
+            graph,
+            height="800px",
+            width="800px",
+            bg_color="#white",
+            font_color="black",
+            edge_color="#000000",
+            shape=None,
+            node_image=None,
+            edge_weight=None,
+            edge_label=None,
+            notebook=True,
+        ):
+    """
+    Returns a dynamic visualisation in static HTML format from a Raphtory graph.
+    """
+    visGraph = Network(height=height, width=width, bgcolor=bg_color, font_color=font_color, notebook=notebook)
+   
+    for v in graph.vertices():
+        image = v.property(node_image) if node_image != None else "https://cdn-icons-png.flaticon.com/512/7584/7584620.png"
+        shape = shape if shape != None else "dot"
+        visGraph.add_node(v.id(), label= v.name(), shape=shape, image=image)
+
+    for e in graph.edges():
+        weight = e.property(edge_weight) if edge_weight != None else 1
+        label = e.property(edge_label) if edge_label != None else ""
+        visGraph.add_edge(e.src().id(), e.dst().id(), value=weight, color=edge_color, title=label)
+       
+    visGraph.show_buttons(filter_=['physics'])
+    visGraph.show('nx.html')
+    return visGraph
+    
+r"""Draw a graph with NetworkX.
+
+.. note::
+
+    Network X is a required dependency.
+    If you intend to use this function make sure that
+    you install Network X with ``pip install networkx``
+
+:param graph: A Raphtory graph.
+:param float k: A float defining optimal distance between nodes. If None the distance is set to 1/sqrt(n) where n is the number of nodes. Increase this value to move nodes farther apart.
+:param int iterations: An integer defining the maximum number of iterations taken to generate the optimum spring layout. Increasing this number will increase the computational time to generate the layout.  By default ``50`` is set.
+:param scalar or array node_size: A scalar defining the size of nodes. By default ``300`` is set.
+:param color or array of colors node_color: Node color. Can be a single color or a sequence of colors with the same length as nodelist. Color can be string or rgb (or rgba) tuple of floats from 0-1. If numeric values are specified they will be mapped to colors using the cmap and vmin,vmax parameters. See matplotlib.scatter for more details. By default ``"#1f78b4"`` (blue) is set.
+:param color or array of colors edge_color: Edge color. Can be a single color or a sequence of colors with the same length as edgelist. Color can be string or rgb (or rgba) tuple of floats from 0-1. If numeric values are specified they will be mapped to colors using the edge_cmap and edge_vmin,edge_vmax parameters. By default ``'k'`` (black) is set.
+:param bool arrows: If None, directed graphs draw arrowheads with FancyArrowPatch, while undirected graphs draw edges via LineCollection for speed. If True, draw arrowheads with FancyArrowPatches (bendable and stylish). If False, draw edges using LineCollection (linear and fast).
+    Note: Arrowheads will be the same color as edges. Default is None.
+:param str arrow_style: Style of the edges, defaults to ``‘-|>’``.
+
+:returns: A networkx visualisation that appears in the notebook output.
+:rtype:  matplotlib.collections.PathCollection and matplotlib.collections.LineCollection or a list of matplotlib.patches.FancyArrowPatch.
+        `PathCollection` of the nodes.  
+        If ``arrows=True``, a list of FancyArrowPatches is returned.
+        If ``arrows=False``, a LineCollection is returned.
+        If ``arrows=None`` (the default), then a LineCollection is returned if
+        `G` is undirected, otherwise returns a list of FancyArrowPatches.
+
+For Example:
+
+.. jupyter-execute::
+
+    from raphtory import Graph
+    from raphtory import vis
+
+    g = Graph()
+    g.add_vertex(1, src, properties={"image": "image.png"})
+    g.add_edge(1, 1, 2, {"title": "edge", "weight": 1})
+    g.add_edge(1, 2, 1, {"title": "edge", "weight": 3})
+
+    vis.to_networkx(graph=g, k=0.15, iterations=100, node_size=500, node_color='red', edge_color='blue', arrows=True)
+
+"""
+def to_networkx(
+                graph,
+                k=None,
+                iterations=50,
+                node_size=300,
+                node_color='#1f78b4',
+                edge_color='k',
+                arrows=None,
+                arrow_style= "-|>"
+                ):
+    """
+    Returns a Network X graph visualiation from a Raphtory graph.
+    """
+    
+    networkXGraph = nx.MultiDiGraph()
+
+    networkXGraph.add_nodes_from(list(graph.vertices().id()))
+
+    edges = []
+    for e in graph.edges():
+        edges.append((e.src().id(), e.dst().id()))
+    
+    networkXGraph.add_edges_from(edges)
+    pos = nx.spring_layout(networkXGraph, k=k, iterations=iterations)
+
+    nx.draw_networkx_nodes(networkXGraph, pos, node_size=node_size, node_color=node_color)
+    nx.draw_networkx_edges(networkXGraph, pos, edge_color=edge_color, arrows=arrows, arrowstyle=arrow_style)
+
+
+
```

## raphtory/__init__.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-import sys
-from .raphtory import *
-sys.modules["raphtory.algorithms"] = algorithms
-sys.modules["raphtory.graph_gen"] = graph_gen
-sys.modules["raphtory.graph_loader"] = graph_loader
-
-
-from .nullmodels import *
-
-__doc__ = raphtory.__doc__
-if hasattr(raphtory, "__all__"):
-    __all__ = raphtory.__all__
-
-algorithms.__doc__ = "Algorithmic functions that can be run on Raphtory graphs"
-graph_gen.__doc__ = "Generate Raphtory graphs from attachment models"
+import sys
+from .raphtory import *
+sys.modules["raphtory.algorithms"] = algorithms
+sys.modules["raphtory.graph_gen"] = graph_gen
+sys.modules["raphtory.graph_loader"] = graph_loader
+
+
+from .nullmodels import *
+
+__doc__ = raphtory.__doc__
+if hasattr(raphtory, "__all__"):
+    __all__ = raphtory.__all__
+
+algorithms.__doc__ = "Algorithmic functions that can be run on Raphtory graphs"
+graph_gen.__doc__ = "Generate Raphtory graphs from attachment models"
 graph_loader.__doc__ = "Load and save Raphtory graphs from/to file(s)"
```

## Comparing `raphtory-0.3.2.dist-info/METADATA` & `raphtory-0.4.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.3.2
+Version: 0.4.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3
+Requires-Dist: pyvis >=0.3.2
+Requires-Dist: networkx >=2.6.3
 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
 Requires-Dist: networkx >=2.6.3 ; extra == 'vis'
 Requires-Dist: matplotlib >=3.4.3 ; extra == 'vis'
 Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
 Provides-Extra: vis
 Summary: Python package for raphtory, a temporal graph library
 Keywords: graph,temporal-graph,temporal
@@ -20,184 +22,184 @@
 Project-URL: homepage, https://github.com/pometry/raphtory
 Project-URL: documentation, https://docs.raphtory.com/
 Project-URL: repository, https://github.com/pometry/raphtory
 Project-URL: twitter, https://twitter.com/raphtory/
 Project-URL: slack, https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA
 Project-URL: youtube, https://www.youtube.com/@pometry8546/videos
 
-<br>
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/6665739/130641943-fa7fcdb8-a0e7-4aa4-863f-3df61b5de775.png" alt="Raphtory" height="100"/>
-</p>
-<p align="center">
-</p>
-
-<p align="center">
-<a href="https://github.com/Raphtory/Raphtory/actions/workflows/test.yml/badge.svg">
-<img alt="Test and Build" src="https://github.com/Raphtory/Raphtory/actions/workflows/test.yml/badge.svg" />
-</a>
-<a href="https://github.com/Raphtory/Raphtory/releases">
-<img alt="Latest Release" src="https://img.shields.io/github/v/release/Raphtory/Raphtory?color=brightgreen&include_prereleases" />
-</a>
-<a href="https://github.com/Raphtory/Raphtory/issues">
-<img alt="Issues" src="https://img.shields.io/github/issues/Raphtory/Raphtory?color=brightgreen" />
-</a>
-<a href="https://crates.io/crates/raphtory">
-<img alt="Crates.io" src="https://img.shields.io/crates/v/raphtory">
-</a>
-<a href="https://pypi.org/project/raphtory/">
-<img alt="PyPI" src="https://img.shields.io/pypi/v/raphtory">
-</a>
-
-<a href="https://mybinder.org/v2/gh/Raphtory/Raphtory/master?labpath=examples%2Fpy%2Flotr%2Flotr.ipynb">
-<img alt="Launch Notebook" src="https://mybinder.org/badge_logo.svg" />
-</a>
-</p>
-<p align="center">
-<a href="https://www.raphtory.com">🌍 Website </a>
-&nbsp
-<a href="https://docs.raphtory.com/">📒 Documentation</a>
-&nbsp 
-<a href="https://www.pometry.com"><img src="https://user-images.githubusercontent.com/6665739/202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png" height="20" align="center"/> Pometry</a> 
-&nbsp
-<a href="https://docs.raphtory.com/en/master/Introduction/ingestion.html">🧙🏻‍ Tutorial</a> 
-&nbsp
-<a href="https://github.com/Raphtory/Raphtory/issues">🐛 Report a Bug</a> 
-&nbsp
-<a href="https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA"><img src="https://user-images.githubusercontent.com/6665739/154071628-a55fb5f9-6994-4dcf-be03-401afc7d9ee0.png" height="20" align="center"/> Join Slack</a> 
-</p>
-
-<br>
-
-Raphtory is an in-memory graph tool written in Rust with friendly Python APIs on top. It is blazingly fast, scales to hundreds of millions of edges 
-on your laptop, and can be dropped into your existing pipelines with a simple `pip install raphtory`.  
-
-It supports time traveling, multilayer modelling, and advanced analytics beyond simple querying like community evolution, dynamic scoring, and mining temporal motifs.
-
-If you wish to contribute, check out the open [list of issues](https://github.com/Pometry/Raphtory/issues), [bounty board](https://github.com/Raphtory/Raphtory/discussions/categories/bounty-board) or hit us up directly on [slack](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA). Successful contributions will be reward with swizzling swag!
-
-
-## Running a basic example
-
-```python
-from raphtory import Graph
-import pandas as pd
-
-# Create a new graph
-graph = Graph()
-
-# Add some data to your graph
-graph.add_vertex(timestamp=1, id="Alice")
-graph.add_vertex(timestamp=1, id="Bob")
-graph.add_vertex(timestamp=1, id="Charlie")
-graph.add_edge  (timestamp=2, src="Bob",   dst="Charlie", properties={"weight":5.0})
-graph.add_edge  (timestamp=3, src="Alice", dst="Bob",     properties={"weight":10.0})
-graph.add_edge  (timestamp=3, src="Bob",   dst="Charlie", properties={"weight":-15.0})
-
-# Check the number of unique nodes/edges in the graph and earliest/latest time seen.
-print(graph)
-
-results = [["earliest_time", "name", "out_degree", "in_degree"]]
-
-# Collect some simple vertex metrics Ran across the history of your graph with a rolling window
-for graph_view in graph.rolling(window=1):
-    for v in graph_view.vertices():
-        results.append([graph_view.earliest_time(), v.name(), v.out_degree(), v.in_degree()])
-
-# Print the results
-print(pd.DataFrame(results[1:], columns=results[0]))
-
-# Grab an edge, explore the history of its 'weight' 
-cb_edge = graph.edge("Bob","Charlie")
-weight_history = cb_edge.property_history("weight")
-print("The edge between Bob and Charlie has the following weight history:", weight_history)
-
-# Compare this weight between time 2 and time 3
-weight_change = cb_edge.at(2)["weight"] - cb_edge.at(3)["weight"]
-print("The weight of the edge between Bob and Charlie has changed by",weight_change,"pts")
-```
-
-```a
-Graph(number_of_edges=2, number_of_vertices=3, earliest_time=1, latest_time=3)
-
-|   | earliest_time | name    | out_degree | in_degree |
-|---|---------------|---------|------------|-----------|
-| 0 | 1             | Alice   | 0          | 0         |
-| 1 | 1             | Bob     | 0          | 0         |
-| 2 | 1             | Charlie | 0          | 0         |
-| 3 | 2             | Bob     | 1          | 0         |
-| 4 | 2             | Charlie | 0          | 1         |
-| 5 | 3             | Alice   | 1          | 0         |
-| 6 | 3             | Bob     | 1          | 1         |
-| 7 | 3             | Charlie | 0          | 1         |
-
-The edge between Bob and Charlie has the following weight history: [(2, 5.0), (3, -15.0)]
-
-The weight of the edge between Bob and Charlie has changed by 20.0 pts
-```
-
-
-## Installing Raphtory 
-
-Raphtory is available for Python and Rust as of version 0.3.0. You should have Python version 3.10 or higher and it's a good idea to use conda, virtualenv, or pyenv. 
-
-```bash
-pip install raphtory
-``` 
-
-## Examples and Notebooks
-
-Check out Raphtory in action with our interactive Jupyter Notebook! Just click the badge below to launch a Raphtory sandbox online, no installation needed.
-
- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Raphtory/Raphtory/master?labpath=examples%2Fpy%2Flotr%2Flotr.ipynb) 
-
-Want to give Raphtory a go on your laptop? You can checkout out the [latest documentation](https://docs.raphtory.com/) and [complete list of available algorithms](https://docs.raphtory.com/en/v0.2.0/api/_autosummary/raphtory.algorithms.html) or hop on our notebook based tutorials below!
-
-
-#### Getting started
-
-| Type     | Description                                                                              |
-|----------|------------------------------------------------------------------------------------------|
-| Tutorial | [Building your first graph](https://docs.raphtory.com/en/master/Introduction/ingestion.html) |
-
-#### Developing an end-to-end application
-
-| Type | Description                                                                                                                                                   |
-| ------------- |---------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Notebook | [Use our powerful time APIs to find pump and dump scams in popular NFTs](https://github.com/Raphtory/Raphtory/blob/master/examples/py/nft/nft_analysis.ipynb) |
-
-
-# Benchmarks
-
-We host a page which triggers and saves the result of two benchmarks upon every push to the master branch. 
-
-View this here [https://pometry.github.io/Raphtory/dev/bench/](https://pometry.github.io/Raphtory/dev/bench/)
-
-# Bounty board
-
-Raphtory is currently offering rewards for contributions, such as new features or algorithms. Contributors will receive swag and prizes! 
-
-To get started, check out our list of desired algorithms at https://github.com/Raphtory/Raphtory/discussions/categories/bounty-board which include some low hanging fruit (🍇) that are easy to implement. 
-
-
-# Community  
-
-Join the growing community of open-source enthusiasts using Raphtory to power their graph analysis projects!
-
-- Follow [![Slack](https://img.shields.io/twitter/follow/raphtory?label=@raphtory)](https://twitter.com/raphtory) for the latest Raphtory news and development
-
-- Join our [![Slack](https://img.shields.io/badge/community-Slack-red)](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) to chat with us and get answers to your questions!
-
-
-## Contributors
-
-<a href="https://github.com/raphtory/raphtory/graphs/contributors"><img src="https://contrib.rocks/image?repo=raphtory/raphtory"/></a>
-
-Want to get involved? Please join the Raphtory [Slack](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) group and speak with us on how you could pitch in!
-
-## License  
-
-Raphtory is licensed under the terms of the GNU General Public License v3.0 (check out our LICENSE file).
-
-
-
+<br>
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/6665739/130641943-fa7fcdb8-a0e7-4aa4-863f-3df61b5de775.png" alt="Raphtory" height="100"/>
+</p>
+<p align="center">
+</p>
+
+<p align="center">
+<a href="https://github.com/Raphtory/Raphtory/actions/workflows/test.yml/badge.svg">
+<img alt="Test and Build" src="https://github.com/Raphtory/Raphtory/actions/workflows/test.yml/badge.svg" />
+</a>
+<a href="https://github.com/Raphtory/Raphtory/releases">
+<img alt="Latest Release" src="https://img.shields.io/github/v/release/Raphtory/Raphtory?color=brightgreen&include_prereleases" />
+</a>
+<a href="https://github.com/Raphtory/Raphtory/issues">
+<img alt="Issues" src="https://img.shields.io/github/issues/Raphtory/Raphtory?color=brightgreen" />
+</a>
+<a href="https://crates.io/crates/raphtory">
+<img alt="Crates.io" src="https://img.shields.io/crates/v/raphtory">
+</a>
+<a href="https://pypi.org/project/raphtory/">
+<img alt="PyPI" src="https://img.shields.io/pypi/v/raphtory">
+</a>
+
+<a href="https://mybinder.org/v2/gh/Raphtory/Raphtory/master?labpath=examples%2Fpy%2Flotr%2Flotr.ipynb">
+<img alt="Launch Notebook" src="https://mybinder.org/badge_logo.svg" />
+</a>
+</p>
+<p align="center">
+<a href="https://www.raphtory.com">🌍 Website </a>
+&nbsp
+<a href="https://docs.raphtory.com/">📒 Documentation</a>
+&nbsp 
+<a href="https://www.pometry.com"><img src="https://user-images.githubusercontent.com/6665739/202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png" height="20" align="center"/> Pometry</a> 
+&nbsp
+<a href="https://docs.raphtory.com/en/master/Introduction/ingestion.html">🧙🏻‍ Tutorial</a> 
+&nbsp
+<a href="https://github.com/Raphtory/Raphtory/issues">🐛 Report a Bug</a> 
+&nbsp
+<a href="https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA"><img src="https://user-images.githubusercontent.com/6665739/154071628-a55fb5f9-6994-4dcf-be03-401afc7d9ee0.png" height="20" align="center"/> Join Slack</a> 
+</p>
+
+<br>
+
+Raphtory is an in-memory graph tool written in Rust with friendly Python APIs on top. It is blazingly fast, scales to hundreds of millions of edges 
+on your laptop, and can be dropped into your existing pipelines with a simple `pip install raphtory`.  
+
+It supports time traveling, multilayer modelling, and advanced analytics beyond simple querying like community evolution, dynamic scoring, and mining temporal motifs.
+
+If you wish to contribute, check out the open [list of issues](https://github.com/Pometry/Raphtory/issues), [bounty board](https://github.com/Raphtory/Raphtory/discussions/categories/bounty-board) or hit us up directly on [slack](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA). Successful contributions will be reward with swizzling swag!
+
+
+## Running a basic example
+
+```python
+from raphtory import Graph
+import pandas as pd
+
+# Create a new graph
+graph = Graph()
+
+# Add some data to your graph
+graph.add_vertex(timestamp=1, id="Alice")
+graph.add_vertex(timestamp=1, id="Bob")
+graph.add_vertex(timestamp=1, id="Charlie")
+graph.add_edge  (timestamp=2, src="Bob",   dst="Charlie", properties={"weight":5.0})
+graph.add_edge  (timestamp=3, src="Alice", dst="Bob",     properties={"weight":10.0})
+graph.add_edge  (timestamp=3, src="Bob",   dst="Charlie", properties={"weight":-15.0})
+
+# Check the number of unique nodes/edges in the graph and earliest/latest time seen.
+print(graph)
+
+results = [["earliest_time", "name", "out_degree", "in_degree"]]
+
+# Collect some simple vertex metrics Ran across the history of your graph with a rolling window
+for graph_view in graph.rolling(window=1):
+    for v in graph_view.vertices():
+        results.append([graph_view.earliest_time(), v.name(), v.out_degree(), v.in_degree()])
+
+# Print the results
+print(pd.DataFrame(results[1:], columns=results[0]))
+
+# Grab an edge, explore the history of its 'weight' 
+cb_edge = graph.edge("Bob","Charlie")
+weight_history = cb_edge.property_history("weight")
+print("The edge between Bob and Charlie has the following weight history:", weight_history)
+
+# Compare this weight between time 2 and time 3
+weight_change = cb_edge.at(2)["weight"] - cb_edge.at(3)["weight"]
+print("The weight of the edge between Bob and Charlie has changed by",weight_change,"pts")
+```
+
+```a
+Graph(number_of_edges=2, number_of_vertices=3, earliest_time=1, latest_time=3)
+
+|   | earliest_time | name    | out_degree | in_degree |
+|---|---------------|---------|------------|-----------|
+| 0 | 1             | Alice   | 0          | 0         |
+| 1 | 1             | Bob     | 0          | 0         |
+| 2 | 1             | Charlie | 0          | 0         |
+| 3 | 2             | Bob     | 1          | 0         |
+| 4 | 2             | Charlie | 0          | 1         |
+| 5 | 3             | Alice   | 1          | 0         |
+| 6 | 3             | Bob     | 1          | 1         |
+| 7 | 3             | Charlie | 0          | 1         |
+
+The edge between Bob and Charlie has the following weight history: [(2, 5.0), (3, -15.0)]
+
+The weight of the edge between Bob and Charlie has changed by 20.0 pts
+```
+
+
+## Installing Raphtory 
+
+Raphtory is available for Python and Rust as of version 0.3.0. You should have Python version 3.10 or higher and it's a good idea to use conda, virtualenv, or pyenv. 
+
+```bash
+pip install raphtory
+``` 
+
+## Examples and Notebooks
+
+Check out Raphtory in action with our interactive Jupyter Notebook! Just click the badge below to launch a Raphtory sandbox online, no installation needed.
+
+ [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Raphtory/Raphtory/master?labpath=examples%2Fpy%2Flotr%2Flotr.ipynb) 
+
+Want to give Raphtory a go on your laptop? You can checkout out the [latest documentation](https://docs.raphtory.com/) and [complete list of available algorithms](https://docs.raphtory.com/en/v0.2.0/api/_autosummary/raphtory.algorithms.html) or hop on our notebook based tutorials below!
+
+
+#### Getting started
+
+| Type     | Description                                                                              |
+|----------|------------------------------------------------------------------------------------------|
+| Tutorial | [Building your first graph](https://docs.raphtory.com/en/master/Introduction/ingestion.html) |
+
+#### Developing an end-to-end application
+
+| Type | Description                                                                                                                                                   |
+| ------------- |---------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Notebook | [Use our powerful time APIs to find pump and dump scams in popular NFTs](https://github.com/Raphtory/Raphtory/blob/master/examples/py/nft/nft_analysis.ipynb) |
+
+
+# Benchmarks
+
+We host a page which triggers and saves the result of two benchmarks upon every push to the master branch. 
+
+View this here [https://pometry.github.io/Raphtory/dev/bench/](https://pometry.github.io/Raphtory/dev/bench/)
+
+# Bounty board
+
+Raphtory is currently offering rewards for contributions, such as new features or algorithms. Contributors will receive swag and prizes! 
+
+To get started, check out our list of desired algorithms at https://github.com/Raphtory/Raphtory/discussions/categories/bounty-board which include some low hanging fruit (🍇) that are easy to implement. 
+
+
+# Community  
+
+Join the growing community of open-source enthusiasts using Raphtory to power their graph analysis projects!
+
+- Follow [![Slack](https://img.shields.io/twitter/follow/raphtory?label=@raphtory)](https://twitter.com/raphtory) for the latest Raphtory news and development
+
+- Join our [![Slack](https://img.shields.io/badge/community-Slack-red)](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) to chat with us and get answers to your questions!
+
+
+## Contributors
+
+<a href="https://github.com/raphtory/raphtory/graphs/contributors"><img src="https://contrib.rocks/image?repo=raphtory/raphtory"/></a>
+
+Want to get involved? Please join the Raphtory [Slack](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) group and speak with us on how you could pitch in!
+
+## License  
+
+Raphtory is licensed under the terms of the GNU General Public License v3.0 (check out our LICENSE file).
+
+
+
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.3.2 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.4.0 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: pandas >=1.3.3 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
-Requires-Dist: networkx >=2.6.3 ; extra == 'vis' Requires-Dist: matplotlib
->=3.4.3 ; extra == 'vis' Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
-Provides-Extra: vis Summary: Python package for raphtory, a temporal graph
-library Keywords: graph,temporal-graph,temporal Home-Page: https://github.com/
-Raphtory/raphtory/ Author: Pometry License: GPL-3.0 Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-
-URL: homepage, https://github.com/pometry/raphtory Project-URL: documentation,
-https://docs.raphtory.com/ Project-URL: repository, https://github.com/pometry/
-raphtory Project-URL: twitter, https://twitter.com/raphtory/ Project-URL:
-slack, https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-
-VgPIFRleJFJBwmpf81tvxA Project-URL: youtube, https://www.youtube.com/
-@pometry8546/videos
+Requires-Dist: pandas >=1.3.3 Requires-Dist: pyvis >=0.3.2 Requires-Dist:
+networkx >=2.6.3 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis' Requires-Dist:
+networkx >=2.6.3 ; extra == 'vis' Requires-Dist: matplotlib >=3.4.3 ; extra ==
+'vis' Requires-Dist: seaborn >=0.11.2 ; extra == 'vis' Provides-Extra: vis
+Summary: Python package for raphtory, a temporal graph library Keywords:
+graph,temporal-graph,temporal Home-Page: https://github.com/Raphtory/raphtory/
+Author: Pometry License: GPL-3.0 Requires-Python: >=3.7 Description-Content-
+Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
+github.com/pometry/raphtory Project-URL: documentation, https://
+docs.raphtory.com/ Project-URL: repository, https://github.com/pometry/raphtory
+Project-URL: twitter, https://twitter.com/raphtory/ Project-URL: slack, https:/
+/join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA
+Project-URL: youtube, https://www.youtube.com/@pometry8546/videos
                                   [Raphtory]
 [Test_and_Build] [Latest_Release] [Issues] [Crates.io] [PyPI] [Launch_Notebook]
 ð_Website   ð_Documentation   [https://user-images.githubusercontent.com/
      6665739/202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png]_Pometry  
            ð§ð»â_Tutorial   ð_Report_a_Bug   [https://user-
     images.githubusercontent.com/6665739/154071628-a55fb5f9-6994-4dcf-be03-
                          401afc7d9ee0.png]_Join_Slack
```

