# Comparing `tmp/google-vizier-0.1.5.tar.gz` & `tmp/google-vizier-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-vizier-0.1.5.tar", last modified: Tue May  2 21:57:00 2023, max compression
+gzip compressed data, was "google-vizier-0.1.6.tar", last modified: Wed Jun  7 15:39:35 2023, max compression
```

## Comparing `google-vizier-0.1.5.tar` & `google-vizier-0.1.6.tar`

### file list

```diff
@@ -1,329 +1,345 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.202545 google-vizier-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 21:56:38.000000 google-vizier-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-02 21:57:00.202545 google-vizier-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-02 21:56:38.000000 google-vizier-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/google_vizier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:57:00.202545 google-vizier-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-02 21:56:38.000000 google-vizier-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/algorithms/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/algorithms/core/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/core/abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/
--rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/acquisitions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/output_warpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/output_warpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/yjt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp_bandit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/grid_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_param_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    27583 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/vectorized_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/vectorized_base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/random/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/regression/
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/optimizer_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/test_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/state_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo/
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob/
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/jax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/jax/models/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/tuned_gp_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/tuned_gp_models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/jax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/xla_pareto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/xla_pareto_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/pythia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/pythia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/vizier_test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/pythia_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/pyvizier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyvizier/oss/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyvizier/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/pythia/study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.194544 google-vizier-0.1.5/vizier/_src/pyvizier/shared/
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/context_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    47569 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/study.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.194544 google-vizier-0.1.5/vizier/_src/raytune/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/run_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/run_tune_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.194544 google-vizier-0.1.5/vizier/_src/service/
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/clients_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/datastore_test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/grpc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/policy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/pythia_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/pythia_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/ram_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/ram_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/service_policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/service_policy_supporter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/sql_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/sql_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/stubs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/stubs_util_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/_src/service/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12258 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    36086 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/algorithms/designers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/algorithms/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/hpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/nas/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/client/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/client/client_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/client/client_abc_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/interfaces/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/jax/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/jax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/jax/optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyglove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pythia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyvizier/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    44020 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/embedder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/input_warping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/input_warping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/multimetric/xla_pareto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/raytune/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/raytune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/protos/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/testing/test_studies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.202545 google-vizier-0.1.5/vizier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/attrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/attrs_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/profiler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 15:39:10.000000 google-vizier-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-06-07 15:39:35.456343 google-vizier-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-07 15:39:10.000000 google-vizier-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.404343 google-vizier-0.1.6/google_vizier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-06-07 15:39:35.000000 google-vizier-0.1.6/google_vizier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-07 15:39:35.000000 google-vizier-0.1.6/google_vizier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:39:35.000000 google-vizier-0.1.6/google_vizier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:39:35.000000 google-vizier-0.1.6/google_vizier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 15:39:35.000000 google-vizier-0.1.6/google_vizier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 15:39:35.000000 google-vizier-0.1.6/google_vizier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:39:35.456343 google-vizier-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-07 15:39:10.000000 google-vizier-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.404343 google-vizier-0.1.6/vizier/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.404343 google-vizier-0.1.6/vizier/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.404343 google-vizier-0.1.6/vizier/_src/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.404343 google-vizier-0.1.6/vizier/_src/algorithms/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/classification/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/classification/classifiers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.404343 google-vizier-0.1.6/vizier/_src/algorithms/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/core/abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.412343 google-vizier-0.1.6/vizier/_src/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/bocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/bocs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/cmaes_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.412343 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/emukit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/emukit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.412343 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/acquisitions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24363 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/output_warpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/output_warpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/yjt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/gp_bandit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/grid_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/harmonica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/harmonica_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/quasi_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/quasi_random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/scalarizing_designer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/designers/scalarizing_designer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.416343 google-vizier-0.1.6/vizier/_src/algorithms/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/ensemble/ensemble_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/ensemble/ensemble_design_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.416343 google-vizier-0.1.6/vizier/_src/algorithms/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/evolution/numpy_populations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/evolution/numpy_populations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/evolution/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.420343 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/designer_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_param_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27893 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/vectorized_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/optimizers/vectorized_base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.420343 google-vizier-0.1.6/vizier/_src/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/policies/designer_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/policies/designer_policy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/policies/random_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/policies/random_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.420343 google-vizier-0.1.6/vizier/_src/algorithms/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/random/random_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/random/random_sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.420343 google-vizier-0.1.6/vizier/_src/algorithms/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/regression/trial_regression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/regression/trial_regression_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.424343 google-vizier-0.1.6/vizier/_src/algorithms/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/testing/comparator_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/testing/comparator_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/testing/optimizer_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/algorithms/testing/test_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.400343 google-vizier-0.1.6/vizier/_src/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.424343 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)    25226 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/convergence_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/simple_regret_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/state_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.432343 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.432343 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/experimenter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.432343 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob/
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/switch_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.432343 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.432343 google-vizier-0.1.6/vizier/_src/benchmarks/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_state_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.432343 google-vizier-0.1.6/vizier/_src/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/gp_bandit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.436343 google-vizier-0.1.6/vizier/_src/jax/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/gaussian_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/gaussian_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/hebo_gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/hebo_gp_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/mask_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/mask_features_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/tuned_gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/models/tuned_gp_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.436343 google-vizier-0.1.6/vizier/_src/jax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/optimizers/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/optimizers/optimizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/predictive_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/predictive_fns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/stochastic_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/stochastic_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/xla_pareto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/jax/xla_pareto_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.436343 google-vizier-0.1.6/vizier/_src/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/oss_vizier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/oss_vizier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/pythia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/pythia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyglove/vizier_test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.440343 google-vizier-0.1.6/vizier/_src/pythia/
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pythia/local_policy_supporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pythia/local_policy_supporters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pythia/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pythia/policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pythia/pythia_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.400343 google-vizier-0.1.6/vizier/_src/pyvizier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.440343 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/hypervolume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/pareto_optimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/safety_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.440343 google-vizier-0.1.6/vizier/_src/pyvizier/oss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/automated_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/automated_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/metadata_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33067 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/proto_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/proto_converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/study_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/oss/study_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.440343 google-vizier-0.1.6/vizier/_src/pyvizier/pythia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/pythia/study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.444343 google-vizier-0.1.6/vizier/_src/pyvizier/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/base_study_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/base_study_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24318 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47570 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_iterators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/pyvizier/shared/trial_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.444343 google-vizier-0.1.6/vizier/_src/raytune/
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/raytune/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/raytune/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/raytune/run_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/raytune/run_tune_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/raytune/vizier_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/raytune/vizier_search_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/_src/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/clients_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/datastore_test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/grpc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/policy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/pythia_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/pythia_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/ram_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/ram_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/service_policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/service_policy_supporter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/sql_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/sql_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/stubs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/stubs_util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/_src/service/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/vizier_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/vizier_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/vizier_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36086 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/vizier_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/_src/service/vizier_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/algorithms/designers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/algorithms/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/benchmarks/experimenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/benchmarks/experimenters/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/benchmarks/experimenters/hpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/benchmarks/experimenters/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/benchmarks/experimenters/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.448343 google-vizier-0.1.6/vizier/benchmarks/experimenters/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/benchmarks/experimenters/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.452343 google-vizier-0.1.6/vizier/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/client/client_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/client/client_abc_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.452343 google-vizier-0.1.6/vizier/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/interfaces/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.452343 google-vizier-0.1.6/vizier/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/jax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/jax/optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.452343 google-vizier-0.1.6/vizier/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyglove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pythia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.452343 google-vizier-0.1.6/vizier/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.452343 google-vizier-0.1.6/vizier/pyvizier/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44805 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43993 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/embedder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/feature_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/feature_mapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/input_warping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/input_warping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/padded_trial_to_array_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/padded_trial_to_array_converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/spatio_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/converters/spatio_temporal_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/pyvizier/multimetric/xla_pareto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/raytune/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/raytune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/service/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/service/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/service/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/service/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/service/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/service/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/service/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/service/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/testing/test_studies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:39:35.456343 google-vizier-0.1.6/vizier/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/utils/attrs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/utils/attrs_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/utils/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-07 15:39:10.000000 google-vizier-0.1.6/vizier/utils/profiler_test.py
```

### Comparing `google-vizier-0.1.5/LICENSE` & `google-vizier-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/PKG-INFO` & `google-vizier-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier
-Version: 0.1.5
+Version: 0.1.6
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
@@ -28,19 +28,16 @@
 
 <figure>
 <img src="docs/assets/vizier_logo2.png" width=20% align="right"/>
 </figure>
 
 # Open Source Vizier: Reliable and Flexible Black-Box Optimization.
 [![PyPI version](https://badge.fury.io/py/google-vizier.svg)](https://badge.fury.io/py/google-vizier)
-![Continuous Integration (Core)](https://github.com/google/vizier/workflows/pytest_core/badge.svg)
-![Continuous Integration (Clients)](https://github.com/google/vizier/workflows/pytest_clients/badge.svg)
-![Continuous Integration (Algorithms)](https://github.com/google/vizier/workflows/pytest_algorithms/badge.svg)
-![Continuous Integration (Benchmarks)](https://github.com/google/vizier/workflows/pytest_benchmarks/badge.svg)
-![Continuous Integration (Docs)](https://github.com/google/vizier/workflows/docs/badge.svg)
+![Continuous Integration](https://github.com/google/vizier/workflows/ci/badge.svg)
+![Docs](https://github.com/google/vizier/workflows/docs/badge.svg)
 
   [**Google AI Blog**](https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html)
 | [**Getting Started**](#getting_started)
 | [**Documentation**](#documentation)
 | [**Installation**](#installation)
 | [**Citing and Highlights**](#citing_vizier)
```

### Comparing `google-vizier-0.1.5/README.md` & `google-vizier-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 <figure>
 <img src="docs/assets/vizier_logo2.png" width=20% align="right"/>
 </figure>
 
 # Open Source Vizier: Reliable and Flexible Black-Box Optimization.
 [![PyPI version](https://badge.fury.io/py/google-vizier.svg)](https://badge.fury.io/py/google-vizier)
-![Continuous Integration (Core)](https://github.com/google/vizier/workflows/pytest_core/badge.svg)
-![Continuous Integration (Clients)](https://github.com/google/vizier/workflows/pytest_clients/badge.svg)
-![Continuous Integration (Algorithms)](https://github.com/google/vizier/workflows/pytest_algorithms/badge.svg)
-![Continuous Integration (Benchmarks)](https://github.com/google/vizier/workflows/pytest_benchmarks/badge.svg)
-![Continuous Integration (Docs)](https://github.com/google/vizier/workflows/docs/badge.svg)
+![Continuous Integration](https://github.com/google/vizier/workflows/ci/badge.svg)
+![Docs](https://github.com/google/vizier/workflows/docs/badge.svg)
 
   [**Google AI Blog**](https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html)
 | [**Getting Started**](#getting_started)
 | [**Documentation**](#documentation)
 | [**Installation**](#installation)
 | [**Citing and Highlights**](#citing_vizier)
```

### Comparing `google-vizier-0.1.5/google_vizier.egg-info/PKG-INFO` & `google-vizier-0.1.6/google_vizier.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier
-Version: 0.1.5
+Version: 0.1.6
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
@@ -28,19 +28,16 @@
 
 <figure>
 <img src="docs/assets/vizier_logo2.png" width=20% align="right"/>
 </figure>
 
 # Open Source Vizier: Reliable and Flexible Black-Box Optimization.
 [![PyPI version](https://badge.fury.io/py/google-vizier.svg)](https://badge.fury.io/py/google-vizier)
-![Continuous Integration (Core)](https://github.com/google/vizier/workflows/pytest_core/badge.svg)
-![Continuous Integration (Clients)](https://github.com/google/vizier/workflows/pytest_clients/badge.svg)
-![Continuous Integration (Algorithms)](https://github.com/google/vizier/workflows/pytest_algorithms/badge.svg)
-![Continuous Integration (Benchmarks)](https://github.com/google/vizier/workflows/pytest_benchmarks/badge.svg)
-![Continuous Integration (Docs)](https://github.com/google/vizier/workflows/docs/badge.svg)
+![Continuous Integration](https://github.com/google/vizier/workflows/ci/badge.svg)
+![Docs](https://github.com/google/vizier/workflows/docs/badge.svg)
 
   [**Google AI Blog**](https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html)
 | [**Getting Started**](#getting_started)
 | [**Documentation**](#documentation)
 | [**Installation**](#installation)
 | [**Citing and Highlights**](#citing_vizier)
```

### Comparing `google-vizier-0.1.5/google_vizier.egg-info/SOURCES.txt` & `google-vizier-0.1.6/google_vizier.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
 vizier/_src/algorithms/designers/eagle_strategy/testing.py
 vizier/_src/algorithms/designers/gp/acquisitions.py
 vizier/_src/algorithms/designers/gp/acquisitions_test.py
 vizier/_src/algorithms/designers/gp/output_warpers.py
 vizier/_src/algorithms/designers/gp/output_warpers_test.py
 vizier/_src/algorithms/designers/gp/yjt.py
+vizier/_src/algorithms/ensemble/ensemble_design.py
+vizier/_src/algorithms/ensemble/ensemble_design_test.py
 vizier/_src/algorithms/evolution/__init__.py
 vizier/_src/algorithms/evolution/nsga2.py
 vizier/_src/algorithms/evolution/nsga2_test.py
 vizier/_src/algorithms/evolution/numpy_populations.py
 vizier/_src/algorithms/evolution/numpy_populations_test.py
 vizier/_src/algorithms/evolution/templates.py
 vizier/_src/algorithms/optimizers/__init__.py
@@ -116,31 +118,38 @@
 vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
 vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
 vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
 vizier/_src/benchmarks/experimenters/sparse_experimenter.py
 vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
 vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
 vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
+vizier/_src/benchmarks/experimenters/switch_experimenter.py
+vizier/_src/benchmarks/experimenters/switch_experimenter_test.py
 vizier/_src/benchmarks/experimenters/combo/common.py
 vizier/_src/benchmarks/experimenters/hpob/handler.py
 vizier/_src/benchmarks/experimenters/synthetic/bbob.py
 vizier/_src/benchmarks/runners/benchmark_runner.py
 vizier/_src/benchmarks/runners/benchmark_runner_test.py
 vizier/_src/benchmarks/runners/benchmark_state.py
 vizier/_src/benchmarks/runners/benchmark_state_test.py
+vizier/_src/jax/gp_bandit_utils.py
+vizier/_src/jax/predictive_fns.py
+vizier/_src/jax/predictive_fns_test.py
 vizier/_src/jax/stochastic_process_model.py
 vizier/_src/jax/stochastic_process_model_test.py
 vizier/_src/jax/types.py
 vizier/_src/jax/xla_pareto.py
 vizier/_src/jax/xla_pareto_test.py
 vizier/_src/jax/models/__init__.py
 vizier/_src/jax/models/gaussian_process_model.py
 vizier/_src/jax/models/gaussian_process_model_test.py
 vizier/_src/jax/models/hebo_gp_model.py
 vizier/_src/jax/models/hebo_gp_model_test.py
+vizier/_src/jax/models/mask_features.py
+vizier/_src/jax/models/mask_features_test.py
 vizier/_src/jax/models/tuned_gp_models.py
 vizier/_src/jax/models/tuned_gp_models_test.py
 vizier/_src/jax/optimizers/optimizers.py
 vizier/_src/jax/optimizers/optimizers_test.py
 vizier/_src/pyglove/algorithms.py
 vizier/_src/pyglove/backend.py
 vizier/_src/pyglove/client.py
@@ -189,14 +198,16 @@
 vizier/_src/pyvizier/shared/study.py
 vizier/_src/pyvizier/shared/trial.py
 vizier/_src/pyvizier/shared/trial_test.py
 vizier/_src/raytune/converters.py
 vizier/_src/raytune/converters_test.py
 vizier/_src/raytune/run_tune.py
 vizier/_src/raytune/run_tune_test.py
+vizier/_src/raytune/vizier_search.py
+vizier/_src/raytune/vizier_search_test.py
 vizier/_src/service/clients.py
 vizier/_src/service/clients_test.py
 vizier/_src/service/constants.py
 vizier/_src/service/custom_errors.py
 vizier/_src/service/datastore.py
 vizier/_src/service/datastore_test_lib.py
 vizier/_src/service/grpc_util.py
@@ -244,14 +255,18 @@
 vizier/pyvizier/converters/core_test.py
 vizier/pyvizier/converters/embedder.py
 vizier/pyvizier/converters/embedder_test.py
 vizier/pyvizier/converters/feature_mapper.py
 vizier/pyvizier/converters/feature_mapper_test.py
 vizier/pyvizier/converters/input_warping.py
 vizier/pyvizier/converters/input_warping_test.py
+vizier/pyvizier/converters/padded_trial_to_array_converter.py
+vizier/pyvizier/converters/padded_trial_to_array_converter_test.py
+vizier/pyvizier/converters/padding.py
+vizier/pyvizier/converters/padding_test.py
 vizier/pyvizier/converters/spatio_temporal.py
 vizier/pyvizier/converters/spatio_temporal_test.py
 vizier/pyvizier/multimetric/__init__.py
 vizier/pyvizier/multimetric/xla_pareto.py
 vizier/raytune/__init__.py
 vizier/service/__init__.py
 vizier/service/clients/__init__.py
```

### Comparing `google-vizier-0.1.5/google_vizier.egg-info/requires.txt` & `google-vizier-0.1.6/google_vizier.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 attrs==21.4.0
 absl-py>=1.0.0
 numpy>=1.21.5
-protobuf<4.0,>=3.6
+protobuf>=3.6
 portpicker>=1.3.1
-grpcio<=1.48.2,>=1.35.0
-grpcio-tools<=1.48.2,>=1.35.0
+grpcio>=1.35.0
+grpcio-tools>=1.35.0
 googleapis-common-protos>=1.56.4
 sqlalchemy==1.4
 
 [algorithms]
 emukit==0.4.9
 scipy<1.8.0,>1.2.3
 cvxpy==1.2.1
@@ -20,20 +20,20 @@
 [benchmarks]
 ale-py
 dopamine-rl
 nats_bench
 xgboost==1.5.1
 
 [jax]
-jax>=0.4.2
-jaxlib>=0.4.2
-jaxopt>=0.5.5
-flax>=0.6.4
-optax>=0.1.4
-chex>=0.1.6
+jax>=0.4.10
+jaxlib>=0.4.10
+jaxopt>=0.7
+flax>=0.6.10
+optax>=0.1.5
+chex>=0.1.7
 tfp-nightly[jax]
 
 [test]
 coverage<=6.4.2,>=4.5
 mock<=4.0.3,>=3.0
 pytest
```

### Comparing `google-vizier-0.1.5/setup.py` & `google-vizier-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/__init__.py` & `google-vizier-0.1.6/vizier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 import sys
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 PROTO_ROOT = os.path.realpath(os.path.join(THIS_DIR, "_src", "service"))
 
 sys.path.append(PROTO_ROOT)
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

### Comparing `google-vizier-0.1.5/vizier/_src/__init__.py` & `google-vizier-0.1.6/vizier/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers.py` & `google-vizier-0.1.6/vizier/_src/algorithms/classification/classifiers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/classification/classifiers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/core/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/core/abstractions.py` & `google-vizier-0.1.6/vizier/_src/algorithms/core/abstractions.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,58 +86,69 @@
     Returns:
       New suggestions.
     """
     pass
 
 
 class Designer(_SuggestionAlgorithm):
-  """Suggestion algorithm for sequential usage.
+  """Interface for sequential suggestion algorithms.
 
-  Designer is the recommended interface for implementing commonly used
-  algorithms such as GP-UCB and evolutionary algorithms. A Designer can be
-  wrapped into a pythia `Policy` via `DesignerPolicy` (stateless) or
-  '(Partially)SerializableDesignerPolicy' (stateful).
-
-  If your Designer is stateless it should match with 'DesignerPolicy' which
-  is responsible for calling the 'update' method and pass all completed trials
-  since the beginning of the trials as well as all currently active
-  trials.
-
-  If your Designer can benefit from a persistent state (stateful), implement
-  `(Partially)SerializableDesigner` interface and use
-  `(Partially)SerializableDesignerPolicy` to wrap it.
-  Vizier service will serialize the Designer's state in DB, restore it for
-  the next usage, and update it with the newly completed and active trials
-  since the last suggestion.
-
-  IMPORTANT: If your Designer changes its state inside `suggest()` (e.g. to
-  incorporate its own suggestions before completion), then use
-  (Partially)SerializableDesigner interface instead or take advantage of the
-  'all_active' trials argument.
-
-  Note that when run inside a service binary, a Designer instance does not
-  persist during the lifetime of a `Study`.
+  A Designer can be wrapped into a pythia `Policy` via `DesignerPolicy`.
+  Prefer implementing a `Designer` interface over `Policy` interface, for
+  shared error handling, performance monitoring, logging, etc.
+
+
+  A big limitation of vanilla `DesignerPolicy` is that it does not retain states
+  between consecutive suggestion requests. It creates a new `Designer` from
+  scratch and calls `Designer.update` with all trials of the study.
+  Many algorithms with a compact state, such as evolutionary search algorithms,
+  can gain a huge performance boost from incremental updates. (Side note:
+  GP-UCB does not fit into this category because its state includes
+  all previous observations, which is not compact).
+
+  If your Designer can take advantage of a persistent state, implement
+  `(Partially)SerializableDesigner` interface, which can be wrapped into
+  `(Partially)SerializableDesignerPolicy`.
+  These Policies serialize the Designer's state, store it in Vizier DB, and
+  load it for the next suggest operation. `Designer.update()` is called only
+  with the newly completed trials (delta).
+
+  IMPORTANT: `Designer` should not change its state inside `suggest()` (e.g. to
+  incorporate its own suggestions before completion). If it does, use
+  (Partially)SerializableDesigner interface.
+
+  NOTE: When run inside a service binary, a `Designer` instance does not
+  persist during the lifetime of a `Study`. This goes true even for the
+  serializable variants; the states are recovered into a new `Designer`
+  instance.
+
+  NOTE: `Designer`s are designed to be used directly in benchmarks without
+  a `Policy` wrapper. Create a single `Designer` instance for the entire study,
+  and incrementally update its state with delta only.
   """
 
   @abc.abstractmethod
   def update(
       self, completed: CompletedTrials, all_active: ActiveTrials
   ) -> None:
-    """Incorporates completed and active trials into the designer's state.
-
-    In production, 'completed' refer to all the completed trials in the study.
-    In benchmarking, 'completed' refer to newly created trials that the designer
-      hasn't seen yet ("delta").
+    """Incorporates trials into the designer's state.
 
-    In both production and benchmarking, 'all_active' refers to ALL the current
-    ACTIVE trials.
+    Example:
+      [t1, t2] # CompletedTrials
+      [t3, t4] # Active Trials
+      designer.update([t1], [t3])  # state includes: t1 and t3.
+      designer.update([t2])        # state includes: t1 and t2 (not t3).
+      designer.update([], [t3,t4]) # state includes: t1, t2, t3, and t4.
+      designer.update([], [t3])    # state includes: t1, t2, and t3.
 
     Arguments:
-      completed: COMPLETED trials.
-      all_active: ACTIVE (aka PENDING) trials.
+      completed: COMPLETED trials that this Designer should additionaly
+        incorporate.
+      all_active: All ACTIVE (aka PENDING) trials in the study from its
+        beginning.
     """
     pass
 
 
 @attr.define(frozen=True)
 class Prediction:
   """Container to hold predictions.
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/bocs.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/bocs_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/cmaes.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/cmaes_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/serialization.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/testing.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/eagle_strategy/testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/emukit.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/emukit_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/output_warpers.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/output_warpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,19 +593,24 @@
   _max_value: Optional[types.Array] = None
   _bijector: tfb.Bijector = attr.field(init=False)
 
   def __attrs_post_init__(self):
     if self.low_bound >= self.high_bound:
       raise ValueError('low_bound needs to be smaller than high_bound.')
 
-  def _validate(self) -> None:
+  def _validate(self, y: types.Array) -> None:
     if self._min_value is None or self._max_value is None:
       raise ValueError(
           'Need to set min_value and max_value. Make sure to call `fit` first.'
       )
+    if y.shape[-1] != self._min_value.shape[-1]:
+      raise ValueError(
+          f'The input array last dimension {y.shape[-1]} is not the same as'
+          f' expected {self._min_value.shape[-1]}. Input shape: {y.shape}.'
+      )
 
   def fit(self, y: types.Array) -> None:
     """Find min/max for each metric to be used in the linear transformation."""
     # y shape: (num_samples, num_metrics)
     logging.info(
         'LinearOutputWarping fit is called with shape: %s', str(y.shape)
     )
@@ -628,19 +633,19 @@
         ),
         tfb.Shift(-self._min_value),
     ])
 
   def warp(self, y: types.Array) -> jax.Array:
     """Warp the y values into [low_bound, high_bound]."""
     # y shape: (num_samples, num_metrics)
-    self._validate()
+    self._validate(y)
     return self._bijector.forward(y)
 
   def unwarp(self, y: types.Array) -> jax.Array:
     """Un-warp the y values into [min_value, max_value]."""
     # y shape: (num_samples, num_metrics)
-    self._validate()
+    self._validate(y)
     return self._bijector.inverse(y)
 
   @property
   def bijector(self) -> tfb.Bijector:
     return self._bijector
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/output_warpers_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/output_warpers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/yjt.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/gp/yjt.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/gp_bandit.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/gp_bandit.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,38 +18,70 @@
 
 A Python implementation of Google Vizier's GP-Bandit algorithm.
 """
 # pylint: disable=logging-fstring-interpolation, g-long-lambda
 
 import copy
 import datetime
+import functools
 import json
 import random
-from typing import Sequence, Optional
+from typing import Any, Optional, Sequence, Union
 
 from absl import logging
 import attr
 import jax
 import numpy as np
 from vizier import algorithms as vza
 from vizier import pyvizier as vz
 from vizier._src.algorithms.designers import quasi_random
 from vizier._src.algorithms.designers.gp import acquisitions
 from vizier._src.algorithms.designers.gp import output_warpers
 from vizier._src.algorithms.optimizers import eagle_strategy as es
 from vizier._src.algorithms.optimizers import vectorized_base as vb
+from vizier._src.jax import gp_bandit_utils
+from vizier._src.jax import predictive_fns
 from vizier._src.jax import stochastic_process_model as sp
 from vizier._src.jax import types
 from vizier._src.jax.models import tuned_gp_models
 from vizier._src.jax.optimizers import optimizers
 from vizier.pyvizier import converters
+from vizier.pyvizier.converters import feature_mapper
+from vizier.pyvizier.converters import padding
 from vizier.utils import json_utils
 from vizier.utils import profiler
 
 
+# Define top-level JIT-ed versions of some library functions. See
+# `gp_bandit_utils.py` for function documentation.
+jit_precompute_cholesky = profiler.record_runtime(
+    jax.jit(gp_bandit_utils.precompute_cholesky, static_argnames=('model',)),
+    name_prefix='VizierGPBandit',
+    name='precompute_cholesky',
+)
+
+jit_vmap_precompute_cholesky = profiler.record_runtime(
+    jax.jit(
+        jax.vmap(gp_bandit_utils.precompute_cholesky, in_axes=(None, None, 0)),
+        static_argnames=('model',),
+    ),
+    name_prefix='VizierGPBandit',
+    name='vmap_precompute_cholesky',
+)
+
+jit_optimize_acquisition = profiler.record_runtime(
+    jax.jit(
+        gp_bandit_utils.optimize_acquisition,
+        static_argnames=('count', 'model', 'use_vmap', 'mapper'),
+    ),
+    name_prefix='VizierGPBandit',
+    name='optimize_acquisition',
+)
+
+
 @attr.define(auto_attribs=False)
 class VizierGPBandit(vza.Designer, vza.Predictor):
   """GP-Bandit using a Flax model.
 
   A minimal example of creating this designer:
   problem = vz.ProblemStatement(...)  # Configure a minimal problem statement.
   designer = VizierGPBandit(problem)
@@ -71,25 +103,31 @@
       acqusition function to use.
     use_trust_region: Uses trust region to constrain initial exploration.
     rng: If not set, uses random numbers.
     metadata_ns: Metadata namespace that this designer writes to.
   """
 
   _problem: vz.ProblemStatement = attr.field(kw_only=False)
-  _acquisition_optimizer: vb.VectorizedOptimizer = attr.field(
+  _acquisition_optimizer_factory: vb.VectorizedOptimizerFactory = attr.field(
       kw_only=True,
-      factory=lambda: VizierGPBandit.default_acquisition_optimizer,
+      factory=lambda: VizierGPBandit.default_acquisition_optimizer_factory,
   )
   _ard_optimizer: optimizers.Optimizer[types.ParameterDict] = attr.field(
       factory=lambda: VizierGPBandit.default_ard_optimizer_noensemble,
       kw_only=True,
   )
   _num_seed_trials: int = attr.field(default=1, kw_only=True)
-  _acquisition_builder: acquisitions.AcquisitionBuilder = attr.field(
-      factory=acquisitions.GPBanditAcquisitionBuilder, kw_only=True
+  _acquisition_function: acquisitions.AcquisitionFunction = attr.field(
+      factory=acquisitions.UCB, kw_only=True
+  )
+  _use_categorical_kernel: bool = attr.field(default=False, kw_only=True)
+  # Whether to pad all inputs, and what type of schedule to use. This is to
+  # ensure fewer JIT compilation passes.
+  _padding_schedule: Optional[padding.PaddingSchedule] = attr.field(
+      default=None, kw_only=True
   )
   _use_trust_region: bool = attr.field(default=True, kw_only=True)
   _rng: jax.random.KeyArray = attr.field(
       factory=lambda: jax.random.PRNGKey(random.getrandbits(32)), kw_only=True
   )
   _metadata_ns: str = attr.field(
       default='oss_gp_bandit', kw_only=True, init=False
@@ -100,60 +138,114 @@
   # ------------------------------------------------------------------
   _trials: list[vz.Trial] = attr.field(factory=list, init=False)
   # The number of trials that have been incorporated
   # into the designer state (Cholesky decomposition, ARD).
   _incorporated_trials_count: int = attr.field(
       default=0, kw_only=True, init=False
   )
-  # Numpy array representing the current trials' features.
-  _features: types.Array = attr.field(init=False)
-  # Numpy array representing the current recent trials' metrics.
-  _labels: types.Array = attr.field(init=False)
-  # The current designer state (Cholesky decomposition, model params).
-  _state: types.ModelState = attr.field(init=False)
-  # The current GP model.
-  _model: sp.StochasticProcessModel = attr.field(init=False)
+  _acquisition_optimizer: vb.VectorizedOptimizer = attr.field(init=False)
   _output_warper_pipeline: output_warpers.OutputWarperPipeline = attr.field(
       init=False
   )
+  _feature_mapper: Optional[
+      feature_mapper.ContinuousCategoricalFeatureMapper
+  ] = attr.field(init=False, default=None)
+  _last_computed_state: types.GPState = attr.field(init=False)
+
   # ------------------------------------------------------------------
   # Below are class contants which are not attr fields.
   # ------------------------------------------------------------------
   # Only one of these optimizers will be used.
   # `default_ard_optimizer_ensemble` returns the best 5 parameter values for
   # ensembling, while `default_ard_optimizer_noensemble` returns only
   # the single best parameter value.
   default_ard_optimizer_ensemble = optimizers.JaxoptLbfgsB(
       random_restarts=8, best_n=5
   )
   default_ard_optimizer_noensemble = optimizers.JaxoptLbfgsB(
       random_restarts=4, best_n=1
   )
-  default_acquisition_optimizer = vb.VectorizedOptimizer(
-      strategy_factory=es.VectorizedEagleStrategyFactory())
+  default_acquisition_optimizer_factory = vb.VectorizedOptimizerFactory(
+      strategy_factory=es.VectorizedEagleStrategyFactory()
+  )
 
   def __attrs_post_init__(self):
     # Extra validations
     if self._problem.search_space.is_conditional:
       raise ValueError(f'{type(self)} does not support conditional search.')
     elif len(self._problem.metric_information) != 1:
       raise ValueError(f'{type(self)} works with exactly one metric.')
+    if self._use_categorical_kernel and self._padding_schedule:
+      raise ValueError(
+          f'{type(self)} does not support padding with categorical kernel.'
+          f' use_categorical_kernel = {self._use_categorical_kernel},'
+          f' padding_schedule = {self._padding_schedule}.'
+      )
     # Extra initializations.
     # Discrete parameters are continuified to account for their actual values.
-    self._converter = converters.TrialToArrayConverter.from_study_config(
-        self._problem,
-        scale=True,
-        pad_oovs=True,
-        max_discrete_indices=0,
-        flip_sign_for_minimization_metrics=True,
-    )
+    if self._padding_schedule:
+      self._converter = (
+          converters.PaddedTrialToArrayConverter.from_study_config(
+              self._problem,
+              scale=True,
+              pad_oovs=True,
+              padding_schedule=self._padding_schedule,
+              max_discrete_indices=0,
+              flip_sign_for_minimization_metrics=True,
+          )
+      )
+    else:
+      self._converter = converters.TrialToArrayConverter.from_study_config(
+          self._problem,
+          scale=True,
+          pad_oovs=True,
+          max_discrete_indices=0,
+          flip_sign_for_minimization_metrics=True,
+      )
     self._quasi_random_sampler = quasi_random.QuasiRandomDesigner(
         self._problem.search_space
     )
     self._output_warper_pipeline = output_warpers.create_default_warper()
+    if self._use_categorical_kernel:
+      self._feature_mapper = feature_mapper.ContinuousCategoricalFeatureMapper(
+          self._converter
+      )
+    self._acquisition_optimizer = self._acquisition_optimizer_factory(
+        self._converter
+    )
+    acquisition_problem = copy.deepcopy(self._problem)
+    if isinstance(
+        self._acquisition_function, acquisitions.MultiAcquisitionFunction
+    ):
+      acquisition_config = vz.MetricsConfig()
+      for k in self._acquisition_function.acquisition_fns.keys():
+        acquisition_config.append(
+            vz.MetricInformation(
+                name=k,
+                goal=vz.ObjectiveMetricGoal.MAXIMIZE,
+            )
+        )
+    else:
+      acquisition_config = vz.MetricsConfig(
+          metrics=[
+              vz.MetricInformation(
+                  name='acquisition', goal=vz.ObjectiveMetricGoal.MAXIMIZE
+              )
+          ]
+      )
+
+    acquisition_problem.metric_information = acquisition_config
+    self._acquisition_problem = acquisition_problem
+
+  def _build_model(self, features):
+    if self._use_categorical_kernel:
+      return tuned_gp_models.VizierGaussianProcessWithCategorical.build_model(
+          features
+      )
+    return tuned_gp_models.VizierGaussianProcess.build_model(features)
 
   @property
   def _use_vmap(self):
     """Returns whether ensemble of parameters is used which requires vmap."""
     # Derived classes of `optimizers.Optimizer` have a `best_n` property that
     # indicates whether the optimizer trains an ensemble of parameters and
     # therefore whether vmap should be used.
@@ -168,14 +260,16 @@
     del all_active
     self._trials.extend(copy.deepcopy(completed.trials))
 
   @property
   def _metric_info(self) -> vz.MetricInformation:
     return self._problem.metric_information.item()
 
+  # TODO: Check the latency of `_generate_seed_trials` and look
+  # into reducing it.
   @profiler.record_runtime(
       name_prefix='VizierGPBandit', name='generate_seed_trials'
   )
   def _generate_seed_trials(self, count: int) -> Sequence[vz.TrialSuggestion]:
     """Generate seed trials.
 
     The first seed trial is chosen as the search space center, the rest of the
@@ -210,147 +304,213 @@
     return seed_suggestions
 
   @profiler.record_runtime(
       name_prefix='VizierGPBandit', name='convert_trials_to_arrays'
   )
   def _convert_trials_to_arrays(
       self, trials: Sequence[vz.Trial]
-  ) -> tuple[types.Array, types.Array]:
+  ) -> tuple[
+      Union[types.MaybePaddedArray, types.ContinuousAndCategoricalArray],
+      types.MaybePaddedArray,
+  ]:
     """Convert trials to scaled features and warped labels."""
-    features, labels = self._converter.to_xy(self._trials)
+    features, pre_labels = self._converter.to_xy(self._trials)
     logging.info(
         'Transforming the labels of shape %s. Features has shape: %s',
-        labels.shape,
+        pre_labels.shape,
         features.shape,
     )
+    # Map to continuous and categorical.
+    if self._use_categorical_kernel:
+      features = self._feature_mapper.map(features)
+
+    labels = pre_labels
+    if self._padding_schedule:
+      # Labels coming from the converter will have shape [P, 1], where P >= T
+      # the number of trials.
+      padded_labels = pre_labels.padded_array
+      # Unpad labels to have shape [T, 1].
+      # This is because the warper may take into account all labels, which may
+      # be NaN.
+      labels = padded_labels[: len(self._trials)]
+
     # Warp the output.
     labels = self._output_warper_pipeline.warp(labels)
     labels = labels.reshape([-1])
+
+    # Pad back
+    if self._padding_schedule:
+      # Pad back to shape [P, 1].
+      padded_labels = np.concatenate(
+          [labels, padded_labels[len(self._trials) :, 0]], axis=0
+      )
+      labels = padding.PaddedArray(
+          padded_array=padded_labels, is_missing=pre_labels.is_missing
+      )
     logging.info('Transformed the labels. Now has shape: %s', labels.shape)
     return features, labels
 
   @profiler.record_runtime(
       name_prefix='VizierGPBandit', name='ard', also_log=True
   )
-  def _find_best_model_params(self) -> types.ParameterDict:
+  def _find_best_model_params(
+      self,
+      model: sp.StochasticProcessModel,
+      loss_fn: optimizers.LossFunction,
+      data: types.StochasticProcessModelData,
+      seed: jax.random.KeyArray,
+  ) -> tuple[types.ParameterDict, Any]:
     """Perform ARD on the current model to find best model parameters."""
-    self._model, loss_fn = (
-        tuned_gp_models.VizierGaussianProcess.model_and_loss_fn(
-            self._features, self._labels
-        )
-    )
     # Run ARD.
-    setup = lambda rng: self._model.init(rng, self._features)['params']
-    constraints = sp.get_constraints(self._model)
-    ard_loss_fn = self._get_loss_fn(loss_fn)
-
-    logging.info('Optimizing the loss function...')
-    self._rng, ard_rng = jax.random.split(self._rng, 2)
-    best_model_params, _ = self._ard_optimizer(
-        setup, ard_loss_fn, ard_rng, constraints=constraints
+    setup = functools.partial(
+        jax.jit(
+            gp_bandit_utils.stochastic_process_model_setup,
+            static_argnames=('model',),
+        ),
+        model=model,
+        data=data,
     )
-    return best_model_params
+    constraints = sp.get_constraints(model)
 
-  def _get_loss_fn(self, loss_fn):
-    if isinstance(self._ard_optimizer, optimizers.OptaxTrainWithRandomRestarts):
-
-      def ard_loss_fn(x):
-        loss_val, metrics = loss_fn(x)
-        # For SGD, normalize the loss so we can use the same learning rate
-        # regardless of the number of examples (see
-        # `OptaxTrainWithRandomRestarts` docstring).
-        return loss_val / self._features.shape[0], metrics
+    logging.info('Optimizing the loss function...')
 
-    else:
-      ard_loss_fn = loss_fn
-    return jax.jit(ard_loss_fn)
+    # The ARD optimizers JIT the train step/loop internally.
+    return self._ard_optimizer(setup, loss_fn, seed, constraints=constraints)
 
   @profiler.record_runtime(name_prefix='VizierGPBandit', name='compute_state')
-  def _compute_state(self):
+  def _compute_state(
+      self,
+  ) -> tuple[types.GPState, Optional[acquisitions.TrustRegion]]:
     """Compute the designer's state.
 
+    Returns:
+      GPBanditState object containing the designer's state.
+
     1. Convert trials to features and labels.
     2. Perform ARD to find best model parameters.
     3. Pre-compute the Cholesky decomposition.
 
     If no new trials were added since last call, no update will occur.
     """
     if len(self._trials) == self._incorporated_trials_count:
       # If there's no change in the number of completed trials, don't update
       # state. The assumption is that trials can't be removed.
-      return
+      return self._last_computed_state
+
     self._incorporated_trials_count = len(self._trials)
     # Convert trials to Numpy arrays. Labels are warped.
-    self._features, self._labels = self._convert_trials_to_arrays(self._trials)
+    features, labels = self._convert_trials_to_arrays(self._trials)
+
+    dimension_is_missing = None
+    label_is_missing = None
+    if self._padding_schedule:
+      dimension_is_missing = features.is_missing[1]
+      label_is_missing = labels.is_missing[0]
+      features = features.padded_array
+      labels = labels.padded_array
     # Update the model.
-    self._model, loss_fn = (
-        tuned_gp_models.VizierGaussianProcess.model_and_loss_fn(
-            self._features, self._labels
-        )
+    # TODO: Add support for PaddedArrays instead of passing in
+    # masks.
+    data = types.StochasticProcessModelData(
+        features=features,
+        labels=labels,
+        label_is_missing=label_is_missing,
+        dimension_is_missing=dimension_is_missing,
+    )
+    model = self._build_model(features)
+    # TODO: Avoid retracing vmapped loss when loss function API is
+    # redesigned.
+    loss_fn = functools.partial(
+        jax.jit(
+            gp_bandit_utils.stochastic_process_model_loss_fn,
+            static_argnames=('model', 'normalize'),
+        ),
+        model=model,
+        data=data,
+        # For SGD, normalize the loss so we can use the same learning rate
+        # regardless of the number of examples (see
+        # `OptaxTrainWithRandomRestarts` docstring).
+        normalize=isinstance(
+            self._ard_optimizer, optimizers.OptaxTrainWithRandomRestarts
+        ),
+    )
+    self._rng, ard_rng = jax.random.split(self._rng, 2)
+    best_model_params, metrics = self._find_best_model_params(
+        model, loss_fn, data, ard_rng
     )
-    best_model_params = self._find_best_model_params()
     # Logging for debugging purposes.
     logging.info('Best model parameters: %s', best_model_params)
-    ard_loss_fn = self._get_loss_fn(loss_fn)
-    if self._use_vmap:
-      ard_loss_fn = jax.vmap(ard_loss_fn)
-    ard_all_losses = ard_loss_fn(best_model_params)[0]
-    logging.info('All losses: %s', ard_all_losses)
-    ard_best_loss = ard_all_losses.flatten()[0].item()
-    logging.info('ARD best loss: %s', ard_best_loss)
 
-    @profiler.record_runtime(
-        name_prefix='VizierGPBandit', name='precompute_cholesky'
-    )
-    @jax.jit
-    def precompute_cholesky(params):
-      return self._model.apply(
-          {'params': params},
-          self._features,
-          self._labels,
-          method=self._model.precompute_predictive,
-          mutable='predictive',
-      )
+    # ARD optimizer metrics dicts are assumed to have a 'loss' field.
+    logging.info('All losses: %s', metrics['loss'])
+    logging.info('ARD best loss: %s', np.min(metrics['loss']))
+
     if self._use_vmap:
-      precompute_cholesky = jax.vmap(precompute_cholesky)
+      precompute_cholesky_fn = jit_vmap_precompute_cholesky
+    else:
+      precompute_cholesky_fn = jit_precompute_cholesky
     # `pp_state` contains intermediates that are expensive to compute, depend
     # only on observed (not predictive) index points, and are needed to compute
     # the posterior predictive GP (i.e. the Cholesky factor of the kernel matrix
     # over observed index points). `pp_state` is passed to
     # `model.posterior_predictive` to avoid re-computing the intermediates
     # unnecessarily.
-    _, pp_state = precompute_cholesky(best_model_params)
-    self._state = {'params': best_model_params, **pp_state}
+    _, pp_state = precompute_cholesky_fn(model, data, best_model_params)
+    model_state = {'params': best_model_params, **pp_state}
 
-    self._acquisition_builder.use_trust_region = self._use_trust_region
-
-    with profiler.record_runtime_context(
-        name='VizierGPBandit.acquisition_build', also_log=True
-    ):
-      self._acquisition_builder.build(
-          problem=self._problem,
-          model=self._model,
-          state=self._state,
-          features=self._features,
-          labels=self._labels,
-          converter=self._converter,
-          use_vmap=self._use_vmap,
+    trust_region = None
+    if self._use_trust_region:
+      trust_region = acquisitions.TrustRegion.build(
+          self._converter.output_specs,
+          data=data,
       )
+    state = types.GPState(data=data, model_state=model_state), trust_region
+    self._last_computed_state = state
+    return state
 
-  @profiler.record_runtime(
-      name_prefix='VizierGPBandit', name='optimize_acquisition'
-  )
-  def _optimize_acquisition(self, count: int) -> list[vz.Trial]:
-    """Optimize the acquisition function."""
-    return self._acquisition_optimizer.optimize(
-        score_fn=self._acquisition_builder.acquisition_on_array,
-        converter=self._converter,
+  def _optimize_acquisition(
+      self,
+      count: int,
+      state: types.GPState,
+      trust_region: Optional[acquisitions.TrustRegion] = None,
+  ) -> list[vz.Trial]:
+    start_time = datetime.datetime.now()
+    acq_rng, self._rng = jax.random.split(self._rng)
+
+    prior_features = vb.trials_to_sorted_array(self._trials, self._converter)
+    model = self._build_model(state.data.features)
+    suggestions = jit_optimize_acquisition(
         count=count,
-        prior_trials=self._trials,
+        model=model,
+        acquisition_fn=self._acquisition_function,
+        optimizer=self._acquisition_optimizer,
+        prior_features=prior_features,
+        state=state,
+        seed=acq_rng,
+        use_vmap=self._use_vmap,
+        trust_region=trust_region,
+        mapper=self._feature_mapper,
+    )
+
+    logging.info(
+        (
+            'Optimization completed. Duration: %s. Evaluations: %s. Best'
+            ' Results: %s'
+        ),
+        datetime.datetime.now() - start_time,
+        (
+            (
+                self._acquisition_optimizer.max_evaluations
+                // self._acquisition_optimizer.suggestion_batch_size
+            )
+            * self._acquisition_optimizer.suggestion_batch_size
+        ),
+        suggestions,
     )
+    return vb.best_candidates_to_trials(suggestions, self._converter)
 
   @profiler.record_runtime(name_prefix='VizierGPBandit')
   def suggest(self, count: int = 1) -> Sequence[vz.TrialSuggestion]:
     logging.info('Suggest called with count=%d', count)
     if count > 1:
       logging.warning(
           'GAUSSIAN_PROCESS_BANDIT currently is not optimized for batched'
@@ -358,50 +518,58 @@
           ' similar.'
       )
     suggest_start_time = datetime.datetime.now()
     if len(self._trials) < self._num_seed_trials:
       return self._generate_seed_trials(count)
 
     logging.info('Updating the designer state based on trials...')
-    self._compute_state()
+    state, _ = self._compute_state()
 
     logging.info('Optimizing acquisition...')
-    best_candidates = self._optimize_acquisition(count)
+    best_candidates = self._optimize_acquisition(count, state)
 
     # Convert best_candidates (in scaled space) into suggestions (in unscaled
     # space); also append debug information like model predictions.
     logging.info('Converting the optimization result into suggestions...')
     optimal_features = self._converter.to_features(best_candidates)  # [N, D]
+    if self._padding_schedule:
+      optimal_features = optimal_features.padded_array
+    if self._use_categorical_kernel:
+      optimal_features = self._feature_mapper.map(optimal_features)
     # Make predictions (in the warped space). [N]
+    model = self._build_model(state.data.features)
     with profiler.record_runtime_context(
         'VizierGPBandit.predict_on_suggestions'
     ):
-      predictions = self._acquisition_builder.predict_on_array(optimal_features)
+      predictions = jax.jit(
+          predictive_fns.predict_on_array, static_argnames=('model', 'use_vmap')
+      )(
+          optimal_features,
+          model=model,
+          state=state,
+          use_vmap=self._use_vmap,
+      )
     predict_mean = predictions['mean']  # [N,]
     predict_stddev = predictions['stddev']  # [N,]
-    logging.info(
-        'Created predictions for the best candidates which were '
-        f'converted to an array of shape: {optimal_features.shape}. '
-        f'mean has shape {predict_mean.shape}. '
-        f'stddev has shape {predict_stddev.shape}.'
-    )
+    # Possibly unpad predictions
+    predict_mean = predict_mean[: len(self._trials)]
+    predict_stddev = predict_stddev[: len(self._trials)]
     # Create suggestions, injecting the predictions as metadata for
     # debugging needs.
     suggestions = []
     for i, candidate in enumerate(best_candidates):
       metadata = candidate.metadata.ns(self._metadata_ns).ns('devinfo')
       acquisition = candidate.final_measurement.metrics.get_value(
           'acquisition', 'nan'
       )
       metadata['prediction_in_warped_y_space'] = json.dumps(
           {
               'mean': predict_mean[i],
               'stddev': predict_stddev[i],
               'acquisition': acquisition,
-              'state': self._state,
           },
           cls=json_utils.NumpyEncoder,
       )
       metadata['time_spent'] = f'{datetime.datetime.now() - suggest_start_time}'
       suggestions.append(
           vz.TrialSuggestion(candidate.parameters, metadata=candidate.metadata)
       )
@@ -429,20 +597,32 @@
       The predictions in the specified trials.
     """
     if rng is None:
       rng = jax.random.PRNGKey(0)
     if num_samples is None:
       num_samples = 1000
 
-    self._compute_state()
+    state, _ = self._compute_state()
+    model = self._build_model(state.data.features)
     xs = self._converter.to_features(trials)
-    samples = self._acquisition_builder.sample_on_array(
+    if self._padding_schedule:
+      xs = xs.padded_array[: len(trials), ...]
+    if self._use_categorical_kernel:
+      xs = self._feature_mapper.map(xs)
+
+    samples = jax.jit(
+        predictive_fns.sample_on_array,
+        static_argnames=('model', 'use_vmap', 'num_samples'),
+    )(
         xs,
         num_samples=num_samples,
         key=rng,
+        model=model,
+        state=state,
+        use_vmap=self._use_vmap,
     )  # (num_samples, batch_size)
     unwarped_samples = None
     # TODO: vectorize output warping.
     for i in range(samples.shape[0]):
       unwarp_samples_ = self._output_warper_pipeline.unwarp(
           samples[i][..., np.newaxis]
       ).reshape(-1)
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/gp_bandit_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/quasi_random_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,190 +10,186 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Tests for gp_bandit."""
+import random
 
-from typing import Any
-
-import mock
 import numpy as np
-import optax
-from vizier import algorithms as vza
+from scipy import stats
+from vizier import pythia
 from vizier import pyvizier as vz
-from vizier._src.algorithms.designers import gp_bandit
 from vizier._src.algorithms.designers import quasi_random
-from vizier._src.algorithms.optimizers import eagle_strategy as es
-from vizier._src.algorithms.optimizers import vectorized_base as vb
+from vizier._src.algorithms.policies import designer_policy
 from vizier._src.algorithms.testing import test_runners
-from vizier._src.jax.optimizers import optimizers
-from vizier.pyvizier import converters
 from vizier.testing import test_studies
-from vizier.utils import profiler
 
 from absl.testing import absltest
-from absl.testing import parameterized
 
 
-ensemble_ard_optimizer = optimizers.OptaxTrainWithRandomRestarts(
-    optax.adam(5e-3), epochs=10, verbose=False, random_restarts=10, best_n=5
-)
-
-noensemble_ard_optimizer = optimizers.OptaxTrainWithRandomRestarts(
-    optax.adam(5e-3), epochs=10, verbose=False, random_restarts=10, best_n=1
-)
-
-
-def _build_mock_continuous_array_specs(n):
-  continuous_spec = mock.create_autospec(converters.NumpyArraySpec)
-  continuous_spec.type = converters.NumpyArraySpecType.CONTINUOUS
-  continuous_spec.num_dimensions = 1
-  return [continuous_spec] * n
-
-
-class GoogleGpBanditTest(parameterized.TestCase):
-
-  @parameterized.parameters(
-      dict(iters=3, batch_size=5, num_seed_trials=5),
-      dict(iters=5, batch_size=1, num_seed_trials=2),
-      dict(ard_optimizer='ensemble'),
-      dict(ard_optimizer='noensemble'),
-  )
-  def test_on_flat_continuous_space(
-      self,
-      *,
-      iters: int = 5,
-      batch_size: int = 1,
-      num_seed_trials: int = 1,
-      ard_optimizer: Any = 'noensemble'
-  ):
-    # We use string names so that test case names are readable. Convert them
-    # to objects.
-    if ard_optimizer == 'noensemble':
-      ard_optimizer = noensemble_ard_optimizer
-    elif ard_optimizer == 'ensemble':
-      ard_optimizer = ensemble_ard_optimizer
-    problem = vz.ProblemStatement(
-        test_studies.flat_continuous_space_with_scaling()
-    )
-    problem.metric_information.append(
-        vz.MetricInformation(
-            name='metric', goal=vz.ObjectiveMetricGoal.MAXIMIZE
-        )
-    )
-    vectorized_optimizer = vb.VectorizedOptimizer(
-        strategy_factory=es.VectorizedEagleStrategyFactory(),
-        max_evaluations=10,
-    )
-    designer = gp_bandit.VizierGPBandit(
-        problem=problem,
-        acquisition_optimizer=vectorized_optimizer,
-        num_seed_trials=num_seed_trials,
-        ard_optimizer=ard_optimizer,
-    )
-    self.assertLen(
-        test_runners.RandomMetricsRunner(
-            problem,
-            iters=iters,
-            batch_size=batch_size,
-            verbose=1,
-            validate_parameters=True,
-        ).run_designer(designer),
-        iters * batch_size,
-    )
-    # Test that latency tracking works.
-    self.assertIn('VizierGPBandit.suggest', profiler.Storage().runtimes())
-    runtimes = profiler.Storage().runtimes().get('VizierGPBandit.suggest')
-    self.assertGreater(runtimes[0].total_seconds(), 0)
-
-    quasi_random_sampler = quasi_random.QuasiRandomDesigner(
-        problem.search_space
-    )
-    predict_trials = quasi_random_sampler.suggest(count=7)
-    prediction = designer.predict(predict_trials)
-    self.assertLen(prediction.mean, 7)
-    self.assertLen(prediction.stddev, 7)
-    self.assertFalse(np.isnan(prediction.mean).any())
-    self.assertFalse(np.isnan(prediction.stddev).any())
-
-  @parameterized.parameters(
-      dict(iters=3, batch_size=5, num_seed_trials=5),
-      dict(iters=5, batch_size=1, num_seed_trials=2),
-      dict(iters=5, batch_size=1, num_seed_trials=1),
-  )
-  def test_on_flat_mixed_space(
-      self, iters: int, batch_size: int, num_seed_trials: int
-  ):
-    problem = vz.ProblemStatement(
-        test_studies.flat_continuous_space_with_scaling()
-    )
-    problem.metric_information.append(
-        vz.MetricInformation(
-            name='metric', goal=vz.ObjectiveMetricGoal.MAXIMIZE
-        )
-    )
-    vectorized_optimizer = vb.VectorizedOptimizer(
-        strategy_factory=es.VectorizedEagleStrategyFactory(), max_evaluations=10
-    )
-    designer = gp_bandit.VizierGPBandit(
-        problem=problem,
-        acquisition_optimizer=vectorized_optimizer,
-        num_seed_trials=num_seed_trials,
-    )
+class HaltonTest(absltest.TestCase):
+
+  def test_generate_primes(self):
+    primes = quasi_random._generate_primes(100)
+    # For each prime, make sure it is not evenly divisible by any number less
+    # than itself.
+    for p in primes:
+      for n in range(2, int(p**0.5) + 1):
+        self.assertNotEqual(0, p % n)
+
+  def test_get_scrambled_halton_element(self):
+    num_dimensions = 4
+    generator = quasi_random._HaltonSequence(
+        num_dimensions=num_dimensions, skip_points=1000, scramble=True
+    )
+    sequence = [generator.get_next_list() for i in range(1000)]
+
+    self.assertLess(max(max(sequence)), 1)
+    self.assertGreater(min(min(sequence)), 0)
+    self.assertLen(sequence, 1000)
+    self.assertLen(sequence[0], 4)
+
+    # Test uniformity of Halton value outputs.
+    sequence = np.array(sequence)
+    for dim in range(num_dimensions):
+      _, p_value = stats.kstest(
+          sequence[:, dim], stats.uniform(loc=0.0, scale=1.0).cdf
+      )
+      # p_value greater than 0.9 roughly means we're very certain it's uniform.
+      self.assertGreater(p_value, 0.9)
+
+  def test_deterministic(self):
+    generator_1 = quasi_random._HaltonSequence(
+        num_dimensions=4, skip_points=100, primes_override=[3, 5, 7, 11]
+    )
+    generator_2 = quasi_random._HaltonSequence(
+        num_dimensions=4, skip_points=100, primes_override=[3, 5, 7, 11]
+    )
+    self.assertEqual(
+        [generator_1.get_next_list() for i in range(100)],
+        [generator_2.get_next_list() for i in range(100)],
+    )
+    self.assertEqual(
+        [generator_1.get_next_list() for i in range(100)],
+        [generator_2.get_next_list() for i in range(100)],
+    )
+
+  def test_unscrambled_sequence(self):
+    generator = quasi_random._HaltonSequence(
+        num_dimensions=1,
+        skip_points=0,
+        primes_override=[3],
+        scramble=False,
+        seed=0,
+    )
+    sequence = [generator.get_next_list()[0] for _ in range(7)]
+
+    expected_sequence = [
+        1 / 3,
+        2 / 3,
+        1 / 9,
+        4 / 9,
+        7 / 9,
+        2 / 9,
+        5 / 9,
+    ]
+
+    self.assertSequenceAlmostEqual(sequence, expected_sequence)
+
+
+class QuasiRandomTest(absltest.TestCase):
+
+  def test_on_flat_space(self):
+    problem = vz.ProblemStatement(test_studies.flat_space_with_all_types())
+    designer = quasi_random.QuasiRandomDesigner(problem.search_space)
     self.assertLen(
-        test_runners.RandomMetricsRunner(
-            problem,
-            iters=iters,
-            batch_size=batch_size,
-            verbose=1,
-            validate_parameters=True,
-        ).run_designer(designer), iters * batch_size)
-
-    quasi_random_sampler = quasi_random.QuasiRandomDesigner(
-        problem.search_space
-    )
-    predict_trials = quasi_random_sampler.suggest(count=7)
-    prediction = designer.predict(predict_trials)
-    self.assertLen(prediction.mean, 7)
-    self.assertLen(prediction.stddev, 7)
-    self.assertFalse(np.isnan(prediction.mean).any())
-    self.assertFalse(np.isnan(prediction.stddev).any())
-
-  def test_prediction_accuracy(self):
-    search_space = vz.SearchSpace()
-    search_space.root.add_float_param('x0', -5.0, 5.0)
-    problem = vz.ProblemStatement(
-        search_space=search_space,
-        metric_information=vz.MetricsConfig(
-            metrics=[
-                vz.MetricInformation(
-                    'obj', goal=vz.ObjectiveMetricGoal.MAXIMIZE
-                ),
-            ]
+        test_runners.run_with_random_metrics(
+            designer, problem, iters=50, batch_size=5, validate_parameters=True
         ),
+        250,
     )
-    f = lambda x: -((x - 0.5) ** 2)
 
-    suggestions = quasi_random.QuasiRandomDesigner(
-        problem.search_space, seed=1
-    ).suggest(100)
-
-    obs_trials = []
-    for idx, suggestion in enumerate(suggestions):
-      trial = suggestion.to_trial(idx)
-      x = suggestions[idx].parameters['x0'].value
-      trial.complete(vz.Measurement(metrics={'obj': f(x)}))
-      obs_trials.append(trial)
-
-    ard_optimizer = optimizers.JaxoptLbfgsB(random_restarts=8, best_n=5)
-    gp_designer = gp_bandit.VizierGPBandit(problem, ard_optimizer=ard_optimizer)
-    gp_designer.update(vza.CompletedTrials(obs_trials), vza.ActiveTrials())
-    pred_trial = vz.Trial({'x0': 0.0})
-    pred = gp_designer.predict([pred_trial])
-    self.assertLess(np.abs(pred.mean[0] - f(0.0)), 2e-2)
+  def test_dump_and_load(self):
+    # Check metadata checkpointing.
+    problem = vz.ProblemStatement(test_studies.flat_space_with_all_types())
+
+    designer = quasi_random.QuasiRandomDesigner(problem.search_space)
+    designer.suggest(random.randint(1, 50))
+    metadata = designer.dump()
+
+    designer2 = quasi_random.QuasiRandomDesigner(problem.search_space)
+    designer2.load(metadata)
+
+    num_suggestions = 10
+    self.assertEqual(
+        designer.suggest(num_suggestions), designer2.suggest(num_suggestions)
+    )
+
+  def test_distribution(self):
+    # Make sure output distribution makes sense.
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    designer = quasi_random.QuasiRandomDesigner(problem.search_space)
+
+    suggestions = designer.suggest(2000)
+    float_points = [
+        suggestion.parameters['float'].value for suggestion in suggestions
+    ]
+
+    # Test uniformity of end-to-end parameter values.
+    # p_value greater than 0.9 roughly means we're very certain it's uniform.
+    # Unfortunately KS-test doesn't work for discrete/categorical distributions.
+    _, float_p_value = stats.kstest(
+        float_points, stats.uniform(loc=0.0, scale=1.0).cdf
+    )
+    self.assertGreater(float_p_value, 0.9)
+
+  def test_equal_seeds(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    designer_1 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=1)
+    suggestions_1 = designer_1.suggest(10)
+    designer_2 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=1)
+    suggestions_2 = designer_2.suggest(10)
+    self.assertEqual(suggestions_1, suggestions_2)
+
+  def test_distinct_seeds(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    designer_1 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=0)
+    suggestions_1 = designer_1.suggest(10)
+    designer_2 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=1)
+    suggestions_2 = designer_2.suggest(10)
+    self.assertNotEqual(suggestions_1, suggestions_2)
+
+  def test_policy_wrapping(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    policy_supporter = pythia.InRamPolicySupporter(problem)
+    policy = designer_policy.PartiallySerializableDesignerPolicy(
+        problem,
+        policy_supporter,
+        quasi_random.QuasiRandomDesigner.from_problem,
+    )
+
+    # Make sure outputs are distinct.
+    all_suggestions = []
+    for _ in range(1000):
+      request = pythia.SuggestRequest(
+          study_descriptor=policy_supporter.study_descriptor(), count=1
+      )
+      decisions = policy.suggest(request)
+      all_suggestions.extend(decisions.suggestions)
+
+    distinct_suggestions = set(
+        [
+            tuple(suggestion.parameters.as_dict().values())
+            for suggestion in all_suggestions
+        ]
+    )
+    self.assertLen(distinct_suggestions, 1000)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/grid.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/grid.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/grid_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/grid_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/harmonica.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/harmonica_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/quasi_random.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/random.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/random.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,21 @@
           pc, scale=True, max_discrete_indices=0, float_dtype=dtype)
 
     self._converter = converters.DefaultTrialConverter(
         [create_input_converter(pc) for pc in search_space.parameters])
 
     self._rng = np.random.RandomState(seed)
 
+  @classmethod
+  def from_problem(
+      cls, problem: vz.ProblemStatement, seed: Optional[int] = None
+  ):
+    """For wrapping via `PartiallySerializableDesignerPolicy`."""
+    return RandomDesigner(problem.search_space, seed=seed)
+
   def update(
       self, completed: vza.CompletedTrials, all_active: vza.ActiveTrials
   ) -> None:
     pass
 
   def suggest(self,
               count: Optional[int] = None) -> Sequence[vz.TrialSuggestion]:
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/random_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/random_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/scalarizing_designer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/designers/scalarizing_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/evolution/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2.py` & `google-vizier-0.1.6/vizier/_src/algorithms/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations.py` & `google-vizier-0.1.6/vizier/_src/algorithms/evolution/numpy_populations.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/evolution/numpy_populations_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/evolution/templates.py` & `google-vizier-0.1.6/vizier/_src/algorithms/evolution/templates.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/base.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/designer_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/designer_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import jax
 from jax import numpy as jnp
 import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import eagle_strategy
 from vizier._src.algorithms.optimizers import random_vectorized_optimizer as rvo
-from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier._src.algorithms.testing import comparator_runner
 from vizier._src.jax import types
 from vizier.pyvizier import converters
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
@@ -108,32 +107,31 @@
   def test_converges(self, create_problem_fn, n_features, score_fn):
     logging.info('Starting a new convergence test (n_features: %s)', n_features)
     evaluations = 20_000
     problem = create_problem_fn(n_features)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     eagle_strategy_factory = eagle_strategy.VectorizedEagleStrategyFactory(
         eagle_config=eagle_strategy.EagleStrategyConfig())
-    eagle_optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=eagle_strategy_factory)
     optimum_features = randomize_array(converter)
     shifted_score_fn = lambda x, shift=optimum_features: score_fn(x - shift)
     shifted_score_fn = score_fn
-    random_optimizer_factory = rvo.create_random_optimizer_factory()
+    random_strategy_factory = rvo.random_strategy_factory
     # Run simple regret convergence test.
     comparator_runner.SimpleRegretComparisonTester(
         baseline_num_trials=2 * evaluations,
         candidate_num_trials=evaluations,
         baseline_suggestion_batch_size=5,
         candidate_suggestion_batch_size=5,
         baseline_num_repeats=5,
         candidate_num_repeats=3,
         alpha=0.05,
-        goal=vz.ObjectiveMetricGoal.MAXIMIZE
+        goal=vz.ObjectiveMetricGoal.MAXIMIZE,
     ).assert_optimizer_better_simple_regret(
         converter=converter,
         score_fn=shifted_score_fn,
-        baseline_optimizer_factory=random_optimizer_factory,
-        candidate_optimizer_factory=eagle_optimizer_factory)
+        baseline_strategy_factory=random_strategy_factory,
+        candidate_strategy_factory=eagle_strategy_factory,
+    )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_param_handler.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_param_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,122 +14,149 @@
 
 from __future__ import annotations
 
 """Utils for vectorized eagle strategy."""
 
 from typing import Optional
 
-import attr
+from flax import struct
 import jax
 from jax import numpy as jnp
 from vizier.pyvizier import converters
 
 
-@attr.define(kw_only=True)
+@struct.dataclass
 class EagleParamHandler:
   """Vectorized eagle strategy utils.
 
   The class is used to account for the different types of Vizier parameters and
   incorporate their naunces into the vectorized eagle strategy.
 
   Attributes:
-    converter: The converter used to convert the original search space. It's
-      used to get metadata on the different parameters and attribute the feature
-      indices to them.
-    config: The eagle strategy configuration used to set the perturbation
-      factors for CATEGORICAL features.
-    categorical_perturbation_factor: The perturbation factor for categorical
-      features.
-    pure_categorical_perturbation_factor: The perturbation factor when all
-      features are categorical.
-    n_features: The total number of feature indices.
+    n_feature_dimensions: The total number of feature indices.
     n_categorical: The number of CATEGORICAL associated indices.
     has_categorical: A flag indicating if at least one feature is categorical.
-    all_features_categorical: A flag indicating if all features are categorical.
-    _categorical_param_mask: A 2D array (n_categorical, n_features) that for
-      each categorical parameters (row) has 1s in its associated feature
-      indices. The array is used for sampling categorical values.
-    _categorical_mask: A 1D array (n_features,) with 1s in the indices of
-      categorical features and otherwise 0s. The array is used for sampling
+    perturbation_factors: Array of continuous and categorical perturbation
+      factors.
+    _categorical_param_mask: A 2D array (n_categorical, n_feature_dimensions)
+      that for each categorical parameters (row) has 1s in its associated
+      feature indices. The array is used for sampling categorical values.
+    _categorical_mask: A 1D array (n_feature_dimensions,) with 1s in the indices
+      of categorical features and otherwise 0s. The array is used for sampling
       categorical values.
-    _tiebreak_mask: A 1D array (n_features,) with multiplies of epsilons used to
-      tie breaking. The array is used for sampling categorical values.
-    _oov_mask: A 1D array (n_features,) with 1s in the non-oov indices. The
-      array is used to generate random features with 0 value in the OOV indices.
+    _tiebreak_mask: A 1D array (n_feature_dimensions,) with multiplies of
+      epsilons used to tie breaking. The array is used for sampling categorical
+      values.
+    _oov_mask: A 1D array (n_feature_dimensions,) with 1s in the non-oov
+      indices. The array is used to generate random features with 0 value in the
+      OOV indices.
     _epsilon: A small value used in tie-breaker
   """
-  converter: converters.TrialToArrayConverter
-  categorical_perturbation_factor: float
-  pure_categorical_perturbation_factor: float
-  # Public variables created by the class
-  n_features: int = attr.field(init=False)
-  n_categorical: int = attr.field(init=False)
-  has_categorical: bool = attr.field(init=False)
-  all_features_categorical: bool = attr.field(init=False)
   # Internal variables
-  _categorical_params_mask: jax.Array = attr.field(init=False)
-  _categorical_mask: jax.Array = attr.field(init=False)
-  _tiebreak_array: jax.Array = attr.field(init=False)
-  _oov_mask: Optional[jax.Array] = attr.field(init=False, default=None)
-  _epsilon: float = attr.field(init=False, default=1e-5)
-
-  def __attrs_post_init__(self):
-    self._init_utils()
+  perturbation_factors: jax.Array
+  _categorical_params_mask: jax.Array
+  _categorical_mask: jax.Array
+  _tiebreak_array: jax.Array
+  _oov_mask: Optional[jax.Array]
+  _epsilon: float
+  # Public variables created by the class
+  n_feature_dimensions: int = struct.field(pytree_node=False)
+  n_categorical: int = struct.field(pytree_node=False)
+  has_categorical: bool = struct.field(pytree_node=False)
+
+  @classmethod
+  def build(
+      cls,
+      converter: converters.TrialToArrayConverter,
+      categorical_perturbation_factor: float,
+      pure_categorical_perturbation_factor: float,
+      epsilon: float = 1e-5,
+  ) -> 'EagleParamHandler':
+    """Docstring."""
 
-  def _init_utils(self):
-    """Initialize the utility class and cache arrays for repeated use."""
     valid_types = [
         converters.NumpyArraySpecType.ONEHOT_EMBEDDING,
         converters.NumpyArraySpecType.CONTINUOUS
     ]
-    unsupported_params = sum([
-        1 for spec in self.converter.output_specs
-        if spec.type not in valid_types
-    ])
+    unsupported_params = sum(
+        1 for spec in converter.output_specs if spec.type not in valid_types
+    )
     if unsupported_params:
       raise ValueError('Only CATEGORICAL/CONTINUOUS parameters are supported!')
 
-    self.n_features = sum(
-        [spec.num_dimensions for spec in self.converter.output_specs])
-    self.n_categorical = sum([
-        1 for spec in self.converter.output_specs
+    n_feature_dimensions = converter.to_features([]).shape[-1]
+    n_categorical = sum(
+        1
+        for spec in converter.output_specs
         if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING
-    ])
-    self.has_categorical = self.n_categorical > 0
-    self.all_features_categorical = self.n_features == self.n_categorical
-    if self.has_categorical:
-      self._create_categorical_masks()
-
-  def _create_categorical_masks(self):
-    """Create the categorical masks."""
-    categorical_params_mask = jnp.zeros((self.n_categorical, self.n_features))
-    oov_mask = jnp.ones((self.n_features,))
-    row = 0
-    col = 0
-    # Create a flag to indicate if the converter uses OOV padding. If none of
-    # the CATEGORICAL params use padding the 'oov_mask' is set to None.
-    is_pad_oov = False
-    for spec in self.converter.output_specs:
-      if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
-        n_dim = spec.num_dimensions
-        categorical_params_mask = categorical_params_mask.at[
-            row, col : col + n_dim
-        ].set(1.0)
-        if spec.num_oovs:
-          oov_mask = oov_mask.at[col + n_dim - 1].set(0.0)
-          is_pad_oov = True
-        row += 1
-        col += n_dim
-      else:
-        col += 1
-
-    self._oov_mask = oov_mask if is_pad_oov else None
-    self._tiebreak_array = -self._epsilon * jnp.arange(1, self.n_features + 1)
-    self._categorical_mask = jnp.sum(categorical_params_mask, axis=0)
-    self._categorical_params_mask = categorical_params_mask
+    )
+    has_categorical = n_categorical > 0
+    all_features_categorical = n_feature_dimensions == n_categorical
+    oov_mask = None
+    tiebreak_array = None
+    categorical_mask = None
+    categorical_params_mask = None
+    if has_categorical:
+      categorical_params_mask = jnp.zeros((n_categorical, n_feature_dimensions))
+      oov_mask = jnp.ones((n_feature_dimensions,))
+      row = 0
+      col = 0
+      # Create a flag to indicate if the converter uses OOV padding. If none of
+      # the CATEGORICAL params use padding the 'oov_mask' is set to None.
+      is_pad_oov = False
+      for spec in converter.output_specs:
+        if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
+          n_dim = spec.num_dimensions
+          categorical_params_mask = categorical_params_mask.at[
+              row, col : col + n_dim
+          ].set(1.0)
+          if spec.num_oovs:
+            oov_mask = oov_mask.at[col + n_dim - 1].set(0.0)
+            is_pad_oov = True
+          row += 1
+          col += n_dim
+        else:
+          col += 1
+
+      oov_mask = oov_mask if is_pad_oov else None
+      tiebreak_array = -epsilon * jnp.arange(1, n_feature_dimensions + 1)
+      categorical_mask = jnp.sum(categorical_params_mask, axis=0)
+
+    perturbation_factors = []
+
+    if all_features_categorical:
+      for spec in converter.output_specs:
+        perturbation_factors.extend(
+            [pure_categorical_perturbation_factor] * spec.num_dimensions
+        )
+    else:
+      for spec in converter.output_specs:
+        if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
+          perturbation_factors.extend(
+              [categorical_perturbation_factor] * spec.num_dimensions
+          )
+
+        elif spec.type == converters.NumpyArraySpecType.CONTINUOUS:
+          perturbation_factors.append(1.0)
+    # Add any extra dimensions at the end.
+    perturbation_factors.extend(
+        [0.0] * (n_feature_dimensions - len(perturbation_factors))
+    )
+    perturbation_factors = jnp.array(perturbation_factors)
+    return EagleParamHandler(
+        n_feature_dimensions=n_feature_dimensions,
+        n_categorical=n_categorical,
+        has_categorical=has_categorical,
+        perturbation_factors=perturbation_factors,
+        _categorical_params_mask=categorical_params_mask,
+        _categorical_mask=categorical_mask,
+        _tiebreak_array=tiebreak_array,
+        _oov_mask=oov_mask,
+        _epsilon=epsilon,
+    )
 
   def sample_categorical(
       self, features: jax.Array, seed: jax.random.KeyArray
   ) -> jax.Array:
     """Sample categorical features.
 
     The categorical sampling is used before returning suggestion to ensure that
@@ -149,19 +176,20 @@
     5. Randomize uniform values for each row to determine which value to sample.
     6. Find the minimum index that its CDF > uniform. See code around
     'sampled_categorical_params' below for more detail and for why we need to
     add the tie-breaking array values.
     7. Flatten each row sampled values and combine with original features.
 
     Arguments:
-      features: (batch_size, n_features)
+      features: (batch_size, n_feature_dimensions)
       seed: Random seed.
 
     Returns:
-      The features with sampled categorical parameters. (batch_size ,n_features)
+      The features with sampled categorical parameters.
+        (batch_size, n_feature_dimensions)
     """
     if not self.has_categorical:
       return features
     batch_size = features.shape[0]
     # Mask each row (which represents a categorical param) to remove values in
     # indices that aren't associated with the parameter indices.
     param_features = features[:, jnp.newaxis, :] * self._categorical_params_mask
@@ -175,61 +203,42 @@
     # Multiply by 'categorical_mask' to mask off cumsum in non-categorical
     # indices, and add 'tiebreak_mask' to find the first index.
     masked_locs = locs * self._categorical_params_mask + self._tiebreak_array
     # Generate the samples so that each parameter features has a single 1 value.
     sampled_categorical_params = jnp.trunc(
         masked_locs / jnp.max(masked_locs, axis=-1, keepdims=True)
     )
-    # Flatten all the categories features to dimension (batch_size, n_features)
+    # Flatten all the categories features to dimension
+    # (batch_size, n_feature_dimensions)
     sampled_features = jnp.sum(sampled_categorical_params, axis=1)
     # Mask categorical features and add the new sampled categorical values.
     return sampled_features + features * (1 - self._categorical_mask)
 
   def random_features(
       self, batch_size: int, seed: jax.random.KeyArray
   ) -> jax.Array:
     """Create random features with uniform distribution.
 
     In case there are CATEGORICAL features with OOV we use the 'oov_mask' which
-    is 1D numpy array (n_features,) with 0s in OOV indices and otherwise 1s.
-    After multiplying (and broadcasting) the randomly generated features with
-    the mask we're guaranteed that no features will be created in OOV indices.
-    Therefore when mutating fireflies' features (index by index), the final
-    suggested features will also have 0s in the OOV indices as desired.
+    is 1D numpy array (n_feature_dimensions,) with 0s in OOV indices and
+    otherwise 1s.  After multiplying (and broadcasting) the randomly generated
+    features with the mask we're guaranteed that no features will be created in
+    OOV indices.  Therefore when mutating fireflies' features (index by index),
+    the final suggested features will also have 0s in the OOV indices as
+    desired.
 
     Arguments:
       batch_size:
       seed: Random seed.
 
     Returns:
       The random features with out of vocabulary indices zeroed out.
     """
-    size = (batch_size, self.n_features)
+    features = jax.random.uniform(
+        seed, shape=(batch_size, self.n_feature_dimensions)
+    )
     if self._oov_mask is not None:
       # Don't create random values for CATEGORICAL features OOV indices.
-      # Broadcasting: (batch_size, n_features) x (n_features,)
-      return jax.random.uniform(seed, shape=size) * self._oov_mask
-    else:
-      return jax.random.uniform(seed, shape=size)
-
-  @property
-  def perturbation_factors(self) -> jax.Array:
-    """Create the perturbations factors.
-
-    Returns:
-      Array of perturbation factors (n_features,)
-    """
-    perturbation_factors = []
-
-    if self.all_features_categorical:
-      for spec in self.converter.output_specs:
-        perturbation_factors.extend(
-            [self.pure_categorical_perturbation_factor] * spec.num_dimensions)
-    else:
-      for spec in self.converter.output_specs:
-        if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
-          perturbation_factors.extend([self.categorical_perturbation_factor] *
-                                      spec.num_dimensions)
-
-        elif spec.type == converters.NumpyArraySpecType.CONTINUOUS:
-          perturbation_factors.append(1.0)
-    return jnp.array(perturbation_factors)
+      # Broadcasting:
+      #   (batch_size, n_feature_dimensions) x (n_feature_dimensions,)
+      features = features * self._oov_mask
+    return features
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 which are closer to the optimum.
 
 Note that the strategy assumes that the search space is not conditional.
 
 Example
 =======
 # Construct the optimizer with eagle strategy.
-optimizer = VectorizedOptimizer(
+optimizer = VectorizedOptimizerFactory(
     VectorizedEagleStrategyFactory(),
 )
 # Run the optimization.
 trials = optimizer.optimize(problem_statement, objective_function)
 """
 # pylint: disable=g-long-lambda
 
 import enum
 import logging
 import math
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import attr
-import chex
+from flax import struct
 import jax
 from jax import numpy as jnp
 from vizier._src.algorithms.optimizers import eagle_param_handler
 from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier._src.jax import types
 from vizier.pyvizier import converters
 
@@ -90,15 +90,15 @@
   """The force normalization mode. Use IntEnum for JIT compatibility."""
 
   MEAN = 0
   RANDOM = 1
   UNNORMALIZED = 2
 
 
-@chex.dataclass(frozen=True)
+@struct.dataclass
 class EagleStrategyConfig:
   """Eagle Strategy optimizer config.
 
   Attributes:
     visibility: The sensetivity to distance between flies when computing pulls.
     gravity: The maximum amount of attraction pull.
     negative_gravity: The maximum amount of repulsion pull.
@@ -127,36 +127,40 @@
   perturbation: float = 0.16
   categorical_perturbation_factor: float = 25
   pure_categorical_perturbation_factor: float = 30
   # Penalty
   perturbation_lower_bound: float = 7e-5
   penalize_factor: float = 7e-1
   # Pool size
-  pool_size_exponent: float = 1.2
-  pool_size: int = 0
-  max_pool_size: int = 100
+  pool_size_exponent: float = struct.field(pytree_node=False, default=1.2)
+  pool_size: int = struct.field(pytree_node=False, default=0)
+  max_pool_size: int = struct.field(pytree_node=False, default=100)
   # Force normalization mode
-  mutate_normalization_type: MutateNormalizationType = (
-      MutateNormalizationType.MEAN
+  mutate_normalization_type: MutateNormalizationType = struct.field(
+      pytree_node=False,
+      default=MutateNormalizationType.MEAN,
   )
   # Multiplier factor when using normalized modes
   normalization_scale: float = 0.5
   # The percentage of the firefly pool to be populated with prior trials
-  prior_trials_pool_pct: float = 0.96
+  prior_trials_pool_pct: float = struct.field(pytree_node=False, default=0.96)
 
 
 @attr.define(frozen=True)
 class VectorizedEagleStrategyFactory(vb.VectorizedStrategyFactory):
   """Eagle strategy factory."""
 
   eagle_config: EagleStrategyConfig = attr.field(factory=EagleStrategyConfig)
 
   def __call__(
       self,
-      converter: converters.TrialToArrayConverter,
+      converter: Union[
+          converters.TrialToArrayConverter,
+          converters.PaddedTrialToArrayConverter,
+      ],
       suggestion_batch_size: Optional[int] = None,
   ) -> "VectorizedEagleStrategy":
     """Create a new vectorized eagle strategy.
 
     In order to create the strategy a converter has to be passed, which the
     strategy will then store a pointer to. The strategy uses the converter to
     get information about the original Vizier Parameters and their relation to
@@ -167,122 +171,116 @@
       converter: TrialToArrayConverter that matches the converter used in
         computing the objective / acuisition function.
       suggestion_batch_size: The batch_size of the returned suggestion array.
 
     Returns:
       A new instance of VectorizedEagleStrategy.
     """
+    param_handler = eagle_param_handler.EagleParamHandler.build(
+        converter,
+        self.eagle_config.categorical_perturbation_factor,
+        self.eagle_config.pure_categorical_perturbation_factor,
+    )
+    n_feature_dimensions_with_padding = converter.to_features([]).shape[-1]
+    n_features = len(converter.output_specs)
+
+    if self.eagle_config.pool_size > 0:
+      # This allow to override the pool size computation.
+      pool_size = self.eagle_config.pool_size
+    else:
+      pool_size = 10 + int(
+          0.5 * n_features + n_features**self.eagle_config.pool_size_exponent
+      )
+      pool_size = min(pool_size, self.eagle_config.max_pool_size)
+      if suggestion_batch_size is not None:
+        # If the batch_size was set, ensure pool_size is multiply of batch_size.
+        pool_size = int(
+            math.ceil(pool_size / suggestion_batch_size) * suggestion_batch_size
+        )
+    logging.info("Pool size: %d", pool_size)
+    if suggestion_batch_size is None:
+      # This configuration updates all the fireflies in each iteration.
+      suggestion_batch_size = pool_size
+    # Use priors to populate Eagle state
     return VectorizedEagleStrategy(
-        converter=converter,
-        config=self.eagle_config,
+        param_handler=param_handler,
+        n_features=n_features,
+        n_feature_dimensions=sum(
+            spec.num_dimensions for spec in converter.output_specs
+        ),
+        n_feature_dimensions_with_padding=n_feature_dimensions_with_padding,
         batch_size=suggestion_batch_size,
+        config=self.eagle_config,
+        pool_size=pool_size,
     )
 
 
-@chex.dataclass(frozen=True)
+@struct.dataclass
 class VectorizedEagleStrategyState:
   """Container for Eagle strategy state."""
 
   iterations: jax.Array  # Scalar integer.
   features: jax.Array  # Shape (pool_size, n_features).
   rewards: jax.Array  # Shape (pool_size,).
   best_reward: jax.Array  # Scalar float.
   perturbations: jax.Array  # Shape (pool_size,).
 
 
-@attr.define
+@struct.dataclass
 class VectorizedEagleStrategy(vb.VectorizedStrategy):
   """Eagle strategy implementation for maximization problem based on Numpy.
 
   Attributes:
     converter: The converter used for the optimization problem.
     config: The Eagle strategy configuration.
     n_features: The number of features.
     batch_size: The number of suggestions generated at each suggestion call.
     pool_size: The total number of flies in the pool.
   """
 
-  converter: converters.TrialToArrayConverter = attr.field(
-      init=True, repr=False
+  param_handler: eagle_param_handler.EagleParamHandler
+  n_features: int = struct.field(pytree_node=False)
+  n_feature_dimensions: int = struct.field(pytree_node=False)
+  n_feature_dimensions_with_padding: int = struct.field(pytree_node=False)
+  pool_size: int = struct.field(pytree_node=False)
+  batch_size: Optional[int] = struct.field(pytree_node=False, default=None)
+  config: EagleStrategyConfig = struct.field(
+      default_factory=EagleStrategyConfig
   )
-  config: EagleStrategyConfig = attr.field(init=True, repr=False)
-  batch_size: Optional[int] = attr.field(init=True, default=None)
-  pool_size: int = attr.field(init=False)
-  # Attributes related to computations.
-  _n_features: int = attr.field(init=False)
-  _perturbation_factors: jax.Array = attr.field(init=False, repr=False)
 
-  def __attrs_post_init__(self):
-    self._initialize()
+  def __post_init__(self):
     logging.info("Eagle class attributes:\n%s", self)
     logging.info("Eagle configuration:\n%s", self.config)
 
-  def __hash__(self):
-    # Make this class hashable so it can be a static arg to a JIT-ed function.
-    return hash(id(self))
-
-  def _compute_pool_size(self) -> int:
-    """Compute the pool size, and ensures it's a multiple of the batch_size."""
-    n_params = len(self.converter.output_specs)
-    pool_size = 10 + int(
-        0.5 * n_params + n_params**self.config.pool_size_exponent
-    )
-    pool_size = min(pool_size, self.config.max_pool_size)
-    if self.batch_size is not None:
-      # If the batch_size was set, ensure pool_size is multiply of batch_size.
-      return int(math.ceil(pool_size / self.batch_size) * self.batch_size)
-    else:
-      return pool_size
-
-  def _initialize(self) -> None:
-    """Initialize the designer state."""
-    self._param_handler = eagle_param_handler.EagleParamHandler(
-        converter=self.converter,
-        categorical_perturbation_factor=self.config.categorical_perturbation_factor,
-        pure_categorical_perturbation_factor=self.config.pure_categorical_perturbation_factor,
-    )
-    self._n_features = self._param_handler.n_features
-    if self.config.pool_size > 0:
-      # This allow to override the pool size computation.
-      self.pool_size = self.config.pool_size
-    else:
-      self.pool_size = self._compute_pool_size()
-    logging.info("Pool size: %d", self.pool_size)
-    if self.batch_size is None:
-      # This configuration updates all the fireflies in each iteration.
-      self.batch_size = self.pool_size
-    self._perturbation_factors = self._param_handler.perturbation_factors
-    # Use priors to populate Eagle state
-
   def init_state(
       self,
-      seed: chex.PRNGKey,
-      prior_features: Optional[chex.Array] = None,
-      prior_rewards: Optional[chex.Array] = None,
+      seed: jax.random.KeyArray,
+      prior_features: Optional[types.Array] = None,
+      prior_rewards: Optional[types.Array] = None,
   ) -> VectorizedEagleStrategyState:
     """Initializes the state."""
     if prior_features is not None or prior_rewards is not None:
       init_features = self._populate_pool_with_prior_trials(
           seed, prior_features, prior_rewards
       )
     else:
-      init_features = self._param_handler.random_features(self.pool_size, seed)
+      init_features = self.param_handler.random_features(self.pool_size, seed)
     return VectorizedEagleStrategyState(
         iterations=jnp.array(0),
         features=init_features,
         rewards=jnp.ones(self.pool_size) * -jnp.inf,
         best_reward=-jnp.inf,
         perturbations=jnp.ones(self.pool_size) * self.config.perturbation,
     )
 
   def _populate_pool_with_prior_trials(
       self,
-      seed: chex.PRNGKey,
-      prior_features: chex.Array,
-      prior_rewards: chex.Array,
+      seed: jax.random.KeyArray,
+      prior_features: types.Array,
+      prior_rewards: types.Array,
   ) -> jax.Array:
     """Populate the pool with prior trials.
 
     Args:
       seed: Random seed.
       prior_features: (n_prior_features, features_count)
       prior_rewards: (n_prior_features, )
@@ -298,39 +296,40 @@
     if prior_features is None or prior_rewards is None:
       raise ValueError("One of prior features / prior rewards wasn't provided!")
     if prior_features.shape[0] != prior_rewards.shape[0]:
       raise ValueError(
           f"prior features shape ({prior_features.shape[0]}) doesn't match"
           f" prior  rewards shape ({prior_rewards.shape[0]})!"
       )
-    if prior_features.shape[1] != self._n_features:
+    if prior_features.shape[1] != self.n_feature_dimensions_with_padding:
       raise ValueError(
-          f"prior features shape ({prior_features.shape[1]}) doesn't match "
-          f"n_features ({self._n_features})!"
+          f"prior features shape ({prior_features.shape[1]}) doesn't match"
+          f" n_features {self.n_feature_dimensions_with_padding}!"
       )
+
     if len(prior_rewards.shape) > 1:
       raise ValueError("prior rewards is expected to be 1D array!")
 
     # Reverse the order of prior trials to assign more weight to recent trials.
     flipped_prior_features = jnp.flip(prior_features, axis=0)
     flipped_prior_rewards = jnp.flip(prior_rewards, axis=0)
 
     # Fill pool with random features.
     n_random_flies = int(
         self.pool_size * (1 - self.config.prior_trials_pool_pct)
     )
     seed1, seed2 = jax.random.split(seed)
-    init_features = self._param_handler.random_features(n_random_flies, seed1)
+    init_features = self.param_handler.random_features(n_random_flies, seed1)
     pool_left_space = self.pool_size - n_random_flies
 
     if prior_features.shape[0] < pool_left_space:
       # Less prior trials than left space. Take all prior trials for the pool.
       init_features = jnp.concatenate([init_features, flipped_prior_features])
       # Randomize the rest of the pool fireflies.
-      random_features = self._param_handler.random_features(
+      random_features = self.param_handler.random_features(
           self.pool_size - len(init_features), seed2
       )
       return jnp.concatenate([init_features, random_features])
     else:
       # More prior trials than left space. Iteratively populate the pool.
       tmp_features = flipped_prior_features[:pool_left_space]
       tmp_rewards = flipped_prior_rewards[:pool_left_space]
@@ -361,15 +360,15 @@
 
   @property
   def suggestion_batch_size(self) -> int:
     """The number of suggestions returned at each call of 'suggest'."""
     return self.batch_size
 
   def suggest(
-      self, state: VectorizedEagleStrategyState, seed: chex.PRNGKey
+      self, state: VectorizedEagleStrategyState, seed: jax.random.KeyArray
   ) -> jax.Array:
     """Suggest new mutated and perturbed features.
 
     After initializing, at each call `batch_size` fireflies are mutated to
     generate new features using pulls (attraction/repulsion) from all other
     fireflies in the pool.
 
@@ -410,31 +409,29 @@
     new_features = jax.lax.cond(
         state.iterations < self.pool_size // self.batch_size,
         lambda x: x,
         _mutate_features,
         features_batch,
     )
 
-    new_features = self._param_handler.sample_categorical(
-        new_features, cat_seed
-    )
+    new_features = self.param_handler.sample_categorical(new_features, cat_seed)
     # TODO: The range of features is not always [0, 1].
     #   Specifically, for features that are single-point, it can be [0, 0]; we
     #   also want this code to be aware of the feature's bounds to enable
     #   contextual bandit operation.  Note that if a parameter's bound changes,
     #   we might also want to change the firefly noise or normalizations.
     return jnp.clip(new_features, 0.0, 1.0)
 
   def _create_features(
       self,
       features: jax.Array,
       rewards: jax.Array,
       features_batch: jax.Array,
       rewards_batch: jax.Array,
-      seed: chex.PRNGKey,
+      seed: jax.random.KeyArray,
   ) -> jax.Array:
     """Create new batch of mutated and perturbed features.
 
     The pool fireflies forces (pull/push) are being normalized to ensure the
     combined force doesn't throw the firefly too far. Mathematically, the
     normalization guarantees that the combined normalized force is within the
     simplex constructed by the unnormalized forces and therefore within bounds.
@@ -468,15 +465,18 @@
     # mask.
     directions = rewards - rewards_batch[:, jnp.newaxis]
     scaled_directions = jnp.where(
         directions >= 0.0, self.config.gravity, -self.config.negative_gravity
     )  # shape (batch_size, pool_size)
 
     # Normalize the distance by the number of features.
-    force = jnp.exp(-self.config.visibility * dists / self._n_features * 10.0)
+    # Get the number of non-padded features.
+    force = jnp.exp(
+        -self.config.visibility * dists / self.n_feature_dimensions * 10.0
+    )
     scaled_force = scaled_directions * force
     # Handle removed fireflies without updated rewards.
     finite_ind = jnp.isfinite(rewards).astype(scaled_force.dtype)
 
     # Ignore fireflies that were removed from the pool.
     scaled_force = scaled_force * finite_ind
 
@@ -534,42 +534,44 @@
     scale = norm_scaled_pulls + norm_scaled_push
     features_changes = jnp.matmul(scale, features) - features_batch * jnp.sum(
         scale, axis=-1, keepdims=True
     )
     return features_batch + features_changes
 
   def _create_random_perturbations(
-      self, perturbations_batch: jax.Array, seed: chex.PRNGKey
+      self,
+      perturbations_batch: jax.Array,
+      seed: jax.random.KeyArray,
   ) -> jax.Array:
     """Create random perturbations for the newly created batch.
 
     Args:
       perturbations_batch: (batch_size,)
       seed: Random seed.
 
     Returns:
       perturbations: (batch_size, n_features)
     """
     # Generate normalized noise for each batch.
     batch_noise = jax.random.laplace(
-        seed, shape=(self.batch_size, self._n_features)
+        seed, shape=(self.batch_size, self.n_feature_dimensions_with_padding)
     )
     batch_noise /= jnp.max(jnp.abs(batch_noise), axis=1, keepdims=True)
     return (
         batch_noise
         * perturbations_batch[:, jnp.newaxis]
-        * self._perturbation_factors
+        * self.param_handler.perturbation_factors
     )
 
   def update(
       self,
       state: VectorizedEagleStrategyState,
       batch_features: types.Array,
       batch_rewards: types.Array,
-      seed: chex.PRNGKey,
+      seed: jax.random.KeyArray,
   ) -> VectorizedEagleStrategyState:
     """Update the firefly pool based on the new batch of results.
 
     Arguments:
       state: Current state.
       batch_features: (batch_size, n_features)
       batch_rewards: (batch_size, )
@@ -674,15 +676,15 @@
 
   def _trim_pool(
       self,
       batch_features: jax.Array,
       batch_rewards: jax.Array,
       batch_perturbations: jax.Array,
       best_reward: jax.Array,
-      seed: chex.PRNGKey,
+      seed: jax.random.KeyArray,
   ) -> Tuple[jax.Array, jax.Array, jax.Array]:
     """Trim the pool by replacing unsuccessful fireflies with new random ones.
 
     A firefly is considered unsuccessful if its current perturbation is below
     'perturbation_lower_bound' and it's not the best fly seen thus far.
     Random features are created to replace the existing ones, and rewards
     are set to -np.inf to indicate that we don't have values for those feaures
@@ -700,15 +702,15 @@
     """
     indx = batch_perturbations < self.config.perturbation_lower_bound
     # Ensure the best firefly is never removed. For optimization purposes,
     # this logic is inside the if statement to be peformed only if needed.
     indx = indx & (batch_rewards != best_reward)
 
     # Replace fireflies with random features and evaluate rewards.
-    random_features = self._param_handler.random_features(self.batch_size, seed)
+    random_features = self.param_handler.random_features(self.batch_size, seed)
     new_batch_features = jnp.where(
         indx[..., jnp.newaxis], random_features, batch_features
     )
     new_batch_perturbations = jnp.where(
         indx, self.config.perturbation, batch_perturbations
     )
     # Setting rewards to -inf to filter out those fireflies during suggest.
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/eagle_strategy_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from jax import numpy as jnp
 import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import eagle_param_handler
 from vizier._src.algorithms.optimizers import eagle_strategy
 from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier.pyvizier import converters
+from vizier.pyvizier.converters import padding
 
 from absl.testing import absltest
 
 
 def _create_features_simple(
     features, rewards, features_batch, rewards_batch, config, n_features
 ):
@@ -66,18 +67,17 @@
         visibility=1, gravity=1, pool_size=4
     )
     problem = vz.ProblemStatement()
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
-    self.eagle = eagle_strategy.VectorizedEagleStrategy(
-        converter=converter, config=self.config, batch_size=2
-    )
-    self.eagle._iterations = 2
+    self.eagle = eagle_strategy.VectorizedEagleStrategyFactory(
+        eagle_config=self.config
+    )(converter=converter, suggestion_batch_size=2)
 
   def test_create_features(self):
     features = jnp.array([[1, 2], [3, 4], [7, 7], [8, 8]])
     rewards = jnp.array([2, 3, 4, 1])
     seed = jax.random.PRNGKey(0)
     features_batch = features[: self.eagle.batch_size]
     rewards_batch = rewards[: self.eagle.batch_size]
@@ -98,15 +98,15 @@
         features_batch,
         rewards_batch,
         self.config.replace(
             mutate_normalization_type=(
                 eagle_strategy.MutateNormalizationType.UNNORMALIZED
             )
         ),
-        self.eagle._n_features,
+        self.eagle.n_feature_dimensions,
     )
     actual = self.eagle._create_features(
         features,
         rewards,
         features_batch,
         rewards_batch,
         seed=seed,
@@ -193,16 +193,16 @@
   ):
     problem = vz.ProblemStatement()
     root = problem.search_space.root
     for i in range(100):
       root.add_float_param(f'x{i}', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     config = eagle_strategy.EagleStrategyConfig(max_pool_size=max_pool_size)
-    eagle = eagle_strategy.VectorizedEagleStrategy(
-        converter=converter, config=config, batch_size=batch_size
+    eagle = eagle_strategy.VectorizedEagleStrategyFactory(eagle_config=config)(
+        converter=converter, suggestion_batch_size=batch_size
     )
     self.assertEqual(eagle.pool_size, max_pool_size)
     self.assertEqual(eagle.batch_size, expected_batch_size)
 
   def test_trim_pool(self):
     pc = self.config.perturbation
     features_batch = jnp.array([[1, 2], [3, 4]], dtype=jnp.float64)
@@ -244,27 +244,49 @@
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     root.add_float_param('x3', 0.0, 1.0)
     eagle_factory = eagle_strategy.VectorizedEagleStrategyFactory()
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     eagle = eagle_factory(converter)
-    self.assertEqual(eagle._n_features, 3)
+    self.assertEqual(eagle.n_feature_dimensions, 3)
 
   def test_optimize_with_eagle(self):
     problem = vz.ProblemStatement()
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     root.add_float_param('x3', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     eagle_factory = eagle_strategy.VectorizedEagleStrategyFactory()
-    optimizer = vb.VectorizedOptimizer(strategy_factory=eagle_factory)
+    optimizer = vb.VectorizedOptimizerFactory(strategy_factory=eagle_factory)(
+        converter
+    )
+    converter = converters.TrialToArrayConverter.from_study_config(problem)
+    optimizer(score_fn=lambda x: -jnp.sum(x, 1), count=1)
+
+  def test_optimize_with_eagle_padding(self):
+    problem = vz.ProblemStatement()
+    root = problem.search_space.select_root()
+    root.add_float_param('x1', 0.0, 1.0)
+    root.add_float_param('x2', 0.0, 1.0)
+    root.add_float_param('x3', 0.0, 1.0)
+    converter = converters.PaddedTrialToArrayConverter.from_study_config(
+        problem,
+        padding_schedule=padding.PaddingSchedule(
+            num_trials=padding.PaddingType.POWERS_OF_2,
+            num_features=padding.PaddingType.POWERS_OF_2,
+        ),
+    )
+    eagle_factory = eagle_strategy.VectorizedEagleStrategyFactory()
     converter = converters.TrialToArrayConverter.from_study_config(problem)
-    optimizer.optimize(converter, score_fn=lambda x: -jnp.sum(x, 1), count=1)
+    optimizer = vb.VectorizedOptimizerFactory(strategy_factory=eagle_factory)(
+        converter
+    )
+    optimizer(score_fn=lambda x: -np.sum(x, 1), count=1)
 
 
 class EagleParamHandlerTest(parameterized.TestCase):
 
   def setUp(self):
     super(EagleParamHandlerTest, self).setUp()
     problem = vz.ProblemStatement()
@@ -273,24 +295,26 @@
     root.add_float_param('f1', 0.0, 5.0)
     root.add_categorical_param('c2', ['a', 'b', 'c'])
     root.add_discrete_param('d1', [2.0, 3.0, 5.0, 11.0])
     converter = converters.TrialToArrayConverter.from_study_config(
         problem, max_discrete_indices=0, pad_oovs=True
     )
     self.config = eagle_strategy.EagleStrategyConfig()
-    self.param_handler = eagle_param_handler.EagleParamHandler(
+    self.param_handler = eagle_param_handler.EagleParamHandler.build(
         converter=converter,
         categorical_perturbation_factor=self.config.categorical_perturbation_factor,
         pure_categorical_perturbation_factor=self.config.pure_categorical_perturbation_factor,
     )
 
   def test_init(self):
-    self.assertEqual(self.param_handler.n_features, 9)
-    self.assertFalse(self.param_handler.all_features_categorical)
-    self.assertTrue(self.param_handler.has_categorical)
+    self.assertEqual(self.param_handler.n_feature_dimensions, 9)
+    self.assertLen(
+        self.param_handler.perturbation_factors,
+        self.param_handler.n_feature_dimensions,
+    )
     self.assertEqual(self.param_handler.n_categorical, 2)
 
   def test_categorical_params_mask(self):
     expected_categorical_params_mask = np.array(
         [[1, 1, 1, 0, 0, 0, 0, 0, 0], [0, 0, 0, 0, 1, 1, 1, 1, 0]]
     )
     np.testing.assert_array_equal(
@@ -352,19 +376,17 @@
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
 
     prior_features = jnp.array([[1, -1], [2, 1], [3, 2], [4, 5]])
     prior_rewards = jnp.array([1, 2, 3, 4])
-    eagle = eagle_strategy.VectorizedEagleStrategy(
-        converter=converter,
-        config=config,
-        batch_size=2,
-    )
+    eagle = eagle_strategy.VectorizedEagleStrategyFactory(
+        eagle_config=config,
+    )(converter=converter, suggestion_batch_size=2)
     init_state = eagle.init_state(
         jax.random.PRNGKey(0), prior_features, prior_rewards
     )
     np.testing.assert_array_equal(
         init_state.features, jnp.flip(prior_features, axis=0)
     )
 
@@ -380,19 +402,17 @@
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
 
     prior_features = np.random.randn(n_prior_trials, 2)
     prior_rewards = np.random.randn(n_prior_trials)
 
-    eagle = eagle_strategy.VectorizedEagleStrategy(
-        converter=converter,
-        config=config,
-        batch_size=2,
-    )
+    eagle = eagle_strategy.VectorizedEagleStrategyFactory(
+        eagle_config=config,
+    )(converter=converter, suggestion_batch_size=2)
     init_state = eagle.init_state(
         jax.random.PRNGKey(0), prior_features, prior_rewards
     )
     self.assertEqual(init_state.features.shape, (config.pool_size, 2))
 
 
 if __name__ == '__main__':
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """L-BFGS-B Strategy optimizer."""
 
-from typing import Optional
+from typing import Optional, Union
 
 import attr
 import jax
 import jax.numpy as jnp
 import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import vectorized_base
@@ -31,46 +31,57 @@
 
 @attr.define(kw_only=True)
 class LBFGSBOptimizer:
   """L-BFGS-B optimizer."""
 
   # Number of parallel runs of L-BFGS-B.
   random_restarts: int = attr.field(init=True, repr=False, default=25)
-  # Number of features to consider at a time. The score function is assumed to
-  # score this many features at a time.
-  parallel_batch_size: Optional[int] = attr.field(default=None)
+  # In parallel optimization (suggesting multiple candidates at once), this is
+  # the number of candidates to consider at once. The score function is assumed
+  # to score this many candidates together and output a scalar.
+  num_parallel_candidates: Optional[int] = attr.field(default=None)
 
   def optimize(
       self,
       converter: converters.TrialToArrayConverter,
-      score_fn: vectorized_base.BatchArrayScoreFunction,
+      score_fn: Union[
+          vectorized_base.ParallelArrayScoreFunction,
+          vectorized_base.ArrayScoreFunction,
+      ],
       *,
       count: int = 1,
       seed: Optional[int] = None,
   ) -> list[vz.Trial]:
     """Optimize a continuous objective function using L-BFGS-B.
 
     Arguments:
       converter: Converter to map between trials and arrays.
-      score_fn: `BatchArrayScoreFunction`. Converts (batches of) features to
-        scores.
-      count: The number of best results to store.
+      score_fn: Converts (batches of) features to scores.
+      count: The number of best results to return.
       seed: Optional seed.
 
     Returns:
       The best trials found in the optimization.
     """
+    if self.num_parallel_candidates and count > 1:
+      # Note that we can't distinguish between 'BatchArrayScoreFunction' and
+      # 'ParallelArrayScoreFunction' using 'isinstance' as they both have the
+      # same function names.
+      raise ValueError(
+          "LBFGSBOptimizer doesn't support batch of batches (count > 1 is"
+          " disallowed when num_parallel_candidates is set)."
+      )
     optimize = optimizers.JaxoptLbfgsB(
         random_restarts=self.random_restarts, best_n=count
     )
     num_features = sum(spec.num_dimensions for spec in converter.output_specs)
 
     feature_shape = [num_features]
-    if self.parallel_batch_size is not None:
-      feature_shape = [self.parallel_batch_size, num_features]
+    if self.num_parallel_candidates is not None:
+      feature_shape = [self.num_parallel_candidates, num_features]
 
     def setup(rng):
       return jax.random.uniform(rng, shape=feature_shape)
 
     rng = jax.random.PRNGKey(seed or 0)
 
     # Constraints are [0, 1].
@@ -87,15 +98,15 @@
       return -score_fn(x[jnp.newaxis, ...])[0], dict()
 
     new_features, _ = optimize(
         setup, wrapped_score_fn, rng, constraints=constraints
     )
     new_rewards = np.asarray(score_fn(new_features[jnp.newaxis, ...]))[0]
 
-    if self.parallel_batch_size is None:
+    if self.num_parallel_candidates is None:
       parameters = converter.to_parameters(new_features[jnp.newaxis, ...])
     else:
       parameters = converter.to_parameters(new_features)
     trials = []
     for i in range(len(parameters)):
       trial = vz.Trial(parameters=parameters[i])
       trial.complete(vz.Measurement({'acquisition': new_rewards}))
@@ -104,13 +115,14 @@
 
 
 @attr.define
 class LBFGSBOptimizerFactory:
   """LBFGSB strategy optimizer factory."""
 
   def __call__(
-      self, random_restarts: int, parallel_batch_size: Optional[int] = None
+      self, random_restarts: int, num_parallel_candidates: Optional[int] = None
   ) -> LBFGSBOptimizer:
     """Generates a new LBFGSBOptimizer object."""
     return LBFGSBOptimizer(
-        parallel_batch_size=parallel_batch_size, random_restarts=random_restarts
+        num_parallel_candidates=num_parallel_candidates,
+        random_restarts=random_restarts,
     )
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,17 @@
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 1.0)
     problem.search_space.root.add_float_param('f2', 0.0, 1.0)
     problem.search_space.root.add_float_param('f3', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     # Minimize sum over all features.
     score_fn = lambda x: -jnp.sum(jnp.square(x - 0.52), axis=[-1, -2])
-    optimizer = lo.LBFGSBOptimizer(parallel_batch_size=3, random_restarts=10)
+    optimizer = lo.LBFGSBOptimizer(
+        num_parallel_candidates=3, random_restarts=10
+    )
     best_candidates = optimizer.optimize(
         converter=converter, score_fn=score_fn, count=1
     )
     self.assertLen(best_candidates, 3)
     # check the best candidates
     for b in best_candidates:
       self.assertLessEqual(np.abs(b.parameters['f1'].value - 0.52), 1e-6)
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -66,34 +66,40 @@
       batch_features: types.Array,
       batch_rewards: types.Array,
       seed: jax.random.KeyArray,
   ) -> None:
     return
 
 
-def _random_strategy_factory(
+def random_strategy_factory(
     converter: converters.TrialToArrayConverter,
     suggestion_batch_size: int,
 ) -> vb.VectorizedStrategy:
   """Creates a new vectorized strategy based on the Protocol."""
   return RandomVectorizedStrategy(
       converter=converter,
       suggestion_batch_size=suggestion_batch_size,
   )
 
 
 def create_random_optimizer(
-    max_evaluations: int, suggestion_batch_size: int
+    converter: converters.TrialToArrayConverter,
+    max_evaluations: int,
+    suggestion_batch_size: int,
 ) -> vb.VectorizedOptimizer:
   """Creates a random optimizer."""
-  return vb.VectorizedOptimizer(
-      strategy_factory=_random_strategy_factory,
+  return vb.VectorizedOptimizerFactory(
+      strategy_factory=random_strategy_factory,
       max_evaluations=max_evaluations,
       suggestion_batch_size=suggestion_batch_size,
-  )
+  )(converter=converter)
 
 
-def create_random_optimizer_factory() -> vb.VectorizedOptimizerFactory:
+def create_random_optimizer_factory(
+    max_evaluations: int, suggestion_batch_size: int
+) -> vb.VectorizedOptimizerFactory:
   """Creates a random optimizer factory."""
   return vb.VectorizedOptimizerFactory(
-      strategy_factory=_random_strategy_factory
+      strategy_factory=random_strategy_factory,
+      max_evaluations=max_evaluations,
+      suggestion_batch_size=suggestion_batch_size,
   )
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,22 @@
   def test_random_optimizer(self):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 10.0)
     problem.search_space.root.add_float_param('f2', 0.0, 10.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     score_fn = lambda x: np.sum(x, axis=-1)
     random_optimizer = rvo.create_random_optimizer(
-        max_evaluations=100, suggestion_batch_size=10)
-    res = random_optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=5)
-    self.assertLen(res, 5)
+        converter=converter, max_evaluations=100, suggestion_batch_size=10
+    )
+    res = random_optimizer(score_fn=score_fn, count=5)
+    self.assertLen(res.rewards, 5)
 
   def test_random_optimizer_factory(self):
-    random_optimizer_factory = rvo.create_random_optimizer_factory()
-    random_optimizer = random_optimizer_factory(
-        max_evaluations=100, suggestion_batch_size=10)
-    self.assertEqual(random_optimizer.suggestion_batch_size, 10)
-    self.assertEqual(random_optimizer.max_evaluations, 100)
+    random_optimizer_factory = rvo.create_random_optimizer_factory(
+        max_evaluations=100, suggestion_batch_size=10
+    )
+    self.assertEqual(random_optimizer_factory.suggestion_batch_size, 10)
+    self.assertEqual(random_optimizer_factory.max_evaluations, 100)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/vectorized_base.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/vectorized_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,33 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Base class for vectorized acquisition optimizers."""
 
 import abc
-import datetime
-import logging
-from typing import Generic, Optional, Protocol, Sequence, TypeVar
+from typing import Generic, Optional, Protocol, TypeVar, Union
 
 import attr
-import chex
+from flax import struct
 import jax
 from jax import numpy as jnp
+import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.jax import types
 from vizier.pyvizier import converters
 
 _S = TypeVar('_S')  # A container of optimizer state that works as a Pytree.
 
+ArrayConverter = Union[
+    converters.TrialToArrayConverter, converters.PaddedTrialToArrayConverter
+]
 
-@chex.dataclass(frozen=True)
+
+@struct.dataclass
 class VectorizedStrategyResults:
   """Container for a vectorized strategy result."""
 
   features: types.Array
   rewards: types.Array
 
 
@@ -106,42 +109,65 @@
 
   It's used in VectorizedOptimizer to create a new strategy every 'optimize'
   call.
   """
 
   def __call__(
       self,
-      converter: converters.TrialToArrayConverter,
+      converter: ArrayConverter,
       *,
       suggestion_batch_size: int,
   ) -> VectorizedStrategy:
     """Create a new vectorized strategy.
 
     Arguments:
       converter: The trial to array converter.
       suggestion_batch_size: The number of trials to be evaluated at once.
     """
     ...
 
 
-class BatchArrayScoreFunction(Protocol):
-  """Protocol for scoring array of batched trials."""
+class ArrayScoreFunction(Protocol):
+  """Protocol for scoring array of trials.
+
+  This protocol is suitable for optimizing batch of candidates (each one with
+  its own separate score).
+  """
 
   def __call__(self, batched_array_trials: types.Array) -> types.Array:
     """Evaluates the array of batched trials.
 
     Arguments:
-      batched_array_trials: 2D Array of shape (batch_size, n_features).
+      batched_array_trials: Array of shape (batch_size, n_feature_dimensions).
+
+    Returns:
+      Array of shape (batch_size,).
+    """
+
+
+class ParallelArrayScoreFunction(Protocol):
+  """Protocol for scoring array of parallel trials.
+
+  This protocol is suitable for optimizing in parallel multiple candidates
+  (e.g. qUCB).
+  """
+
+  def __call__(self, parallel_array_trials: types.Array) -> types.Array:
+    """Evaluates the array of batched trials.
+
+    Arguments:
+      parallel_array_trials: Array of shape (batch_size, n_parallel_candidates,
+        n_feature_dimensions).
 
     Returns:
-      1D Array of shape (batch_size,).
+      Array of shape (batch_size).
     """
 
 
-@attr.define(kw_only=True)
+@struct.dataclass
 class VectorizedOptimizer:
   """Vectorized strategy optimizer.
 
   The optimizer is stateless and will create a new vectorized strategy at the
   beginning of every 'optimize' call.
 
   The optimizer is responsible for running the iterative optimization process
@@ -151,38 +177,37 @@
   3. Tell the strategy about the rewards of its suggestion, so the strategy can
   update its internal state.
 
   The optimization process will terminate when the time limit or the total
   objective function evaluations limit has exceeded.
 
   Attributes:
-    strategy_factory: A factory for generating new strategy.
+    strategy: A factory for generating new strategy.
+    n_feature_dimensions_with_padding: Number of feature dimensions including
+      padding.
+    n_feature_dimensions: Number of feature dimensions (less than or equal to
+      `n_feature_dimensions_with_padding`).
+    suggestion_batch_size: Number of suggested points returned at each call.
     max_evaluations: The maximum number of objective function evaluations.
-    max_duration: The maximum duration of the optimization process.
-    suggestion_batch_size: The batch size of the suggestion vector received at
-      each 'suggest' call.
-    jit_loop: If True, JIT compile the optimization loop. If False, the loop
-      body (an optimization step) will still be JIT compiled, but the outer loop
-      will not be. (This arg is for speed testing and may be removed later.)
   """
 
-  strategy_factory: VectorizedStrategyFactory
-  suggestion_batch_size: int = 25
-  max_evaluations: int = 75_000
-  jit_loop: bool = True
+  strategy: VectorizedStrategy
+  n_feature_dimensions: int = struct.field(pytree_node=False)
+  n_feature_dimensions_with_padding: int = struct.field(pytree_node=False)
+  suggestion_batch_size: int = struct.field(pytree_node=False, default=25)
+  max_evaluations: int = struct.field(pytree_node=False, default=75_000)
 
-  def optimize(
+  def __call__(
       self,
-      converter: converters.TrialToArrayConverter,
-      score_fn: BatchArrayScoreFunction,
+      score_fn: ArrayScoreFunction,
       *,
       count: int = 1,
-      prior_trials: Optional[Sequence[vz.Trial]] = None,
+      prior_features: Optional[types.Array] = None,
       seed: Optional[int] = None,
-  ) -> list[vz.Trial]:
+  ) -> VectorizedStrategyResults:
     """Optimize the objective function.
 
     The ask-evaluate-tell optimization procedure that runs until the allocated
     time or evaluations count exceeds.
 
     The number of suggestions is determined by the strategy, which is the
     `suggestion_count` property.
@@ -194,93 +219,83 @@
     of the type associated with each array index, and which indices are part of
     the same CATEGORICAL parameter one-hot encoding.
 
     The optimization stops when either of 'max_evaluations' or 'max_duration' is
     reached.
 
     Arguments:
-      converter: The converter used to convert Trials to arrays.
       score_fn: A callback that expects 2D Array with dimensions (batch_size,
         features_count) and returns a 1D Array (batch_size,).
       count: The number of suggestions to generate.
-      prior_trials: Completed trials to be used for knowledge transfer. When the
-        optimizer is used to optimize a designer's acquisition function, the
+      prior_features: Completed trials to be used for knowledge transfer. When
+        the optimizer is used to optimize a designer's acquisition function, the
         prior trials are the previous designer suggestions provided in the
         ordered they were suggested.
       seed: The seed to use in the random generator.
 
     Returns:
       The best trials found in the optimization.
     """
-    seed = jax.random.PRNGKey(seed or 0)
-    if prior_trials:
-      # Sort the trials by the order they were created.
-      prior_trials = sorted(prior_trials, key=lambda x: x.creation_time)
-      prior_features = converter.to_features(prior_trials)
-      prior_rewards = score_fn(prior_features).reshape(-1)
-    else:
-      prior_features, prior_rewards = None, None
+    seed = jax.random.PRNGKey(0) if seed is None else seed
 
-    strategy = self.strategy_factory(
-        converter=converter,
-        suggestion_batch_size=self.suggestion_batch_size,
+    input_is_padded = (
+        self.n_feature_dimensions_with_padding > self.n_feature_dimensions
     )
+    dimension_is_missing = None
+    if input_is_padded:
+      dimension_is_missing = np.array(
+          [False] * self.n_feature_dimensions
+          + [True]
+          * (self.n_feature_dimensions_with_padding - self.n_feature_dimensions)
+      )
+    prior_rewards = None
+    if prior_features is not None:
+      prior_rewards = score_fn(prior_features).reshape(-1)
 
     def _optimization_one_step(_, args):
       state, best_results, seed = args
       suggest_seed, update_seed, new_seed = jax.random.split(seed, num=3)
-      new_features = strategy.suggest(state, suggest_seed)
+      new_features = self.strategy.suggest(state, suggest_seed)
+      # Ensure masking out padded dimensions in new features.
+      if input_is_padded:
+        new_features = jnp.where(
+            dimension_is_missing, jnp.zeros_like(new_features), new_features
+        )
+      # We assume `score_fn` is aware of padded dimensions.
       new_rewards = score_fn(new_features)
-      new_state = strategy.update(state, new_features, new_rewards, update_seed)
+      new_state = self.strategy.update(
+          state, new_features, new_rewards, update_seed
+      )
       new_best_results = self._update_best_results(
           best_results, count, new_features, new_rewards
       )
       return new_state, new_best_results, new_seed
 
-    def _optimize():
-      init_seed, loop_seed = jax.random.split(seed)
-      n_features = sum(spec.num_dimensions for spec in converter.output_specs)
-      init_best_results = VectorizedStrategyResults(
-          rewards=-jnp.inf * jnp.ones([count]),
-          features=jnp.zeros([count, n_features]),
-      )
-      init_args = (
-          strategy.init_state(
-              init_seed,
-              prior_features=prior_features,
-              prior_rewards=prior_rewards,
-          ),
-          init_best_results,
-          loop_seed,
-      )
-      return jax.lax.fori_loop(
-          0,
-          self.max_evaluations // self.suggestion_batch_size,
-          _optimization_one_step,
-          init_args,
-      )
-
-    if self.jit_loop:
-      _optimize = jax.jit(_optimize)  # pylint: disable=invalid-name
-
-    start_time = datetime.datetime.now()
-    _, best_results, _ = _optimize()
-    logging.info(
-        (
-            'Optimization completed. Duration: %s. Evaluations: %s. Best'
-            ' Results: %s'
-        ),
-        datetime.datetime.now() - start_time,
-        (
-            (self.max_evaluations // self.suggestion_batch_size)
-            * self.suggestion_batch_size
+    init_seed, loop_seed = jax.random.split(seed)
+    init_best_results = VectorizedStrategyResults(
+        rewards=-jnp.inf * jnp.ones([count]),
+        features=jnp.zeros([count, self.n_feature_dimensions_with_padding]),
+    )
+    init_args = (
+        self.strategy.init_state(
+            init_seed,
+            prior_features=prior_features,
+            prior_rewards=prior_rewards,
         ),
-        best_results,
+        init_best_results,
+        loop_seed,
     )
-    return self._best_candidates(best_results, converter)
+    _, best_results, _ = jax.lax.fori_loop(
+        0,
+        self.max_evaluations // self.suggestion_batch_size,
+        _optimization_one_step,
+        init_args,
+    )
+
+    return best_results
 
   def _update_best_results(
       self,
       best_results: VectorizedStrategyResults,
       count: int,
       batch_features: jax.Array,
       batch_rewards: jax.Array,
@@ -308,45 +323,74 @@
     )
     top_indices = jnp.argpartition(-all_rewards, count - 1)[:count]
     return VectorizedStrategyResults(
         rewards=all_rewards[top_indices],
         features=all_features[top_indices],
     )
 
-  def _best_candidates(
-      self,
-      best_results: VectorizedStrategyResults,
-      converter: converters.TrialToArrayConverter,
-  ) -> list[vz.Trial]:
-    """Returns the best candidate trials in the original search space."""
-    trials = []
-    sorted_ind = jnp.argsort(-best_results.rewards)
-    for i in range(len(best_results.rewards)):
-      # Create trials and convert the strategy features back to parameters.
-      ind = sorted_ind[i]
-      trial = vz.Trial(
-          parameters=converter.to_parameters(
-              jnp.expand_dims(best_results.features[ind], axis=0)
-          )[0]
-      )
-      trial.complete(vz.Measurement({'acquisition': best_results.rewards[ind]}))
-      trials.append(trial)
-    return trials
+
+def best_candidates_to_trials(
+    best_results: VectorizedStrategyResults,
+    converter: ArrayConverter,
+) -> list[vz.Trial]:
+  """Returns the best candidate trials in the original search space."""
+  trials = []
+  sorted_ind = jnp.argsort(-best_results.rewards)
+  for i in range(len(best_results.rewards)):
+    # Create trials and convert the strategy features back to parameters.
+    ind = sorted_ind[i]
+    trial = vz.Trial(
+        parameters=converter.to_parameters(
+            jnp.expand_dims(best_results.features[ind], axis=0)
+        )[0]
+    )
+    trial.complete(vz.Measurement({'acquisition': best_results.rewards[ind]}))
+    trials.append(trial)
+  return trials
+
+
+def trials_to_sorted_array(
+    prior_trials: list[vz.Trial],
+    converter: ArrayConverter,
+) -> Optional[types.Array]:
+  """Sorts trials by the order they were created and converts to array."""
+  if prior_trials:
+    prior_trials = sorted(prior_trials, key=lambda x: x.creation_time)
+    prior_features = converter.to_features(prior_trials)
+    # TODO: Update this code to work more cleanly with
+    # PaddedArrays.
+    if isinstance(converter, converters.PaddedTrialToArrayConverter):
+      # We need to mask out the `NaN` padded trials with zeroes.
+      prior_features = prior_features.padded_array
+      prior_features[len(prior_trials) :, ...] = 0.0
+  else:
+    prior_features = None
+  return prior_features
 
 
 @attr.define
 class VectorizedOptimizerFactory:
   """Vectorized strategy optimizer factory."""
 
   strategy_factory: VectorizedStrategyFactory
+  max_evaluations: int = 75_000
+  suggestion_batch_size: int = 25
 
   def __call__(
       self,
-      suggestion_batch_size: int,
-      max_evaluations: int,
+      converter: ArrayConverter,
   ) -> VectorizedOptimizer:
     """Generates a new VectorizedOptimizer object."""
+    strategy = self.strategy_factory(
+        converter, suggestion_batch_size=self.suggestion_batch_size
+    )
+    n_feature_dimensions = sum(
+        spec.num_dimensions for spec in converter.output_specs
+    )
+    n_feature_dimensions_with_padding = converter.to_features([]).shape[-1]
     return VectorizedOptimizer(
-        strategy_factory=self.strategy_factory,
-        suggestion_batch_size=suggestion_batch_size,
-        max_evaluations=max_evaluations,
+        strategy=strategy,
+        n_feature_dimensions=n_feature_dimensions,
+        n_feature_dimensions_with_padding=n_feature_dimensions_with_padding,
+        suggestion_batch_size=self.suggestion_batch_size,
+        max_evaluations=self.max_evaluations,
     )
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/vectorized_base_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/optimizers/vectorized_base_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -148,37 +148,37 @@
   @parameterized.parameters(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
   def test_optimize_candidates_len(self, count):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 10.0)
     problem.search_space.root.add_float_param('f2', 0.0, 10.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     score_fn = lambda x: jnp.sum(x, axis=-1)
-    optimizer = vb.VectorizedOptimizer(
+    optimizer = vb.VectorizedOptimizerFactory(
         strategy_factory=fake_increment_strategy_factory,
         max_evaluations=100,
-    )
-    res = optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=count
-    )
+    )(converter=converter)
+    res_array = optimizer(score_fn=score_fn, count=count)
+    res = vb.best_candidates_to_trials(res_array, converter=converter)
     self.assertLen(res, count)
 
   def test_best_candidates_count_is_1(self):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 1.0)
     problem.search_space.root.add_float_param('f2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     score_fn = lambda x: -jnp.max(jnp.square(x - 0.52), axis=-1)
     strategy_factory = FakeIncrementVectorizedStrategy
-    optimizer = vb.VectorizedOptimizer(
+    optimizer = vb.VectorizedOptimizerFactory(
         strategy_factory=strategy_factory,
         suggestion_batch_size=5,
         max_evaluations=10,
-    )
-    best_candidates = optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=1
+    )(converter=converter)
+    best_candidates_array = optimizer(score_fn=score_fn, count=1)
+    best_candidates = vb.best_candidates_to_trials(
+        best_candidates_array, converter=converter
     )
     # check the best candidate
     self.assertEqual(best_candidates[0].parameters['f1'].value, 0.5)
     self.assertEqual(best_candidates[0].parameters['f2'].value, 0.5)
     self.assertAlmostEqual(
         best_candidates[0].final_measurement.metrics['acquisition'].value,
         -((0.5 - 0.52) ** 2),
@@ -186,21 +186,22 @@
 
   def test_best_candidates_count_is_3(self):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 1.0)
     problem.search_space.root.add_float_param('f2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     score_fn = lambda x: -jnp.max(jnp.square(x - 0.52), axis=-1)
-    optimizer = vb.VectorizedOptimizer(
+    optimizer = vb.VectorizedOptimizerFactory(
         strategy_factory=fake_increment_strategy_factory,
         suggestion_batch_size=5,
         max_evaluations=10,
-    )
-    best_candidates = optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=3
+    )(converter=converter)
+    best_candidates_array = optimizer(score_fn=score_fn, count=3)
+    best_candidates = vb.best_candidates_to_trials(
+        best_candidates_array, converter=converter
     )
     # check 1st best candidate
     self.assertAlmostEqual(best_candidates[0].parameters['f1'].value, 0.5)
     self.assertAlmostEqual(best_candidates[0].parameters['f2'].value, 0.5)
     self.assertAlmostEqual(
         best_candidates[0].final_measurement.metrics['acquisition'].value,
         -((0.5 - 0.52) ** 2),
@@ -217,62 +218,76 @@
     self.assertAlmostEqual(best_candidates[2].parameters['f2'].value, 0.4)
     self.assertAlmostEqual(
         best_candidates[2].final_measurement.metrics['acquisition'].value,
         -((0.4 - 0.52) ** 2),
     )
 
   def test_vectorized_optimizer_factory(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('f1', 0.0, 1.0)
+    converter = converters.TrialToArrayConverter.from_study_config(problem)
     optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=fake_increment_strategy_factory
+        strategy_factory=fake_increment_strategy_factory,
+        suggestion_batch_size=5,
+        max_evaluations=1000,
     )
-    optimizer = optimizer_factory(suggestion_batch_size=5, max_evaluations=1000)
+    optimizer = optimizer_factory(converter)
     self.assertEqual(optimizer.max_evaluations, 1000)
     self.assertEqual(optimizer.suggestion_batch_size, 5)
 
   def test_prior_trials(self):
     """Test that the optimizer can correctly parsae and pass seed trials."""
     optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=fake_prior_trials_strategy_factory
+        strategy_factory=fake_prior_trials_strategy_factory,
+        suggestion_batch_size=5,
+        max_evaluations=100,
     )
-    optimizer = optimizer_factory(suggestion_batch_size=5, max_evaluations=100)
 
     study_config = vz.ProblemStatement(
         metric_information=[
             vz.MetricInformation(
                 name='obj', goal=vz.ObjectiveMetricGoal.MAXIMIZE
             )
         ]
     )
     root = study_config.search_space.root
     root.add_float_param('x1', 0.0, 10.0)
     root.add_float_param('x2', 0.0, 10.0)
     converter = converters.TrialToArrayConverter.from_study_config(study_config)
+    optimizer = optimizer_factory(converter)
 
     trial1 = vz.Trial(parameters={'x1': 1, 'x2': 1})
     measurement1 = vz.Measurement(metrics={'obj': vz.Metric(value=-10.33)})
     trial1.complete(measurement1, inplace=True)
 
     trial2 = vz.Trial(parameters={'x1': 2, 'x2': 2})
     measurement2 = vz.Measurement(metrics={'obj': vz.Metric(value=5.0)})
     trial2.complete(measurement2, inplace=True)
 
-    best_trial = optimizer.optimize(
-        converter,
+    prior_features = vb.trials_to_sorted_array(
+        [trial1, trial2, trial1], converter=converter
+    )
+    best_trial_array = optimizer(
         lambda x: -jnp.max(jnp.square(x - 0.52), axis=-1),
         count=1,
-        prior_trials=[trial1, trial2, trial1],
+        prior_features=prior_features,
+    )
+    best_trial = vb.best_candidates_to_trials(
+        best_trial_array, converter=converter
     )
     self.assertEqual(best_trial[0].parameters['x1'].value, 2)
     self.assertEqual(best_trial[0].parameters['x2'].value, 2)
 
-    best_trial = optimizer.optimize(
-        converter,
+    best_trial_array = optimizer(
         lambda x: -jnp.max(jnp.square(x - 0.52), axis=-1),
         count=1,
-        prior_trials=[trial1],
+        prior_features=vb.trials_to_sorted_array([trial1], converter=converter),
+    )
+    best_trial = vb.best_candidates_to_trials(
+        best_trial_array, converter=converter
     )
     self.assertEqual(best_trial[0].parameters['x1'].value, 1)
     self.assertEqual(best_trial[0].parameters['x2'].value, 1)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/policies/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy.py` & `google-vizier-0.1.6/vizier/_src/algorithms/policies/designer_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/policies/designer_policy_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 
 class DesignerPolicyNormalOperationTest(absltest.TestCase):
   """Tests Designer policies under error-free conditions."""
 
   def setUp(self):
     super().setUp()
-    self.maxDiff = None  # pylint: disable=invalid-name
+    self.maxDiff = None
 
   def test_restore_fully_serializable_designer(self):
     runner = _create_runner()
     policy = dp.SerializableDesignerPolicy(
         problem_statement=vz.ProblemStatement(),
         supporter=runner,
         designer_factory=lambda _, **kwargs: _FakeSerializableDesigner(),
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy.py` & `google-vizier-0.1.6/vizier/_src/algorithms/policies/random_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/policies/random_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample.py` & `google-vizier-0.1.6/vizier/_src/algorithms/random/random_sample.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/random/random_sample_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils.py` & `google-vizier-0.1.6/vizier/_src/algorithms/regression/trial_regression_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/regression/trial_regression_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/testing/__init__.py` & `google-vizier-0.1.6/vizier/_src/algorithms/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner.py` & `google-vizier-0.1.6/vizier/_src/algorithms/testing/comparator_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 NOTE: assert_converges_faster is a generic method name that conveys the general
 use of the class.
 """
 
 import logging
 
 import attr
+from jax import random
 import numpy as np
 from vizier import benchmarks
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier._src.benchmarks.analyzers import simple_regret_score
 from vizier.pyvizier import converters
 
@@ -92,21 +93,24 @@
                   baseline_state.algorithm.supporter.GetTrials()))
       candidate_curves.append(
           benchmarks.ConvergenceCurveConverter(
               baseline_statement.metric_information.item()).convert(
                   candidate_state.algorithm.supporter.GetTrials()))
 
     baseline_curve = benchmarks.ConvergenceCurve.align_xs(
-        baseline_curves, interpolate_repeats=True)
+        baseline_curves, interpolate_repeats=True
+    )[0]
     candidate_curve = benchmarks.ConvergenceCurve.align_xs(
-        candidate_curves, interpolate_repeats=True)
-    comparator = benchmarks.ConvergenceCurveComparator(baseline_curve)
+        candidate_curves, interpolate_repeats=True
+    )[0]
+    comparator = benchmarks.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=baseline_curve, compared_curve=candidate_curve
+    )
 
-    if (log_eff_score :=
-        comparator.get_log_efficiency_score(candidate_curve)) < score_threshold:
+    if (log_eff_score := comparator.score()) < score_threshold:
       raise FailedComparisonTestError(
           f'Log efficiency score {log_eff_score} is less than {score_threshold}'
           f' when comparing algorithms: {candidate_state_factory} '
           f'vs baseline of {baseline_state_factory} for {self.num_trials} '
           f' Trials with {self.num_repeats} repeats')
 
 
@@ -134,38 +138,45 @@
           attr.validators.ge(0), attr.validators.le(0.1)),
       default=0.05)
   goal: vz.ObjectiveMetricGoal
 
   def assert_optimizer_better_simple_regret(
       self,
       converter: converters.TrialToArrayConverter,
-      score_fn: vb.BatchArrayScoreFunction,
-      baseline_optimizer_factory: vb.VectorizedOptimizerFactory,
-      candidate_optimizer_factory: vb.VectorizedOptimizerFactory,
+      score_fn: vb.ArrayScoreFunction,
+      baseline_strategy_factory: vb.VectorizedStrategyFactory,
+      candidate_strategy_factory: vb.VectorizedStrategyFactory,
   ) -> None:
     """Assert if candidate optimizer has better simple regret than the baseline.
     """
     baseline_obj_values = []
     candidate_obj_values = []
 
-    baseline_optimizer = baseline_optimizer_factory(
+    baseline_optimizer_factory = vb.VectorizedOptimizerFactory(
+        baseline_strategy_factory,
         suggestion_batch_size=self.baseline_suggestion_batch_size,
-        max_evaluations=self.baseline_num_trials)
-
-    candidate_optimizer = candidate_optimizer_factory(
+        max_evaluations=self.baseline_num_trials,
+    )
+    candidate_optimizer_factory = vb.VectorizedOptimizerFactory(
+        candidate_strategy_factory,
         suggestion_batch_size=self.candidate_suggestion_batch_size,
-        max_evaluations=self.candidate_num_trials)
+        max_evaluations=self.candidate_num_trials,
+    )
+    baseline_optimizer = baseline_optimizer_factory(converter)
+    candidate_optimizer = candidate_optimizer_factory(converter)
 
     for i in range(self.baseline_num_repeats):
-      trial = baseline_optimizer.optimize(converter, score_fn, count=1, seed=i)
+      res = baseline_optimizer(score_fn, count=1, seed=random.PRNGKey(i))
+      trial = vb.best_candidates_to_trials(res, converter)
       baseline_obj_values.append(
           trial[0].final_measurement.metrics['acquisition'].value)
 
     for i in range(self.candidate_num_repeats):
-      trial = candidate_optimizer.optimize(converter, score_fn, count=1, seed=i)
+      res = candidate_optimizer(score_fn, count=1, seed=random.PRNGKey(i))
+      trial = vb.best_candidates_to_trials(res, converter)
       candidate_obj_values.append(
           trial[0].final_measurement.metrics['acquisition'].value)
 
     self._conclude_test(baseline_obj_values, candidate_obj_values)
 
   def assert_benchmark_state_better_simple_regret(
       self,
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner_test.py` & `google-vizier-0.1.6/vizier/_src/algorithms/testing/comparator_runner_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,36 +346,28 @@
       return FakeVectorizedStrategy(
           converter=converter,
           good_value=candidate_x_value,
           bad_value=0.0,
           num_trial_to_converge=0,
       )
 
-    baseline_optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=_baseline_strategy_factory
-    )
-
-    candidate_optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=_candidate_strategy_factory
-    )
-
     if should_pass:
       simple_regret_test.assert_optimizer_better_simple_regret(
           self.converter,
           score_fn,
-          baseline_optimizer_factory,
-          candidate_optimizer_factory,
+          _baseline_strategy_factory,
+          _candidate_strategy_factory,
       )
     else:
       with self.assertRaises(  # pylint: disable=g-error-prone-assert-raises
           comparator_runner.FailedSimpleRegretConvergenceTestError
       ):
         simple_regret_test.assert_optimizer_better_simple_regret(
             self.converter,
             score_fn,
-            baseline_optimizer_factory,
-            candidate_optimizer_factory,
+            _baseline_strategy_factory,
+            _candidate_strategy_factory,
         )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/testing/optimizer_test_utils.py` & `google-vizier-0.1.6/vizier/_src/algorithms/testing/optimizer_test_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/algorithms/testing/test_runners.py` & `google-vizier-0.1.6/vizier/_src/algorithms/testing/test_runners.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/convergence_curve.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Converters and comparators for convergence curves."""
 
+import abc
+import bisect
 import enum
+import logging
 from typing import Callable, List, Optional, Sequence, Union
 
 import attr
 import numpy as np
 from vizier import pyvizier
 from vizier.pyvizier import converters
 from vizier.pyvizier import multimetric
@@ -43,92 +46,154 @@
     INCREASING = 'increasing'
     DECREASING = 'decreasing'
 
   trend: YTrend = YTrend.UNKNOWN
 
   def __attrs_post_init__(self):
     if len(self.ys.shape) != 2:
-      raise ValueError(f'Shapes for ys should be batch size by time {self.ys}')
+      raise ValueError(
+          'The shape of ys should be (batch_size, n_steps); but ys shape is'
+          f' {self.ys.shape}'
+      )
     if len(self.xs) != self.ys.shape[1]:
       raise ValueError(
           f'Shape mismatch for time dim: {len(self.xs)} vs {self.ys.shape}'
       )
+    # Allow for small numerical imprecisions.
     if self.trend == ConvergenceCurve.YTrend.INCREASING:
-      if not np.all(np.nan_to_num(np.diff(self.ys, axis=-1)) >= 0):
+      if not np.all(np.nan_to_num(np.diff(self.ys, axis=-1)) >= -1e-8):
         raise ValueError(f'Increasing trend not found: {self.ys}')
 
     if self.trend == ConvergenceCurve.YTrend.DECREASING:
-      if not np.all(np.nan_to_num(np.diff(self.ys, axis=-1)) <= 0):
+      if not np.all(np.nan_to_num(np.diff(self.ys, axis=-1)) <= 1e-8):
         raise ValueError(f'Decreasing trend not found: {self.ys}')
 
   @property
   def batch_size(self) -> int:
     return self.ys.shape[0]
 
   @classmethod
-  def align_xs(cls,
-               curves: Sequence['ConvergenceCurve'],
-               *,
-               resolution: Optional[int] = None,
-               interpolate_repeats=False) -> 'ConvergenceCurve':
-    """Align curves to the same xs using linear interpolation.
+  def _interpolate_curves(
+      cls,
+      curves: Sequence['ConvergenceCurve'],
+      *,
+      resolution: Optional[int] = None,
+      interpolate_repeats: bool = False,
+  ) -> tuple[np.ndarray, list[np.ndarray]]:
+    """Interpolate curves to have the same xs using linear interpolation.
 
     If xs are greater than xp[-1], then default is np.nan.
 
     Args:
       curves:
       resolution: Number of points to interpolate to. Leave it None to use the
         maximal resolution.
-      interpolate_repeats: Interpolate repeated values in the curve via
-      linear interpolation (except for the last repeated segment).
+      interpolate_repeats: Interpolate repeated values (xs and ys) in the curve
+        via linear interpolation (except for the last repeated segment).
 
     Returns:
-      ConvergenceCurve whose batch size is equal to the sum of the batch size
-      of `curves`.
+      A tuple of the interpolated xs array, and a list of the interpolated ys
+      arrays.
     """
     if not curves:
       raise ValueError('Empty sequence of curves.')
     if len(set([c.trend for c in curves])) > 1:
       raise ValueError('All curves must be increasing or decreasing.')
     minx = np.min([np.min(c.xs) for c in curves])
     maxx = np.max([np.max(c.xs) for c in curves])
     resolution = resolution or np.max([np.size(c.xs) for c in curves])
     xs = np.linspace(minx, maxx, resolution)
 
     all_ys = []
     for curve in curves:
+      curve_ys = []
       for ys in curve.ys:
         if interpolate_repeats:
           _, indices = np.unique(ys, return_index=True)
           # Sorting indices from increasing order due to sign differences.
           indices = sorted(indices)
           if len(ys) - 1 not in indices:
             indices.append(len(ys) - 1)
         else:
           # Use the whole curve.
           indices = range(len(ys))
-
-        all_ys.append(
+        curve_ys.append(
             np.interp(
                 xs,
                 np.array([curve.xs[i] for i in indices]),
                 np.array([ys[i] for i in indices]),
-                right=np.nan))
+                right=np.nan,
+            )
+        )
+      all_ys.append(np.stack(curve_ys, axis=0))
+    return xs, all_ys
 
+  @classmethod
+  def _align_xs_combine_ys(
+      cls,
+      curves: Sequence['ConvergenceCurve'],
+      *,
+      resolution: Optional[int] = None,
+      interpolate_repeats: bool = False,
+  ) -> list['ConvergenceCurve']:
+    """Align curves (same xs) using linear interpolation and combine all ys."""
+    xs, all_ys = cls._interpolate_curves(
+        curves, resolution=resolution, interpolate_repeats=interpolate_repeats
+    )
     # Take all non-empty ylabels.
     ylabels = list(set([c.ylabel for c in curves if c.ylabel]))
     if not ylabels:
       ylabel = ''
     elif len(ylabels) > 1:
-      print('Curves have different ylabels: %s.', ylabels)
+      logging.info(
+          'Curves have different ylabels: %s. None of them is selected.',
+          ylabels,
+      )
       ylabel = ''
     else:
       ylabel = ylabels[0]
+    return [
+        cls(xs=xs, ys=np.vstack(all_ys), ylabel=ylabel, trend=curves[0].trend)
+    ]
 
-    return cls(xs=xs, ys=np.stack(all_ys), ylabel=ylabel, trend=curves[0].trend)
+  @classmethod
+  def _align_xs_keep_ys(
+      cls,
+      curves: Sequence['ConvergenceCurve'],
+      *,
+      resolution: Optional[int] = None,
+      interpolate_repeats: bool = False,
+  ) -> list['ConvergenceCurve']:
+    """Align curves (same xs) using linear interpolation and keep ys."""
+    xs, all_ys = cls._interpolate_curves(
+        curves, resolution=resolution, interpolate_repeats=interpolate_repeats
+    )
+    return [
+        cls(xs=xs, ys=ys, ylabel=curves[i].ylabel, trend=curves[0].trend)
+        for i, ys in enumerate(all_ys)
+    ]
+
+  @classmethod
+  def align_xs(
+      cls,
+      curves: Sequence['ConvergenceCurve'],
+      *,
+      resolution: Optional[int] = None,
+      interpolate_repeats: bool = False,
+      keep_curves_separate: bool = False,
+  ) -> list['ConvergenceCurve']:
+    """Align curves (same xs) using linear interpolation."""
+    if keep_curves_separate:
+      return cls._align_xs_keep_ys(
+          curves, resolution=resolution, interpolate_repeats=interpolate_repeats
+      )
+    else:
+      return cls._align_xs_combine_ys(
+          curves, resolution=resolution, interpolate_repeats=interpolate_repeats
+      )
 
   @classmethod
   def extrapolate_ys(cls,
                      curve: 'ConvergenceCurve',
                      steps: int = 0) -> 'ConvergenceCurve':
     """Extrapolates the future ys using a variant of linear extrapolation.
 
@@ -189,31 +254,31 @@
     self.cost_fn = cost_fn
     self.measurements_type = measurements_type
 
   def convert(self, trials: Sequence[pyvizier.Trial]) -> ConvergenceCurve:
     """Returns ConvergenceCurve of batch size 1."""
     yvals = [np.nan]
     xvals = [0]
-    comparator = self.comparator
+
     for trial in trials:
       candidates = [np.nan]
       if self.measurements_type in ('final', 'all'):
         if trial.final_measurement and (self.metric_information.name
                                         in trial.final_measurement.metrics):
           candidates.append(trial.final_measurement.metrics[
               self.metric_information.name].value)
       if self.measurements_type in ('intermediate', 'all'):
         for measurement in trial.measurements:
           if self.metric_information.name in measurement.metrics:
             candidates.append(
                 measurement.metrics[self.metric_information.name].value)
 
-      yvalue = comparator(candidates)
+      yvalue = self.comparator(candidates)
       xvals.append(xvals[-1] + self.cost_fn(trial))
-      yvals.append(comparator([yvalue, yvals[-1]]))
+      yvals.append(self.comparator([yvalue, yvals[-1]]))
 
     yvals = np.asarray(yvals[1:])
     if self.metric_information.goal == pyvizier.ObjectiveMetricGoal.MAXIMIZE:
       trend = ConvergenceCurve.YTrend.INCREASING
       flipped = False
     elif self.flip_signs_for_min:
       trend = ConvergenceCurve.YTrend.INCREASING
@@ -292,162 +357,364 @@
         xs=np.asarray(range(1, len(hv_curve) + 1)),
         ys=np.asarray(hv_curve).reshape([1, -1]),
         trend=ConvergenceCurve.YTrend.INCREASING,
         ylabel='hypervolume',
     )
 
 
-class ConvergenceCurveComparator:
+@attr.define
+class ConvergenceComparatorBase(abc.ABC):
+  """Base class for convergence curve compartors.
+
+  Attributes:
+    baseline_curve: The baseline ConvergenceCurve.
+    compared_curve: The compared ConvergenceCurve.
+    baseline_quantile: Quantile in [0, 1] of the batched baseline curve to use
+      for efficiency comparison. The higher the quantile, the better the quality
+      of the baseline batch.
+    compared_quantile: Quantile in [0, 1] of the batched compared curve to use
+      for efficiency comparison. The higher the quantile, the better the quality
+      of the baseline batch.
+  """
+
+  _baseline_curve: ConvergenceCurve = attr.field()
+  _compared_curve: ConvergenceCurve = attr.field()
+  _baseline_quantile: float = attr.field(
+      default=0.5,
+      validator=[attr.validators.le(1), attr.validators.ge(0)],
+      kw_only=True,
+  )
+  _compared_quantile: float = attr.field(
+      default=0.5,
+      validator=[attr.validators.le(1), attr.validators.ge(0)],
+      kw_only=True,
+  )
+  _sign: float = attr.field(init=False)
+
+  def __attrs_post_init__(self):
+    """Validates the curves and determines the sign.
+
+    Raises:
+      ValueError: If baseline curve is not INCREASING or DECREASING.
+      ValueError: If the trends mismatch.
+      ValueError: If baseline_quantile or compared_quantile are not in [0, 1].
+    """
+    if self._baseline_curve.trend not in (
+        ConvergenceCurve.YTrend.INCREASING,
+        ConvergenceCurve.YTrend.DECREASING,
+    ):
+      raise ValueError(
+          f'Curve trend {self._baseline_curve.trend} must be either'
+          'increasing or decreasing.'
+      )
+    if self._baseline_curve.trend != self._compared_curve.trend:
+      raise ValueError(
+          f'Baseline curve trend {self._baseline_curve.trend}'
+          f' must match compared curve trend {self._compared_curve.trend}'
+      )
+    self._sign = (
+        1.0
+        if (self._baseline_curve.trend == ConvergenceCurve.YTrend.INCREASING)
+        else -1.0
+    )
+
+  def _standardize_curves(
+      self,
+      xs_cutoff: Optional[float] = None,
+  ) -> tuple[np.ndarray, np.ndarray]:
+    """Standardize convergence curves.
+
+    Note: This is an helper function that the class implementing this interface
+    can choose to use or not.
+
+    1. Align xs and keeping each ys.
+    2. Apply quantiles and impute NaN.
+    3. Remove values where xs < xs_cutoff.
+
+    Args:
+      xs_cutoff: The xs value before which values are ignored.
+
+    Returns:
+      The standardize baseline and compared curves.
+    """
+    # Align the curves while keeping each ys.
+    align_baseline_curve, align_compared_curve = ConvergenceCurve.align_xs(
+        [self._baseline_curve, self._compared_curve],
+        interpolate_repeats=False,
+        keep_curves_separate=True,
+    )
+    # Apply batch quantiels.
+    baseline_ys = np.nanquantile(
+        self._sign * align_baseline_curve.ys,
+        self._baseline_quantile,
+        axis=0,
+    )
+    compared_ys = np.nanquantile(
+        self._sign * align_compared_curve.ys,
+        self._compared_quantile,
+        axis=0,
+    )
+    # Impute NaN values as -inf. This happens due to `align_xs` assigning
+    # np.nan for xs that are outside the original convergence curve.
+    baseline_ys = np.nan_to_num(baseline_ys, nan=-np.inf)
+    compared_ys = np.nan_to_num(compared_ys, nan=-np.inf)
+
+    # Remove burn cutoff values.
+    if xs_cutoff is not None:
+      baseline_cutoff_ind = np.where(align_baseline_curve.xs >= xs_cutoff)[0]
+      compared_cutoff_ind = np.where(align_compared_curve.xs >= xs_cutoff)[0]
+      if np.size(baseline_cutoff_ind) == 0 or np.size(compared_cutoff_ind) == 0:
+        raise ValueError('fThe given burn_cutoff {xs_cutoff} value is too high')
+      else:
+        baseline_ys = baseline_ys[baseline_cutoff_ind[0] :]
+        compared_ys = compared_ys[compared_cutoff_ind[0] :]
+
+    return baseline_ys, compared_ys
+
+  @abc.abstractmethod
+  def score(self) -> float:
+    ...
+
+
+@attr.define
+class LogEfficiencyConvergenceCurveComparator(ConvergenceComparatorBase):
   """Comparator methods for ConvergenceCurves.
 
   Methods in this class generally return comparison metrics for a compared curve
   against a baseline curve. Only works for curves with INCREASING or DECREASING
   trend.
 
   Example usage:
     baseline_curve = ConvergenceCurve(...)
-    comparator = ConvergenceCurveComparator(baseline_curve)
+    comparator = LogEfficiencyConvergenceCurveComparator(baseline_curve)
     comparator.log_efficiency_curve(compared_curve)
   """
+  max_score: float = attr.field(
+      default=5.0, validator=[attr.validators.ge(0)], kw_only=True
+  )
+  summary_function: Callable[[np.ndarray], float] = attr.field(
+      default=np.median
+  )
 
-  def __init__(self, baseline_curve: ConvergenceCurve):
-    """Initialize class with baseline curve.
-
-    Args:
-      baseline_curve: A baseline ConvergenceCurve to compare against.
-
-    Raises:
-      ValueError: If baseline curve is not INCREASING or DECREASING.
-    """
-    if baseline_curve.trend not in (ConvergenceCurve.YTrend.INCREASING,
-                                    ConvergenceCurve.YTrend.DECREASING):
-      raise ValueError(f'Curve trend {baseline_curve.trend} must be either'
-                       'increasing or decreasing.')
-    self._baseline_curve = baseline_curve
-    self._sign = 1.0 if (self._baseline_curve.trend
-                         == ConvergenceCurve.YTrend.INCREASING) else -1.0
-
-  def log_efficiency_curve(self,
-                           compared_curve: ConvergenceCurve,
-                           baseline_quantile: float = 0.5,
-                           compared_quantile: float = 0.5) -> ConvergenceCurve:
+  def log_efficiency_curve(self) -> ConvergenceCurve:
     """Builds the log sample efficiency curve.
 
     The compared curve should approximately use exp(-relative efficiency)% less
     Trials than the baseline curve. Note that a positive relative effiency
     demonstrates that the compared curve is better than the baseline. Also,
     the relative efficiency CURVES are not fully symmetric due to differences
     in drops in objective values.
 
-    Args:
-      compared_curve: Compared convergence curve.
-      baseline_quantile: Quantile in [0, 1] of the batched baseline curve to use
-        for efficiency comparison. The higher the quantile, the better the
-        quality of the baseline batch.
-      compared_quantile: Quantile in [0, 1] of the batched compared curve to use
-        for efficiency comparison. The higher the quantile, the better the
-        quality of the baseline batch.
-
     Returns:
       ConvergenceCurves with ys (batch size 1) as the relative efficiency curve.
 
       The xs of curve is equal to the xs of baseline curve but there
       may be indices equal to positive 'inf' which indicate that no point
       in the compared curve outperforms the baseline at that index.
 
     Raises:
       ValueError: If the trends do mismatch.
       ValueError: If baseline_quantile or compared_quantile are not in [0, 1].
     """
-    if self._baseline_curve.trend != compared_curve.trend:
-      raise ValueError(
-          f'Baseline curve trend {self._baseline_curve.trend}'
-          f' must match compared curve trend {compared_curve.trend}')
+
     baseline_quantile = np.nanquantile(
-        self._sign * self._baseline_curve.ys, baseline_quantile, axis=0)
+        self._sign * self._baseline_curve.ys, self._baseline_quantile, axis=0
+    )
     # This may not be [1,2,...] due to repeats.
     baseline_index_curve = build_convergence_curve(baseline_quantile,
                                                    baseline_quantile)
 
     other_index_curve = build_convergence_curve(
         baseline_quantile,
         np.nanquantile(
-            self._sign * compared_curve.ys, compared_quantile, axis=0))
+            self._sign * self._compared_curve.ys,
+            self._compared_quantile,
+            axis=0,
+        ),
+    )
 
     ys = np.log(1 + np.asarray(baseline_index_curve)) - np.log(
         1 + np.asarray(other_index_curve))
     return ConvergenceCurve(
         xs=self._baseline_curve.xs, ys=ys.reshape(1, len(ys)))
 
-  def get_log_efficiency_score(self,
-                               compared_curve: ConvergenceCurve,
-                               baseline_quantile=0.5,
-                               compared_quantile=0.5,
-                               max_score=5) -> float:
+  def score(self) -> float:
     """Gets a finalized log efficiency score.
 
     The compared curve should approximately use exp(-score)% Trials compared to
     the baseline curve. Note that a high positive score demonstrates that the
     compared curve uses less Trials and is better than the baseline.
 
-    Args:
-      compared_curve: Compared convergence curve.
-      baseline_quantile: Quantile in [0, 1] of the batched baseline curve to use
-        for efficiency comparison. The higher the quantile, the better the
-        quality of the baseline batch.
-      compared_quantile: Quantile in [0, 1] of the batched compared curve to use
-        for efficiency comparison. The higher the quantile, the better the
-        quality of the baseline batch.
-      max_score: Maximum log efficiency score.
-
     Returns:
       Sample efficiency score. This score is symmetric and always finite when
       baseline_quantile <= compare_quantile (recommended setting).
     """
-    baseline_curve = ConvergenceCurve.align_xs([self._baseline_curve],
-                                               interpolate_repeats=True)
-    compared_curve = ConvergenceCurve.align_xs([compared_curve],
-                                               interpolate_repeats=True)
+    baseline_curve = ConvergenceCurve.align_xs(
+        [self._baseline_curve], interpolate_repeats=True
+    )[0]
+    compared_curve = ConvergenceCurve.align_xs(
+        [self._compared_curve], interpolate_repeats=True
+    )[0]
     # Combined curve (as the baseline) becomes the y-values at which
     # Trial efficiency is evaluated.
-    combined_curve = ConvergenceCurve.align_xs([baseline_curve, compared_curve])
+    combined_curve = ConvergenceCurve.align_xs(
+        [baseline_curve, compared_curve]
+    )[0]
     combined_curve.ys = np.nanmedian(combined_curve.ys, axis=0, keepdims=True)
-    comparator = ConvergenceCurveComparator(baseline_curve=combined_curve)
 
     # Look ahead for exp(max_score)*T steps, as score is in the log space.
-    extend_steps = int(np.exp(max_score) * len(self._baseline_curve.xs))
-    extended_baseline = ConvergenceCurve.extrapolate_ys(self._baseline_curve,
-                                                        extend_steps)
-    extended_compared = ConvergenceCurve.extrapolate_ys(compared_curve,
-                                                        extend_steps)
-
-    efficiency_baseline = comparator.log_efficiency_curve(
-        extended_baseline, compared_quantile=baseline_quantile)
-    efficiency_compared = comparator.log_efficiency_curve(
-        extended_compared, compared_quantile=compared_quantile)
+    extend_steps = int(np.exp(self.max_score) * len(self._baseline_curve.xs))
+    extended_baseline = ConvergenceCurve.extrapolate_ys(
+        baseline_curve, extend_steps
+    )
+    extended_compared = ConvergenceCurve.extrapolate_ys(
+        compared_curve, extend_steps
+    )
+    baseline_comparator = LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=combined_curve,
+        compared_curve=extended_baseline,
+        compared_quantile=self._baseline_quantile,
+    )
+    efficiency_baseline = baseline_comparator.log_efficiency_curve()
+    compared_comparator = LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=combined_curve,
+        compared_curve=extended_compared,
+        compared_quantile=self._compared_quantile,
+    )
+    efficiency_compared = compared_comparator.log_efficiency_curve()
 
     # Clip log efficiency and return median log efficiency in last half.
     diff = np.clip(
-        efficiency_compared.ys, a_min=-max_score, a_max=max_score) - np.clip(
-            efficiency_baseline.ys, a_min=-max_score, a_max=max_score)
-    return np.median(diff[int(len(diff) / 2):])
+        efficiency_compared.ys, a_min=-self.max_score, a_max=self.max_score
+    ) - np.clip(
+        efficiency_baseline.ys, a_min=-self.max_score, a_max=self.max_score
+    )
+    return self.summary_function(diff)
+
+
+@attr.define
+class SimpleConvergenceCurveComparator(ConvergenceComparatorBase):
+  """Comparator method based on simple comparison.
+
+  Attributes:
+    burn_cutoff: The cutoff below which values not included in score.
+  """
+
+  _xs_cutoff: Optional[float] = None
+
+  def score(self) -> float:
+    """Computes the simple convergence score.
 
+    The score is the percentage of indices (after the burn cutoff) for which the
+    interpolated values of 'compared_curve' are better than the interpolated
+    values of 'baseline_curve'. A large score value means 'compared' is better.
 
-def build_convergence_curve(baseline_curve: Sequence[float],
-                            compared_curve: Sequence[float]) -> List[float]:
+    Returns:
+      The percentage better convergence score [0.0, 1.0].
+
+    Raises:
+      ValueError: If curve trends are not INCREASING or DECREASING, or not
+      equal.
+    """
+    baseline_ys, compared_ys = self._standardize_curves(self._xs_cutoff)
+    # Compute mean indices that compared is better than baseline.
+    return np.mean(baseline_ys < compared_ys)
+
+
+@attr.define
+class PercentageBetterConvergenceCurveComparator(ConvergenceComparatorBase):
+  """Comparator method based on percentage better.
+
+  Attributes:
+    burn_cutoff: The cutoff below which values not included in score.
+  """
+
+  _xs_cutoff: Optional[float] = None
+
+  def _compute_directional_score(
+      self, baseline: np.ndarray, compared: np.ndarray
+  ) -> float:
+    """Compute the percentage better score.
+
+    The score is the average percentage steps that 'compared' is better than
+    'baseline'.
+
+    Note that: sum_i sum_j 1{c_j > b_i} = sum_j sum_i {b_i < c_j}. Therefore, we
+    can either iterate over 'compared' and count the number of steps that
+    'baseline' is worse OR we can iterate over 'baseline' and count the number
+    of steps that 'compared' is better (which is the current implementation).
+
+    Implementation
+    --------------
+    1. For each index of `baseline`:
+      - Finds the smallest index of 'comared' that is better.
+      - Compute the percentage of `compared` steps that are better.
+    2. Average the percentages across all 'baseline' indices.
+
+    The more dominante 'compared' over 'baseline' the closer the score is to
+    1.0.
+
+    Args:
+      baseline: The baseline convergence curve.
+      compared: The compared convergence curve.
+
+    Returns:
+      The average number of steps that compared is better than baseline (score
+      is in [0, 1]).
+    """
+    convergence_curve = build_convergence_curve(list(baseline), list(compared))
+    pct_baseline_compared = [
+        (len(compared) - i) / len(compared) if i != float('inf') else 0
+        for i in convergence_curve
+    ]
+    return np.mean(pct_baseline_compared)
+
+  def score(self) -> float:
+    """Computes the percentage better score.
+
+    The score has two components:
+    (a) sub-score quantifying how much 'compared' domniates 'baseline'.
+    (b) sub-score quantifying how much 'baseline' domniates 'compared'.
+
+    The final score is (a) - (b).
+
+    Returns:
+      The normalized percentage better convergence score [-1.0, 1.0].
+
+    Raises:
+      ValueError: If curve trends are not INCREASING or DECREASING, or not
+      equal.
+    """
+    baseline_ys, compared_ys = self._standardize_curves(self._xs_cutoff)
+    baseline_compared_score = self._compute_directional_score(
+        baseline_ys, compared_ys
+    )
+    compared_baseline_score = self._compute_directional_score(
+        compared_ys, baseline_ys
+    )
+    return baseline_compared_score - compared_baseline_score
+
+
+def build_convergence_curve(
+    baseline_curve: Sequence[float], compared_curve: Sequence[float]
+) -> List[float]:
   """Builds a relative convergence curve (see returns for definition).
 
+  Finds the smallest index j for each element i in 'baseline_curve'
+  such that baseline_curve[i] <= compared_curve[j]. The function uses the
+  'bisect_left' function to efficiently perform binary search under the
+  assumption that 'baseline_curve' and 'compared_curve' are sorted in
+  non-decreasing order.
+
   Args:
     baseline_curve: Baseline maximization convergence curve.
     compared_curve: Compared maximization convergence curve.
 
   Returns:
     A list of numbers where i-th (zero-index) element is the smallest "j" such
     that baseline_curve[i] <= compared_curve[j]
   """
   convergence_curve = []
-  t1 = 0
-  for t0 in range(len(baseline_curve)):
-    while t1 < len(compared_curve) and compared_curve[t1] < baseline_curve[t0]:
-      t1 += 1
-    convergence_curve.append(float('inf') if t1 >= len(compared_curve) else t1)
+  for value in baseline_curve:
+    j = bisect.bisect_left(compared_curve, value)
+    convergence_curve.append(j if j != len(compared_curve) else float('inf'))
   return convergence_curve
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/convergence_curve_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,51 +33,52 @@
         trial.complete(
             pyvizier.Measurement(metrics={'': pyvizier.Metric(value=v)})))
   return trials
 
 
 class ConvergenceCurveTest(absltest.TestCase):
 
-  def test_align_xs_on_different_lengths(self):
+  def test_align_xs_merge_ys_on_different_lengths(self):
     c1 = convergence.ConvergenceCurve(
         xs=np.array([1, 2, 3]),
         ys=np.array([[2, 1, 1]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     c2 = convergence.ConvergenceCurve(
         xs=np.array([1]),
         ys=np.array([[3]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
-    aligned = convergence.ConvergenceCurve.align_xs([c1, c2])
+    aligned = convergence.ConvergenceCurve.align_xs([c1, c2])[0]
 
     np.testing.assert_array_equal(aligned.xs, [1, 2, 3])
     np.testing.assert_array_equal(aligned.ys,
                                   np.array([[2, 1, 1], [3, np.nan, np.nan]]))
 
-  def test_align_xs_on_distinct_xvalues(self):
+  def test_align_xs_merge_ys_on_distinct_xvalues(self):
     c1 = convergence.ConvergenceCurve(
         xs=np.array([1, 3, 4]),
         ys=np.array([[2, 1, 1]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     c2 = convergence.ConvergenceCurve(
         xs=np.array([2]),
         ys=np.array([[3]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
-    aligned = convergence.ConvergenceCurve.align_xs([c1, c2])
+    aligned = convergence.ConvergenceCurve.align_xs([c1, c2])[0]
 
     np.testing.assert_array_equal(aligned.xs.shape, (3,))
     np.testing.assert_array_equal(aligned.ys,
                                   np.array([[2, 1.25, 1], [3, np.nan, np.nan]]))
 
-  def test_align_xs_with_interpolation(self):
+  def test_align_xs_merge_ys_with_interpolation(self):
     c1 = convergence.ConvergenceCurve(
         xs=np.array([1, 2, 3, 4, 5]),
         ys=np.array([[2, 2, 1, 0.5, 0.5], [1, 1, 1, 1, 1]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
-    aligned = convergence.ConvergenceCurve.align_xs([c1],
-                                                    interpolate_repeats=True)
+    aligned = convergence.ConvergenceCurve.align_xs(
+        [c1], interpolate_repeats=True
+    )[0]
 
     np.testing.assert_array_equal(aligned.xs, np.array([1, 2, 3, 4, 5]))
     np.testing.assert_array_equal(
         aligned.ys, np.array([[2, 1.5, 1.0, 0.5, 0.5], [1, 1, 1, 1, 1]]))
 
   def test_extrapolate_ys_with_steps(self):
     c1 = convergence.ConvergenceCurve(
@@ -88,26 +89,53 @@
     extra_c1 = convergence.ConvergenceCurve.extrapolate_ys(c1, steps=2)
 
     np.testing.assert_array_equal(extra_c1.xs.shape, (6,))
     np.testing.assert_array_equal(
         extra_c1.ys,
         np.array([[2, 1.5, 1.0, 0.5, 0.0, -0.5], [1, 1, 1, 1, 1, 1]]))
 
-  def test_align_xs_on_increasing_and_dicreasing_fails(self):
+  def test_align_xs_merge_ys_on_increasing_and_dicreasing_fails(self):
     c1 = convergence.ConvergenceCurve(
         xs=np.array([1, 3, 4]),
         ys=np.array([[2, 3, 3]]),
         trend=convergence.ConvergenceCurve.YTrend.INCREASING,
     )
     c2 = convergence.ConvergenceCurve(
         xs=np.array([2]),
         ys=np.array([[3]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     with self.assertRaisesRegex(ValueError, 'increasing'):
-      convergence.ConvergenceCurve.align_xs([c1, c2])
+      # pylint: disable=[expression-not-assigned]
+      convergence.ConvergenceCurve.align_xs([c1, c2])[0]
+
+  def test_align_xs_keep_ys(self):
+    c1 = convergence.ConvergenceCurve(
+        xs=np.array([1, 3, 4]),
+        ys=np.array([[2, 1, 1], [8, 3, 1]]),
+        trend=convergence.ConvergenceCurve.YTrend.DECREASING,
+    )
+    c2 = convergence.ConvergenceCurve(
+        xs=np.array([2]),
+        ys=np.array([[3]]),
+        trend=convergence.ConvergenceCurve.YTrend.DECREASING,
+    )
+
+    aligned1, aligned2 = convergence.ConvergenceCurve.align_xs(
+        [c1, c2], keep_curves_separate=True
+    )
+
+    np.testing.assert_array_equal(aligned1.xs, np.array([1.0, 2.5, 4.0]))
+    np.testing.assert_array_equal(aligned2.xs, np.array([1.0, 2.5, 4.0]))
+
+    np.testing.assert_array_equal(
+        aligned1.ys, np.array([[2.0, 1.25, 1.0], [8.0, 4.25, 1.0]])
+    )
+    np.testing.assert_array_equal(
+        aligned2.ys, np.array([[3.0, np.nan, np.nan]])
+    )
 
 
 class ConvergenceCurveConverterTest(parameterized.TestCase):
 
   @parameterized.named_parameters(
       ('maximize', pyvizier.ObjectiveMetricGoal.MAXIMIZE, [[2, 2, 3]]),
       ('minimize', pyvizier.ObjectiveMetricGoal.MINIMIZE, [[2, 1, 1]]))
@@ -162,106 +190,228 @@
     )
 
     curve = generator.convert(pytrials)
     np.testing.assert_array_equal(curve.xs, [1, 2, 3])
     np.testing.assert_array_almost_equal(curve.ys, [[0.0, 3.0, 8.0]], decimal=1)
 
 
-class ConvergenceComparatorTest(absltest.TestCase):
+class LogEfficiencyConvergenceComparatorTest(absltest.TestCase):
 
   def setUp(self):
-    super(ConvergenceComparatorTest, self).setUp()
+    super(LogEfficiencyConvergenceComparatorTest, self).setUp()
     xs = np.array(range(0, 20))
     xs_t = xs.reshape(1, len(xs))
     self._baseline_curve = convergence.ConvergenceCurve(
         xs=xs,
         ys=np.exp(np.array([-0.9, -1.0, -1.1]).reshape(3, 1) * xs_t),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
-    self._baseline = convergence.ConvergenceCurveComparator(
-        self._baseline_curve)
 
     self._worse_curves = convergence.ConvergenceCurve(
         xs=xs,
         ys=np.exp(-0.5 * xs_t),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     self._better_curves = convergence.ConvergenceCurve(
         xs=xs,
         ys=np.exp(np.array([-1.5, -1.8, -2.0]).reshape(3, 1) * xs_t),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
 
-  def testGetRelativeEfficiencyCurve(self):
+  def test_get_relative_efficiency_curve(self):
     baseline_length = len(self._baseline_curve.xs)
-    rel_effiency = self._baseline.log_efficiency_curve(self._better_curves)
-    higher_quantile = self._baseline.log_efficiency_curve(
-        self._better_curves, compared_quantile=0.9)
+    rel_effiency = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=self._baseline_curve, compared_curve=self._better_curves
+    ).log_efficiency_curve()
+    higher_quantile = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=self._baseline_curve,
+        compared_curve=self._better_curves,
+        compared_quantile=0.9,
+    ).log_efficiency_curve()
 
     self.assertEqual(rel_effiency.ys.shape, (1, baseline_length))
     self.assertEqual(higher_quantile.ys.shape, (1, baseline_length))
     # Better curves should have positive efficiency.
     self.assertTrue((rel_effiency.ys >= 0.0).all())
     # Higher quantile means better efficiency which means more positive scores.
     self.assertTrue((higher_quantile.ys >= rel_effiency.ys).all())
 
-  def testGetRelativeEfficiencyFlat(self):
+  def test_get_relative_efficiency_flat(self):
     flat_curve = convergence.ConvergenceCurve(
         xs=np.array(range(0, 20)),
         ys=np.array([4.0, 3.0, 2.0] + [1.5] * 17).reshape(1, 20),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
-    comparator = convergence.ConvergenceCurveComparator(flat_curve)
-    self_eff = comparator.log_efficiency_curve(flat_curve)
+    self_eff = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=flat_curve, compared_curve=flat_curve
+    ).log_efficiency_curve()
     # Relative efficiency of a curve on itself is close to 0.
     self.assertAlmostEqual(np.linalg.norm(self_eff.ys), 0.0, delta=0.1)
 
-  def testGetRelativeEfficiencyShortCurve(self):
+  def test_get_relative_efficiency_short_curve(self):
     baseline_length = len(self._baseline_curve.xs)
     short_length = round(baseline_length / 2)
     short_curve = convergence.ConvergenceCurve(
         xs=self._baseline_curve.xs[:short_length],
         ys=self._baseline_curve.ys[:, :short_length],
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
-    short_efficiency = self._baseline.log_efficiency_curve(short_curve)
+    short_efficiency = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=self._baseline_curve, compared_curve=short_curve
+    ).log_efficiency_curve()
     self.assertEqual(short_efficiency.ys.shape, (1, baseline_length))
     self.assertEqual(float(short_efficiency.ys[:, -1]), -float('inf'))
 
-  def testGetEfficiencyScore(self):
+  def test_get_efficiency_score(self):
     # Higher compared quantile should increase score. Higher baseline
     # quantile should decrease score.
-    median_score = self._baseline.get_log_efficiency_score(self._better_curves)
+    median_score = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=self._baseline_curve, compared_curve=self._better_curves
+    ).score()
     self.assertGreater(
-        self._baseline.get_log_efficiency_score(
-            self._better_curves, compared_quantile=0.9), median_score)
+        convergence.LogEfficiencyConvergenceCurveComparator(
+            baseline_curve=self._baseline_curve,
+            compared_curve=self._better_curves,
+            compared_quantile=0.9,
+        ).score(),
+        median_score,
+    )
     self.assertLess(
-        self._baseline.get_log_efficiency_score(
-            self._better_curves, baseline_quantile=0.9), median_score)
+        convergence.LogEfficiencyConvergenceCurveComparator(
+            baseline_curve=self._baseline_curve,
+            compared_curve=self._better_curves,
+            baseline_quantile=0.9,
+        ).score(),
+        median_score,
+    )
 
-  def testEffiencyScoreSymmetry(self):
-    base_score = self._baseline.get_log_efficiency_score(self._better_curves)
-    reversed_score = convergence.ConvergenceCurveComparator(
-        self._better_curves).get_log_efficiency_score(self._baseline_curve)
+  def test_effiency_score_symmetry(self):
+    base_score = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=self._baseline_curve, compared_curve=self._better_curves
+    ).score()
+    reversed_score = convergence.LogEfficiencyConvergenceCurveComparator(
+        baseline_curve=self._better_curves, compared_curve=self._baseline_curve
+    ).score()
     self.assertAlmostEqual(base_score, -reversed_score, delta=0.01)
 
-  def testEfficiencyScoreValue(self):
+  def test_efficiency_score_value(self):
     xs = self._baseline_curve.xs
     xs_t = xs.reshape(1, len(xs))
 
     worse_curves = convergence.ConvergenceCurve(
         xs=xs,
         ys=np.exp(-0.5 * xs_t),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     better_curves = convergence.ConvergenceCurve(
         xs=xs,
         ys=np.exp(np.array([-1.5, -1.8, -2.0]).reshape(3, 1) * xs_t),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     # Efficiency score for exponential curves can be approximated.
+
     self.assertGreater(
-        self._baseline.get_log_efficiency_score(better_curves), 0.4)
-    self.assertLess(self._baseline.get_log_efficiency_score(worse_curves), -0.4)
+        convergence.LogEfficiencyConvergenceCurveComparator(
+            baseline_curve=self._baseline_curve, compared_curve=better_curves
+        ).score(),
+        0.4,
+    )
+    self.assertLess(
+        convergence.LogEfficiencyConvergenceCurveComparator(
+            baseline_curve=self._baseline_curve, compared_curve=worse_curves
+        ).score(),
+        -0.4,
+    )
 
-  def testComparatorFailure(self):
+  def test_comparator_failure(self):
     unknown_curve = convergence.ConvergenceCurve(
         xs=self._baseline_curve.xs, ys=self._baseline_curve.ys)
     with self.assertRaisesRegex(ValueError, 'increasing or decreasing'):
-      convergence.ConvergenceCurveComparator(unknown_curve)
+      convergence.LogEfficiencyConvergenceCurveComparator(
+          baseline_curve=unknown_curve, compared_curve=self._baseline_curve
+      )
+
+
+class SimpleConvergenceComparatorTest(parameterized.TestCase):
+
+  @parameterized.parameters(
+      {
+          'ys1': np.array([[11, 12, 20, 50, 100, 300]]),
+          'ys2': np.array([[1, 2, 10]]),
+          'cutoff': None,
+          'res': 0.0,
+      },
+      {
+          'ys1': np.array([[1, 2, 10]]),
+          'ys2': np.array([[11, 12, 20, 50, 100, 300]]),
+          'cutoff': None,
+          'res': 1.0,
+      },
+      {
+          'ys1': np.array([[1, 4, 8, 10]]),
+          'ys2': np.array([[2, 5, 6, 8]]),
+          'cutoff': None,
+          'res': 0.5,
+      },
+      {
+          'ys1': np.array([[1, 4, 8, 10, 12]]),
+          'ys2': np.array([[2, 5, 6, 8, 10]]),
+          'cutoff': 1,
+          'res': 0.25,
+      },
+      {
+          'ys1': np.array([[1, 4, 8, 10, 12]]),
+          'ys2': np.array([[2, 5, 6, 8, 10]]),
+          'cutoff': 3,
+          'res': 0.0,
+      },
+      {
+          'ys1': np.array([[2, 5, 6, 8, 10]]),
+          'ys2': np.array([[1, 4, 8, 10, 12]]),
+          'cutoff': 3,
+          'res': 1.0,
+      },
+  )
+  def test_score_one_curve_above_other(self, ys1, ys2, res, cutoff):
+    xs1 = np.arange(ys1.shape[1])
+    xs2 = np.arange(ys2.shape[1])
+    curve1 = convergence.ConvergenceCurve(
+        xs=xs1, ys=ys1, trend=convergence.ConvergenceCurve.YTrend.INCREASING
+    )
+    curve2 = convergence.ConvergenceCurve(
+        xs=xs2, ys=ys2, trend=convergence.ConvergenceCurve.YTrend.INCREASING
+    )
+    comparator = convergence.SimpleConvergenceCurveComparator(
+        curve1, curve2, xs_cutoff=cutoff
+    )
+    self.assertEqual(comparator.score(), res)
+
+
+class PercentageBetterConvergenceComparatorTest(parameterized.TestCase):
+
+  @parameterized.parameters(
+      {
+          'ys1': np.array([[1, 2, 3, 4], [1, 2, 3, 4]]),
+          'ys2': np.array([[-1, 20, 30, 70]]),
+          'res': 0.5,
+      },
+      {
+          'ys1': np.array([[1, 2, 3, 4]]),
+          'ys2': np.array([[10, 20, 30, 70]]),
+          'res': 1.0,
+      },
+      {
+          'ys1': np.array([[10, 20, 30, 70]]),
+          'ys2': np.array([[1, 2, 3, 4]]),
+          'res': -1.0,
+      },
+  )
+  def test_score(self, ys1, ys2, res):
+    xs1 = np.arange(ys1.shape[1])
+    xs2 = np.arange(ys2.shape[1])
+    curve1 = convergence.ConvergenceCurve(
+        xs=xs1, ys=ys1, trend=convergence.ConvergenceCurve.YTrend.INCREASING
+    )
+    curve2 = convergence.ConvergenceCurve(
+        xs=xs2, ys=ys2, trend=convergence.ConvergenceCurve.YTrend.INCREASING
+    )
+    comparator = convergence.PercentageBetterConvergenceCurveComparator(
+        curve1, curve2
+    )
+    self.assertEqual(comparator.score(), res)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/simple_regret_score.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/state_analyzer.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/state_analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,8 +64,8 @@
             f'States must have same problem {problem_statement}'
             f' and {state.experimenter.problem_statement()}'
         )
 
       state_trials = state.algorithm.supporter.GetTrials()
       curve = converter.convert(state_trials)
       curves.append(curve)
-    return convergence_curve.ConvergenceCurve.align_xs(curves)
+    return convergence_curve.ConvergenceCurve.align_xs(curves)[0]
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/state_analyzer_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/analyzers/state_analyzer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo/common.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,32 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Experimenter that discretizes the parameters of search space."""
 
 import copy
-from typing import Mapping, Sequence
+from typing import Mapping, Sequence, Union
 
 import numpy as np
 from vizier import pyvizier
 from vizier._src.benchmarks.experimenters import experimenter
 from vizier.pyvizier import converters
 
 
 class DiscretizingExperimenter(experimenter.Experimenter):
   """DiscretizingExperimenter discretizes the parameters of search space."""
 
-  def __init__(self,
-               exptr: experimenter.Experimenter,
-               discretization: Mapping[str, pyvizier.MonotypeParameterSequence],
-               *,
-               allow_oov: bool = False):
+  def __init__(
+      self,
+      exptr: experimenter.Experimenter,
+      discretization: Mapping[str, pyvizier.MonotypeParameterSequence],
+      *,
+      allow_oov: bool = False,
+  ):
     """DiscretizingExperimenter discretizes continuous parameters.
 
     Currently only supports flat double search spaces. Note that the discretized
     parameters must fit within the bounds of the continuous parameters. This
     also supports CATEGORICAL parameters but feasible categories must be
     convertible to floats.
 
@@ -52,34 +54,39 @@
     """
     self._exptr = exptr
     self._discretization = discretization
     self._allow_oov = allow_oov
     exptr_problem_statement = exptr.problem_statement()
 
     if exptr_problem_statement.search_space.is_conditional:
-      raise ValueError('Search space should not have conditional'
-                       f' parameters  {exptr_problem_statement}')
+      raise ValueError(
+          'Search space should not have conditional'
+          f' parameters  {exptr_problem_statement}'
+      )
 
     search_params = exptr_problem_statement.search_space.parameters
     param_names = [param.name for param in search_params]
     for name in discretization.keys():
       if name not in param_names:
-        raise ValueError(f'Parameter {name} not in search space'
-                         f' parameters for discretization: {search_params}')
+        raise ValueError(
+            f'Parameter {name} not in search space'
+            f' parameters for discretization: {search_params}'
+        )
 
     self._problem_statement = copy.deepcopy(exptr_problem_statement)
     self._problem_statement.search_space = pyvizier.SearchSpace()
     for parameter in search_params:
       if parameter.name not in discretization:
         self._problem_statement.search_space.add(parameter)
         continue
 
       if parameter.type != pyvizier.ParameterType.DOUBLE:
         raise ValueError(
-            f'Non-double parameters cannot be discretized {parameter}')
+            f'Non-double parameters cannot be discretized {parameter}'
+        )
       # Discretize the parameters.
       min_value, max_value = parameter.bounds
       for value in discretization[parameter.name]:
         float_value = float(value)
         if float_value > max_value or float_value < min_value:
           raise ValueError(f'Discretized values are not in bounds {parameter}')
       self._problem_statement.search_space.add(
@@ -102,15 +109,16 @@
       old_parameters.append(suggestion.parameters)
       new_parameter_dict = {}
       for name, param in suggestion.parameters.items():
         if name in self._discretization:
           if self._allow_oov:
             if param.value not in self._discretization[name]:
               raise ValueError(
-                  f'Parameter {param} not in {self._discretization[name]}')
+                  f'Parameter {param} not in {self._discretization[name]}'
+              )
           new_parameter_dict[name] = param.as_float
         else:
           new_parameter_dict[name] = param
       suggestion.parameters = pyvizier.ParameterDict(new_parameter_dict)
     self._exptr.evaluate(suggestions)
     for old_param, suggestion in zip(old_parameters, suggestions):
       suggestion.parameters = old_param
@@ -119,44 +127,57 @@
     return f'DiscretizingExperimenter({self._discretization}) on {self._exptr}'
 
   @classmethod
   def create_with_grid(
       cls,
       exptr: experimenter.Experimenter,
       grid_discretization_count: Mapping[str, int],
-      convert_to_str: bool = False,
+      convert_to_str: Union[bool, Mapping[str, bool]] = False,
   ) -> 'DiscretizingExperimenter':
     """Creates Experimenter with continuous parameters discretized via grid.
 
     Note that the grid is generated according to ModelInputConverter scaling.
 
     Args:
       exptr: Experimenter with continuous parameters to be discretized.
       grid_discretization_count: Mapping from parameter names to number of
         feasible values to generate on grid. Parameter names should be a subset
         of all parameter names in the search space of the exptr.
-      convert_to_str: If true, convert values to categories/strings. Otherwise,
-        the values are discrete numbers.
+      convert_to_str: For each parameter, if true, convert values to
+        categories/strings. Otherwise, the values are discrete numbers. Can also
+        be pure boolean, for all parameters.
 
     Returns:
       DiscreteExperimenter.
 
     Raises:
       ValueError: Invalid keys, discretizing non-double/singleton parameters.
     """
+    if isinstance(convert_to_str, bool):
+      convert_to_str = {
+          k: convert_to_str for k in grid_discretization_count.keys()
+      }
+
+    if set(grid_discretization_count.keys()) != set(convert_to_str.keys()):
+      raise ValueError(
+          f'Grid discretization keys {grid_discretization_count.keys()} must'
+          f' match convert_to_str keys {convert_to_str.keys()}'
+      )
+
     # Create grid for each parameter config.
     discretization = {}
     problem_statement = copy.deepcopy(exptr.problem_statement())
     if not set(grid_discretization_count.keys()).issubset(
         set(problem_statement.search_space.parameter_names)
     ):
       raise ValueError(
           f'Grid discretization keys {grid_discretization_count.keys()}'
           f' are not in search space {problem_statement.search_space}'
       )
+
     for param in problem_statement.search_space.parameters:
       if param.name in grid_discretization_count:
         if param.type != pyvizier.ParameterType.DOUBLE:
           raise ValueError(
               f'Non-double parameters cannot be grid-discretized {param}'
           )
 
@@ -166,13 +187,13 @@
 
         if min_value == max_value:
           raise ValueError(f'Cannot discretize singleton parameter {param}')
         converter = converters.DefaultModelInputConverter(param, scale=True)
         grid_scalars = np.linspace(0.0, 1.0, num=num_feasible_points)
         grid_values = converter.to_parameter_values(grid_scalars)
 
-        if convert_to_str:
+        if convert_to_str[param.name]:
           discretization[param.name] = [point.as_str for point in grid_values]
         else:
           discretization[param.name] = [point.as_float for point in grid_values]
 
     return cls(exptr, discretization)
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/experimenter_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,27 +33,33 @@
 from vizier.interfaces import serializable
 from vizier.utils import json_utils
 
 BBOB_FACTORY_KEY = 'bbob_factory'
 SINGLE_OBJECTIVE_FACTORY_KEY = 'single_objective_factory'
 
 
-class ExperimenterFactory(serializable.Serializable):
+class ExperimenterFactory(abc.ABC):
   """Abstraction for creating Experimenters."""
 
   @abc.abstractmethod
   def __call__(
       self, *, seed: Optional[int] = None
   ) -> experimenter.Experimenter:
     """Creates the Experimenter."""
     pass
 
 
+class SerializableExperimenterFactory(
+    ExperimenterFactory, serializable.Serializable
+):
+  """Abstraction for experimenter factories with dump/recover methods."""
+
+
 @attr.define
-class BBOBExperimenterFactory(ExperimenterFactory):
+class BBOBExperimenterFactory(SerializableExperimenterFactory):
   """Factory for a BBOB function."""
 
   # Should be a BBOB function name in bbob.py (name should match exactly).
   name: str = attr.field(default='', validator=attr.validators.instance_of(str))
   dim: int = attr.field(
       default=1,
       validator=[attr.validators.instance_of(int), attr.validators.gt(0)],
@@ -63,33 +69,34 @@
       self, seed: Optional[int] = None
   ) -> numpy_experimenter.NumpyExperimenter:
     del seed
     bbob_function = getattr(bbob, self.name, None)
     if bbob_function is None:
       raise ValueError(f'{self.name} is not a valid BBOB function in bbob.py')
     return numpy_experimenter.NumpyExperimenter(
-        bbob_function, bbob.DefaultBBOBProblemStatement(self.dim))
+        bbob_function, bbob.DefaultBBOBProblemStatement(self.dim)
+    )
 
   def dump(self) -> vz.Metadata:
     metadata = vz.Metadata()
     metadata_dict = {'name': self.name, 'dim': self.dim}
     metadata[BBOB_FACTORY_KEY] = json.dumps(metadata_dict)
     return metadata
 
   @classmethod
   def recover(cls, metadata: vz.Metadata) -> 'BBOBExperimenterFactory':
     metadata_dict = json.loads(metadata[BBOB_FACTORY_KEY])
     return cls(**metadata_dict)
 
 
 @attr.define
-class SingleObjectiveExperimenterFactory(ExperimenterFactory):
+class SingleObjectiveExperimenterFactory(SerializableExperimenterFactory):
   """Factory for a single objective Experimenter."""
 
-  base_factory: ExperimenterFactory = attr.field()
+  base_factory: SerializableExperimenterFactory = attr.field()
   # An array of doubles that is broadcastable to dim of search space.
   shift: Optional[np.ndarray] = attr.field(default=None)
   # Should be one of the noise types in noisy_experimenter.py
   noise_type: Optional[str] = attr.field(default=None)
   # Number of normalization samples. If zero, no normalization is done.
   num_normalization_samples: int = attr.field(default=0)
   # Dictionary of parameter indices to discretize in a grid.
@@ -105,25 +112,26 @@
   categorical_dict: dict[int, int] = attr.field(default=attr.Factory(dict))
 
   def __call__(self, seed: Optional[int] = None) -> experimenter.Experimenter:
     """Creates the SingleObjective Experimenter."""
     exptr = self.base_factory()
     if self.shift is not None:
       exptr = shifting_experimenter.ShiftingExperimenter(
-          exptr, shift=self.shift)
+          exptr, shift=self.shift
+      )
     if self.num_normalization_samples:
       exptr = normalizing_experimenter.NormalizingExperimenter(
           exptr, num_normalization_samples=self.num_normalization_samples
       )
 
     # Discretization and categorization.
     if self.discrete_dict.keys() & self.categorical_dict.keys():
       raise ValueError(
-          f'{self.discrete_dict} discretizing indicies overlap with '
-          f'{self.categorical_dict} categorical indicies'
+          f'{self.discrete_dict} discretizing indices overlap with '
+          f'{self.categorical_dict} categorical indices'
       )
 
     pcs = list(exptr.problem_statement().search_space.parameters)
     if self.discrete_dict:
       discretization = {
           pcs[idx].name: points for idx, points in self.discrete_dict.items()
       }
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob/handler.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob/handler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/noisy_experimenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,17 @@
   Returns:
     Callable that returns the noisy version of the input.
 
   Raises:
     ValueError: if noise is not supported.
   """
   rng = np.random.default_rng(seed or 0)
-  if noise == 'MODERATE_GAUSSIAN':
+  if noise == 'NO_NOISE':
+    noise_fn = lambda v: v
+  elif noise == 'MODERATE_GAUSSIAN':
     noise_fn = lambda v: v * rng.lognormal(0, 0.01)
   elif noise == 'SEVERE_GAUSSIAN':
     noise_fn = lambda v: v * rng.lognormal(0, 0.1)
   elif noise == 'MODERATE_UNIFORM':
     noise_fn = functools.partial(
         _uniform_noise,
         rng=rng,
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,25 +65,26 @@
     noised_value = t.final_measurement.metrics[metric_name].value
     self.assertEqual(unnoised_value - 1, noised_value)
     self.assertEqual(
         unnoised_value,
         t.final_measurement.metrics[metric_name + '_before_noise'].value)
 
   @parameterized.named_parameters(
+      ('NO_NOISE', 'NO_NOISE', 1e-5),
       ('SEVERE_ADDITIVE_GAUSSIAN', 'SEVERE_ADDITIVE_GAUSSIAN', 3),
       ('MODERATE_ADDITIVE_GAUSSIAN', 'MODERATE_ADDITIVE_GAUSSIAN', 0.3),
       ('LIGHT_ADDITIVE_GAUSSIAN', 'LIGHT_ADDITIVE_GAUSSIAN', 0.03),
       ('MODERATE_GAUSSIAN', 'MODERATE_GAUSSIAN', 0.05),
       ('SEVERE_GAUSSIAN', 'SEVERE_GAUSSIAN', 0.5),
       ('MODERATE_UNIFORM', 'MODERATE_UNIFORM', 0.2),
       ('SEVERE_UNIFORM', 'SEVERE_UNIFORM', 3.5),
       ('MODERATE_SELDOM_CAUCHY', 'MODERATE_SELDOM_CAUCHY', 10.3),
       ('SEVERE_SELDOM_CAUCHY', 'SEVERE_SELDOM_CAUCHY', 100.3),
   )
-  def testGaussianNoiseApply(self, noise, delta):
+  def testGaussianNoiseApply(self, noise: str, delta: float):
     dim = 2
     exptr = numpy_experimenter.NumpyExperimenter(
         bbob.Sphere, bbob.DefaultBBOBProblemStatement(dim))
     noisy_exptr = noisy_experimenter.NoisyExperimenter.from_type(
         exptr=exptr, noise_type=noise
     )
 
@@ -99,15 +100,15 @@
     noisy_exptr.evaluate([t])
     noised_value1 = t.final_measurement.metrics[metric_name].value
 
     noisy_exptr.evaluate([t])
     noised_value2 = t.final_measurement.metrics[metric_name].value
 
     # Seldom noise is only injected sporadically.
-    if 'SELDOM' not in noise:
+    if 'SELDOM' not in noise and noise != 'NO_NOISE':
       self.assertNotEqual(noised_value1, noised_value2)
     self.assertAlmostEqual(noised_value1, unnoised_value, delta=delta)
     self.assertAlmostEqual(noised_value2, unnoised_value, delta=delta)
 
   def testSeedDeterminism(self):
     dim = 2
     seed = 7
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/numpy_experimenter.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,47 +75,42 @@
       )
     if problem_statement.search_space.is_conditional:
       raise ValueError(f'Statement should be flat {problem_statement}')
     for parameter in problem_statement.search_space.parameters:
       if not parameter.type.is_numeric():
         raise ValueError(f'Non-numeric parameters {parameter}')
 
-    self._metric_name = (
-        problem_statement.metric_information.of_type(
-            pyvizier.MetricType.OBJECTIVE
-        )
-        .item()
-        .name
+    objective_metrics = problem_statement.metric_information.of_type(
+        pyvizier.MetricType.OBJECTIVE
     )
+    self._metric_name = objective_metrics.item().name
+
     self._problem_statement = copy.deepcopy(problem_statement)
     self._converter = converters.TrialToArrayConverter.from_study_config(
         study_config=self._problem_statement,
         scale=False,
         flip_sign_for_minimization_metrics=False,
     )
 
   def problem_statement(self) -> pyvizier.ProblemStatement:
     return copy.deepcopy(self._problem_statement)
 
   def evaluate(self, suggestions: Sequence[pyvizier.Trial]):
     # Features has shape (num_trials, num_features).
     features = self._converter.to_features(suggestions)
     for idx, suggestion in enumerate(suggestions):
-      if len(features[idx]) != self._dimension:
-        raise ValueError(
-            f'Features {features[idx]} should have length {self._dimension}'
-        )
       val = self.impl(features[idx])
       if math.isfinite(val):
         suggestion.complete(
             pyvizier.Measurement(metrics={self._metric_name: val})
         )
       else:
+        self.problem_statement().search_space.assert_contains(
+            suggestions[idx].parameters
+        )
         suggestion.complete(
             pyvizier.Measurement(),
             infeasibility_reason='Objective value is not finite: %f' % val,
         )
-      if not suggestion.is_completed:
-        raise RuntimeError(f'Trial {suggestion} not completed')
 
   def __repr__(self) -> str:
     return f'NumpyExperimenter {{name: {self._impl_name}}}'
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,16 +72,26 @@
     t1 = pyvizier.Trial(parameters={
         param.name: float(index) for index, param in enumerate(parameters)
     })
     t2 = pyvizier.Trial(parameters={
         param.name: -float(index) for index, param in enumerate(parameters)
     })
 
-    completed_trials = [t1, t2]
-    exptr.evaluate(completed_trials)
-    for trial in completed_trials:
+    trials = [t1, t2]
+    exptr.evaluate(trials)
+    for trial in trials:
       self.assertEmpty(trial.final_measurement.metrics)
       self.assertTrue(trial.infeasible)
 
+  def testNotInSearchSpace(self):
+    exptr = numpy_experimenter.NumpyExperimenter(
+        impl=lambda x: x,
+        problem_statement=bbob.DefaultBBOBProblemStatement(1),
+    )
+
+    t1 = pyvizier.Trial(parameters={'yyyy': 0.0})
+    with self.assertRaises(ValueError):
+      exptr.evaluate([t1])
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/shifting_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sparse_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/synthetic/bbob.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/experimenters/synthetic/bbob.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_runner_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state_test.py` & `google-vizier-0.1.6/vizier/_src/benchmarks/runners/benchmark_state_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/jax/models/__init__.py` & `google-vizier-0.1.6/vizier/_src/jax/models/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model.py` & `google-vizier-0.1.6/vizier/_src/jax/models/gaussian_process_model.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model_test.py` & `google-vizier-0.1.6/vizier/_src/jax/models/gaussian_process_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model.py` & `google-vizier-0.1.6/vizier/_src/jax/models/hebo_gp_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,57 +19,40 @@
 
 Faithful reimplementation of HEBO model based off of:
 Paper: https://arxiv.org/abs/2012.03826
 Repo: https://github.com/huawei-noah/HEBO.
 """
 
 from typing import Generator, Optional
-import attr
+from flax import struct
 import jax
 from jax import numpy as jnp
-from jax.config import config
 from tensorflow_probability.substrates import jax as tfp
 from vizier._src.jax import stochastic_process_model as sp
 from vizier._src.jax import types
-from vizier._src.jax.optimizers import optimizers
-
-config.update('jax_enable_x64', True)
 
 tfd = tfp.distributions
 tfb = tfp.bijectors
 tfpk = tfp.math.psd_kernels
 
 
-@attr.define
+@struct.dataclass
 class VizierHeboGaussianProcess(
     sp.ModelCoroutine[types.Array, tfd.GaussianProcess]
 ):
   """Hebo Gaussian process model."""
 
   @classmethod
-  def model_and_loss_fn(
+  def build_model(
       cls,
       features: types.Array,
-      labels: types.Array,
-  ) -> tuple[sp.StochasticProcessModel, optimizers.LossFunction]:
+  ) -> sp.StochasticProcessModel:
     """Returns the model and loss function."""
     gp_coroutine = VizierHeboGaussianProcess()
-    model = sp.StochasticProcessModel(gp_coroutine)
-
-    # Define the ARD loss function.
-    def loss_fn(params):
-      gp, mutables = model.apply({'params': params},
-                                 features,
-                                 mutable=['losses', 'predictive'])
-      loss = -gp.log_prob(labels) + jax.tree_util.tree_reduce(
-          jnp.add, mutables['losses']
-      )
-      return loss, dict()
-
-    return model, loss_fn
+    return sp.StochasticProcessModel(gp_coroutine)
 
   def __call__(
       self, inputs: Optional[types.Array] = None
   ) -> Generator[sp.ModelParameter, jax.Array, tfd.GaussianProcess]:
     """Creates a generator.
 
     Args:
```

### Comparing `google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model_test.py` & `google-vizier-0.1.6/vizier/_src/jax/models/hebo_gp_model_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for hebo_gp_model."""
 
+import functools
+
 from absl import logging
 import jax
 from jax import numpy as jnp
+from jax.config import config
 import optax
+from vizier._src.jax import gp_bandit_utils
 from vizier._src.jax import stochastic_process_model as sp
+from vizier._src.jax import types
 from vizier._src.jax.models import hebo_gp_model
 from vizier._src.jax.optimizers import optimizers
 
 from absl.testing import absltest
 
+
 VizierHeboGaussianProcess = hebo_gp_model.VizierHeboGaussianProcess
 
 
 class VizierHeboGaussianProcessTest(absltest.TestCase):
 
   def setUp(self):
     super(VizierHeboGaussianProcessTest, self).setUp()
@@ -57,31 +63,42 @@
     self.y_obs = jnp.array([
         0.55552674, -0.29054829, -0.04703586, 0.0217839, 0.15445438, 0.46654119,
         0.12255823, -0.19540335, -0.11772564, -0.44447326
     ],
                            dtype=jnp.float64)
 
   def test_log_prob_and_loss(self):
-    model, loss_fn = VizierHeboGaussianProcess.model_and_loss_fn(
-        features=self.x_obs, labels=self.y_obs)
+    model = VizierHeboGaussianProcess.build_model(features=self.x_obs)
     setup = lambda rng: model.init(rng, self.x_obs)['params']
     key = jax.random.PRNGKey(2)
     init_params = setup(key)
     optimize = optimizers.OptaxTrainWithRandomRestarts(
         optax.adam(5e-3), epochs=500, verbose=True, random_restarts=20
     )
     constraints = sp.get_constraints(model)
+    data = types.StochasticProcessModelData(
+        features=self.x_obs, labels=self.y_obs
+    )
+    loss_fn = functools.partial(
+        jax.jit(
+            gp_bandit_utils.stochastic_process_model_loss_fn,
+            static_argnames=('model', 'normalize'),
+        ),
+        model=model,
+        data=data,
+    )
     params, metrics = optimize(setup, loss_fn, key, constraints=constraints)
 
     init_gp = model.apply({'params': init_params}, self.x_obs)
     gp = model.apply({'params': params}, self.x_obs)
     self.assertGreater(gp.log_prob(self.y_obs), init_gp.log_prob(self.y_obs))
     losses_every_50 = metrics['loss'][::50]
     self.assertTrue((losses_every_50[1:] < losses_every_50[:-1]).all())
 
     logging.info('Optimal parameters: %s', params)
     logging.info('Optimal loss fn: %s', loss_fn(params)[0])
     self.assertLess(loss_fn(params)[0], 0.3)
 
 
 if __name__ == '__main__':
+  config.update('jax_enable_x64', True)
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers.py` & `google-vizier-0.1.6/vizier/_src/jax/optimizers/optimizers.py`

 * *Files 10% similar despite different names*

```diff
@@ -186,14 +186,15 @@
       # Random restarts are implemented via jax.vmap.
       # Note that both setup_all and train_step are vmapped.
       rngs = random.split(rng, self.random_restarts)
       params, opt_state = jax.vmap(_setup_all)(rngs)
       train_step = jax.vmap(_train_step)
     else:
       params, opt_state = _setup_all(rng)
+      train_step = _train_step
 
     logging.info('Initialized parameters. %s',
                  jax.tree_map(lambda x: x.shape, params))
 
     # See https://jax.readthedocs.io/en/latest/faq.html#buffer-donation.
     train_step = jax.jit(train_step, donate_argnums=[0, 1])
     metrics = []
@@ -218,46 +219,54 @@
         jnp.array,
         transposed_metrics,
         is_leaf=lambda x: jax.tree_util.tree_structure(x) == outer_treedef,
     )
 
     final_losses = metrics['loss'][-1]
     logging.info('Final loss: %s', final_losses)
-    # Extract the best only.
-    argsorted = jnp.argsort(final_losses)
-    logging.info('Best loss(es): %s', final_losses[argsorted[: self.best_n]])
-    params = jax.tree_map(lambda x: x[argsorted[: self.best_n]], params)
-    if self.best_n == 1:
-      params = jax.tree_map(functools.partial(jnp.squeeze, axis=0), params)
+    if self.random_restarts > 1:
+      # Extract the best only.
+      argsorted = jnp.argsort(final_losses)
+      logging.info('Best loss(es): %s', final_losses[argsorted[: self.best_n]])
+      params = jax.tree_map(lambda x: x[argsorted[: self.best_n]], params)
+      if self.best_n == 1:
+        params = jax.tree_map(functools.partial(jnp.squeeze, axis=0), params)
     if bijector is not None:
       params = bijector(params)
     return params, metrics
 
 
 @attr.define
 class JaxoptLbfgsB(Optimizer[_Params]):
   """Jaxopt's L-BFGS-B optimizer.
 
-  Jaxopt calls Scipy's L-BFGS-B, which wraps a Fortran implementation.
+  Jaxopt calls the Scipy or Jax implementation of L-BFGS-B.
   L-BFGS-B is a version of L-BFGS that incorporates box constraints on
   parameters.
   https://digital.library.unt.edu/ark:/67531/metadc666315/m2/1/high_res_d/204262.pdf
 
   Attributes:
     num_line_search_steps: Maximum number of line search steps.
     random_restarts: Must be positive; number of random initializations for the
       optimization.
     best_n: Number of best values to return from the initializations; must be
       less than or equal to `random_restarts`.
+     use_scipy: Uses the scipy version of L-BFGS-B. If False, uses the pure JAX
+       L-BFGS-B in Jaxopt, which runs on accelerators.
+     tol: Tolerance for stopping criteria.
+     maxiter: Max number of iterations.
     _speed_test: If True, return speed test results.
   """
 
   num_line_search_steps: int = attr.field(kw_only=True, default=20)
   random_restarts: int = attr.field(kw_only=True, default=4)
   best_n: int = attr.field(kw_only=True, default=1)
+  use_scipy: bool = attr.field(kw_only=True, default=True)
+  tol: float = attr.field(kw_only=True, default=1e-8)
+  maxiter: int = attr.field(kw_only=True, default=50)
   _speed_test: bool = attr.field(kw_only=True, default=False)
 
   def __attrs_post_init__(self):
     if self.random_restarts < self.best_n:
       raise ValueError(
           f'Cannot generate {self.best_n} results from'
           f' {self.random_restarts} restarts'
@@ -298,42 +307,71 @@
 
     if bounds is not None:
       lb = _none_to_inf(bounds[0], -jnp.inf)
       ub = _none_to_inf(bounds[1], jnp.inf)
       bounds = (lb, ub)
 
     loss = lambda p: loss_fn(p)[0]
-    lbfgsb = jaxopt.ScipyBoundedMinimize(
-        fun=loss,
-        method='L-BFGS-B',
-        options={'maxls': self.num_line_search_steps},
-    )
+
+    if self.use_scipy:
+      lbfgsb = jaxopt.ScipyBoundedMinimize(
+          fun=loss,
+          method='L-BFGS-B',
+          maxiter=self.maxiter,
+          options={
+              'gtol': self.tol,
+              'maxls': self.num_line_search_steps,
+          },
+      )
+    else:
+      lbfgsb = jaxopt.LBFGSB(
+          fun=loss,
+          maxls=self.num_line_search_steps,
+          tol=self.tol,
+          maxiter=self.maxiter,
+      )
 
     metrics = {}
     if self._speed_test:
       start_time = time.time()
       _ = lbfgsb.run(init_params=p, bounds=bounds)
-      metrics['compile_time'] = time.time() - start_time
+      metrics['compile+runtime'] = time.time() - start_time
 
+    # TODO: Make sure the loss fn isn't retraced for new instances
+    # of the optimizer.
     train_times = []
     losses = []
     params = []
-    for i, rng in enumerate(jax.random.split(rng, num=self.random_restarts)):
-      with jax.profiler.StepTraceAnnotation('train', step_num=i):
+    if self.use_scipy:
+      logging.info('Using SCIPY L-BFGS-B w/ %d restarts.', self.random_restarts)
+      for rng in jax.random.split(rng, num=self.random_restarts):
         p = setup(rng)
         start_time = time.time()
-        # TODO: Avoid using `run` since it re-JITs unnecessarily.
+
         position, opt_state = lbfgsb.run(init_params=p, bounds=bounds)
         train_times.append(time.time() - start_time)
         losses.append(opt_state.fun_val)
         params.append(position)
-        logging.info('Loss: %s', opt_state.fun_val)
-        logging.info('Last step time: %s', train_times[-1])
+        logging.info(
+            'Loss: %s, last step time: %s', opt_state.fun_val, train_times[-1]
+        )
+
+      all_params = jax.tree_util.tree_map(lambda *x: jnp.stack(x), *params)
+    else:
+      logging.info('Using JAX L-BFGS-B w/ %d restarts.', self.random_restarts)
+      rngs = jax.random.split(rng, num=self.random_restarts)
+      init_params = jax.vmap(setup)(rngs)
+
+      start_time = time.time()
+      all_params, opt_states = jax.lax.map(
+          lambda p: lbfgsb.run(init_params=p, bounds=bounds), init_params
+      )
+      train_times = time.time() - start_time
+      losses = opt_states.value
 
-    all_params = jax.tree_util.tree_map(lambda *x: jnp.stack(x), *params)
     losses = jnp.array(losses)
     argsorted = jnp.argsort(losses)
     logging.info('Best loss(es): %s', losses[argsorted[: self.best_n]])
     optimal_params = jax.tree_util.tree_map(
         lambda p: p[argsorted[: self.best_n]], all_params
     )
     if self.best_n == 1:
```

### Comparing `google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers_test.py` & `google-vizier-0.1.6/vizier/_src/jax/optimizers/optimizers_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -81,49 +81,89 @@
       for y_, b_ in zip(tree.flatten(optimal_params), tree.flatten(lb)):
         if b_ is not None:
           self.assertTrue((y_ > b_).all())
       for y_, b_ in zip(tree.flatten(optimal_params), tree.flatten(ub)):
         if b_ is not None:
           self.assertTrue((y_ < b_).all())
 
-  def test_sinusodial_bestn_optax(self):
+  @parameterized.parameters(
+      (1, 1),
+      (1, 5),
+      (5, 20),
+  )
+  def test_sinusodial_bestn_optax(self, best_n, random_restarts):
     optimize = optimizers.OptaxTrainWithRandomRestarts(
         optax.adam(5e-3),
         epochs=100,
         verbose=True,
-        random_restarts=100,
-        best_n=5)
+        random_restarts=random_restarts,
+        best_n=best_n,
+    )
     constraint_fn = tfb.JointMap({'x1': tfb.Exp(), 'x2': tfb.Softplus()})
     optimal_params, _ = optimize(
         optimizer_setup,
         loss_fn,
         jax.random.PRNGKey(0),
         # Optax uses the bijector and not the bounds, so it is safe to pass only
         # the bijector.
         constraints=sp.Constraint(bijector=constraint_fn),
     )
     logging.info('Optimal: %s', optimal_params)
 
+    batch_shape = (best_n,) if best_n > 1 else ()
+    self.assertSequenceEqual(optimal_params['x2'].shape, batch_shape + (2,))
+    self.assertSequenceEqual(optimal_params['x1'].shape, batch_shape + (1,))
+
+  @parameterized.parameters(
+      (None,),
+      ((-4.0, None),),
+      ((None, 5.0), False),
+      ((-3.0, 3.0),),
+  )
+  def test_sinusodial_bestn_scipy_l_bfgs_b(self, bounds, nest_constraint=True):
+    if bounds is None:
+      constraints = None
+    else:
+      if nest_constraint:
+        bounds = tree.map_structure(_make_constraint_array, bounds)
+      constraints = sp.Constraint.create(bounds, tfb.SoftClip)
+    optimize = optimizers.JaxoptLbfgsB(
+        random_restarts=6, best_n=5, use_scipy=True
+    )
+    optimal_params, _ = optimize(
+        optimizer_setup, loss_fn, jax.random.PRNGKey(0), constraints=constraints
+    )
+    logging.info('Optimal: %s', optimal_params)
+
     self.assertSequenceEqual(optimal_params['x2'].shape, (5, 2))
     self.assertSequenceEqual(optimal_params['x1'].shape, (5, 1))
+    if bounds is not None:
+      for y_, b_ in zip(tree.flatten(optimal_params), tree.flatten(bounds[0])):
+        if b_ is not None:
+          self.assertTrue((y_ > b_).all())
+      for y_, b_ in zip(tree.flatten(optimal_params), tree.flatten(bounds[1])):
+        if b_ is not None:
+          self.assertTrue((y_ < b_).all())
 
   @parameterized.parameters(
       (None,),
       ((-4.0, None),),
       ((None, 5.0), False),
       ((-3.0, 3.0),),
   )
-  def test_sinusodial_bestn_l_bfgs_b(self, bounds, nest_constraint=True):
+  def test_sinusodial_bestn_jax_l_bfgs_b(self, bounds, nest_constraint=True):
     if bounds is None:
       constraints = None
     else:
       if nest_constraint:
         bounds = tree.map_structure(_make_constraint_array, bounds)
       constraints = sp.Constraint.create(bounds, tfb.SoftClip)
-    optimize = optimizers.JaxoptLbfgsB(random_restarts=10, best_n=5)
+    optimize = optimizers.JaxoptLbfgsB(
+        random_restarts=6, best_n=5, use_scipy=False
+    )
     optimal_params, _ = optimize(
         optimizer_setup, loss_fn, jax.random.PRNGKey(0), constraints=constraints
     )
     logging.info('Optimal: %s', optimal_params)
 
     self.assertSequenceEqual(optimal_params['x2'].shape, (5, 2))
     self.assertSequenceEqual(optimal_params['x1'].shape, (5, 1))
```

### Comparing `google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model.py` & `google-vizier-0.1.6/vizier/_src/jax/stochastic_process_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,40 +19,42 @@
 import abc
 from typing import Any, Callable, Generator, Generic, Optional, Protocol, TypeVar
 
 from absl import logging
 import attr
 from flax import config as flax_config
 from flax import linen as nn
+from flax import struct
 import jax
 from jax import numpy as jnp
 from jax import tree_util
 from jax.typing import ArrayLike
 from tensorflow_probability.substrates import jax as tfp
 import tree
 from vizier._src.jax import types
 
 flax_config.update('flax_return_frozendict', False)
 
 tfd = tfp.distributions
 tfb = tfp.bijectors
+tfpke = tfp.experimental.psd_kernels
 
 _In = TypeVar('_In', bound=types.ArrayTree)
 _D = TypeVar('_D', bound=tfd.Distribution)
 
 
 class InitFn(Protocol):
   """Protocol for Flax parameter initialization functions."""
 
   @abc.abstractmethod
   def __call__(self, rng: jax.random.KeyArray) -> jax.Array:
     pass
 
 
-@attr.frozen
+@struct.dataclass
 class Constraint:
   """Class specifying parameter constraints.
 
   `ModelParameter`s may optionally contain a `Constraint` object that specifies
   the lower/upper bounds of the parameter and a bijector that maps from the
   space of all real numbers to the interval between the lower and upper bounds.
 
@@ -213,16 +215,19 @@
   to initialize Flax parameters and build stochastic process objects.
 
   When a `ModelCoroutine` is called, it returns a generator-iterator, which
   should be iterated to build the `ModelParameter`s and the stochastic process
   object. See the full protocol below.
   """
 
-  def __call__(self,
-               inputs: Optional[_In] = None) -> ModelParameterGenerator[_D]:
+  def __call__(
+      self,
+      inputs: Optional[_In] = None,
+      **kwargs,
+  ) -> ModelParameterGenerator[_D]:
     """Coroutine function to be called from `StochasticProcessModel`.
 
     The coroutine is implemented via an enhanced generator
     (https://peps.python.org/pep-0342/). The generator-iterator returned by this
     method corresponds to the pytype
     `Generator[YieldType, SendType, ReturnType]`. (Python also has a newer, more
     flexible `Coroutine` type declared with `async`/`await` syntax. Here, when
@@ -271,14 +276,15 @@
           constraint=Constraint(bounds=(jnp.zeros([]), None)))
       return tfd.GaussianProcess(kernel=kernel, index_points=inputs,
           observation_noise_variance=observation_noise)
     ```
 
     Args:
       inputs: An ArrayTree of index points or None.
+      **kwargs:
     """
     pass
 
 
 class StochasticProcessModel(nn.Module, Generic[_In]):
   """Builds a Stochastic Process Flax module.
 
@@ -351,27 +357,28 @@
         param: jax.Array = self.param(p.name, p.init_fn)
         p: ModelParameter = generator.send(param)
     except StopIteration:
       # Ignore the return value from the generator since this method only builds
       # the Flax parameters.
       pass
 
-  def __call__(self, x: _In) -> _D:
+  def __call__(self, x: _In, **kwargs) -> _D:
     """Returns a stochastic process distribution.
 
     If the Flax module's `apply` method is called with `mutable=True` or
     `mutable=('losses,')` regularization losses are additionally returned.
 
     Args:
       x: ArrayTree of index points in the constrained space.
+      **kwargs:
 
     Returns:
       dist: `tfd.Distribution` instance with x as index points.
     """
-    gen = self.coroutine(inputs=x)
+    gen = self.coroutine(inputs=x, **kwargs)
     if self.is_initializing() and isinstance(self.mean_fn, nn.Module):
       # If mean_fn is a module, call it so its parameters are initialized.
       _ = self.mean_fn(x)  # pylint: disable=not-callable
     try:
       p: ModelParameter = next(gen)
       while True:
         # "params" is the name that `nn.Module` gives to the collection of read-
@@ -387,35 +394,52 @@
         p = gen.send(param)
     except StopIteration as e:
       # After the generator is exhausted, it raises a `StopIteration` error. The
       # `StopIteration` object has a property `value` of type `_D`.
       gp = e.value
       return gp.copy(mean_fn=self.mean_fn)
 
+  # TODO: Add support for PaddedArrays instead of passing in
+  # masks.
   def precompute_predictive(
-      self, x_observed: _In, y_observed: ArrayLike
+      self,
+      x_observed: _In,
+      y_observed: ArrayLike,
+      observations_is_missing: Optional[ArrayLike] = None,
   ) -> None:
     """Builds a stochastic process regression model conditioned on observations.
 
     The mutable variable returned by this method as auxiliary output should be
     passed as state to `posterior_predictive`. This avoids repeated, expensive
     operations (often Cholesky decompositions) when computing the posterior
     predictive.
 
     Args:
       x_observed: Index points on which to condition the posterior predictive.
       y_observed: Observations on which to condition the posterior predictive.
+      observations_is_missing: Boolean array describing which observations are
+        missing.
     """
     # Call the `tfd.Distribution` object's `posterior_predictive` method. This
     # triggers an expensive computation, typically a Cholesky decomposition, and
     # returns a new `tfd.Distribution` representing the posterior predictive.
     # Expensive intermediates are stored in the `precomputed_cholesky` Flax
     # variable and returned as auxiliary output.
+    kwargs = {}
+    if observations_is_missing is not None:
+      kwargs['observations_is_missing'] = observations_is_missing
+
+    if isinstance(x_observed, types.ContinuousAndCategoricalArray):
+      x_observed = tfpke.ContinuousAndCategoricalValues(
+          continuous=x_observed.continuous, categorical=x_observed.categorical
+      )
+
     predictive_dist = self(x_observed).posterior_predictive(
-        index_points=None, observations=y_observed)
+        index_points=None, observations=y_observed, **kwargs
+    )
     # pylint: disable=protected-access
     cached_predictive_intermediates = {
         '_precomputed_divisor_matrix_cholesky': (
             predictive_dist._precomputed_divisor_matrix_cholesky
         ),
         '_precomputed_solve_on_observation': (
             predictive_dist._precomputed_solve_on_observation
@@ -425,16 +449,23 @@
     self.sow(
         'predictive',
         'precomputed_cholesky',
         cached_predictive_intermediates,
         reduce_fn=lambda _, b: b,
     )
 
+  # TODO: Add support for PaddedArrays instead of passing in
+  # masks.
   def posterior_predictive(
-      self, x_predictive: _In, x_observed: _In, y_observed: ArrayLike
+      self,
+      x_predictive: _In,
+      x_observed: _In,
+      y_observed: ArrayLike,
+      *,
+      observations_is_missing: Optional[ArrayLike] = None,
   ) -> _D:
     """Returns a posterior predictive stochastic process.
 
     The posterior predictive distribution over the function values at
     `x_predictive`, typically a `tfd.GaussianProcessRegressionModel` or
     `tfd.StudentTProcessRegressionModel`, is built using the mutable variable in
     `predictive/precomputed_cholesky`. This avoids repeated, expensive
@@ -442,14 +473,16 @@
     data). See the class docstring for how to use `precompute_predictive` in
     combination with `posterior_predictive`.
 
     Args:
       x_predictive: Predictive index points.
       x_observed: Index points on which to condition the posterior predictive.
       y_observed: Observations on which to condition the posterior predictive.
+      observations_is_missing: Boolean array describing which observations are
+        missing.
 
     Returns:
       pp_dist: The posterior predictive distribution over `x_predictive`.
     """
     if not self.has_variable('predictive', 'precomputed_cholesky'):
       raise ValueError(
           'The mutable variable returned by '
@@ -458,18 +491,28 @@
       )
     # Access the precomputed values stored in the Flax variable, and build the
     # distribution object over the predictive index points (avoiding
     # recomputation).
     cached_intermediates = self.get_variable(
         'predictive', 'precomputed_cholesky'
     )
+    kwargs = cached_intermediates
+    if observations_is_missing is not None:
+      kwargs = kwargs.copy({'observations_is_missing': observations_is_missing})
+
+    if isinstance(x_predictive, types.ContinuousAndCategoricalArray):
+      x_predictive = tfpke.ContinuousAndCategoricalValues(
+          continuous=x_predictive.continuous,
+          categorical=x_predictive.categorical,
+      )
+
     return self(x_observed).posterior_predictive(
         observations=y_observed,
         predictive_index_points=x_predictive,
-        **cached_intermediates,
+        **kwargs,
     )
 
 
 class VectorToArrayTree(tfb.Chain):
   """Bijector that converts a vector to a dict like `params`.
 
   The bijector splits the vector, reshapes the splits, and then packs the splits
```

### Comparing `google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model_test.py` & `google-vizier-0.1.6/vizier/_src/jax/stochastic_process_model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 """Tests for stochastic_process_model."""
 
 import functools
 from unittest import mock
 
 from absl.testing import parameterized
 from flax import linen as nn
-
 import jax
 from jax import numpy as jnp
 from jax import random
 from jax.config import config
 import numpy as np
 from tensorflow_probability.substrates import jax as tfp
 import tree
 from vizier._src.jax import stochastic_process_model as sp_model
+from vizier._src.jax import types
+
 from absl.testing import absltest
 
-config.update('jax_enable_x64', True)
 
 tfb = tfp.bijectors
 tfd = tfp.distributions
 tfpk = tfp.math.psd_kernels
 tfde = tfp.experimental.distributions
 tfpke = tfp.experimental.psd_kernels
 
@@ -90,14 +90,19 @@
 def _test_coroutine(
     inputs=None,
     kernel_coroutine=_continuous_kernel_coroutine,
     num_tasks=1,
     dtype=np.float64,
 ):
   """A coroutine that follows the `ModelCoroutine` protocol."""
+  if isinstance(inputs, types.ContinuousAndCategoricalArray):
+    inputs = tfpke.ContinuousAndCategoricalValues(
+        inputs.continuous, inputs.categorical
+    )
+
   kernel = yield from kernel_coroutine(dtype=dtype)
   if num_tasks == 1:
     return tfd.StudentTProcess(
         df=dtype(5.0),
         kernel=kernel,
         index_points=inputs,
         observation_noise_variance=np.ones([], dtype=dtype),
@@ -136,27 +141,27 @@
   cat_dim = 3
   x_observed_cont = random.uniform(
       cont_obs_key, shape=(num_observed, cont_dim), dtype=dtype
   )
   x_observed_cat = random.randint(
       cat_obs_key, shape=(num_observed, cat_dim), minval=0, maxval=6
   )
-  x_observed = tfpke.ContinuousAndCategoricalValues(
+  x_observed = types.ContinuousAndCategoricalArray(
       x_observed_cont, x_observed_cat
   )
   y_shape = (num_observed,) if num_tasks == 1 else (num_observed, num_tasks)
   y_observed = random.uniform(y_key, shape=y_shape, dtype=dtype)
 
   x_predictive_cont = random.uniform(
       cont_pred_key, shape=(100, num_predictive, cont_dim), dtype=dtype
   )
   x_predictive_cat = random.randint(
       cat_pred_key, shape=(num_predictive, cat_dim), minval=0, maxval=6
   )
-  x_predictive = tfpke.ContinuousAndCategoricalValues(
+  x_predictive = types.ContinuousAndCategoricalArray(
       x_predictive_cont, x_predictive_cat
   )
   return x_observed, y_observed, x_predictive
 
 
 class MeanFn(nn.Module):
 
@@ -570,8 +575,9 @@
         self.assertTrue((y_ >= b_).all())
     for y_, b_ in zip(tree.flatten(p), tree.flatten(upper)):
       if b_ is not None:
         self.assertTrue((y_ <= b_).all())
 
 
 if __name__ == '__main__':
+  config.update('jax_enable_x64', True)
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/jax/xla_pareto.py` & `google-vizier-0.1.6/vizier/_src/jax/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/jax/xla_pareto_test.py` & `google-vizier-0.1.6/vizier/_src/jax/xla_pareto_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/algorithms.py` & `google-vizier-0.1.6/vizier/_src/pyglove/algorithms.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/backend.py` & `google-vizier-0.1.6/vizier/_src/pyglove/backend.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/client.py` & `google-vizier-0.1.6/vizier/_src/pyglove/client.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/constants.py` & `google-vizier-0.1.6/vizier/_src/pyglove/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/converters.py` & `google-vizier-0.1.6/vizier/_src/pyglove/converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/converters_test.py` & `google-vizier-0.1.6/vizier/_src/pyglove/converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/core.py` & `google-vizier-0.1.6/vizier/_src/pyglove/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/e2e_test.py` & `google-vizier-0.1.6/vizier/_src/pyglove/e2e_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier.py` & `google-vizier-0.1.6/vizier/_src/pyglove/oss_vizier.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier_test.py` & `google-vizier-0.1.6/vizier/_src/pyglove/oss_vizier_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/performance_test.py` & `google-vizier-0.1.6/vizier/_src/pyglove/performance_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/pythia.py` & `google-vizier-0.1.6/vizier/_src/pyglove/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/pythia_test.py` & `google-vizier-0.1.6/vizier/_src/pyglove/pythia_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyglove/vizier_test_lib.py` & `google-vizier-0.1.6/vizier/_src/pyglove/vizier_test_lib.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters.py` & `google-vizier-0.1.6/vizier/_src/pythia/local_policy_supporters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters_test.py` & `google-vizier-0.1.6/vizier/_src/pythia/local_policy_supporters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pythia/policy.py` & `google-vizier-0.1.6/vizier/_src/pythia/policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 """Base class for all PythiaPolicies."""
 
 import abc
 from typing import Any, FrozenSet, Optional
 
 import attr
-from vizier import pyvizier as vz
+from vizier._src.pyvizier.pythia import study
+from vizier._src.pyvizier.shared import base_study_config
+from vizier._src.pyvizier.shared import trial
 
 
 def _is_positive(instance: Any, attribute: Any, value: Any):
   del instance, attribute
   if value <= 0:
     raise ValueError(f'value must be positive! given: {value}')
 
@@ -59,19 +61,21 @@
       default=True,
       validator=[attr.validators.instance_of(bool)],
       on_setattr=attr.setters.validate)
 
   # TODO: Add a proper support for this in the service side.
   # NOTE: As of 2022Q3, the standard deviation field of Metrics in this value
   #   are ignored (i.e. $predicted_final_measurement.metrics[].std).
-  predicted_final_measurement: Optional[vz.Measurement] = attr.ib(
+  predicted_final_measurement: Optional[trial.Measurement] = attr.ib(
       default=None,
       validator=attr.validators.optional(
-          attr.validators.instance_of(vz.Measurement)),
-      on_setattr=attr.setters.validate)
+          attr.validators.instance_of(trial.Measurement)
+      ),
+      on_setattr=attr.setters.validate,
+  )
 
 
 @attr.define
 class EarlyStopDecisions:
   """This is the output of the Policy.early_stop() method.
 
   Attributes:
@@ -82,17 +86,18 @@
 
   decisions: list[EarlyStopDecision] = attr.field(
       factory=list,
       validator=attr.validators.deep_iterable(
           attr.validators.instance_of(EarlyStopDecision)),
       converter=list)
 
-  metadata: vz.MetadataDelta = attr.field(
-      default=attr.Factory(vz.MetadataDelta),
-      validator=attr.validators.instance_of(vz.MetadataDelta))
+  metadata: trial.MetadataDelta = attr.field(
+      default=attr.Factory(trial.MetadataDelta),
+      validator=attr.validators.instance_of(trial.MetadataDelta),
+  )
 
 
 @attr.define
 class EarlyStopRequest:
   """Early stopping request.
 
   Attributes:
@@ -101,16 +106,17 @@
       Trials". This is a hint; it is allowable to consider stopping more or
       fewer trials.
     study_config:
     checkpoint_dir: If the policy wishes to use a checkpoint, then this is the
       path to find one.
     max_trial_id: max(trial.id for all existing Trials in the Study)
   """
-  _study_descriptor: vz.StudyDescriptor = attr.field(
-      kw_only=True, validator=attr.validators.instance_of(vz.StudyDescriptor))
+  _study_descriptor: study.StudyDescriptor = attr.field(
+      kw_only=True, validator=attr.validators.instance_of(study.StudyDescriptor)
+  )
 
   trial_ids: Optional[FrozenSet[int]] = attr.field(
       default=None,
       validator=lambda x, c, v: x is None or isinstance(x, FrozenSet),
       converter=lambda x: None if x is None else frozenset(x))
 
   checkpoint_dir: Optional[str] = attr.field(
@@ -118,15 +124,15 @@
       validator=attr.validators.optional(attr.validators.instance_of(str)))
 
   @property
   def study_guid(self) -> str:
     return self._study_descriptor.guid
 
   @property
-  def study_config(self) -> vz.ProblemStatement:
+  def study_config(self) -> base_study_config.ProblemStatement:
     return self._study_descriptor.config
 
   @property
   def max_trial_id(self) -> int:
     return self._study_descriptor.max_trial_id
 
 
@@ -136,24 +142,27 @@
 
   Attributes:
     suggestions: Trials to be suggested to the user.
     metadata: Metadata that's associated with the Study or with already existing
       Trials.
   """
 
-  suggestions: list[vz.TrialSuggestion] = attr.field(
+  suggestions: list[trial.TrialSuggestion] = attr.field(
       init=True,
       validator=attr.validators.deep_iterable(
-          attr.validators.instance_of(vz.TrialSuggestion)),
-      converter=list)
+          attr.validators.instance_of(trial.TrialSuggestion)
+      ),
+      converter=list,
+  )
 
-  metadata: vz.MetadataDelta = attr.field(
+  metadata: trial.MetadataDelta = attr.field(
       init=True,
-      default=attr.Factory(vz.MetadataDelta),
-      validator=attr.validators.instance_of(vz.MetadataDelta))
+      default=attr.Factory(trial.MetadataDelta),
+      validator=attr.validators.instance_of(trial.MetadataDelta),
+  )
 
 
 @attr.define
 class SuggestRequest:
   """Suggestion Request.
 
   Attributes:
@@ -161,32 +170,33 @@
     study_guid: Study id
     count: A recommendation for how many suggestions should be generated.
     study_config:
     checkpoint_dir: (If set) A system-provided directory where the policy can
       store a checkpoint.
     max_trial_id: max(trial.id for all existing Trials in the Study)
   """
-  _study_descriptor: vz.StudyDescriptor = attr.field(
-      validator=attr.validators.instance_of(vz.StudyDescriptor),
+  _study_descriptor: study.StudyDescriptor = attr.field(
+      validator=attr.validators.instance_of(study.StudyDescriptor),
       on_setattr=attr.setters.frozen,
-      kw_only=True)
+      kw_only=True,
+  )
 
   count: int = attr.field(
       validator=[attr.validators.instance_of(int), _is_positive],
       on_setattr=attr.setters.validate,
       kw_only=True)
 
   checkpoint_dir: Optional[str] = attr.field(
       default=None,
       validator=attr.validators.optional(attr.validators.instance_of(str)),
       on_setattr=attr.setters.validate,
       kw_only=True)
 
   @property
-  def study_config(self) -> vz.ProblemStatement:
+  def study_config(self) -> base_study_config.ProblemStatement:
     return self._study_descriptor.config
 
   @property
   def study_guid(self) -> str:
     return str(self._study_descriptor.guid)
 
   @property
```

### Comparing `google-vizier-0.1.5/vizier/_src/pythia/policy_supporter.py` & `google-vizier-0.1.6/vizier/_src/pythia/policy_supporter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pythia/pythia_errors.py` & `google-vizier-0.1.6/vizier/_src/pythia/pythia_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/hypervolume.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/hypervolume_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/pareto_optimal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/safety.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/multimetric/safety_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/automated_stopping.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/automated_stopping_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/compare.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/compare.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/metadata_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/metadata_util_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/proto_converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,80 +11,85 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Converters for OSS Vizier's protos from/to PyVizier's classes."""
+
 import datetime
 import logging
 from typing import Iterable, List, Optional, Sequence, Tuple, Union
 
 from absl import logging
-from vizier import pyvizier as vz
 from vizier._src.pythia import policy
 from vizier._src.pyvizier.oss import metadata_util
 from vizier._src.pyvizier.pythia import study
+from vizier._src.pyvizier.shared import base_study_config
+from vizier._src.pyvizier.shared import common
+from vizier._src.pyvizier.shared import parameter_config
+from vizier._src.pyvizier.shared import trial
 from vizier._src.service import pythia_service_pb2
 from vizier._src.service import study_pb2
 from vizier._src.service import vizier_service_pb2
 
-ScaleType = vz.ScaleType
+
+ScaleType = parameter_config.ScaleType
 _ScaleTypePb2 = study_pb2.StudySpec.ParameterSpec.ScaleType
-ParameterType = vz.ParameterType
-MonotypeParameterSequence = vz.MonotypeParameterSequence
+ParameterType = parameter_config.ParameterType
+MonotypeParameterSequence = parameter_config.MonotypeParameterSequence
 
 
 class StudyStateConverter:
   """Proto converter for Study states."""
 
   _pyvizier_to_proto = {
-      vz.StudyState.ACTIVE: study_pb2.Study.State.ACTIVE,
-      vz.StudyState.ABORTED: study_pb2.Study.State.INACTIVE,
-      vz.StudyState.COMPLETED: study_pb2.Study.State.COMPLETED,
+      study.StudyState.ACTIVE: study_pb2.Study.State.ACTIVE,
+      study.StudyState.ABORTED: study_pb2.Study.State.INACTIVE,
+      study.StudyState.COMPLETED: study_pb2.Study.State.COMPLETED,
   }
   _proto_to_pyvizier = {v: k for k, v in _pyvizier_to_proto.items()}
 
   @classmethod
-  def to_proto(cls, state: vz.StudyState) -> study_pb2.Study.State:
+  def to_proto(cls, state: study.StudyState) -> study_pb2.Study.State:
     if state in cls._pyvizier_to_proto:
       return cls._pyvizier_to_proto[state]
     return study_pb2.Study.State.STATE_UNSPECIFIED
 
   @classmethod
-  def from_proto(cls, proto: study_pb2.Study.State) -> vz.StudyState:
+  def from_proto(cls, proto: study_pb2.Study.State) -> study.StudyState:
     if proto in cls._proto_to_pyvizier:
       return cls._proto_to_pyvizier[proto]
     elif proto == study_pb2.Study.State.STATE_UNSPECIFIED:
       # OSS Vizier server treats STATE_UNSPECIFIED as ACTIVE.
-      return vz.StudyState.ACTIVE
+      return study.StudyState.ACTIVE
     else:
       raise ValueError(
           'Proto Study state {} has no equivalent in PyVizier.'.format(
               study_pb2.Study.State.Name(proto)
           )
       )
 
 
 class _ScaleTypeMap:
   """Proto converter for scale type."""
 
   _pyvizier_to_proto = {
-      vz.ScaleType.LINEAR: _ScaleTypePb2.UNIT_LINEAR_SCALE,
-      vz.ScaleType.LOG: _ScaleTypePb2.UNIT_LOG_SCALE,
-      vz.ScaleType.REVERSE_LOG: _ScaleTypePb2.UNIT_REVERSE_LOG_SCALE,
+      ScaleType.LINEAR: _ScaleTypePb2.UNIT_LINEAR_SCALE,
+      ScaleType.LOG: _ScaleTypePb2.UNIT_LOG_SCALE,
+      ScaleType.REVERSE_LOG: _ScaleTypePb2.UNIT_REVERSE_LOG_SCALE,
   }
   _proto_to_pyvizier = {v: k for k, v in _pyvizier_to_proto.items()}
 
   @classmethod
-  def to_proto(cls, pyvizier: vz.ScaleType) -> _ScaleTypePb2:
+  def to_proto(cls, pyvizier: ScaleType) -> _ScaleTypePb2:
     return cls._pyvizier_to_proto[pyvizier]
 
   @classmethod
-  def from_proto(cls, proto: _ScaleTypePb2) -> vz.ScaleType:
+  def from_proto(cls, proto: _ScaleTypePb2) -> ScaleType:
     return cls._proto_to_pyvizier[proto]
 
 
 class ParameterConfigConverter:
   """Converter for ParameterConfig."""
 
   @classmethod
@@ -150,15 +155,15 @@
 
   @classmethod
   def from_proto(
       cls,
       proto: study_pb2.StudySpec.ParameterSpec,
       *,
       strict_validation: bool = False,
-  ) -> vz.ParameterConfig:
+  ) -> parameter_config.ParameterConfig:
     """Creates a ParameterConfig.
 
     Args:
       proto:
       strict_validation: If True, raise ValueError to enforce that
         from_proto(proto).to_proto == proto.
 
@@ -202,15 +207,15 @@
       children = None
 
     scale_type = None
     if proto.scale_type:
       scale_type = _ScaleTypeMap.from_proto(proto.scale_type)
 
     try:
-      config = vz.ParameterConfig.factory(
+      config = parameter_config.ParameterConfig.factory(
           name=proto.parameter_id,
           feasible_values=feasible_values,
           bounds=bounds,
           children=children,
           scale_type=scale_type,
           default_value=default_value,
       )
@@ -227,26 +232,28 @@
       )
     return config
 
   @classmethod
   def _set_child_parameter_configs(
       cls,
       parent_proto: study_pb2.StudySpec.ParameterSpec,
-      pc: vz.ParameterConfig,
+      pc: parameter_config.ParameterConfig,
   ):
     """Sets the parent_proto's conditional_parameter_specs field.
 
     Args:
       parent_proto: Modified in place.
       pc: Parent ParameterConfig to copy children from.
 
     Raises:
       ValueError: If the child configs are invalid
     """
-    children: List[Tuple[MonotypeParameterSequence, vz.ParameterConfig]] = []
+    children: List[
+        Tuple[MonotypeParameterSequence, parameter_config.ParameterConfig]
+    ] = []
     for child in pc.child_parameter_configs:
       children.append((child.matching_parent_values, child))
     if not children:
       return
 
     parent_proto.ClearField('conditional_parameter_specs')
     for child_pair in children:
@@ -286,15 +293,15 @@
         cls._set_child_parameter_configs(child_proto, child)
       parent_proto.conditional_parameter_specs.extend(
           [conditional_parameter_spec]
       )
 
   @classmethod
   def to_proto(
-      cls, pc: vz.ParameterConfig
+      cls, pc: parameter_config.ParameterConfig
   ) -> study_pb2.StudySpec.ParameterSpec:
     """Returns a ParameterConfig Proto."""
     proto = study_pb2.StudySpec.ParameterSpec(parameter_id=pc.name)
     if pc.type == ParameterType.DISCRETE:
       cls._set_feasible_points(proto, [float(v) for v in pc.feasible_values])
     elif pc.type == ParameterType.CATEGORICAL:
       cls._set_categories(proto, pc.feasible_values)
@@ -316,31 +323,31 @@
 
 class ParameterValueConverter:
   """Converter for vz.ParameterValue."""
 
   @classmethod
   def from_proto(
       cls, proto: study_pb2.Trial.Parameter
-  ) -> Optional[vz.ParameterValue]:
+  ) -> Optional[trial.ParameterValue]:
     """Returns whichever value that is populated, or None."""
     value_proto = proto.value
     oneof_name = value_proto.WhichOneof('kind')
     potential_value = getattr(value_proto, oneof_name)
     if (
         isinstance(potential_value, float)
         or isinstance(potential_value, str)
         or isinstance(potential_value, bool)
     ):
-      return vz.ParameterValue(potential_value)
+      return trial.ParameterValue(potential_value)
     else:
       return None
 
   @classmethod
   def to_proto(
-      cls, parameter_value: vz.ParameterValue, name: str
+      cls, parameter_value: trial.ParameterValue, name: str
   ) -> study_pb2.Trial.Parameter:
     """Returns Parameter Proto."""
     proto = study_pb2.Trial.Parameter(parameter_id=name)
 
     if isinstance(parameter_value.value, int):
       proto.value.number_value = parameter_value.value
     elif isinstance(parameter_value.value, bool):
@@ -353,15 +360,15 @@
     return proto
 
 
 class MeasurementConverter:
   """Converter for vz.Measurement."""
 
   @classmethod
-  def from_proto(cls, proto: study_pb2.Measurement) -> vz.Measurement:
+  def from_proto(cls, proto: study_pb2.Measurement) -> trial.Measurement:
     """Creates a valid instance from proto.
 
     Args:
       proto: Measurement proto.
 
     Returns:
       A valid instance of Measurement object. Metrics with invalid values
@@ -385,25 +392,25 @@
             ),
             5,
             metric.metric_id,
             metric.value,
             metrics[metric.metric_id].value,
         )
       try:
-        metrics[metric.metric_id] = vz.Metric(value=metric.value)
+        metrics[metric.metric_id] = trial.Metric(value=metric.value)
       except ValueError:
         pass
-    return vz.Measurement(
+    return trial.Measurement(
         metrics=metrics,
         elapsed_secs=proto.elapsed_duration.seconds,
         steps=proto.step_count,
     )
 
   @classmethod
-  def to_proto(cls, measurement: vz.Measurement) -> study_pb2.Measurement:
+  def to_proto(cls, measurement: trial.Measurement) -> study_pb2.Measurement:
     """Converts to Measurement proto."""
     proto = study_pb2.Measurement()
     for name, metric in measurement.metrics.items():
       proto.metrics.add(metric_id=name, value=metric.value)
 
     proto.step_count = measurement.steps
     int_seconds = int(measurement.elapsed_secs)
@@ -416,136 +423,138 @@
 
 class MetricInformationConverter:
   """A converter to/from study_pb2.StudySpec.MetricInformation."""
 
   @classmethod
   def from_proto(
       cls, proto: study_pb2.StudySpec.MetricSpec
-  ) -> vz.MetricInformation:
+  ) -> base_study_config.MetricInformation:
     """Converts a MetricInformation proto to a MetricInformation object."""
-    if proto.goal not in list(vz.ObjectiveMetricGoal):
+    if proto.goal not in list(base_study_config.ObjectiveMetricGoal):
       raise ValueError('Unknown MetricInformation.goal: {}'.format(proto.goal))
 
     safety_threshold = None
     desired_min_safe_trials_fraction = None
 
     if proto.HasField('safety_config'):
       safety_threshold = proto.safety_config.safety_threshold
     if proto.safety_config.HasField('desired_min_safe_trials_fraction'):
       desired_min_safe_trials_fraction = (
           proto.safety_config.desired_min_safe_trials_fraction
       )
 
-    return vz.MetricInformation(
+    return base_study_config.MetricInformation(
         name=proto.metric_id,
         goal=proto.goal,
         safety_threshold=safety_threshold,
         desired_min_safe_trials_fraction=desired_min_safe_trials_fraction,
         min_value=None,
         max_value=None,
     )
 
   @classmethod
   def to_proto(
-      cls, obj: vz.MetricInformation
+      cls, obj: base_study_config.MetricInformation
   ) -> study_pb2.StudySpec.MetricSpec:
     """Returns this object as a proto."""
 
     proto = study_pb2.StudySpec.MetricSpec(
         metric_id=obj.name, goal=obj.goal.value
     )
 
-    if obj.type == vz.MetricType.SAFETY:
+    if obj.type == base_study_config.MetricType.SAFETY:
       proto.safety_config.safety_threshold = obj.safety_threshold
       if obj.desired_min_safe_trials_fraction is not None:
         proto.safety_config.desired_min_safe_trials_fraction = (
             obj.desired_min_safe_trials_fraction
         )
     return proto
 
 
 class SearchSpaceConverter:
   """A wrapper for study_pb2.StudySpec."""
 
   @classmethod
-  def from_proto(cls, proto: study_pb2.StudySpec) -> vz.SearchSpace:
+  def from_proto(
+      cls, proto: study_pb2.StudySpec
+  ) -> parameter_config.SearchSpace:
     """Extracts a SearchSpace object from a StudyConfig proto."""
-    space = vz.SearchSpace()
+    space = parameter_config.SearchSpace()
     for pc in proto.parameters:
       space.add(ParameterConfigConverter.from_proto(pc))
     return space
 
   @classmethod
   def parameter_protos(
-      cls, obj: vz.SearchSpace
+      cls, obj: parameter_config.SearchSpace
   ) -> List[study_pb2.StudySpec.ParameterSpec]:
     """Returns the search space as a List of ParameterConfig protos."""
     return [ParameterConfigConverter.to_proto(pc) for pc in obj.parameters]
 
 
 class MetricsConfigConverter:
   """A wrapper for study_pb2.StudySpec.MetricSpec's."""
 
   @classmethod
   def from_protos(
       cls, protos: Iterable[study_pb2.StudySpec.MetricSpec]
-  ) -> vz.MetricsConfig:
-    return vz.MetricsConfig(
+  ) -> base_study_config.MetricsConfig:
+    return base_study_config.MetricsConfig(
         [MetricInformationConverter.from_proto(m) for m in protos]
     )
 
   @classmethod
   def to_protos(
-      cls, obj: vz.MetricsConfig
+      cls, obj: base_study_config.MetricsConfig
   ) -> List[study_pb2.StudySpec.MetricSpec]:
     return [MetricInformationConverter.to_proto(metric) for metric in obj]
 
 
 def _to_pyvizier_trial_status(
     proto_state: study_pb2.Trial.State,
-) -> vz.TrialStatus:
+) -> trial.TrialStatus:
   """from_proto conversion for Trial statuses."""
   if proto_state == study_pb2.Trial.State.REQUESTED:
-    return vz.TrialStatus.REQUESTED
+    return trial.TrialStatus.REQUESTED
   elif proto_state == study_pb2.Trial.State.ACTIVE:
-    return vz.TrialStatus.ACTIVE
+    return trial.TrialStatus.ACTIVE
   if proto_state == study_pb2.Trial.State.STOPPING:
-    return vz.TrialStatus.STOPPING
+    return trial.TrialStatus.STOPPING
   if proto_state == study_pb2.Trial.State.SUCCEEDED:
-    return vz.TrialStatus.COMPLETED
+    return trial.TrialStatus.COMPLETED
   elif proto_state == study_pb2.Trial.State.INFEASIBLE:
-    return vz.TrialStatus.COMPLETED
+    return trial.TrialStatus.COMPLETED
   else:
-    return vz.TrialStatus.UNKNOWN
+    return trial.TrialStatus.UNKNOWN
 
 
 def _from_pyvizier_trial_status(
-    status: vz.TrialStatus, infeasible: bool
+    status: trial.TrialStatus, infeasible: bool
 ) -> study_pb2.Trial.State:
   """to_proto conversion for Trial states."""
-  if status == vz.TrialStatus.REQUESTED:
+  if status == trial.TrialStatus.REQUESTED:
     return study_pb2.Trial.State.REQUESTED
-  elif status == vz.TrialStatus.ACTIVE:
+  elif status == trial.TrialStatus.ACTIVE:
     return study_pb2.Trial.State.ACTIVE
-  elif status == vz.TrialStatus.STOPPING:
+  elif status == trial.TrialStatus.STOPPING:
     return study_pb2.Trial.State.STOPPING
-  elif status == vz.TrialStatus.COMPLETED:
+  elif status == trial.TrialStatus.COMPLETED:
     if infeasible:
       return study_pb2.Trial.State.INFEASIBLE
     else:
       return study_pb2.Trial.State.SUCCEEDED
   else:
     return study_pb2.Trial.State.STATE_UNSPECIFIED
 
 
 class TrialConverter:
   """Converter for vz.Trial."""
 
   @classmethod
-  def from_proto(cls, proto: study_pb2.Trial) -> vz.Trial:
+  def from_proto(cls, proto: study_pb2.Trial) -> trial.Trial:
     """Converts from Trial proto to object.
 
     Args:
       proto: Trial proto.
 
     Returns:
       A Trial object.
@@ -577,29 +586,29 @@
     if proto.state == study_pb2.Trial.State.SUCCEEDED:
       if proto.HasField('end_time'):
         completion_ts = proto.end_time.seconds + 1e-9 * proto.end_time.nanos
         completion_time = datetime.datetime.fromtimestamp(completion_ts)
     elif proto.state == study_pb2.Trial.State.INFEASIBLE:
       infeasibility_reason = proto.infeasible_reason
 
-    metadata = vz.Metadata()
+    metadata = common.Metadata()
     for kv in proto.metadata:
-      metadata.abs_ns(vz.Namespace.decode(kv.ns))[kv.key] = (
+      metadata.abs_ns(common.Namespace.decode(kv.ns))[kv.key] = (
           kv.proto if kv.HasField('proto') else kv.value
       )
 
     measurements = []
     for measure in proto.measurements:
       measurements.append(MeasurementConverter.from_proto(measure))
 
     creation_time = None
     if proto.HasField('start_time'):
       creation_ts = proto.start_time.seconds + 1e-9 * proto.start_time.nanos
       creation_time = datetime.datetime.fromtimestamp(creation_ts)
-    return vz.Trial(
+    return trial.Trial(
         id=int(proto.id),
         description=proto.name,
         assigned_worker=proto.client_id or None,
         is_requested=proto.state == proto.REQUESTED,
         stopping_reason=(
             'stopping reason not supported yet'
             if proto.state == proto.STOPPING
@@ -611,24 +620,24 @@
         infeasibility_reason=infeasibility_reason,
         final_measurement=final_measurement,
         measurements=measurements,
         metadata=metadata,
     )  # pytype: disable=wrong-arg-types
 
   @classmethod
-  def from_protos(cls, protos: Iterable[study_pb2.Trial]) -> List[vz.Trial]:
+  def from_protos(cls, protos: Iterable[study_pb2.Trial]) -> List[trial.Trial]:
     """Convenience wrapper for from_proto."""
     return [TrialConverter.from_proto(proto) for proto in protos]
 
   @classmethod
-  def to_protos(cls, pytrials: Iterable[vz.Trial]) -> List[study_pb2.Trial]:
+  def to_protos(cls, pytrials: Iterable[trial.Trial]) -> List[study_pb2.Trial]:
     return [TrialConverter.to_proto(pytrial) for pytrial in pytrials]
 
   @classmethod
-  def to_proto(cls, pytrial: vz.Trial) -> study_pb2.Trial:
+  def to_proto(cls, pytrial: trial.Trial) -> study_pb2.Trial:
     """Converts a pyvizier Trial to a Trial proto."""
     proto = study_pb2.Trial()
     if pytrial.description is not None:
       proto.name = pytrial.description
     proto.id = str(pytrial.id)
     proto.state = _from_pyvizier_trial_status(
         pytrial.status, pytrial.infeasible
@@ -669,53 +678,53 @@
 
 class TrialSuggestionConverter:
   """Converts vz.TrialSuggestion <--> Pythia TrialSuggestion proto."""
 
   @classmethod
   def from_proto(
       cls, proto: pythia_service_pb2.TrialSuggestion
-  ) -> vz.TrialSuggestion:
+  ) -> trial.TrialSuggestion:
     """Converts from TrialSuggestion proto to PyVizier TrialSuggestion."""
     parameters = {}
     for parameter in proto.parameters:
       value = ParameterValueConverter.from_proto(parameter)
       if value is None:
         raise RuntimeError('Parameter %s exists without a value.' % parameter)
       if parameter.parameter_id in parameters:
         raise ValueError(
             'Invalid trial proto contains duplicate parameter {}: {}'.format(
                 parameter.parameter_id, proto
             )
         )
       parameters[parameter.parameter_id] = value
 
-    metadata = vz.Metadata()
+    metadata = common.Metadata()
     for kv in proto.metadata:
-      metadata.abs_ns(vz.Namespace.decode(kv.ns))[kv.key] = (
+      metadata.abs_ns(common.Namespace.decode(kv.ns))[kv.key] = (
           kv.proto if kv.HasField('proto') else kv.value
       )
 
-    return vz.TrialSuggestion(parameters=parameters, metadata=metadata)
+    return trial.TrialSuggestion(parameters=parameters, metadata=metadata)
 
   @classmethod
   def from_protos(
       cls, protos: Iterable[pythia_service_pb2.TrialSuggestion]
-  ) -> List[vz.TrialSuggestion]:
+  ) -> List[trial.TrialSuggestion]:
     """Convenience wrapper for from_proto."""
     return [cls.from_proto(proto) for proto in protos]
 
   @classmethod
   def to_protos(
-      cls, pytrials: Iterable[vz.TrialSuggestion]
+      cls, pytrials: Iterable[trial.TrialSuggestion]
   ) -> List[pythia_service_pb2.TrialSuggestion]:
     return [cls.to_proto(pytrial) for pytrial in pytrials]
 
   @classmethod
   def to_proto(
-      cls, suggestion: vz.TrialSuggestion
+      cls, suggestion: trial.TrialSuggestion
   ) -> pythia_service_pb2.TrialSuggestion:
     """Converts a pyvizier TrialSuggestion to the corresponding proto."""
     proto = pythia_service_pb2.TrialSuggestion()
 
     for name, value in suggestion.parameters.items():
       proto.parameters.append(ParameterValueConverter.to_proto(value, name))
 
@@ -726,34 +735,34 @@
 
 
 class MetadataDeltaConverter:
   """Converts pyvizier.MetadataDelta <--> List of UnitMetadataUpdate protos."""
 
   @classmethod
   def to_protos(
-      cls, delta: vz.MetadataDelta
+      cls, delta: trial.MetadataDelta
   ) -> List[vizier_service_pb2.UnitMetadataUpdate]:
     """Converts pyvizier.MetadataDelta to a List of UnitMetadataUpdate protos."""
     unit_metadata_updates = metadata_util.study_metadata_to_update_list(
         delta.on_study
     )
     unit_metadata_updates.extend(
         metadata_util.trial_metadata_to_update_list(delta.on_trials)
     )
     return unit_metadata_updates
 
   @classmethod
   def from_protos(
       cls, protos: Iterable[vizier_service_pb2.UnitMetadataUpdate]
-  ) -> vz.MetadataDelta:
+  ) -> trial.MetadataDelta:
     """Converts a list of UnitMetadataUpdate protos to pyvizier.MetadataDelta."""
-    mdd = vz.MetadataDelta()
+    mdd = trial.MetadataDelta()
     for u_m_u in protos:
       key_value = u_m_u.metadatum
-      namespace = vz.Namespace.decode(key_value.ns)
+      namespace = common.Namespace.decode(key_value.ns)
       value = (
           key_value.proto if key_value.HasField('proto') else key_value.value
       )
       if u_m_u.HasField('trial_id'):
         mdd.on_trials[int(u_m_u.trial_id)].abs_ns(namespace)[
             key_value.key
         ] = value
@@ -764,15 +773,15 @@
 
 class ProblemStatementConverter:
   """Converts pyvizier.ProblemStatement <-> Pythia ProblemStatement proto."""
 
   @classmethod
   def to_proto(
       cls,
-      problem_statement: vz.ProblemStatement,
+      problem_statement: base_study_config.ProblemStatement,
   ) -> pythia_service_pb2.ProblemStatement:
     """Converts PyVizier ProblemStatement to Proto version."""
     parameter_spec_protos = SearchSpaceConverter.parameter_protos(
         problem_statement.search_space
     )
     metric_information_protos = MetricsConfigConverter.to_protos(
         problem_statement.metric_information
@@ -785,23 +794,23 @@
         metric_information=metric_information_protos,
         metadata=keyvalue_protos,
     )
 
   @classmethod
   def from_proto(
       cls, proto: pythia_service_pb2.ProblemStatement
-  ) -> vz.ProblemStatement:
+  ) -> base_study_config.ProblemStatement:
     """Converts ProblemStatement Proto to PyVizier version."""
     study_spec = study_pb2.StudySpec(parameters=proto.search_space)
     search_space = SearchSpaceConverter.from_proto(study_spec)
     metric_information = MetricsConfigConverter.from_protos(
         proto.metric_information
     )
     metadata = metadata_util.from_key_value_list(proto.metadata)
-    return vz.ProblemStatement(
+    return base_study_config.ProblemStatement(
         search_space=search_space,
         metric_information=metric_information,
         metadata=metadata,
     )
 
 
 class StudyDescriptorConverter:
```

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/proto_converters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/study_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,32 +24,42 @@
   2) Can be initialized from an existing StudyConfig proto, to enable easy
      Pythonic accessors to information contained in StudyConfig protos,
      and easy field editing capabilities.
 
   * `SearchSpace` and `SearchSpaceSelector` classes deals with Vizier search
     spaces. Both flat spaces and conditional parameters are supported.
 """
+
 import collections
 import copy
 import enum
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import attr
-from vizier import pyvizier as vz
 from vizier._src.pyvizier.oss import automated_stopping
 from vizier._src.pyvizier.oss import metadata_util
 from vizier._src.pyvizier.oss import proto_converters
+from vizier._src.pyvizier.shared import base_study_config
+from vizier._src.pyvizier.shared import common
+from vizier._src.pyvizier.shared import parameter_config
+from vizier._src.pyvizier.shared import trial
 from vizier._src.service import constants
 from vizier._src.service import study_pb2
 
+
 ################### PyTypes ###################
 # Possible types for trial parameter values after cast to external types.
 # TODO: Define this in _src/shared/
-ParameterValueSequence = Union[vz.ParameterValueTypes, Sequence[int],
-                               Sequence[float], Sequence[str], Sequence[bool]]
+ParameterValueSequence = Union[
+    trial.ParameterValueTypes,
+    Sequence[int],
+    Sequence[float],
+    Sequence[str],
+    Sequence[bool],
+]
 
 ################### Enums ###################
 
 
 class Algorithm(enum.Enum):
   """Valid Values for StudyConfig.Algorithm."""
   # Let Vizier choose algorithm. Currently defaults to GAUSSIAN_PROCESS_BANDIT.
@@ -100,15 +110,15 @@
 #     study_config.metadata['metadata_key'] = 'metadata_value'
 #     new_proto = study_config.to_proto()
 #
 # (2) By directly calling __init__ and setting attributes:
 #     study_config = pyvizier.StudyConfig(
 #       metric_information=[pyvizier.MetricInformation(
 #         name='accuracy', goal=pyvizier.ObjectiveMetricGoal.MAXIMIZE)],
-#       search_space=SearchSpace.from_proto(proto),
+#       search_space=vz.SearchSpace.from_proto(proto),
 #     )
 #     # OR:
 #     study_config = pyvizier.StudyConfig()
 #     study_config.metric_information.append(
 #        pyvizier.MetricInformation(
 #          name='accuracy', goal=pyvizier.ObjectiveMetricGoal.MAXIMIZE))
 #
@@ -117,22 +127,23 @@
 #     root = study_config.search_space.root
 #     root.add_float_param('learning_rate', 0.001, 1.0,
 #       scale_type=pyvizier.ScaleType.LOG)
 #
 
 
 @attr.define(frozen=False, init=True, slots=True, kw_only=True)
-class StudyConfig(vz.ProblemStatement):
+class StudyConfig(base_study_config.ProblemStatement):
   """A builder and wrapper for study_pb2.StudySpec proto."""
 
-  search_space: vz.SearchSpace = attr.field(
+  search_space: parameter_config.SearchSpace = attr.field(
       init=True,
-      factory=vz.SearchSpace,
-      validator=attr.validators.instance_of(vz.SearchSpace),
-      on_setattr=attr.setters.validate)
+      factory=parameter_config.SearchSpace,
+      validator=attr.validators.instance_of(parameter_config.SearchSpace),
+      on_setattr=attr.setters.validate,
+  )
 
   algorithm: str = attr.field(
       init=True,
       validator=attr.validators.instance_of((Algorithm, str)),
       converter=lambda x: x.value if isinstance(x, enum.Enum) else x,
       on_setattr=[attr.setters.convert, attr.setters.validate],
       default='ALGORITHM_UNSPECIFIED',
@@ -142,20 +153,21 @@
       init=True,
       validator=attr.validators.optional(attr.validators.instance_of(str)),
       on_setattr=[attr.setters.convert, attr.setters.validate],
       default=None,
       kw_only=True)
 
   # TODO: This name/type combo is confusing.
-  metric_information: vz.MetricsConfig = attr.field(
+  metric_information: base_study_config.MetricsConfig = attr.field(
       init=True,
-      factory=vz.MetricsConfig,
-      converter=vz.MetricsConfig,
-      validator=attr.validators.instance_of(vz.MetricsConfig),
-      kw_only=True)
+      factory=base_study_config.MetricsConfig,
+      converter=base_study_config.MetricsConfig,
+      validator=attr.validators.instance_of(base_study_config.MetricsConfig),
+      kw_only=True,
+  )
 
   observation_noise: ObservationNoise = attr.field(
       init=True,
       validator=attr.validators.instance_of(ObservationNoise),
       on_setattr=attr.setters.validate,
       default=ObservationNoise.OBSERVATION_NOISE_UNSPECIFIED,
       kw_only=True)
@@ -166,36 +178,37 @@
           default=None,
           validator=attr.validators.optional(
               attr.validators.instance_of(
                   automated_stopping.AutomatedStoppingConfig)),
           on_setattr=attr.setters.validate,
           kw_only=True)
 
-  metadata: vz.Metadata = attr.field(
+  metadata: common.Metadata = attr.field(
       init=True,
       kw_only=True,
-      factory=vz.Metadata,
-      validator=attr.validators.instance_of(vz.Metadata),
-      on_setattr=[attr.setters.convert, attr.setters.validate])
+      factory=common.Metadata,
+      validator=attr.validators.instance_of(common.Metadata),
+      on_setattr=[attr.setters.convert, attr.setters.validate],
+  )
 
   # An internal representation as a StudyConfig proto.
   # If this object was created from a StudyConfig proto, a copy of the original
   # proto is kept, to make sure that unknown proto fields are preserved in
   # round trip serialization.
   # TODO: Fix the broken proto validation.
   _study_config: study_pb2.StudySpec = attr.field(
       init=True,
       factory=study_pb2.StudySpec,
       kw_only=True)
 
   # Public attributes, methods and properties.
   @classmethod
-  def pythia_endpoint_metadata(cls, pythia_endpoint: str) -> vz.Metadata:
+  def pythia_endpoint_metadata(cls, pythia_endpoint: str) -> common.Metadata:
     """Returns the MetaData for updating the pythia endpoint."""
-    metadata = vz.Metadata()
+    metadata = common.Metadata()
     metadata.ns(constants.PYTHIA_ENDPOINT_NAMESPACE)[
         constants.PYTHIA_ENDPOINT_KEY
     ] = pythia_endpoint
     return metadata
 
   @classmethod
   def from_proto(cls, proto: study_pb2.StudySpec) -> 'StudyConfig':
@@ -205,35 +218,39 @@
       proto: StudyConfig proto.
 
     Returns:
       A StudyConfig object.
     """
     algorithm = proto.algorithm
 
-    metric_information = vz.MetricsConfig(
-        sorted([
-            proto_converters.MetricInformationConverter.from_proto(m)
-            for m in proto.metrics
-        ],
-               key=lambda x: x.name))
+    metric_information = base_study_config.MetricsConfig(
+        sorted(
+            [
+                proto_converters.MetricInformationConverter.from_proto(m)
+                for m in proto.metrics
+            ],
+            key=lambda x: x.name,
+        )
+    )
 
     oneof_name = proto.WhichOneof('automated_stopping_spec')
     if not oneof_name:
       automated_stopping_config = None
     else:
       automated_stopping_config = (
           automated_stopping.AutomatedStoppingConfig.from_proto(
               getattr(proto, oneof_name)
           )
       )
 
-    metadata = vz.Metadata()
+    metadata = common.Metadata()
     for kv in proto.metadata:
-      metadata.abs_ns(vz.Namespace.decode(kv.ns))[kv.key] = (
-          kv.proto if kv.HasField('proto') else kv.value)
+      metadata.abs_ns(common.Namespace.decode(kv.ns))[kv.key] = (
+          kv.proto if kv.HasField('proto') else kv.value
+      )
 
     # Store the pythia_endpoint as a property for convenience.
     pythia_endpoint = None
     try:
       pythia_endpoint = metadata.ns(constants.PYTHIA_ENDPOINT_NAMESPACE)[
           constants.PYTHIA_ENDPOINT_KEY
       ]
@@ -276,39 +293,41 @@
     proto.ClearField('metadata')
     for ns in self.metadata.namespaces():
       ns_string = ns.encode()
       ns_layer = self.metadata.abs_ns(ns)
       for key, value in ns_layer.items():
         metadata_util.assign(proto, key=key, ns=ns_string, value=value)
     if self.pythia_endpoint is not None:
-      ns = vz.Namespace([constants.PYTHIA_ENDPOINT_NAMESPACE])
+      ns = common.Namespace([constants.PYTHIA_ENDPOINT_NAMESPACE])
       metadata_util.assign(
           proto,
           key=constants.PYTHIA_ENDPOINT_KEY,
           ns=ns.encode(),
           value=self.pythia_endpoint,
           mode='insert_or_assign',
       )
     return proto
 
   def _trial_to_external_values(
-      self, pytrial: vz.Trial) -> Dict[str, Union[float, int, str, bool]]:
+      self, pytrial: trial.Trial
+  ) -> Dict[str, Union[float, int, str, bool]]:
     """Returns the trial paremeter values cast to external types."""
     parameter_values: Dict[str, Union[float, int, str]] = {}
     external_values: Dict[str, Union[float, int, str, bool]] = {}
     # parameter_configs is a list of Tuple[parent_name, ParameterConfig].
-    parameter_configs: List[Tuple[Optional[str], vz.ParameterConfig]] = [
-        (None, p) for p in self.search_space.parameters
-    ]
+    parameter_configs: List[
+        Tuple[Optional[str], parameter_config.ParameterConfig]
+    ] = [(None, p) for p in self.search_space.parameters]
     remaining_parameters = copy.deepcopy(pytrial.parameters)
     # Traverse the conditional tree using a BFS.
     while parameter_configs and remaining_parameters:
       parent_name, pc = parameter_configs.pop(0)
       parameter_configs.extend(
-          (pc.name, child) for child in pc.child_parameter_configs)
+          (pc.name, child) for child in pc.child_parameter_configs
+      )
       if pc.name not in remaining_parameters:
         continue
       if parent_name is not None:
         # This is a child parameter. If the parent was not seen,
         # skip this parameter config.
         if parent_name not in parameter_values:
           continue
@@ -340,15 +359,16 @@
       ValueError: If the trial parameters do not exist in this search space.
       ValueError: If the trial contains duplicate parameters.
     """
     pytrial = proto_converters.TrialConverter.from_proto(proto)
     return self._pytrial_parameters(pytrial)
 
   def _pytrial_parameters(
-      self, pytrial: vz.Trial) -> Dict[str, ParameterValueSequence]:
+      self, pytrial: trial.Trial
+  ) -> Dict[str, ParameterValueSequence]:
     """Returns the trial values, cast to external types, if they exist.
 
     Args:
       pytrial:
 
     Returns:
       Parameter values dict: cast to each parameter's external_type, if exists.
@@ -366,16 +386,16 @@
                        'all trial parameters: {}'.format(pytrial))
 
     # Combine multi-dimensional parameter values to a list of values.
     trial_final_values: Dict[str, ParameterValueSequence] = {}
     # multi_dim_params: Dict[str, List[Tuple[int, ParameterValueSequence]]]
     multi_dim_params = collections.defaultdict(list)
     for name in trial_external_values:
-      base_index = (
-          vz.SearchSpaceSelector.parse_multi_dimensional_parameter_name(name)
+      base_index = parameter_config.SearchSpaceSelector.parse_multi_dimensional_parameter_name(
+          name
       )
       if base_index is None:
         trial_final_values[name] = trial_external_values[name]
       else:
         base_name, index = base_index
         multi_dim_params[base_name].append((index, trial_external_values[name]))
     for name in multi_dim_params:
@@ -403,18 +423,17 @@
     Returns:
       Dict[metric name, metric value]
     """
     pytrial = proto_converters.TrialConverter.from_proto(proto)
     return self._pytrial_metrics(
         pytrial, include_all_metrics=include_all_metrics)
 
-  def _pytrial_metrics(self,
-                       pytrial: vz.Trial,
-                       *,
-                       include_all_metrics=False) -> Dict[str, float]:
+  def _pytrial_metrics(
+      self, pytrial: trial.Trial, *, include_all_metrics=False
+  ) -> Dict[str, float]:
     """Returns the trial's final measurement metric values.
 
     If the trial is not completed, or infeasible, no metrics are returned.
     By default, only metrics configured in the StudyConfig are returned
     (e.g. only objective and safety metrics).
 
     Args:
```

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/oss/study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/pythia/study.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/pythia/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/base_study_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,16 @@
 
     Avoids the common pitfalls of using
       `metric.min_value or default_value`
     which would incorrectly use the default_value when min_value == 0, and
     requires default_value to have been computed.
 
     Args:
-      default_value_fn: Default value if min_value is not finite.
+      default_value_fn: Default value if min_value is not finite. This function
+        does not run at all if min_value is finite.
     """
     if np.isfinite(self.min_value):
       return self.min_value
     else:
       return default_value_fn()
 
   def max_value_or(self, default_value_fn: Callable[[], float]) -> float:
@@ -185,15 +186,16 @@
 
     Avoids the common pitfalls of using
       `metric.max_value or default_value`
     which would incorrectly use the default_value when max_value == 0, and
     requires default_value to have been computed.
 
     Args:
-      default_value_fn: Default value if max_value is not configured.
+      default_value_fn: Default value if max_value is not finite. This function
+        does not run at all if max_value is configured.
     """
     if np.isfinite(self.max_value):
       return self.max_value
     else:
       return default_value_fn()
 
   @property
```

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/base_study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/common.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
 from absl import logging
 import attr
 
 from google.protobuf import any_pb2
 from google.protobuf.message import Message
 
-M = TypeVar('M', bound=Message)
+_M = TypeVar('_M', bound=Message)
 T = TypeVar('T')
 T1 = TypeVar('T1')
 T2 = TypeVar('T2')
 MetadataValue = Union[str, any_pb2.Any, Message]
+_V = TypeVar('_V', bound=MetadataValue)
 
 # Namespace Encoding.
 #
 # By definition, ∀ ns ∈ Namespace, Namespace.decode(ns.encode()) == ns.
 # The tricky part of that definition is handling namespaces with components
 # that are empty strings.  Notably, we want to make sure that
 # Namespace(()).encode() != Namespace(('',)).encode().
@@ -394,16 +395,19 @@
         ', '.join(itemlist), self._namespace.encode()
     )
 
   def __str__(self) -> str:
     """Prints items in the current namespace."""
     return 'namespace: {} items: {}'.format(str(self._namespace), self._store)
 
-  def get_proto(self, key: str, *, cls: Type[M]) -> Optional[M]:
+  def get_proto(self, key: str, *, cls: Type[_M]) -> Optional[_M]:
     """Deprecated: use get() instead."""
+    logging.warning(
+        'Metadata.get_proto() is deprecated, prefer Metadata.get().'
+    )
     value = self._store.get(key, None)
     if value is None:
       return None
 
     if isinstance(value, cls):
       # Starting from 3.10, pytype supports typeguard, which obsoletes
       # the need for the `pytype:disable` clause.
@@ -569,14 +573,30 @@
     Yields:
       Tuple of (namespace, key, value).
     """
     for ns in self.namespaces():
       for k, v in self.abs_ns(ns).items():
         yield (ns, k, v)
 
+  def items_by_cls(self, *, cls: Type[_V]) -> Iterator[Tuple[str, _V]]:
+    """Yields an iterator over items whose type=$cls in the current namespace.
+
+    This iterates through the metadata items in the current namespace, like
+    __iter__(), except that it only returns items of the specified type.
+
+    Args:
+      cls: What type of objects to filter for?
+
+    Yields:
+      Tuple of (key, value).
+    """
+    for k_v in self.items():
+      if isinstance(k_v[1], cls):
+        yield k_v
+
   # START OF abstract methods inherited from `MutableMapping` base class.
   def __getitem__(self, key: str) -> MetadataValue:
     return self._store.__getitem__(key)
 
   def __setitem__(self, key: str, value: MetadataValue):
     self._store[key] = value
```

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/common_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/common_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,10 +373,22 @@
     m3 = common.Metadata()
     m3['foo'] = 'Y'  # This will be overwritten.
     m3['z'] = 'Z'  # This will not be overwritten.
     m3.attach(mm.ns('ns1').ns('ns:11'))
     self.assertEqual(m3['z'], 'Z')
     self.assertEqual(m3['foo'], 'bar')
 
+  def test_metadata_items_by_cls(self):
+    mm = common.Metadata(foo='bar', nerf='gleep')
+    mm['aaa'] = duration_pb2.Duration(seconds=5)
+    mm.ns('ns1')['foo'] = 'bar1'
+    test1 = list(sorted(mm.items_by_cls(cls=str)))
+    self.assertLen(test1, 2)
+    self.assertEqual(test1[0], ('foo', 'bar'))
+    self.assertEqual(test1[1], ('nerf', 'gleep'))
+    test2 = list(sorted(mm.items_by_cls(cls=duration_pb2.Duration)))
+    self.assertLen(test2, 1)
+    self.assertEqual(test2[0][1].seconds, 5)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/context.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/context.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/context_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/context_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """ParameterConfig wraps ParameterConfig and ParameterSpec protos."""
 
 import collections
-from typing import Sized, Collection, Set as AbstractSet
+from typing import Collection, Set as AbstractSet, Sized
 import copy
 import enum
 import json
 import math
 import re
 from typing import Generator, Iterator, List, Optional, Sequence, Tuple, Union, overload
 
@@ -747,15 +747,15 @@
     spaces = []
     for value in values:
       for config in self._selected:
         spaces.append(config.subspace(value))
     return SearchSpaceSelector(spaces)
 
 
-class InvalidParameterError(Exception):
+class InvalidParameterError(ValueError):
   """Error thrown when parameter values are invalid."""
 
 
 ################### Main Classes ###################
 SearchSpaceOrSpaces = Union['SearchSpace', Collection['SearchSpace']]
 
 
@@ -904,16 +904,16 @@
       name: The parameter's name. Cannot be empty.
       feasible_values: The set of feasible values for this parameter.
       default_value: A default value for the Parameter.
       scale_type: Scaling to be applied. NOT VALIDATED.
       index: Specifies the multi-dimensional index for this parameter. E.g. if
         name='batch_size' and index=0, then a single ParameterConfig with name
         'batch_size[0]' is added. `index` should be >= 0.
-      auto_cast: If False, the external type will be set to INTEGER if all
-        values are castable to an integer without losing precision. If True, the
+      auto_cast: If True, the external type will be set to INTEGER if all values
+        are castable to an integer without losing precision. If False, the
         external type will be set to float.
       experimental_fidelity_config: EXPERIMENTAL. See FidelityConfig doc.
 
     Returns:
       ParameterConfigSelector for the newly added parameter(s).
 
     Raises:
```

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_iterators.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/parameter_iterators_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/study.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/trial.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial_test.py` & `google-vizier-0.1.6/vizier/_src/pyvizier/shared/trial_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/raytune/converters.py` & `google-vizier-0.1.6/vizier/_src/raytune/vizier_search_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,63 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Converters for PyVizier with RayTune."""
-
-from typing import Any, Dict, Callable
-
+"""Test for VizierSearch. Cannot be tested internally but can be on GitHub."""
 from ray import tune
-from vizier import pyvizier as vz
+from vizier._src.raytune import converters
+from vizier._src.raytune import vizier_search
 from vizier.benchmarks import experimenters
+from vizier.service import clients
+from vizier.service import pyvizier as vz
+
+from absl.testing import absltest
+
+
+# Required to use local Vizier service.
+clients.environment_variables.servicer_use_sql_ram()
 
 
-class SearchSpaceConverter:
-  """Converts pyvizier.SearchSpace <-> RayTune Search Space."""
+class VizierSearchTest(absltest.TestCase):
+
+  def test_search_with_study_config(self):
+    dim = 4
+    bbob_factory = experimenters.BBOBExperimenterFactory(name='Sphere', dim=dim)
+    exptr = bbob_factory()
+
+    study_config = vz.StudyConfig.from_problem(exptr.problem_statement())
+    study_config.algorithm = 'RANDOM_SEARCH'
+    self.assertLen(study_config.search_space.parameters, dim)
+    searcher = vizier_search.VizierSearch('test study', study_config)
+
+    trainable = converters.ExperimenterConverter.to_callable(exptr)
+    tuner = tune.Tuner(
+        trainable,
+        param_space=None,
+        tune_config=tune.TuneConfig(num_samples=10, search_alg=searcher),
+    )
+    tuner.fit()
+    self.assertLen(tuner.get_results(), 10)
+
+  def test_search_with_ray_search_space(self):
+    dim = 4
+    bbob_factory = experimenters.BBOBExperimenterFactory(name='Sphere', dim=dim)
+    exptr = bbob_factory()
+
+    trainable = converters.ExperimenterConverter.to_callable(exptr)
+    tuner = tune.Tuner(
+        trainable,
+        param_space=None,
+        tune_config=tune.TuneConfig(
+            num_samples=10, search_alg=vizier_search.VizierSearch()
+        ),
+    )
+    tuner.fit()
+    self.assertLen(tuner.get_results(), 10)
 
-  @classmethod
-  def to_dict(
-      cls,
-      search_space: vz.SearchSpace,
-  ) -> Dict[str, Any]:
-    """Converts PyVizier ProblemStatement to Proto version."""
-    param_space = {}
-
-    for param in search_space.parameters:
-      if param.type == vz.ParameterType.DOUBLE:
-        lower, upper = param.bounds
-        if param.scale_type == vz.ScaleType.LINEAR:
-          param_space[param.name] = tune.uniform(lower, upper)
-        elif param.scale_type == vz.ScaleType.LOG:
-          param_space[param.name] = tune.loguniform(lower, upper)
-        else:
-          raise ValueError(f'DOUBLE scale {param.scale_type} not supported.')
-      elif param.type == vz.ParameterType.INTEGER:
-        lower, upper = param.bounds
-        param_space[param.name] = tune.randint(lower, upper)
-      else:
-        feasible_values = param.feasible_values
-        param_space[param.name] = tune.choice(feasible_values)
-    return param_space
-
-
-class ExperimenterConverter:
-  """Converts Experimenters to Ray Trainables."""
-
-  @classmethod
-  def to_callable(
-      cls,
-      experimenter: experimenters.Experimenter,
-  ) -> Callable[[vz.ParameterDict], Dict[str, float]]:
-    """Returns a callable that takes Parameters and returns metric values."""
-
-    def trainable(config: vz.ParameterDict) -> Dict[str, float]:
-      trial = vz.Trial(parameters=config)
-      experimenter.evaluate([trial])
-      if trial.final_measurement is None:
-        raise ValueError(f'No final_measurement on trial{trial.id}')
-      return {k: v.value for k, v in trial.final_measurement.metrics.items()}
 
-    return trainable
+if __name__ == '__main__':
+  absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/_src/raytune/run_tune.py` & `google-vizier-0.1.6/vizier/_src/raytune/run_tune.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/raytune/run_tune_test.py` & `google-vizier-0.1.6/vizier/_src/raytune/run_tune_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+"""Github test for run_tune."""
+# pytype: skip-file
 import itertools
 
 import numpy as np
 from ray import tune
 from vizier._src.raytune import run_tune
 
 from absl.testing import absltest
```

### Comparing `google-vizier-0.1.5/vizier/_src/service/clients.py` & `google-vizier-0.1.6/vizier/_src/service/clients.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/clients_test.py` & `google-vizier-0.1.6/vizier/_src/service/clients_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/constants.py` & `google-vizier-0.1.6/vizier/_src/service/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/custom_errors.py` & `google-vizier-0.1.6/vizier/_src/service/custom_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/datastore.py` & `google-vizier-0.1.6/vizier/_src/service/datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/datastore_test_lib.py` & `google-vizier-0.1.6/vizier/_src/service/datastore_test_lib.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/grpc_util.py` & `google-vizier-0.1.6/vizier/_src/service/grpc_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/performance_test.py` & `google-vizier-0.1.6/vizier/_src/service/performance_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/policy_factory.py` & `google-vizier-0.1.6/vizier/_src/service/policy_factory.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/pythia_service.py` & `google-vizier-0.1.6/vizier/_src/service/pythia_service.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/pythia_util.py` & `google-vizier-0.1.6/vizier/_src/service/pythia_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/ram_datastore.py` & `google-vizier-0.1.6/vizier/_src/service/ram_datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/ram_datastore_test.py` & `google-vizier-0.1.6/vizier/_src/service/ram_datastore_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/resources.py` & `google-vizier-0.1.6/vizier/_src/service/resources.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/resources_test.py` & `google-vizier-0.1.6/vizier/_src/service/resources_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/service_policy_supporter.py` & `google-vizier-0.1.6/vizier/_src/service/service_policy_supporter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/service_policy_supporter_test.py` & `google-vizier-0.1.6/vizier/_src/service/service_policy_supporter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/sql_datastore.py` & `google-vizier-0.1.6/vizier/_src/service/sql_datastore.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/sql_datastore_test.py` & `google-vizier-0.1.6/vizier/_src/service/sql_datastore_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/stubs_util.py` & `google-vizier-0.1.6/vizier/_src/service/stubs_util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/stubs_util_test.py` & `google-vizier-0.1.6/vizier/_src/service/stubs_util_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/testing/util.py` & `google-vizier-0.1.6/vizier/_src/service/testing/util.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/types.py` & `google-vizier-0.1.6/vizier/_src/service/types.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/vizier_client.py` & `google-vizier-0.1.6/vizier/_src/service/vizier_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,27 +39,35 @@
 from vizier.service import pyvizier
 from vizier.utils import attrs_utils
 
 from google.longrunning import operations_pb2
 from google.protobuf import duration_pb2
 from google.protobuf import json_format
 
-flags.DEFINE_integer(
+_VIZIER_NEW_SUGGESTION_POLLING_SECONDS = flags.DEFINE_integer(
     'vizier_new_suggestion_polling_secs',
     1,
     (
         'The period to wait between polling for the status of long-running '
         'SuggestOperations. Vizier may increase this period if multiple polls '
         'are needed. (You may use zero for interactive demos, but it is only '
         'appropriate for very small Studies.)'
     ),
 )
 FLAGS = flags.FLAGS
 
 
+# TODO: Add an e2e test for this.
+def _get_new_suggestion_polling_secs() -> int:
+  if FLAGS.is_parsed():
+    return _VIZIER_NEW_SUGGESTION_POLLING_SECONDS.value
+  else:
+    return int(_VIZIER_NEW_SUGGESTION_POLLING_SECONDS.default)
+
+
 @attr.define
 class _EnvironmentVariables:
   server_endpoint: str = attr.field(
       default=constants.NO_ENDPOINT, validator=attr.validators.instance_of(str)
   )
   servicer_kwargs: Dict[str, Any] = attr.field(factory=dict)
 
@@ -161,15 +169,15 @@
       if rpc_error.code() == grpc.StatusCode.FAILED_PRECONDITION:  # pytype:disable=attribute-error
         return []
       raise rpc_error
 
     num_attempts = 0
     while not operation.done:
       sleep_time = PollingDelay(
-          num_attempts, FLAGS.vizier_new_suggestion_polling_secs
+          num_attempts, _get_new_suggestion_polling_secs()
       )
       num_attempts += 1
       logging.info(
           'Waiting for operation with name %s to be done', operation.name
       )
       time.sleep(sleep_time.total_seconds())
```

### Comparing `google-vizier-0.1.5/vizier/_src/service/vizier_client_test.py` & `google-vizier-0.1.6/vizier/_src/service/vizier_client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 # TODO: Rewrite using RPC calls and remove all direct lookups
 # into the datastore.
 # TODO: Cover delete_trial, delete_study, get_study_config, and
 # add_trial, OR turn it into a private module
 
 from typing import List
-from absl import logging
 
+from absl import logging
 from vizier._src.service import constants
 from vizier._src.service import resources
 from vizier._src.service import study_pb2
 from vizier._src.service import vizier_client
 from vizier._src.service import vizier_server
 from vizier._src.service import vizier_service_pb2_grpc
 from vizier.service import pyvizier
@@ -216,25 +216,26 @@
     )
     self.assertLen(suggestions_list, suggestion_count)
     logging.info('Suggestions List: %s', suggestions_list)
 
   # Only test algorithms which don't depend on external libraries (except for
   # numpy).
   @parameterized.parameters(
-      (pyvizier.Algorithm.RANDOM_SEARCH, 50, 1, False),
-      (pyvizier.Algorithm.QUASI_RANDOM_SEARCH, 50, 1, False),
-      (pyvizier.Algorithm.GRID_SEARCH, 50, 1, False),
-      (pyvizier.Algorithm.NSGA2, 50, 1, True),
+      dict(algorithm=pyvizier.Algorithm.RANDOM_SEARCH),
+      dict(algorithm=pyvizier.Algorithm.QUASI_RANDOM_SEARCH),
+      dict(algorithm=pyvizier.Algorithm.GRID_SEARCH),
+      dict(algorithm=pyvizier.Algorithm.NSGA2, multi_objective=True),
   )
   def test_e2e_tuning(
       self,
+      *,
       algorithm,
-      num_iterations: int,
-      batch_size: int,
-      multi_objective: bool,
+      num_iterations: int = 50,
+      batch_size: int = 1,
+      multi_objective: bool = False,
   ):
     # Runs end-to-end tuning via back-and-forth communication to server.
     def learning_curve_generator(learning_rate: float) -> List[float]:
       return [learning_rate * step for step in range(10)]
 
     study_config = pyvizier.StudyConfig()
     study_config.search_space.root.add_float_param(
```

### Comparing `google-vizier-0.1.5/vizier/_src/service/vizier_server.py` & `google-vizier-0.1.6/vizier/_src/service/vizier_server.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/vizier_service.py` & `google-vizier-0.1.6/vizier/_src/service/vizier_service.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/_src/service/vizier_service_test.py` & `google-vizier-0.1.6/vizier/_src/service/vizier_service_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/algorithms/__init__.py` & `google-vizier-0.1.6/vizier/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/algorithms/designers/__init__.py` & `google-vizier-0.1.6/vizier/algorithms/designers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""List of Designers."""
+"""List of Designers and related algorithms."""
+
 from vizier._src.algorithms.designers.bocs import BOCSDesigner
 from vizier._src.algorithms.designers.cmaes import CMAESDesigner
 from vizier._src.algorithms.designers.eagle_strategy.eagle_strategy import EagleStrategyDesigner
 from vizier._src.algorithms.designers.emukit import EmukitDesigner
 from vizier._src.algorithms.designers.gp_bandit import VizierGPBandit
 from vizier._src.algorithms.designers.grid import GridSearchDesigner
 from vizier._src.algorithms.designers.harmonica import HarmonicaDesigner
```

### Comparing `google-vizier-0.1.5/vizier/algorithms/policies/__init__.py` & `google-vizier-0.1.6/vizier/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/benchmarks/__init__.py` & `google-vizier-0.1.6/vizier/benchmarks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Benchmarking utilities."""
+
+from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceComparatorBase
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurve
-from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurveComparator
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurveConverter
 from vizier._src.benchmarks.analyzers.convergence_curve import HypervolumeCurveConverter
+from vizier._src.benchmarks.analyzers.convergence_curve import LogEfficiencyConvergenceCurveComparator
+from vizier._src.benchmarks.analyzers.convergence_curve import PercentageBetterConvergenceCurveComparator
 from vizier._src.benchmarks.analyzers.state_analyzer import BenchmarkStateAnalyzer
 from vizier._src.benchmarks.runners.benchmark_runner import BenchmarkRunner
 from vizier._src.benchmarks.runners.benchmark_runner import BenchmarkSubroutine
 from vizier._src.benchmarks.runners.benchmark_runner import EvaluateActiveTrials
 from vizier._src.benchmarks.runners.benchmark_runner import FillActiveTrials
 from vizier._src.benchmarks.runners.benchmark_runner import GenerateAndEvaluate
 from vizier._src.benchmarks.runners.benchmark_runner import GenerateSuggestions
```

### Comparing `google-vizier-0.1.5/vizier/benchmarks/experimenters/__init__.py` & `google-vizier-0.1.6/vizier/benchmarks/experimenters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 from vizier._src.benchmarks.experimenters.combo_experimenter import IsingExperimenter
 from vizier._src.benchmarks.experimenters.combo_experimenter import MAXSATExperimenter
 from vizier._src.benchmarks.experimenters.combo_experimenter import PestControlExperimenter
 from vizier._src.benchmarks.experimenters.discretizing_experimenter import DiscretizingExperimenter
 from vizier._src.benchmarks.experimenters.experimenter import Experimenter
 from vizier._src.benchmarks.experimenters.experimenter_factory import BBOBExperimenterFactory
 from vizier._src.benchmarks.experimenters.experimenter_factory import ExperimenterFactory
+from vizier._src.benchmarks.experimenters.experimenter_factory import SerializableExperimenterFactory
 from vizier._src.benchmarks.experimenters.experimenter_factory import SingleObjectiveExperimenterFactory
 from vizier._src.benchmarks.experimenters.l1_categorical_experimenter import L1CategorialExperimenter
 from vizier._src.benchmarks.experimenters.multiobjective_experimenter import MultiObjectiveExperimenter
 from vizier._src.benchmarks.experimenters.noisy_experimenter import NoisyExperimenter
 from vizier._src.benchmarks.experimenters.normalizing_experimenter import NormalizingExperimenter
 from vizier._src.benchmarks.experimenters.numpy_experimenter import NumpyExperimenter
 from vizier._src.benchmarks.experimenters.shifting_experimenter import ShiftingExperimenter
 from vizier._src.benchmarks.experimenters.sign_flip_experimenter import SignFlipExperimenter
 from vizier._src.benchmarks.experimenters.sparse_experimenter import SparseExperimenter
 from vizier._src.benchmarks.experimenters.surrogate_experimenter import PredictorExperimenter
+from vizier._src.benchmarks.experimenters.switch_experimenter import SwitchExperimenter
 from vizier._src.benchmarks.experimenters.synthetic import bbob
```

### Comparing `google-vizier-0.1.5/vizier/benchmarks/experimenters/hpo/__init__.py` & `google-vizier-0.1.6/vizier/benchmarks/experimenters/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/benchmarks/experimenters/nas/__init__.py` & `google-vizier-0.1.6/vizier/benchmarks/experimenters/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/benchmarks/experimenters/rl/__init__.py` & `google-vizier-0.1.6/vizier/benchmarks/experimenters/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/client/__init__.py` & `google-vizier-0.1.6/vizier/client/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/client/client_abc.py` & `google-vizier-0.1.6/vizier/client/client_abc.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/client/client_abc_testing.py` & `google-vizier-0.1.6/vizier/client/client_abc_testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/interfaces/__init__.py` & `google-vizier-0.1.6/vizier/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/interfaces/serializable.py` & `google-vizier-0.1.6/vizier/interfaces/serializable.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/jax/__init__.py` & `google-vizier-0.1.6/vizier/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/jax/models.py` & `google-vizier-0.1.6/vizier/jax/models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/jax/optimizers.py` & `google-vizier-0.1.6/vizier/jax/optimizers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyglove/__init__.py` & `google-vizier-0.1.6/vizier/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pythia.py` & `google-vizier-0.1.6/vizier/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/__init__.py` & `google-vizier-0.1.6/vizier/pyvizier/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from __future__ import annotations
 
 """PyVizier classes for general use.
 
 Contains API shared across all platforms (Internal, Cloud, OSS).
 """
 
+from vizier._src.pyvizier.oss.study_config import ParameterValueSequence
 from vizier._src.pyvizier.pythia.study import StudyDescriptor
 from vizier._src.pyvizier.pythia.study import StudyState
 from vizier._src.pyvizier.pythia.study import StudyStateInfo
 from vizier._src.pyvizier.shared.base_study_config import MetricInformation
 from vizier._src.pyvizier.shared.base_study_config import MetricsConfig
 from vizier._src.pyvizier.shared.base_study_config import MetricType
 from vizier._src.pyvizier.shared.base_study_config import ObjectiveMetricGoal
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/__init__.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 from vizier.pyvizier.converters.core import ModelOutputConverter
 from vizier.pyvizier.converters.core import NumpyArraySpec
 from vizier.pyvizier.converters.core import NumpyArraySpecType
 from vizier.pyvizier.converters.core import STUDY_ID_FIELD
 from vizier.pyvizier.converters.core import TrialToArrayConverter
 from vizier.pyvizier.converters.core import TrialToNumpyDict
 from vizier.pyvizier.converters.embedder import ProblemAndTrialsScaler
-from vizier.pyvizier.converters.feature_mapper import ContinuousCategoricalFeatureMapper
+from vizier.pyvizier.converters.padded_trial_to_array_converter import PaddedTrialToArrayConverter
 from vizier.pyvizier.converters.spatio_temporal import DenseSpatioTemporalConverter
 from vizier.pyvizier.converters.spatio_temporal import SparseSpatioTemporalConverter
 from vizier.pyvizier.converters.spatio_temporal import TimedLabels
 from vizier.pyvizier.converters.spatio_temporal import TimedLabelsExtractor
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/core.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,15 +619,24 @@
     values = [value_converter(t) for t in trials]
     array = np.asarray(values, dtype=self._getter_spec.dtype).reshape([-1, 1])
     return self.onehot_encoder.forward_fn(self.scaler.forward_fn(array))
 
   def _to_parameter_value(
       self, value: Union['np.float', float, int]
   ) -> Optional[pyvizier.ParameterValue]:
-    """Converts to a single parameter value; see to_parameter_values()."""
+    """Converts to a single parameter value; see to_parameter_values().
+
+    Be aware that the value is automatically truncated.
+
+    Args:
+      value:
+
+    Returns:
+      ParameterValue.
+    """
     # TODO: NaNs and out-of-vocab values should return None instead
     # of raising an error.
     if not self._converts_to_parameter:
       return None
     if self.parameter_config.type == pyvizier.ParameterType.DOUBLE:
       # Input parameter was DOUBLE. Output is also DOUBLE.
       return pyvizier.ParameterValue(
@@ -1195,38 +1204,42 @@
   have functions that return shape or metric informations. Use it at your own
   risk.
   """
 
   _experimental_override = 'I am aware that this code may break at any point.'
 
   def __init__(
-      self, impl: DefaultTrialConverter, experimental_override: str = ''
+      self,
+      impl: DefaultTrialConverter,
+      experimental_override: str = '',
   ):
     """SHOULD NOT BE USED! Use factory classmethods e.g. from_study_config."""
 
     if experimental_override != self._experimental_override:
       raise ValueError(
           'Set "experimental_override" if you want to call __init__ directly. '
           'Otherwise, use TrialToArrayConverter.from_study_config.'
       )
     self._impl = impl
 
   def to_features(self, trials) -> np.ndarray:
-    """Returns the labels array with dimenion: (n_trials, n_features)."""
+    """Returns the features array with dimension: (n_trials, n_features)."""
     return dict_to_array(self._impl.to_features(trials))
 
   def to_labels(self, trials) -> np.ndarray:
     """Returns the labels array with dimenion: (n_trials, n_metrics)."""
+    # Pad up the labels.
     return dict_to_array(self._impl.to_labels(trials))
 
   def to_xy(self, trials) -> Tuple[np.ndarray, np.ndarray]:
     return self.to_features(trials), self.to_labels(trials)
 
   def to_parameters(self, arr: np.ndarray) -> Sequence[pyvizier.ParameterDict]:
     """Convert to nearest feasible parameter value. NaNs are preserved."""
+    # TODO: Add a boolean flag to diable automatic clipping.
     arrformat = DictOf2DArrays(self._impl.to_features([]))
     return self._impl.to_parameters(arrformat.dict_like(arr))
 
   @classmethod
   def from_study_config(
       cls,
       study_config: pyvizier.ProblemStatement,
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/core_test.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 Trial = pyvizier.Trial
 
 
-class TrialToArrayConverterTest(absltest.TestCase):
+class TrialToArrayConverterTest(parameterized.TestCase):
   """Test TrialToArrayConverter class."""
 
   def setUp(self):
     super().setUp()
     self._study_config = pyvizier.ProblemStatement(
         search_space=test_studies.flat_space_with_all_types(),
         metric_information=[
@@ -47,15 +47,15 @@
 
     self._designer = random.RandomDesigner(
         self._study_config.search_space, seed=0
     )
     self._trials = test_runners.run_with_random_metrics(
         self._designer, self._study_config, iters=1, batch_size=10
     )
-    self.maxDiff = None  # pylint: disable=invalid-name
+    self.maxDiff = None
 
   def test_back_to_back_conversion(self):
     converter = core.TrialToArrayConverter.from_study_config(self._study_config)
     self.assertSequenceEqual(
         [t.parameters for t in self._trials],
         converter.to_parameters(converter.to_features(self._trials)),
     )
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/embedder.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/embedder.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/embedder_test.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/embedder_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/feature_mapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,26 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Mappers between different feature formats."""
 
-import collections
-
 import numpy as np
+from vizier._src.jax import types
 from vizier.pyvizier.converters import core
 
 
-# This namedtuple was copied from TFP to reduce dependency.
-ContinuousAndCategoricalValues = collections.namedtuple(
-    'ContinuousAndCategoricalValues', ['continuous', 'categorical']
-)
-
-
 class ContinuousCategoricalFeatureMapper:
   """Maps features from TrialToArrayConverter to ContinuousAndCategoricalValues.
 
   The class allows to separate the continuous features from the categorical
   features and organize them in an ContinuousAndCategoricalValues namedtuple.
 
   Naming convension:
@@ -70,62 +63,92 @@
         categorical_dims.append(spec.num_dimensions)
       elif spec.type == core.NumpyArraySpecType.DISCRETE:
         # There shouldn't be DISCRETE spec type as onehot_embed=True is the
         # default in TrialToArrayConverter, and DISCRETE parameters are either
         # converted to CONTINUOUS or ONEHOT_EMBEDDING.
         raise ValueError("DISCRETE spec type shouldn't exists.")
       else:
-        raise ValueError('Unexpected spec type %s!' % spec.type)
-    # Create shift array that contains the cumulative number of categorical
-    # dimensions until each categorical parameter such that the categorical
-    # parameter itself is not included, and therefore the padding and [0:-1].
-    # This array will be used to map between the onehot active bit (index) of
-    # each categorical parameter to respective integer categorical value.
+        raise ValueError("Unexpected spec type %s!" % spec.type)
+    # Create shift array containing the cumulative number of categorical
+    # dimensions until each categorical parameter (itself not included). One-hot
+    # active bit (index) is mapped to integer value, by subtracting 'shift'.
     # For example, if categorical_dims=[3, 2], then cumsum(pad(..)) will
-    # generate [0, 3, 5], so shift will be [0, 3].
+    # generate [0, 3, 5], so 'shift' will be [0, 3].
     self.shift = np.cumsum(np.pad(categorical_dims, (1, 0)))[0:-1]  # (P,)
+    self.categorical_dims = categorical_dims
+    self.converter = converter
 
-  def map(self, features: np.ndarray) -> ContinuousAndCategoricalValues:
+  def map(self, features: np.ndarray) -> types.ContinuousAndCategoricalArray:
     """Split features by 'continuous' and 'categorical'.
 
     In addition to splitting the method converts the one-hot encoding
     categorical features to integer indices.
 
     For example, if the search space is:
       - categorical parameter C1 with values ['a', 'b', 'c].
       - continuous parameter F1.
       - categorical parameter C2 with values ['x', 'y'].
 
     Then for input parameters C1='b', F1=0.23, C2='y' and associated features:
     [[0, 1, 0, 0.23, 0, 1]] the result would be:
     ContinuousAndCategoricalValues(
         continuous=[[0.23]]
-        categorical=[[1,1]])
+        categorical=[[1, 1]])
 
     Arguments:
-      features: Numpy array (trials_num, feature_count) which is the output of
+      features: Numpy array (n_trials, n_features) which is the output of
         'to_features' method.
 
     Returns:
       namedtuple with continuous features and categorical integer indices.
     """
     # Split features to continuous and categorical.
     continuous_features = features[:, self._continuous_indices]  # (B,C)
     # Assign empty array as the default value.
     categorical_index_features = np.zeros((features.shape[0], 0))
     if self._n_categorical_params > 0:
       categorical_features = features[:, self._categorical_indices]  # (B,F)
       # Find the non-zero column indices associated with categorical parameters.
-      # For example (cont. from above), with the input of [0, 1, 0, 0.23, 0, 1]
+      # For example (cont. from above), with the input of [0,1,0, 0.23, 0,1]
       # 'categorical_features' is [[0,1,0,0,1]] and 'nonzero_indices' is [1,4]
       nonzero_indices = np.nonzero(categorical_features)[1]  # (P*B,)
       # Reshape the non-zero indices to align with the no. of categorical params
       # and shift by the cardinality of each parameter to compute the integer
-      # category value expected by ContinuousAndCategoricalValues.
-      # For example (cont. from above), [[1,4]] - [0,3] = [1, 1]
+      # category value. For example (cont. from above), [[1,4]] - [0,3] = [1, 1]
       categorical_index_features = (
           np.reshape(nonzero_indices, (-1, self._n_categorical_params))  # (B,P)
           - self.shift  # (P,)
       )  # (B,P)
-    return ContinuousAndCategoricalValues(
+    return types.ContinuousAndCategoricalArray(
         continuous=continuous_features, categorical=categorical_index_features
     )
+
+  def unmap(self, features: types.ContinuousAndCategoricalArray) -> np.ndarray:
+    """Convert back from ContinuousAndCategoricalArray to features."""
+    if features.continuous.shape[0] != features.categorical.shape[0]:
+      raise ValueError(
+          "'continuous' and 'categorical' first dimension doesn't match!"
+      )
+    batch_size = features.continuous.shape[0]
+    unmapped_features = np.zeros(
+        (batch_size, sum(self.categorical_dims) + len(self._continuous_indices))
+    )
+    con_ind = 0
+    cat_ind = 0
+    ind = 0
+    # Extract the continuous and categorical feature indices.
+    for spec in self.converter.output_specs:
+      if spec.type == core.NumpyArraySpecType.CONTINUOUS:
+        unmapped_features[:, ind] = features.continuous[:, con_ind]
+        con_ind += 1
+        ind += 1
+
+      elif spec.type == core.NumpyArraySpecType.ONEHOT_EMBEDDING:
+        unmapped_features[:, ind : ind + spec.num_dimensions] = np.eye(
+            spec.num_dimensions
+        )[features.categorical[:, cat_ind]]
+        cat_ind += 1
+        ind += spec.num_dimensions
+      else:
+        raise ValueError("Unexpected spec type %s!" % spec.type)
+
+    return unmapped_features
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper_test.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/feature_mapper_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,77 +39,93 @@
     trial3 = vz.Trial(parameters={'C1': 'c', 'C2': 'x', 'C3': '1', 'C4': '*'})
     converter = core.TrialToArrayConverter.from_study_config(
         problem,
         pad_oovs=pad_oovs,
         max_discrete_indices=0,
     )
     features = converter.to_features([trial1, trial2, trial3])
-    res = fm.ContinuousCategoricalFeatureMapper(converter).map(features)
+    feature_mapper = fm.ContinuousCategoricalFeatureMapper(converter)
+    res = feature_mapper.map(features)
 
     np.testing.assert_equal(
         res.categorical, np.array([[1, 3, 0, 0], [0, 3, 0, 0], [2, 1, 1, 0]])
     )
     np.testing.assert_equal(np.zeros((3, 0)), res.continuous)
+    # Test un-mapping
+    unmapped_features = feature_mapper.unmap(res)
+    np.testing.assert_equal(unmapped_features, features)
 
   @parameterized.product(pad_oovs=[False, True], max_discrete_indices=[0, 10])
   def test_discrete_only(self, pad_oovs, max_discrete_indices):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_discrete_param('d1', [1, 10, 20])
     trial1 = vz.Trial(parameters={'d1': 10})
     trial2 = vz.Trial(parameters={'d1': 1})
     trial3 = vz.Trial(parameters={'d1': 20})
     converter = core.TrialToArrayConverter.from_study_config(
         problem, pad_oovs=pad_oovs, max_discrete_indices=max_discrete_indices
     )
     features = converter.to_features([trial1, trial2, trial3])
+    feature_mapper = fm.ContinuousCategoricalFeatureMapper(converter)
     res = fm.ContinuousCategoricalFeatureMapper(converter).map(features)
     if max_discrete_indices == 10:
       # DISCRETE params are one-hot encoded. Should be mapped to categorical.
       np.testing.assert_equal(res.categorical, np.array([[1], [0], [2]]))
       np.testing.assert_equal(np.zeros((3, 0)), res.continuous)
     elif max_discrete_indices == 0:
       # DISCRETE params are continufied. Should be mapped to continuous.
       np.testing.assert_almost_equal(
           res.continuous, np.array([[(10 - 1) / (20 - 1)], [0.0], [1.0]])
       )
       np.testing.assert_equal(np.zeros((3, 0)), res.categorical)
+    # Test un-mapping
+    unmapped_features = feature_mapper.unmap(res)
+    np.testing.assert_equal(unmapped_features, features)
 
   def test_integer_only(self):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_int_param('i1', 0, 10)
     problem.search_space.root.add_int_param('i2', 0, 10)
     converter = core.TrialToArrayConverter.from_study_config(
         problem, pad_oovs=True, max_discrete_indices=0
     )
     trial1 = vz.Trial(parameters={'i1': 10, 'i2': 5})
     trial2 = vz.Trial(parameters={'i1': 1, 'i2': 3})
     trial3 = vz.Trial(parameters={'i1': 2, 'i2': 4})
     features = converter.to_features([trial1, trial2, trial3])
+    feature_mapper = fm.ContinuousCategoricalFeatureMapper(converter)
     res = fm.ContinuousCategoricalFeatureMapper(converter).map(features)
     np.testing.assert_equal(
         res.continuous, np.array([[1.0, 0.5], [0.1, 0.3], [0.2, 0.4]])
     )
     np.testing.assert_equal(np.zeros((3, 0)), res.categorical)
+    # Test un-mapping
+    unmapped_features = feature_mapper.unmap(res)
+    np.testing.assert_equal(unmapped_features, features)
 
   def test_float_only(self):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 1.0)
     problem.search_space.root.add_float_param('f2', 0.0, 1.0)
     converter = core.TrialToArrayConverter.from_study_config(
         problem, pad_oovs=True, max_discrete_indices=0
     )
     trial1 = vz.Trial(parameters={'f1': 1.0, 'f2': 0.5})
     trial2 = vz.Trial(parameters={'f1': 0.1, 'f2': 0.3})
     trial3 = vz.Trial(parameters={'f1': 0.2, 'f2': 0.4})
     features = converter.to_features([trial1, trial2, trial3])
+    feature_mapper = fm.ContinuousCategoricalFeatureMapper(converter)
     res = fm.ContinuousCategoricalFeatureMapper(converter).map(features)
     np.testing.assert_equal(
         res.continuous, np.array([[1.0, 0.5], [0.1, 0.3], [0.2, 0.4]])
     )
     np.testing.assert_equal(np.zeros((3, 0)), res.categorical)
+    # Test un-mapping
+    unmapped_features = feature_mapper.unmap(res)
+    np.testing.assert_equal(unmapped_features, features)
 
   @parameterized.product(pad_oovs=[False, True], max_discrete_indices=[0, 10])
   def test_mixed_space(self, pad_oovs, max_discrete_indices):
     problem = vz.ProblemStatement()
     problem.search_space.root.add_float_param('f1', 0.0, 1.0)
     problem.search_space.root.add_float_param('f2', 0.0, 1.0)
     problem.search_space.root.add_discrete_param('d1', [1, 10, 20])
@@ -117,14 +133,15 @@
     trial1 = vz.Trial(parameters={'f1': 1.0, 'f2': 0.5, 'd1': 10, 'c1': 'b'})
     trial2 = vz.Trial(parameters={'f1': 0.1, 'f2': 0.3, 'd1': 10, 'c1': 'a'})
     trial3 = vz.Trial(parameters={'f1': 0.2, 'f2': 0.4, 'd1': 20, 'c1': 'c'})
     converter = core.TrialToArrayConverter.from_study_config(
         problem, pad_oovs=pad_oovs, max_discrete_indices=max_discrete_indices
     )
     features = converter.to_features([trial1, trial2, trial3])
+    feature_mapper = fm.ContinuousCategoricalFeatureMapper(converter)
     res = fm.ContinuousCategoricalFeatureMapper(converter).map(features)
     if max_discrete_indices == 10:
       np.testing.assert_equal(
           res.continuous, np.array([[1.0, 0.5], [0.1, 0.3], [0.2, 0.4]])
       )
       np.testing.assert_equal(
           res.categorical, np.array([[1, 1], [1, 0], [2, 2]])
@@ -135,11 +152,14 @@
           np.array([
               [1.0, 0.5, (10 - 1) / (20 - 1)],
               [0.1, 0.3, (10 - 1) / (20 - 1)],
               [0.2, 0.4, 1.0],
           ]),
       )
       np.testing.assert_equal(res.categorical, np.array([[1], [0], [2]]))
+    # Test un-mapping
+    unmapped_features = feature_mapper.unmap(res)
+    np.testing.assert_equal(unmapped_features, features)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/input_warping.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/input_warping.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/input_warping_test.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/input_warping_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/spatio_temporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,17 +467,15 @@
     return self.trial_converter.metric_information
 
   def to_features(self,
                   trials: Sequence[pyvizier.Trial]) -> Dict[str, np.ndarray]:
     return self.trial_converter.to_features(trials)
 
   def to_xty(
-      self,
-      trials,
-      temporal_selection: str = 'auto'
+      self, trials: Sequence[pyvizier.Trial], temporal_selection: str = 'auto'
   ) -> Tuple[Dict[str, np.ndarray], np.ndarray, Dict[str, np.ndarray]]:
     """Returns x, t, and y.
 
     Args:
       trials:
       temporal_selection: 'infer', 'default', 'auto'. If 'infer', values are
         auto-inferred based on timestamps that exist in `trials`. If 'default',
```

### Comparing `google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal_test.py` & `google-vizier-0.1.6/vizier/pyvizier/converters/spatio_temporal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/multimetric/__init__.py` & `google-vizier-0.1.6/vizier/pyvizier/multimetric/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/pyvizier/multimetric/xla_pareto.py` & `google-vizier-0.1.6/vizier/pyvizier/multimetric/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/raytune/__init__.py` & `google-vizier-0.1.6/vizier/raytune/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/service/__init__.py` & `google-vizier-0.1.6/vizier/service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/service/clients/__init__.py` & `google-vizier-0.1.6/vizier/service/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/service/protos/__init__.py` & `google-vizier-0.1.6/vizier/service/protos/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/service/pyvizier/__init__.py` & `google-vizier-0.1.6/vizier/service/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/service/servers/__init__.py` & `google-vizier-0.1.6/vizier/service/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/testing/__init__.py` & `google-vizier-0.1.6/vizier/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/testing/test_studies.py` & `google-vizier-0.1.6/vizier/testing/test_studies.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/utils/attrs_utils.py` & `google-vizier-0.1.6/vizier/utils/attrs_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/utils/attrs_utils_test.py` & `google-vizier-0.1.6/vizier/utils/attrs_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/utils/json_utils.py` & `google-vizier-0.1.6/vizier/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/utils/json_utils_test.py` & `google-vizier-0.1.6/vizier/utils/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/utils/profiler.py` & `google-vizier-0.1.6/vizier/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.5/vizier/utils/profiler_test.py` & `google-vizier-0.1.6/vizier/utils/profiler_test.py`

 * *Files identical despite different names*

