# Comparing `tmp/smt-2.0b3.tar.gz` & `tmp/smt-2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\rlafage\workspace\smt\dist\.tmp-ul6sai3g\smt-2.0b3.tar", last modified: Wed May 17 09:23:58 2023, max compression
+gzip compressed data, was "D:\rlafage\workspace\smt\dist\.tmp-26vteikw\smt-2.0b4.tar", last modified: Wed Jun  7 09:50:02 2023, max compression
```

## Comparing `smt-2.0b3.tar` & `smt-2.0b4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.583097 smt-2.0b3/
--rw-rw-rw-   0        0        0     1543 2018-12-22 21:42:35.000000 smt-2.0b3/LICENSE.txt
--rw-rw-rw-   0        0        0       84 2019-06-10 15:38:34.000000 smt-2.0b3/MANIFEST.in
--rw-rw-rw-   0        0        0     1760 2023-05-17 09:23:58.583097 smt-2.0b3/PKG-INFO
--rw-rw-rw-   0        0        0     2990 2023-03-08 08:23:36.000000 smt-2.0b3/README.md
--rw-rw-rw-   0        0        0       69 2023-03-02 15:01:33.000000 smt-2.0b3/pyproject.toml
--rw-rw-rw-   0        0        0      114 2023-05-17 09:23:58.583097 smt-2.0b3/setup.cfg
--rw-rw-rw-   0        0        0     3885 2023-05-16 15:13:53.000000 smt-2.0b3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.420324 smt-2.0b3/smt/
--rw-rw-rw-   0        0        0       23 2023-05-17 09:22:32.000000 smt-2.0b3/smt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.451581 smt-2.0b3/smt/applications/
--rw-rw-rw-   0        0        0      187 2021-01-26 14:08:32.000000 smt-2.0b3/smt/applications/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/application.py
--rw-rw-rw-   0        0        0    15322 2023-05-17 09:22:32.000000 smt-2.0b3/smt/applications/ego.py
--rw-rw-rw-   0        0        0    28217 2023-05-16 15:13:53.000000 smt-2.0b3/smt/applications/mfk.py
--rw-rw-rw-   0        0        0     2382 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/mfkpls.py
--rw-rw-rw-   0        0        0     2137 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/mfkplsk.py
--rw-rw-rw-   0        0        0    12570 2023-05-17 09:22:32.000000 smt-2.0b3/smt/applications/mixed_integer.py
--rw-rw-rw-   0        0        0    26146 2023-05-16 15:13:53.000000 smt-2.0b3/smt/applications/moe.py
--rw-rw-rw-   0        0        0    10088 2023-04-13 14:40:53.000000 smt-2.0b3/smt/applications/vfm.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.498456 smt-2.0b3/smt/problems/
--rw-rw-rw-   0        0        0      860 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/__init__.py
--rw-rw-rw-   0        0        0     1738 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/branin.py
--rw-rw-rw-   0        0        0     4199 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/cantilever_beam.py
--rw-rw-rw-   0        0        0     5334 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/hierarchical_goldstein.py
--rw-rw-rw-   0        0        0     1358 2020-11-30 16:48:50.000000 smt-2.0b3/smt/problems/lp_norm.py
--rw-rw-rw-   0        0        0     1890 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/mixed_cantilever_beam.py
--rw-rw-rw-   0        0        0      992 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_cantilever_beam.py
--rw-rw-rw-   0        0        0      968 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_robot_arm.py
--rw-rw-rw-   0        0        0      963 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_rosenbrock.py
--rw-rw-rw-   0        0        0      881 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/ndim_step_function.py
--rw-rw-rw-   0        0        0     3276 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/neural_network.py
--rw-rw-rw-   0        0        0     4754 2023-05-17 09:22:32.000000 smt-2.0b3/smt/problems/problem.py
--rw-rw-rw-   0        0        0     2728 2023-05-16 15:13:53.000000 smt-2.0b3/smt/problems/reduced_problem.py
--rw-rw-rw-   0        0        0     3100 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/robot_arm.py
--rw-rw-rw-   0        0        0     1467 2020-11-30 16:48:50.000000 smt-2.0b3/smt/problems/rosenbrock.py
--rw-rw-rw-   0        0        0     1146 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/sphere.py
--rw-rw-rw-   0        0        0     2108 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/tensor_product.py
--rw-rw-rw-   0        0        0     4703 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/torsion_vibration.py
--rw-rw-rw-   0        0        0     3157 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/water_flow.py
--rw-rw-rw-   0        0        0     2805 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/water_flow_lfidelity.py
--rw-rw-rw-   0        0        0     3036 2022-08-23 09:30:16.000000 smt-2.0b3/smt/problems/welded_beam.py
--rw-rw-rw-   0        0        0     3372 2022-08-22 07:12:21.000000 smt-2.0b3/smt/problems/wing_weight.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.498456 smt-2.0b3/smt/sampling_methods/
--rw-rw-rw-   0        0        0       93 2018-12-22 21:42:35.000000 smt-2.0b3/smt/sampling_methods/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-01-12 17:00:33.000000 smt-2.0b3/smt/sampling_methods/full_factorial.py
--rw-rw-rw-   0        0        0    13859 2023-04-13 14:40:53.000000 smt-2.0b3/smt/sampling_methods/lhs.py
--rw-rw-rw-   0        0        0      829 2021-01-28 14:52:03.000000 smt-2.0b3/smt/sampling_methods/random.py
--rw-rw-rw-   0        0        0     4675 2023-01-12 17:00:33.000000 smt-2.0b3/smt/sampling_methods/sampling_method.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.400117 smt-2.0b3/smt/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.514080 smt-2.0b3/smt/src/idw/
--rw-rw-rw-   0        0        0     2529 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/idw/idw.cpp
--rw-rw-rw-   0        0        0      335 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/idw/idw.hpp
--rw-rw-rw-   0        0        0   313797 2023-05-17 09:23:55.000000 smt-2.0b3/smt/src/idw/idwclib.cpp
--rw-rw-rw-   0        0        0      931 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/idw/idwclib.pyx
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.520589 smt-2.0b3/smt/src/rbf/
--rw-rw-rw-   0        0        0     2080 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rbf/rbf.cpp
--rw-rw-rw-   0        0        0      366 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rbf/rbf.hpp
--rw-rw-rw-   0        0        0   316817 2023-05-17 09:23:55.000000 smt-2.0b3/smt/src/rbf/rbfclib.cpp
--rw-rw-rw-   0        0        0     1058 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rbf/rbfclib.pyx
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.520589 smt-2.0b3/smt/src/rmts/
--rw-rw-rw-   0        0        0     7239 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtb.cpp
--rw-rw-rw-   0        0        0      394 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtb.hpp
--rw-rw-rw-   0        0        0     5968 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtc.cpp
--rw-rw-rw-   0        0        0      692 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtc.hpp
--rw-rw-rw-   0        0        0     2684 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmts.cpp
--rw-rw-rw-   0        0        0      608 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmts.hpp
--rw-rw-rw-   0        0        0   430206 2023-05-17 09:23:56.000000 smt-2.0b3/smt/src/rmts/rmtsclib.cpp
--rw-rw-rw-   0        0        0     3618 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/rmtsclib.pyx
--rw-rw-rw-   0        0        0      532 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/utils.cpp
--rw-rw-rw-   0        0        0      178 2018-12-22 21:42:35.000000 smt-2.0b3/smt/src/rmts/utils.hpp
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.551848 smt-2.0b3/smt/surrogate_models/
--rw-rw-rw-   0        0        0      561 2023-05-17 09:22:32.000000 smt-2.0b3/smt/surrogate_models/__init__.py
--rw-rw-rw-   0        0        0     1985 2023-05-16 15:13:53.000000 smt-2.0b3/smt/surrogate_models/gekpls.py
--rw-rw-rw-   0        0        0    10492 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/genn.py
--rw-rw-rw-   0        0        0     3805 2021-01-26 14:08:32.000000 smt-2.0b3/smt/surrogate_models/idw.py
--rw-rw-rw-   0        0        0     4633 2023-05-15 09:02:07.000000 smt-2.0b3/smt/surrogate_models/kpls.py
--rw-rw-rw-   0        0        0     1436 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/kplsk.py
--rw-rw-rw-   0        0        0      955 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/krg.py
--rw-rw-rw-   0        0        0    75098 2023-05-17 09:22:32.000000 smt-2.0b3/smt/surrogate_models/krg_based.py
--rw-rw-rw-   0        0        0     2783 2023-01-12 15:06:16.000000 smt-2.0b3/smt/surrogate_models/ls.py
--rw-rw-rw-   0        0        0    17716 2023-05-16 15:13:53.000000 smt-2.0b3/smt/surrogate_models/mgp.py
--rw-rw-rw-   0        0        0     4937 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/qp.py
--rw-rw-rw-   0        0        0     6530 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/rbf.py
--rw-rw-rw-   0        0        0     4635 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/rmtb.py
--rw-rw-rw-   0        0        0     5761 2021-01-12 13:42:11.000000 smt-2.0b3/smt/surrogate_models/rmtc.py
--rw-rw-rw-   0        0        0    20916 2023-04-13 14:40:53.000000 smt-2.0b3/smt/surrogate_models/rmts.py
--rw-rw-rw-   0        0        0    19436 2023-05-16 15:13:53.000000 smt-2.0b3/smt/surrogate_models/surrogate_model.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.567473 smt-2.0b3/smt/utils/
--rw-rw-rw-   0        0        0       37 2018-12-22 21:42:35.000000 smt-2.0b3/smt/utils/__init__.py
--rw-rw-rw-   0        0        0     1863 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/caching.py
--rw-rw-rw-   0        0        0      949 2022-10-21 19:56:44.000000 smt-2.0b3/smt/utils/checks.py
--rw-rw-rw-   0        0        0    28396 2023-05-17 09:22:32.000000 smt-2.0b3/smt/utils/design_space.py
--rw-rw-rw-   0        0        0    13183 2023-03-01 09:44:14.000000 smt-2.0b3/smt/utils/krg_sampling.py
--rw-rw-rw-   0        0        0    50183 2023-05-17 09:22:32.000000 smt-2.0b3/smt/utils/kriging.py
--rw-rw-rw-   0        0        0     8022 2022-08-23 09:30:16.000000 smt-2.0b3/smt/utils/line_search.py
--rw-rw-rw-   0        0        0    17986 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/linear_solvers.py
--rw-rw-rw-   0        0        0     3750 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.583097 smt-2.0b3/smt/utils/neural_net/
--rw-rw-rw-   0        0        0      293 2019-04-14 10:57:11.000000 smt-2.0b3/smt/utils/neural_net/__init__.py
--rw-rw-rw-   0        0        0     2528 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/neural_net/activation.py
--rw-rw-rw-   0        0        0    11665 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/bwd_prop.py
--rw-rw-rw-   0        0        0    10006 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/data.py
--rw-rw-rw-   0        0        0     9734 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/fwd_prop.py
--rw-rw-rw-   0        0        0     3604 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/loss.py
--rw-rw-rw-   0        0        0     1080 2019-04-14 10:57:11.000000 smt-2.0b3/smt/utils/neural_net/metrics.py
--rw-rw-rw-   0        0        0    21968 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/model.py
--rw-rw-rw-   0        0        0    13245 2023-04-13 14:40:53.000000 smt-2.0b3/smt/utils/neural_net/optimizer.py
--rw-rw-rw-   0        0        0     4630 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/options_dictionary.py
--rw-rw-rw-   0        0        0     3608 2020-11-30 16:48:50.000000 smt-2.0b3/smt/utils/printer.py
--rw-rw-rw-   0        0        0     4087 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/silence.py
--rw-rw-rw-   0        0        0     1413 2020-04-22 07:33:16.000000 smt-2.0b3/smt/utils/sm_test_case.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:23:58.420324 smt-2.0b3/smt.egg-info/
--rw-rw-rw-   0        0        0     1760 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-17 09:23:58.000000 smt-2.0b3/smt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-09-09 08:43:37.000000 smt-2.0b3/smt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-17 09:23:57.000000 smt-2.0b3/smt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.125724 smt-2.0b4/
+-rw-rw-rw-   0        0        0     1543 2018-12-22 21:42:35.000000 smt-2.0b4/LICENSE.txt
+-rw-rw-rw-   0        0        0       84 2019-06-10 15:38:34.000000 smt-2.0b4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1760 2023-06-07 09:50:02.125724 smt-2.0b4/PKG-INFO
+-rw-rw-rw-   0        0        0     3714 2023-06-02 05:57:57.000000 smt-2.0b4/README.md
+-rw-rw-rw-   0        0        0       69 2023-03-02 15:01:33.000000 smt-2.0b4/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-06-07 09:50:02.130775 smt-2.0b4/setup.cfg
+-rw-rw-rw-   0        0        0     3885 2023-06-02 05:57:57.000000 smt-2.0b4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:01.851055 smt-2.0b4/smt/
+-rw-rw-rw-   0        0        0       23 2023-06-07 09:47:59.000000 smt-2.0b4/smt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:01.915661 smt-2.0b4/smt/applications/
+-rw-rw-rw-   0        0        0      187 2021-01-26 14:08:32.000000 smt-2.0b4/smt/applications/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-05-22 12:35:13.000000 smt-2.0b4/smt/applications/application.py
+-rw-rw-rw-   0        0        0    15322 2023-06-07 09:47:19.000000 smt-2.0b4/smt/applications/ego.py
+-rw-rw-rw-   0        0        0    28217 2023-05-22 12:35:13.000000 smt-2.0b4/smt/applications/mfk.py
+-rw-rw-rw-   0        0        0     2382 2023-05-22 12:35:13.000000 smt-2.0b4/smt/applications/mfkpls.py
+-rw-rw-rw-   0        0        0     2137 2023-05-22 12:35:13.000000 smt-2.0b4/smt/applications/mfkplsk.py
+-rw-rw-rw-   0        0        0    12568 2023-06-06 19:29:31.000000 smt-2.0b4/smt/applications/mixed_integer.py
+-rw-rw-rw-   0        0        0    26146 2023-05-22 12:35:13.000000 smt-2.0b4/smt/applications/moe.py
+-rw-rw-rw-   0        0        0    10088 2023-05-22 12:35:13.000000 smt-2.0b4/smt/applications/vfm.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:01.981042 smt-2.0b4/smt/problems/
+-rw-rw-rw-   0        0        0      860 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/branin.py
+-rw-rw-rw-   0        0        0     4199 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/cantilever_beam.py
+-rw-rw-rw-   0        0        0     5334 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/hierarchical_goldstein.py
+-rw-rw-rw-   0        0        0     1358 2020-11-30 16:48:50.000000 smt-2.0b4/smt/problems/lp_norm.py
+-rw-rw-rw-   0        0        0     1890 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/mixed_cantilever_beam.py
+-rw-rw-rw-   0        0        0      992 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/ndim_cantilever_beam.py
+-rw-rw-rw-   0        0        0      968 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/ndim_robot_arm.py
+-rw-rw-rw-   0        0        0      963 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/ndim_rosenbrock.py
+-rw-rw-rw-   0        0        0      881 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/ndim_step_function.py
+-rw-rw-rw-   0        0        0     3276 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/neural_network.py
+-rw-rw-rw-   0        0        0     4754 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/problem.py
+-rw-rw-rw-   0        0        0     2728 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/reduced_problem.py
+-rw-rw-rw-   0        0        0     3100 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/robot_arm.py
+-rw-rw-rw-   0        0        0     1467 2020-11-30 16:48:50.000000 smt-2.0b4/smt/problems/rosenbrock.py
+-rw-rw-rw-   0        0        0     1146 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/sphere.py
+-rw-rw-rw-   0        0        0     2108 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/tensor_product.py
+-rw-rw-rw-   0        0        0     4703 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/torsion_vibration.py
+-rw-rw-rw-   0        0        0     3157 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/water_flow.py
+-rw-rw-rw-   0        0        0     2805 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/water_flow_lfidelity.py
+-rw-rw-rw-   0        0        0     3036 2023-05-22 12:35:13.000000 smt-2.0b4/smt/problems/welded_beam.py
+-rw-rw-rw-   0        0        0     3372 2022-08-22 07:12:21.000000 smt-2.0b4/smt/problems/wing_weight.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:01.995642 smt-2.0b4/smt/sampling_methods/
+-rw-rw-rw-   0        0        0       93 2018-12-22 21:42:35.000000 smt-2.0b4/smt/sampling_methods/__init__.py
+-rw-rw-rw-   0        0        0     2016 2023-05-22 12:35:13.000000 smt-2.0b4/smt/sampling_methods/full_factorial.py
+-rw-rw-rw-   0        0        0    13859 2023-05-22 12:35:13.000000 smt-2.0b4/smt/sampling_methods/lhs.py
+-rw-rw-rw-   0        0        0      829 2021-01-28 14:52:03.000000 smt-2.0b4/smt/sampling_methods/random.py
+-rw-rw-rw-   0        0        0     4675 2023-05-22 12:35:13.000000 smt-2.0b4/smt/sampling_methods/sampling_method.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:01.822963 smt-2.0b4/smt/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.000663 smt-2.0b4/smt/src/idw/
+-rw-rw-rw-   0        0        0     2529 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/idw/idw.cpp
+-rw-rw-rw-   0        0        0      335 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/idw/idw.hpp
+-rw-rw-rw-   0        0        0   314512 2023-06-07 09:49:58.000000 smt-2.0b4/smt/src/idw/idwclib.cpp
+-rw-rw-rw-   0        0        0      931 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/idw/idwclib.pyx
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.005668 smt-2.0b4/smt/src/rbf/
+-rw-rw-rw-   0        0        0     2080 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rbf/rbf.cpp
+-rw-rw-rw-   0        0        0      366 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rbf/rbf.hpp
+-rw-rw-rw-   0        0        0   317532 2023-06-07 09:49:58.000000 smt-2.0b4/smt/src/rbf/rbfclib.cpp
+-rw-rw-rw-   0        0        0     1058 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rbf/rbfclib.pyx
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.020822 smt-2.0b4/smt/src/rmts/
+-rw-rw-rw-   0        0        0     7239 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmtb.cpp
+-rw-rw-rw-   0        0        0      394 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmtb.hpp
+-rw-rw-rw-   0        0        0     5968 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmtc.cpp
+-rw-rw-rw-   0        0        0      692 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmtc.hpp
+-rw-rw-rw-   0        0        0     2684 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmts.cpp
+-rw-rw-rw-   0        0        0      608 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmts.hpp
+-rw-rw-rw-   0        0        0   430952 2023-06-07 09:49:59.000000 smt-2.0b4/smt/src/rmts/rmtsclib.cpp
+-rw-rw-rw-   0        0        0     3618 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/rmtsclib.pyx
+-rw-rw-rw-   0        0        0      532 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/utils.cpp
+-rw-rw-rw-   0        0        0      178 2018-12-22 21:42:35.000000 smt-2.0b4/smt/src/rmts/utils.hpp
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.065961 smt-2.0b4/smt/surrogate_models/
+-rw-rw-rw-   0        0        0      561 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/__init__.py
+-rw-rw-rw-   0        0        0     1985 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/gekpls.py
+-rw-rw-rw-   0        0        0    10492 2021-01-12 13:42:11.000000 smt-2.0b4/smt/surrogate_models/genn.py
+-rw-rw-rw-   0        0        0     3805 2021-01-26 14:08:32.000000 smt-2.0b4/smt/surrogate_models/idw.py
+-rw-rw-rw-   0        0        0     4633 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/kpls.py
+-rw-rw-rw-   0        0        0     1436 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/kplsk.py
+-rw-rw-rw-   0        0        0      955 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/krg.py
+-rw-rw-rw-   0        0        0    74391 2023-06-07 09:47:19.000000 smt-2.0b4/smt/surrogate_models/krg_based.py
+-rw-rw-rw-   0        0        0     2783 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/ls.py
+-rw-rw-rw-   0        0        0    17716 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/mgp.py
+-rw-rw-rw-   0        0        0     4937 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/qp.py
+-rw-rw-rw-   0        0        0     6530 2021-01-12 13:42:11.000000 smt-2.0b4/smt/surrogate_models/rbf.py
+-rw-rw-rw-   0        0        0     4635 2021-01-12 13:42:11.000000 smt-2.0b4/smt/surrogate_models/rmtb.py
+-rw-rw-rw-   0        0        0     5761 2021-01-12 13:42:11.000000 smt-2.0b4/smt/surrogate_models/rmtc.py
+-rw-rw-rw-   0        0        0    20916 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/rmts.py
+-rw-rw-rw-   0        0        0    19436 2023-05-22 12:35:13.000000 smt-2.0b4/smt/surrogate_models/surrogate_model.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.101099 smt-2.0b4/smt/utils/
+-rw-rw-rw-   0        0        0       37 2018-12-22 21:42:35.000000 smt-2.0b4/smt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1863 2020-04-22 07:33:16.000000 smt-2.0b4/smt/utils/caching.py
+-rw-rw-rw-   0        0        0      949 2022-10-21 19:56:44.000000 smt-2.0b4/smt/utils/checks.py
+-rw-rw-rw-   0        0        0    29638 2023-06-03 21:09:34.000000 smt-2.0b4/smt/utils/design_space.py
+-rw-rw-rw-   0        0        0    13183 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/krg_sampling.py
+-rw-rw-rw-   0        0        0    50115 2023-06-07 09:47:19.000000 smt-2.0b4/smt/utils/kriging.py
+-rw-rw-rw-   0        0        0     8022 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/line_search.py
+-rw-rw-rw-   0        0        0    17986 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/linear_solvers.py
+-rw-rw-rw-   0        0        0     3750 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:02.125724 smt-2.0b4/smt/utils/neural_net/
+-rw-rw-rw-   0        0        0      293 2019-04-14 10:57:11.000000 smt-2.0b4/smt/utils/neural_net/__init__.py
+-rw-rw-rw-   0        0        0     2528 2020-04-22 07:33:16.000000 smt-2.0b4/smt/utils/neural_net/activation.py
+-rw-rw-rw-   0        0        0    11665 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/neural_net/bwd_prop.py
+-rw-rw-rw-   0        0        0    10006 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/neural_net/data.py
+-rw-rw-rw-   0        0        0     9734 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/neural_net/fwd_prop.py
+-rw-rw-rw-   0        0        0     3604 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/neural_net/loss.py
+-rw-rw-rw-   0        0        0     1080 2019-04-14 10:57:11.000000 smt-2.0b4/smt/utils/neural_net/metrics.py
+-rw-rw-rw-   0        0        0    21968 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/neural_net/model.py
+-rw-rw-rw-   0        0        0    13245 2023-05-22 12:35:13.000000 smt-2.0b4/smt/utils/neural_net/optimizer.py
+-rw-rw-rw-   0        0        0     4630 2020-04-22 07:33:16.000000 smt-2.0b4/smt/utils/options_dictionary.py
+-rw-rw-rw-   0        0        0     3608 2020-11-30 16:48:50.000000 smt-2.0b4/smt/utils/printer.py
+-rw-rw-rw-   0        0        0     4087 2020-04-22 07:33:16.000000 smt-2.0b4/smt/utils/silence.py
+-rw-rw-rw-   0        0        0     1413 2020-04-22 07:33:16.000000 smt-2.0b4/smt/utils/sm_test_case.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:50:01.860825 smt-2.0b4/smt.egg-info/
+-rw-rw-rw-   0        0        0     1760 2023-06-07 09:50:01.000000 smt-2.0b4/smt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-06-07 09:50:01.000000 smt-2.0b4/smt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:50:01.000000 smt-2.0b4/smt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-09-09 08:43:37.000000 smt-2.0b4/smt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-06-07 09:50:01.000000 smt-2.0b4/smt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-07 09:50:01.000000 smt-2.0b4/smt.egg-info/top_level.txt
```

### Comparing `smt-2.0b3/LICENSE.txt` & `smt-2.0b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/PKG-INFO` & `smt-2.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smt
-Version: 2.0b3
+Version: 2.0b4
 Summary: The Surrogate Modeling Toolbox (SMT)
 Home-page: https://github.com/SMTorg/smt
 Download-URL: https://github.com/SMTorg/smt/releases
 Author: Mohamed Amine Bouhlel et al.
 Author-email: mbouhlel@umich.edu
 License: BSD-3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `smt-2.0b3/README.md` & `smt-2.0b4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,34 @@
 SMT is different from existing surrogate modeling libraries because of its emphasis on derivatives, including training derivatives used for gradient-enhanced modeling, prediction derivatives, and derivatives with respect to the training data.
 
 It also includes new surrogate models that are not available elsewhere: kriging by partial-least squares reduction and energy-minimizing spline interpolation.
 SMT is documented using custom tools for embedding automatically-tested code and dynamically-generated plots to produce high-quality user guides with minimal effort from contributors.
 
 SMT is distributed under the New BSD license.
 
-To cite SMT: M. A. Bouhlel and J. T. Hwang and N. Bartoli and R. Lafage and J. Morlier and J. R. R. A. Martins. A Python surrogate modeling framework with derivatives. Advances in Engineering Software, 2019.
+To cite SMT 2.0: P. Saves and R. Lafage and N. Bartoli and Y. Diouane and J. H. Bussemaker and T. Lefebvre and J. T. Hwang and J. Morlier and J. R. R. A. Martins. SMT 2.0: A Surrogate Modeling Toolbox with a focus on Hierarchical and Mixed Variables Gaussian Processes. ArXiv preprint, 2023.
+
+```
+@article{SMT2ArXiv,
+	Author = {P. Saves and R. Lafage and N. Bartoli and Y. Diouane and J. H. Bussemaker and T. Lefebvre and J. T. Hwang and J. Morlier and J. R. R. A. Martins},
+	Journal = {ArXiv preprint},	
+	Title = {{SMT} 2.0: A Surrogate Modeling Toolbox with a focus on Hierarchical and Mixed Variables Gaussian Processes},
+	Publisher = {ArXiv},		
+	doi = {https://doi.org/10.48550/arXiv.2305.13998},
+	Year = {2023}}
+```
+
+To cite SMT legacy: M. A. Bouhlel and J. T. Hwang and N. Bartoli and R. Lafage and J. Morlier and J. R. R. A. Martins. A Python surrogate modeling framework with derivatives. Advances in Engineering Software, 2019.
 
 ```
 @article{SMT2019,
 	Author = {Mohamed Amine Bouhlel and John T. Hwang and Nathalie Bartoli and Rémi Lafage and Joseph Morlier and Joaquim R. R. A. Martins},
 	Journal = {Advances in Engineering Software},
 	Title = {A Python surrogate modeling framework with derivatives},
 	pages = {102662},
-	year = {2019},
 	issn = {0965-9978},
 	doi = {https://doi.org/10.1016/j.advengsoft.2019.03.005},
 	Year = {2019}}
 ```
 
 # Required packages
 SMT depends on the following modules: numpy, scipy, scikit-learn, pyDOE2 and Cython.
```

### Comparing `smt-2.0b3/setup.py` & `smt-2.0b4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     ],
     install_requires=[
         "scikit-learn",
         "pyDOE2",
         "scipy",
     ],
     extras_require={
-        'numba': [  # pip install smt[numba]
+        "numba": [  # pip install smt[numba]
             "numba~=0.56.4",
         ],
     },
     python_requires=">=3.7",
     zip_safe=False,
     ext_modules=ext,
     url="https://github.com/SMTorg/smt",  # use the URL to the github repo
```

### Comparing `smt-2.0b3/smt/applications/application.py` & `smt-2.0b4/smt/applications/application.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/applications/ego.py` & `smt-2.0b4/smt/applications/ego.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
             cons = []
             for j in range(len(bounds)):
                 lower, upper = bounds[j]
                 l = {"type": "ineq", "fun": lambda x, lb=lower, i=j: x[i] - lb}
                 u = {"type": "ineq", "fun": lambda x, ub=upper, i=j: ub - x[i]}
                 cons.append(l)
                 cons.append(u)
-            options = {"maxiter": 500, "catol": 1e-6, "tol": 1e-6, "rhobeg": 0.2}
+            options = {"maxiter": 200, "catol": 1e-6, "tol": 1e-6, "rhobeg": 0.4}
             bounds = None
         else:
             bounds = self.design_space.get_num_bounds()
             method = "SLSQP"
             cons = ()
             options = {"maxiter": 200}
```

### Comparing `smt-2.0b3/smt/applications/mfk.py` & `smt-2.0b4/smt/applications/mfk.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/applications/mfkpls.py` & `smt-2.0b4/smt/applications/mfkpls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/applications/mfkplsk.py` & `smt-2.0b4/smt/applications/mfkplsk.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/applications/mixed_integer.py` & `smt-2.0b4/smt/applications/mixed_integer.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 + str(self._surrogate.name)
                 + " is not supported. Please use MixedIntegerKrigingModel instead."
             )
         self.design_space = ensure_design_space(design_space=design_space)
 
         self._input_in_folded_space = input_in_folded_space
         self.supports = self._surrogate.supports
-        self.options["print_global"] = False
+        self.options["print_global"] = True
 
         if "poly" in self._surrogate.options:
             if self._surrogate.options["poly"] != "constant":
                 raise ValueError("constant regression must be used with mixed integer")
 
     @property
     def name(self):
@@ -190,15 +190,15 @@
                 + str(self._surrogate.name)
                 + " is not supported. Please use MixedIntegerSurrogateModel instead."
             )
         self.options["design_space"] = self._surrogate.design_space
 
         self._input_in_folded_space = input_in_folded_space
         self.supports = self._surrogate.supports
-        self.options["print_global"] = False
+        self.options["print_global"] = True
 
         if "poly" in self._surrogate.options:
             if self._surrogate.options["poly"] != "constant":
                 raise ValueError("constant regression must be used with mixed integer")
 
         design_space = self.design_space
         if (
```

### Comparing `smt-2.0b3/smt/applications/moe.py` & `smt-2.0b4/smt/applications/moe.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/applications/vfm.py` & `smt-2.0b4/smt/applications/vfm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/__init__.py` & `smt-2.0b4/smt/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/branin.py` & `smt-2.0b4/smt/problems/branin.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/cantilever_beam.py` & `smt-2.0b4/smt/problems/cantilever_beam.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/hierarchical_goldstein.py` & `smt-2.0b4/smt/problems/hierarchical_goldstein.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/lp_norm.py` & `smt-2.0b4/smt/problems/lp_norm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/mixed_cantilever_beam.py` & `smt-2.0b4/smt/problems/mixed_cantilever_beam.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/ndim_cantilever_beam.py` & `smt-2.0b4/smt/problems/ndim_cantilever_beam.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/ndim_robot_arm.py` & `smt-2.0b4/smt/problems/ndim_robot_arm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/ndim_rosenbrock.py` & `smt-2.0b4/smt/problems/ndim_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/ndim_step_function.py` & `smt-2.0b4/smt/problems/ndim_step_function.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/neural_network.py` & `smt-2.0b4/smt/problems/neural_network.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/problem.py` & `smt-2.0b4/smt/problems/problem.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/reduced_problem.py` & `smt-2.0b4/smt/problems/reduced_problem.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/robot_arm.py` & `smt-2.0b4/smt/problems/robot_arm.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/rosenbrock.py` & `smt-2.0b4/smt/problems/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/sphere.py` & `smt-2.0b4/smt/problems/sphere.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/tensor_product.py` & `smt-2.0b4/smt/problems/tensor_product.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/torsion_vibration.py` & `smt-2.0b4/smt/problems/torsion_vibration.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/water_flow.py` & `smt-2.0b4/smt/problems/water_flow.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/water_flow_lfidelity.py` & `smt-2.0b4/smt/problems/water_flow_lfidelity.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/welded_beam.py` & `smt-2.0b4/smt/problems/welded_beam.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/problems/wing_weight.py` & `smt-2.0b4/smt/problems/wing_weight.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/sampling_methods/full_factorial.py` & `smt-2.0b4/smt/sampling_methods/full_factorial.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/sampling_methods/lhs.py` & `smt-2.0b4/smt/sampling_methods/lhs.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/sampling_methods/random.py` & `smt-2.0b4/smt/sampling_methods/random.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/sampling_methods/sampling_method.py` & `smt-2.0b4/smt/sampling_methods/sampling_method.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/idw/idw.cpp` & `smt-2.0b4/smt/src/idw/idw.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/idw/idwclib.cpp` & `smt-2.0b4/smt/src/idw/idwclib.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
             "smt\\src\\idw\\idw.hpp"
         ],
         "include_dirs": [
             "smt/src/idw",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include"
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include"
         ],
         "language": "c++",
         "name": "smt.surrogate_models.idwclib",
         "sources": [
             "smt/src/idw/idwclib.pyx",
             "smt/src/idw/idw.cpp"
         ]
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,16 +100,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1070,195 +1074,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":692
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":699
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":704
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":714
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":717
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":724
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1290,42 +1294,42 @@
 /*--- Type declarations ---*/
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_3smt_16surrogate_models_7idwclib_PyIDW;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":728
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":730
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":732
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1558,30 +1562,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
@@ -3551,15 +3555,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3568,29 +3572,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3601,15 +3605,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3618,29 +3622,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3651,15 +3655,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3668,29 +3672,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3701,15 +3705,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3718,29 +3722,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3751,15 +3755,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3768,29 +3772,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3801,212 +3805,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4022,15 +4026,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4038,53 +4042,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -4092,30 +4096,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4130,15 +4134,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4154,15 +4158,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4170,53 +4174,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -4224,30 +4228,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4262,15 +4266,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4286,15 +4290,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4302,53 +4306,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -4356,30 +4360,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4394,176 +4398,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4676,15 +4680,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -4789,26 +4793,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -4890,88 +4894,51 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT(arrayobject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_35(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5211,15 +5178,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6593,18 +6560,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -6650,22 +6617,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -7403,15 +7370,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7637,15 +7604,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `smt-2.0b3/smt/src/idw/idwclib.pyx` & `smt-2.0b4/smt/src/idw/idwclib.pyx`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rbf/rbf.cpp` & `smt-2.0b4/smt/src/rbf/rbf.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rbf/rbfclib.cpp` & `smt-2.0b4/smt/src/rbf/rbfclib.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
             "smt\\src\\rbf\\rbf.hpp"
         ],
         "include_dirs": [
             "smt/src/rbf",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include"
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include"
         ],
         "language": "c++",
         "name": "smt.surrogate_models.rbfclib",
         "sources": [
             "smt/src/rbf/rbfclib.pyx",
             "smt/src/rbf/rbf.cpp"
         ]
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -100,16 +100,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1070,195 +1074,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":692
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":699
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":704
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":714
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":717
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":724
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1290,42 +1294,42 @@
 /*--- Type declarations ---*/
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_3smt_16surrogate_models_7rbfclib_PyRBF;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":728
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":730
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":732
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1558,30 +1562,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
@@ -3602,15 +3606,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3619,29 +3623,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3652,15 +3656,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3669,29 +3673,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3702,15 +3706,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3719,29 +3723,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3752,15 +3756,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3769,29 +3773,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3802,15 +3806,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3819,29 +3823,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3852,212 +3856,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4073,15 +4077,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4089,53 +4093,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -4143,30 +4147,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4181,15 +4185,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4205,15 +4209,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4221,53 +4225,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -4275,30 +4279,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4313,15 +4317,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4337,15 +4341,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4353,53 +4357,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -4407,30 +4411,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4445,176 +4449,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4727,15 +4731,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -4842,26 +4846,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -4943,88 +4947,51 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT(arrayobject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_35(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5264,15 +5231,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6646,18 +6613,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -6703,22 +6670,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -7456,15 +7423,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7690,15 +7657,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `smt-2.0b3/smt/src/rbf/rbfclib.pyx` & `smt-2.0b4/smt/src/rbf/rbfclib.pyx`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/rmtb.cpp` & `smt-2.0b4/smt/src/rmts/rmtb.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/rmtc.cpp` & `smt-2.0b4/smt/src/rmts/rmtc.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/rmtc.hpp` & `smt-2.0b4/smt/src/rmts/rmtc.hpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/rmts.cpp` & `smt-2.0b4/smt/src/rmts/rmts.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/rmts.hpp` & `smt-2.0b4/smt/src/rmts/rmts.hpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/rmtsclib.cpp` & `smt-2.0b4/smt/src/rmts/rmtsclib.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h",
             "smt\\src\\rmts\\rmtb.hpp",
             "smt\\src\\rmts\\rmtc.hpp"
         ],
         "include_dirs": [
             "smt/src/rmts",
-            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-iv5uk8cr\\lib\\site-packages\\numpy\\core\\include"
+            "D:\\rlafage\\AppData\\Local\\Temp\\build-env-wnv9gqcp\\lib\\site-packages\\numpy\\core\\include"
         ],
         "language": "c++",
         "name": "smt.surrogate_models.rmtsclib",
         "sources": [
             "smt/src/rmts/rmtsclib.pyx",
             "smt/src/rmts/utils.cpp",
             "smt/src/rmts/rmts.cpp",
@@ -35,16 +35,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -104,16 +104,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1075,195 +1079,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":692
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":699
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":704
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":714
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":717
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":724
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1296,42 +1300,42 @@
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_3smt_16surrogate_models_8rmtsclib_PyRMTB;
 struct __pyx_obj_3smt_16surrogate_models_8rmtsclib_PyRMTC;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":728
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":730
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":732
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1577,30 +1581,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
@@ -5650,15 +5654,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5667,29 +5671,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5700,15 +5704,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5717,29 +5721,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5750,15 +5754,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5767,29 +5771,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5800,15 +5804,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5817,29 +5821,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5850,15 +5854,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5867,29 +5871,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5900,212 +5904,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":750
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":753
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":749
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":934
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":936
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6121,15 +6125,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6137,53 +6141,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 942, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":943
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 944, __pyx_L5_except_error)
@@ -6191,30 +6195,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":940
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6229,15 +6233,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6253,15 +6257,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6269,53 +6273,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 948, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":949
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 950, __pyx_L5_except_error)
@@ -6323,30 +6327,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":946
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6361,15 +6365,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6385,15 +6389,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6401,53 +6405,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 954, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":955
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(3, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":956
+      /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 956, __pyx_L5_except_error)
@@ -6455,30 +6459,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(3, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":952
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6493,176 +6497,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":966
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":981
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":996
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1006
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+/* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1017
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6776,15 +6780,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_3smt_16surrogate_models_8rmtsclib_PyRMTC(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -6893,15 +6897,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -7036,26 +7040,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(3, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 950, __pyx_L1_error)
@@ -7147,88 +7151,51 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT(arrayobject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_35(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(3, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(3, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(3, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(3, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(3, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(3, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(3, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(3, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(3, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(3, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(3, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(3, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(3, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(3, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(3, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7468,15 +7435,15 @@
  * import numpy as np
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-iv5uk8cr/lib/site-packages/numpy/__init__.pxd":1013
+  /* "../../AppData/Local/Temp/build-env-wnv9gqcp/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8850,18 +8817,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -8907,22 +8874,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -9660,15 +9627,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9894,15 +9861,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `smt-2.0b3/smt/src/rmts/rmtsclib.pyx` & `smt-2.0b4/smt/src/rmts/rmtsclib.pyx`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/src/rmts/utils.cpp` & `smt-2.0b4/smt/src/rmts/utils.cpp`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/__init__.py` & `smt-2.0b4/smt/surrogate_models/__init__.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/gekpls.py` & `smt-2.0b4/smt/surrogate_models/gekpls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/genn.py` & `smt-2.0b4/smt/surrogate_models/genn.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/idw.py` & `smt-2.0b4/smt/surrogate_models/idw.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/kpls.py` & `smt-2.0b4/smt/surrogate_models/kpls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/kplsk.py` & `smt-2.0b4/smt/surrogate_models/kplsk.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/krg.py` & `smt-2.0b4/smt/surrogate_models/krg.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/krg_based.py` & `smt-2.0b4/smt/surrogate_models/krg_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,25 @@
         if not (self.is_continuous):
             D, self.ij, X = gower_componentwise_distances(
                 X=X,
                 x_is_acting=is_acting,
                 design_space=self.design_space,
                 hierarchical_kernel=self.options["hierarchical_kernel"],
             )
+            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
+                X2, _ = self.design_space.unfold_x(self.training_points[None][0][0])
+                (
+                    self.X2_norma,
+                    _,
+                    self.X2_offset,
+                    _,
+                    self.X2_scale,
+                    _,
+                ) = standardization(X2, self.training_points[None][0][1])
+                D, _ = cross_distances(self.X2_norma)
             self.Lij, self.n_levels = cross_levels(
                 X=self.X_train, ij=self.ij, design_space=self.design_space
             )
             _, self.cat_features = compute_X_cont(self.X_train, self.design_space)
         # Center and scale X and y
         (
             self.X_norma,
@@ -359,15 +370,14 @@
         # outputs['sol'] = self.sol
 
         self._new_train()
 
     def _initialize_theta(self, theta, n_levels, cat_features, cat_kernel):
         if self._corr_params is not None:
             return self._corr_params
-
         nx = self.nx
         try:
             cat_kernel_comps = self.options["cat_kernel_comps"]
             if cat_kernel_comps is not None:
                 n_levels = np.array(cat_kernel_comps)
         except KeyError:
             cat_kernel_comps = None
@@ -388,31 +398,24 @@
         n_theta_cont = 0
         for feat in cat_features:
             if feat:
                 if cat_kernel in [
                     MixIntKernelType.EXP_HOMO_HSPHERE,
                     MixIntKernelType.HOMO_HSPHERE,
                 ]:
-                    # theta_cont_features[
-                    #     j : j + int(nlevels[i] * (nlevels[i] - 1) / 2)
-                    # ] = False  # Matrix is already False
                     theta_cat_features[
                         j : j + int(n_levels[i] * (n_levels[i] - 1) / 2), i
                     ] = [True] * int(n_levels[i] * (n_levels[i] - 1) / 2)
                     j += int(n_levels[i] * (n_levels[i] - 1) / 2)
                 i += 1
             else:
-                if cat_kernel in [
-                    MixIntKernelType.EXP_HOMO_HSPHERE,
-                    MixIntKernelType.HOMO_HSPHERE,
-                ]:
-                    if n_theta_cont < ncomp:
-                        theta_cont_features[j] = True
-                        j += 1
-                        n_theta_cont += 1
+                if n_theta_cont < ncomp:
+                    theta_cont_features[j] = True
+                    j += 1
+                    n_theta_cont += 1
 
         theta_cat_features = (
             [
                 np.where(theta_cat_features[:, i_lvl])[0]
                 for i_lvl in range(len(n_levels))
             ],
             np.any(theta_cat_features, axis=1) if len(n_levels) > 0 else None,
@@ -498,38 +501,34 @@
             X_pls_space, _ = design_space.unfold_x(X)
             nx = len(theta)
 
         elif cat_kernel == MixIntKernelType.GOWER:
             X_pls_space = np.copy(X)
         else:
             X_pls_space, _ = compute_X_cont(X, design_space)
-            d_cont = dx[:, np.logical_not(cat_features)]
         if cat_kernel_comps is not None or ncomp < 1e5:
             ###Modifier la condition : if PLS cont
             if self.pls_coeff_cont == []:
                 X, y = self._compute_pls(X_pls_space.copy(), y.copy())
                 self.pls_coeff_cont = self.coeff_pls
-            if (
-                cat_kernel == MixIntKernelType.CONT_RELAX
-                or cat_kernel == MixIntKernelType.GOWER
-            ):
+            if cat_kernel in [MixIntKernelType.GOWER, MixIntKernelType.CONT_RELAX]:
                 d = componentwise_distance_PLS(
                     dx,
                     corr,
                     self.options["n_comp"],
                     self.pls_coeff_cont,
                     power,
                     theta=None,
                     return_derivative=False,
                 )
                 r = _correlation_types[corr](theta, d)
                 return r
             else:
                 d_cont = componentwise_distance_PLS(
-                    d_cont,
+                    dx[:, np.logical_not(cat_features)],
                     corr,
                     self.options["n_comp"],
                     self.pls_coeff_cont,
                     power,
                     theta=None,
                     return_derivative=False,
                 )
@@ -538,24 +537,20 @@
                 dx,
                 corr,
                 nx,
                 power,
                 theta=None,
                 return_derivative=False,
             )
-            if cat_kernel != MixIntKernelType.CONT_RELAX:
+            if cat_kernel in [MixIntKernelType.GOWER, MixIntKernelType.CONT_RELAX]:
+                r = _correlation_types[corr](theta, d)
+                return r
+            else:
                 d_cont = d[:, np.logical_not(cat_features)]
 
-        if (
-            cat_kernel == MixIntKernelType.CONT_RELAX
-            or cat_kernel == MixIntKernelType.GOWER
-        ):
-            r = _correlation_types[corr](theta, d)
-            return r
-
         theta_cont = theta[theta_cont_features[:, 0]]
         r_cont = _correlation_types[corr](theta_cont, d_cont)
         r_cat = np.copy(r_cont) * 0
         r = np.copy(r_cont)
         ##Theta_cat_i loop
         try:
             self.coeff_pls_cat
@@ -702,26 +697,14 @@
         if self.options["use_het_noise"]:
             noise = self.optimal_noise
         if self.options["eval_noise"] and not self.options["use_het_noise"]:
             theta = tmp_var[0 : self.D.shape[1]]
             noise = tmp_var[self.D.shape[1] :]
         if not (self.is_continuous):
             dx = self.D
-            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
-                X2, _ = self.design_space.unfold_x(self.training_points[None][0][0])
-                (
-                    self.X2_norma,
-                    _,
-                    self.X2_offset,
-                    _,
-                    self.X2_scale,
-                    _,
-                ) = standardization(X2, self.training_points[None][0][1])
-                dx, _ = cross_distances(self.X2_norma)
-
             r = self._matrix_data_corr(
                 corr=self.options["corr"],
                 design_space=self.design_space,
                 power=self.options["pow_exp_power"],
                 theta=theta,
                 theta_bounds=self.options["theta_bounds"],
                 dx=dx,
@@ -1185,25 +1168,23 @@
                 x,
                 x_is_acting=is_acting,
                 design_space=self.design_space,
                 hierarchical_kernel=self.options["hierarchical_kernel"],
                 y=np.copy(self.X_train),
                 y_is_acting=self.is_acting_train,
             )
+            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
+                Xpred, _ = self.design_space.unfold_x(x)
+                Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
+                dx = differences(Xpred_norma, Y=self.X2_norma.copy())
             _, ij = cross_distances(x, self.X_train)
             Lij, _ = cross_levels(
                 X=x, ij=ij, design_space=self.design_space, y=self.X_train
             )
             self.ij = ij
-            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
-                Xpred, _ = self.design_space.unfold_x(x)
-                Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
-                # Get pairwise componentwise L1-distances to the input training set
-                dx = differences(Xpred_norma, Y=self.X2_norma.copy())
-
             r = self._matrix_data_corr(
                 corr=self.options["corr"],
                 design_space=self.design_space,
                 power=self.options["pow_exp_power"],
                 theta=self.optimal_theta,
                 theta_bounds=self.options["theta_bounds"],
                 dx=dx,
@@ -1348,26 +1329,23 @@
                 x,
                 x_is_acting=is_acting,
                 design_space=self.design_space,
                 hierarchical_kernel=self.options["hierarchical_kernel"],
                 y=np.copy(self.X_train),
                 y_is_acting=self.is_acting_train,
             )
+            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
+                Xpred, _ = self.design_space.unfold_x(x)
+                Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
+                dx = differences(Xpred_norma, Y=self.X2_norma.copy())
             _, ij = cross_distances(x, self.X_train)
             Lij, _ = cross_levels(
                 X=x, ij=ij, design_space=self.design_space, y=self.X_train
             )
             self.ij = ij
-            if self.options["categorical_kernel"] == MixIntKernelType.CONT_RELAX:
-                Xpred, _ = self.design_space.unfold_x(x)
-                Xpred_norma = (Xpred - self.X2_offset) / self.X2_scale
-
-                # Get pairwise componentwise L1-distances to the input training set
-                dx = differences(Xpred_norma, Y=self.X2_norma.copy())
-
             r = self._matrix_data_corr(
                 corr=self.options["corr"],
                 design_space=self.design_space,
                 power=self.options["pow_exp_power"],
                 theta=self.optimal_theta,
                 theta_bounds=self.options["theta_bounds"],
                 dx=dx,
@@ -1531,15 +1509,15 @@
                 res = (
                     -np.log(10.0)
                     * (10.0**log10t_2d)
                     * (self._reduced_likelihood_gradient(10.0**log10t_2d)[0])
                 )
                 return res
 
-        limit, _rhobeg = 15 * len(self.options["theta0"]), 0.5
+        limit, _rhobeg = max(10 * len(self.options["theta0"]), 25), 0.5
         exit_function = False
         if "KPLSK" in self.name:
             n_iter = 1
         else:
             n_iter = 0
 
         for ii in range(n_iter, -1, -1):
```

### Comparing `smt-2.0b3/smt/surrogate_models/ls.py` & `smt-2.0b4/smt/surrogate_models/ls.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/mgp.py` & `smt-2.0b4/smt/surrogate_models/mgp.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/qp.py` & `smt-2.0b4/smt/surrogate_models/qp.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/rbf.py` & `smt-2.0b4/smt/surrogate_models/rbf.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/rmtb.py` & `smt-2.0b4/smt/surrogate_models/rmtb.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/rmtc.py` & `smt-2.0b4/smt/surrogate_models/rmtc.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/rmts.py` & `smt-2.0b4/smt/surrogate_models/rmts.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/surrogate_models/surrogate_model.py` & `smt-2.0b4/smt/surrogate_models/surrogate_model.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/caching.py` & `smt-2.0b4/smt/utils/caching.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/checks.py` & `smt-2.0b4/smt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/design_space.py` & `smt-2.0b4/smt/utils/design_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,33 +243,62 @@
 
         # Unfold if needed
         if x_is_unfolded:
             x_corrected, is_acting = self.unfold_x(x_corrected, is_acting)
 
         return x_corrected, is_acting
 
-    def decode_values(self, x: np.ndarray, i_dv: int) -> List[Union[str, int, float]]:
+    def decode_values(
+        self, x: np.ndarray, i_dv: int = None
+    ) -> List[Union[str, int, float, list]]:
         """
         Return decoded values: converts ordinal and categorical back to their original values.
+
+        If i_dv is given, decoding is done for one specific design variable only.
+        If i_dv=None, decoding will be done for all design variables: 1d input is interpreted as a design vector,
+        2d input is interpreted as a set of design vectors.
         """
-        if len(x.shape) == 2:
-            x_i = x[:, i_dv]
-        elif len(x.shape) == 1:
-            x_i = x
-        else:
-            raise ValueError("Expected either 1 or 2-dimensional matrix!")
-
-        dv = self.design_variables[i_dv]
-        if isinstance(dv, (OrdinalVariable, CategoricalVariable)):
-            values = dv.values
-            decoded_values = [values[int(x_ij)] for x_ij in x_i]
-            return decoded_values
 
-        # No need to decode for integer or float variable
-        return list(x_i)
+        def _decode_dv(x_encoded: np.ndarray, i_dv_decode):
+            dv = self.design_variables[i_dv_decode]
+            if isinstance(dv, (OrdinalVariable, CategoricalVariable)):
+                values = dv.values
+                decoded_values = [values[int(x_ij)] for x_ij in x_encoded]
+                return decoded_values
+
+            # No need to decode integer or float variables
+            return list(x_encoded)
+
+        # Decode one design variable
+        if i_dv is not None:
+            if len(x.shape) == 2:
+                x_i = x[:, i_dv]
+            elif len(x.shape) == 1:
+                x_i = x
+            else:
+                raise ValueError("Expected either 1 or 2-dimensional matrix!")
+
+            # No need to decode for integer or float variable
+            return _decode_dv(x_i, i_dv_decode=i_dv)
+
+        # Decode design vectors
+        n_dv = self.n_dv
+        is_1d = len(x.shape) == 1
+        x_mat = np.atleast_2d(x)
+        if x_mat.shape[1] != n_dv:
+            raise ValueError(
+                f"Incorrect number of inputs, expected {n_dv} design variables, received {x_mat.shape[1]}"
+            )
+
+        decoded_des_vars = [_decode_dv(x_mat[:, i], i_dv_decode=i) for i in range(n_dv)]
+        decoded_des_vectors = [
+            [decoded_des_vars[i][ix] for i in range(n_dv)]
+            for ix in range(x_mat.shape[0])
+        ]
+        return decoded_des_vectors[0] if is_1d else decoded_des_vectors
 
     def sample_valid_x(self, n: int, unfolded=False) -> Tuple[np.ndarray, np.ndarray]:
         """
         Sample n design vectors and additionally return the is_acting matrix.
 
         Parameters
         ----------
```

### Comparing `smt-2.0b3/smt/utils/krg_sampling.py` & `smt-2.0b4/smt/utils/krg_sampling.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/kriging.py` & `smt-2.0b4/smt/utils/kriging.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 
 This package is distributed under New BSD license.
 """
 import warnings
 import numpy as np
 from enum import Enum
 from copy import deepcopy
-
+import os
 from sklearn.cross_decomposition import PLSRegression as pls
 
 from pyDOE2 import bbdesign
 from sklearn.metrics.pairwise import check_pairwise_arrays
 from smt.utils.design_space import BaseDesignSpace, CategoricalVariable
 
-try:
-    from numba import njit, prange
-
-    USE_NUMBA_JIT = True  # Set False to temporarily disable
 
-except ImportError:  # pip install smt[numba]
-    USE_NUMBA_JIT = False
-    prange = range
+USE_NUMBA_JIT = int(os.getenv("USE_NUMBA_JIT", 0))
+prange = range
+if USE_NUMBA_JIT:
+    from numba import njit, prange
 
 """
 Quick benchmarking with the mixed-integer hierarchical Goldstein function indicates the following:
 
 | Scenario                 | No numba | Numba   | Numba with caching | Speedup | Overhead |
 |--------------------------|----------|---------|--------------------|---------|----------|
 | HGoldstein 15 pt DoE     | 1.3 sec  | ~25 sec | 1.1 sec            | 15%     | 24 sec   |
```

### Comparing `smt-2.0b3/smt/utils/line_search.py` & `smt-2.0b4/smt/utils/line_search.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/linear_solvers.py` & `smt-2.0b4/smt/utils/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/misc.py` & `smt-2.0b4/smt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/activation.py` & `smt-2.0b4/smt/utils/neural_net/activation.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/bwd_prop.py` & `smt-2.0b4/smt/utils/neural_net/bwd_prop.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/data.py` & `smt-2.0b4/smt/utils/neural_net/data.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/fwd_prop.py` & `smt-2.0b4/smt/utils/neural_net/fwd_prop.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/loss.py` & `smt-2.0b4/smt/utils/neural_net/loss.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/metrics.py` & `smt-2.0b4/smt/utils/neural_net/metrics.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/model.py` & `smt-2.0b4/smt/utils/neural_net/model.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/neural_net/optimizer.py` & `smt-2.0b4/smt/utils/neural_net/optimizer.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/options_dictionary.py` & `smt-2.0b4/smt/utils/options_dictionary.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/printer.py` & `smt-2.0b4/smt/utils/printer.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/silence.py` & `smt-2.0b4/smt/utils/silence.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt/utils/sm_test_case.py` & `smt-2.0b4/smt/utils/sm_test_case.py`

 * *Files identical despite different names*

### Comparing `smt-2.0b3/smt.egg-info/PKG-INFO` & `smt-2.0b4/smt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smt
-Version: 2.0b3
+Version: 2.0b4
 Summary: The Surrogate Modeling Toolbox (SMT)
 Home-page: https://github.com/SMTorg/smt
 Download-URL: https://github.com/SMTorg/smt/releases
 Author: Mohamed Amine Bouhlel et al.
 Author-email: mbouhlel@umich.edu
 License: BSD-3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `smt-2.0b3/smt.egg-info/SOURCES.txt` & `smt-2.0b4/smt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

