# Comparing `tmp/modular_rl-0.3.0.tar.gz` & `tmp/modular_rl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.3.0.tar", last modified: Tue Jun  6 22:29:53 2023, max compression
+gzip compressed data, was "modular_rl-0.3.1.tar", last modified: Tue Jun  6 22:51:54 2023, max compression
```

## Comparing `modular_rl-0.3.0.tar` & `modular_rl-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.139493 modular_rl-0.3.0/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     5465 2023-06-06 22:29:53.138484 modular_rl-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4099 2023-06-04 21:09:01.000000 modular_rl-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.078710 modular_rl-0.3.0/modular_rl/
--rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.099473 modular_rl-0.3.0/modular_rl/agents/
--rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.0/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0     9544 2023-06-06 21:33:56.000000 modular_rl-0.3.0/modular_rl/agents/_agent.py
--rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.0/modular_rl/agents/_custom.py
--rw-rw-rw-   0        0        0    12360 2023-06-06 21:42:41.000000 modular_rl-0.3.0/modular_rl/agents/mcis.py
--rw-rw-rw-   0        0        0    11964 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    20686 2023-06-06 22:24:07.000000 modular_rl-0.3.0/modular_rl/agents/mim.py
--rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.0/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.100701 modular_rl-0.3.0/modular_rl/envs/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/__init__.py
--rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.105921 modular_rl-0.3.0/modular_rl/envs/mim/
--rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/mim/__init__.py
--rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/mim/card_evaluator.py
--rw-rw-rw-   0        0        0     4474 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/mim/mim.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.111871 modular_rl-0.3.0/modular_rl/networks/
--rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/networks/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/networks/actor_critic.py
--rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.0/modular_rl/networks/policy.py
--rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.0/modular_rl/networks/value.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.118471 modular_rl-0.3.0/modular_rl/params/
--rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/params/mcis.py
--rw-rw-rw-   0        0        0     2345 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0      975 2023-06-06 21:47:23.000000 modular_rl-0.3.0/modular_rl/params/mim.py
--rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1352 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.125524 modular_rl-0.3.0/modular_rl/tester/
--rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/tester/__init__.py
--rw-rw-rw-   0        0        0      978 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/tester/mcis.py
--rw-rw-rw-   0        0        0      366 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/tester/mcts.py
--rw-rw-rw-   0        0        0      323 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/tester/mim.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.3.0/modular_rl/tester/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.128026 modular_rl-0.3.0/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.0/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.086917 modular_rl-0.3.0/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     5465 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-06-06 21:24:49.000000 modular_rl-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 22:29:53.139493 modular_rl-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-06-06 21:25:01.000000 modular_rl-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.136420 modular_rl-0.3.0/tests/
--rw-rw-rw-   0        0        0       97 2023-06-04 21:09:01.000000 modular_rl-0.3.0/tests/test_mcis.py
--rw-rw-rw-   0        0        0      105 2023-06-04 21:09:01.000000 modular_rl-0.3.0/tests/test_mcis_modular.py
--rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.3.0/tests/test_mcts.py
--rw-rw-rw-   0        0        0      107 2023-06-04 21:09:01.000000 modular_rl-0.3.0/tests/test_mim.py
--rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.3.0/tests/test_ppo.py
--rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.3.0/tests/test_ppo_modular.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.852496 modular_rl-0.3.1/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5670 2023-06-06 22:51:54.852496 modular_rl-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4164 2023-06-06 22:51:16.000000 modular_rl-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.794867 modular_rl-0.3.1/modular_rl/
+-rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.812342 modular_rl-0.3.1/modular_rl/agents/
+-rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.1/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0     9544 2023-06-06 21:33:56.000000 modular_rl-0.3.1/modular_rl/agents/_agent.py
+-rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.1/modular_rl/agents/_custom.py
+-rw-rw-rw-   0        0        0    12360 2023-06-06 21:42:41.000000 modular_rl-0.3.1/modular_rl/agents/mcis.py
+-rw-rw-rw-   0        0        0    11964 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    20686 2023-06-06 22:24:07.000000 modular_rl-0.3.1/modular_rl/agents/mim.py
+-rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.1/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.814474 modular_rl-0.3.1/modular_rl/envs/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.817646 modular_rl-0.3.1/modular_rl/envs/mim/
+-rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/mim/__init__.py
+-rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/mim/card_evaluator.py
+-rw-rw-rw-   0        0        0     4474 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/mim/mim.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.823543 modular_rl-0.3.1/modular_rl/networks/
+-rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/networks/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/networks/actor_critic.py
+-rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.1/modular_rl/networks/policy.py
+-rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.1/modular_rl/networks/value.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.832480 modular_rl-0.3.1/modular_rl/params/
+-rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/params/mcis.py
+-rw-rw-rw-   0        0        0     2345 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     1938 2023-06-06 22:34:44.000000 modular_rl-0.3.1/modular_rl/params/mim.py
+-rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.3.1/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.838130 modular_rl-0.3.1/modular_rl/tester/
+-rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/tester/__init__.py
+-rw-rw-rw-   0        0        0      978 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/tester/mcis.py
+-rw-rw-rw-   0        0        0      366 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/tester/mcts.py
+-rw-rw-rw-   0        0        0      689 2023-06-06 22:45:16.000000 modular_rl-0.3.1/modular_rl/tester/mim.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.3.1/modular_rl/tester/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.840339 modular_rl-0.3.1/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.1/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.802163 modular_rl-0.3.1/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     5670 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-06-06 22:51:47.000000 modular_rl-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 22:51:54.852496 modular_rl-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-06-06 22:51:40.000000 modular_rl-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.851292 modular_rl-0.3.1/tests/
+-rw-rw-rw-   0        0        0       97 2023-06-04 21:09:01.000000 modular_rl-0.3.1/tests/test_mcis.py
+-rw-rw-rw-   0        0        0      105 2023-06-04 21:09:01.000000 modular_rl-0.3.1/tests/test_mcis_modular.py
+-rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.3.1/tests/test_mcts.py
+-rw-rw-rw-   0        0        0      107 2023-06-04 21:09:01.000000 modular_rl-0.3.1/tests/test_mim.py
+-rw-rw-rw-   0        0        0      111 2023-06-06 22:42:10.000000 modular_rl-0.3.1/tests/test_mim_modular.py
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.3.1/tests/test_ppo.py
+-rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.3.1/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.3.0/LICENSE` & `modular_rl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/PKG-INFO` & `modular_rl-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_rl
-Version: 0.3.0
+Version: 0.3.1
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 Home-page: https://github.com/horrible-gh/ModularRL
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -31,28 +31,32 @@
 ```powershell
 pip install modular_rl
 ```
 
 ## Features
 
 -   Implementations of various reinforcement learning algorithms,
