# Comparing `tmp/flatland-railway-extension-0.2.2.tar.gz` & `tmp/flatland-railway-extension-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flatland-railway-extension-0.2.2.tar", last modified: Mon Mar 27 20:21:12 2023, max compression
+gzip compressed data, was "flatland-railway-extension-0.2.3.tar", last modified: Wed Jun  7 04:47:06 2023, max compression
```

## Comparing `flatland-railway-extension-0.2.2.tar` & `flatland-railway-extension-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/
--rw-rw-rw-   0        0        0    21080 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/DynamicAgent.py
--rw-rw-rw-   0        0        0      686 2022-12-21 10:36:28.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/DynamicsResourceData.py
--rw-rw-rw-   0        0        0    10121 2023-03-27 20:18:24.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/FlatlandDynamics.py
--rw-rw-rw-   0        0        0     4829 2023-03-10 21:45:18.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
--rw-rw-rw-   0        0        0     8950 2023-03-27 15:17:52.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/FlatlandResourceAllocator.py
--rw-rw-rw-   0        0        0     1682 2022-12-21 10:36:28.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/InfrastructureData.py
--rw-rw-rw-   0        0        0     7890 2023-03-27 20:18:24.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
--rw-rw-rw-   0        0        0     5009 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/RollingStock.py
--rw-rw-rw-   0        0        0     1478 2022-12-21 10:36:28.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/XAgent.py
--rw-rw-rw-   0        0        0        0 2022-12-21 13:08:09.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/data_exports/
--rw-rw-rw-   0        0        0     6857 2022-12-21 10:36:28.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py
--rw-rw-rw-   0        0        0        0 2022-12-21 13:08:09.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/data_exports/__init__.py
--rw-rw-rw-   0        0        0     7031 2023-03-27 20:18:24.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_dynamics.py
--rw-rw-rw-   0        0        0     4913 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_extensions.py
--rw-rw-rw-   0        0        0     3981 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_graph.py
--rw-rw-rw-   0        0        0     2857 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
--rw-rw-rw-   0        0        0     6927 2023-03-27 15:17:30.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_simple_flatland_navigation.py
--rw-rw-rw-   0        0        0        0 2022-12-21 13:08:09.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/examples/__init__.py
--rw-rw-rw-   0        0        0     2751 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/FlatlandEnvironmentHelper.py
--rw-rw-rw-   0        0        0    15048 2023-03-10 21:45:18.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/FlatlandGraphBuilder.py
--rw-rw-rw-   0        0        0     7805 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/RailroadSwitchAnalyser.py
--rw-rw-rw-   0        0        0     9991 2022-12-21 10:36:28.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/RailroadSwitchCluster.py
--rw-rw-rw-   0        0        0      515 2022-11-15 13:11:08.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/Timer.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/utils/
--rw-rw-rw-   0        0        0      248 2022-12-28 20:59:52.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/utils/cached_methods.py
--rw-rw-rw-   0        0        0     5982 2023-03-16 20:19:45.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py
--rw-rw-rw-   0        0        0     6048 2023-03-16 20:19:45.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/utils/FlatlandRenderer.py
--rw-rw-rw-   0        0        0     2200 2023-03-16 20:19:45.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/utils/ShortestPathNextStepObservation.py
--rw-rw-rw-   0        0        0        0 2022-12-21 13:08:09.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/utils/__init__.py
--rw-rw-rw-   0        0        0       25 2023-03-16 21:01:59.000000 flatland-railway-extension-0.2.2/flatland_railway_extension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-27 20:21:11.000000 flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2023-03-27 20:21:11.000000 flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-03-27 20:21:11.000000 flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1965 2023-03-27 20:21:11.000000 flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       27 2023-03-27 20:21:11.000000 flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1214 2022-12-21 10:36:28.000000 flatland-railway-extension-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      455 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    14342 2023-03-27 20:18:24.000000 flatland-railway-extension-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 20:21:12.000000 flatland-railway-extension-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-03-27 20:17:57.000000 flatland-railway-extension-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.236448 flatland-railway-extension-0.2.3/
+-rw-rw-rw-   0        0        0     1214 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-06-07 04:47:06.236448 flatland-railway-extension-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    14346 2023-05-09 20:30:03.000000 flatland-railway-extension-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.189517 flatland-railway-extension-0.2.3/flatland_railway_extension/
+-rw-rw-rw-   0        0        0     3133 2023-06-01 07:54:21.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/FlatlandEnvironmentHelper.py
+-rw-rw-rw-   0        0        0    17522 2023-06-05 08:52:25.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/FlatlandGraphBuilder.py
+-rw-rw-rw-   0        0        0     7805 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/RailroadSwitchAnalyser.py
+-rw-rw-rw-   0        0        0     9991 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/RailroadSwitchCluster.py
+-rw-rw-rw-   0        0        0       25 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.220833 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/
+-rw-rw-rw-   0        0        0    21375 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/DynamicAgent.py
+-rw-rw-rw-   0        0        0      686 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/DynamicsResourceData.py
+-rw-rw-rw-   0        0        0    10121 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/FlatlandDynamics.py
+-rw-rw-rw-   0        0        0     4829 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
+-rw-rw-rw-   0        0        0     8950 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/FlatlandResourceAllocator.py
+-rw-rw-rw-   0        0        0     1682 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/InfrastructureData.py
+-rw-rw-rw-   0        0        0     1511 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py
+-rw-rw-rw-   0        0        0     8028 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
+-rw-rw-rw-   0        0        0     5009 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/RollingStock.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.220833 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.236448 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/data_exports/
+-rw-rw-rw-   0        0        0     6857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/data_exports/__init__.py
+-rw-rw-rw-   0        0        0     7031 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_dynamics.py
+-rw-rw-rw-   0        0        0     4913 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_extensions.py
+-rw-rw-rw-   0        0        0     3981 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_graph.py
+-rw-rw-rw-   0        0        0     2857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
+-rw-rw-rw-   0        0        0     6927 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_simple_flatland_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.236448 flatland-railway-extension-0.2.3/flatland_railway_extension/utils/
+-rw-rw-rw-   0        0        0     5982 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py
+-rw-rw-rw-   0        0        0     6048 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/utils/FlatlandRenderer.py
+-rw-rw-rw-   0        0        0     2200 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/utils/ShortestPathNextStepObservation.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/utils/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.3/flatland_railway_extension/utils/cached_methods.py
+drwxrwxrwx   0        0        0        0 2023-06-07 04:47:06.205160 flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-06-07 04:47:06.000000 flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1952 2023-06-07 04:47:06.000000 flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 04:47:06.000000 flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-07 04:47:06.000000 flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-07 04:47:06.000000 flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 04:47:06.236448 flatland-railway-extension-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-06-07 04:44:34.000000 flatland-railway-extension-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/DynamicAgent.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/DynamicAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Idea: Adrian Egli / Erik Nygren
 # Permission to use - If you use this or any idea out of this code for a
