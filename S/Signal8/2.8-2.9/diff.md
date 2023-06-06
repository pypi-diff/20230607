# Comparing `tmp/Signal8-2.8.tar.gz` & `tmp/Signal8-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.8.tar", last modified: Mon Jun  5 17:29:45 2023, max compression
+gzip compressed data, was "Signal8-2.9.tar", last modified: Tue Jun  6 22:07:51 2023, max compression
```

## Comparing `Signal8-2.8.tar` & `Signal8-2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.432397 Signal8-2.8/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.8/LICENSE
--rw-rw-rw-   0        0        0     4369 2023-06-05 17:29:45.431397 Signal8-2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3881 2023-06-01 21:25:48.000000 Signal8-2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.339880 Signal8-2.8/Signal8/
--rw-rw-rw-   0        0        0    11220 2023-06-05 17:28:53.000000 Signal8-2.8/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-2.8/Signal8/__init__.py
--rw-rw-rw-   0        0        0      253 2023-06-05 17:26:53.000000 Signal8-2.8/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.426399 Signal8-2.8/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.8/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5783 2023-06-05 17:17:47.000000 Signal8-2.8/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-05 17:25:42.000000 Signal8-2.8/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-2.8/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.8/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12407 2023-06-05 17:15:50.000000 Signal8-2.8/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.8/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:29:45.382879 Signal8-2.8/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4369 2023-06-05 17:29:44.000000 Signal8-2.8/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-05 17:29:45.000000 Signal8-2.8/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:29:44.000000 Signal8-2.8/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 17:29:44.000000 Signal8-2.8/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 17:29:45.433400 Signal8-2.8/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-05 17:29:06.000000 Signal8-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.629105 Signal8-2.9/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.9/LICENSE
+-rw-rw-rw-   0        0        0     5556 2023-06-06 22:07:51.627104 Signal8-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.484102 Signal8-2.9/Signal8/
+-rw-rw-rw-   0        0        0    11051 2023-06-06 22:06:46.000000 Signal8-2.9/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-2.9/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-06-06 22:03:30.000000 Signal8-2.9/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.619105 Signal8-2.9/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.9/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5809 2023-06-06 17:48:52.000000 Signal8-2.9/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2811 2023-06-06 21:50:32.000000 Signal8-2.9/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-2.9/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.9/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-2.9/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.9/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.536105 Signal8-2.9/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5556 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 22:07:51.629105 Signal8-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-06 22:06:58.000000 Signal8-2.9/setup.py
```

### Comparing `Signal8-2.8/LICENSE` & `Signal8-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.8/Signal8/Signal8.py` & `Signal8-2.9/Signal8/Signal8.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 class Scenario(BaseScenario):
     def make_world(self, problem_type, num_agents):
         world = World()
         self._add_logger()
         world.problem_type = problem_type
         
         self.npc = []
-        self.obstacle_locks = []
         self.scripted_obstacle_threads = []
         self.scripted_obstacle_running = False
 
         world.agents = [Agent() for _ in range(num_agents)]
         for i, agent in enumerate(world.agents):
             agent.name = f"agent_{i}"
             agent.collide = True
@@ -100,15 +99,15 @@
 
         return temp_goal_constr
     
     # Reset position of dynamic obstacles
     def _reset_dynamic_obstacle(self, world, obstacle, np_random, temp_dynamic_obs_constr):
         obstacle.size = 0.025
         obstacle.movable = True
-        self.obstacle_locks += [threading.Lock()]
+        obstacle.lock = threading.Lock()
         obstacle.color = np.array([0.26, 0.32, 0.36])
         obstacle.state.p_vel = np.zeros(world.dim_p)
         dynamic_obs_constr = random.choice(temp_dynamic_obs_constr)
         obstacle.state.p_pos = np_random.uniform(*zip(*dynamic_obs_constr))
         temp_dynamic_obs_constr.remove(dynamic_obs_constr)
 
     # Reset position of static obstacles, taking leftover entities from goal constraints
