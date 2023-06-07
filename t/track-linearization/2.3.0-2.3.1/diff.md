# Comparing `tmp/track_linearization-2.3.0.tar.gz` & `tmp/track_linearization-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track_linearization-2.3.0.tar", last modified: Fri Oct 21 02:52:06 2022, max compression
+gzip compressed data, was "track_linearization-2.3.1.tar", last modified: Wed Jun  7 20:22:12 2023, max compression
```

## Comparing `track_linearization-2.3.0.tar` & `track_linearization-2.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-10-21 02:52:06.115650 track_linearization-2.3.0/
--rw-r--r--   0 edeno      (501) staff       (20)      112 2022-10-21 02:52:06.115249 track_linearization-2.3.0/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)      841 2022-09-26 22:47:03.000000 track_linearization-2.3.0/README.md
--rw-r--r--   0 edeno      (501) staff       (20)       38 2022-10-21 02:52:06.115877 track_linearization-2.3.0/setup.cfg
--rw-r--r--   0 edeno      (501) staff       (20)      495 2022-10-21 02:51:35.000000 track_linearization-2.3.0/setup.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-10-21 02:52:06.112348 track_linearization-2.3.0/track_linearization/
--rw-r--r--   0 edeno      (501) staff       (20)      230 2022-09-26 22:44:15.000000 track_linearization-2.3.0/track_linearization/__init__.py
--rw-r--r--   0 edeno      (501) staff       (20)    18659 2022-10-21 02:44:34.000000 track_linearization-2.3.0/track_linearization/core.py
--rw-r--r--   0 edeno      (501) staff       (20)    11619 2022-09-26 22:44:53.000000 track_linearization-2.3.0/track_linearization/utils.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2022-10-21 02:52:06.114830 track_linearization-2.3.0/track_linearization.egg-info/
--rw-r--r--   0 edeno      (501) staff       (20)      112 2022-10-21 02:52:06.000000 track_linearization-2.3.0/track_linearization.egg-info/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)      321 2022-10-21 02:52:06.000000 track_linearization-2.3.0/track_linearization.egg-info/SOURCES.txt
--rw-r--r--   0 edeno      (501) staff       (20)        1 2022-10-21 02:52:06.000000 track_linearization-2.3.0/track_linearization.egg-info/dependency_links.txt
--rw-r--r--   0 edeno      (501) staff       (20)       57 2022-10-21 02:52:06.000000 track_linearization-2.3.0/track_linearization.egg-info/requires.txt
--rw-r--r--   0 edeno      (501) staff       (20)       20 2022-10-21 02:52:06.000000 track_linearization-2.3.0/track_linearization.egg-info/top_level.txt
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-06-07 20:22:12.913287 track_linearization-2.3.1/
+-rw-r--r--   0 edeno      (501) staff       (20)      112 2023-06-07 20:22:12.913100 track_linearization-2.3.1/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)      841 2022-09-26 22:47:03.000000 track_linearization-2.3.1/README.md
+-rw-r--r--   0 edeno      (501) staff       (20)       38 2023-06-07 20:22:12.913342 track_linearization-2.3.1/setup.cfg
+-rw-r--r--   0 edeno      (501) staff       (20)      495 2023-06-07 20:20:18.000000 track_linearization-2.3.1/setup.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-06-07 20:22:12.911991 track_linearization-2.3.1/track_linearization/
+-rw-r--r--   0 edeno      (501) staff       (20)      230 2022-09-26 22:44:15.000000 track_linearization-2.3.1/track_linearization/__init__.py
+-rw-r--r--   0 edeno      (501) staff       (20)    18657 2023-06-07 20:17:05.000000 track_linearization-2.3.1/track_linearization/core.py
+-rw-r--r--   0 edeno      (501) staff       (20)    11810 2023-06-07 20:17:05.000000 track_linearization-2.3.1/track_linearization/utils.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-06-07 20:22:12.912876 track_linearization-2.3.1/track_linearization.egg-info/
+-rw-r--r--   0 edeno      (501) staff       (20)      112 2023-06-07 20:22:12.000000 track_linearization-2.3.1/track_linearization.egg-info/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)      321 2023-06-07 20:22:12.000000 track_linearization-2.3.1/track_linearization.egg-info/SOURCES.txt
+-rw-r--r--   0 edeno      (501) staff       (20)        1 2023-06-07 20:22:12.000000 track_linearization-2.3.1/track_linearization.egg-info/dependency_links.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       57 2023-06-07 20:22:12.000000 track_linearization-2.3.1/track_linearization.egg-info/requires.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       20 2023-06-07 20:22:12.000000 track_linearization-2.3.1/track_linearization.egg-info/top_level.txt
```

### Comparing `track_linearization-2.3.0/README.md` & `track_linearization-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `track_linearization-2.3.0/track_linearization/core.py` & `track_linearization-2.3.1/track_linearization/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,20 +370,18 @@
     track_segment_id_with_nan[~is_bad] = track_segment_id
     return track_segment_id_with_nan
 
 
 def batch_linear_distance(
     track_graph, projected_track_positions, edge_ids, linear_zero_node_id
 ):
-
     copy_graph = track_graph.copy()
     linear_distance = []
 
     for (x3, y3), (node1, node2) in zip(projected_track_positions, edge_ids):
-
         x1, y1 = copy_graph.nodes[node1]["pos"]
         left_distance = sqrt((x3 - x1) ** 2 + (y3 - y1) ** 2)
         nx.add_path(copy_graph, [node1, "projected"], distance=left_distance)
 
         x2, y2 = copy_graph.nodes[node2]["pos"]
         right_distance = sqrt((x3 - x2) ** 2 + (y3 - y2) ** 2)
         nx.add_path(copy_graph, ["projected", node2], distance=right_distance)
```