-# publication, you must credit the authors. No commerical
+# publication, you must credit the authors. No commercial
 # use allowed.
 from functools import lru_cache
 from typing import Tuple, List, Union
 
 import numpy as np
 from flatland.envs.agent_utils import EnvAgent
 from matplotlib import pyplot as plt
 
 from flatland_railway_extension.environments.DynamicsResourceData import DynamicsResourceData
 from flatland_railway_extension.environments.InfrastructureData import InfrastructureData
+from flatland_railway_extension.environments.MultiResourcesAllocationAgent import MultiResourcesAllocationAgent
 from flatland_railway_extension.environments.RollingStock import RollingStock
-from flatland_railway_extension.environments.XAgent import XAgent
 from flatland_railway_extension.utils.cached_methods import min_cached, max_cached
 
 _infrastructure_lru_cache_functions = []
 
 
 def enable_infrastructure_data_lru_cache(*args, **kwargs):
     def decorator(func):
@@ -28,38 +28,38 @@
 
 
 def reset_infrastructure_data_lru_cache():
     for func in _infrastructure_lru_cache_functions:
         func.cache_clear()
 
 
-class DynamicAgent(XAgent):
+class DynamicAgent(MultiResourcesAllocationAgent):
     def __init__(self, original_env_agent: EnvAgent):
         super(DynamicAgent, self).__init__(original_env_agent)
 
         # set the extended dynamic agent attributes
         self.set_length(100)
         self.set_mass(300)
         self.set_rolling_stock(RollingStock())
 
         # infrastructure
