# Comparing `tmp/amazon-braket-algorithm-library-1.3.5.tar.gz` & `tmp/amazon-braket-algorithm-library-1.3.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-algorithm-library-1.3.5.tar", last modified: Mon May 29 16:07:04 2023, max compression
+gzip compressed data, was "amazon-braket-algorithm-library-1.3.5.post0.tar", last modified: Wed Jun  7 16:06:37 2023, max compression
```

## Comparing `amazon-braket-algorithm-library-1.3.5.tar` & `amazon-braket-algorithm-library-1.3.5.post0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.004869 amazon-braket-algorithm-library-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.004869 amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-29 16:07:03.000000 amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-29 16:07:03.000000 amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:07:03.000000 amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-29 16:07:03.000000 amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 16:07:03.000000 amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.004869 amazon-braket-algorithm-library-1.3.5/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.004869 amazon-braket-algorithm-library-1.3.5/src/braket/_algos/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/_algos/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.004869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bells_inequality/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bells_inequality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bernstein_vazirani/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/chsh_inequality/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/chsh_inequality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/deutsch_jozsa/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/grovers_search/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/grovers_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/grovers_search/grovers_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_approximate_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_circuit_born_machine/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_fourier_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_phase_estimation/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_walk/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_walk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/shors/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/shors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/shors/shors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:07:04.008869 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/simons/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/simons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-29 16:06:54.000000 amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/simons/simons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-07 16:06:37.117391 amazon-braket-algorithm-library-1.3.5.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-07 16:06:37.000000 amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-07 16:06:37.000000 amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:06:37.000000 amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 16:06:37.000000 amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 16:06:37.000000 amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/_algos/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/_algos/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.109391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bells_inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bells_inequality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bernstein_vazirani/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/chsh_inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/chsh_inequality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/deutsch_jozsa/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/grovers_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/grovers_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/grovers_search/grovers_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_approximate_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_circuit_born_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_fourier_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_phase_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_walk/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_walk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/shors/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/shors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/shors/shors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:06:37.113391 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/simons/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/simons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-07 16:06:28.000000 amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/simons/simons.py
```

### Comparing `amazon-braket-algorithm-library-1.3.5/LICENSE` & `amazon-braket-algorithm-library-1.3.5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/PKG-INFO` & `amazon-braket-algorithm-library-1.3.5.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-algorithm-library
-Version: 1.3.5
+Version: 1.3.5.post0
 Summary: An open source library of quantum computing algorithms implemented on Amazon Braket
 Home-page: https://github.com/aws-samples/amazon-braket-algorithm-library
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `amazon-braket-algorithm-library-1.3.5/README.md` & `amazon-braket-algorithm-library-1.3.5.post0/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/setup.py` & `amazon-braket-algorithm-library-1.3.5.post0/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/PKG-INFO` & `amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-algorithm-library
-Version: 1.3.5
+Version: 1.3.5.post0
 Summary: An open source library of quantum computing algorithms implemented on Amazon Braket
 Home-page: https://github.com/aws-samples/amazon-braket-algorithm-library
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `amazon-braket-algorithm-library-1.3.5/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt` & `amazon-braket-algorithm-library-1.3.5.post0/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/_algos/_version.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/_algos/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "1.3.5"
+__version__ = "1.3.5.post0"
```

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bells_inequality/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bells_inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/chsh_inequality/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/chsh_inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/grovers_search/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/grovers_search/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/grovers_search/grovers_search.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/grovers_search/grovers_search.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,17 @@
     ovlp: float,
     one_body: np.ndarray,
     lambda_l: np.ndarray,
     u_l: np.ndarray,
     trial_state_circuit: Callable,
     dev: qml.device,
 ) -> complex:
-    r"""This function estimates the integral $\\langle \\Psi_Q|H|\\phi_l\rangle$ with rotated basis.
+    r"""
+    This function estimates the integral :math:`$\\langle \\Psi_Q|H|\\phi_l\rangle$`
+    with rotated basis.
 
     Args:
         walker (ndarray): np.ndarray; matrix representation of the walker state, not necessarily
             orthonormalized.
         ovlp (float): amplitude between walker and the quantum trial state
         one_body (ndarray): (corrected) one-body term in the second quantized hamiltonian
             written in chemist's notation. This term is assumed to be diagonal in the current
```

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,17 @@
         interaction_strength = ising[qubit_pair[0], qubit_pair[1]]
         circ.decomposed_zz_gate(qubit_pair[0], qubit_pair[1], gamma * interaction_strength)
     return circ
 
 
 @circuit.subroutine(register=True)
 def decomposed_zz_gate(qubit0: int, qubit1: int, gamma: float) -> Circuit:
-    """Return a circuit implementing exp(-i gamma Z_i Z_j) using CNOT gates if ZZ not supported.
+    """
+    Return a circuit implementing :math:`exp(-i * \\gamma * Z_i * Z_j)` using CNOT gates
+    if ZZ not supported.
 
     Args:
         qubit0 (int): Index value for the controlling qubit for CNOT gate
         qubit1 (int): Index value for the target qubit for CNOT gate
         gamma (float): Rotation angle to apply parameterized rotation around z
 
     Returns:
```

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,16 @@
             grad[i] = grad_pos - grad_neg
         return grad
 
 
 def _compute_kernel(px: np.ndarray, py: np.ndarray, sigma_list: List[float] = [0.1, 1]) -> float:
     r"""Gaussian radial basis function (RBF) kernel.
 
-    `K(x, y) = sum_\sigma exp(-|x-y|^2/(2\sigma^2 ))`
+    .. math::
+        K(x, y) = sum_\sigma exp(-|x-y|^2/(2\sigma^2 ))
 
     Args:
         px (ndarray): Probability distribution
         py (ndarray): Target probability distribution
         sigma_list (List[float]): Standard deviations of distribution. Defaults to [0.1, 1].
 
     Returns:
@@ -169,19 +170,21 @@
 
 
 def mmd_loss(px: np.ndarray, py: np.ndarray, sigma_list: List[float] = [0.1, 1]) -> float:
     r"""Maximum Mean Discrepancy loss (MMD).
 
     MMD determines if two distributions are equal by looking at the difference between
     their means in feature space.
-    ::
+
+    .. math::
         MMD(x, y) = | \sum_{j=1}^N \phi(y_j) - \sum_{i=1}^N \phi(x_i) |_2^2
 
     With a RBF kernel, we apply the kernel trick to expand MMD to
-    ::
+
+    .. math::
         MMD(x, y) = \sum_{j=1}^N \sum_{j'=1}^N k(y_j, y_{j'})
                 + \sum_{i=1}^N \sum_{i'=1}^N k(x_i, x_{i'})
                 - 2 \sum_{j=1}^N \sum_{i=1}^N k(y_j, x_i)
 
     For the RBF kernel, MMD is zero if and only if the distributions are identical.
 
     Args:
```

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_walk/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_walk/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/shors/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/shors/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/shors/shors.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/shors/shors.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/simons/__init__.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/simons/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.3.5/src/braket/experimental/algorithms/simons/simons.py` & `amazon-braket-algorithm-library-1.3.5.post0/src/braket/experimental/algorithms/simons/simons.py`

 * *Files identical despite different names*