@@ -144,27 +143,25 @@
                 self._reset_dynamic_obstacle(world, obstacle, np_random, temp_dynamic_obs_constr)
                 self.npc += [NPC(obstacle.state.p_pos)]
             else:
                 self._reset_static_obstacle(world, obstacle, np_random, temp_static_obs_constr)
     
     # Start a thread for each dynamic obstacle
     def _start_scripted_obstacles(self, world):
-        idx = 0
         self.scripted_obstacle_running = True
         for obstacle in world.obstacles:
             if obstacle.movable:
-                t = threading.Thread(target=self.run_scripted_obstacle, args=(world, obstacle, idx))
+                t = threading.Thread(target=self.run_scripted_obstacle, args=(world, obstacle))
                 t.start()
                 self.scripted_obstacle_threads.append(t)   
-                idx += 1
                 
-    def reset_world(self, world, np_random, problem_name=None):
+    def reset_world(self, world, np_random, instance_name=None):
         self.npc.clear()
         self.stop_scripted_obstacles()
-        self._set_problem_instance(world, np_random, problem_name)
+        self._set_problem_instance(world, np_random, instance_name)
         leftover_entities = self._reset_agents_and_goals(world, np_random)
         self._reset_obstacles(world, np_random, leftover_entities)
         self._start_scripted_obstacles(world)
     
     # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
@@ -177,15 +174,15 @@
         max_observable_dist = agent.max_observable_dist
         
         observed_obstacles = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_obstacles)]
         observed_goal = np.full_like(agent_pos, max_observable_dist)
         
         for i, obstacle in enumerate(world.obstacles):
             if obstacle.movable:
-                with self.obstacle_locks[i]:
+                with obstacle.lock:
                     obs_pos = obstacle.state.p_pos
             else:
                 obs_pos = obstacle.state.p_pos
             relative_pos = obs_pos - agent_pos
             dist = np.linalg.norm(relative_pos)
             if dist <= max_observable_dist:
                 observed_obstacles[i] = relative_pos
@@ -195,18 +192,18 @@
         goal_dist = np.linalg.norm(relative_goal_pos)
         if goal_dist <= max_observable_dist:
             observed_goal = relative_goal_pos
         
         return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
             
     # Run a thread for each scripted obstacle
-    def run_scripted_obstacle(self, world, obstacle, obstacle_idx):
+    def run_scripted_obstacle(self, world, obstacle):
         sensitivity = 2.0
         while self.scripted_obstacle_running:
-            with self.obstacle_locks[obstacle_idx]:
+            with obstacle.lock:
                 # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
                 action = self._action_callback(obstacle, world)
                 obstacle.action = action * sensitivity
                 obstacle.move()
                 time.sleep(0.25)
         
     # disaster response: increase obstacle size to resemble increasing size of fire
@@ -232,15 +229,14 @@
 
     # Stop all threads for scripted obstacles
     def stop_scripted_obstacles(self):
         self.scripted_obstacle_running = False
         for t in self.scripted_obstacle_threads:
             t.join()
         self.scripted_obstacle_threads.clear()
-        self.obstacle_locks.clear()
         
     # Create a logger to log information from threads
     def _add_logger(self):
         self.logger = logging.getLogger('Dynamic Obstacles')
         self.logger.setLevel(logging.DEBUG)
 
         ch = logging.StreamHandler()
```

### Comparing `Signal8-2.8/Signal8/utils/core.py` & `Signal8-2.9/Signal8/utils/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         super().__init__()
         # entity can be moved / pushed
         self.movable = False
         # action
         self.action = None
         # script behavior to execute
         self.action_callback = None
+        self.lock = None
     
     # updates the state of the obstacle
     def move(self, dt=0.1, damping=0.25):
         self.state.p_vel = self.state.p_vel * (1 - damping)
         self.state.p_vel += (self.action / self.mass) * dt
         self.state.p_pos += self.state.p_vel * dt