-        self.v_max_simulation = 300 / 3.6
+        self.v_max_simulation: float = 300 / 3.6
         self._infrastructure_data: Union[InfrastructureData, None] = None
 
         # set the internal simulation data (resource allocation, velocity, ... )
 
         # current pointer and data to visited cells/resources
         self.visited_cell_path: List[Tuple[int, int]] = []
         self.visited_direction_path: List[Tuple[int, int]] = []
         self.visited_cell_distance: List[float] = []
-        self.visited_cell_path_reservation_point_index = 0
-        self.visited_cell_path_end_of_agent_index = 0
-        self.visited_cell_path_start_of_agent_index = 0
-        self.visited_cell_path_reservation_point_distance = 0
-        self.visited_cell_path_end_of_agent_distance = 0
+        self.visited_cell_path_reservation_point_index: int = 0
+        self.visited_cell_path_end_of_agent_index: int = 0
+        self.visited_cell_path_start_of_agent_index: int = 0
+        self.visited_cell_path_reservation_point_distance: int = 0
+        self.visited_cell_path_end_of_agent_distance: int = 0
 
         # current simulation data
         self.current_velocity_reservation_point: float = 0.0
         self.current_velocity_agent: float = 0.0
         self.current_acceleration_agent: float = 0.0
         self.current_max_velocity: float = 0.0
         self.current_distance_reservation_point: float = 0.0
@@ -290,15 +290,14 @@
         # check and allow reservation point move forward
         move_reservation_point = \
             self.current_distance_reservation_point > self.visited_cell_path_reservation_point_distance
 
         return move_reservation_point
 
     def update_agent_positions(self):
-        self._max_episode_steps = 10000
         pos = self.position
         if pos is not None:
             # The resource is only added if it was not the last one added - i.e. the agent switched to a new one.
             allocated_resource = self.get_allocated_resource()
             if len(allocated_resource) > 0:
                 allocated_resource = [allocated_resource[len(allocated_resource) - 1]]
             if pos not in allocated_resource:
@@ -315,15 +314,15 @@
                 cmp_value=self.current_distance_agent,
                 start_index=self.visited_cell_path_end_of_agent_index
             )
 
             if self.visited_cell_path_end_of_agent_index >= self.visited_cell_path_reservation_point_index:
                 self.visited_cell_path_end_of_agent_index = self.visited_cell_path_reservation_point_index - 1
 
-            # update current position of the agent' start with respect to visited cells
+            # update current position of the agent start with respect to visited cells
             self.visited_cell_path_start_of_agent_index = DynamicAgent.get_first_element_index_greater_than(
                 input_list=self.visited_cell_distance,
                 cmp_value=self.current_distance_agent + self.length,
                 start_index=self.visited_cell_path_start_of_agent_index
             )
 
             if self.visited_cell_path_start_of_agent_index >= self.visited_cell_path_reservation_point_index:
@@ -341,23 +340,23 @@
             self.hard_brake_data.append(self.hard_brake)
             self.is_malfunction_state_data.append(self.state.is_malfunction_state())
         else:
             self.set_hard_brake(True)
 
     def set_length(self, length: float):
         '''
-        Sets the physical total length in meter
+        Sets the physical total length
         :param length: in meter
         '''
         self.length: float = length
 
     def set_mass(self, mass: float):
         '''
-        Sets the physical total mass in tonne
-        :param mass:
+        Sets the physical total mass
+        :param mass: in tonne
         '''
         self.mass: float = mass
 
     def set_rolling_stock(self, rolling_stock: RollingStock):
         '''
         Sets the rolling stock information / traction data
         :param rolling_stock: a reference to the rolling stock object
@@ -378,22 +377,28 @@
 
     def set_tractive_effort_rendering(self, enable=True):
         self._enabled_tractive_effort_rendering = enable
 
     @staticmethod
     def get_first_element_index_greater_than(input_list, cmp_value, start_index=0):
         '''
