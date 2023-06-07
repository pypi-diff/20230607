# Comparing `tmp/diambra-arena-2.1.0rc7.tar.gz` & `tmp/diambra-arena-2.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.1.0rc7.tar", last modified: Sun May 21 23:56:49 2023, max compression
+gzip compressed data, was "diambra-arena-2.1.0rc8.tar", last modified: Wed Jun  7 20:04:33 2023, max compression
```

## Comparing `diambra-arena-2.1.0rc7.tar` & `diambra-arena-2.1.0rc8.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.480239 diambra-arena-2.1.0rc7/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.484238 diambra-arena-2.1.0rc7/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/arena_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/arena_imitation_learning_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.484238 diambra-arena-2.1.0rc7/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.484238 diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.488238 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.492239 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/p2_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.492239 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.496239 diambra-arena-2.1.0rc7/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    55998 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/.splashScreen.gif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.500239 diambra-arena-2.1.0rc7/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper_hardcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-21 23:56:26.000000 diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.504239 diambra-arena-2.1.0rc7/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 23:56:49.000000 diambra-arena-2.1.0rc7/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:49.508239 diambra-arena-2.1.0rc7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_gym_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_imitation_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6112 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-21 23:56:27.000000 diambra-arena-2.1.0rc7/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.914884 diambra-arena-2.1.0rc8/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/arena_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/arena_imitation_learning_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/p2_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.918884 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.922884 diambra-arena-2.1.0rc8/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/.splash_screen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/engine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.922884 diambra-arena-2.1.0rc8/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper_hardcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 20:04:33.000000 diambra-arena-2.1.0rc8/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:04:33.926884 diambra-arena-2.1.0rc8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_gym_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_imitation_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-07 20:04:17.000000 diambra-arena-2.1.0rc8/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.1.0rc7/LICENSE.txt` & `diambra-arena-2.1.0rc8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/PKG-INFO` & `diambra-arena-2.1.0rc8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc7
+Version: 2.1.0rc8
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -19,32 +19,44 @@
 Provides-Extra: core
 Provides-Extra: tests
 Provides-Extra: stable-baselines
 Provides-Extra: stable-baselines3
 Provides-Extra: ray-rllib
 License-File: LICENSE.txt
 
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.png" alt="diambra" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.jpg" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
 </p>
 <p align="center">
   <a href="https://www.linkedin.com/company/diambra">Linkedin</a> •
   <a href="https://diambra.ai/discord">Discord</a> •
   <a href="https://www.twitch.tv/diambra_ai">Twitch</a> •
   <a href="https://www.youtube.com/c/diambra_ai">YouTube</a> •
   <a href="https://twitter.com/diambra_ai">Twitter</a>
 </p>
 
 <p align="center">
-<a href="https://arxiv.org/abs/2210.10595"><img src="http://img.shields.io/badge/paper-arxiv.2210.10595-B31B1B.svg" alt="Paper"/></a>
+<a href="https://arxiv.org/abs/2210.10595"><img src="https://img.shields.io/badge/paper-arXiv:2210.10595-B31B1B?logo=arxiv" alt="Paper"/></a>
+</p>
+<p align="center">
+<a href="https://github.com/diambra/arena/actions/workflows/test.yaml"><img src="https://img.shields.io/github/actions/workflow/status/diambra/arena/test.yaml?label=arena%20tests&logo=github" alt="Arena Test"/></a>
+<a href="https://github.com/diambra/arena/actions/workflows/test_agents.yaml"><img src="https://img.shields.io/github/actions/workflow/status/diambra/arena/test_agents.yaml?label=agents%20tests&logo=github" alt="Agents Test"/></a>
+<a href="https://github.com/diambra/arena/tags"><img src="https://img.shields.io/github/v/tag/diambra/arena?label=latest%20tag&logo=github" alt="Latest Tag"/></a>
+<a href="https://pypi.org/project/diambra-arena/"><img src="https://img.shields.io/pypi/v/diambra-arena?logo=pypi" alt="Pypi version"/></a>
+</p>
+<p align="center">
+<a href="https://docs.diambra.ai/#installation"><img src="https://img.shields.io/badge/supported%20os-linux%20%7C%20win%20%7C%20macOS-blue?logo=docker" alt="Supported OS"/></a>
+<a href="https://docs.diambra.ai/"><img src="https://img.shields.io/github/last-commit/diambra/docs/main?label=docs%20last%20update&logo=readthedocs" alt="Last Docs Update"/></a>
 </p>
 