-    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
+    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
 -   Customizable agent settings and network architectures
 -   Modular structure for easy adaptation and extension across different algorithms
 -   Model saving and loading functionality for easy reuse of trained models
 
 ## Supported Algorithms
 
 -   Proximal Policy Optimization (PPO)
 -   Monte Carlo Tree Search (MCTS)
+-   Monte Carlo Information Set (MCIS)
+-   Modular's sIMulator (MIM)
 
 Refer to the respective agent classes for each algorithm:
 
 -   AgentPPO (Modular)
 -   AgentMCTS
+-   AgentMCIS (Modular)
+-   AgentMIM (Modular)
 
 ## Example Usage
 
 You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
 
 ```python
 import modular_rl.tester as tester
@@ -147,14 +151,14 @@
 
 loaded_agent = AgentPPO(env, setting)
 loaded_agent.load_model("my_saved_model.pth")
 ```
 
 ## Key Classes
 
--   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
+-   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
 -   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
 -   AgentSettings: A configuration class for setting up the agents.
 
 ## License
 
 MIT License
```

### Comparing `modular_rl-0.3.0/README.md` & `modular_rl-0.3.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,140 @@
-# ModularRL
-
-ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-
-## Installation
-
-```powershell
-pip install modular_rl
-```
-
-## Features
-
--   Implementations of various reinforcement learning algorithms,
-    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
--   Customizable agent settings and network architectures
--   Modular structure for easy adaptation and extension across different algorithms
--   Model saving and loading functionality for easy reuse of trained models
-
-## Supported Algorithms
-
--   Proximal Policy Optimization (PPO)
--   Monte Carlo Tree Search (MCTS)
-
-Refer to the respective agent classes for each algorithm:
-
--   AgentPPO (Modular)
--   AgentMCTS
-
-## Example Usage
-
-You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
-
-```python
-import modular_rl.tester as tester
-
-tester.init_ppo()
-# or
-tester.init_ppo_modular()
-
-tester.init_mcts()
-```
-
-As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
-
-Please note that not all algorithms support modular training due to the nature of their design.
-For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
-You can refer to the list of supported algorithms to determine which training method is appropriate.
-
-Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init():
-    env = AgentPPO(env=None, setting=AgentSettings.default)
-    env.learn()
-
-init()
-```
-
-To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init_modular():
-    # Semi-automatic (defined record usage)
-    # Implement your environment and pass it to 'env' parameter.
-    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
-    env.reset()
-    env.learn_reset()
-    action, reward, is_done = env.learn_next()
-    env.learn_check()
-    env.update()
-
-    # Proceed with the learning manually.
-    env.reset()
-    # Implement the 'reset' method in your environment.
-    '''
-    def reset(self):
-        ...
-        return initial_state
-    '''
-    env.learn_reset()
-    initial_state = env.learn_reset()
-    action, dist = env.select_action(initial_state)
-
-    '''
-    Note:
-    Please implement the resulting state of update_step in the step function of your environment.
-
-    For example:
-
-    def step(self, action):
-        ...
-        return next_state, reward, is_done, _
-    '''
-
-    env.update_step(initial_state, dist, action, -1)
-
-    env.learn_check()
-    env.update()
-
-    env.learn_close()
-
-init_modular()
-```
-
-## Saving and Loading Models
-
-Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
-The file_name parameter should be the name of the file to save or load the model to/from.
-
-Example:
-
-```python
-agent = AgentPPO(env, setting)
-agent.train()
-
-agent.save_model("my_saved_model.pth")
-
-loaded_agent = AgentPPO(env, setting)
-loaded_agent.load_model("my_saved_model.pth")
-```
-
-## Key Classes
-
--   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
--   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
--   AgentSettings: A configuration class for setting up the agents.
-
-## License
-
-MIT License
+# ModularRL
+
+ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+
+## Installation
+
+```powershell
+pip install modular_rl
+```
+
+## Features
+
+-   Implementations of various reinforcement learning algorithms,
+    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+-   Monte Carlo Information Set (MCIS)
+-   Modular's sIMulator (MIM)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (Modular)
+-   AgentMCTS
+-   AgentMCIS (Modular)
+-   AgentMIM (Modular)
+
+## Example Usage
+
+You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
+
+```python
+import modular_rl.tester as tester
+
+tester.init_ppo()
+# or
+tester.init_ppo_modular()
+
+tester.init_mcts()
+```
+
+As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
+
+Please note that not all algorithms support modular training due to the nature of their design.
+For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
+You can refer to the list of supported algorithms to determine which training method is appropriate.
+
+Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init():
+    env = AgentPPO(env=None, setting=AgentSettings.default)
+    env.learn()
+
+init()
+```
+
+To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init_modular():
+    # Semi-automatic (defined record usage)
+    # Implement your environment and pass it to 'env' parameter.
+    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
+    env.reset()
+    env.learn_reset()
+    action, reward, is_done = env.learn_next()
+    env.learn_check()
+    env.update()
+
+    # Proceed with the learning manually.
+    env.reset()
+    # Implement the 'reset' method in your environment.
+    '''
+    def reset(self):
+        ...
+        return initial_state
+    '''
+    env.learn_reset()
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+
+    '''
+    Note:
+    Please implement the resulting state of update_step in the step function of your environment.
+
+    For example:
+
+    def step(self, action):
+        ...
+        return next_state, reward, is_done, _
+    '''
+
+    env.update_step(initial_state, dist, action, -1)
+
+    env.learn_check()
+    env.update()
+
+    env.learn_close()
+
+init_modular()
+```
+
+## Saving and Loading Models
+
+Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
+The file_name parameter should be the name of the file to save or load the model to/from.
+
+Example:
+
+```python
+agent = AgentPPO(env, setting)
+agent.train()
+
+agent.save_model("my_saved_model.pth")
+
+loaded_agent = AgentPPO(env, setting)
+loaded_agent.load_model("my_saved_model.pth")
+```
+
+## Key Classes
+
+-   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.3.0/modular_rl/agents/_agent.py` & `modular_rl-0.3.1/modular_rl/agents/_agent.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/agents/_custom.py` & `modular_rl-0.3.1/modular_rl/agents/_custom.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/agents/mcis.py` & `modular_rl-0.3.1/modular_rl/agents/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/agents/mcts.py` & `modular_rl-0.3.1/modular_rl/agents/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/agents/mim.py` & `modular_rl-0.3.1/modular_rl/agents/mim.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/agents/ppo.py` & `modular_rl-0.3.1/modular_rl/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/envs/mim/card_evaluator.py` & `modular_rl-0.3.1/modular_rl/envs/mim/card_evaluator.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/envs/mim/mim.py` & `modular_rl-0.3.1/modular_rl/envs/mim/mim.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/networks/actor_critic.py` & `modular_rl-0.3.1/modular_rl/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/networks/policy.py` & `modular_rl-0.3.1/modular_rl/networks/policy.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/networks/value.py` & `modular_rl-0.3.1/modular_rl/networks/value.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/params/mcis.py` & `modular_rl-0.3.1/modular_rl/params/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/params/mcts.py` & `modular_rl-0.3.1/modular_rl/params/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/params/mim.py` & `modular_rl-0.3.1/modular_rl/params/mim.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,7 +10,22 @@
         # The adjustment factor applied to actions that are ranked inferior (i.e., they have a lower score). Lower values result in greater up-weighting.
         'inferior_rank_adjustment_factor': 0.85,
         'log_level': 'debug',  # Log level for the logger
         'log_init_pass': False,  # If True, skip logger initialization
         'max_episodes': 10,  # Maximum number of episodes for training
         'max_timesteps': 200,  # Maximum number of timesteps for each episode
     }