-        This methods calculates the same as ...
+        This method calculates the same as ...
 
-        indices = np.argwhere(np.array(input_list) > cmp_value)
-        if len(indices) == 0:
-            if len(self.visited_cell_distance) == 0:
-                return 0
-        else:
-            return indices[0][0]
+        >>> input_list = [1,2,3,4,5,6]
+        >>> cmp_value = 2
+        >>> indices = np.argwhere(np.array(input_list) > cmp_value)
+        >>> def test_value(in_indices, in_input_list) -> int:
+        ...     if len(in_indices) == 0:
+        ...         if len(in_input_list) == 0:
+        ...             return 0
+        ...     else:
+        ...         return indices[0][0]
+        ...     return 0
+        >>> test_value(indices, input_list)
+        2
 
         ... but 20x faster for small input_lists
         '''
         idx = start_index
         while idx < (len(input_list) - 1):
             val = input_list[idx]
             if val > cmp_value:
```

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/DynamicsResourceData.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/DynamicsResourceData.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/FlatlandDynamics.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/FlatlandDynamics.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/FlatlandResourceAllocator.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/FlatlandResourceAllocator.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/InfrastructureData.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/InfrastructureData.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from flatland.envs.observations import GlobalObsForRailEnv
 from flatland.envs.rail_env import RailEnv
 from flatland.envs.rail_env_action import RailEnvActions
 from flatland.envs.step_utils import env_utils
 
 from flatland_railway_extension.RailroadSwitchCluster import RailroadSwitchCluster
 from flatland_railway_extension.environments.FlatlandResourceAllocator import FlatlandResourceAllocator
-from flatland_railway_extension.environments.XAgent import XAgent
+from flatland_railway_extension.environments.MultiResourcesAllocationAgent import MultiResourcesAllocationAgent
 
 
 class MultiResourcesAllocationRailEnv(RailEnv):
     def __init__(self,
                  width,
                  height,
                  rail_generator=None,
@@ -67,15 +67,15 @@
         self._railroad_switch_cluster_connecting_edge_locking = railroad_switch_cluster_connecting_edge_locking
 
     def deactivate_railroad_switch_cluster_locking(self):
         self._railroad_switch_cluster = None
         self._railroad_switch_cluster_switch_group_locking = False
         self._railroad_switch_cluster_connecting_edge_locking = False
 
-    def _allocate_resources(self, agent: XAgent, positions: List[Tuple[int, int]]):
+    def _allocate_resources(self, agent: MultiResourcesAllocationAgent, positions: List[Tuple[int, int]]):
         if self._flatland_resource_allocator is None:
             return True
         resources = positions
         if self._railroad_switch_cluster is not None:
             for position in positions:
                 if position is not None:
                     cluster_id = self._railroad_switch_cluster.get_cluster_id(position)
@@ -86,28 +86,28 @@
                                 resources.append(r)
                     if self._railroad_switch_cluster_connecting_edge_locking:
                         for r in cluster_member.connecting_edge_cluster_cell_members:
                             if r not in resources:
                                 resources.append(r)
         return self._flatland_resource_allocator.allocate_resource(agent.handle, resources)
 
-    def allocate_resources_at_position(self, agent: XAgent, position: Tuple[int, int]) -> bool:
+    def allocate_resources_at_position(self, agent: MultiResourcesAllocationAgent, position: Tuple[int, int]) -> bool:
         return self._allocate_resources(agent, [position])
 
-    def allocate_current_resources(self, agent: XAgent) -> bool:
+    def allocate_current_resources(self, agent: MultiResourcesAllocationAgent) -> bool:
         positions = agent.get_allocated_resource()
         if len(positions) == 0 and agent.position is not None:
             positions.append(agent.position)
         return self._allocate_resources(agent, positions)
 
     def reset_agents(self):
         super(MultiResourcesAllocationRailEnv, self).reset_agents()
         x_agents = []
         for agent in self.agents:
-            x_agents.append(XAgent(agent))
+            x_agents.append(MultiResourcesAllocationAgent(agent))
         self.agents = x_agents
 
     def step(self, action_dict_: Dict[int, RailEnvActions]):
         if self._flatland_resource_allocator is not None:
             self._flatland_resource_allocator.reset_locks()
             for agent_handle, agent in enumerate(self.agents):
                 agent.all_resource_ok(self.allocate_current_resources(agent))
```

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/RollingStock.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/RollingStock.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/environments/XAgent.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Tuple, List
 
 from flatland.envs.agent_utils import EnvAgent
 
 
-class XAgent(EnvAgent):
+class MultiResourcesAllocationAgent(EnvAgent):
     def __init__(self, original_env_agent: EnvAgent):
-        super(XAgent, self).__init__(original_env_agent.initial_position,
-                                     original_env_agent.initial_direction, original_env_agent.direction,
-                                     original_env_agent.target)
+        super(MultiResourcesAllocationAgent, self).__init__(
+            original_env_agent.initial_position,
+            original_env_agent.initial_direction, original_env_agent.direction,
+            original_env_agent.target)
 
         # copy all attributes data from original EnvAgent allocated in RailEnv
         self._copy_attribute_from_env_agent(original_env_agent)
         self._done = False
 
     def _copy_attribute_from_env_agent(self, env_agent: EnvAgent):
         '''