+
+
 # DIAMBRA Arena
 
 ## Index
 
 - **[Overview](#overview)**
 - **[Competition Platform](#competition-platform)**
 - **[Installation](#installation)**
@@ -85,23 +97,21 @@
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
 **Many more are coming soon...**
 
 ## Competition Platform
 
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/leaderboard.jpg" alt="DIAMBRA Leaderboard" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/.github/master/img/platform.jpg" alt="DIAMBRA Competition Platform" width="100%"/>
 
 Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
 
-It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments. 
+It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments.
 
-It also offers you the possibility to unlock cool achievements depending on the performances of your agent. 
-
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/achievements.jpg" alt="DIAMBRA Achievements" width="100%"/>
+It also offers you the possibility to unlock cool achievements depending on the performances of your agent.
 
 Submitted agents are evaluated and their episodes are streamed on our Twitch channel.
 
 We aimed at making the submission process as smooth as possible, **<a href="https://diambra.ai/register/" target="_blank">join us and try it now!</a>**
 
 ## Installation
 
@@ -121,50 +131,48 @@
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
 
 #### Download Game ROM(s) and Check Validity
 
-Check available games with the following command:
+Check out available games:
 
 ```
 diambra arena list-roms
 ```
 
-Output example:
+Output extract:
 
 ```shell
 [...]
  Title: Dead Or Alive ++ - GameId: doapp
    Difficulty levels: Min 1 - Max 4
    SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
    Original ROM name: doapp.zip
    Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-japan', '80781', 'wowroms']
    Characters list: ['Kasumi', 'Zack', 'Hayabusa', 'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-Lee', 'Ayane']
 [...]
 ```
 
 Search ROMs on the web using **Search Keywords** provided by the game list command reported above. **Pay attention, follow game-specific notes reported there, and store all ROMs in the same folder, whose absolute path will be referred in the following as** `your/roms/local/path`.
 
-**Specific game ROM files are required, check validity of the downloaded ROMs as follows.**
-
-Check ROM(s) validity running:
+**Specific game ROM files are required, check validity of the downloaded ROMs:**
 
 ```
 diambra arena check-roms your/roms/local/path/romFileName.zip
 ```
 
-The output for a valid ROM file would look like the following:
+The output for a valid ROM file would look like:
 
 ```
 Correct ROM file for Dead Or Alive ++, sha256 = d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
 ```
 
-**Make sure to check out our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>, and in particular Section 7. By using the software, you accept the in full.</span>**
+**Make sure to check out our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>, and in particular Section 7. By using the software, you accept them in full.</span>**
 
 #### Base script
 
 Running a complete episode with a random agent requires less than 20 python lines:
 
 ```python {linenos=inline}
  import diambra.arena
@@ -207,17 +215,17 @@
 
 These examples show how to leverage both single and two players modes, how to set up environment wrappers specifying all their options, how to record human expert demonstrations and how to load them to apply imitation learning. They can be used as templates and starting points to explore all the features of the software package.
 
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.gif" alt="diambraGif" width="100%"/>
 
 ## Reinforcement Learning Libs Compatibility
 
-DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents repository</a>. It can easily be interfaced with any other package in a similar way.
+DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines 3 and Ray RLlib, while Stable Baselines is also available but deprecated. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents</a>  repository. It can easily be interfaced with any other package in a similar way.
 
-Native interfaces, that can be installed with the dedicated options listed below, have been tested with the following versions:
+Native interfaces, installed with the specific options listed below, are tested with the following versions:
 
 - Stable Baselines 3 | `pip install diambra-arena[stable-baselines3]` (<a href="https://stable-baselines3.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/DLR-RM/stable-baselines3" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines3/" target="_blank">Pypi</a>): 1.6.1
 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (<a href="https://docs.ray.io/en/latest/index.html" target="_blank">Docs</a> - <a href="https://github.com/ray-project/ray" target="_blank">GitHub</a> - <a href="https://pypi.org/project/ray/" target="_blank">Pypi</a>): 2.0.0
 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (<a href="https://stable-baselines.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/hill-a/stable-baselines" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines/" target="_blank">Pypi</a>): 2.10.2
 
 ## References
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc7 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc8 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -10,14 +10,16 @@
 Entertainment Classifier: Topic :: Games/Entertainment :: Arcade Classifier:
 Topic :: Education Description-Content-Type: text/markdown Provides-Extra: core
 Provides-Extra: tests Provides-Extra: stable-baselines Provides-Extra: stable-
 baselines3 Provides-Extra: ray-rllib License-File: LICENSE.txt [diambra]
                            Documentation â¢ Website
             Linkedin â¢ Discord â¢ Twitch â¢ YouTube â¢ Twitter
                                     [Paper]
+            [Arena_Test] [Agents_Test] [Latest_Tag] [Pypi_version]
+                       [Supported_OS] [Last_Docs_Update]
 # DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
 (#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
 Examples](#quickstart--examples)** - **[Reinforcement Learning Libs
 Compatibility](#reinforcement-learning-libs-compatibility)** - **[References]
 (#references)** - **[Support, Feature Requests & Bugs Reports](#support-
 feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
 Use](#terms-of-use)** ## Overview DIAMBRA Arena is a software package featuring
@@ -75,52 +77,51 @@
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
 Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
-Leaderboard] Our competition platform allows you to submit your agents and
-compete with other coders around the globe in epic video games tournaments! It
-features a public global leaderboard where users are ranked by the best score
-achieved by their agents in our different environments. It also offers you the
-possibility to unlock cool achievements depending on the performances of your
-agent. [DIAMBRA Achievements] Submitted agents are evaluated and their episodes
-are streamed on our Twitch channel. We aimed at making the submission process
-as smooth as possible, **join_us_and_try_it_now!** ## Installation - Create_an
-account_on_our_website, it requires just a few clicks and is 100% free -
-Install Docker Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line
-Interface: `python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -
-m pip install diambra-arena` **Using a virtual environment to isolate your
-python packages installation is strongly suggested** ## Quickstart & Examples
-DIAMBRA Arena usage follows the standard RL interaction framework: the agent
-sends an action to the environment, which process it and performs a transition
+Competition Platform] Our competition platform allows you to submit your agents
+and compete with other coders around the globe in epic video games tournaments!
+It features a public global leaderboard where users are ranked by the best
+score achieved by their agents in our different environments. It also offers
+you the possibility to unlock cool achievements depending on the performances
+of your agent. Submitted agents are evaluated and their episodes are streamed
+on our Twitch channel. We aimed at making the submission process as smooth as
+possible, **join_us_and_try_it_now!** ## Installation - Create_an_account_on
+our_website, it requires just a few clicks and is 100% free - Install Docker
+Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line Interface:
+`python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -m pip
+install diambra-arena` **Using a virtual environment to isolate your python
+packages installation is strongly suggested** ## Quickstart & Examples DIAMBRA
+Arena usage follows the standard RL interaction framework: the agent sends an
+action to the environment, which process it and performs a transition
 accordingly, from the starting state to the new state, returning the
 observation and the reward to the agent to close the interaction loop. The
 figure below shows this typical interaction scheme and data flow.
                                   [rlScheme]
-#### Download Game ROM(s) and Check Validity Check available games with the
-following command: ``` diambra arena list-roms ``` Output example: ```shell
-[...] Title: Dead Or Alive ++ - GameId: doapp Difficulty levels: Min 1 - Max 4
-SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
-Original ROM name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]',
-'dead-or-alive-japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack',
-'Hayabusa', 'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-
-Lee', 'Ayane'] [...] ``` Search ROMs on the web using **Search Keywords**
-provided by the game list command reported above. **Pay attention, follow game-
-specific notes reported there, and store all ROMs in the same folder, whose
-absolute path will be referred in the following as** `your/roms/local/path`.
-**Specific game ROM files are required, check validity of the downloaded ROMs
-as follows.** Check ROM(s) validity running: ``` diambra arena check-roms your/
-roms/local/path/romFileName.zip ``` The output for a valid ROM file would look
-like the following: ``` Correct ROM file for Dead Or Alive ++, sha256 =
+#### Download Game ROM(s) and Check Validity Check out available games: ```
+diambra arena list-roms ``` Output extract: ```shell [...] Title: Dead Or Alive
+++ - GameId: doapp Difficulty levels: Min 1 - Max 4 SHA256 sum:
+d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e Original ROM
+name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-
+japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack', 'Hayabusa',
+'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-Lee', 'Ayane']
+[...] ``` Search ROMs on the web using **Search Keywords** provided by the game
+list command reported above. **Pay attention, follow game-specific notes
+reported there, and store all ROMs in the same folder, whose absolute path will
+be referred in the following as** `your/roms/local/path`. **Specific game ROM
+files are required, check validity of the downloaded ROMs:** ``` diambra arena
+check-roms your/roms/local/path/romFileName.zip ``` The output for a valid ROM
+file would look like: ``` Correct ROM file for Dead Or Alive ++, sha256 =
 d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e ``` **Make
 sure to check out our Terms_of_Use, and in particular Section 7. By using the
-software, you accept the in full.** #### Base script Running a complete episode
-with a random agent requires less than 20 python lines: ```python
+software, you accept them in full.** #### Base script Running a complete
+episode with a random agent requires less than 20 python lines: ```python
 {linenos=inline} import diambra.arena env = diambra.arena.make("doapp")
 observation = env.reset() while True: env.render() actions =
 env.action_space.sample() observation, reward, done, info = env.step(actions)
 if done: observation = env.reset() break env.close() ``` To execute the script
 run: ``` diambra run -r your/roms/local/path python script.py ``` Additional
 details and use cases are provided in the Getting_Started section of the
 documentation. ### Examples The `examples/` folder contains ready to use
@@ -130,31 +131,31 @@
 both single and two players modes, how to set up environment wrappers
 specifying all their options, how to record human expert demonstrations and how
 to load them to apply imitation learning. They can be used as templates and
 starting points to explore all the features of the software package.
 [diambraGif] ## Reinforcement Learning Libs Compatibility DIAMBRA Arena is
 built to maximize compatibility will all major Reinforcement Learning
 libraries. It natively provides interfaces with the two most import packages:
-Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is
-illustrated in detail in the documentation and in the DIAMBRA_Agents
-repository. It can easily be interfaced with any other package in a similar
-way. Native interfaces, that can be installed with the dedicated options listed
-below, have been tested with the following versions: - Stable Baselines 3 |
-`pip install diambra-arena[stable-baselines3]` (Docs - GitHub - Pypi): 1.6.1 -
-Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs - GitHub - Pypi):
-2.0.0 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (Docs
-- GitHub - Pypi): 2.10.2 ## References - Documentation: https://docs.diambra.ai
-- Paper: https://arxiv.org/abs/2210.10595 - Website: https://diambra.ai -
-Discord: https://diambra.ai/discord - Linkedin: https://www.linkedin.com/
-company/diambra - Twitch: https://www.twitch.tv/diambra_ai - YouTube: https://
-www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/diambra_ai ##
-Support, Feature Requests & Bugs Reports To receive support, use the dedicated
-channel in our Discord_Server. To request features or report bugs, use the
-GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595
-```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
-Arena: a New Reinforcement Learning Platform for Research and
+Stable Baselines 3 and Ray RLlib, while Stable Baselines is also available but
+deprecated. Their usage is illustrated in detail in the documentation and in
+the DIAMBRA_Agents repository. It can easily be interfaced with any other
+package in a similar way. Native interfaces, installed with the specific
+options listed below, are tested with the following versions: - Stable
+Baselines 3 | `pip install diambra-arena[stable-baselines3]` (Docs - GitHub -
+Pypi): 1.6.1 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs -
+GitHub - Pypi): 2.0.0 - Stable Baselines | `pip install diambra-arena[stable-
+baselines]` (Docs - GitHub - Pypi): 2.10.2 ## References - Documentation:
+https://docs.diambra.ai - Paper: https://arxiv.org/abs/2210.10595 - Website:
+https://diambra.ai - Discord: https://diambra.ai/discord - Linkedin: https://
+www.linkedin.com/company/diambra - Twitch: https://www.twitch.tv/diambra_ai -
+YouTube: https://www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/
+diambra_ai ## Support, Feature Requests & Bugs Reports To receive support, use
+the dedicated channel in our Discord_Server. To request features or report
+bugs, use the GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/
+2210.10595 ```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title =
+"{DIAMBRA Arena: a New Reinforcement Learning Platform for Research and
 Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
 learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
 = {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
 eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
 Arena software package is subject to our Terms_of_Use. By using it, you accept
 them in full. ###### DIAMBRA, Inc. Â© Copyright 2018-2023. All Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc7/README.md` & `diambra-arena-2.1.0rc8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.png" alt="diambra" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.jpg" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
 </p>
 <p align="center">
   <a href="https://www.linkedin.com/company/diambra">Linkedin</a> •
   <a href="https://diambra.ai/discord">Discord</a> •
   <a href="https://www.twitch.tv/diambra_ai">Twitch</a> •
   <a href="https://www.youtube.com/c/diambra_ai">YouTube</a> •
   <a href="https://twitter.com/diambra_ai">Twitter</a>
 </p>
 
 <p align="center">
-<a href="https://arxiv.org/abs/2210.10595"><img src="http://img.shields.io/badge/paper-arxiv.2210.10595-B31B1B.svg" alt="Paper"/></a>
+<a href="https://arxiv.org/abs/2210.10595"><img src="https://img.shields.io/badge/paper-arXiv:2210.10595-B31B1B?logo=arxiv" alt="Paper"/></a>
+</p>
+<p align="center">
+<a href="https://github.com/diambra/arena/actions/workflows/test.yaml"><img src="https://img.shields.io/github/actions/workflow/status/diambra/arena/test.yaml?label=arena%20tests&logo=github" alt="Arena Test"/></a>
+<a href="https://github.com/diambra/arena/actions/workflows/test_agents.yaml"><img src="https://img.shields.io/github/actions/workflow/status/diambra/arena/test_agents.yaml?label=agents%20tests&logo=github" alt="Agents Test"/></a>
+<a href="https://github.com/diambra/arena/tags"><img src="https://img.shields.io/github/v/tag/diambra/arena?label=latest%20tag&logo=github" alt="Latest Tag"/></a>
+<a href="https://pypi.org/project/diambra-arena/"><img src="https://img.shields.io/pypi/v/diambra-arena?logo=pypi" alt="Pypi version"/></a>
+</p>
+<p align="center">
+<a href="https://docs.diambra.ai/#installation"><img src="https://img.shields.io/badge/supported%20os-linux%20%7C%20win%20%7C%20macOS-blue?logo=docker" alt="Supported OS"/></a>
+<a href="https://docs.diambra.ai/"><img src="https://img.shields.io/github/last-commit/diambra/docs/main?label=docs%20last%20update&logo=readthedocs" alt="Last Docs Update"/></a>
 </p>
 
+
+
 # DIAMBRA Arena
 
 ## Index
 
 - **[Overview](#overview)**
 - **[Competition Platform](#competition-platform)**
 - **[Installation](#installation)**
@@ -60,23 +72,21 @@
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
 **Many more are coming soon...**
 
 ## Competition Platform
 
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/leaderboard.jpg" alt="DIAMBRA Leaderboard" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/.github/master/img/platform.jpg" alt="DIAMBRA Competition Platform" width="100%"/>
 
 Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
 
-It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments. 
+It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments.
 
-It also offers you the possibility to unlock cool achievements depending on the performances of your agent. 
-
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/achievements.jpg" alt="DIAMBRA Achievements" width="100%"/>
+It also offers you the possibility to unlock cool achievements depending on the performances of your agent.
 
 Submitted agents are evaluated and their episodes are streamed on our Twitch channel.
 
 We aimed at making the submission process as smooth as possible, **<a href="https://diambra.ai/register/" target="_blank">join us and try it now!</a>**
 
 ## Installation
 
@@ -96,50 +106,48 @@
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
 
 #### Download Game ROM(s) and Check Validity
 
-Check available games with the following command:
+Check out available games:
 
 ```
 diambra arena list-roms
 ```
 
-Output example:
+Output extract:
 
 ```shell
 [...]
  Title: Dead Or Alive ++ - GameId: doapp
    Difficulty levels: Min 1 - Max 4
    SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
    Original ROM name: doapp.zip
    Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-japan', '80781', 'wowroms']
    Characters list: ['Kasumi', 'Zack', 'Hayabusa', 'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-Lee', 'Ayane']
 [...]
 ```
 
 Search ROMs on the web using **Search Keywords** provided by the game list command reported above. **Pay attention, follow game-specific notes reported there, and store all ROMs in the same folder, whose absolute path will be referred in the following as** `your/roms/local/path`.
 
-**Specific game ROM files are required, check validity of the downloaded ROMs as follows.**
-
-Check ROM(s) validity running:
+**Specific game ROM files are required, check validity of the downloaded ROMs:**
 
 ```
 diambra arena check-roms your/roms/local/path/romFileName.zip
 ```
 
-The output for a valid ROM file would look like the following:
+The output for a valid ROM file would look like:
 
 ```
 Correct ROM file for Dead Or Alive ++, sha256 = d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
 ```
 
-**Make sure to check out our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>, and in particular Section 7. By using the software, you accept the in full.</span>**
+**Make sure to check out our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>, and in particular Section 7. By using the software, you accept them in full.</span>**
 
 #### Base script
 
 Running a complete episode with a random agent requires less than 20 python lines:
 
 ```python {linenos=inline}
  import diambra.arena
@@ -182,17 +190,17 @@
 
 These examples show how to leverage both single and two players modes, how to set up environment wrappers specifying all their options, how to record human expert demonstrations and how to load them to apply imitation learning. They can be used as templates and starting points to explore all the features of the software package.
 
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.gif" alt="diambraGif" width="100%"/>
 
 ## Reinforcement Learning Libs Compatibility
 
-DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents repository</a>. It can easily be interfaced with any other package in a similar way.
+DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines 3 and Ray RLlib, while Stable Baselines is also available but deprecated. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents</a>  repository. It can easily be interfaced with any other package in a similar way.
 
-Native interfaces, that can be installed with the dedicated options listed below, have been tested with the following versions:
+Native interfaces, installed with the specific options listed below, are tested with the following versions:
 
 - Stable Baselines 3 | `pip install diambra-arena[stable-baselines3]` (<a href="https://stable-baselines3.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/DLR-RM/stable-baselines3" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines3/" target="_blank">Pypi</a>): 1.6.1
 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (<a href="https://docs.ray.io/en/latest/index.html" target="_blank">Docs</a> - <a href="https://github.com/ray-project/ray" target="_blank">GitHub</a> - <a href="https://pypi.org/project/ray/" target="_blank">Pypi</a>): 2.0.0
 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (<a href="https://stable-baselines.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/hill-a/stable-baselines" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines/" target="_blank">Pypi</a>): 2.10.2
 
 ## References
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 [diambra]
                            Documentation â¢ Website
             Linkedin â¢ Discord â¢ Twitch â¢ YouTube â¢ Twitter
                                     [Paper]
+            [Arena_Test] [Agents_Test] [Latest_Tag] [Pypi_version]
+                       [Supported_OS] [Last_Docs_Update]
 # DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
 (#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
 Examples](#quickstart--examples)** - **[Reinforcement Learning Libs
 Compatibility](#reinforcement-learning-libs-compatibility)** - **[References]
 (#references)** - **[Support, Feature Requests & Bugs Reports](#support-
 feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
 Use](#terms-of-use)** ## Overview DIAMBRA Arena is a software package featuring
@@ -63,52 +65,51 @@
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
 Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
-Leaderboard] Our competition platform allows you to submit your agents and
-compete with other coders around the globe in epic video games tournaments! It
-features a public global leaderboard where users are ranked by the best score
-achieved by their agents in our different environments. It also offers you the
-possibility to unlock cool achievements depending on the performances of your
-agent. [DIAMBRA Achievements] Submitted agents are evaluated and their episodes
-are streamed on our Twitch channel. We aimed at making the submission process
-as smooth as possible, **join_us_and_try_it_now!** ## Installation - Create_an
-account_on_our_website, it requires just a few clicks and is 100% free -
-Install Docker Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line
-Interface: `python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -
-m pip install diambra-arena` **Using a virtual environment to isolate your
-python packages installation is strongly suggested** ## Quickstart & Examples
-DIAMBRA Arena usage follows the standard RL interaction framework: the agent
-sends an action to the environment, which process it and performs a transition
+Competition Platform] Our competition platform allows you to submit your agents
+and compete with other coders around the globe in epic video games tournaments!
+It features a public global leaderboard where users are ranked by the best
+score achieved by their agents in our different environments. It also offers
+you the possibility to unlock cool achievements depending on the performances
+of your agent. Submitted agents are evaluated and their episodes are streamed
+on our Twitch channel. We aimed at making the submission process as smooth as
+possible, **join_us_and_try_it_now!** ## Installation - Create_an_account_on
+our_website, it requires just a few clicks and is 100% free - Install Docker
+Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line Interface:
+`python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -m pip
+install diambra-arena` **Using a virtual environment to isolate your python
+packages installation is strongly suggested** ## Quickstart & Examples DIAMBRA
+Arena usage follows the standard RL interaction framework: the agent sends an
+action to the environment, which process it and performs a transition
 accordingly, from the starting state to the new state, returning the
 observation and the reward to the agent to close the interaction loop. The
 figure below shows this typical interaction scheme and data flow.
                                   [rlScheme]
-#### Download Game ROM(s) and Check Validity Check available games with the
-following command: ``` diambra arena list-roms ``` Output example: ```shell
-[...] Title: Dead Or Alive ++ - GameId: doapp Difficulty levels: Min 1 - Max 4
-SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
-Original ROM name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]',
-'dead-or-alive-japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack',
-'Hayabusa', 'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-
-Lee', 'Ayane'] [...] ``` Search ROMs on the web using **Search Keywords**
-provided by the game list command reported above. **Pay attention, follow game-
-specific notes reported there, and store all ROMs in the same folder, whose
-absolute path will be referred in the following as** `your/roms/local/path`.
-**Specific game ROM files are required, check validity of the downloaded ROMs
-as follows.** Check ROM(s) validity running: ``` diambra arena check-roms your/
-roms/local/path/romFileName.zip ``` The output for a valid ROM file would look
-like the following: ``` Correct ROM file for Dead Or Alive ++, sha256 =
+#### Download Game ROM(s) and Check Validity Check out available games: ```
+diambra arena list-roms ``` Output extract: ```shell [...] Title: Dead Or Alive
+++ - GameId: doapp Difficulty levels: Min 1 - Max 4 SHA256 sum:
+d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e Original ROM
+name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-
+japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack', 'Hayabusa',
+'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-Lee', 'Ayane']
+[...] ``` Search ROMs on the web using **Search Keywords** provided by the game
+list command reported above. **Pay attention, follow game-specific notes
+reported there, and store all ROMs in the same folder, whose absolute path will
+be referred in the following as** `your/roms/local/path`. **Specific game ROM
+files are required, check validity of the downloaded ROMs:** ``` diambra arena
+check-roms your/roms/local/path/romFileName.zip ``` The output for a valid ROM
+file would look like: ``` Correct ROM file for Dead Or Alive ++, sha256 =
 d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e ``` **Make
 sure to check out our Terms_of_Use, and in particular Section 7. By using the
-software, you accept the in full.** #### Base script Running a complete episode
-with a random agent requires less than 20 python lines: ```python
+software, you accept them in full.** #### Base script Running a complete
+episode with a random agent requires less than 20 python lines: ```python
 {linenos=inline} import diambra.arena env = diambra.arena.make("doapp")
 observation = env.reset() while True: env.render() actions =
 env.action_space.sample() observation, reward, done, info = env.step(actions)
 if done: observation = env.reset() break env.close() ``` To execute the script
 run: ``` diambra run -r your/roms/local/path python script.py ``` Additional
 details and use cases are provided in the Getting_Started section of the
 documentation. ### Examples The `examples/` folder contains ready to use
@@ -118,31 +119,31 @@
 both single and two players modes, how to set up environment wrappers
 specifying all their options, how to record human expert demonstrations and how
 to load them to apply imitation learning. They can be used as templates and
 starting points to explore all the features of the software package.
 [diambraGif] ## Reinforcement Learning Libs Compatibility DIAMBRA Arena is
 built to maximize compatibility will all major Reinforcement Learning
 libraries. It natively provides interfaces with the two most import packages:
-Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is
-illustrated in detail in the documentation and in the DIAMBRA_Agents
-repository. It can easily be interfaced with any other package in a similar
-way. Native interfaces, that can be installed with the dedicated options listed
-below, have been tested with the following versions: - Stable Baselines 3 |
-`pip install diambra-arena[stable-baselines3]` (Docs - GitHub - Pypi): 1.6.1 -
-Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs - GitHub - Pypi):
-2.0.0 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (Docs
-- GitHub - Pypi): 2.10.2 ## References - Documentation: https://docs.diambra.ai
-- Paper: https://arxiv.org/abs/2210.10595 - Website: https://diambra.ai -
-Discord: https://diambra.ai/discord - Linkedin: https://www.linkedin.com/
-company/diambra - Twitch: https://www.twitch.tv/diambra_ai - YouTube: https://
-www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/diambra_ai ##
-Support, Feature Requests & Bugs Reports To receive support, use the dedicated
-channel in our Discord_Server. To request features or report bugs, use the
-GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595
-```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
-Arena: a New Reinforcement Learning Platform for Research and
+Stable Baselines 3 and Ray RLlib, while Stable Baselines is also available but
+deprecated. Their usage is illustrated in detail in the documentation and in
+the DIAMBRA_Agents repository. It can easily be interfaced with any other
+package in a similar way. Native interfaces, installed with the specific
+options listed below, are tested with the following versions: - Stable
+Baselines 3 | `pip install diambra-arena[stable-baselines3]` (Docs - GitHub -
+Pypi): 1.6.1 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs -
+GitHub - Pypi): 2.0.0 - Stable Baselines | `pip install diambra-arena[stable-
+baselines]` (Docs - GitHub - Pypi): 2.10.2 ## References - Documentation:
+https://docs.diambra.ai - Paper: https://arxiv.org/abs/2210.10595 - Website:
+https://diambra.ai - Discord: https://diambra.ai/discord - Linkedin: https://
+www.linkedin.com/company/diambra - Twitch: https://www.twitch.tv/diambra_ai -
+YouTube: https://www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/
+diambra_ai ## Support, Feature Requests & Bugs Reports To receive support, use
+the dedicated channel in our Discord_Server. To request features or report
+bugs, use the GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/
+2210.10595 ```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title =
+"{DIAMBRA Arena: a New Reinforcement Learning Platform for Research and
 Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
 learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
 = {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
 eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
 Arena software package is subject to our Terms_of_Use. By using it, you accept
 them in full. ###### DIAMBRA, Inc. Â© Copyright 2018-2023. All Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/arena_gym.py` & `diambra-arena-2.1.0rc8/diambra/arena/arena_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/arena_imitation_learning_gym.py` & `diambra-arena-2.1.0rc8/diambra/arena/arena_imitation_learning_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/engine/interface.py` & `diambra-arena-2.1.0rc8/diambra/arena/engine/interface.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/env_settings.py` & `diambra-arena-2.1.0rc8/diambra/arena/env_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/make_env.py` & `diambra-arena-2.1.0rc8/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/ray_rllib/make_ray_env.py` & `diambra-arena-2.1.0rc8/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 import diambra.arena
 import logging
 import gym
 from ray.rllib.env.env_context import EnvContext
 from copy import deepcopy
 import pickle
 
@@ -18,18 +17,18 @@
         self.load_spaces_from_file = False
 
         if "load_spaces_from_file" in config.keys() and config["load_spaces_from_file"] is True:
             if "env_spaces_file_name" not in config.keys():
                 raise Exception("Loading environment spaces from file selected, but no file specified.")
             else:
                 self.env_spaces_file_name = config["env_spaces_file_name"]
-                
+
                 if not os.path.isfile(self.env_spaces_file_name):
-                    raise FileNotFoundError("Unable to load environment spaces from specified file ({}), no file found.".format(self.env_spaces_file_name))    
-                else:    
+                    raise FileNotFoundError("Unable to load environment spaces from specified file ({}), no file found.".format(self.env_spaces_file_name))
+                else:
                     self.load_spaces_from_file = config["load_spaces_from_file"]
         else:
             if "env_spaces_file_name" in config.keys():
                 self.env_spaces_file_name = config["env_spaces_file_name"]
 
         if self.load_spaces_from_file is False:
 
@@ -66,15 +65,15 @@
 
             if create_env_on_driver is True:
                 self.rank += num_envs_per_worker
 
             self.logger.debug("Rank: {}".format(self.rank))
 
             self.env = diambra.arena.make(self.game_id, self.settings, self.wrappers_settings,
-                                        seed=self.seed + self.rank, rank=self.rank)
+                                          seed=self.seed + self.rank, rank=self.rank)
 
             env_spaces_dict = {}
             env_spaces_dict["action_space"] = self.env.action_space
             env_spaces_dict["observation_space"] = self.env.observation_space
 
             # Saving environment spaces
             self.logger.info("Saving environment spaces in: {}".format(self.env_spaces_file_name))
```

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/make_sb_env.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/sb_utils.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/sb_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,19 +116,19 @@
 
         return True
 
 # Update p2Brain model Callback
 
 
 class UpdateRLPolicyWeights(BaseCallback):
-    def __init__(self, check_freq: int, num_env: int, save_path: str,
+    def __init__(self, check_freq: int, num_envs: int, save_path: str,
                  prev_agents_sampling={"probability": 0.0, "list": []}, verbose=1):
         super(UpdateRLPolicyWeights, self).__init__(verbose)
-        self.check_freq = int(check_freq / num_env)
-        self.num_env = num_env
+        self.check_freq = int(check_freq / num_envs)
+        self.num_envs = num_envs
         self.save_path = os.path.join(save_path, 'lastModel')
         self.sampling_probability = prev_agents_sampling["probability"]
         self.prev_agents_list = prev_agents_sampling["list"]
         time_dep_seed = int((time.time() - int(time.time() - 0.5)) * 1000)
         np.random.seed(time_dep_seed)
 
     def _on_step(self) -> bool:
```

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/p2_wrap.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/p2_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/stable_baselines3/sb3_utils.py` & `diambra-arena-2.1.0rc8/diambra/arena/stable_baselines3/sb3_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/utils/controller.py` & `diambra-arena-2.1.0rc8/diambra/arena/utils/controller.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/utils/gym_utils.py` & `diambra-arena-2.1.0rc8/diambra/arena/utils/gym_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/utils/policies.py` & `diambra-arena-2.1.0rc8/diambra/arena/utils/policies.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/utils/splash_screen.py` & `diambra-arena-2.1.0rc8/diambra/arena/utils/splash_screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import tkinter as tk
 import screeninfo
 
-gif_file_path = os.path.join(os.path.dirname(__file__), ".splashScreen.gif")
+gif_file_path = os.path.join(os.path.dirname(__file__), ".splash_screen.gif")
 
 
 def get_monitor_from_coord(x, y):
     monitors = screeninfo.get_monitors()
 
     for m in reversed(monitors):
         if m.x <= x <= m.width + m.x and m.y <= y <= m.height + m.y:
```

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/wrappers/arena_wrappers.py` & `diambra-arena-2.1.0rc8/diambra/arena/wrappers/arena_wrappers.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper.py` & `diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/wrappers/obs_wrapper_hardcore.py` & `diambra-arena-2.1.0rc8/diambra/arena/wrappers/obs_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper.py` & `diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py` & `diambra-arena-2.1.0rc8/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc7/diambra_arena.egg-info/PKG-INFO` & `diambra-arena-2.1.0rc8/diambra_arena.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc7
+Version: 2.1.0rc8
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -19,32 +19,44 @@
 Provides-Extra: core
 Provides-Extra: tests
 Provides-Extra: stable-baselines
 Provides-Extra: stable-baselines3
 Provides-Extra: ray-rllib
 License-File: LICENSE.txt
 
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.png" alt="diambra" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.jpg" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
 </p>
 <p align="center">
   <a href="https://www.linkedin.com/company/diambra">Linkedin</a> •
   <a href="https://diambra.ai/discord">Discord</a> •
   <a href="https://www.twitch.tv/diambra_ai">Twitch</a> •
   <a href="https://www.youtube.com/c/diambra_ai">YouTube</a> •
   <a href="https://twitter.com/diambra_ai">Twitter</a>
 </p>
 
 <p align="center">
-<a href="https://arxiv.org/abs/2210.10595"><img src="http://img.shields.io/badge/paper-arxiv.2210.10595-B31B1B.svg" alt="Paper"/></a>
+<a href="https://arxiv.org/abs/2210.10595"><img src="https://img.shields.io/badge/paper-arXiv:2210.10595-B31B1B?logo=arxiv" alt="Paper"/></a>
+</p>
+<p align="center">
+<a href="https://github.com/diambra/arena/actions/workflows/test.yaml"><img src="https://img.shields.io/github/actions/workflow/status/diambra/arena/test.yaml?label=arena%20tests&logo=github" alt="Arena Test"/></a>
+<a href="https://github.com/diambra/arena/actions/workflows/test_agents.yaml"><img src="https://img.shields.io/github/actions/workflow/status/diambra/arena/test_agents.yaml?label=agents%20tests&logo=github" alt="Agents Test"/></a>
+<a href="https://github.com/diambra/arena/tags"><img src="https://img.shields.io/github/v/tag/diambra/arena?label=latest%20tag&logo=github" alt="Latest Tag"/></a>
+<a href="https://pypi.org/project/diambra-arena/"><img src="https://img.shields.io/pypi/v/diambra-arena?logo=pypi" alt="Pypi version"/></a>
+</p>
+<p align="center">
+<a href="https://docs.diambra.ai/#installation"><img src="https://img.shields.io/badge/supported%20os-linux%20%7C%20win%20%7C%20macOS-blue?logo=docker" alt="Supported OS"/></a>
+<a href="https://docs.diambra.ai/"><img src="https://img.shields.io/github/last-commit/diambra/docs/main?label=docs%20last%20update&logo=readthedocs" alt="Last Docs Update"/></a>
 </p>
 
+
+
 # DIAMBRA Arena
 
 ## Index
 
 - **[Overview](#overview)**
 - **[Competition Platform](#competition-platform)**
 - **[Installation](#installation)**
@@ -85,23 +97,21 @@
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
 **Many more are coming soon...**
 
 ## Competition Platform
 
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/leaderboard.jpg" alt="DIAMBRA Leaderboard" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/.github/master/img/platform.jpg" alt="DIAMBRA Competition Platform" width="100%"/>
 
 Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
 
-It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments. 
+It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments.
 
-It also offers you the possibility to unlock cool achievements depending on the performances of your agent. 
-
-<img src="https://raw.githubusercontent.com/diambra/arena/main/img/achievements.jpg" alt="DIAMBRA Achievements" width="100%"/>
+It also offers you the possibility to unlock cool achievements depending on the performances of your agent.
 
 Submitted agents are evaluated and their episodes are streamed on our Twitch channel.
 
 We aimed at making the submission process as smooth as possible, **<a href="https://diambra.ai/register/" target="_blank">join us and try it now!</a>**
 
 ## Installation
 
@@ -121,50 +131,48 @@
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
 
 #### Download Game ROM(s) and Check Validity
 
-Check available games with the following command:
+Check out available games:
 
 ```
 diambra arena list-roms
 ```
 
-Output example:
+Output extract:
 
 ```shell
 [...]
  Title: Dead Or Alive ++ - GameId: doapp
    Difficulty levels: Min 1 - Max 4
    SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
    Original ROM name: doapp.zip
    Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-japan', '80781', 'wowroms']
    Characters list: ['Kasumi', 'Zack', 'Hayabusa', 'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-Lee', 'Ayane']
 [...]
 ```
 
 Search ROMs on the web using **Search Keywords** provided by the game list command reported above. **Pay attention, follow game-specific notes reported there, and store all ROMs in the same folder, whose absolute path will be referred in the following as** `your/roms/local/path`.
 
-**Specific game ROM files are required, check validity of the downloaded ROMs as follows.**
-
-Check ROM(s) validity running:
+**Specific game ROM files are required, check validity of the downloaded ROMs:**
 
 ```
 diambra arena check-roms your/roms/local/path/romFileName.zip
 ```
 
-The output for a valid ROM file would look like the following:
+The output for a valid ROM file would look like:
 
 ```
 Correct ROM file for Dead Or Alive ++, sha256 = d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
 ```
 
-**Make sure to check out our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>, and in particular Section 7. By using the software, you accept the in full.</span>**
+**Make sure to check out our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>, and in particular Section 7. By using the software, you accept them in full.</span>**
 
 #### Base script
 
 Running a complete episode with a random agent requires less than 20 python lines:
 
 ```python {linenos=inline}
  import diambra.arena
@@ -207,17 +215,17 @@
 
 These examples show how to leverage both single and two players modes, how to set up environment wrappers specifying all their options, how to record human expert demonstrations and how to load them to apply imitation learning. They can be used as templates and starting points to explore all the features of the software package.
 
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.gif" alt="diambraGif" width="100%"/>
 
 ## Reinforcement Learning Libs Compatibility
 
-DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents repository</a>. It can easily be interfaced with any other package in a similar way.
+DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines 3 and Ray RLlib, while Stable Baselines is also available but deprecated. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents</a>  repository. It can easily be interfaced with any other package in a similar way.
 
-Native interfaces, that can be installed with the dedicated options listed below, have been tested with the following versions:
+Native interfaces, installed with the specific options listed below, are tested with the following versions:
 
 - Stable Baselines 3 | `pip install diambra-arena[stable-baselines3]` (<a href="https://stable-baselines3.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/DLR-RM/stable-baselines3" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines3/" target="_blank">Pypi</a>): 1.6.1
 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (<a href="https://docs.ray.io/en/latest/index.html" target="_blank">Docs</a> - <a href="https://github.com/ray-project/ray" target="_blank">GitHub</a> - <a href="https://pypi.org/project/ray/" target="_blank">Pypi</a>): 2.0.0
 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (<a href="https://stable-baselines.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/hill-a/stable-baselines" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines/" target="_blank">Pypi</a>): 2.10.2
 
 ## References
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc7 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc8 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -10,14 +10,16 @@
 Entertainment Classifier: Topic :: Games/Entertainment :: Arcade Classifier:
 Topic :: Education Description-Content-Type: text/markdown Provides-Extra: core
 Provides-Extra: tests Provides-Extra: stable-baselines Provides-Extra: stable-
 baselines3 Provides-Extra: ray-rllib License-File: LICENSE.txt [diambra]
                            Documentation â¢ Website
             Linkedin â¢ Discord â¢ Twitch â¢ YouTube â¢ Twitter
                                     [Paper]
+            [Arena_Test] [Agents_Test] [Latest_Tag] [Pypi_version]
+                       [Supported_OS] [Last_Docs_Update]
 # DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
 (#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
 Examples](#quickstart--examples)** - **[Reinforcement Learning Libs
 Compatibility](#reinforcement-learning-libs-compatibility)** - **[References]
 (#references)** - **[Support, Feature Requests & Bugs Reports](#support-
 feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
 Use](#terms-of-use)** ## Overview DIAMBRA Arena is a software package featuring
@@ -75,52 +77,51 @@
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
 Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
-Leaderboard] Our competition platform allows you to submit your agents and
-compete with other coders around the globe in epic video games tournaments! It
-features a public global leaderboard where users are ranked by the best score
-achieved by their agents in our different environments. It also offers you the
-possibility to unlock cool achievements depending on the performances of your
-agent. [DIAMBRA Achievements] Submitted agents are evaluated and their episodes
-are streamed on our Twitch channel. We aimed at making the submission process
-as smooth as possible, **join_us_and_try_it_now!** ## Installation - Create_an
-account_on_our_website, it requires just a few clicks and is 100% free -
-Install Docker Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line
-Interface: `python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -
-m pip install diambra-arena` **Using a virtual environment to isolate your
-python packages installation is strongly suggested** ## Quickstart & Examples
-DIAMBRA Arena usage follows the standard RL interaction framework: the agent
-sends an action to the environment, which process it and performs a transition
+Competition Platform] Our competition platform allows you to submit your agents
+and compete with other coders around the globe in epic video games tournaments!
+It features a public global leaderboard where users are ranked by the best
+score achieved by their agents in our different environments. It also offers
+you the possibility to unlock cool achievements depending on the performances
+of your agent. Submitted agents are evaluated and their episodes are streamed
+on our Twitch channel. We aimed at making the submission process as smooth as
+possible, **join_us_and_try_it_now!** ## Installation - Create_an_account_on
+our_website, it requires just a few clicks and is 100% free - Install Docker
+Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line Interface:
+`python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -m pip
+install diambra-arena` **Using a virtual environment to isolate your python
+packages installation is strongly suggested** ## Quickstart & Examples DIAMBRA
+Arena usage follows the standard RL interaction framework: the agent sends an
+action to the environment, which process it and performs a transition
 accordingly, from the starting state to the new state, returning the
 observation and the reward to the agent to close the interaction loop. The
 figure below shows this typical interaction scheme and data flow.
                                   [rlScheme]
-#### Download Game ROM(s) and Check Validity Check available games with the
-following command: ``` diambra arena list-roms ``` Output example: ```shell
-[...] Title: Dead Or Alive ++ - GameId: doapp Difficulty levels: Min 1 - Max 4
-SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
-Original ROM name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]',
-'dead-or-alive-japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack',
-'Hayabusa', 'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-
-Lee', 'Ayane'] [...] ``` Search ROMs on the web using **Search Keywords**
-provided by the game list command reported above. **Pay attention, follow game-
-specific notes reported there, and store all ROMs in the same folder, whose
-absolute path will be referred in the following as** `your/roms/local/path`.
-**Specific game ROM files are required, check validity of the downloaded ROMs
-as follows.** Check ROM(s) validity running: ``` diambra arena check-roms your/
-roms/local/path/romFileName.zip ``` The output for a valid ROM file would look
-like the following: ``` Correct ROM file for Dead Or Alive ++, sha256 =
+#### Download Game ROM(s) and Check Validity Check out available games: ```
+diambra arena list-roms ``` Output extract: ```shell [...] Title: Dead Or Alive
+++ - GameId: doapp Difficulty levels: Min 1 - Max 4 SHA256 sum:
+d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e Original ROM
+name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-
+japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack', 'Hayabusa',
+'Bayman', 'Lei-Fang', 'Raidou', 'Gen-Fu', 'Tina', 'Bass', 'Jann-Lee', 'Ayane']
+[...] ``` Search ROMs on the web using **Search Keywords** provided by the game
+list command reported above. **Pay attention, follow game-specific notes
+reported there, and store all ROMs in the same folder, whose absolute path will
+be referred in the following as** `your/roms/local/path`. **Specific game ROM
+files are required, check validity of the downloaded ROMs:** ``` diambra arena
+check-roms your/roms/local/path/romFileName.zip ``` The output for a valid ROM
+file would look like: ``` Correct ROM file for Dead Or Alive ++, sha256 =
 d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e ``` **Make
 sure to check out our Terms_of_Use, and in particular Section 7. By using the
-software, you accept the in full.** #### Base script Running a complete episode
-with a random agent requires less than 20 python lines: ```python
+software, you accept them in full.** #### Base script Running a complete
+episode with a random agent requires less than 20 python lines: ```python
 {linenos=inline} import diambra.arena env = diambra.arena.make("doapp")
 observation = env.reset() while True: env.render() actions =
 env.action_space.sample() observation, reward, done, info = env.step(actions)
 if done: observation = env.reset() break env.close() ``` To execute the script
 run: ``` diambra run -r your/roms/local/path python script.py ``` Additional
 details and use cases are provided in the Getting_Started section of the
 documentation. ### Examples The `examples/` folder contains ready to use
@@ -130,31 +131,31 @@
 both single and two players modes, how to set up environment wrappers
 specifying all their options, how to record human expert demonstrations and how
 to load them to apply imitation learning. They can be used as templates and
 starting points to explore all the features of the software package.
 [diambraGif] ## Reinforcement Learning Libs Compatibility DIAMBRA Arena is
 built to maximize compatibility will all major Reinforcement Learning
 libraries. It natively provides interfaces with the two most import packages:
-Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is
-illustrated in detail in the documentation and in the DIAMBRA_Agents
-repository. It can easily be interfaced with any other package in a similar
-way. Native interfaces, that can be installed with the dedicated options listed
-below, have been tested with the following versions: - Stable Baselines 3 |
-`pip install diambra-arena[stable-baselines3]` (Docs - GitHub - Pypi): 1.6.1 -
-Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs - GitHub - Pypi):
-2.0.0 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (Docs
-- GitHub - Pypi): 2.10.2 ## References - Documentation: https://docs.diambra.ai
-- Paper: https://arxiv.org/abs/2210.10595 - Website: https://diambra.ai -
-Discord: https://diambra.ai/discord - Linkedin: https://www.linkedin.com/
-company/diambra - Twitch: https://www.twitch.tv/diambra_ai - YouTube: https://
-www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/diambra_ai ##
-Support, Feature Requests & Bugs Reports To receive support, use the dedicated
-channel in our Discord_Server. To request features or report bugs, use the
-GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595
-```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
-Arena: a New Reinforcement Learning Platform for Research and
+Stable Baselines 3 and Ray RLlib, while Stable Baselines is also available but
+deprecated. Their usage is illustrated in detail in the documentation and in
+the DIAMBRA_Agents repository. It can easily be interfaced with any other
+package in a similar way. Native interfaces, installed with the specific
+options listed below, are tested with the following versions: - Stable
+Baselines 3 | `pip install diambra-arena[stable-baselines3]` (Docs - GitHub -
+Pypi): 1.6.1 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs -
+GitHub - Pypi): 2.0.0 - Stable Baselines | `pip install diambra-arena[stable-
+baselines]` (Docs - GitHub - Pypi): 2.10.2 ## References - Documentation:
+https://docs.diambra.ai - Paper: https://arxiv.org/abs/2210.10595 - Website:
+https://diambra.ai - Discord: https://diambra.ai/discord - Linkedin: https://
+www.linkedin.com/company/diambra - Twitch: https://www.twitch.tv/diambra_ai -
+YouTube: https://www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/
+diambra_ai ## Support, Feature Requests & Bugs Reports To receive support, use
+the dedicated channel in our Discord_Server. To request features or report
+bugs, use the GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/
+2210.10595 ```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title =
+"{DIAMBRA Arena: a New Reinforcement Learning Platform for Research and
 Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
 learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
 = {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
 eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
 Arena software package is subject to our Terms_of_Use. By using it, you accept
 them in full. ###### DIAMBRA, Inc. Â© Copyright 2018-2023. All Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc7/diambra_arena.egg-info/SOURCES.txt` & `diambra-arena-2.1.0rc8/diambra_arena.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 diambra/arena/stable_baselines/wrappers/__init__.py
 diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
 diambra/arena/stable_baselines/wrappers/p2_wrap.py
 diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
 diambra/arena/stable_baselines3/__init__.py
 diambra/arena/stable_baselines3/make_sb3_env.py
 diambra/arena/stable_baselines3/sb3_utils.py
-diambra/arena/utils/.splashScreen.gif
+diambra/arena/utils/.splash_screen.gif
 diambra/arena/utils/__init__.py
 diambra/arena/utils/controller.py
+diambra/arena/utils/engine_mock.py
 diambra/arena/utils/gym_utils.py
 diambra/arena/utils/integratedGames.json
 diambra/arena/utils/policies.py
 diambra/arena/utils/splash_screen.py
 diambra/arena/wrappers/__init__.py
 diambra/arena/wrappers/arena_wrappers.py
 diambra/arena/wrappers/obs_wrapper.py
```

### Comparing `diambra-arena-2.1.0rc7/setup.py` & `diambra-arena-2.1.0rc8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     description="DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments",
     long_description = (Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     license='Custom',
     install_requires=[
             'pip>=21',
             'importlib-metadata<=4.12.0; python_version <= "3.7"', # problem with gym for importlib-metadata==5.0.0 and python <=3.7
+            'wheel==0.38.4', # Required until we can upgrade to gym >= 0.22.0
             'setuptools',
             'distro>=1',
             'gym<=0.21.0',
             'inputs',
             'screeninfo',
             'tk',
             'opencv-python>=4.4.0.42',
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_gym_settings.py` & `diambra-arena-2.1.0rc8/tests/test_gym_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env python3
 import pytest
-import sys
 import random
-import os
-from engine_mock import DiambraEngineMock, EngineMockParams
 import diambra.arena
+from diambra.arena.utils.engine_mock import DiambraEngineMock
 from diambra.arena.utils.gym_utils import available_games
-import numpy as np
 from pytest_utils import generate_pytest_decorator_input
 
 # Example Usage:
 # pytest
 # (optional)
 #    module.py (Run specific module)
 #    -s (show output)
-#    -k 'expression' (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. 'wrappers and doapp')
+#    -k "expression" (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. "wrappers and doapp")
 
 def env_exec(settings, wrappers_settings, traj_rec_settings):
     try:
         env = diambra.arena.make(settings["game_id"], settings, wrappers_settings, traj_rec_settings)
 
         env.close()
 
@@ -27,28 +24,25 @@
     except Exception as e:
         print(e)
         print("ERROR, ABORTED.")
         return 1
 
 def func(settings, wrappers_settings, traj_rec_settings, mocker):
 
-    diambra_engine_mock_params = EngineMockParams()
-    diambra_engine_mock = DiambraEngineMock(diambra_engine_mock_params)
+    diambra_engine_mock = DiambraEngineMock()
 
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.__init__', diambra_engine_mock._mock__init__)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._env_init', diambra_engine_mock._mock_env_init)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._reset', diambra_engine_mock._mock_reset)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_1p', diambra_engine_mock._mock_step_1p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_2p', diambra_engine_mock._mock_step_2p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.close', diambra_engine_mock._mock_close)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.__init__", diambra_engine_mock._mock__init__)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._env_init", diambra_engine_mock._mock_env_init)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._reset", diambra_engine_mock._mock_reset)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_1p", diambra_engine_mock._mock_step_1p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_2p", diambra_engine_mock._mock_step_2p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.close", diambra_engine_mock._mock_close)
 
     try:
         return env_exec(settings, wrappers_settings, traj_rec_settings)