+
+    default_modular = {
+        # The column name used to track the score for evaluating agent's actions.
+        'score_column': 'score',
+        # The number of iterations for each simulation during the MIM's action selection process.
+        'simulation_iterations': 1,
+        # The adjustment factor applied to actions that are ranked superior (i.e., they have a higher score). Lower values result in greater down-weighting.
+        'superior_rank_adjustment_factor': 0.9,
+        # The adjustment factor applied to actions that are ranked inferior (i.e., they have a lower score). Lower values result in greater up-weighting.
+        'inferior_rank_adjustment_factor': 0.85,
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+        'max_episodes': 1,  # Maximum number of episodes for training
+        'max_timesteps': 1,  # Maximum number of timesteps for each episode
+    }
```

### Comparing `modular_rl-0.3.0/modular_rl/params/ppo.py` & `modular_rl-0.3.1/modular_rl/params/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/settings.py` & `modular_rl-0.3.1/modular_rl/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-'''
-The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
-
-It provides default values for various parameters used in the agents, such as the maximum number of episodes,
-maximum number of timesteps per episode, update timestep, network architecture, learning rate,
-discount factor, early stopping threshold, and whether to end training when the environment is done.
-
-The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
-The default dictionary provides default values for all parameters, while the modular version provides default values
-with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
-key-value pairs to the AgentSettings constructor.
-
-'''
-
-from modular_rl.params.ppo import ParamPPO
-from modular_rl.params.mcts import ParamMCTS
-from modular_rl.params.mcis import ParamMCIS
-from modular_rl.params.mim import ParamMIM
-
-class AgentSettings:
-    default_ppo = ParamPPO.default
-    default_ppo_modular = ParamPPO.default_modular
-    default_mcts = ParamMCTS.default
-    default_mcts_modular = ParamMCTS.default_modular
-    default_mcis = ParamMCIS.default
-    default_mcis_modular = ParamMCIS.default_modular
-    default_mim = ParamMIM.default
+'''
+The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
+
+It provides default values for various parameters used in the agents, such as the maximum number of episodes,
+maximum number of timesteps per episode, update timestep, network architecture, learning rate,
+discount factor, early stopping threshold, and whether to end training when the environment is done.
+
+The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
+The default dictionary provides default values for all parameters, while the modular version provides default values
+with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
+key-value pairs to the AgentSettings constructor.
+
+'''
+
+from modular_rl.params.ppo import ParamPPO
+from modular_rl.params.mcts import ParamMCTS
+from modular_rl.params.mcis import ParamMCIS
+from modular_rl.params.mim import ParamMIM
+
+
+class AgentSettings:
+    default_ppo = ParamPPO.default
+    default_ppo_modular = ParamPPO.default_modular
+    default_mcts = ParamMCTS.default
+    default_mcts_modular = ParamMCTS.default_modular
+    default_mcis = ParamMCIS.default
+    default_mcis_modular = ParamMCIS.default_modular
+    default_mim = ParamMIM.default
+    default_mim_modular = ParamMIM.default_modular
```

### Comparing `modular_rl-0.3.0/modular_rl/tester/mcis.py` & `modular_rl-0.3.1/modular_rl/tester/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/tester/ppo.py` & `modular_rl-0.3.1/modular_rl/tester/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl/util/node.py` & `modular_rl-0.3.1/modular_rl/util/node.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.0/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.3.1/modular_rl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-rl
-Version: 0.3.0
+Version: 0.3.1
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 Home-page: https://github.com/horrible-gh/ModularRL
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -31,28 +31,32 @@
 ```powershell
 pip install modular_rl
 ```
 
 ## Features
 
 -   Implementations of various reinforcement learning algorithms,