### Comparing `track_linearization-2.3.0/track_linearization/utils.py` & `track_linearization-2.3.1/track_linearization/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     """
     track_graph = nx.Graph()
 
     for node_id, node_position in enumerate(node_positions):
         track_graph.add_node(node_id, pos=tuple(node_position))
 
-    for (node1, node2) in edges:
+    for node1, node2 in edges:
         pos1 = np.asarray(track_graph.nodes[node1]["pos"])
         pos2 = np.asarray(track_graph.nodes[node2]["pos"])
         distance = np.linalg.norm(pos1 - pos2)
         track_graph.add_edge(node1, node2, distance=distance)
 
     for edge_id, edge in enumerate(track_graph.edges):
         track_graph.edges[edge]["edge_id"] = edge_id
@@ -53,15 +53,18 @@
         Plots the names of the edges
     kwds : additional plotting keyworks for `draw_networkx`
 
     """
     if ax is None:
         ax = plt.gca()
     node_position = nx.get_node_attributes(track_graph, "pos")
-    nx.draw_networkx(track_graph, node_position, ax=ax, **kwds)
+    nx.draw_networkx_nodes(track_graph, node_position, ax=ax, **kwds)
+    for node_id1, node_id2 in track_graph.edges:
+        pos = np.stack((node_position[node_id1], node_position[node_id2]))
+        ax.plot(pos[:, 0], pos[:, 1], color="black", zorder=-1)
 
     if draw_edge_labels:
         edge_ids = {edge: ind for ind, edge in enumerate(track_graph.edges)}
         nx.draw_networkx_edge_labels(
             track_graph, node_position, edge_labels=edge_ids, ax=ax
         )
 
@@ -73,15 +76,14 @@
     ax=None,
     axis="x",
     other_axis_start=0.0,
     draw_edge_labels=False,
     node_size=300,
     node_color="#1f77b4",
 ):
-
     if ax is None:
         ax = plt.gca()
     # If no edge_order is given, then arange edges in the order passed to
     # construct the track graph
     if edge_order is None:
         edge_order = np.asarray(track_graph.edges)
```