-
-        return 0
     except Exception as e:
         print(e)
         return 1
 
 games_dict = available_games(False)
 gym_settings_var_order = ["player", "step_ratio", "frame_shape", "tower", "super_art",
                           "fighting_style", "ultimate_style", "continue_game", "action_space",
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_imitation_learning.py` & `diambra-arena-2.1.0rc8/tests/test_imitation_learning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 import pytest
 import diambra.arena
-import argparse
 import os
-import sys
 from os import listdir
 import numpy as np
 
 def func(path, hardcore):
     try:
         nProc = 1
 
@@ -109,19 +107,19 @@
         return 0
     except Exception as e:
         print(e)
         return 1
 
 
 base_path = os.path.dirname(__file__)
-normal_discrete = os.path.join(base_path, 'data/Discrete/Normal')
-hardcore_discrete = os.path.join(base_path, 'data/Discrete/HC')
+normal_discrete = os.path.join(base_path, "data/Discrete/Normal")
+hardcore_discrete = os.path.join(base_path, "data/Discrete/HC")
 
-normal_multi_discrete = os.path.join(base_path, 'data/MultiDiscrete/Normal')
-hardcore_multi_discrete = os.path.join(base_path, 'data/MultiDiscrete/HC')
+normal_multi_discrete = os.path.join(base_path, "data/MultiDiscrete/Normal")
+hardcore_multi_discrete = os.path.join(base_path, "data/MultiDiscrete/HC")
 
 @pytest.mark.parametrize("path", [normal_discrete, normal_multi_discrete])
 def test_imitation_normal_mode(path):
     assert func(path, False) == 0
 
 @pytest.mark.parametrize("path", [hardcore_discrete, hardcore_multi_discrete])
 def test_imitation_hardcore_mode(path):
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_integration.py` & `diambra-arena-2.1.0rc8/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 #!/usr/bin/env python3
 import pytest
 from env_exec_interface import env_exec
-import sys
 import random
 from os.path import expanduser
 import os
-import time
-import numpy as np
 
 # Example Usage:
 # pytest
 # (optional)
 #    module.py (Run specific module)
 #    -s (show output)
-#    -k 'expression' (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. 'wrappers and doapp')
+#    -k "expression" (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. "wrappers and doapp")
 
 def func(game_id, player, continue_game, action_space, attack_buttons_combination,
          wrappers_settings, traj_rec_settings, hardcore_prob, no_action_prob):
 
     # Args
     args = {}
     args["interactive_viz"] = False
@@ -35,16 +32,14 @@
         settings["attack_but_combination"] = (attack_buttons_combination, attack_buttons_combination)
         if settings["player"] != "P1P2":
             settings["action_space"] = settings["action_space"][0]
             settings["attack_but_combination"] = settings["attack_but_combination"][0]
         settings["hardcore"] = random.choices([True, False], [hardcore_probability, 1.0 - hardcore_probability])[0]
 
         return env_exec(settings, wrappers_settings, traj_rec_settings, args)
-
-        return 0
     except Exception as e:
         print(e)
         return 1
 
 game_ids = ["doapp", "sfiii3n", "tektagt", "umk3", "samsh5sp", "kof98umh"]
 players = ["Random", "P1P2"]
 action_spaces = ["multi_discrete"]
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_random.py` & `diambra-arena-2.1.0rc8/tests/test_random.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,56 @@
 #!/usr/bin/env python3
 import pytest
 from env_exec_interface import env_exec
-import sys
 import random
 from os.path import expanduser
 import os
-from engine_mock import DiambraEngineMock, EngineMockParams
+import diambra.arena
+from diambra.arena.utils.engine_mock import DiambraEngineMock
 
 # Example Usage:
 # pytest
 # (optional)
 #    module.py (Run specific module)
 #    -s (show output)
-#    -k 'expression' (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. 'wrappers and doapp')
+#    -k "expression" (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. "wrappers and doapp")
 
-def func(player, continue_game, action_space, attack_buttons_combination,
+def func(player, continue_game, action_space, attack_buttons_combination, frame_shape,
          wrappers_settings, traj_rec_settings, hardcore_prob, no_action_prob, mocker):
 
     # Args
     args = {}
     args["interactive_viz"] = False
     args["n_episodes"] = 1
+    args["no_action"] = random.choices([True, False], [no_action_prob, 1.0 - no_action_prob])[0]
 
-    args["no_action"] = random.choices([True, False], [no_action_probability, 1.0 - no_action_probability])[0]
+    diambra_engine_mock = DiambraEngineMock()
 
-    round_winning_probability = 0.5
-    perfect_probability=0.2
-    if args["no_action"] is True:
-        round_winning_probability = 0.0
-        perfect_probability = 0.0
-
-    rounds_per_stage = random.choice([2, 3])
-    stages_per_game = random.choice([2, 3])
-    number_of_chars = random.choice([11,33])
-    number_of_chars_per_round = random.choice([1, 2])
-    min_health = random.choice([-1, 0])
-    max_health = random.choice([100, 208])
-    frame_shape = random.choice([[128, 128, 3], [480, 512, 3]])
-    n_actions = random.choice([[9, 7, 12], [9, 6, 6], [9, 6, 12]])
-
-    diambra_engine_mock_params = EngineMockParams(round_winning_probability=round_winning_probability,
-                                                  perfect_probability=perfect_probability, rounds_per_stage=rounds_per_stage,
-                                                  stages_per_game=stages_per_game, number_of_chars=number_of_chars,
-                                                  number_of_chars_per_round=number_of_chars_per_round,
-                                                  min_health=min_health, max_health=max_health, frame_shape=frame_shape,
-                                                  n_actions=n_actions)
-    diambra_engine_mock = DiambraEngineMock(diambra_engine_mock_params)
-
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.__init__', diambra_engine_mock._mock__init__)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._env_init', diambra_engine_mock._mock_env_init)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._reset', diambra_engine_mock._mock_reset)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_1p', diambra_engine_mock._mock_step_1p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_2p', diambra_engine_mock._mock_step_2p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.close', diambra_engine_mock._mock_close)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.__init__", diambra_engine_mock._mock__init__)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._env_init", diambra_engine_mock._mock_env_init)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._reset", diambra_engine_mock._mock_reset)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_1p", diambra_engine_mock._mock_step_1p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_2p", diambra_engine_mock._mock_step_2p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.close", diambra_engine_mock._mock_close)
 
     try:
         # Settings
         settings = {}
