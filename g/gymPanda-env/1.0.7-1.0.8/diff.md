# Comparing `tmp/gymPanda_env-1.0.7-py3-none-any.whl.zip` & `tmp/gymPanda_env-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3402 bytes, number of entries: 7
+Zip file size: 3403 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      128 b- defN 23-Jun-07 18:48 gym_panda_env/__init__.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 18:46 gym_panda_env/envs/__init__.py
--rw-rw-r--  2.0 unx     4822 b- defN 23-Jun-07 19:26 gym_panda_env/envs/panda_env.py
--rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:26 gymPanda_env-1.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:26 gymPanda_env-1.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:26 gymPanda_env-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:26 gymPanda_env-1.0.7.dist-info/RECORD
-7 files, 5917 bytes uncompressed, 2380 bytes compressed:  59.8%
+-rw-rw-r--  2.0 unx     4827 b- defN 23-Jun-07 19:27 gym_panda_env/envs/panda_env.py
+-rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/RECORD
+7 files, 5922 bytes uncompressed, 2381 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gym_panda_env/envs/__init__.py
 Comment: 
 
 Filename: gym_panda_env/envs/panda_env.py
 Comment: 
 
-Filename: gymPanda_env-1.0.7.dist-info/METADATA
+Filename: gymPanda_env-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: gymPanda_env-1.0.7.dist-info/WHEEL
+Filename: gymPanda_env-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: gymPanda_env-1.0.7.dist-info/top_level.txt
+Filename: gymPanda_env-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: gymPanda_env-1.0.7.dist-info/RECORD
+Filename: gymPanda_env-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_panda_env/envs/panda_env.py

```diff
@@ -73,15 +73,15 @@
 
         state_object= [random.uniform(0.5,0.8),random.uniform(-0.2,0.2),0.05]
         self.objectUid = p.loadURDF(os.path.join(urdfRootPath, "random_urdfs/000/000.urdf"), basePosition=state_object)
 
         state_robot = p.getLinkState(self.pandaUid, 11)[0]
         state_fingers = (p.getJointState(self.pandaUid,9)[0], p.getJointState(self.pandaUid, 10)[0])
 
-        observation = state_robot + state_fingers
+        self.observation = state_robot + state_fingers
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,1) # rendering's back on again
         return np.array(self.observation).astype(np.float32)
 
     def render(self, mode='human'):
         view_matrix = p.computeViewMatrixFromYawPitchRoll(cameraTargetPosition=[0.7,0,0.05],
                                                             distance=.7,
                                                             yaw=90,
```