```

### Comparing `Signal8-2.8/Signal8/utils/npc.py` & `Signal8-2.9/Signal8/utils/npc.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     
     def get_scripted_action(self, obs, instance_num):
         destination = self.farming_instances[instance_num]['destination']
         direction = self.farming_instances[instance_num]['direction']
         bounds = self.farming_instances[instance_num]['bounds']
         
         action = np.array([0, 0])
-        x, y, = obs.state.p_pos
+        with obs.lock:
+            x, y, = obs.state.p_pos
         
         if self.status == 'moving_to_destination':
             if np.allclose([x, y], destination, atol=0.05):
                 self.status = 'zigzagging'
                 self.direction = direction
             else:
                 action = self._move_towards_point(x, y, destination)
```

### Comparing `Signal8-2.8/Signal8/utils/problems.py` & `Signal8-2.9/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.8/Signal8/utils/simple_env.py` & `Signal8-2.9/Signal8/utils/simple_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,18 +129,18 @@
     def get_start_state(self):
         if not self._reset_called:
             raise Exception("Cannot get start state without calling reset() first")
         
         agent_pos = np.array([agent.state.p_pos for agent in self.world.agents])
         goal_pos = np.array([(agent.goal_a.state.p_pos, agent.goal_b.state.p_pos) for agent in self.world.agents])
         try:
-            [self.scenario.obstacle_locks[i].acquire() for i in range(len(self.scenario.obstacle_locks))]
+            [obs.lock.acquire() for obs in self.world.obstacles if obs.lock is not None]
             obs_pos = np.array([obs.state.p_pos for obs in self.world.obstacles])
         finally:
-            [self.scenario.obstacle_locks[i].release() for i in range(len(self.scenario.obstacle_locks))]
+            [obs.lock.release() for obs in self.world.obstacles if obs.lock is not None]
         
         entities = {'agents': agent_pos, 'goals': goal_pos, 'obstacles': obs_pos}
         return entities
         
     def _execute_world_step(self):
         # set action for each agent
         for i, agent in enumerate(self.world.agents):
@@ -202,16 +202,15 @@
         goal_a_dist = [np.linalg.norm(agent.state.p_pos - agent.goal_a.state.p_pos) for agent in self.world.agents]
         goal_b_dist = [np.linalg.norm(agent.state.p_pos - agent.goal_b.state.p_pos) for agent in self.world.agents]
         static_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in static_obs)
                            for agent in self.world.agents]
 
         crossed_threshold_static = [dist <= static_obs_threshold for dist in static_obs_dist]
 
-        for lock in self.scenario.obstacle_locks:
-            lock.acquire()
+        [obs.lock.acquire() for obs in dynamic_obs]
 
         try:
             dynamic_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in dynamic_obs)
                                 for agent in self.world.agents] 
             dynamic_obs_threshold = [agent.size + obs.size for agent, obs in zip(self.world.agents, dynamic_obs)]   
 
             crossed_threshold_dynamic = [dist <= threshold for dist, threshold in zip(dynamic_obs_dist, dynamic_obs_threshold)]
@@ -226,16 +225,15 @@
 
             for i, dist in enumerate(goal_b_dist):
                 if self.world.agents[i].reached_goal:
                     if dist <= goal_dist_threshold:
                         self.agents[i].reached_safety = True
                         terminations[i] = True
         finally:
-            for lock in self.scenario.obstacle_locks:
-                lock.release()
+            [obs.lock.release() for obs in dynamic_obs]
 
         return {'terminations': terminations, 'truncations': truncations}
 
 
     def step(self, action):
         if (
             self.terminations[self.agent_selection]
```

### Comparing `Signal8-2.8/Signal8/utils/test_dynamic_obs.py` & `Signal8-2.9/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.8/Signal8.egg-info/SOURCES.txt` & `Signal8-2.9/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.8/setup.py` & `Signal8-2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.8",
+    version="2.9",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