@@ -35,11 +36,11 @@
     def all_resource_ok(self, resource_allocation_ok):
         pass
 
     def update_agent(self):
         pass
 
     def reset(self):
-        super(XAgent, self).reset()
+        super(MultiResourcesAllocationAgent, self).reset()
 
     def do_debug_plot(self, idx=1, nbr_agents=1, show=True, show_title=True):
         pass
```

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_dynamics.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_dynamics.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_extensions.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_extensions.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_graph.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_graph.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/examples/demo_simple_flatland_navigation.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/examples/demo_simple_flatland_navigation.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/FlatlandEnvironmentHelper.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/FlatlandEnvironmentHelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import random
+from typing import Union, Type
 
 import numpy as np
+from flatland.core.env_observation_builder import ObservationBuilder
 from flatland.envs.malfunction_generators import MalfunctionParameters, ParamMalfunctionGen
 # import all flatland dependances
 from flatland.envs.rail_env import RailEnv
 from flatland.envs.rail_generators import sparse_rail_generator
 
 from flatland_railway_extension.utils.ShortestPathNextStepObservation import ShortestPathNextStepObservation
 
 
 class FlatlandEnvironmentHelper:
-    def __init__(self, rail_env=RailEnv, grid_width=30, grid_height=40, number_of_agents=10, n_cities=3,
-                 random_seed=0):
+    def __init__(self, rail_env: Type[RailEnv] = RailEnv,
+                 grid_width=30, grid_height=40, number_of_agents=10, n_cities=3,
+                 random_seed=0, obs_builder_object: Union[ObservationBuilder, None] = None):
         self.grid_width = grid_width
         self.grid_height = grid_height
         self.number_of_agents = number_of_agents
         self.n_cities = n_cities
         self._random_seed(random_seed)
+        self._obs_builder_object = obs_builder_object
         self.env = self._create_flatland_env(rail_env)
         self.env.reset()
 
     def _random_seed(self, random_seed):
         self.random_seed = random_seed
         np.random.seed(self.random_seed)
         random.seed(self.random_seed)
 
-    def _create_flatland_env(self, rail_env,
+    def _create_flatland_env(self, rail_env: Type[RailEnv],
                              max_rails_between_cities=2,
                              max_rails_in_city=4,
                              malfunction_rate=1 / 1000) -> RailEnv:
+
+        if self._obs_builder_object == None:
+            self._obs_builder_object = ShortestPathNextStepObservation()
+
         return rail_env(
             width=self.grid_width,
             height=self.grid_height,
             rail_generator=sparse_rail_generator(
                 max_num_cities=self.n_cities,
                 seed=self.random_seed,
                 grid_mode=True,
@@ -42,15 +50,15 @@
             malfunction_generator=ParamMalfunctionGen(
                 MalfunctionParameters(
                     malfunction_rate=malfunction_rate, min_duration=10, max_duration=50
                 )
             ),
             random_seed=self.random_seed,
             number_of_agents=self.number_of_agents,
-            obs_builder_object=ShortestPathNextStepObservation()
+            obs_builder_object=self._obs_builder_object
         )
 
     def get_rail_env(self):
         return self.env
 
     def get_agent_position_and_direction(self, handle):
         '''
```

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/FlatlandGraphBuilder.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/FlatlandGraphBuilder.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,24 @@
 from flatland_railway_extension.RailroadSwitchAnalyser import RailroadSwitchAnalyser
 from flatland_railway_extension.environments.InfrastructureData import InfrastructureData
 
 
 class FlatlandGraphBuilder:
     def __init__(self,
                  railroad_switch_analyser: RailroadSwitchAnalyser,
-                 infrastructure_data: Union[InfrastructureData, None] = None):
+                 infrastructure_data: Union[InfrastructureData, None] = None,
+                 activate_simplified: bool = False):
         self.railroad_switch_analyser = railroad_switch_analyser
         self._graph: Union[nx.DiGraph, None] = None
         self._nodes: Union[Dict[str, Tuple[int, int, float]], None] = None
         self.set_infrastructure_data(infrastructure_data)
