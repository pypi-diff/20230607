# Comparing `tmp/modular_rl-0.2.3.tar.gz` & `tmp/modular_rl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.2.3.tar", last modified: Tue May 30 13:36:16 2023, max compression
+gzip compressed data, was "modular_rl-0.3.0.tar", last modified: Tue Jun  6 22:29:53 2023, max compression
```

## Comparing `modular_rl-0.2.3.tar` & `modular_rl-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,58 @@
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.599220 modular_rl-0.2.3/
--rw-r--r--   0 sjm        (501) staff       (20)     1068 2023-05-13 00:53:55.000000 modular_rl-0.2.3/LICENSE
--rw-r--r--   0 sjm        (501) staff       (20)     5305 2023-05-30 13:36:16.598637 modular_rl-0.2.3/PKG-INFO
--rw-r--r--   0 sjm        (501) staff       (20)     3963 2023-05-13 00:53:55.000000 modular_rl-0.2.3/README.md
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.542870 modular_rl-0.2.3/modular_rl/
--rw-r--r--   0 sjm        (501) staff       (20)       36 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/__init__.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.561426 modular_rl-0.2.3/modular_rl/agents/
--rw-r--r--   0 sjm        (501) staff       (20)       82 2023-05-29 21:48:43.000000 modular_rl-0.2.3/modular_rl/agents/__init__.py
--rw-r--r--   0 sjm        (501) staff       (20)     9785 2023-05-30 12:42:39.000000 modular_rl-0.2.3/modular_rl/agents/_agent.py
--rw-r--r--   0 sjm        (501) staff       (20)    11169 2023-05-30 13:01:06.000000 modular_rl-0.2.3/modular_rl/agents/mcis.py
--rw-r--r--   0 sjm        (501) staff       (20)    11655 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/agents/mcts.py
--rw-r--r--   0 sjm        (501) staff       (20)    15091 2023-05-30 12:43:22.000000 modular_rl-0.2.3/modular_rl/agents/ppo.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.568544 modular_rl-0.2.3/modular_rl/networks/
--rw-r--r--   0 sjm        (501) staff       (20)       66 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/__init__.py
--rw-r--r--   0 sjm        (501) staff       (20)     2121 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/actor_critic.py
--rw-r--r--   0 sjm        (501) staff       (20)     2802 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/policy.py
--rw-r--r--   0 sjm        (501) staff       (20)     2616 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/value.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.576163 modular_rl-0.2.3/modular_rl/params/
--rw-r--r--   0 sjm        (501) staff       (20)       82 2023-05-29 21:49:11.000000 modular_rl-0.2.3/modular_rl/params/__init__.py
--rw-r--r--   0 sjm        (501) staff       (20)     2124 2023-05-29 12:03:11.000000 modular_rl-0.2.3/modular_rl/params/mcis.py
--rw-r--r--   0 sjm        (501) staff       (20)     2305 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/params/mcts.py
--rw-r--r--   0 sjm        (501) staff       (20)     2015 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/params/ppo.py
--rw-r--r--   0 sjm        (501) staff       (20)     1248 2023-05-29 21:50:50.000000 modular_rl-0.2.3/modular_rl/settings.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.583572 modular_rl-0.2.3/modular_rl/tester/
--rw-r--r--   0 sjm        (501) staff       (20)       59 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/tester/__init__.py
--rw-r--r--   0 sjm        (501) staff       (20)      945 2023-05-30 12:20:33.000000 modular_rl-0.2.3/modular_rl/tester/mcis.py
--rw-r--r--   0 sjm        (501) staff       (20)      353 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/tester/mcts.py
--rw-r--r--   0 sjm        (501) staff       (20)     1505 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/tester/ppo.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.587074 modular_rl-0.2.3/modular_rl/util/
--rw-r--r--   0 sjm        (501) staff       (20)        0 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/util/__init__.py
--rw-r--r--   0 sjm        (501) staff       (20)     2468 2023-05-30 11:09:00.000000 modular_rl-0.2.3/modular_rl/util/node.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.549749 modular_rl-0.2.3/modular_rl.egg-info/
--rw-r--r--   0 sjm        (501) staff       (20)     5305 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/PKG-INFO
--rw-r--r--   0 sjm        (501) staff       (20)      893 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/SOURCES.txt
--rw-r--r--   0 sjm        (501) staff       (20)        1 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/dependency_links.txt
--rw-r--r--   0 sjm        (501) staff       (20)       26 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/requires.txt
--rw-r--r--   0 sjm        (501) staff       (20)       11 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/top_level.txt
--rw-r--r--   0 sjm        (501) staff       (20)     1414 2023-05-29 21:51:26.000000 modular_rl-0.2.3/pyproject.toml
--rw-r--r--   0 sjm        (501) staff       (20)       38 2023-05-30 13:36:16.599360 modular_rl-0.2.3/setup.cfg
--rw-r--r--   0 sjm        (501) staff       (20)      937 2023-05-29 21:51:36.000000 modular_rl-0.2.3/setup.py
-drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.594842 modular_rl-0.2.3/tests/
--rw-r--r--   0 sjm        (501) staff       (20)       93 2023-05-29 21:52:50.000000 modular_rl-0.2.3/tests/test_mcis.py
--rw-r--r--   0 sjm        (501) staff       (20)      101 2023-05-30 12:23:04.000000 modular_rl-0.2.3/tests/test_mcis_modular.py
--rw-r--r--   0 sjm        (501) staff       (20)       93 2023-05-13 00:53:55.000000 modular_rl-0.2.3/tests/test_mcts.py
--rw-r--r--   0 sjm        (501) staff       (20)       58 2023-05-13 00:53:55.000000 modular_rl-0.2.3/tests/test_ppo.py
--rw-r--r--   0 sjm        (501) staff       (20)       66 2023-05-13 00:53:55.000000 modular_rl-0.2.3/tests/test_ppo_modular.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.139493 modular_rl-0.3.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5465 2023-06-06 22:29:53.138484 modular_rl-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4099 2023-06-04 21:09:01.000000 modular_rl-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.078710 modular_rl-0.3.0/modular_rl/
+-rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.099473 modular_rl-0.3.0/modular_rl/agents/
+-rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.0/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0     9544 2023-06-06 21:33:56.000000 modular_rl-0.3.0/modular_rl/agents/_agent.py
+-rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.0/modular_rl/agents/_custom.py
+-rw-rw-rw-   0        0        0    12360 2023-06-06 21:42:41.000000 modular_rl-0.3.0/modular_rl/agents/mcis.py
+-rw-rw-rw-   0        0        0    11964 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    20686 2023-06-06 22:24:07.000000 modular_rl-0.3.0/modular_rl/agents/mim.py
+-rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.0/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.100701 modular_rl-0.3.0/modular_rl/envs/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.105921 modular_rl-0.3.0/modular_rl/envs/mim/
+-rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/mim/__init__.py
+-rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/mim/card_evaluator.py
+-rw-rw-rw-   0        0        0     4474 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/envs/mim/mim.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.111871 modular_rl-0.3.0/modular_rl/networks/
+-rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/networks/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/networks/actor_critic.py
+-rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.0/modular_rl/networks/policy.py
+-rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.0/modular_rl/networks/value.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.118471 modular_rl-0.3.0/modular_rl/params/
+-rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/params/mcis.py
+-rw-rw-rw-   0        0        0     2345 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0      975 2023-06-06 21:47:23.000000 modular_rl-0.3.0/modular_rl/params/mim.py
+-rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1352 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.125524 modular_rl-0.3.0/modular_rl/tester/
+-rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/tester/__init__.py
+-rw-rw-rw-   0        0        0      978 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/tester/mcis.py
+-rw-rw-rw-   0        0        0      366 2023-05-07 14:51:41.000000 modular_rl-0.3.0/modular_rl/tester/mcts.py
+-rw-rw-rw-   0        0        0      323 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/tester/mim.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.3.0/modular_rl/tester/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.128026 modular_rl-0.3.0/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.0/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.0/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.086917 modular_rl-0.3.0/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     5465 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 22:29:52.000000 modular_rl-0.3.0/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-06-06 21:24:49.000000 modular_rl-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 22:29:53.139493 modular_rl-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-06-06 21:25:01.000000 modular_rl-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:29:53.136420 modular_rl-0.3.0/tests/
+-rw-rw-rw-   0        0        0       97 2023-06-04 21:09:01.000000 modular_rl-0.3.0/tests/test_mcis.py
+-rw-rw-rw-   0        0        0      105 2023-06-04 21:09:01.000000 modular_rl-0.3.0/tests/test_mcis_modular.py
+-rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.3.0/tests/test_mcts.py
+-rw-rw-rw-   0        0        0      107 2023-06-04 21:09:01.000000 modular_rl-0.3.0/tests/test_mim.py
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.3.0/tests/test_ppo.py
+-rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.3.0/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.2.3/LICENSE` & `modular_rl-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 horrible-gh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 horrible-gh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `modular_rl-0.2.3/PKG-INFO` & `modular_rl-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-Metadata-Version: 2.1
-Name: modular_rl
-Version: 0.2.3
-Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-Home-page: https://github.com/horrible-gh/ModularRL
-Author: sjm
-Author-email: horrible <shinjpn1@gmail.com>
-Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
-Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
-Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
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
+Metadata-Version: 2.1
+Name: modular_rl
+Version: 0.3.0
+Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+Home-page: https://github.com/horrible-gh/ModularRL
+Author: sjm
+Author-email: horrible <shinjpn1@gmail.com>
+Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
+Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
+Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
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
+    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (Modular)
+-   AgentMCTS
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
+-   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.2.3/README.md` & `modular_rl-0.3.0/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,136 +1,136 @@
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
+    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (Modular)
+-   AgentMCTS
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
+-   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.2.3/modular_rl/agents/_agent.py` & `modular_rl-0.3.0/modular_rl/agents/_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible-gh
 
-Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
-It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
-and sets various learning parameters.
-It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
-save and load a checkpoint, and reset learning parameters.
-The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms.
+The library is designed to be easily customizable and modular,
+allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 
 This software includes the following third-party libraries:
 Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
 NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
 PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
 """
 
@@ -46,15 +43,15 @@
         self.value_optimizer = None
 
         self.actor_critic_net = None
         self.actor_critic_optimizer = None
 
         # Training parameters(Common)
         self.max_episodes = setting.get('max_episodes', 30)
-        self.max_timesteps = setting.get('max_timesteps', 1000)
+        self.max_timesteps = setting.get('max_timesteps', 100)
         self.update_timestep = setting.get('update_timestep', 200)
         self.gamma = setting.get('gamma', 0.99)
         self.early_stop_threshold = setting.get('early_stop_threshold', -1)
         self.done_loop_end = setting.get('done_loop_end', False)
 
         # Set learn episode parameters
         self.episode_reward = 0
@@ -130,15 +127,14 @@
         '''
 
         state_num = len(state)
         if state_num == 2:
             state, _ = state  # Unpack the tuple
         return state
 
-
     def learn_reset(self):
         """
         Reset the agent's state and episode reward.
         """
 
         self.state = self.env.reset()
         return self._check_state(self.state)
@@ -245,15 +241,15 @@
         step_output_num = len(step_output)
         if step_output_num == 4:
             next_state, reward, is_done, _ = step_output
         elif step_output_num == 5:
             next_state, reward, is_done, _, _ = step_output
         return next_state, reward, is_done
 
-    def update_reward(self, reward) :
+    def update_reward(self, reward):
         self.episode_reward += reward
         self.total_reward += reward
         self.prev_reward = reward
 
     def update_episode(self):
         self.episode += 1
         self.episode_reward = 0
```

