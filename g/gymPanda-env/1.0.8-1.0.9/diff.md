# Comparing `tmp/gymPanda_env-1.0.8-py3-none-any.whl.zip` & `tmp/gymPanda_env-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3403 bytes, number of entries: 7
+Zip file size: 3386 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      128 b- defN 23-Jun-07 18:48 gym_panda_env/__init__.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 18:46 gym_panda_env/envs/__init__.py
--rw-rw-r--  2.0 unx     4827 b- defN 23-Jun-07 19:27 gym_panda_env/envs/panda_env.py
--rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:27 gymPanda_env-1.0.8.dist-info/RECORD
-7 files, 5922 bytes uncompressed, 2381 bytes compressed:  59.8%
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-07 19:32 gym_panda_env/envs/panda_env.py
+-rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:32 gymPanda_env-1.0.9.dist-info/RECORD
+7 files, 5878 bytes uncompressed, 2364 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gym_panda_env/envs/__init__.py
 Comment: 
 
 Filename: gym_panda_env/envs/panda_env.py
 Comment: 
 
-Filename: gymPanda_env-1.0.8.dist-info/METADATA
+Filename: gymPanda_env-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: gymPanda_env-1.0.8.dist-info/WHEEL
+Filename: gymPanda_env-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: gymPanda_env-1.0.8.dist-info/top_level.txt
+Filename: gymPanda_env-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: gymPanda_env-1.0.8.dist-info/RECORD
+Filename: gymPanda_env-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_panda_env/envs/panda_env.py

```diff
@@ -44,16 +44,14 @@
         if state_object[2]>0.45:
             reward = 1
             done = True
         else:
             reward = 0
             done = False
 
-        self.step_counter += 1
-            
         info = {'object_position': state_object}
         observation = state_robot + state_fingers
 
         return observation, reward, done, info
 
     def reset(self):
         p.resetSimulation()
```