-        self.activate_full_graph()
+        if activate_simplified:
+            self.activate_simplified()
+        else:
+            self.activate_full_graph()
 
     def set_infrastructure_data(self, infrastructure_data: Union[InfrastructureData, None]):
         self._infrastructure_data = infrastructure_data
 
     def activate_full_graph(self):
         self._graph, self._nodes, self._from_vertex_edge_map = self._create_full_graph()
 
@@ -240,30 +244,32 @@
 
     @staticmethod
     def get_resource_id_from_node_id(node_name: str):
         xy_d = node_name.split('_')
         resource_id = '{}_{}'.format(int(xy_d[0]), int(xy_d[1]))
         return resource_id
 
+    def get_mapped_vertex(self, flatland_position, flatland_direction):
+        node_key = '{}_{}_{}'.format(flatland_position[0], flatland_position[1], flatland_direction)
+        return self._from_vertex_edge_map.get(node_key)
+
     def get_shortest_path(self, start_position, start_direction, target_position, weight=None):
         '''
         This methods traverse the _graph to get shortest path. The target gets scaned for all four incoming directions.
         :param start_position: 2d coordinate
         :param start_direction: orientation passed a agent moving direction
         :param target_position: 2d coordinate of target position
         :return: shortest path, all paths, len of all found paths
         '''
-        from_node = '{}_{}_{}'.format(start_position[0], start_position[1], start_direction)
+        from_edge = self.get_mapped_vertex(start_position, start_direction)
         paths = []
         paths_len = []
         for target_direction in range(4):
             path = []
-            to_node = '{}_{}_{}'.format(target_position[0], target_position[1], target_direction)
-            from_edge = self._from_vertex_edge_map.get(from_node)
-            to_edge = self._from_vertex_edge_map.get(to_node)
+            to_edge = self.get_mapped_vertex(target_position, target_direction)
             if from_edge is not None and to_edge is not None:
                 from_node_intern = from_edge[0]
                 to_node_intern = to_edge[1]
                 fn = self.get_graph().nodes.get(from_node_intern, None)
                 tn = self.get_graph().nodes.get(to_node_intern, None)
 
                 if fn is not None and tn is not None:
@@ -289,14 +295,55 @@
             path_len = len(path)
             if path_len == 0:
                 path_len = np.inf
             paths_len.append(path_len)
         arg_sorted_path_len = np.argsort(paths_len)
         return paths[arg_sorted_path_len[0]], paths, paths_len
 