-    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
+    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
 -   Customizable agent settings and network architectures
 -   Modular structure for easy adaptation and extension across different algorithms
 -   Model saving and loading functionality for easy reuse of trained models
 
 ## Supported Algorithms
 
 -   Proximal Policy Optimization (PPO)
 -   Monte Carlo Tree Search (MCTS)
+-   Monte Carlo Information Set (MCIS)
+-   Modular's sIMulator (MIM)
 
 Refer to the respective agent classes for each algorithm:
 
 -   AgentPPO (Modular)
 -   AgentMCTS
+-   AgentMCIS (Modular)
+-   AgentMIM (Modular)
 
 ## Example Usage
 
 You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
 
 ```python
 import modular_rl.tester as tester
@@ -147,14 +151,14 @@
 
 loaded_agent = AgentPPO(env, setting)
 loaded_agent.load_model("my_saved_model.pth")
 ```
 
 ## Key Classes
 
--   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
+-   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
 -   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
 -   AgentSettings: A configuration class for setting up the agents.
 
 ## License
 
 MIT License
```

### Comparing `modular_rl-0.3.0/modular_rl.egg-info/SOURCES.txt` & `modular_rl-0.3.1/modular_rl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,9 +37,10 @@
 modular_rl/tester/ppo.py
 modular_rl/util/__init__.py
 modular_rl/util/node.py
 tests/test_mcis.py
 tests/test_mcis_modular.py
 tests/test_mcts.py
 tests/test_mim.py
+tests/test_mim_modular.py
 tests/test_ppo.py
 tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.3.0/pyproject.toml` & `modular_rl-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.3.0/setup.py` & `modular_rl-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.3.0',
+    version='0.3.1',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/ModularRL',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