### Comparing `modular_rl-0.2.3/modular_rl/agents/mcis.py` & `modular_rl-0.3.0/modular_rl/agents/mcis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 
-import gym
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentMCIS is an implementation of the Monte Carlo Importance Sampling (MCIS) algorithm.
+The algorithm is used for solving problems of sequential decision making under uncertainty.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+This class has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+
+Importance Sampling is used to estimate the properties of a particular target distribution, given some observed data and a proposal distribution.
+This implementation makes use of Monte Carlo methods, which rely on repeated random sampling to obtain numerical results.
+
+This software includes the following third-party libraries:
+Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+PyTorch (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+"""
+
 import torch
-import torch.optim as optim
 from torch.distributions import Categorical
 import torch.nn.functional as F
-from modular_rl.networks.actor_critic import ActorCriticNetwork
 from modular_rl.util.node import Node
 from modular_rl.agents._agent import Agent
-from LogAssist.log import Logger
 import numpy as np
 
+
 class AgentMCIS(Agent):
     def __init__(self, env, setting):
         """
         Initialize the AgentMCIS class with the specified environment and settings.
 
         :param env: The environment to use for training.
         :type env: gym.Env or None
@@ -33,15 +52,14 @@
         if self.device == None:
             self.device = torch.device(
                 "cuda" if torch.cuda.is_available() else "cpu")
 
         # Save selected learning data separately
         # self.state_tensor
 
-
     def update_step(self, state, action, reward, done, next_state):
         """
         Updates the provided state, action, reward, done, and next_state.
 
         :param state: The current state of the environment.
         :type state: numpy.ndarray
         :param action: The action taken by the agent.
@@ -93,22 +111,21 @@
                 state_tensor = self.check_tensor(node.state).to(self.device)
                 action_probs, value = self.actor_critic_net(state_tensor)
                 action_space = self.env.action_space.n
                 node.expand(action_space, action_probs, False)
             state_tensor = self.check_tensor(node.state).to(self.device)
             _, value = self.actor_critic_net(state_tensor)
             self.backpropagate(search_path, value.item(), node.done)
-        root_state_tensor = self.check_tensor(root.state).to(self.device)  # This line is added
+        root_state_tensor = self.check_tensor(
+            root.state).to(self.device)  # This line is added
         action_probs, _ = self.actor_critic_net(root_state_tensor)
-        chosen_action = np.random.choice(range(len(action_probs)), p=action_probs.detach().numpy())
+        chosen_action = np.random.choice(
+            range(len(action_probs)), p=action_probs.detach().numpy())
         return chosen_action
 
-
-
-
     def backpropagate(self, search_path, reward, done):
         """
         Backpropagate the value estimates back to the root node.
 
         :param search_path: The nodes visited during the search.
         :type search_path: list of Node
         :param reward: The reward obtained after the search.
@@ -119,15 +136,14 @@
         for node in reversed(search_path):
             node.update_stats(reward)
             if not done:
                 state_tensor = self.check_tensor(node.state).to(self.device)
                 _, reward = self.actor_critic_net(state_tensor)
                 reward = reward.item()
 
-
     def learn(self):
         """
         Train the agent.
         """
         self.train()
 
     def train(self):
@@ -159,15 +175,14 @@
                     self.learn_check()
                     break
 
                 state = next_state
 
             self.episode += 1
 
-
     def compute_loss(self, state, action, reward, next_state, done):
         '''
         This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
         The actor loss is computed based on the policy gradient algorithm,
         and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
 
         compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
@@ -185,23 +200,23 @@
         :param done: A flag indicating whether the episode has ended.
         :return: The computed actor and critic loss values.
         '''
 
         # Predict action probabilities and values
         action_probs, values = self.actor_critic_net(state)
 
-        #Logger.verb('agents:mcis:compute_loss',f'{self.actor_critic_net(next_state)}')
+        # Logger.verb('agents:mcis:compute_loss',f'{self.actor_critic_net(next_state)}')
 
         # Compute the value loss
         actor_output, critic_output = self.actor_critic_net(next_state)
-        target_values = reward + self.gamma * torch.mean(critic_output) * (1 - done)
+        target_values = reward + self.gamma * \
+            torch.mean(critic_output) * (1 - done)
         target_values = target_values.unsqueeze(1)
         critic_loss = F.mse_loss(values, target_values.detach())
 
-
         # Compute the policy loss
         m = Categorical(action_probs)
         logprobs = m.log_prob(self.check_tensor(action))
         actor_loss = -logprobs * (target_values - values).detach()
 
         # Take mean of actor_loss and critic_loss
         actor_loss = actor_loss.mean()
@@ -213,25 +228,28 @@
         """
         This function updates the network parameters using the optimizer and computed loss values.
         """
 
         if not self.states:  # Check if the states list is empty
             return
 
-        #Logger.verb('agents:mcis:update',f'states={self.states},actions={self.actions},rewards={self.rewards},dones={self.dones}')
+        # Logger.verb('agents:mcis:update',f'states={self.states},actions={self.actions},rewards={self.rewards},dones={self.dones}')
 
         # Prepare data
-        states_tensor = torch.stack([self.check_tensor(state) for state in self.states]).to(self.device)
+        states_tensor = torch.stack(
+            [self.check_tensor(state) for state in self.states]).to(self.device)
         actions_tensor = torch.Tensor(self.actions).to(self.device)
         rewards_tensor = torch.Tensor(self.rewards).to(self.device)
-        next_states_tensor = torch.stack([self.check_tensor(state) for state in self.next_states]).to(self.device)
+        next_states_tensor = torch.stack(
+            [self.check_tensor(state) for state in self.next_states]).to(self.device)
         dones_tensor = torch.Tensor(self.dones).to(self.device)
 
         # Compute loss
-        actor_loss, critic_loss = self.compute_loss(states_tensor, actions_tensor, rewards_tensor, next_states_tensor, dones_tensor)
+        actor_loss, critic_loss = self.compute_loss(
+            states_tensor, actions_tensor, rewards_tensor, next_states_tensor, dones_tensor)
 
         # Compute gradients and update network parameters
         self.actor_critic_optimizer.zero_grad()
         loss = actor_loss + critic_loss
         loss.backward()
         self.actor_critic_optimizer.step()
```

### Comparing `modular_rl-0.2.3/modular_rl/agents/mcts.py` & `modular_rl-0.3.0/modular_rl/agents/mcts.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
-It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
-and sets various learning parameters.
-It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
-save and load a checkpoint, and reset learning parameters.
-The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
-
-This software includes the following third-party libraries:
-Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-"""
-
-import gym
-import torch
-import torch.optim as optim
-from torch.distributions import Categorical
-import torch.nn.functional as F
-from modular_rl.networks.actor_critic import ActorCriticNetwork
-from modular_rl.util.node import Node
-from modular_rl.agents._agent import Agent
-from LogAssist.log import Logger
-
-
-class AgentMCTS(Agent):
-    def __init__(self, env, setting):
-        """
-        Initialize the AgentMCTS class with the specified environment and settings.
-
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the MCTS algorithm.
-        :type setting: AgentSettings
-        """
-
-        super().__init__(env, setting)
-        super().init_actor_critic()
-
-        # MCTS parameters
-        self.num_simulations = setting.get('num_simulations', 800)
-        self.cpuct = setting.get('cpuct', 1.0)
-        self.temperature = setting.get('temperature', 1.0)
-
-        self.device = setting.get('device', None)
-        if self.device == None:
-            self.device = torch.device(
-                "cuda" if torch.cuda.is_available() else "cpu")
-
-        # Save selected learning data separately
-        # self.state_tensor
-
-    def select_action(self, state):
-        """
-        Select an action using MCTS.
-
-        :param state: The current state.
-        :type state: numpy.ndarray
-        :return: The selected action.
-        :rtype: int
-        """
-
-        state_tensor = self.check_tensor(self._check_state(state))
-        action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = action_probs.detach().numpy().flatten()
-        root = Node(state, action_probs)
-        Logger.verb(
-            'agents:mcts:select_action:self.num_simulations', self.num_simulations)
-        Logger.verb(
-            'agents:mcts:select_action:root', root)
-        Logger.verb(
-            'agents:mcts:select_action:action_probs', action_probs)
-        Logger.verb('agents:mcts:select_action:node', f'Root node: {root}')
-        for _ in range(self.num_simulations):
-            node = root
-            search_path = [node]
-            # Logger.verb(
-            #    'agents:mcts:select_action:search_path', search_path)
-            # Selection
-            while node.expanded():
-                action, node = node.select_child(self.cpuct)
-                search_path.append(node)
-            Logger.verb('agents:mcts:select_action:After selection',
-                        f' {search_path[-1]}')
-
-            # Expansion
-            if len(search_path) > 1:
-                parent, action = search_path[-2], search_path[-1].action
-            else:
-                # or some other suitable defaults
-                parent, action = search_path[0], None
-
-            # Logger.verb('mcts:select_action:action', action)
-            step_output = self.env.step(action) if action is not None else (
-                parent.state, 0, False, None)
-            step_output_num = len(step_output)
-
-            if step_output_num == 4:
-                state, reward, done, _ = step_output
-            elif step_output_num == 5:
-                state, reward, done, _, _ = step_output
-
-            if not done:
-                # Logger.verb(
-                #    'agents:mcts:select_action:state', state)
-                if not torch.is_tensor(state):
-                    state_tensor = torch.from_numpy(
-                        state).float().to(self.device)
-                else:
-                    state_tensor = state.to(self.device)
-
-                action_probs, value = self.actor_critic_net(state_tensor)
-                action_space = self.env.action_space.n
-                node.expand(action_space, action_probs)
-
-            # Backpropagation
-            self.backpropagate(search_path, reward, done)
-
-        chosen_action = root.select_action(self.temperature)
-        chosen_action_reward = root.children[chosen_action].total_value
-        chosen_action_state = root.children[chosen_action].state
-        # Assuming that a non-zero reward indicates a terminal state
-        done = (chosen_action_reward != 0)
-
-        # Save selected learning data separately
-        self.state = chosen_action_state
-        self.action = chosen_action
-        self.reward = chosen_action_reward
-        self.done = done
-
-        self.total_reward += reward
-        self.prev_reward = reward
-
-        return chosen_action_state, chosen_action, chosen_action_reward, done
-
-    def backpropagate(self, search_path, reward, done):
-        """
-        Backpropagate the value estimates back to the root node.
-
-        :param search_path: The nodes visited during the search.
-        :type search_path: list of Node
-        :param reward: The reward obtained after the search.
-        :type reward: float
-        :param done: Whether the episode has ended.
-        :type done: bool
-        """
-        for node in reversed(search_path):
-            node.update_stats(reward)
-            if not done:
-                _, reward = self.actor_critic_net(node.state)
-                reward = reward.item()
-
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.train()
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-            # state = self.env.reset()
-
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-                self.state_tensor = self.check_tensor(state).squeeze(0)
-                self.next_state, self.action, self.reward, self.done = self.select_action(
-                    self.state_tensor)
-
-                self.learn_check()
-
-                if self.done:
-                    # self.update()
-                    break
-
-                self.update()
-
-                state = self.next_state
-
-            self.episode += 1
-            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
-
-    def compute_loss(self, state, action, reward, next_state, done):
-        '''
-        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
-        The actor loss is computed based on the policy gradient algorithm,
-        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
-
-        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
-
-        The state parameter is the current state of the environment.
-        The action parameter is the action taken in the current state.
-        The reward parameter is the reward received for taking the action in the current state.
-        The next_state parameter is the state resulting from taking the action in the current state.
-        The done parameter is a flag indicating whether the episode has ended.
-
-        :param state: The current state of the environment.
-        :param action: The action taken in the current state.
-        :param reward: The reward received for taking the action in the current state.
-        :param next_state: The state resulting from taking the action in the current state.
-        :param done: A flag indicating whether the episode has ended.
-        :return: The computed actor and critic loss values.
-        '''
-
-        # Predict action probabilities and values
-        action_probs, values = self.actor_critic_net(state)
-
-        # Compute the value loss
-        target_values = reward + self.gamma * \
-            self.actor_critic_net(next_state)[1] * (1 - done)
-        critic_loss = F.mse_loss(values, target_values.detach())
-
-        # Compute the policy loss
-        m = Categorical(action_probs)
-        logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * (target_values - values).detach()
-
-        return actor_loss, critic_loss
-
-    def update(self):
-        '''
-        This function updates the network parameters using the optimizer and computed loss values.
-
-        update() function updates the network parameters using the optimizer and computed loss values.
-        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
-
-        This function does not take any parameters and does not return anything.
-
-        :return: None
-        '''
-
-        # Update the network
-        self.actor_critic_optimizer.zero_grad()
-        actor_loss, critic_loss = self.compute_loss(
-            self.state_tensor, self.action, self.reward, self.next_state, self.done)
-        loss = actor_loss + critic_loss
-        loss.backward()
-        self.actor_critic_optimizer.step()
-
-    def check_tensor(self, obj):
-        '''
-        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
-
-        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
-        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
-        If it is already a tensor, it simply returns the tensor.
-
-        The obj parameter is the object to check/convert to a PyTorch tensor.
-
-        The function returns the input object as a PyTorch tensor.
-
-        :param obj: The object to check/convert to a PyTorch tensor.
-        :return: The input object as a PyTorch tensor.
-        '''
-
-        if not torch.is_tensor(obj):
-            obj_tensor = torch.FloatTensor(obj)
-        else:
-            obj_tensor = obj
-        return obj_tensor
-
-    def save_model(self, file_name):
-        """
-        This function saves the model to the specified file.
-
-        :param file_name: The name of the file to save the model to.
-        :return: None
-        """
-        self.save(file_name)
-
-    def save(self, file_name):
-        """
-        This function saves the actor critic network to the specified file.
-
-        :param file_name: The name of the file to save the actor critic network to.
-        :return: None
-        """
-
-        self.save_actor_critic(file_name)
-
-    def load_model(self, file_name):
-        """
-        This function loads the model from the specified file.
-
-        :param file_name: The name of the file to load the model from.
-        :return: None
-        """
-        self.load(file_name)
-
-    def load(self, file_name):
-        """
-        This function loads the actor critic network from the specified file.
-
-        :param file_name: The name of the file to load the actor critic network from.
-        :return: None
-        """
-
-        self.load_actor_critic(file_name)
+
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+
+This software includes the following third-party libraries:
+Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+"""
+
+import gym
+import torch
+import torch.optim as optim
+from torch.distributions import Categorical
+import torch.nn.functional as F
+from modular_rl.networks.actor_critic import ActorCriticNetwork
+from modular_rl.util.node import Node
+from modular_rl.agents._agent import Agent
+from LogAssist.log import Logger
+
+
+class AgentMCTS(Agent):
+    def __init__(self, env, setting):
+        """
+        Initialize the AgentMCTS class with the specified environment and settings.
+
+        :param env: The environment to use for training.
+        :type env: gym.Env or None
+        :param setting: The settings for the MCTS algorithm.
+        :type setting: AgentSettings
+        """
+
+        super().__init__(env, setting)
+        super().init_actor_critic()
+
+        # MCTS parameters
+        self.num_simulations = setting.get('num_simulations', 800)
+        self.cpuct = setting.get('cpuct', 1.0)
+        self.temperature = setting.get('temperature', 1.0)
+
+        self.device = setting.get('device', None)
+        if self.device == None:
+            self.device = torch.device(
+                "cuda" if torch.cuda.is_available() else "cpu")
+
+        # Save selected learning data separately
+        # self.state_tensor
+
+    def select_action(self, state):
+        """
+        Select an action using MCTS.
+
+        :param state: The current state.
+        :type state: numpy.ndarray
+        :return: The selected action.
+        :rtype: int
+        """
+
+        state_tensor = self.check_tensor(self._check_state(state))
+        action_probs, _ = self.actor_critic_net(state_tensor)
+        action_probs = action_probs.detach().numpy().flatten()
+        root = Node(state, action_probs)
+        Logger.verb(
+            'agents:mcts:select_action:self.num_simulations', self.num_simulations)
+        Logger.verb(
+            'agents:mcts:select_action:root', root)
+        Logger.verb(
+            'agents:mcts:select_action:action_probs', action_probs)
+        Logger.verb('agents:mcts:select_action:node', f'Root node: {root}')
+        for _ in range(self.num_simulations):
+            node = root
+            search_path = [node]
+            # Logger.verb(
+            #    'agents:mcts:select_action:search_path', search_path)
+            # Selection
+            while node.expanded():
+                action, node = node.select_child(self.cpuct)
+                search_path.append(node)
+            Logger.verb('agents:mcts:select_action:After selection',
+                        f' {search_path[-1]}')
+
+            # Expansion
+            if len(search_path) > 1:
+                parent, action = search_path[-2], search_path[-1].action
+            else:
+                # or some other suitable defaults
+                parent, action = search_path[0], None
+
+            # Logger.verb('mcts:select_action:action', action)
+            step_output = self.env.step(action) if action is not None else (
+                parent.state, 0, False, None)
+            step_output_num = len(step_output)
+
+            if step_output_num == 4:
+                state, reward, done, _ = step_output
+            elif step_output_num == 5:
+                state, reward, done, _, _ = step_output
+
+            if not done:
+                # Logger.verb(
+                #    'agents:mcts:select_action:state', state)
+                if not torch.is_tensor(state):
+                    state_tensor = torch.from_numpy(
+                        state).float().to(self.device)
+                else:
+                    state_tensor = state.to(self.device)
+
+                action_probs, value = self.actor_critic_net(state_tensor)
+                action_space = self.env.action_space.n
+                node.expand(action_space, action_probs)
+
+            # Backpropagation
+            self.backpropagate(search_path, reward, done)
+
+        chosen_action = root.select_action(self.temperature)
+        chosen_action_reward = root.children[chosen_action].total_value
+        chosen_action_state = root.children[chosen_action].state
+        # Assuming that a non-zero reward indicates a terminal state
+        done = (chosen_action_reward != 0)
+
+        # Save selected learning data separately
+        self.state = chosen_action_state
+        self.action = chosen_action
+        self.reward = chosen_action_reward
+        self.done = done
+
+        self.total_reward += reward
+        self.prev_reward = reward
+
+        return chosen_action_state, chosen_action, chosen_action_reward, done
+
+    def backpropagate(self, search_path, reward, done):
+        """
+        Backpropagate the value estimates back to the root node.
+
+        :param search_path: The nodes visited during the search.
+        :type search_path: list of Node
+        :param reward: The reward obtained after the search.
+        :type reward: float
+        :param done: Whether the episode has ended.
+        :type done: bool
+        """
+        for node in reversed(search_path):
+            node.update_stats(reward)
+            if not done:
+                _, reward = self.actor_critic_net(node.state)
+                reward = reward.item()
+
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.train()
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+            # state = self.env.reset()
+
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+                self.state_tensor = self.check_tensor(state).squeeze(0)
+                self.next_state, self.action, self.reward, self.done = self.select_action(
+                    self.state_tensor)
+
+                self.learn_check()
+
+                if self.done:
+                    # self.update()
+                    break
+
+                self.update()
+
+                state = self.next_state
+
+            self.episode += 1
+            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
+
+    def compute_loss(self, state, action, reward, next_state, done):
+        '''
+        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
+        The actor loss is computed based on the policy gradient algorithm,
+        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
+
+        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
+
+        The state parameter is the current state of the environment.
+        The action parameter is the action taken in the current state.
+        The reward parameter is the reward received for taking the action in the current state.
+        The next_state parameter is the state resulting from taking the action in the current state.
+        The done parameter is a flag indicating whether the episode has ended.
+
+        :param state: The current state of the environment.
+        :param action: The action taken in the current state.
+        :param reward: The reward received for taking the action in the current state.
+        :param next_state: The state resulting from taking the action in the current state.
+        :param done: A flag indicating whether the episode has ended.
+        :return: The computed actor and critic loss values.
+        '''
+
+        # Predict action probabilities and values
+        action_probs, values = self.actor_critic_net(state)
+
+        # Compute the value loss
+        target_values = reward + self.gamma * \
+            self.actor_critic_net(next_state)[1] * (1 - done)
+        critic_loss = F.mse_loss(values, target_values.detach())
+
+        # Compute the policy loss
+        m = Categorical(action_probs)
+        logprobs = m.log_prob(self.check_tensor(action))
+        actor_loss = -logprobs * (target_values - values).detach()
+
+        return actor_loss, critic_loss
+
+    def update(self):
+        '''
+        This function updates the network parameters using the optimizer and computed loss values.
+
+        update() function updates the network parameters using the optimizer and computed loss values.
+        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
+
+        This function does not take any parameters and does not return anything.
+
+        :return: None
+        '''
+
+        # Update the network
+        self.actor_critic_optimizer.zero_grad()
+        actor_loss, critic_loss = self.compute_loss(
+            self.state_tensor, self.action, self.reward, self.next_state, self.done)
+        loss = actor_loss + critic_loss
+        loss.backward()
+        self.actor_critic_optimizer.step()
+
+    def check_tensor(self, obj):
+        '''
+        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
+
+        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
+        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
+        If it is already a tensor, it simply returns the tensor.
+
+        The obj parameter is the object to check/convert to a PyTorch tensor.
+
+        The function returns the input object as a PyTorch tensor.
+
+        :param obj: The object to check/convert to a PyTorch tensor.
+        :return: The input object as a PyTorch tensor.
+        '''
+
+        if not torch.is_tensor(obj):
+            obj_tensor = torch.FloatTensor(obj)
+        else:
+            obj_tensor = obj
+        return obj_tensor
+
+    def save_model(self, file_name):
+        """
+        This function saves the model to the specified file.
+
+        :param file_name: The name of the file to save the model to.
+        :return: None
+        """
+        self.save(file_name)
+
+    def save(self, file_name):
+        """
+        This function saves the actor critic network to the specified file.
+
+        :param file_name: The name of the file to save the actor critic network to.
+        :return: None
+        """
+
+        self.save_actor_critic(file_name)
+
+    def load_model(self, file_name):
+        """
+        This function loads the model from the specified file.
+
+        :param file_name: The name of the file to load the model from.
+        :return: None
+        """
+        self.load(file_name)
+
+    def load(self, file_name):
+        """
+        This function loads the actor critic network from the specified file.
+
+        :param file_name: The name of the file to load the actor critic network from.
+        :return: None
+        """
+
+        self.load_actor_critic(file_name)
```

### Comparing `modular_rl-0.2.3/modular_rl/agents/ppo.py` & `modular_rl-0.3.0/modular_rl/agents/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,16 @@
 This software includes the following third-party libraries:
 Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
 NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
 PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
 """
 
 import torch
-import torch.optim as optim
 from torch.distributions import Categorical
 import numpy as np
-from modular_rl.networks.policy import PolicyNetwork
-from modular_rl.networks.value import ValueNetwork
 from modular_rl.agents._agent import Agent
 from LogAssist.log import Logger
 
 
 class AgentPPO(Agent):
     def __init__(self, env, setting):
         """
@@ -318,15 +315,14 @@
                 if self.episode + 1 >= self.max_episodes:
                     break
 
             self.env.close()
         else:
             self.reset()
 
-
     def learn_next(self):
         """
         Perform a single learning step and update the episode and total rewards.
 
         :return: The action taken, the resulting reward, and whether the episode is done or not.
         :rtype: tuple(torch.Tensor, float, bool)
         """
```

### Comparing `modular_rl-0.2.3/modular_rl/networks/actor_critic.py` & `modular_rl-0.3.0/modular_rl/networks/actor_critic.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible
-
-This software includes the following third-party libraries:
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-
-"""
-import torch.nn as nn
-
-
-class ActorCriticNetwork(nn.Module):
-    def __init__(self, state_dim, action_dim, hidden_size=256):
-        '''
-        This code defines a class ActorCriticNetwork that implements an actor-critic network using PyTorch.
-        The actor-critic algorithm is a popular reinforcement learning algorithm that is used to learn how to maximize rewards in an environment by having an agent interact with the environment.
-        This network takes as input the state and action dimensions, and the number of neurons in the hidden layers of both the actor and critic networks.
-        It then predicts state-value and action-value for the given input.
-
-        :param state_dim: (int) The dimensionality of the state space.
-        :param action_dim: (int) The dimensionality of the action space.
-        :param hidden_size: (int) The number of neurons in the hidden layers of both the actor and critic networks.
-        '''
-
-        super(ActorCriticNetwork, self).__init__()
-
-        # Actor network
-        self.actor = nn.Sequential(
-            nn.Linear(state_dim, hidden_size),
-            nn.ReLU(),
-            nn.Linear(hidden_size, action_dim),
-            nn.Softmax(dim=-1)
-        )
-
-        # Critic network
-        self.critic = nn.Sequential(
-            nn.Linear(state_dim, hidden_size),
-            nn.ReLU(),
-            nn.Linear(hidden_size, 1)
-        )
-
-    def forward(self, state):
-        '''
-        The forward method of this class takes a state tensor of shape (batch_size, state_dim) as input and returns the action probabilities and state value.
-        The :param comments provide additional information about the inputs to the functions.
-
-        :param state: (tensor) The input state tensor of shape (batch_size, state_dim).
-        '''
-        action_probs = self.actor(state)
-        value = self.critic(state)
-        return action_probs, value
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible
+
+This software includes the following third-party libraries:
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+
+"""
+import torch.nn as nn
+
+
+class ActorCriticNetwork(nn.Module):
+    def __init__(self, state_dim, action_dim, hidden_size=256):
+        '''
+        This code defines a class ActorCriticNetwork that implements an actor-critic network using PyTorch.
+        The actor-critic algorithm is a popular reinforcement learning algorithm that is used to learn how to maximize rewards in an environment by having an agent interact with the environment.
+        This network takes as input the state and action dimensions, and the number of neurons in the hidden layers of both the actor and critic networks.
+        It then predicts state-value and action-value for the given input.
+
+        :param state_dim: (int) The dimensionality of the state space.
+        :param action_dim: (int) The dimensionality of the action space.
+        :param hidden_size: (int) The number of neurons in the hidden layers of both the actor and critic networks.
+        '''
+
+        super(ActorCriticNetwork, self).__init__()
+
+        # Actor network
+        self.actor = nn.Sequential(
+            nn.Linear(state_dim, hidden_size),
+            nn.ReLU(),
+            nn.Linear(hidden_size, action_dim),
+            nn.Softmax(dim=-1)
+        )
+
+        # Critic network
+        self.critic = nn.Sequential(
+            nn.Linear(state_dim, hidden_size),
+            nn.ReLU(),
+            nn.Linear(hidden_size, 1)
+        )
+
+    def forward(self, state):
+        '''
+        The forward method of this class takes a state tensor of shape (batch_size, state_dim) as input and returns the action probabilities and state value.
+        The :param comments provide additional information about the inputs to the functions.
+
+        :param state: (tensor) The input state tensor of shape (batch_size, state_dim).
+        '''
+        action_probs = self.actor(state)
+        value = self.critic(state)
+        return action_probs, value
```

### Comparing `modular_rl-0.2.3/modular_rl/networks/policy.py` & `modular_rl-0.3.0/modular_rl/networks/value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,72 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible
-
-PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
-The purpose of this network is to determine the best action to take in the current state.
-
-ValueNetwork, on the other hand, 
-is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
-The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
-
-Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
-which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
-
-This software includes the following third-party libraries:
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-
-"""
-import torch.nn as nn
-import torch
-
-
-class PolicyNetwork(nn.Module):
-    def __init__(self, input_dim, output_dim, hidden_option='medium', num_layers=2):
-        """
-        Initialize the PolicyNetwork class with the specified input dimension, output dimension, and network settings.
-
-        :param input_dim: The dimension of the input layer.
-        :type input_dim: int
-        :param output_dim: The dimension of the output layer.
-        :type output_dim: int
-        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
-        :type hidden_option: str
-        :param num_layers: The number of hidden layers.
-        :type num_layers: int
-        """
-
-        super(PolicyNetwork, self).__init__()
-
-        hidden_dim_map = {
-            'small': 32,
-            'medium': 64,
-            'large': 128,
-            'huge': 256,
-            'exhuge': 512
-        }
-
-        hidden_dim = hidden_dim_map[hidden_option]
-
-        # Create each layer
-        layers = []
-        for i in range(num_layers):
-            if i == 0:
-                layers.append(nn.Linear(input_dim, hidden_dim))
-            elif i == num_layers - 1:
-                layers.append(nn.Linear(hidden_dim, output_dim))
-            else:
-                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
-            layers.append(nn.ReLU())
-        self.net = nn.Sequential(*layers)
-
-    def forward(self, x):
-        """
-        Compute a forward pass of the policy network.
-
-        :param x: The input tensor.
-        :type x: torch.Tensor
-        :return: The output tensor.
-        :rtype: torch.Tensor
-        """
-
-        x = self.net(x)
-        x = torch.softmax(x, dim=-1)
-        return x
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible
+
+PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
+The purpose of this network is to determine the best action to take in the current state.
+
+ValueNetwork, on the other hand, 
+is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
+The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
+
+Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
+which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
+
+This software includes the following third-party libraries:
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+
+"""
+import torch.nn as nn
+
+
+class ValueNetwork(nn.Module):
+    def __init__(self, input_dim, hidden_option='medium', num_layers=2):
+        """
+        Initialize the ValueNetwork class with the specified input dimension and network settings.
+
+        :param input_dim: The dimension of the input layer.
+        :type input_dim: int
+        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
+        :type hidden_option: str
+        :param num_layers: The number of hidden layers.
+        :type num_layers: int
+        """
+
+        super(ValueNetwork, self).__init__()
+
+        hidden_dim_map = {
+            'small': 32,
+            'medium': 64,
+            'large': 128,
+            'huge': 256,
+            'exhuge': 512
+        }
+
+        hidden_dim = hidden_dim_map[hidden_option]
+
+        # Create each layer
+        layers = []
+        for i in range(num_layers):
+            if i == 0:
+                layers.append(nn.Linear(input_dim, hidden_dim))
+            elif i == num_layers - 1:
+                layers.append(nn.Linear(hidden_dim, 1))
+            else:
+                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
+            layers.append(nn.ReLU())
+        self.net = nn.Sequential(*layers)
+
+    def forward(self, x):
+        """
+        Compute a forward pass of the value network.
+
+        :param x: The input tensor.
+        :type x: torch.Tensor
+        :return: The output tensor.
+        :rtype: torch.Tensor
+        """
+
+        x = self.net(x)
+        return x
```

### Comparing `modular_rl-0.2.3/modular_rl/networks/value.py` & `modular_rl-0.3.0/modular_rl/networks/policy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,76 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible
-
-PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
-The purpose of this network is to determine the best action to take in the current state.
-
-ValueNetwork, on the other hand, 
-is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
-The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
-
-Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
-which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
-
-This software includes the following third-party libraries:
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-
-"""
-import torch.nn as nn
-
-
-class ValueNetwork(nn.Module):
-    def __init__(self, input_dim, hidden_option='medium', num_layers=2):
-        """
-        Initialize the ValueNetwork class with the specified input dimension and network settings.
-
-        :param input_dim: The dimension of the input layer.
-        :type input_dim: int
-        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
-        :type hidden_option: str
-        :param num_layers: The number of hidden layers.
-        :type num_layers: int
-        """
-
-        super(ValueNetwork, self).__init__()
-
-        hidden_dim_map = {
-            'small': 32,
-            'medium': 64,
-            'large': 128,
-            'huge': 256,
-            'exhuge': 512
-        }
-
-        hidden_dim = hidden_dim_map[hidden_option]
-
-        # Create each layer
-        layers = []
-        for i in range(num_layers):
-            if i == 0:
-                layers.append(nn.Linear(input_dim, hidden_dim))
-            elif i == num_layers - 1:
-                layers.append(nn.Linear(hidden_dim, 1))
-            else:
-                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
-            layers.append(nn.ReLU())
-        self.net = nn.Sequential(*layers)
-
-    def forward(self, x):
-        """
-        Compute a forward pass of the value network.
-
-        :param x: The input tensor.
-        :type x: torch.Tensor
-        :return: The output tensor.
-        :rtype: torch.Tensor
-        """
-
-        x = self.net(x)
-        return x
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible
+
+PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
+The purpose of this network is to determine the best action to take in the current state.
+
+ValueNetwork, on the other hand, 
+is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
+The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
+
+Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
+which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
+
+This software includes the following third-party libraries:
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+
+"""
+import torch.nn as nn
+import torch
+
+
+class PolicyNetwork(nn.Module):
+    def __init__(self, input_dim, output_dim, hidden_option='medium', num_layers=2):
+        """
+        Initialize the PolicyNetwork class with the specified input dimension, output dimension, and network settings.
+
+        :param input_dim: The dimension of the input layer.
+        :type input_dim: int
+        :param output_dim: The dimension of the output layer.
+        :type output_dim: int
+        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
+        :type hidden_option: str
+        :param num_layers: The number of hidden layers.
+        :type num_layers: int
+        """
+
+        super(PolicyNetwork, self).__init__()
+
+        hidden_dim_map = {
+            'small': 32,
+            'medium': 64,
+            'large': 128,
+            'huge': 256,
+            'exhuge': 512
+        }
+
+        hidden_dim = hidden_dim_map[hidden_option]
+
+        # Create each layer
+        layers = []
+        for i in range(num_layers):
+            if i == 0:
+                layers.append(nn.Linear(input_dim, hidden_dim))
+            elif i == num_layers - 1:
+                layers.append(nn.Linear(hidden_dim, output_dim))
+            else:
+                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
+            layers.append(nn.ReLU())
+        self.net = nn.Sequential(*layers)
+
+    def forward(self, x):
+        """
+        Compute a forward pass of the policy network.
+
+        :param x: The input tensor.
+        :type x: torch.Tensor
+        :return: The output tensor.
+        :rtype: torch.Tensor
+        """
+
+        x = self.net(x)
+        x = torch.softmax(x, dim=-1)
+        return x
```

### Comparing `modular_rl-0.2.3/modular_rl/params/mcis.py` & `modular_rl-0.3.0/modular_rl/params/mcts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-class ParamMCIS:
-    default = {
-        'max_episodes': 10,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 10,  # Number of MCIS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCIS
-        'temperature': 1.0,  # Temperature for action selection during MCIS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 800,  # Number of MCIS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCIS
-        'temperature': 1.0,  # Temperature for action selection during MCIS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
+class ParamMCTS:
+    default = {
+        'max_episodes': 10,  # Maximum number of episodes for training
+        'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'update_timestep': 2000,  # Update the policy every specified timestep
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 10,  # Number of MCTS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
+
+    default_modular = {
+        # Maximum number of episodes for training (-1 for no limit)
+        'max_episodes': -1,
+        # Maximum number of timesteps for each episode (-1 for no limit)
+        'max_timesteps': -1,
+        # Update the policy every specified timestep (-1 for no limit)
+        'update_timestep': -1,
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 800,  # Number of MCTS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.2.3/modular_rl/params/mcts.py` & `modular_rl-0.3.0/modular_rl/params/mcis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-class ParamMCTS:
-    default = {
-        'max_episodes': 10,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'update_timestep': 2000,  # Update the policy every specified timestep
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 10,  # Number of MCTS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
-        # Update the policy every specified timestep (-1 for no limit)
-        'update_timestep': -1,
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 800,  # Number of MCTS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
+class ParamMCIS:
+    default = {
+        'max_episodes': 10,  # Maximum number of episodes for training
+        'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 10,  # Number of MCIS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCIS
+        'temperature': 1.0,  # Temperature for action selection during MCIS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
+
+    default_modular = {
+        # Maximum number of episodes for training (-1 for no limit)
+        'max_episodes': -1,
+        # Maximum number of timesteps for each episode (-1 for no limit)
+        'max_timesteps': -1,
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 800,  # Number of MCIS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCIS
+        'temperature': 1.0,  # Temperature for action selection during MCIS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.2.3/modular_rl/params/ppo.py` & `modular_rl-0.3.0/modular_rl/params/ppo.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-class ParamPPO:
-    default = {
-        'max_episodes': 30,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'update_timestep': 2000,  # Update the policy every specified timestep
-        'ppo_epochs': 4,  # Number of PPO epochs
-        'mini_batch_size': 64,  # Batch size for PPO updates
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'gamma': 0.99,  # Discount factor
-        'lam': 0.95,  # Lambda parameter for GAE
-        'clip_param': 0.2,  # Clipping parameter for PPO
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
-        # Update the policy every specified timestep (-1 for no limit)
-        'update_timestep': -1,
-        'ppo_epochs': 4,  # Number of PPO epochs
-        'mini_batch_size': 64,  # Batch size for PPO updates
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'gamma': 0.99,  # Discount factor
-        'lam': 0.95,  # Lambda parameter for GAE
-        'clip_param': 0.2,  # Clipping parameter for PPO
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
+class ParamPPO:
+    default = {
+        'max_episodes': 30,  # Maximum number of episodes for training
+        'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'update_timestep': 2000,  # Update the policy every specified timestep
+        'ppo_epochs': 4,  # Number of PPO epochs
+        'mini_batch_size': 64,  # Batch size for PPO updates
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'gamma': 0.99,  # Discount factor
+        'lam': 0.95,  # Lambda parameter for GAE
+        'clip_param': 0.2,  # Clipping parameter for PPO
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
+
+    default_modular = {
+        # Maximum number of episodes for training (-1 for no limit)
+        'max_episodes': -1,
+        # Maximum number of timesteps for each episode (-1 for no limit)
+        'max_timesteps': -1,
+        # Update the policy every specified timestep (-1 for no limit)
+        'update_timestep': -1,
+        'ppo_epochs': 4,  # Number of PPO epochs
+        'mini_batch_size': 64,  # Batch size for PPO updates
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'gamma': 0.99,  # Discount factor
+        'lam': 0.95,  # Lambda parameter for GAE
+        'clip_param': 0.2,  # Clipping parameter for PPO
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.2.3/modular_rl/settings.py` & `modular_rl-0.3.0/modular_rl/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
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
-
-
-class AgentSettings:
-    default_ppo = ParamPPO.default
-    default_ppo_modular = ParamPPO.default_modular
-    default_mcts = ParamMCTS.default
-    default_mcts_modular = ParamMCTS.default_modular
-    default_mcis = ParamMCIS.default
-    default_mcis_modular = ParamMCIS.default_modular
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
+class AgentSettings:
+    default_ppo = ParamPPO.default
+    default_ppo_modular = ParamPPO.default_modular
+    default_mcts = ParamMCTS.default
+    default_mcts_modular = ParamMCTS.default_modular
+    default_mcis = ParamMCIS.default
+    default_mcis_modular = ParamMCIS.default_modular
+    default_mim = ParamMIM.default
```

### Comparing `modular_rl-0.2.3/modular_rl/tester/ppo.py` & `modular_rl-0.3.0/modular_rl/tester/ppo.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# -*- coding: utf-8 -*-
-from modular_rl.agents.ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-'''
-This code is a Python script that initializes and trains an instance of the AgentPPO class with default settings using the init_ppo() function. 
-Additionally, the init_ppo_modular() function is provided to demonstrate the usage of the AgentPPO class with modified settings.
-
-In init_ppo_modular(), an instance of AgentPPO is created with a modified default_modular settings dictionary. 
-The function then calls various methods of the instance, such as reset(), learn_reset(), learn_next(), and update() to demonstrate the functionality of the class. 
-The instance is then saved to a file using the save_model() method, which is not shown in the provided code.
-
-'''
-
-
-def init_ppo():
-    env = AgentPPO(env=None, setting=AgentSettings.default_ppo)
-    env.learn()
-
-
-def init_ppo_modular():
-    env = AgentPPO(env=None, setting=AgentSettings.default_ppo_modular)
-    env.reset()
-    env.learn_reset()
-    env.learn_next()
-    env.learn_check()
-    env.learn_next()
-    env.learn_check()
-    env.update()
-
-    env.reset()
-    ppo_manual_step(env)
-    env.learn_check()
-    ppo_manual_step(env)
-    env.learn_check()
-    env.update()
-
-    env.learn_close()
-
-    # env.save_model('test.pth')
-
-
-def ppo_manual_step(env):
-    initial_state = env.learn_reset()
-    action, _ = env.select_action(initial_state)
-    next_state = env.learn_reset()
-    env.update_step(next_state, None, action, -1)
+# -*- coding: utf-8 -*-
+from modular_rl.agents.ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+'''
+This code is a Python script that initializes and trains an instance of the AgentPPO class with default settings using the init_ppo() function. 
+Additionally, the init_ppo_modular() function is provided to demonstrate the usage of the AgentPPO class with modified settings.
+
+In init_ppo_modular(), an instance of AgentPPO is created with a modified default_modular settings dictionary. 
+The function then calls various methods of the instance, such as reset(), learn_reset(), learn_next(), and update() to demonstrate the functionality of the class. 
+The instance is then saved to a file using the save_model() method, which is not shown in the provided code.
+
+'''
+
+
+def init_ppo():
+    env = AgentPPO(env=None, setting=AgentSettings.default_ppo)
+    env.learn()
+
+
+def init_ppo_modular():
+    env = AgentPPO(env=None, setting=AgentSettings.default_ppo_modular)
+    env.reset()
+    env.learn_reset()
+    env.learn_next()
+    env.learn_check()
+    env.learn_next()
+    env.learn_check()
+    env.update()
+
+    env.reset()
+    ppo_manual_step(env)
+    env.learn_check()
+    ppo_manual_step(env)
+    env.learn_check()
+    env.update()
+
+    env.learn_close()
+
+    # env.save_model('test.pth')
+
+
+def ppo_manual_step(env):
+    initial_state = env.learn_reset()
+    action, _ = env.select_action(initial_state)
+    next_state = env.learn_reset()
+    env.update_step(next_state, None, action, -1)
```

### Comparing `modular_rl-0.2.3/modular_rl/util/node.py` & `modular_rl-0.3.0/modular_rl/util/node.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import math
-from LogAssist.log import Logger
-import numpy as np
-
-
-class Node:
-    def __init__(self, state, prior, action=None, done=False):
-        self.state = state
-        self.prior = prior
-        self.action = action  # 액션 정보를 저장하는 속성 추가
-        self.visit_count = 0
-        self.value_sum = 0
-        self.children = {}
-        self.total_value = 0
-        self.done = done  # Assign the done attribute
-
-
-    def __repr__(self):
-        return f'Node(state={self.state}, total_value={self.total_value}, visit_count={self.visit_count}, is_expanded={self.expanded()}, action_probs={self.action}, children={self.children})'
-
-    def expanded(self):
-        return len(self.children) > 0
-
-    def value(self):
-        if self.visit_count == 0:
-            return 0
-        return self.total_value / self.visit_count  # 총 보상을 방문 횟수로 나누어 평균 보상을 반환
-
-    def select_child(self, cpuct):
-        best_score = -math.inf
-        best_action = -1
-        best_child = None
-
-        for action, child in self.children.items():
-            uct_score = child.value() + cpuct * child.prior * math.sqrt(self.visit_count) / \
-                (1 + child.visit_count)
-            if uct_score > best_score:
-                best_score = uct_score
-                best_action = action
-                best_child = child
-
-        return best_action, best_child
-
-    def expand(self, action_space, child_priors, child_done):  # Add a child_done parameter
-        for action, prior in zip(range(action_space), child_priors):
-            if action not in self.children:
-                self.children[action] = Node(self.state, prior, action, child_done)  # Pass the child_done to the new Node
-
-    def update_stats(self, reward):
-        self.total_value += reward  # 총 보상 업데이트
-        self.visit_count += 1  # 방문 횟수 증가
-
-    def select_action(self, temperature=1):
-        visit_counts = np.array(
-            [child.visit_count for child in self.children.values()])
-        actions = [action for action in self.children.keys()]
-        if temperature == 0:
-            action = actions[np.argmax(visit_counts)]
-        else:
-            visit_counts = visit_counts ** (1/temperature)  # apply temperature
-            # normalize to get probabilities
-            visit_counts = visit_counts / sum(visit_counts)
-            action = np.random.choice(actions, p=visit_counts)
-
-        return action
+import math
+from LogAssist.log import Logger
+import numpy as np
+
+
+class Node:
+    def __init__(self, state, prior, action=None, done=False):
+        self.state = state
+        self.prior = prior
+        self.action = action  # 액션 정보를 저장하는 속성 추가
+        self.visit_count = 0
+        self.value_sum = 0
+        self.children = {}
+        self.total_value = 0
+        self.done = done  # Assign the done attribute
+
+
+    def __repr__(self):
+        return f'Node(state={self.state}, total_value={self.total_value}, visit_count={self.visit_count}, is_expanded={self.expanded()}, action_probs={self.action}, children={self.children})'
+
+    def expanded(self):
+        return len(self.children) > 0
+
+    def value(self):
+        if self.visit_count == 0:
+            return 0
+        return self.total_value / self.visit_count  # 총 보상을 방문 횟수로 나누어 평균 보상을 반환
+
+    def select_child(self, cpuct):
+        best_score = -math.inf
+        best_action = -1
+        best_child = None
+
+        for action, child in self.children.items():
+            uct_score = child.value() + cpuct * child.prior * math.sqrt(self.visit_count) / \
+                (1 + child.visit_count)
+            if uct_score > best_score:
+                best_score = uct_score
+                best_action = action
+                best_child = child
+
+        return best_action, best_child
+
+    def expand(self, action_space, child_priors, child_done):  # Add a child_done parameter
+        for action, prior in zip(range(action_space), child_priors):
+            if action not in self.children:
+                self.children[action] = Node(self.state, prior, action, child_done)  # Pass the child_done to the new Node
+
+    def update_stats(self, reward):
+        self.total_value += reward  # 총 보상 업데이트
+        self.visit_count += 1  # 방문 횟수 증가
+
+    def select_action(self, temperature=1):
+        visit_counts = np.array(
+            [child.visit_count for child in self.children.values()])
+        actions = [action for action in self.children.keys()]
+        if temperature == 0:
+            action = actions[np.argmax(visit_counts)]
+        else:
+            visit_counts = visit_counts ** (1/temperature)  # apply temperature
+            # normalize to get probabilities
+            visit_counts = visit_counts / sum(visit_counts)
+            action = np.random.choice(actions, p=visit_counts)
+
+        return action
```

### Comparing `modular_rl-0.2.3/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.3.0/modular_rl.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-Metadata-Version: 2.1
-Name: modular-rl
-Version: 0.2.3
-Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-Home-page: https://github.com/horrible-gh/ModularRL
-Author: sjm
-Author-email: horrible <shinjpn1@gmail.com>
-Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
-Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
-Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
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
+Metadata-Version: 2.1
+Name: modular-rl
+Version: 0.3.0
+Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+Home-page: https://github.com/horrible-gh/ModularRL
+Author: sjm
+Author-email: horrible <shinjpn1@gmail.com>
+Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
+Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
+Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
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
+    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (Modular)
+-   AgentMCTS
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
+-   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.2.3/pyproject.toml` & `modular_rl-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.2.3"
+version = "0.3.0"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.2.3/setup.py` & `modular_rl-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.2.3',
+    version='0.3.0',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/ModularRL',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -21,10 +21,10 @@
         'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.6',
     install_requires=[
         'numpy>=1.18.0',
         'torch>=1.24.2',
         'gym>=0.23.0',
-        'LogAssist>=1.0.4'
+        'LogAssist>=1.0.6'
     ],
 )
```