-        settings["game_id"] = "doapp"
+        settings["game_id"] = random.choice(list(diambra.arena.available_games(print_out=False).keys()))
         settings["player"] = player
+        settings["frame_shape"] = frame_shape
         settings["continue_game"] = continue_game
         settings["action_space"] = (action_space, action_space)
         settings["attack_but_combination"] = (attack_buttons_combination, attack_buttons_combination)
         if settings["player"] != "P1P2":
             settings["action_space"] = settings["action_space"][0]
             settings["attack_but_combination"] = settings["attack_but_combination"][0]
-        settings["hardcore"] = random.choices([True, False], [hardcore_probability, 1.0 - hardcore_probability])[0]
+        settings["hardcore"] = random.choices([True, False], [hardcore_prob, 1.0 - hardcore_prob])[0]
 
         return env_exec(settings, wrappers_settings, traj_rec_settings, args)
-
-        return 0
     except Exception as e:
         print(e)
         return 1
 
 players = ["Random", "P1P2"]
 continue_games = [-1.0, 0.0, 0.3]
 action_spaces = ["discrete", "multi_discrete"]
@@ -83,25 +60,28 @@
 rec_traj_probability = 0.5
 
 @pytest.mark.parametrize("player", players)
 @pytest.mark.parametrize("continue_game", continue_games)
 @pytest.mark.parametrize("action_space", action_spaces)
 @pytest.mark.parametrize("attack_buttons_combination", attack_buttons_combinations)
 def test_random_gym(player, continue_game, action_space, attack_buttons_combination, mocker):
