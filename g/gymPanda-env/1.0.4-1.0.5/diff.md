# Comparing `tmp/gymPanda_env-1.0.4-py3-none-any.whl.zip` & `tmp/gymPanda_env-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3335 bytes, number of entries: 7
+Zip file size: 3361 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      128 b- defN 23-Jun-07 18:48 gym_panda_env/__init__.py
 -rw-rw-r--  2.0 unx       52 b- defN 23-Jun-07 18:46 gym_panda_env/envs/__init__.py
--rw-rw-r--  2.0 unx     4692 b- defN 23-Jun-07 18:36 gym_panda_env/envs/panda_env.py
--rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:00 gymPanda_env-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:00 gymPanda_env-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:00 gymPanda_env-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:00 gymPanda_env-1.0.4.dist-info/RECORD
-7 files, 5787 bytes uncompressed, 2313 bytes compressed:  60.0%
+-rw-rw-r--  2.0 unx     4720 b- defN 23-Jun-07 19:20 gym_panda_env/envs/panda_env.py
+-rw-rw-r--  2.0 unx      238 b- defN 23-Jun-07 19:20 gymPanda_env-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 19:20 gymPanda_env-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-07 19:20 gymPanda_env-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      571 b- defN 23-Jun-07 19:20 gymPanda_env-1.0.5.dist-info/RECORD
+7 files, 5815 bytes uncompressed, 2339 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: gym_panda_env/envs/__init__.py
 Comment: 
 
 Filename: gym_panda_env/envs/panda_env.py
 Comment: 
 
-Filename: gymPanda_env-1.0.4.dist-info/METADATA
+Filename: gymPanda_env-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: gymPanda_env-1.0.4.dist-info/WHEEL
+Filename: gymPanda_env-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: gymPanda_env-1.0.4.dist-info/top_level.txt
+Filename: gymPanda_env-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gymPanda_env-1.0.4.dist-info/RECORD
+Filename: gymPanda_env-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_panda_env/envs/panda_env.py

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import random
 
 class PandaGymEnv(gym.Env):
     metadata = {'render.modes': ['human']}
 
     def __init__(self):
-        p.connect(p.GUI) #Connects to GUI
+        p.connect(p.GUI, options="--opengl2") #Connects to GUI
         p.resetDebugVisualizerCamera(cameraDistance=1.5, cameraYaw=0, cameraPitch=-40, cameraTargetPosition=[0.55,-0.35,0.2]) # Set convinient camera pose
         self.action_space = spaces.Box(np.array([-1]*4), np.array([1]*4)) # Define continuous action space without fingers orientation here
         self.observation_space = spaces.Box(np.array([-1]*5), np.array([1]*5)) # Define observation space 
 
     def step(self, action):
         p.configureDebugVisualizer(p.COV_ENABLE_SINGLE_STEP_RENDERING) #Smooth display
         orientation = p.getQuaternionFromEuler([0.,-math.pi,math.pi/2.])
@@ -28,15 +28,15 @@
         fingers = action[3]
 
         currentPose = p.getLinkState(self.pandaUid, 11)
         currentPosition = currentPose[0]
         newPosition = [currentPosition[0] + dx,
                        currentPosition[1] + dy,
                        currentPosition[2] + dz]
-        jointPoses = p.calculateInverseKinematics(self.pandaUid,11,newPosition, orientation)
+        jointPoses = p.calculateInverseKinematics(self.pandaUid,11,newPosition, orientation)[0:7]
         p.setJointMotorControlArray(self.pandaUid, list(range(7))+[9,10], p.POSITION_CONTROL, list(jointPoses)+2*[fingers])
 
         p.stepSimulation()
 
         state_object, _ = p.getBasePositionAndOrientation(self.objectUid)
         state_robot = p.getLinkState(self.pandaUid, 11)[0]
         state_fingers = (p.getJointState(self.pandaUid,9)[0], p.getJointState(self.pandaUid, 10)[0])
@@ -55,17 +55,18 @@
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,0) # we will enable rendering after we loaded everything
         p.setGravity(0,0,-10)
         urdfRootPath=pybullet_data.getDataPath()
 
         tableUid = p.loadURDF(os.path.join(urdfRootPath, "table/table.urdf"),basePosition=[0.5,0,-0.65])
         trayUid = p.loadURDF(os.path.join(urdfRootPath, "tray/traybox.urdf"),basePosition=[0.65,0,0])
         planeUid = p.loadURDF(os.path.join(urdfRootPath,"plane.urdf"), basePosition=[0,0,-0.65])
+        self.pandaUid = p.loadURDF(os.path.join(urdfRootPath, "franka_panda/panda.urdf"),useFixedBase=True)
+
 
         rest_poses = [0,-0.215,0,-2.57,0,2.356,2.356,0.08,0.08]
-        self.pandaUid = p.loadURDF(os.path.join(urdfRootPath, "franka_panda/panda.urdf"),useFixedBase=True)
         for i in range(7):
             p.resetJointState(self.pandaUid,i, rest_poses[i])
 
         state_object= [random.uniform(0.5,0.8),random.uniform(-0.2,0.2),0.05]
         self.objectUid = p.loadURDF(os.path.join(urdfRootPath, "random_urdfs/000/000.urdf"), basePosition=state_object)
 
         state_robot = p.getLinkState(self.pandaUid, 11)[0]
@@ -96,8 +97,8 @@
         rgb_array = np.reshape(rgb_array, (720,960, 4))
 
         rgb_array = rgb_array[:, :, :3]
         return rgb_array
 
 
     def close(self):
-        p.disconnect()
+        p.disconnect()
```