+    def get_shortest_path_edges(self, start_position, start_direction, target_position, weight=None):
+        '''
+        This methods traverse the _graph to get shortest path. The target gets scaned for all four incoming directions.
+        :param start_position: 2d coordinate
+        :param start_direction: orientation passed a agent moving direction
+        :param target_position: 2d coordinate of target position
+        :return: shortest path [edge[resource],..., edge[...]], all paths, total nbr of resource (len) of all found paths
+        '''
+        from_edge = self.get_mapped_vertex(start_position, start_direction)
+        paths = []
+        paths_len = []
+        for target_direction in range(4):
+            path = []
+            to_edge = self.get_mapped_vertex(target_position, target_direction)
+            path_len = 0
+            if from_edge is not None and to_edge is not None:
+                from_node_intern = from_edge[0]
+                to_node_intern = to_edge[1]
+                fn = self.get_graph().nodes.get(from_node_intern, None)
+                tn = self.get_graph().nodes.get(to_node_intern, None)
+
+                if fn is not None and tn is not None:
+                    try:
+                        s_path = nx.shortest_path(self.get_graph(), from_node_intern, to_node_intern, weight=weight)
+                        start_p = from_node_intern
+                        for p in s_path:
+                            if start_p != p:
+                                # xy, _ = FlatlandGraphBuilder.get_coordinate_direction_from_node_id(p)
+                                resources = self.get_graph().get_edge_data(start_p, p).get('resources')
+                                path.append(resources)
+                                path_len += len(resources)
+                            start_p = p
+                    except nx.NetworkXNoPath:
+                        pass
+            paths.append(path)
+            if path_len == 0 and not fast_position_equal(start_position, target_position):
+                path_len = np.inf
+            paths_len.append(path_len)
+        arg_sorted_path_len = np.argsort(paths_len)
+        return paths[arg_sorted_path_len[0]], paths, paths_len
+
     def prepare_observation_data_plot(self, start_position, start_direction, target_position, weight=None):
         '''
         Prepare the classified cells (railroad_switches, railroad_switch_neighbours) to render. The rendering used
         the observation rendering data structure.
         :param start_position: 2d coordinate
         :param start_direction: orientation passed a agent moving direction
         :param target_position: 2d coordinate of target position
```

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/RailroadSwitchAnalyser.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/RailroadSwitchAnalyser.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/RailroadSwitchCluster.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/RailroadSwitchCluster.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/utils/FlatlandRenderer.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/utils/FlatlandRenderer.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension/utils/ShortestPathNextStepObservation.py` & `flatland-railway-extension-0.2.3/flatland_railway_extension/utils/ShortestPathNextStepObservation.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/flatland_railway_extension.egg-info/SOURCES.txt` & `flatland-railway-extension-0.2.3/flatland_railway_extension.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 LICENSE
 README.md
 setup.py
 flatland_railway_extension/FlatlandEnvironmentHelper.py
 flatland_railway_extension/FlatlandGraphBuilder.py
 flatland_railway_extension/RailroadSwitchAnalyser.py
 flatland_railway_extension/RailroadSwitchCluster.py
-flatland_railway_extension/Timer.py
 flatland_railway_extension/__init__.py
 flatland_railway_extension.egg-info/PKG-INFO
 flatland_railway_extension.egg-info/SOURCES.txt
 flatland_railway_extension.egg-info/dependency_links.txt
 flatland_railway_extension.egg-info/requires.txt
 flatland_railway_extension.egg-info/top_level.txt
 flatland_railway_extension/environments/DynamicAgent.py
 flatland_railway_extension/environments/DynamicsResourceData.py
 flatland_railway_extension/environments/FlatlandDynamics.py
 flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
 flatland_railway_extension/environments/FlatlandResourceAllocator.py
 flatland_railway_extension/environments/InfrastructureData.py
+flatland_railway_extension/environments/MultiResourcesAllocationAgent.py
 flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
 flatland_railway_extension/environments/RollingStock.py
-flatland_railway_extension/environments/XAgent.py
 flatland_railway_extension/environments/__init__.py
 flatland_railway_extension/examples/__init__.py
 flatland_railway_extension/examples/demo_flatland_dynamics.py
 flatland_railway_extension/examples/demo_flatland_extensions.py
 flatland_railway_extension/examples/demo_flatland_graph.py
 flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
 flatland_railway_extension/examples/demo_simple_flatland_navigation.py
```

### Comparing `flatland-railway-extension-0.2.2/LICENSE` & `flatland-railway-extension-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.2/README.md` & `flatland-railway-extension-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 augmentation of reality is that the agents behave more dynamically in terms of movement. Agents are able to interact more realistic with each others. The vehicle movement dynamics of each agent can be enabled by using
 the [FlatlandDynamics](https://github.com/aiAdrian/flatland_railway_extension/blob/master/flatland_railway_extension/environments/FlatlandDynamics.py)
 environment. By combing all of those extensions the simulation will become very realistic.
 
 The goal of this extension package is that researchers can show where the limits and strengths of their proposed methods
 lie. Some optimization methods will not be able to deal with vehicle dynamics; some algorithms are not suitable for
 solving problems with multiple resource allocation at time. Others are might very slow to solve such complex dynamic
-problems and there is might a solution which can solve it in raisonable time, but the solution quality must be further
+problems and there is might a solution which can solve it in reasonable time, but the solution quality must be further
 improved. It's very exciting to see where the effective limits of each method lie and whether someone find a real-time
 solver of all kind of those problems.
 
 ### Example
 
 <p align="center" width="100%">
     <img width="33%" src="https://raw.githubusercontent.com/aiAdrian/flatland_railway_extension/master/images/flatland_scenario.png"> 
@@ -172,20 +172,20 @@
 ## Working code
 
 - [Google coLab notebook - Recife export](https://github.com/aiAdrian/flatland_railway_extension/blob/master/Flatland_recife.ipynb)
 - [Google coLab notebook - Simulation with multi-resource reservation](https://github.com/aiAdrian/flatland_railway_extension/blob/master/Flatland_Resource_Allocation.ipynb)
 - [Google coLab notebook - Flatland dynamics](https://github.com/aiAdrian/flatland_railway_extension/blob/master/Flatland_Dynamics.ipynb)
 
 ## Installation 
-The code is tested with Python 3.6, 3.7 and is expected to also work with higher versions of Python.
+The code is tested with Python (3.6), *3.7* - expected to work with higher versions of Python.
 
 #### Prerequisites (optional)
 Install [Anaconda](https://www.anaconda.com/products/distribution) and create a new conda environment: 
 ```
-$ conda create python=3.6 --name flatland-ext
+$ conda create python=3.7 --name flatland-ext
 $ conda activate flatland-ext
 ```
 
 #### From sources
 The Flatland code source is available from [AIcrowd gitlab](https://gitlab.aicrowd.com/flatland/flatland) and Flatland railway extension can be found at [github](https://github.com/aiAdrian/flatland_railway_extension): 
 ```
 $ git clone http://gitlab.aicrowd.com/flatland/flatland.git
@@ -242,11 +242,11 @@
 ##### Permission to use
 
 If you use this or any idea out of this code for/in any academic publication or commercial products -
 you must credit the authors.
 
 
 
-[^1]: On Windows Subsystem for Linux (WSL) you may need to install some additional packages `pip install pyvirtualdisplay`, `pip install piglet` and `sudo apt install libnvidia-gl-440` to get the rendering working. However, using Flatland Railway Extension with WSL is not recommended, we recommend native Windows or Linux operating system. OS/X is not tested yet.
+[^1]: On Windows Subsystem for Linux (WSL) you may need to install some additional packages `pip install pyvirtualdisplay`, `pip install piglet` and `sudo apt install libnvidia-gl-440` to get the rendering working. However, using Flatland Railway Extension with WSL is not recommended, we recommend native Windows or Linux operating system. OS/X is not very well tested yet.
```

### Comparing `flatland-railway-extension-0.2.2/setup.py` & `flatland-railway-extension-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # twine upload dist/*
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='flatland-railway-extension',
-    version='0.2.2',
+    version='0.2.3',
     author='Adrian Egli',
     author_email="3dhelp@gmail.com",
     description='Extends Flatland Railway Simulator with helpful features.',
     url='https://github.com/aiAdrian/flatland_railway_extension',
     keywords='flatland, railway, extension, dynamics, simulation, multi-agent, reinforcement learning',
     python_requires='>=3.6, <4',
     packages=find_packages('.'),
```