+    frame_shape = random.choice([(128, 128, 1), (256, 256, 0)])
     wrappers_settings = {}
     traj_rec_settings = {}
-    assert func(player, continue_game, action_space, attack_buttons_combination,
+    assert func(player, continue_game, action_space, attack_buttons_combination, frame_shape,
                 wrappers_settings, traj_rec_settings, hardcore_probability, no_action_probability, mocker) == 0
 
 @pytest.mark.parametrize("player", players)
 @pytest.mark.parametrize("continue_game", continue_games)
 @pytest.mark.parametrize("action_space", action_spaces)
 @pytest.mark.parametrize("attack_buttons_combination", attack_buttons_combinations)
 def test_random_wrappers(player, continue_game, action_space, attack_buttons_combination, mocker):
 
+    frame_shape = (256, 256, 0)
+
     # Env wrappers settings
     wrappers_settings = {}
     wrappers_settings["no_op_max"] = 0
     wrappers_settings["sticky_actions"] = 1
     wrappers_settings["hwc_obs_resize"] = (128, 128, 1)
     wrappers_settings["reward_normalization"] = True
     wrappers_settings["clip_rewards"] = False
@@ -122,9 +102,9 @@
     traj_rec_settings["ignore_p2"] = False
 
     if (random.choices([True, False], [rec_traj_probability, 1.0 - rec_traj_probability])[0] is False):
         traj_rec_settings = {}
     else:
         wrappers_settings["flatten"] = False
 
-    assert func(player, continue_game, action_space, attack_buttons_combination,
+    assert func(player, continue_game, action_space, attack_buttons_combination, frame_shape,
                 wrappers_settings, traj_rec_settings, hardcore_probability, no_action_probability, mocker) == 0
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_recording_settings.py` & `diambra-arena-2.1.0rc8/tests/test_recording_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python
 import pytest
-import sys
-import random
 from os.path import expanduser
 import os
-from engine_mock import DiambraEngineMock, EngineMockParams
+from diambra.arena.utils.engine_mock import DiambraEngineMock
 import diambra.arena
-import numpy as np
 from pytest_utils import generate_pytest_decorator_input
 from diambra.arena.utils.gym_utils import available_games
 
 # Example Usage:
 # pytest
 # (optional)
 #    module.py (Run specific module)
 #    -s (show output)
-#    -k 'expression' (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. 'wrappers and doapp')
+#    -k "expression" (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. "wrappers and doapp")
 
 def env_exec(settings, wrappers_settings, traj_rec_settings):
     try:
         env = diambra.arena.make(settings["game_id"], settings, wrappers_settings, traj_rec_settings)
         env.close()
 
         print("COMPLETED SUCCESSFULLY!")
@@ -27,28 +24,25 @@
     except Exception as e:
         print(e)
         print("ERROR, ABORTED.")
         return 1
 
 def func(settings, wrappers_settings, traj_rec_settings, mocker):
 
-    diambra_engine_mock_params = EngineMockParams()
-    diambra_engine_mock = DiambraEngineMock(diambra_engine_mock_params)
+    diambra_engine_mock = DiambraEngineMock()
 
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.__init__', diambra_engine_mock._mock__init__)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._env_init', diambra_engine_mock._mock_env_init)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._reset', diambra_engine_mock._mock_reset)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_1p', diambra_engine_mock._mock_step_1p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_2p', diambra_engine_mock._mock_step_2p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.close', diambra_engine_mock._mock_close)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.__init__", diambra_engine_mock._mock__init__)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._env_init", diambra_engine_mock._mock_env_init)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._reset", diambra_engine_mock._mock_reset)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_1p", diambra_engine_mock._mock_step_1p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_2p", diambra_engine_mock._mock_step_2p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.close", diambra_engine_mock._mock_close)
 
     try:
         return env_exec(settings, wrappers_settings, traj_rec_settings)
-
-        return 0
     except Exception as e:
         print(e)
         return 1
 
 wrappers_settings_var_order = ["username", "file_path", "ignore_p2"]
 games_dict = available_games(False)
 home_dir = expanduser("~")
@@ -102,8 +96,8 @@
 
     # Recording settings
     traj_rec_settings = {}
     traj_rec_settings["username"] = username
     traj_rec_settings["file_path"] = file_path
     traj_rec_settings["ignore_p2"] = ignore_p2
 
-    assert func(settings, wrappers_settings, traj_rec_settings, mocker) == expected
+    assert func(settings, wrappers_settings, traj_rec_settings, mocker) == expected
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_speed.py` & `diambra-arena-2.1.0rc8/tests/test_speed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 #!/usr/bin/env python3
 import pytest
 from env_exec_interface import env_exec
-import sys
 import time
-import random
 from os.path import expanduser
-import os
-from engine_mock import DiambraEngineMock, EngineMockParams
 import diambra.arena
+from diambra.arena.utils.engine_mock import DiambraEngineMock
 import numpy as np
 import warnings
 
 def reject_outliers(data):
     u = np.mean(data)
     s = np.std(data)
     filtered = [e for e in data if (u - 2 * s < e < u + 2 * s)]
     return filtered
 
 def func(player, wrappers_settings, target_speed, mocker):
 
-    diambra_engine_mock_params = EngineMockParams(round_winning_probability=0.5,
-                                                  perfect_probability=0.0, fps=500)
-    diambra_engine_mock = DiambraEngineMock(diambra_engine_mock_params)
+    diambra_engine_mock = DiambraEngineMock(fps=500)
 
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.__init__', diambra_engine_mock._mock__init__)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._env_init', diambra_engine_mock._mock_env_init)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._reset', diambra_engine_mock._mock_reset)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_1p', diambra_engine_mock._mock_step_1p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_2p', diambra_engine_mock._mock_step_2p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.close', diambra_engine_mock._mock_close)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.__init__", diambra_engine_mock._mock__init__)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._env_init", diambra_engine_mock._mock_env_init)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._reset", diambra_engine_mock._mock_reset)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_1p", diambra_engine_mock._mock_step_1p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_2p", diambra_engine_mock._mock_step_2p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.close", diambra_engine_mock._mock_close)
 
     try:
         # Settings
         settings = {}
         settings["player"] = player
         settings["action_space"] = "discrete"
         settings["attack_but_combination"] = False
```

### Comparing `diambra-arena-2.1.0rc7/tests/test_wrappers_settings.py` & `diambra-arena-2.1.0rc8/tests/test_wrappers_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 #!/usr/bin/env python
 import pytest
-import sys
-import random
 from os.path import expanduser
-import os
-from engine_mock import DiambraEngineMock, EngineMockParams
 import diambra.arena
-import numpy as np
+from diambra.arena.utils.engine_mock import DiambraEngineMock
 from pytest_utils import generate_pytest_decorator_input
 from diambra.arena.utils.gym_utils import available_games
 
 # Example Usage:
 # pytest
 # (optional)
 #    module.py (Run specific module)
 #    -s (show output)
-#    -k 'expression' (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. 'wrappers and doapp')
+#    -k "expression" (filter tests using case-insensitive with parts of the test name and/or parameters values combined with boolean operators, e.g. "wrappers and doapp")
 
 def env_exec(settings, wrappers_settings, traj_rec_settings):
     try:
         env = diambra.arena.make(settings["game_id"], settings, wrappers_settings, traj_rec_settings)
         env.close()
 
         print("COMPLETED SUCCESSFULLY!")
@@ -27,28 +23,25 @@
     except Exception as e:
         print(e)
         print("ERROR, ABORTED.")
         return 1
 
 def func(settings, wrappers_settings, traj_rec_settings, mocker):
 
-    diambra_engine_mock_params = EngineMockParams()
-    diambra_engine_mock = DiambraEngineMock(diambra_engine_mock_params)
+    diambra_engine_mock = DiambraEngineMock()
 
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.__init__', diambra_engine_mock._mock__init__)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._env_init', diambra_engine_mock._mock_env_init)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._reset', diambra_engine_mock._mock_reset)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_1p', diambra_engine_mock._mock_step_1p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine._step_2p', diambra_engine_mock._mock_step_2p)
-    mocker.patch('diambra.arena.engine.interface.DiambraEngine.close', diambra_engine_mock._mock_close)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.__init__", diambra_engine_mock._mock__init__)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._env_init", diambra_engine_mock._mock_env_init)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._reset", diambra_engine_mock._mock_reset)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_1p", diambra_engine_mock._mock_step_1p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine._step_2p", diambra_engine_mock._mock_step_2p)
+    mocker.patch("diambra.arena.engine.interface.DiambraEngine.close", diambra_engine_mock._mock_close)
 
     try:
         return env_exec(settings, wrappers_settings, traj_rec_settings)
-
-        return 0
     except Exception as e:
         print(e)
         return 1
 
 wrappers_settings_var_order = ["no_op_max", "sticky_actions", "hwc_obs_resize", "reward_normalization",
                                "reward_normalization_factor", "clip_rewards", "frame_stack", "dilation",
                                "actions_stack", "scale", "scale_mod", "flatten", "filter_keys"]
@@ -131,8 +124,8 @@
     wrappers_settings["scale_mod"] = scale_mod
     wrappers_settings["flatten"] = flatten
     wrappers_settings["filter_keys"] = filter_keys
 
     # Recording settings
     traj_rec_settings = {}
 
-    assert func(settings, wrappers_settings, traj_rec_settings, mocker) == expected
+    assert func(settings, wrappers_settings, traj_rec_settings, mocker) == expected
```

