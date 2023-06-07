# Comparing `tmp/autofit-2023.3.27.1.tar.gz` & `tmp/autofit-2023.7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofit-2023.3.27.1.tar", last modified: Mon Mar 27 14:47:32 2023, max compression
+gzip compressed data, was "autofit-2023.7.7.1.tar", last modified: Wed Jun  7 09:42:59 2023, max compression
```

## Comparing `autofit-2023.3.27.1.tar` & `autofit-2023.7.7.1.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.866167 autofit-2023.3.27.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.234824 autofit-2023.3.27.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.285811 autofit-2023.3.27.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2821 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/CITATIONS.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18817 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/CONTRIBUTING.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9144 2023-03-27 14:47:32.866167 autofit-2023.3.27.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8348 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.294381 autofit-2023.3.27.1/autofit/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5173 2023-03-27 14:47:16.000000 autofit-2023.3.27.1/autofit/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.301382 autofit-2023.3.27.1/autofit/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      106 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8710 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/aggregator/aggregator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9866 2021-06-17 13:08:20.000000 autofit-2023.3.27.1/autofit/aggregator/predicate.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4019 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/aggregator/search_output.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       27 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.310522 autofit-2023.3.27.1/autofit/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/config/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2708 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/logging.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.320536 autofit-2023.3.27.1/autofit/config/non_linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/non_linear/GridSearch.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      439 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/non_linear/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5905 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/non_linear/mcmc.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6765 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/non_linear/nest.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8407 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/config/non_linear/optimize.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1252 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/notation.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.339070 autofit-2023.3.27.1/autofit/config/priors/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      511 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/Exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/Gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      796 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/GaussianKurtosis.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/MultiLevelGaussians.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1706 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/model.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      123 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/prior.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/profiles.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1187 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/priors/template.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.344827 autofit-2023.3.27.1/autofit/config/visualize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      301 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/visualize/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/config/visualize/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1849 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/config/visualize/plots_search.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.348828 autofit-2023.3.27.1/autofit/database/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.354828 autofit-2023.3.27.1/autofit/database/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14744 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/aggregator/aggregator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7526 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/aggregator/scrape.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.363067 autofit-2023.3.27.1/autofit/database/migration/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       82 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/migration/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6131 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/migration/migration.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2485 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/migration/session_wrapper.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      450 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/migration/steps.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.371951 autofit-2023.3.27.1/autofit/database/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       85 2021-02-10 16:12:06.000000 autofit-2023.3.27.1/autofit/database/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8253 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/database/model/fit.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3125 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/model/instance.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6319 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/model/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2853 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/model/prior.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.376745 autofit-2023.3.27.1/autofit/database/query/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      468 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/query/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6665 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/query/condition.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4888 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/query/junction.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.387321 autofit-2023.3.27.1/autofit/database/query/query/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      129 2021-07-01 15:18:16.000000 autofit-2023.3.27.1/autofit/database/query/query/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1643 2021-07-01 15:18:16.000000 autofit-2023.3.27.1/autofit/database/query/query/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3320 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/query/query/attribute.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1199 2021-03-18 16:58:04.000000 autofit-2023.3.27.1/autofit/database/query/query/info.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8878 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/query/query/named.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1086 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/database/sqlalchemy_.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.394294 autofit-2023.3.27.1/autofit/example/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      126 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/example/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4491 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/example/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5889 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/example/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1746 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/example/util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1647 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/exc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.399276 autofit-2023.3.27.1/autofit/graphical/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.408190 autofit-2023.3.27.1/autofit/graphical/declarative/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8443 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3186 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/collection.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.418743 autofit-2023.3.27.1/autofit/graphical/declarative/factor/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/factor/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2554 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/factor/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3875 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/factor/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6630 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/factor/hierarchical.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1920 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/factor/prior.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8192 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/graph.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4964 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/declarative/result.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.431650 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17275 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/ep_mean_field.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1567 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/factor_optimiser.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9719 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/history.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17048 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/optimiser.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4417 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/stochastic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1621 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/expectation_propagation/visualise.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.442650 autofit-2023.3.27.1/autofit/graphical/factor_graphs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      274 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/factor_graphs/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14386 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/factor_graphs/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16292 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/factor_graphs/factor.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16109 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/factor_graphs/graph.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4682 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/factor_graphs/jacobians.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6392 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/factor_graphs/transform.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.450054 autofit-2023.3.27.1/autofit/graphical/laplace/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      155 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/laplace/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/laplace/line_search.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12011 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/graphical/laplace/newton.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6087 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/laplace/optimiser.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18773 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/mean_field.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13310 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/graphical/utils.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6343 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/interpolator.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.463235 autofit-2023.3.27.1/autofit/mapper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4849 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/identifier.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.466646 autofit-2023.3.27.1/autofit/mapper/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4507 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/mock/mock_model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13242 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/mapper/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2656 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/model_mapper.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5478 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/mapper/model_object.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23069 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/operator.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.484588 autofit-2023.3.27.1/autofit/mapper/prior/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      154 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7904 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/abstract.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.493230 autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6412 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/arithmetic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2661 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/assertion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7211 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/compound.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2066 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/mapper/prior/deferred.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3214 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3124 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/log_gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4258 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/log_uniform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/tuple_prior.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3275 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/uniform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2654 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior/width_modifier.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.508722 autofit-2023.3.27.1/autofit/mapper/prior_model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    61638 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      666 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/annotation.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/attribute_pair.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8639 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/collection.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14044 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/prior_model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2787 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/recursion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/mapper/prior_model/util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17043 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/variable.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19865 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mapper/variable_operator.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.524704 autofit-2023.3.27.1/autofit/messages/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14132 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4679 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/beta.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9403 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/composed_transform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2568 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/fixed.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/gamma.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7813 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/interface.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8528 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/normal.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11028 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/transform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/messages/utils.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1775 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/mock.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.534704 autofit-2023.3.27.1/autofit/non_linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/non_linear/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35707 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/abstract_search.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.547857 autofit-2023.3.27.1/autofit/non_linear/analysis/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      120 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4137 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9342 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/combined.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3827 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/free_parameter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3862 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/indexed.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1901 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/model_analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4550 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/analysis/multiprocessing.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.553587 autofit-2023.3.27.1/autofit/non_linear/grid/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/non_linear/grid/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.561587 autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13550 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/job.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7283 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2556 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/result_builder.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15721 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/grid/sensitivity.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1728 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/grid/simple_grid.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11223 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/initializer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.568198 autofit-2023.3.27.1/autofit/non_linear/mcmc/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1650 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/abstract_mcmc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5401 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/auto_correlations.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.575750 autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9990 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/emcee.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1105 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4770 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/samples.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.583752 autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1140 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4765 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11570 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/zeus.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.593484 autofit-2023.3.27.1/autofit/non_linear/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      761 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mock/mock_analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1319 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mock/mock_result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3584 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mock/mock_samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5717 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/mock/mock_search.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.598485 autofit-2023.3.27.1/autofit/non_linear/nest/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4048 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/abstract_nest.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.610252 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      144 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15669 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6070 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/dynamic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3701 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4272 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6353 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/static.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.618432 autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1756 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11292 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/ultranest.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.622430 autofit-2023.3.27.1/autofit/non_linear/optimize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1055 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/abstract_optimize.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.629431 autofit-2023.3.27.1/autofit/non_linear/optimize/drawer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/drawer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7760 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/drawer/drawer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      102 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/drawer/plotter.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.634873 autofit-2023.3.27.1/autofit/non_linear/optimize/lbfgs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/lbfgs/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6894 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/lbfgs/lbfgs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2799 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/lbfgs/samples.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.646664 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9683 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3455 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/globe.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3460 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/local.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1892 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/plotter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2894 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/samples.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.653664 autofit-2023.3.27.1/autofit/non_linear/parallel/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      167 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/parallel/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5220 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/parallel/process.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9687 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/parallel/sneaky.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.664632 autofit-2023.3.27.1/autofit/non_linear/paths/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/paths/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12102 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/paths/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5780 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/paths/database.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11042 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/paths/directory.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1582 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/paths/null.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3621 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/paths/sub_directory_paths.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8898 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/result.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.678632 autofit-2023.3.27.1/autofit/non_linear/samples/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9194 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/mcmc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6968 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/nest.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17364 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/pdf.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8118 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/sample.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21413 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/samples.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/samples/stored.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2726 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/non_linear/timer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.683632 autofit-2023.3.27.1/autofit/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      436 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3998 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/plot/output.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/autofit/plot/samples_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.690618 autofit-2023.3.27.1/autofit/text/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       50 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/autofit/text/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6261 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/text/formatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2873 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/text/samples_text.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4039 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/text/text_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.698619 autofit-2023.3.27.1/autofit/tools/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/autofit/tools/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      766 2021-01-22 12:56:54.000000 autofit-2023.3.27.1/autofit/tools/add_notebook_quotes.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      438 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/tools/namer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6651 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/tools/update_identifiers.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3670 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/autofit/tools/util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.865100 autofit-2023.3.27.1/autofit.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11169 2023-03-27 14:47:32.000000 autofit-2023.3.27.1/autofit.egg-info/SOURCES.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/build_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.706031 autofit-2023.3.27.1/docs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/docs/Makefile
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.709030 autofit-2023.3.27.1/docs/_templates/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/_templates/custom-class-template.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/_templates/custom_module_template.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.722552 autofit-2023.3.27.1/docs/api/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      967 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/analysis.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      944 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1281 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/model.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      846 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/plot.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1201 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/priors.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/samples.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2659 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/searches.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      649 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/api/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3755 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.730534 autofit-2023.3.27.1/docs/cookbooks/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8234 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/cookbooks/cookbook_1_basics.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11816 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/cookbooks/cookbook_2_collections.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11221 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/cookbooks/cookbook_3_multiple_datasets.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10571 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/cookbooks/cookbook_4_multi_level.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11943 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/cookbooks/cookbook_5_model_linking.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.739534 autofit-2023.3.27.1/docs/features/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6471 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/features/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8209 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/features/graphical.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.770624 autofit-2023.3.27.1/docs/features/images/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    53610 2021-01-26 21:44:53.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x1_1__low_snr.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38449 2021-01-26 21:44:53.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x1_2__low_snr.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37485 2021-01-26 21:44:53.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x1_3__low_snr.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33505 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x1_with_feature.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44404 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x1_with_feature_fit_feature.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43221 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46794 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x2_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25965 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x2_left.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38024 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x2_left_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47517 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x2_right_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33623 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/gaussian_x2_split.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23811 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/sensitivity_data_high.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28902 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/sensitivity_data_high_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34204 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/sensitivity_data_low.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40377 2021-01-26 18:42:54.000000 autofit-2023.3.27.1/docs/features/images/sensitivity_data_low_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9083 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/features/search_chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5844 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/features/search_grid_search.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12076 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/features/sensitivity_mapping.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.782575 autofit-2023.3.27.1/docs/general/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10257 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/general/adding_a_model_component.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/general/citations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1017 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/general/configs.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2021-01-28 19:37:07.000000 autofit-2023.3.27.1/docs/general/credits.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1097 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/general/roadmap.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      494 2020-11-16 19:40:51.000000 autofit-2023.3.27.1/docs/general/software.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2300 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/general/workspace.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.789574 autofit-2023.3.27.1/docs/howtofit/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2033 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/howtofit/chapter_1_introduction.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1614 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/howtofit/chapter_database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2198 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/howtofit/chapter_graphical_models.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5493 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/howtofit/howtofit.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.795100 autofit-2023.3.27.1/docs/images/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69268 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/images/cornerplot.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/docs/images/toy_model_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57271 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/docs/images/toy_model_fit_x2.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9989 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/index.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.805099 autofit-2023.3.27.1/docs/installation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1409 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/installation/conda.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1543 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/installation/overview.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1156 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/installation/pip.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1439 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/installation/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1446 2021-01-26 22:07:31.000000 autofit-2023.3.27.1/docs/installation/troubleshooting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/docs/make.bat
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.814099 autofit-2023.3.27.1/docs/overview/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.826099 autofit-2023.3.27.1/docs/overview/image/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1010915 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/image/cluster_example.jpg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  2030601 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/image/lens_model.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  3051390 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/image/lens_model_cluster.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13863 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/model_complex.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10198 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/model_fit.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12585 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/docs/overview/multi_datasets.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6800 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/non_linear_search.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11893 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/overview/result.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      344 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/docs/requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.833099 autofit-2023.3.27.1/docs/science_examples/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13077 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/docs/science_examples/astronomy.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      139 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/eden.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.846301 autofit-2023.3.27.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1339 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/files/citation.tex
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13632 2023-02-21 14:10:09.000000 autofit-2023.3.27.1/files/citations.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1171 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/files/citations.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2021-06-17 13:08:20.000000 autofit-2023.3.27.1/files/eden.ini
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27322 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/files/gaussian_example.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2021-02-11 23:21:00.000000 autofit-2023.3.27.1/files/release.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1226 2021-06-17 13:08:20.000000 autofit-2023.3.27.1/files/to_do_list
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.3.27.1/files/toy_model_fit.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       72 2023-03-27 14:43:03.000000 autofit-2023.3.27.1/optional_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.854100 autofit-2023.3.27.1/paper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2020-11-16 19:40:52.000000 autofit-2023.3.27.1/paper/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12475 2023-02-21 14:10:09.000000 autofit-2023.3.27.1/paper/paper.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2021-12-09 20:28:25.000000 autofit-2023.3.27.1/paper/paper.json
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11881 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/paper/paper.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/readthedocs.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      240 2023-03-27 14:45:58.000000 autofit-2023.3.27.1/requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-03-27 14:47:32.863100 autofit-2023.3.27.1/scripts/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-02-24 17:53:38.000000 autofit-2023.3.27.1/scripts/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      454 2021-01-22 12:56:54.000000 autofit-2023.3.27.1/scripts/add_notebook_quotes.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      268 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/scripts/aggregate.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/scripts/example_map.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      833 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/scripts/update_identifiers.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/scripts/update_identifiers_from_file.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2023-03-27 14:47:32.867100 autofit-2023.3.27.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1918 2023-03-27 14:45:03.000000 autofit-2023.3.27.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2081 2023-02-21 14:09:59.000000 autofit-2023.3.27.1/to_do_list
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.841664 autofit-2023.7.7.1/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:58.992246 autofit-2023.7.7.1/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.048964 autofit-2023.7.7.1/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2821 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18817 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2454 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9143 2023-06-07 09:42:59.841664 autofit-2023.7.7.1/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8348 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.059876 autofit-2023.7.7.1/autofit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5232 2023-06-07 09:38:14.000000 autofit-2023.7.7.1/autofit/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.067824 autofit-2023.7.7.1/autofit/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      106 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8944 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/aggregator/aggregator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9866 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/aggregator/predicate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4275 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/aggregator/search_output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       27 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.077823 autofit-2023.7.7.1/autofit/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2023-05-09 16:10:42.000000 autofit-2023.7.7.1/autofit/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2870 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/logging.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.089820 autofit-2023.7.7.1/autofit/config/non_linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/GridSearch.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      439 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5905 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/mcmc.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6765 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/non_linear/nest.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8407 2023-03-27 14:43:03.000000 autofit-2023.7.7.1/autofit/config/non_linear/optimize.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1252 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.112582 autofit-2023.7.7.1/autofit/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      511 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/Exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/Gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      796 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/GaussianKurtosis.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/MultiLevelGaussians.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1706 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/model.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      123 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/prior.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/profiles.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1187 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/priors/template.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.119581 autofit-2023.7.7.1/autofit/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      301 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1849 2023-03-27 14:43:03.000000 autofit-2023.7.7.1/autofit/config/visualize/plots_search.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.124017 autofit-2023.7.7.1/autofit/database/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.130954 autofit-2023.7.7.1/autofit/database/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/database/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15442 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/aggregator/aggregator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6939 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/aggregator/scrape.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.141104 autofit-2023.7.7.1/autofit/database/migration/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       82 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/database/migration/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6131 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/migration/migration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2485 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/migration/session_wrapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      450 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/migration/steps.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.152914 autofit-2023.7.7.1/autofit/database/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       85 2021-02-10 16:12:06.000000 autofit-2023.7.7.1/autofit/database/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8445 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/model/fit.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3125 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/model/instance.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6319 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/model/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2853 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/model/prior.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.159919 autofit-2023.7.7.1/autofit/database/query/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      468 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6449 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/query/condition.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4888 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/junction.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.174281 autofit-2023.7.7.1/autofit/database/query/query/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      129 2021-07-01 15:18:16.000000 autofit-2023.7.7.1/autofit/database/query/query/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1643 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/query/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-05-15 17:36:10.000000 autofit-2023.7.7.1/autofit/database/query/query/attribute.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1199 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/query/info.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8878 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/query/query/named.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1086 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/database/sqlalchemy_.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.182851 autofit-2023.7.7.1/autofit/example/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      126 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/example/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6895 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/autofit/example/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5889 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/autofit/example/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1746 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/example/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1647 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      845 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.189851 autofit-2023.7.7.1/autofit/graphical/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.201945 autofit-2023.7.7.1/autofit/graphical/declarative/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        1 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/declarative/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8648 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3186 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/collection.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.215895 autofit-2023.7.7.1/autofit/graphical/declarative/factor/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2554 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4025 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6630 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/hierarchical.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1920 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/declarative/factor/prior.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8192 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/graph.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4964 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/declarative/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.233904 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      213 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17242 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/ep_mean_field.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2068 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/factor_optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9719 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/history.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17494 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4417 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/stochastic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1621 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/expectation_propagation/visualise.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.249913 autofit-2023.7.7.1/autofit/graphical/factor_graphs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      274 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14727 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16298 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/factor.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16109 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/graph.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4870 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/jacobians.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6392 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/factor_graphs/transform.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.259665 autofit-2023.7.7.1/autofit/graphical/laplace/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      155 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/graphical/laplace/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/laplace/line_search.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12004 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/laplace/newton.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6087 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/laplace/optimiser.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18909 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/mean_field.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16822 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/graphical/utils.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6343 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/interpolator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.277189 autofit-2023.7.7.1/autofit/mapper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      124 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4849 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/identifier.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.281189 autofit-2023.7.7.1/autofit/mapper/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4507 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/mock/mock_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13695 2023-06-03 08:34:09.000000 autofit-2023.7.7.1/autofit/mapper/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2656 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/model_mapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5691 2023-06-03 08:34:09.000000 autofit-2023.7.7.1/autofit/mapper/model_object.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23069 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/operator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.304591 autofit-2023.7.7.1/autofit/mapper/prior/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      154 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7904 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/abstract.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.315604 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6412 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/arithmetic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2661 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/assertion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7211 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/compound.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2066 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior/deferred.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3214 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3124 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/log_gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4258 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/log_uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/tuple_prior.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3275 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/prior/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2654 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior/width_modifier.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.335469 autofit-2023.7.7.1/autofit/mapper/prior_model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63100 2023-06-03 08:34:09.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      666 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/annotation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/attribute_pair.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8290 2023-05-10 13:42:01.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/collection.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13987 2023-05-10 13:42:01.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/prior_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2787 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/recursion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/mapper/prior_model/util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17043 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/variable.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19865 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mapper/variable_operator.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.357353 autofit-2023.7.7.1/autofit/messages/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      315 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14433 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4679 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/beta.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9477 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/composed_transform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2568 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/fixed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/gamma.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7813 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/messages/interface.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8896 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/normal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11028 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/messages/transform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/messages/utils.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1775 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.370727 autofit-2023.7.7.1/autofit/non_linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36116 2023-06-05 20:26:47.000000 autofit-2023.7.7.1/autofit/non_linear/abstract_search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.388446 autofit-2023.7.7.1/autofit/non_linear/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      120 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5735 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12394 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/combined.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3827 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/free_parameter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4103 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/indexed.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1901 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/model_analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4550 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/analysis/multiprocessing.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.396357 autofit-2023.7.7.1/autofit/non_linear/grid/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/non_linear/grid/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.407213 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13550 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/job.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7283 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2556 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result_builder.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15909 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/sensitivity.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1728 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/grid/simple_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11223 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/initializer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.415889 autofit-2023.7.7.1/autofit/non_linear/mcmc/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1650 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/abstract_mcmc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5401 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/auto_correlations.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.426889 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9990 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/emcee.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1105 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4770 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/samples.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.438889 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1140 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4765 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11570 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/zeus.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.452533 autofit-2023.7.7.1/autofit/non_linear/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      761 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1319 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3584 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5717 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/mock/mock_search.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.457532 autofit-2023.7.7.1/autofit/non_linear/nest/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/nest/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4048 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/abstract_nest.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.475536 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      144 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15669 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6070 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/dynamic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3701 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4272 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6353 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/static.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.487098 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1756 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11292 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/ultranest.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.492109 autofit-2023.7.7.1/autofit/non_linear/optimize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1055 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/abstract_optimize.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.500107 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7760 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/drawer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      102 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/plotter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.509088 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6894 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/lbfgs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2799 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/samples.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.526148 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9683 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3455 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/globe.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3460 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/local.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1892 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/plotter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2894 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/samples.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.533670 autofit-2023.7.7.1/autofit/non_linear/parallel/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      167 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/parallel/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5220 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/parallel/process.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9687 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/parallel/sneaky.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.548604 autofit-2023.7.7.1/autofit/non_linear/paths/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/paths/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12102 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/paths/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5834 2023-05-10 13:42:01.000000 autofit-2023.7.7.1/autofit/non_linear/paths/database.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11042 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/paths/directory.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1582 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/paths/null.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3621 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/paths/sub_directory_paths.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8898 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.566829 autofit-2023.7.7.1/autofit/non_linear/samples/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/non_linear/samples/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9194 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/mcmc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6968 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/nest.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17430 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/pdf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8118 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/sample.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21413 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/samples.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/samples/stored.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2726 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/non_linear/timer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.573608 autofit-2023.7.7.1/autofit/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      436 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3998 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/plot/output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/plot/samples_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.582545 autofit-2023.7.7.1/autofit/text/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       50 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/autofit/text/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6261 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/text/formatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2873 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/text/samples_text.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4039 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/text/text_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.593388 autofit-2023.7.7.1/autofit/tools/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/autofit/tools/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      766 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/tools/add_notebook_quotes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      438 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/autofit/tools/namer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6651 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/tools/update_identifiers.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3670 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/autofit/tools/util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.840108 autofit-2023.7.7.1/autofit.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11169 2023-06-07 09:42:58.000000 autofit-2023.7.7.1/autofit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       40 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/build_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.603329 autofit-2023.7.7.1/docs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/docs/Makefile
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.607250 autofit-2023.7.7.1/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.625162 autofit-2023.7.7.1/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      967 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/analysis.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      944 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1281 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/model.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      846 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1201 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/priors.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/samples.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2659 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/searches.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      649 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3755 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.636170 autofit-2023.7.7.1/docs/cookbooks/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8234 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_1_basics.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11816 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_2_collections.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11221 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_3_multiple_datasets.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10571 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_4_multi_level.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11943 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/cookbooks/cookbook_5_model_linking.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.647167 autofit-2023.7.7.1/docs/features/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6471 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8209 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/graphical.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.688758 autofit-2023.7.7.1/docs/features/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    53610 2021-01-26 21:44:53.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_1__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38449 2021-01-26 21:44:53.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_2__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37485 2021-01-26 21:44:53.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_3__low_snr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33505 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44404 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43221 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46794 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25965 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_left.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38024 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_left_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47517 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_right_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33623 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/gaussian_x2_split.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23811 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_high.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28902 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_high_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34204 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_low.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40377 2021-01-26 18:42:54.000000 autofit-2023.7.7.1/docs/features/images/sensitivity_data_low_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9083 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5844 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/features/search_grid_search.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12076 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/docs/features/sensitivity_mapping.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.705765 autofit-2023.7.7.1/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10257 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/adding_a_model_component.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1017 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2021-01-28 19:37:07.000000 autofit-2023.7.7.1/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1097 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/roadmap.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      494 2020-11-16 19:40:51.000000 autofit-2023.7.7.1/docs/general/software.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2300 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.715423 autofit-2023.7.7.1/docs/howtofit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2033 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1614 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/chapter_database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2198 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/chapter_graphical_models.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5493 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/howtofit/howtofit.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.723051 autofit-2023.7.7.1/docs/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69268 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/images/cornerplot.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/docs/images/toy_model_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57271 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/docs/images/toy_model_fit_x2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9989 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.736045 autofit-2023.7.7.1/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1409 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1543 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1156 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1439 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1446 2021-01-26 22:07:31.000000 autofit-2023.7.7.1/docs/installation/troubleshooting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/docs/make.bat
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.748639 autofit-2023.7.7.1/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.763170 autofit-2023.7.7.1/docs/overview/image/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1010915 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/image/cluster_example.jpg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  2030601 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/image/lens_model.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  3051390 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/image/lens_model_cluster.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13863 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/model_complex.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10198 2023-05-09 16:10:42.000000 autofit-2023.7.7.1/docs/overview/model_fit.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12585 2023-03-27 14:43:03.000000 autofit-2023.7.7.1/docs/overview/multi_datasets.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6800 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/overview/non_linear_search.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11895 2023-06-05 10:53:40.000000 autofit-2023.7.7.1/docs/overview/result.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      344 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/docs/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.771730 autofit-2023.7.7.1/docs/science_examples/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13077 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/docs/science_examples/astronomy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      139 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/eden.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.790293 autofit-2023.7.7.1/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1339 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/files/citation.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13632 2023-02-21 14:10:09.000000 autofit-2023.7.7.1/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1171 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2021-06-17 13:08:20.000000 autofit-2023.7.7.1/files/eden.ini
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27322 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/files/gaussian_example.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2021-02-11 23:21:00.000000 autofit-2023.7.7.1/files/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1226 2021-06-17 13:08:20.000000 autofit-2023.7.7.1/files/to_do_list
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43169 2020-11-10 18:15:59.000000 autofit-2023.7.7.1/files/toy_model_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       74 2023-06-01 08:52:02.000000 autofit-2023.7.7.1/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.798829 autofit-2023.7.7.1/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2020-11-16 19:40:52.000000 autofit-2023.7.7.1/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12475 2023-02-21 14:10:09.000000 autofit-2023.7.7.1/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      813 2021-12-09 20:28:25.000000 autofit-2023.7.7.1/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11881 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/readthedocs.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      240 2023-05-10 13:41:29.000000 autofit-2023.7.7.1/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:42:59.818429 autofit-2023.7.7.1/scripts/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-02-24 17:53:38.000000 autofit-2023.7.7.1/scripts/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      454 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/add_notebook_quotes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      268 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/aggregate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/scripts/example_map.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      833 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/update_identifiers.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-06-05 20:26:39.000000 autofit-2023.7.7.1/scripts/update_identifiers_from_file.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2023-06-07 09:42:59.843660 autofit-2023.7.7.1/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1917 2023-06-07 09:42:35.000000 autofit-2023.7.7.1/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2081 2023-02-21 14:09:59.000000 autofit-2023.7.7.1/to_do_list
```

### Comparing `autofit-2023.3.27.1/.github/workflows/main.yml` & `autofit-2023.7.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/CITATIONS.rst` & `autofit-2023.7.7.1/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/CODE_OF_CONDUCT.md` & `autofit-2023.7.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/CONTRIBUTING.md` & `autofit-2023.7.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/LICENSE` & `autofit-2023.7.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/PKG-INFO` & `autofit-2023.7.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofit
-Version: 2023.3.27.1
+Version: 2023.7.7.1
 Summary: Classy Probabilistic Programming
 Home-page: https://github.com/rhayes777/PyAutoFit
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autofit-2023.3.27.1/README.rst` & `autofit-2023.7.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/__init__.py` & `autofit-2023.7.7.1/autofit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 from .mapper.prior_model.collection import Collection
 from .mapper.prior_model.prior_model import Model
 from .mapper.prior_model.prior_model import Model
 from .mapper.prior_model.util import PriorModelNameValue
 from .non_linear.abstract_search import NonLinearSearch
 from .non_linear.abstract_search import PriorPasser
 from .non_linear.analysis.analysis import Analysis
+from .non_linear.analysis.combined import CombinedAnalysis
 from .non_linear.grid.grid_search import GridSearchResult
 from .non_linear.initializer import InitializerBall
 from .non_linear.initializer import InitializerPrior
 from .non_linear.initializer import SpecificRangeInitializer
 from .non_linear.mcmc.auto_correlations import AutoCorrelationsSettings
 from .non_linear.mcmc.emcee.emcee import Emcee
 from .non_linear.mcmc.zeus.zeus import Zeus
@@ -105,8 +106,8 @@
 @register(abc.ABCMeta)
 def save_abc(pickler, obj):
     pickle._Pickler.save_type(pickler, obj)
 
 
 conf.instance.register(__file__)
 
-__version__ = "2023.3.27.1"
+__version__ = "2023.7.7.1"
```

### Comparing `autofit-2023.3.27.1/autofit/aggregator/aggregator.py` & `autofit-2023.7.7.1/autofit/aggregator/aggregator.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,20 +44,15 @@
         predicates
             Predicates that evaluate to `True` or `False` for any given phase.
 
         Returns
         -------
         A collection of groups of the same length with each group having the same or fewer members.
         """
-        return AggregatorGroup(
-            [
-                group.filter(*predicates)
-                for group in self.groups
-            ]
-        )
+        return AggregatorGroup([group.filter(*predicates) for group in self.groups])
 
     def __getitem__(self, item):
         return self.groups[item]
 
     def __len__(self):
         return len(self.groups)
 
@@ -71,18 +66,15 @@
         name
             The name of the attribute to be extracted
 
         Returns
         -------
         A list of lists of values.
         """
-        return [
-            group.values(name)
-            for group in self.groups
-        ]
+        return [group.values(name) for group in self.groups]
 
 
 class AbstractAggregator:
     def __init__(self, search_outputs: List[SearchOutput]):
         """
         An aggregator that comprises several search_outputs which matching filters.
 
@@ -94,31 +86,23 @@
         self.search_outputs = search_outputs
 
     def remove_unzipped(self):
         """
         Removes the unzipped output directory for each phase.
         """
         for phase in self.search_outputs:
-
             split_path = path.split(phase.directory)[0]
 
             unzipped_path = path.join(split_path)
 
-            rmtree(
-                unzipped_path,
-                ignore_errors=True
-            )
+            rmtree(unzipped_path, ignore_errors=True)
 
     def __getitem__(
-            self,
-            item: Union[slice, int]
-    ) -> Union[
-        "AbstractAggregator",
-        SearchOutput
-    ]:
+        self, item: Union[slice, int]
+    ) -> Union["AbstractAggregator", SearchOutput]:
         """
         If an index is passed in then a specific phase output is returned.
 
         If a slice is passed in then an aggregator comprising several search_outputs is returned.
 
         Parameters
         ----------
@@ -126,17 +110,15 @@
             A slice or index
 
         Returns
         -------
         An aggregator or phase
         """
         if isinstance(item, slice):
-            return AbstractAggregator(
-                self.search_outputs[item]
-            )
+            return AbstractAggregator(self.search_outputs[item])
         return self.search_outputs[item]
 
     def __len__(self):
         return len(self.search_outputs)
 
     def __getattr__(self, item):
         return AttributePredicate(item)
@@ -180,38 +162,49 @@
             phase output. If a pickle file with this name is in the
             phase output directory then that pickle will be loaded.
 
         Returns
         -------
         A generator of values for the attribute
         """
-        return map(
-            lambda phase: getattr(
-                phase, name
-            ),
-            self.search_outputs
-        )
+        return map(lambda phase: getattr(phase, name), self.search_outputs)
+
+    def child_values(self, name: str) -> Iterator[List]:
+        """
+        Get values with a given name from the child analyses of each search in
+        this aggregator.
+
+        Parameters
+        ----------
+        name
+            The name of an attribute expected to be associated with
+            child analysis output. If a pickle file with this name
+            is in the child analysis output directory then that pickle
+            will be loaded.
+
+        Returns
+        -------
+        A generator of values for the attribute
+        """
+        return (phase.child_values(name) for phase in self.search_outputs)
 
     def map(self, func):
         """
         Map some function onto the aggregated output objects.
 
         Parameters
         ----------
         func
             A function
 
         Returns
         -------
         A generator of results
         """
-        return map(
-            func,
-            self.search_outputs
-        )
+        return map(func, self.search_outputs)
 
     def group_by(self, field: str) -> AggregatorGroup:
         """
         Group the search_outputs by a field, e.g. pipeline.
 
         The object returned still permits filtering and attribute querying.
 
@@ -237,19 +230,15 @@
         return "\n\n".join(
             "{}\n\n{}".format(phase.header, phase.model_results)
             for phase in self.search_outputs
         )
 
 
 class Aggregator(AbstractAggregator):
-    def __init__(
-            self,
-            directory: Union[str, os.PathLike],
-            completed_only=False
-    ):
+    def __init__(self, directory: Union[str, os.PathLike], completed_only=False):
         """
         Class to aggregate phase results for all subdirectories in a given directory.
 
         The whole directory structure is traversed and a Phase object created for each directory that contains a
         metadata file.
 
         Parameters
@@ -272,22 +261,22 @@
             for filename in filenames:
                 if filename.endswith(".zip"):
                     try:
                         with zipfile.ZipFile(path.join(root, filename), "r") as f:
                             f.extractall(path.join(root, filename[:-4]))
                     except zipfile.BadZipFile:
                         raise zipfile.BadZipFile(
-                            f"File is not a zip file: \n "
-                            f"{root} \n"
-                            f"{filename}"
+                            f"File is not a zip file: \n " f"{root} \n" f"{filename}"
                         )
 
         for root, _, filenames in os.walk(directory):
             if "metadata" in filenames:
                 if not completed_only or ".completed" in filenames:
                     search_outputs.append(SearchOutput(root))
 
         if len(search_outputs) == 0:
             print(f"\nNo search_outputs found in {directory}\n")
         else:
-            print(f"\n A total of {str(len(search_outputs))} search_outputs and results were found.")
+            print(
+                f"\n A total of {str(len(search_outputs))} search_outputs and results were found."
+            )
         super().__init__(search_outputs)
```

### Comparing `autofit-2023.3.27.1/autofit/aggregator/predicate.py` & `autofit-2023.7.7.1/autofit/aggregator/predicate.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/aggregator/search_output.py` & `autofit-2023.7.7.1/autofit/aggregator/search_output.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,106 @@
 import logging
 import os
 import pickle
 from os import path
+from pathlib import Path
 
 import dill
 
 from autofit.non_linear import abstract_search
 
 original_create_file_handle = dill._dill._create_filehandle
 
 
 def _create_file_handle(*args, **kwargs):
     """
     Handle FileNotFoundError when attempting to deserialize pickles
     using dill and return None instead.
     """
     try:
-        return original_create_file_handle(
-            *args, **kwargs
-        )
+        return original_create_file_handle(*args, **kwargs)
     except pickle.UnpicklingError as e:
-        if not isinstance(
-                e.args[0],
-                FileNotFoundError
-        ):
+        if not isinstance(e.args[0], FileNotFoundError):
             raise e
         logging.warning(
             f"Could not create a handler for {e.args[0].filename} as it does not exist"
         )
         return None
 
 
 dill._dill._create_filehandle = _create_file_handle
 
 
-class SearchOutput:
+class Output:
+    def __init__(self, directory: Path):
+        self.directory = directory
+
+    @property
+    def pickle_path(self):
+        return self.directory / "pickles"
+
+    def __getattr__(self, item):
+        """
+        Attempt to load a pickle by the same name from the search output directory.
+
+        dataset.pickle, meta_dataset.pickle etc.
+        """
+        try:
+            with open(self.pickle_path / f"{item}.pickle", "rb") as f:
+                return pickle.load(f)
+        except FileNotFoundError:
+            pass
+
+
+class SearchOutput(Output):
     """
     @DynamicAttrs
     """
 
     def __init__(self, directory: str):
         """
         Represents the output of a single search. Comprises a metadata file and other dataset files.
 
         Parameters
         ----------
         directory
             The directory of the search
         """
-        self.directory = directory
+        super().__init__(Path(directory))
         self.__search = None
         self.__model = None
         self.file_path = os.path.join(directory, "metadata")
         with open(self.file_path) as f:
             self.text = f.read()
-            pairs = [
-                line.split("=")
-                for line
-                in self.text.split("\n")
-                if "=" in line
-            ]
+            pairs = [line.split("=") for line in self.text.split("\n") if "=" in line]
             self.__dict__.update({pair[0]: pair[1] for pair in pairs})
 
     @property
-    def pickle_path(self):
-        return path.join(self.directory, "pickles")
+    def child_analyses(self):
+        """
+        A list of child analyses loaded from the analyses directory
+        """
+        return list(map(Output, Path(self.directory).glob("analyses/*")))
 
     @property
     def model_results(self) -> str:
         """
         Reads the model.results file
         """
-        with open(os.path.join(self.directory, "model.results")) as f:
+        with open(self.directory / "model.results") as f:
             return f.read()
 
     @property
     def mask(self):
         """
         A pickled mask object
         """
-        with open(
-                os.path.join(self.pickle_path, "mask.pickle"), "rb"
-        ) as f:
+        with open(self.pickle_path / "mask.pickle", "rb") as f:
             return dill.load(f)
 
-    def __getattr__(self, item):
-        """
-        Attempt to load a pickle by the same name from the search output directory.
-
-        dataset.pickle, meta_dataset.pickle etc.
-        """
-        try:
-            with open(
-                    os.path.join(self.pickle_path, f"{item}.pickle"), "rb"
-            ) as f:
-                return pickle.load(f)
-        except FileNotFoundError:
-            pass
-
     @property
     def header(self) -> str:
         """
         A header created by joining the search name
         """
         phase = self.phase or ""
         dataset_name = self.dataset_name or ""
@@ -110,29 +109,35 @@
     @property
     def search(self) -> abstract_search.NonLinearSearch:
         """
         The search object that was used in this phase
         """
         if self.__search is None:
             try:
-                with open(os.path.join(self.pickle_path, "search.pickle"), "r+b") as f:
+                with open(self.pickle_path / "search.pickle", "r+b") as f:
                     self.__search = pickle.loads(f.read())
             except (FileNotFoundError, ModuleNotFoundError) as e:
                 print(self.pickle_path)
                 logging.exception(e)
         return self.__search
 
+    def child_values(self, name):
+        """
+        Get the values of a given key for all children
+        """
+        return [getattr(child, name) for child in self.child_analyses]
+
     @property
     def model(self):
         """
         The model that was used in this phase
         """
         if self.__model is None:
             try:
-                with open(os.path.join(self.pickle_path, "model.pickle"), "r+b") as f:
+                with open(self.pickle_path / "model.pickle", "r+b") as f:
                     self.__model = pickle.loads(f.read())
             except (FileNotFoundError, ModuleNotFoundError) as e:
                 print(self.pickle_path)
                 logging.exception(e)
         return self.__model
 
     def __str__(self):
```

### Comparing `autofit-2023.3.27.1/autofit/config/README.rst` & `autofit-2023.7.7.1/autofit/config/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/general.yaml` & `autofit-2023.7.7.1/autofit/config/general.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 inversion:
   check_reconstruction: true        # If True, the inversion's reconstruction is checked to ensure the solution of a meshs's mapper is not an invalid solution where the values are all the same.
   reconstruction_vmax_factor: 0.5   # Plots of an Inversion's reconstruction use the reconstructed data's bright value multiplied by this factor.  
 model:
   ignore_prior_limits: false        # If ``True`` the limits applied to priors will be ignored, where limits set upper / lower limits. This stops PriorLimitException's from being raised.
 output:
   force_pickle_overwrite: false     # If True pickle files output by a search (e.g. samples.pickle) are recreated when a new model-fit is performed.
+  force_visualize_overwrite: false # If True, visualization images output by a search (e.g. subplots of the fit) are recreated when a new model-fit is performed.
   info_whitespace_length: 80        # Length of whitespace between the parameter names and values in the model.info / result.info
   log_level: INFO                   # The level of information output by logging.
   log_to_file: false                # If True, outputs the non-linear search log to a file (and not printed to screen).
   log_file: output.log              # The name of the file the logged output is written to (in the non-linear search output folder)
   model_results_decimal_places: 3   # Number of decimal places estimated parameter values / errors are output in model.results.
   remove_files: false               # If True, all output files of a non-linear search (e.g. samples, visualization, etc.) are deleted once the model-fit has completed, such that only the .zip file remains.
   samples_to_csv: true              # If True, non-linear search samples are written to a .csv file.
```

### Comparing `autofit-2023.3.27.1/autofit/config/non_linear/mcmc.yaml` & `autofit-2023.7.7.1/autofit/config/non_linear/mcmc.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/non_linear/nest.yaml` & `autofit-2023.7.7.1/autofit/config/non_linear/nest.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/non_linear/optimize.yaml` & `autofit-2023.7.7.1/autofit/config/non_linear/optimize.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/notation.yaml` & `autofit-2023.7.7.1/autofit/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/priors/Gaussian.yaml` & `autofit-2023.7.7.1/autofit/config/priors/Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/priors/GaussianKurtosis.yaml` & `autofit-2023.7.7.1/autofit/config/priors/GaussianKurtosis.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/priors/README.rst` & `autofit-2023.7.7.1/autofit/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/priors/model.yaml` & `autofit-2023.7.7.1/autofit/config/priors/model.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/priors/profiles.yaml` & `autofit-2023.7.7.1/autofit/config/priors/profiles.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/priors/template.yaml` & `autofit-2023.7.7.1/autofit/config/priors/template.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/config/visualize/plots_search.yaml` & `autofit-2023.7.7.1/autofit/config/visualize/plots_search.yaml`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/__init__.py` & `autofit-2023.7.7.1/autofit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/aggregator/aggregator.py` & `autofit-2023.7.7.1/autofit/database/aggregator/aggregator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 from autofit.database import query as q
 from .scrape import Scraper
 from autofit.database import model as m
 from ..query.query import AbstractQuery, Attribute
 from ..query.query.attribute import BestFitQuery
 
-logger = logging.getLogger(
-    __name__
-)
+logger = logging.getLogger(__name__)
 
 
 class NullPredicate(AbstractQuery):
     @property
     def fit_query(self) -> str:
         return "SELECT id FROM fit"
 
@@ -58,18 +56,15 @@
         unique_tag
         path_prefix
         is_complete
         is_grid_search
     """
 
     @staticmethod
-    def for_name(name: str) -> Union[
-        AbstractQuery,
-        Attribute
-    ]:
+    def for_name(name: str) -> Union[AbstractQuery, Attribute]:
         """
         Create a query based on some attribute of the Fit.
 
         Parameters
         ----------
         name
             The name of an attribute of the Fit class
@@ -79,20 +74,16 @@
         A query based on an attribute
 
         Examples
         --------
         aggregator.fit.name == 'example name'
         """
         if name not in m.fit_attributes:
-            raise AttributeError(
-                f"Fit has no attribute {name}"
-            )
-        if m.fit_attributes[
-            name
-        ].type.python_type == bool:
+            raise AttributeError(f"Fit has no attribute {name}")
+        if m.fit_attributes[name].type.python_type == bool:
             return q.BA(name)
         return q.A(name)
 
 
 class Reverse:
     def __init__(self, item):
         self.item = item
@@ -126,62 +117,85 @@
         for fit in self:
             value = fit[name]
             if value is not None:
                 values.append(value)
 
         return values
 
+    def child_values(self, name: str) -> List[list]:
+        """
+        Retrieve the value associated with each fit with the given
+        parameter name
+
+        Parameters
+        ----------
+        name
+            The name of some pickle, such as 'samples'
+
+        Returns
+        -------
+        A list of objects, one for each fit
+        """
+        return [fit.child_values(name) for fit in self]
+
     def __iter__(self):
-        return iter(
-            self.fits
-        )
+        return iter(self.fits)
 
     def __len__(self):
         return len(self.fits)
 
     def __eq__(self, other):
         if isinstance(other, list):
             return self.fits == other
         return super().__eq__(other)
 
 
 class Aggregator(AbstractAggregator):
     def __init__(
-            self,
-            session: sa.orm.Session,
-            filename: Optional[str] = None,
-            predicate: AbstractQuery = NullPredicate(),
-            offset=0,
-            limit=None,
-            order_bys=None
+        self,
+        session: sa.orm.Session,
+        filename: Optional[str] = None,
+        predicate: AbstractQuery = NullPredicate(),
+        offset=0,
+        limit=None,
+        order_bys=None,
+        top_level_only=True,
     ):
         """
         Query results from an intermediary SQLite database.
 
         Results can be scraped from a directory structure and stored in the database.
 
         Parameters
         ----------
         session
             A session for communicating with the database.
         filename
+            The path to the database file. If None, the database is in memory.
+        predicate
+            A predicate to filter the results by.
+        offset
+            The number of results to skip
+        limit
+            The maximum number of results to return
+        order_bys
+            A list of attributes to order the results by
+        top_level_only
+            If True, only return the top level fits
         """
         self.session = session
         self.filename = filename
         self._fits = None
         self._predicate = predicate
         self._offset = offset
         self._limit = limit
         self._order_bys = order_bys or list()
+        self._top_level_only = top_level_only
 
-    def order_by(
-            self,
-            item: Attribute,
-            reverse=False
-    ) -> "Aggregator":
+    def order_by(self, item: Attribute, reverse=False) -> "Aggregator":
         """
         Order the results by a given attribute of the search. Can be applied
         multiple times with the first application taking precedence.
 
         Parameters
         ----------
         item
@@ -197,17 +211,15 @@
         --------
         aggregator = aggregator.order_by(
             aggregator.search.unique_tag
         )
         """
         if reverse:
             item = Reverse(item)
-        return self._new_with(
-            order_bys=self._order_bys + [item]
-        )
+        return self._new_with(order_bys=self._order_bys + [item])
 
     @property
     def search(self) -> FitQuery:
         """
         An object facilitating queries on fit attributes such as:
             name
             unique_tag
@@ -227,17 +239,15 @@
     @property
     def fits(self) -> List[m.Fit]:
         """
         Lazily query the database for a list of Fit objects that
         match the aggregator's predicate.
         """
         if self._fits is None:
-            self._fits = self._fits_for_query(
-                self._predicate.fit_query
-            )
+            self._fits = self._fits_for_query(self._predicate.fit_query)
         return self._fits
 
     def map(self, func):
         for fit in self.fits:
             yield func(fit)
 
     def __repr__(self):
@@ -285,22 +295,20 @@
         >>> )
         >>>
         >>> lens = aggregator.galaxies.lens
         >>>
         >>> aggregator.filter((lens.bulge == SersicCore) & (lens.disk == Sersic))
         >>> aggregator.filter((lens.bulge == SersicCore) | (lens.disk == Sersic))
         """
-        return self._new_with(
-            predicate=self._predicate & predicate
-        )
+        return self._new_with(predicate=self._predicate & predicate)
 
     def _new_with(
-            self,
-            type_=None,
-            **kwargs,
+        self,
+        type_=None,
+        **kwargs,
     ) -> "Aggregator":
         """
         Create a new instance with the same attribute values except
         for those overridden by kwargs
 
         Parameters
         ----------
@@ -315,111 +323,71 @@
         have been overridden
         """
         kwargs = {
             "session": self.session,
             "filename": self.filename,
             "predicate": self._predicate,
             "order_bys": self._order_bys,
-            **kwargs
+            "top_level_only": self._top_level_only,
+            **kwargs,
         }
         type_ = type_ or type(self)
-        return type_(
-            **kwargs
-        )
+        return type_(**kwargs)
 
     def __getitem__(self, item):
         offset = self._offset
         limit = self._limit
-        if isinstance(
-                item, int
-        ):
+        if isinstance(item, int):
             return self.fits[item]
-        elif isinstance(
-                item, slice
-        ):
+        elif isinstance(item, slice):
             if item.start is not None:
                 if item.start >= 0:
                     offset += item.start
                 else:
                     offset = len(self) + item.start
             if item.stop is not None:
                 if item.stop >= 0:
                     limit = len(self) - item.stop - offset
                 else:
                     limit = len(self) + item.stop
-        return self._new_with(
-            offset=offset,
-            limit=limit
-        )
+        return self._new_with(offset=offset, limit=limit)
 
-    def _fits_for_query(
-            self,
-            query: str
-    ) -> List[m.Fit]:
+    def _fits_for_query(self, query: str) -> List[m.Fit]:
         """
         Execute a raw SQL query and return a Fit object
         for each Fit id returned by the query
 
         Parameters
         ----------
         query
             A SQL query that selects ids from the fit table
 
         Returns
         -------
         A list of fit objects, one for each id returned by the
         query
         """
-        logger.debug(
-            f"Executing query: {query}"
-        )
-        fit_ids = {
-            row[0]
-            for row
-            in self.session.execute(
-                query
-            )
-        }
+        logger.debug(f"Executing query: {query}")
+        fit_ids = {row[0] for row in self.session.execute(query)}
 
-        logger.info(
-            f"{len(fit_ids)} fit(s) found matching query"
-        )
-        query = self.session.query(
-            m.Fit
-        ).filter(
-            m.Fit.id.in_(
-                fit_ids
-            )
-        )
+        logger.info(f"{len(fit_ids)} fit(s) found matching query")
+        query = self.session.query(m.Fit).filter(m.Fit.id.in_(fit_ids))
         for order_by in self._order_bys:
-            attribute = getattr(
-                m.Fit,
-                order_by.attribute
-            )
-
-            if isinstance(
-                    order_by,
-                    Reverse
-            ):
+            attribute = getattr(m.Fit, order_by.attribute)
+
+            if isinstance(order_by, Reverse):
                 attribute = sa.desc(attribute)
-            query = query.order_by(
-                attribute
-            )
-
-        return query.offset(
-            self._offset
-        ).limit(
-            self._limit
-        ).all()
-
-    def add_directory(
-            self,
-            directory: str,
-            auto_commit=True
-    ):
+            query = query.order_by(attribute)
+
+        fits = query.offset(self._offset).limit(self._limit).all()
+        if self._top_level_only:
+            return [fit for fit in fits if fit.parent is None]
+        return fits
+
+    def add_directory(self, directory: str, auto_commit=True):
         """
         Recursively search a directory for autofit results
         and add them to this database.
 
         Any pickles found in the pickles file are implicitly added
         to the fit object.
 
@@ -433,132 +401,132 @@
         auto_commit
             If True the session is committed writing the new objects
             to the database
         directory
             A directory containing autofit results embedded in a
             file structure
         """
-        scraper = Scraper(
-            directory,
-            self.session
-        )
+        scraper = Scraper(directory, self.session)
         scraper.scrape()
 
         if auto_commit:
             self.session.commit()
 
     @classmethod
     def from_database(
-            cls,
-            filename: str,
-            completed_only: bool = False
+        cls,
+        filename: str,
+        completed_only: bool = False,
+        top_level_only: bool = True,
     ) -> "Aggregator":
         """
         Create an instance from a sqlite database file.
 
         If no file exists then one is created with the schema of the database.
 
         Parameters
         ----------
         completed_only
+            If True only completed fits are returned
         filename
             The name of the database file.
+        top_level_only
+            If True only top level fits are returned
 
         Returns
         -------
         An aggregator connected to the database specified by the file.
         """
         from autofit.database import open_database
-        session = open_database(
-            str(filename)
-        )
-        aggregator = Aggregator(
-            session,
-            filename
-        )
+
+        session = open_database(str(filename))
+        aggregator = Aggregator(session, filename, top_level_only=top_level_only)
         if completed_only:
-            return aggregator(
-                aggregator.search.is_complete
-            )
+            return aggregator(aggregator.search.is_complete)
         return aggregator
 
     def grid_searches(self) -> "GridSearchAggregator":
         """
         Filter to only grid searches and return an aggregator
         with grid search specific functionality.
 
         Grid searches are initially implicitly ordered by their id
         """
         return cast(
             GridSearchAggregator,
             self._new_with(
                 type_=GridSearchAggregator,
                 predicate=self._predicate & self.search.is_grid_search,
-                order_bys=[Attribute("id")]
+                order_bys=[Attribute("id")],
+                top_level_only=False,
             ),
         )
 
 
 class GridSearchAggregator(Aggregator):
+    def __init__(
+        self,
+        session: sa.orm.Session,
+        filename: Optional[str] = None,
+        predicate: AbstractQuery = NullPredicate(),
+        offset=0,
+        limit=None,
+        order_bys=None,
+        top_level_only=False,
+    ):
+        super().__init__(
+            session=session,
+            filename=filename,
+            predicate=predicate,
+            offset=offset,
+            limit=limit,
+            order_bys=order_bys,
+            top_level_only=top_level_only,
+        )
+
     def best_fits(self) -> "GridSearchAggregator":
         """
         The best fit from each of the grid searches
 
         Best fits are initially implicitly ordered by their parent id
         """
         return self._new_with(
-            predicate=BestFitQuery(
-                self._predicate
-            ),
-            order_bys=[Attribute("parent_id")]
+            predicate=BestFitQuery(self._predicate), order_bys=[Attribute("parent_id")]
         )
 
     def children(self) -> "GridSearchAggregator":
         """
         An aggregator comprising the children of the fits encapsulated
         by this aggregator. This is used to query children in a grid search.
 
         Children are initially implicitly ordered by their parent id
         """
         return self._new_with(
-            predicate=q.ChildQuery(
-                self._predicate
-            ),
-            order_bys=[Attribute("parent_id")]
+            predicate=q.ChildQuery(self._predicate), order_bys=[Attribute("parent_id")]
         )
 
-    def cell_number(
-            self,
-            number: int
-    ) -> "CellAggregator":
+    def cell_number(self, number: int) -> "CellAggregator":
         """
         Create an aggregator for accessing all values for child fits
         with a given index, ordered by parameter values.
 
         Parameters
         ----------
         number
             The number of the fit in the grid search
 
         Returns
         -------
         An aggregator comprising fits for a given cell for each grid search
         """
-        return CellAggregator(
-            number,
-            self
-        )
+        return CellAggregator(number, self)
 
 
 class CellAggregator(AbstractAggregator):
-    def __init__(
-            self,
-            number: int,
-            aggregator: GridSearchAggregator
-    ):
+    def __init__(self, number: int, aggregator: GridSearchAggregator):
         """
         Aggregator for accessing data for a specific fit number in each
         grid search.
 
         Parameters
         ----------
         number
@@ -578,11 +546,11 @@
         """
         if self._fits is None:
             self._fits = list()
             for fit in self.aggregator:
                 self._fits.append(
                     sorted(
                         fit.children,
-                        key=lambda f: f.model.order_no if f.model is not None else 0
+                        key=lambda f: f.model.order_no if f.model is not None else 0,
                     )[self.number]
                 )
         return self._fits
```

### Comparing `autofit-2023.3.27.1/autofit/database/aggregator/scrape.py` & `autofit-2023.7.7.1/autofit/database/aggregator/scrape.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,40 +4,32 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from .. import model as m
 from ..sqlalchemy_ import sa
 from ...mapper.model_object import Identifier
 
-logger = logging.getLogger(
-    __name__
-)
+logger = logging.getLogger(__name__)
 
 
-def _parent_identifier(
-        directory: str
-) -> Optional[str]:
+def _parent_identifier(directory: str) -> Optional[str]:
     """
     Read the parent identifier for a fit in a directory.
 
     Defaults to None if no .parent_identifier file is found.
     """
     try:
         with open(f"{directory}/.parent_identifier") as f:
             return f.read()
     except FileNotFoundError:
         return None
 
 
 class Scraper:
-    def __init__(
-            self,
-            directory: Union[Path, str],
-            session: sa.orm.Session
-    ):
+    def __init__(self, directory: Union[Path, str], session: sa.orm.Session):
         """
         Facilitates scraping of data output into a directory
         into the database.
 
         Parameters
         ----------
         directory
@@ -50,157 +42,126 @@
 
     def scrape(self):
         """
         Recursively scrape fits from the directory and
         add them to the session
         """
         for fit in self._fits():
-            self.session.add(
-                fit
-            )
+            self.session.add(fit)
         for grid_search in self._grid_searches():
-            self.session.add(
-                grid_search
-            )
+            self.session.add(grid_search)
 
     def _fits(self):
         """
         Scrape data output into a directory tree so it can be added to the
         aggregator database.
 
         Returns
         -------
         Generator yielding Fit database objects
         """
-        logger.info(
-            f"Scraping directory {self.directory}"
-        )
+        logger.info(f"Scraping directory {self.directory}")
         from autofit.aggregator.aggregator import Aggregator as ClassicAggregator
-        aggregator = ClassicAggregator(
-            self.directory
-        )
-        logger.info(
-            f"{len(aggregator)} searches found"
-        )
-        for item in aggregator:
 
-            is_complete = os.path.exists(
-                f"{item.directory}/.completed"
-            )
+        aggregator = ClassicAggregator(self.directory)
+        logger.info(f"{len(aggregator)} searches found")
+        for item in aggregator:
+            is_complete = os.path.exists(f"{item.directory}/.completed")
 
-            parent_identifier = _parent_identifier(
-                directory=item.directory
-            )
+            parent_identifier = _parent_identifier(directory=item.directory)
 
             model = item.model
             samples = item.samples
 
             identifier = _make_identifier(item)
 
             logger.info(
                 f"Creating fit for: "
                 f"{item.search.paths.path_prefix} "
                 f"{item.search.unique_tag} "
                 f"{item.search.name} "
-                f"{identifier} ")
+                f"{identifier} "
+            )
 
             try:
                 instance = samples.max_log_likelihood()
             except (AttributeError, NotImplementedError):
                 instance = None
 
             try:
-                fit = self._retrieve_model_fit(
-                    item
-                )
-                logger.warning(
-                    f"Fit already existed with identifier {identifier}"
-                )
+                fit = self._retrieve_model_fit(item)
+                logger.warning(f"Fit already existed with identifier {identifier}")
             except sa.orm.exc.NoResultFound:
                 try:
                     log_likelihood = samples.max_log_likelihood_sample.log_likelihood
                 except AttributeError:
                     log_likelihood = None
                 fit = m.Fit(
                     id=identifier,
                     name=item.search.name,
                     unique_tag=item.search.unique_tag,
                     model=model,
                     instance=instance,
                     is_complete=is_complete,
                     info=item.info,
                     max_log_likelihood=log_likelihood,
-                    parent_id=parent_identifier
+                    parent_id=parent_identifier,
                 )
 
             pickle_path = Path(item.pickle_path)
-            _add_pickles(
-                fit,
-                pickle_path
-            )
+            _add_pickles(fit, pickle_path)
+            for i, child_analysis in enumerate(item.child_analyses):
+                child_fit = m.Fit(
+                    id=f"{identifier}_{i}",
+                )
+                _add_pickles(child_fit, child_analysis.pickle_path)
+                fit.children.append(child_fit)
 
             yield fit
 
-    def _grid_searches(
-            self
-    ):
+    def _grid_searches(self):
         """
         Retrieve grid searches recursively from an output directory by
         searching for the .is_grid_search file.
 
         Should be called after adding Fits as it relies on querying fits
 
         Yields
         ------
         Fit objects representing grid searches with child fits associated
         """
         from autofit.aggregator.aggregator import Aggregator as ClassicAggregator
+
         for root, _, filenames in os.walk(self.directory):
             if ".is_grid_search" in filenames:
                 path = Path(root)
 
                 is_complete = (path / ".completed").exists()
 
-                with open(
-                        path / ".is_grid_search"
-                ) as f:
+                with open(path / ".is_grid_search") as f:
                     unique_tag = f.read()
 
                 grid_search = m.Fit(
                     id=path.name,
                     unique_tag=unique_tag,
                     is_grid_search=True,
-                    parent_id=_parent_identifier(
-                        root
-                    ),
-                    is_complete=is_complete
+                    parent_id=_parent_identifier(root),
+                    is_complete=is_complete,
                 )
 
                 pickle_path = path / "pickles"
-                _add_pickles(
-                    grid_search,
-                    pickle_path
-                )
+                _add_pickles(grid_search, pickle_path)
 
-                aggregator = ClassicAggregator(
-                    root
-                )
+                aggregator = ClassicAggregator(root)
                 for item in aggregator:
-                    fit = self._retrieve_model_fit(
-                        item
-                    )
-                    grid_search.children.append(
-                        fit
-                    )
+                    fit = self._retrieve_model_fit(item)
+                    grid_search.children.append(fit)
                 yield grid_search
 
-    def _retrieve_model_fit(
-            self,
-            item
-    ) -> m.Fit:
+    def _retrieve_model_fit(self, item) -> m.Fit:
         """
         Retrieve a Fit, if one exists, corresponding to a given SearchOutput
 
         Parameters
         ----------
         item
             A SearchOutput from the classic Aggregator
@@ -210,26 +171,20 @@
         A fit with the corresponding identifier
 
         Raises
         ------
         NoResultFound
             If no fit is found with the identifier
         """
-        return self.session.query(
-            m.Fit
-        ).filter(
-            m.Fit.id == _make_identifier(
-                item
-            )
-        ).one()
+        return (
+            self.session.query(m.Fit).filter(m.Fit.id == _make_identifier(item)).one()
+        )
 
 
-def _make_identifier(
-        item
-) -> str:
+def _make_identifier(item) -> str:
     """
     Create a unique identifier for a SearchOutput.
 
     This accounts for the Search, Model and unique_tag
 
     Parameters
     ----------
@@ -239,52 +194,38 @@
     Returns
     -------
     A unique identifier that is sensitive to changes that affect
     the search
     """
     search = item.search
     model = item.model
-    return str(Identifier([
-        search,
-        model,
-        search.unique_tag
-    ]))
+    return str(Identifier([search, model, search.unique_tag]))
 
 
-def _add_pickles(
-        fit: m.Fit,
-        pickle_path: Path
-):
+def _add_pickles(fit: m.Fit, pickle_path: Path):
     """
     Load pickles from the path and add them to the database.
 
     Parameters
     ----------
     fit
         A fit to which the pickles belong
     pickle_path
         The path in which the pickles are stored
     """
     try:
-        filenames = os.listdir(
-            pickle_path
-        )
+        filenames = os.listdir(pickle_path)
     except FileNotFoundError as e:
         logger.exception(e)
         filenames = []
 
     for filename in filenames:
-
         try:
-            with open(
-                    pickle_path / filename,
-                    "r+b"
-            ) as f:
-                fit[
-                    filename.split(".")[0]
-                ] = pickle.load(f)
+            with open(pickle_path / filename, "r+b") as f:
+                fit[filename.split(".")[0]] = pickle.load(f)
         except (pickle.UnpicklingError, ModuleNotFoundError) as e:
-
             if filename == "dynesty.pickle":
                 continue
 
-            raise pickle.UnpicklingError(f"Failed to unpickle: {pickle_path} {filename}") from e
+            raise pickle.UnpicklingError(
+                f"Failed to unpickle: {pickle_path} {filename}"
+            ) from e
```

### Comparing `autofit-2023.3.27.1/autofit/database/migration/migration.py` & `autofit-2023.7.7.1/autofit/database/migration/migration.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/migration/session_wrapper.py` & `autofit-2023.7.7.1/autofit/database/migration/session_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/model/fit.py` & `autofit-2023.7.7.1/autofit/database/model/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,15 +135,18 @@
                 return named_instance
         raise KeyError(f"Instance {item} not found")
 
 
 class Fit(Base):
     __tablename__ = "fit"
 
-    id = sa.Column(sa.String, primary_key=True,)
+    id = sa.Column(
+        sa.String,
+        primary_key=True,
+    )
     is_complete = sa.Column(sa.Boolean)
 
     _named_instances: List[NamedInstance] = sa.orm.relationship("NamedInstance")
 
     @property
     @try_none
     def instance(self):
@@ -169,14 +172,20 @@
 
     parent_id = sa.Column(sa.String, sa.ForeignKey("fit.id"))
 
     children: List["Fit"] = sa.orm.relationship(
         "Fit", backref=sa.orm.backref("parent", remote_side=[id])
     )
 
+    def child_values(self, name):
+        """
+        Get the values of a given key for all children
+        """
+        return [child[name] for child in self.children]
+
     @property
     def best_fit(self) -> "Fit":
         """
         Only for grid searches. Returns the child search with
         the highest log likelihood.
         """
         if not self.is_grid_search:
```

### Comparing `autofit-2023.3.27.1/autofit/database/model/instance.py` & `autofit-2023.7.7.1/autofit/database/model/instance.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/model/model.py` & `autofit-2023.7.7.1/autofit/database/model/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/model/prior.py` & `autofit-2023.7.7.1/autofit/database/model/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/query/condition.py` & `autofit-2023.7.7.1/autofit/database/query/condition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Set, Optional
 
 from autofit.database.model import get_class_path
 
 
 class Table:
-    def __init__(
-            self,
-            name: str,
-            abbreviation: Optional[str] = None
-    ):
+    def __init__(self, name: str, abbreviation: Optional[str] = None):
         """
         A table containing some type of object in the database.
 
         object is parent to all other tables.
         value contains any numeric values.
         string_value contains any string values.
 
@@ -71,44 +67,33 @@
 
     @abstractmethod
     def __str__(self):
         """
         The condition written as SQL
         """
 
-    def __and__(
-            self,
-            other:
-            "AbstractCondition"
-    ):
+    def __and__(self, other: "AbstractCondition"):
         """
         Combine this and another query with an AND statement.
-        
+
         Simplification is applied so that the query will execute as fast as possible.
         """
         from .junction import And
-        return And(
-            self,
-            other
-        )
-
-    def __or__(
-            self,
-            other: "AbstractCondition"
-    ):
+
+        return And(self, other)
+
+    def __or__(self, other: "AbstractCondition"):
         """
         Combine this and another query with an AND statement.
 
         Simplification is applied so that the query will execute as fast as possible.
         """
         from .junction import Or
-        return Or(
-            self,
-            other
-        )
+
+        return Or(self, other)
 
     def __hash__(self):
         return hash(str(self))
 
     def __eq__(self, other):
         return str(self) == str(other)
 
@@ -119,29 +104,24 @@
         return str(self) < str(other)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {str(self)}>"
 
 
 class NoneCondition(AbstractCondition):
-
     @property
     def tables(self) -> Set[Table]:
         return {none_table}
 
     def __str__(self):
         return "1 = 1"
 
 
 class AbstractValueCondition(AbstractCondition, ABC):
-    def __init__(
-            self,
-            symbol: str,
-            value
-    ):
+    def __init__(self, symbol: str, value):
         """
         A condition which compares the named column to a value
 
         Parameters
         ----------
         symbol
             =, <=, >=, < or >
@@ -234,17 +214,15 @@
         return f"{object_table.abbreviation}.class_path = '{self.class_path}'"
 
     @property
     def class_path(self) -> str:
         """
         The full import path of the type
         """
-        return get_class_path(
-            self.cls
-        )
+        return get_class_path(self.cls)
 
 
 class AttributeCondition(AbstractCondition, ABC):
     def __init__(self, attribute, value):
         self.attribute = attribute
         self._value = value
 
@@ -256,22 +234,21 @@
     def __str__(self):
         pass
 
 
 class EqualityAttributeCondition(AttributeCondition):
     @property
     def value(self):
-        if isinstance(
-                self._value,
-                str
-        ):
+        if isinstance(self._value, str):
             return f"'{self._value}'"
         return self._value
 
     def __str__(self):
+        if self._value is None:
+            return f"{self.attribute} IS NULL"
         return f"{self.attribute} = {self.value}"
 
 
 class ContainsAttributeCondition(AttributeCondition):
     def __str__(self):
         return f"{self.attribute} LIKE '%{self._value}%'"
```

### Comparing `autofit-2023.3.27.1/autofit/database/query/junction.py` & `autofit-2023.7.7.1/autofit/database/query/junction.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/query/query/abstract.py` & `autofit-2023.7.7.1/autofit/database/query/query/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/query/query/attribute.py` & `autofit-2023.7.7.1/autofit/database/query/query/attribute.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,99 +20,73 @@
         Parameters
         ----------
         attribute
             The name of that attribute
         """
         self.attribute = attribute
 
-    def _make_query(
-            self,
-            cls,
-            value
-    ) -> AttributeQuery:
+    def _make_query(self, cls, value) -> AttributeQuery:
         """
         Create a query against this attribute
 
         Parameters
         ----------
         cls
             An AttributeCondition that describes the query
         value
             The value that the attribute is compared to
 
         Returns
         -------
         A query on ids of the fit table
         """
-        return AttributeQuery(
-            cls(
-                attribute=self.attribute,
-                value=value
-            )
-        )
+        return AttributeQuery(cls(attribute=self.attribute, value=value))
 
     def __eq__(self, other) -> AttributeQuery:
         """
         Check whether an attribute, such as a search name, is equal
         to some value
         """
-        return self._make_query(
-            cls=c.EqualityAttributeCondition,
-            value=other
-        )
+        return self._make_query(cls=c.EqualityAttributeCondition, value=other)
 
     def in_(self, item: str) -> AttributeQuery:
         """
         Check whether an attribute is contained within a substring
         """
-        return self._make_query(
-            cls=c.InAttributeCondition,
-            value=item
-        )
+        return self._make_query(cls=c.InAttributeCondition, value=item)
 
     def contains(self, item: str) -> AttributeQuery:
         """
         Check whether an attribute, such as a search name, contains
         some string
         """
-        return self._make_query(
-            cls=c.ContainsAttributeCondition,
-            value=item
-        )
+        return self._make_query(cls=c.ContainsAttributeCondition, value=item)
 
 
 class BooleanAttribute(Attribute, AttributeQuery):
     def __init__(self, attribute):
         super().__init__(attribute)
-        super(AttributeQuery, self).__init__(
-            c.AttributeCondition(
-                attribute
-            )
-        )
+        super(AttributeQuery, self).__init__(c.AttributeCondition(attribute))
 
     def __hash__(self):
         return hash(str(self))
 
 
 class ChildQuery(AttributeQuery):
     def __init__(self, predicate: AbstractQuery):
-        super().__init__(
-            predicate
-        )
+        super().__init__(predicate)
 
     @property
     def condition(self):
         return f"parent_id in ({super().condition})"
 
 
 class BestFitQuery(ChildQuery):
     def __init__(self, predicate: AbstractQuery):
-        super().__init__(
-            predicate
-        )
+        super().__init__(predicate)
 
     @property
     def fit_query(self) -> str:
         return f"""WITH children AS (
                     SELECT id, parent_id, max_log_likelihood 
                     FROM fit WHERE {self.condition}
                    ),
```

### Comparing `autofit-2023.3.27.1/autofit/database/query/query/info.py` & `autofit-2023.7.7.1/autofit/database/query/query/info.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/query/query/named.py` & `autofit-2023.7.7.1/autofit/database/query/query/named.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/database/sqlalchemy_.py` & `autofit-2023.7.7.1/autofit/database/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/example/model.py` & `autofit-2023.7.7.1/autofit/example/model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/example/util.py` & `autofit-2023.7.7.1/autofit/example/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/exc.py` & `autofit-2023.7.7.1/autofit/exc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/fixtures.py` & `autofit-2023.7.7.1/autofit/fixtures.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/__init__.py` & `autofit-2023.7.7.1/autofit/graphical/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/abstract.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -220,14 +220,16 @@
 
         return EPResult(
             ep_history=opt.ep_history,
             declarative_factor=self,
             updated_ep_mean_field=updated_ep_mean_field,
         )
 
+    # TODO : Visualize method before fit?
+
     def visualize(
             self,
             paths: AbstractPaths,
             instance: ModelInstance,
             during_analysis: bool
     ):
         """
@@ -249,14 +251,20 @@
                 instance
         ):
             model_factor.visualize(
                 paths,
                 instance,
                 during_analysis
             )
+            model_factor.visualize_combined(
+                None,
+                paths,
+                instance,
+                during_analysis
+            )
 
     @property
     def global_prior_model(self) -> Collection:
         """
         A collection of prior models, with one model for each factor.
         """
         return GlobalPriorModel(self)
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/collection.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/collection.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/factor/abstract.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/factor/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/factor/analysis.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/factor/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,17 +121,18 @@
             Object describing where data should be saved to
         instance
             A collection of instances, each corresponding to a factor
         during_analysis
             Is this visualisation during analysis?
         """
         self.analysis.visualize(
-            paths,
-            instance,
-            during_analysis
+            paths=paths, instance=instance, during_analysis=during_analysis
+        )
+        self.analysis.visualize_combined(
+            analyses=None, paths=paths, instance=instance, during_analysis=during_analysis
         )
 
     def log_likelihood_function(
             self,
             instance: ModelInstance
     ) -> float:
         return self.analysis.log_likelihood_function(instance)
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/factor/hierarchical.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/factor/hierarchical.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/factor/prior.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/factor/prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/graph.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/declarative/result.py` & `autofit-2023.7.7.1/autofit/graphical/declarative/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/expectation_propagation/ep_mean_field.py` & `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/ep_mean_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,14 @@
         factor_mean_field = self._factor_mean_field.copy()
         factor_dist = factor_mean_field.pop(factor)
         cavity_dist = MeanField({
             v: 1.0
             for v in factor_dist.all_variables
         }).prod(
             *factor_mean_field.values(),
-            default=factor_dist,
         )
 
         model_dist = factor_dist.prod(cavity_dist, default=factor)
 
         return FactorApproximation(factor, cavity_dist, factor_dist, model_dist)
 
     get_factor_approx = factor_approximation
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/expectation_propagation/factor_optimiser.py` & `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/factor_optimiser.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,15 +27,24 @@
     ) -> Tuple[MeanField, Status]:
         pass
 
     def exact_fit(
         self, factor_approx: FactorApproximation, status: Status = Status()
     ) -> Tuple[MeanField, Status]:
         factor = factor_approx.factor
-        cavity_dist = factor_approx.cavity_dist
+        cavity_dist = factor_approx.cavity_dist.copy()
+
+        """For exact_fits of FactorApproximations we need the full cavity_dist, 
+        so in this case we need to create zeros_like versions of the missing 
+        cavity_dists - e.g. for the Normal Distribution the zeros_like dist 
+        has infinite variance, note that its logpdf will be - inf 
+        so we don't want to evaluate it in general."""
+        for v in factor_approx.mean_field.keys() - cavity_dist:
+            cavity_dist[v] = factor_approx.mean_field[v].zeros_like()
+
         with LogWarnings(logger=self.logger, action="always") as caught_warnings:
             if factor._calc_exact_update:
                 factor_mean_field = factor.calc_exact_update(cavity_dist)
                 new_model_dist = factor_mean_field * cavity_dist
             elif factor._calc_exact_projection:
                 new_model_dist = factor.calc_exact_projection(cavity_dist)
             else:
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/expectation_propagation/history.py` & `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/history.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/expectation_propagation/optimiser.py` & `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/optimiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,14 @@
             Optionally specify an alternate history
         factor_order
             The factors in the graph but placed in the order in which they should
             be optimised
         paths
             Optionally define how data should be output
         """
-        self.paths = paths or DirectoryPaths(identifier=str(Identifier(factor_graph)))
-
         factor_optimisers = factor_optimisers or {}
         self.factor_graph = factor_graph
         self.factors = factor_order or self.factor_graph.factors
         self.default_optimiser = default_optimiser
         self.updater = updater or SimplerUpdater(delta=1.0)
 
         if default_optimiser is None:
@@ -184,23 +182,34 @@
                 )
         else:
             self.factor_optimisers = {
                 factor: factor_optimisers.get(factor, default_optimiser)
                 for factor in self.factors
             }
 
-        for optimiser in self.factor_optimisers.values():
-            optimiser.paths = self.paths
-
+            
         self.ep_history = ep_history or EPHistory()
 
-        with open(self.output_path / "graph.info", "w+") as f:
-            f.write(self.factor_graph.info)
+        self.visualiser = None
+        if paths is None:
+            try:
+                paths = DirectoryPaths(identifier=str(Identifier(factor_graph)))
+            except KeyError: 
+                pass 
+
+        self.paths = paths
+        if self.paths:
+            for optimiser in self.factor_optimisers.values():
+                # optimiser.paths = optimiser_paths or self.paths
+                optimiser.paths = self.paths
+
+            with open(self.output_path / "graph.info", "w+") as f:
+                f.write(self.factor_graph.info)
 
-        self.visualiser = Visualise(self.ep_history, self.output_path)
+            self.visualiser = Visualise(self.ep_history, self.output_path)
 
     @classmethod
     def from_meanfield(
         cls,
         model_approx: EPMeanField,
         default_optimiser: Optional[AbstractFactorOptimiser] = None,
         factor_optimisers: Optional[Dict[Factor, AbstractFactorOptimiser]] = None,
@@ -228,23 +237,26 @@
             factor_optimisers=factor_optimisers,
             ep_history=ep_history,
             factor_order=factor_order,
             paths=paths,
         )
 
     @property
-    def output_path(self) -> Path:
+    def output_path(self) -> Optional[Path]:
         """
         The path at which data will be output. Uses the name of the optimiser.
 
         If the path does not exist it is created.
         """
-        path = Path(self.paths.output_path)
-        os.makedirs(path, exist_ok=True)
-        return path
+        if self.paths:
+            path = Path(self.paths.output_path)
+            os.makedirs(path, exist_ok=True)
+            return path
+        
+        return None
 
     def _log_factor(self, factor: Factor):
         """
         Log information for the factor and its history.
         """
         factor_logger = logging.getLogger(factor.name)
         try:
@@ -312,32 +324,34 @@
                     self._log_factor(factor)
 
                 if self.ep_history(factor, model_approx, status):
                     logger.info("Terminating optimisation")
                     break  # callback controls convergence
 
             else:  # If no break do next iteration
-                if _should_visualise:
+                if self.visualiser and _should_visualise:
                     self.visualiser()
-                if _should_output:
+                if self.output_path and _should_output:
                     self._output_results(model_approx)
                 continue
             break  # stop iterations
 
-        self.visualiser()
-        self._output_results(model_approx)
+        if self.paths:
+            self.visualiser()
+            self._output_results(model_approx)
 
         return model_approx
 
     def _output_results(self, model_approx: EPMeanField):
         """
         Save the graph.results text
         """
-        with open(self.output_path / "graph.results", "w+") as f:
-            f.write(self.factor_graph.make_results_text(model_approx))
+        if self.paths:
+            with open(self.output_path / "graph.results", "w+") as f:
+                f.write(self.factor_graph.make_results_text(model_approx))
 
 
 class ParallelEPOptimiser(EPOptimiser):
     def __init__(
         self,
         factor_graph: FactorGraph,
         n_cores: int,
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/expectation_propagation/stochastic.py` & `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/stochastic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/expectation_propagation/visualise.py` & `autofit-2023.7.7.1/autofit/graphical/expectation_propagation/visualise.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/factor_graphs/abstract.py` & `autofit-2023.7.7.1/autofit/graphical/factor_graphs/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 import numpy as np
 
 from autoconf import cached_property
 from autofit.graphical.utils import (
     FlattenArrays,
     nested_filter,
     nested_update,
+    nested_zip,
+    nested_set, 
+    nested_map, 
+    nested_items, 
     is_variable,
     Status, 
 )
 from autofit.mapper.variable import (
     Variable,
     Plate,
     FactorValue,
@@ -88,26 +92,26 @@
             for v, x in values.items()
             if v.name in self.variable_name_kw
         }
 
     def resolve_args(
             self, values: Dict[Variable, np.ndarray]
     ) -> Tuple[np.ndarray, ...]:
-        return (values[k] for k in self.args)
+        return nested_update(self.args, values)
 
     @cached_property
     def fixed_values(self) -> VariableData:
         return VariableData()
 
     @cached_property
     def variables(self) -> Set[Variable]:
         """
         Dictionary mapping the names of variables to those variables
         """
-        return frozenset(self._kwargs.values())
+        return frozenset(self.flat_args)
 
     @property
     def free_variables(self) -> Set[Variable]:
         return self.variables - self.fixed_values.keys()
 
     @property
     def kwargs(self) -> Dict[str, Variable]:
@@ -117,20 +121,24 @@
     def kwargs(self, kwargs):
         del self.variables
         del self.name_variable_dict
         del self.variable_name_dict
         self._kwargs = kwargs
 
     @property
-    def args(self) -> Tuple[Variable, ...]:
+    def args(self) -> Tuple[Any, ...]:
         return tuple(self.kwargs.values())
 
     @property
     def arg_names(self) -> Tuple[str, ...]:
         return tuple(self.kwargs)
+    
+    @property 
+    def flat_args(self) -> Tuple[Variable, ...]:
+        return tuple(x for x, in nested_zip(self._kwargs))
 
     @property
     def factor_out(self):
         return self._factor_out
 
     @factor_out.setter
     def factor_out(self, factor_out):
@@ -241,15 +249,15 @@
         pass
 
     @property
     def _unique_representation(self):
         return (
             self._factor,
             self.arg_names,
-            self.args,
+            self.flat_args,
             self.deterministic_variables,
         )
 
     def __hash__(self):
         return hash(self._unique_representation)
 
     def __eq__(self, other) -> bool:
@@ -268,47 +276,49 @@
         same values (within numerical precision of the finite differences)
 
         factor._numerical_factor_jacobian(*args)
 
         factor._factor(*args), jax.jacobian(factor._factor, range(len(args)))(*args)
         """
         eps = eps or self.eps
-        args = tuple(np.array(value, dtype=np.float64) for value in args)
+
+        args = nested_map(lambda _, val: np.array(val, dtype=np.float64), self.args, args)
 
         raw_fval0 = self._factor_args(*args)
         fval0 = self._factor_value(raw_fval0).to_dict()
 
         jac = {
-            v0: tuple(
-                np.empty_like(val, shape=np.shape(val) + np.shape(value))
-                for value in args
-            )
-            for v0, val in fval0.items()
+            v0: nested_map(
+                lambda _, v: np.empty_like(val, shape=np.shape(val) + np.shape(v)),
+                self.args, args
+            ) for v0, val in fval0.items()
         }
-        for i, val in enumerate(args):
+        for ks, _, val in nested_items(self.args, args):
             with np.nditer(val, op_flags=["readwrite"], flags=["multi_index"]) as it:
                 for x_i in it:
                     val[it.multi_index] += eps
                     fval1 = self._factor_value(self._factor_args(*args)).to_dict()
                     jac_v1_i = (fval1 - fval0) / eps
                     x_i -= eps
                     indexes = (Ellipsis,) + it.multi_index
                     for v0, jac_v0v_i in jac_v1_i.items():
-                        jac[v0][i][indexes] = jac_v0v_i
+                        key_path = (v0, *ks, indexes)
+                        nested_set(jac, key_path, jac_v0v_i)
+                        # jac[v0][i][indexes] = jac_v0v_i
 
         # This replicates the output of normal
         # jax.jacobian(self.factor, len(self.args))(*args)
         jac_out = nested_update(self.factor_out, jac)
 
         return raw_fval0, jac_out
 
     def numerical_func_jacobian(
             self, values: VariableData, **kwargs
     ) -> tuple:
-        args = (values[k] for k in self.args)
+        args = self.resolve_args(values)
         raw_fval, raw_jac = self._numerical_factor_jacobian(*args, **kwargs)
         fval = self._factor_value(raw_fval)
         jvp = self._jac_out_to_jvp(raw_jac, values=fval.to_dict().merge(values))
         return fval, jvp
 
     def jacobian(self, values: Dict[Variable, np.array], **kwargs):
         return self.func_jacobian(values, **kwargs)[1]
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/factor_graphs/factor.py` & `autofit-2023.7.7.1/autofit/graphical/factor_graphs/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
     _HAS_JAX = True
 except ImportError:
     _HAS_JAX = False
 
 from autofit.graphical.utils import (
     nested_filter,
+    to_variabledata, 
+    nested_zip, 
     is_variable,
     try_getitem,
 )
 from autofit.mapper.variable import Variable, Plate, VariableData
 
 from autofit.graphical.factor_graphs.abstract import FactorValue, AbstractFactor
 
@@ -187,15 +189,14 @@
             self,
             name=name,
             plates=plates,
             factor_out=factor_out,
             **kwargs,
         )
 
-        # self.factor_out = factor_out
         self.eps = eps
         self._set_factor(factor)
         self._set_jacobians(
             vjp=vjp,
             factor_vjp=factor_vjp,
             factor_jacobian=factor_jacobian,
             jacobian=jacobian,
@@ -315,24 +316,24 @@
                     self._jacobian = jax.jacobian(self._factor, range(self.n_args))
 
     def _factor_value(self, raw_fval) -> FactorValue:
         """Converts the raw output of the factor into a `FactorValue`
         where the values of the deterministic values are stored in a dict
         attribute `FactorValue.deterministic_values`
         """
-        det_values = VariableData(nested_filter(is_variable, self.factor_out, raw_fval))
+        det_values = to_variabledata(self.factor_out, raw_fval)
         fval = det_values.pop(FactorValue, 0.0)
         return FactorValue(fval, det_values)
 
     def __call__(self, values: VariableData) -> FactorValue:
         """Calls the factor with the values specified by the dictionary of
         values passed, returns a FactorValue with the value returned by the
         factor, and any deterministic factors"""
-        args = [values[v] for v in self.args]
-        key = self._key("__call__", *args)
+        args = self.resolve_args(values)
+        key = self._key("__call__", *(val for _, val in nested_zip(self.args, args)))
 
         if key not in self._cache:
             raw_fval = self._factor_args(*args)
             self._cache[key] = self._factor_value(raw_fval)
         return self._cache[key]
 
     def _jax_factor_vjp(self, *args) -> Tuple[Any, Callable]:
@@ -347,15 +348,15 @@
         values, and a `VectorJacobianProduct` operator that allows the
         calculation of the gradient of the input values to be calculated
         with respect to the gradients of the output values (i.e backprop)
         """
         from autofit.graphical.factor_graphs.jacobians import (
             VectorJacobianProduct,
         )
-        raw_fval, fvjp = self._factor_vjp(*(values[v] for v in self.args))
+        raw_fval, fvjp = self._factor_vjp(*self.resolve_args(values))
         fval = self._factor_value(raw_fval)
 
         fvjp_op = VectorJacobianProduct(
             self.factor_out,
             fvjp,
             *self.args,
             out_shapes=fval.to_dict().shapes,
@@ -376,15 +377,15 @@
                 h.update(np.array(arg))
 
         return h.intdigest()
 
     def _jvp_func_jacobian(
             self, values: VariableData, **kwargs
     ) -> Tuple[FactorValue, "JacobianVectorProduct"]:
-        args = list(values[k] for k in self.args)
+        args = self.resolve_args(values)
         key = self._key("_jvp_func_jacobian", *args)
 
         if key not in self._cache:
             raw_fval, raw_jac = self._factor_jacobian(*args, **kwargs)
             fval = self._factor_value(raw_fval)
             jvp = self._jac_out_to_jvp(raw_jac, values=fval.to_dict().merge(values))
             self._cache[key] = (fval, jvp)
@@ -398,15 +399,15 @@
     def _factor_args(self, *args):
         return self._factor(*args)
 
     def _unpack_jacobian_out(self, raw_jac: Any) -> Dict[Variable, VariableData]:
         jac = {}
         for v0, vjac in nested_filter(is_variable, self.factor_out, raw_jac):
             jac[v0] = VariableData()
-            for v1, j in zip(self.args, vjac):
+            for v1, j in nested_zip(self.args, vjac):
                 jac[v0][v1] = j
 
         return jac
 
     def _jac_out_to_jvp(
             self, raw_jac: Any, values: VariableData
     ) -> "JacobianVectorProduct":
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/factor_graphs/graph.py` & `autofit-2023.7.7.1/autofit/graphical/factor_graphs/graph.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/factor_graphs/jacobians.py` & `autofit-2023.7.7.1/autofit/graphical/factor_graphs/jacobians.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import numpy as np
 
 from autoconf import cached_property
 from autofit.graphical.utils import (
     nested_filter,
     nested_update,
     is_variable,
+    to_variabledata,
 )
 from autofit.mapper.variable import (
     Variable,
     FactorValue,
     VariableData,
     VariableLinearOperator,
 )
@@ -110,17 +111,19 @@
         return f"{cls_name}({out_var} → ∂({in_var})ᵀ {out_var})"
 
     def grad(self, values=None):
         grad = VariableData({FactorValue: 1.0})
         if values:
             grad.update(values)
 
-        for v, g in self(grad).items():
+        jac = self(grad)
+        for v, g in jac.items():
             grad[v] = grad.get(v, 0) + g
 
+        grad.pop(FactorValue)
         return grad
 
 
 class JacobianVectorProduct(AbstractJacobian, RectVariableOperator):
     __init__ = RectVariableOperator.__init__
 
     @property
@@ -134,21 +137,26 @@
     @property
     def factor_out(self):
         return tuple(self.out_variables)
 
 
 class VectorJacobianProduct(AbstractJacobian):
     def __init__(
-            self, factor_out, vjp: Callable, *variables: Variable, out_shapes=None
+            self, factor_out, vjp: Callable, *args: Variable, out_shapes=None
     ):
         self.factor_out = factor_out
         self.vjp = vjp
-        self._variables = variables
+        self._args = args
+        self._variables = tuple(v for v, in nested_filter(is_variable, args))
         self.out_shapes = out_shapes
 
+    @property 
+    def args(self):
+        return self._args 
+
     @property
     def variables(self):
         return self._variables
 
     @cached_property
     def out_variables(self):
         return set(v[0] for v in nested_filter(is_variable, self.factor_out))
@@ -168,15 +176,15 @@
             values = float(values)
 
         return values
 
     def __call__(self, values: Union[VariableData, FactorValue]) -> VariableData:
         v = self._get_cotangent(values)
         grads = self.vjp(v)
-        return VariableData(zip(self.variables, grads))
+        return to_variabledata(self.args, grads)
 
     __rmul__ = __call__
 
     def _not_implemented(self, *args):
         raise NotImplementedError()
 
     __rtruediv__ = _not_implemented
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/factor_graphs/transform.py` & `autofit-2023.7.7.1/autofit/graphical/factor_graphs/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/laplace/line_search.py` & `autofit-2023.7.7.1/autofit/graphical/laplace/line_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/laplace/newton.py` & `autofit-2023.7.7.1/autofit/graphical/laplace/newton.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     zk = yk + Bk * dk
     dzk = dk * zk
     # alpha = -zk.dot(dk) / dzk.dot(dzk)
 
     d = dzk.dot(dzk)
     if d > tol * dk.norm() ** 2 * zk.norm() ** 2:
         alpha = -zk.dot(dk) / d
-        Bk = Bk.diagonalupdate(alpha * (zk ** 2))
+        Bk = Bk.diagonalupdate((zk ** 2) * alpha)
 
     state1.hessian = Bk
     return state1
 
 
 def diag_sr1_update_(
     state1: OptimisationState, state: OptimisationState, tol=1e-8, **kwargs
@@ -89,15 +89,15 @@
     tols = tol * dk.var_norm() ** 2 * zk.var_norm() ** 2
     for v, d in (dzk ** 2).var_sum().items():
         if d > tols[v]:
             alpha[v] /= d
         else:
             alpha[v] = 0.0
 
-    Bk = Bk.diagonalupdate(alpha * (zk ** 2))
+    Bk = Bk.diagonalupdate((zk ** 2) * alpha)
 
     state1.hessian = Bk
     return state1
 
 
 def diag_sr1_bfgs_update(
     state1: OptimisationState, state: OptimisationState, **kwargs
@@ -180,15 +180,15 @@
     zk = VariableData.sub(
         state1.value.deterministic_values, state.value.deterministic_values
     )
     Bxk, Bzk = state1.hessian, state.det_hessian
     zk2 = zk ** 2
     zk4 = (zk2 ** 2).sum()
     alpha = (dk.dot(Bxk.dot(dk)) - zk.dot(Bzk.dot(zk))) / zk4
-    state1.det_hessian = Bzk.diagonalupdate(float(alpha) * zk2)
+    state1.det_hessian = Bzk.diagonalupdate(zk2 * alpha)
 
     return state1
 
 
 class QuasiNewtonUpdate:
     def __init__(self, quasi_newton_update, det_quasi_newton_update):
         self.quasi_newton_update = quasi_newton_update
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/laplace/optimiser.py` & `autofit-2023.7.7.1/autofit/graphical/laplace/optimiser.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/graphical/mean_field.py` & `autofit-2023.7.7.1/autofit/graphical/mean_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from collections import ChainMap
 from numbers import Real
 from typing import Dict, Tuple, Optional, Union, Iterable
+from operator import attrgetter
 
 import numpy as np
 
 from autoconf import cached_property
 from autofit import exc
 from autofit.graphical.factor_graphs.abstract import AbstractNode
 from autofit.graphical.factor_graphs.factor import Factor
@@ -85,14 +86,17 @@
         if isinstance(dists, MeanField):
             self.log_norm = dists.log_norm
             self._plates = dists.plates
         else:
             self.log_norm = log_norm
             self._plates = self.sorted_plates if plates is None else plates
 
+    def copy(self) -> "MeanField":
+        return type(self)(self)
+
     def __radd__(self, other):
         return self + other
 
     def __add__(self, other):
         return type(self)(
             {variable: message + other for variable, message in self.items()},
             plates=self.plates,
@@ -146,14 +150,18 @@
     @property
     def shapes(self):
         return {v: np.shape(m) for v, m in self.items()}
 
     @property
     def sizes(self):
         return {v: np.size(m) for v, m in self.items()}
+    
+    @property 
+    def names(self):
+        return {v.name: m for v, m in self.items()}
 
     def __getitem__(self, index):
         if isinstance(index, Variable):
             return dict.__getitem__(self, index)
         else:
             return self.subset(self.variables, plates_index=index)
 
@@ -208,63 +216,65 @@
                 rescaled[v] = message
             elif scale == 0:
                 rescaled[v] = 1.0
             else:
                 rescaled[v] = message ** scale
 
         return MeanField(rescaled)
+    
+    def map(self, func):
+        return VariableData({v: func(dist) for v, dist in self.items()})
+
+    def attr(self, attr: str):
+        return MeanField.map(self, attrgetter(attr))
 
     @property
     def mean(self):
-        return VariableData({v: dist.mean for v, dist in self.items()})
+        return self.attr("mean")
 
     @property
     def variance(self):
-        return VariableData({v: dist.variance for v, dist in self.items()})
+        return self.attr("variance")
 
     @property
     def std(self):
-        return VariableData({v: dist.std for v, dist in self.items()})
+        return self.attr("std")
 
     @property
     def scale(self):
-        return VariableData({v: dist.scale for v, dist in self.items()})
+        return self.attr("scale")
 
     @property
     def lower_limit(self):
-        return VariableData(
-            {
-                v: np.full(m.shape, m.lower_limit) if m.shape else m.lower_limit
-                for v, m in self.items()
-            }
+        return self.map(
+            lambda m: np.full(m.shape, m.lower_limit) if m.shape else m.lower_limit
         )
 
     @property
     def upper_limit(self):
-        return VariableData(
-            {
-                v: np.full(m.shape, m.upper_limit) if m.shape else m.upper_limit
-                for v, m in self.items()
-            }
+        return self.map(
+            lambda m: np.full(m.shape, m.upper_limit) if m.shape else m.upper_limit
         )
+    
+    def zeros_like(self):
+        return MeanField.map(self, lambda m: m.zeros_like())
 
     def precision(self, variables=None):
         variables = variables or self.all_variables
-        variances = MeanField.variance.fget(self).subset(variables)
+        variances = MeanField.attr(self, "variance").subset(variables)
         return VariableFullOperator.from_diagonal(variances ** -1)
 
     @property
     def arguments(self) -> Dict[Variable, Prior]:
         """
         Arguments that can be used to update a Model
         """
         return {v: dist for v, dist in self.items()}
 
     def _logpdf(self, *args: np.ndarray) -> np.ndarray:
-        var_names = self.name_variable_dict
         return self.logpdf(dict(zip(self.args, args)))
 
     def logpdf(self, values: Dict[Variable, np.ndarray],) -> np.ndarray:
         """Calculates the logpdf of the passed values for messages
 
         the result is broadcast to the appropriate shape given the variable
         plates
```

### Comparing `autofit-2023.3.27.1/autofit/graphical/utils.py` & `autofit-2023.7.7.1/autofit/graphical/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,16 +50,124 @@
 
 
 def is_iterable(arg):
     return isinstance(arg, abc.Iterable) and not isinstance(
         arg, six.string_types
     )
 
+def is_namedtuple(obj):
+    return isinstance(obj, tuple) and hasattr(obj, '_fields')
 
-def nested_filter(func, *args):
+def nested_getitem(obj, key):
+    """
+    Example
+    -------
+    >>> nested_getitem([1, (2, 3), [3, {'a': 1, 'b': 2}]], (2, 1, 'b'))
+    2
+    """
+    for k in key:
+        obj = obj[k]
+    return obj 
+
+
+def nested_get(obj, key, default=None):
+    """
+    Example
+    -------
+    >>> nested_get([1, (2, 3), [3, {'a': 1, 'b': 2}]], (2, 1, 'b'))
+    2
+    >>> nested_get([1, (2, 3), [3, {'a': 1, 'b': 2}]], (2, 1, 'c'), 'default')
+    'default'
+    """
+    try:
+        return nested_getitem(obj, key)
+    except (KeyError, IndexError):
+        return default
+    
+
+def nested_set(obj, key, val):
+    """
+    Example
+    -------
+    >>> obj = [1, (2, 3), [3, {'a': 1, 'b': 2}]]
+    >>> nested_set(obj, (2, 1, 'b'), 3)
+    >>> obj
+    [1, (2, 3), [3, {'a': 1, 'b': 3}]]
+
+    >>> nested_set(obj, (2, 1,), ()))
+    >>> obj
+    [1, (2, 3), [3, ()]]
+    """
+    *parents, k = key 
+    for p in parents:
+        obj = obj[p]
+    obj[k] = val 
+
+
+def nested_items(*args, key=(), key_func=None):
+    """
+    Example
+    -------
+    >>> list(nested_items([1, (2, 3), [3, {'a': 1, 'b': 2}]]))
+    [((0,), 1), ((1, 0), 2), ((1, 1), 3), ((2, 0), 3), ((2, 1, 'a'), 1), ((2, 1, 'b'), 2)]
+
+    >>> list(nested_items([1, (2, 3)], [4, (5, 6)]))
+    [((0,), 1, 4), ((1, 0), 2, 5), ((1, 1), 3, 6)]
+    """
+    out, *_ = args
+    if isinstance(out, dict):
+        for k in sorted(out, key=key_func):
+            yield from nested_items(*(out[k] for out in args), key=key + (k,), key_func=key_func)
+    elif isinstance(out, (tuple, list)):
+        for i, elems in enumerate(zip(*args)):
+            yield from nested_items(*elems, key=key + (i,), key_func=key_func)
+    else:
+        yield (key,) + args
+
+
+def nested_zip(*args, key_func=None):
+    """ Iterates through a potentially nested set of list, tuples and dictionaries, 
+    recursively looping through the structure and returning the leaves of the tree
+
+    Example
+    -------
+    >>> list(nested_zip([1, (2, 3), [3, 2, {1, 2}]]))
+    [(1,), (2,), (3,), (3,), (2,), (1,), (2,)]
+
+    >>> list(nested_zip(
+    ...     [1, (2, 3), [3, 2, {1, 2}]],
+    ...     [1, ('a', 3), [3, 'b', {1, 'c'}]]
+    ... ))
+    [(1, 1), (2, 'a'), (3, 3), (3, 3), (2, 'b'), (1, 1), (2, 'c')]
+    """
+    out, *_ = args
+    if isinstance(out, dict):
+        for k in sorted(out, key=key_func):
+            yield from nested_zip(*(out[k] for out in args), key_func=key_func)
+    elif is_iterable(out):
+        for elems in zip(*args):
+            yield from nested_zip(*elems, key_func=key_func)
+    else:
+        yield args
+
+
+def nested_iter(args, key_func=None):
+    """Iterates through a potentially nested set of list, tuples and dictionaries, 
+    recursively looping through the structure and returning the leaves of the tree
+
+    Example
+    -------
+    >>> list(nested_iter([1, (2, 3), [3, 2, {1, 2}]]))    
+    [1, 2, 3, 3, 2, 1, 2]
+    """
+    for elem, in nested_zip(args, key_func=key_func):
+        yield elem
+
+
+def nested_filter(func, *args, key_func=None):
     """ Iterates through a potentially nested set of list, tuples and dictionaries, 
     recursively looping through the structure and returning the arguments
     that func return true on, 
 
     Example
     -------
     >>> list(nested_filter(
@@ -71,66 +179,79 @@
     >>> list(nested_filter(
     ...     lambda x, *args: x==2,
     ...     [1, (2, 3), [3, 2, {1, 2}]],
     ...     [1, ('a', 3), [3, 'b', {1, 'c'}]]
     ... ))
     [(2, 'a'), (2, 'b'), (2, 'c')]
     """
+    for leaves in nested_zip(*args, key_func=key_func):
+        if func(*leaves):
+            yield leaves
+
+
+def nested_map(func, *args, key_func=None):
+    """
+    Given a potentially nested set of list, tuples and dictionaries, recursively loop through the structure and
+    replace any values that appear in the dict to_replace
+    can set to replace dictionary keys optionally,
+
+    Example
+    -------
+    >>> nested_map(lambda x: x*2, [1, (2, 3), [3, 2, {1, 2}, {'a': 'b'}]])
+    [2, (4, 6), [6, 4, {2, 4}, {'a': 'bb'}]]
+
+    >>> graph.utils.nested_map(
+    ...     lambda x, y: x*y, 
+    ...     [1, (2, 3), [3, {'a': 1, 'b': 2}]],
+    ...     [1, (2, 3), [3, {'a': 1, 'b': 2}]]
+    ... )
+    [1, (4, 9), [9, {'a': 1, 'b': 4}]]
+    """
     out, *_ = args
     if isinstance(out, dict):
-        for k in out:
-            yield from nested_filter(func, *(out[k] for out in args))
+        return type(out)(
+            {
+                k: nested_map(func, *(arg[k] for arg in args), key_func=key_func)
+                for k in sorted(out, key=key_func)
+            }
+        )
+    elif is_namedtuple(out):
+        return type(out)(*(nested_map(func, *elems) for elems in zip(*args)))
     elif is_iterable(out):
-        for elems in zip(*args):
-            yield from nested_filter(func, *elems)
-    else:
-        if func(*args):
-            yield args
+        return type(out)(nested_map(func, *elems) for elems in zip(*args))
+
+    return func(*args)
 
 
-def nested_update(out, to_replace: dict, replace_keys=False):
+def nested_update(out, to_replace):
     """
     Given a potentially nested set of list, tuples and dictionaries, recursively loop through the structure and
     replace any values that appear in the dict to_replace
     can set to replace dictionary keys optionally,
 
+    Does not replace values in place, so can 'mutate' tuples
+
     Example
     -------
     >>> nested_update([1, (2, 3), [3, 2, {1, 2}]], {2: 'a'})
     [1, ('a', 3), [3, 'a', {1, 'a'}]]
 
     >>> nested_update([{2: 2}], {2: 'a'})
     [{2: 'a'}]
-
-    >>> nested_update([{2: 2}], {2: 'a'}, True)
-    [{'a': 'a'}]
     """
-    try:
-        return to_replace[out]
-    except KeyError:
-        pass
 
-    if isinstance(out, dict):
-        if replace_keys:
-            return type(out)(
-                {
-                    nested_update(k, to_replace, replace_keys): nested_update(
-                        v, to_replace, replace_keys
-                    )
-                    for k, v in out.items()
-                }
-            )
-        else:
-            return type(out)(
-                {k: nested_update(v, to_replace, replace_keys) for k, v in out.items()}
-            )
-    elif is_iterable(out):
-        return type(out)(nested_update(elem, to_replace, replace_keys) for elem in out)
+    def replace(val):
+        return to_replace.get(val, val)
+    
+    return nested_map(replace, out)
+
+from_variabledata = nested_update
 
-    return out
+def to_variabledata(variables, raw_values) -> VariableData:
+    return VariableData(nested_filter(is_variable, variables, raw_values))
 
 
 class StatusFlag(Enum):
     FAILURE = 0
     SUCCESS = 1
     NO_CHANGE = 2
     BAD_PROJECTION = 3
```

### Comparing `autofit-2023.3.27.1/autofit/interpolator.py` & `autofit-2023.7.7.1/autofit/interpolator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/identifier.py` & `autofit-2023.7.7.1/autofit/mapper/identifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/mock/mock_model.py` & `autofit-2023.7.7.1/autofit/mapper/mock/mock_model.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/model.py` & `autofit-2023.7.7.1/autofit/mapper/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,19 @@
     -------
     Function with cache
     """
 
     @wraps(func)
     def cache(self, *args, **kwargs):
         if hasattr(self, "_is_frozen") and self._is_frozen:
-            key = (func.__name__, self, *args,) + tuple(kwargs.items())
+            key = (
+                func.__name__,
+                self,
+                *args,
+            ) + tuple(kwargs.items())
 
             if key not in self._frozen_cache:
                 self._frozen_cache[key] = func(self, *args, **kwargs)
             return self._frozen_cache[key]
         return func(self, *args, **kwargs)
 
     return cache
@@ -218,15 +222,17 @@
                 and isinstance(t[1], class_type),
                 self.__dict__.items(),
             )
         )
 
     @frozen_cache
     def models_with_type(
-        self, cls: Union[Type, Tuple[Type, ...]], include_zero_dimension=False,
+        self,
+        cls: Union[Type, Tuple[Type, ...]],
+        include_zero_dimension=False,
     ) -> List["AbstractModel"]:
         """
         Return all models of a given type in the model tree.
 
         Parameters
         ----------
         cls
@@ -334,14 +340,23 @@
         return []
 
     results = []
     if isinstance(obj, cls):
         results.append((tuple(), obj))
         if ignore_children:
             return results
+
+    if isinstance(obj, list):
+        for i, item in enumerate(obj):
+            for path, instance in path_instances_of_class(
+                item, cls, ignore_class=ignore_class, ignore_children=ignore_children
+            ):
+                results.append(((i,) + path, instance))
+        return results
+
     try:
         from autofit.mapper.prior_model.annotation import AnnotationPriorModel
 
         if isinstance(obj, dict):
             d = obj
         else:
             d = obj.__dict__
@@ -440,8 +455,12 @@
         Returns
         -------
         A model
         """
 
         from autofit.mapper.prior_model.abstract import AbstractPriorModel
 
-        return AbstractPriorModel.from_instance(self, model_classes, excluded_classes,)
+        return AbstractPriorModel.from_instance(
+            self,
+            model_classes,
+            excluded_classes,
+        )
```

### Comparing `autofit-2023.3.27.1/autofit/mapper/model_mapper.py` & `autofit-2023.7.7.1/autofit/mapper/model_mapper.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/model_object.py` & `autofit-2023.7.7.1/autofit/mapper/model_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     _ids = itertools.count()
 
     @classmethod
     def next_id(cls):
         return next(cls._ids)
 
     def __init__(
-        self, id_=None, label=None,
+        self,
+        id_=None,
+        label=None,
     ):
         """
         A generic object in AutoFit
 
         Parameters
         ----------
         id_
@@ -44,17 +46,24 @@
         Returns
         -------
         A copy of this with an updated value
         """
         new = copy.deepcopy(self)
         obj = new
         for key in path[:-1]:
-            obj = getattr(obj, key)
-
-        setattr(obj, path[-1], value)
+            if isinstance(key, int):
+                obj = obj[key]
+            else:
+                obj = getattr(obj, key)
+
+        key = path[-1]
+        if isinstance(key, int):
+            obj[key] = value
+        else:
+            setattr(obj, key, value)
         return new
 
     def has(self, cls: Union[Type, Tuple[Type, ...]]) -> bool:
         """
         Does this instance have an attribute which is of type cls?
         """
         for value in self.__dict__.values():
```

### Comparing `autofit-2023.3.27.1/autofit/mapper/operator.py` & `autofit-2023.7.7.1/autofit/mapper/operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/abstract.py` & `autofit-2023.7.7.1/autofit/mapper/prior/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/arithmetic.py` & `autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/assertion.py` & `autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/assertion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/arithmetic/compound.py` & `autofit-2023.7.7.1/autofit/mapper/prior/arithmetic/compound.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/deferred.py` & `autofit-2023.7.7.1/autofit/mapper/prior/deferred.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/gaussian.py` & `autofit-2023.7.7.1/autofit/mapper/prior/gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/log_gaussian.py` & `autofit-2023.7.7.1/autofit/mapper/prior/log_gaussian.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/log_uniform.py` & `autofit-2023.7.7.1/autofit/mapper/prior/log_uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/tuple_prior.py` & `autofit-2023.7.7.1/autofit/mapper/prior/tuple_prior.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/uniform.py` & `autofit-2023.7.7.1/autofit/mapper/prior/uniform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior/width_modifier.py` & `autofit-2023.7.7.1/autofit/mapper/prior/width_modifier.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior_model/abstract.py` & `autofit-2023.7.7.1/autofit/mapper/prior_model/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,44 +41,14 @@
     def for_class_and_attributes_name(cls, attribute_name):
         limit_dict = conf.instance.prior_config.for_class_and_suffix_path(
             cls, [attribute_name, "gaussian_limits"]
         )
         return limit_dict["lower"], limit_dict["upper"]
 
 
-def check_assertions(func):
-    @wraps(func)
-    def wrapper(s, arguments):
-        # noinspection PyProtectedMember
-        failed_assertions = [
-            assertion
-            for assertion in s._assertions
-            if assertion is False
-            or assertion is not True
-            and not assertion.instance_for_arguments(arguments,)
-        ]
-        number_of_failed_assertions = len(failed_assertions)
-        if number_of_failed_assertions > 0:
-            name_string = "\n".join(
-                [
-                    assertion.name
-                    for assertion in failed_assertions
-                    if hasattr(assertion, "name") and assertion.name is not None
-                ]
-            )
-            if not conf.instance["general"]["test"]["exception_override"]:
-                raise exc.FitException(
-                    f"{number_of_failed_assertions} assertions failed!\n{name_string}"
-                )
-
-        return func(s, arguments)
-
-    return wrapper
-
-
 class TuplePathModifier:
     def __init__(self, model_: "AbstractPriorModel"):
         """
         Modifies paths to priors contained in tuples.
 
         When a tuple is found in a signature a PriorTuple is created.
 
@@ -187,16 +157,54 @@
     @DynamicAttrs
     """
 
     def __init__(self, label=None):
         super().__init__(label=label)
         self._assertions = list()
 
+    def check_assertions(self, arguments: Dict[Prior, float]):
+        """
+        Check that all assertions are satisfied by the given arguments.
+
+        Parameters
+        ----------
+        arguments
+            A dictionary mapping priors to values
+
+        Raises
+        ------
+        FitException
+            If any assertion is not satisfied
+        """
+        failed_assertions = [
+            assertion
+            for assertion in self._assertions
+            if assertion is False
+            or assertion is not True
+            and not assertion.instance_for_arguments(
+                arguments,
+            )
+        ]
+        number_of_failed_assertions = len(failed_assertions)
+        if number_of_failed_assertions > 0:
+            name_string = "\n".join(
+                [
+                    assertion.name
+                    for assertion in failed_assertions
+                    if hasattr(assertion, "name") and assertion.name is not None
+                ]
+            )
+            raise exc.FitException(
+                f"{number_of_failed_assertions} assertions failed!\n{name_string}"
+            )
+
     def cast(
-        self, value_dict: Dict["AbstractModel", dict], new_class: type,
+        self,
+        value_dict: Dict["AbstractModel", dict],
+        new_class: type,
     ) -> "AbstractPriorModel":
         """
         Cast models to a new type. Allows selected models in within this
         model to be given a new type and new arguments.
 
         Parameters
         ----------
@@ -260,15 +268,21 @@
         if len(tree) == 0:
             return self
 
         with_paths = self.without_attributes()
         for name, subtree in tree.items():
             # noinspection PyProtectedMember
             new_value = getattr(self, name)
-            if isinstance(new_value, (AbstractPriorModel, TuplePrior,)):
+            if isinstance(
+                new_value,
+                (
+                    AbstractPriorModel,
+                    TuplePrior,
+                ),
+            ):
                 new_value = new_value._with_paths(subtree)
             setattr(with_paths, name, new_value)
         return with_paths
 
     @split_paths
     def with_paths(self, paths: List[Tuple[str, ...]]) -> "AbstractModel":
         """
@@ -305,15 +319,21 @@
         without_paths = copy.deepcopy(self)
         for name, subtree in tree.items():
             # noinspection PyProtectedMember
             if len(subtree) == 0:
                 delattr(without_paths, name)
             else:
                 new_value = getattr(without_paths, name)
-                if isinstance(new_value, (AbstractPriorModel, TuplePrior,)):
+                if isinstance(
+                    new_value,
+                    (
+                        AbstractPriorModel,
+                        TuplePrior,
+                    ),
+                ):
                     new_value = new_value._without_paths(subtree)
                 setattr(without_paths, name, new_value)
         return without_paths
 
     @split_paths
     def without_paths(self, paths: List[Tuple[str, ...]]) -> "AbstractModel":
         """
@@ -444,22 +464,32 @@
             try:
                 item = copy.copy(source)
                 if isinstance(item, dict):
                     from autofit.mapper.prior_model.collection import Collection
 
                     item = Collection(item)
                 for attribute in path:
-                    item = copy.copy(getattr(item, attribute))
+                    if isinstance(attribute, int):
+                        item = item[attribute]
+                    else:
+                        item = copy.copy(getattr(item, attribute))
 
                 target = self
                 for attribute in path[:-1]:
-                    target = getattr(target, attribute)
+                    if isinstance(attribute, int):
+                        target = target[attribute]
+                    else:
+                        target = getattr(target, attribute)
                     assert_no_assertions(target)
 
-                setattr(target, path[-1], item)
+                attribute = path[-1]
+                if isinstance(attribute, int):
+                    target[attribute] = item
+                else:
+                    setattr(target, path[-1], item)
             except AttributeError:
                 pass
 
     def instance_from_unit_vector(self, unit_vector, ignore_prior_limits=False):
         """
         Returns a ModelInstance, which has an attribute and class instance corresponding
         to every `Model` attributed to this instance.
@@ -495,23 +525,27 @@
             )
 
         arguments = dict(
             map(
                 lambda prior_tuple, unit: (
                     prior_tuple.prior,
                     prior_tuple.prior.value_for(
-                        unit, ignore_prior_limits=ignore_prior_limits,
+                        unit,
+                        ignore_prior_limits=ignore_prior_limits,
                     ),
                 ),
                 self.prior_tuples_ordered_by_id,
                 unit_vector,
             )
         )
 
-        return self.instance_for_arguments(arguments,)
+        return self.instance_for_arguments(
+            arguments,
+            ignore_assertions=ignore_prior_limits,
+        )
 
     @property
     @cast_collection(PriorNameValue)
     @frozen_cache
     def unique_prior_tuples(self):
         """
         Returns
@@ -617,15 +651,18 @@
             A list of physical values constructed by taking the mean possible value from
             each prior.
         """
         vector = []
 
         for prior in self.priors_ordered_by_id:
             vector.append(
-                prior.random(lower_limit=lower_limit, upper_limit=upper_limit,)
+                prior.random(
+                    lower_limit=lower_limit,
+                    upper_limit=upper_limit,
+                )
             )
 
         return vector
 
     def random_instance_from_priors_within_limits(
         self, lower_limit: float = 0.0, upper_limit: float = 1.0
     ):
@@ -656,15 +693,15 @@
             lower_limit=lower_limit, upper_limit=upper_limit
         )
 
         return self.instance_from_vector(vector=vector)
 
     @property
     def random_vector_from_priors(self):
-        """ Generate a random vector of physical values by drawing uniform random values between 0 and 1 and using
+        """Generate a random vector of physical values by drawing uniform random values between 0 and 1 and using
         the model priors to map them from unit values to physical values.
         Returns
         -------
         physical_values: [float]
             A list of physical values constructed by taking random values from each prior.
         """
         return self.random_vector_from_priors_within_limits(
@@ -712,15 +749,17 @@
             )
         )
 
         if not ignore_prior_limits:
             for prior, value in arguments.items():
                 prior.assert_within_limits(value)
 
-        return self.instance_for_arguments(arguments,)
+        return self.instance_for_arguments(
+            arguments,
+        )
 
     def has(self, cls: Union[Type, Tuple[Type, ...]]) -> bool:
         """
         Parameters
         ----------
         cls
             The type to check for
@@ -745,15 +784,16 @@
         """
         True iff this model contains a Model of type
         cls, recursively.
         """
         return (
             len(
                 self.model_tuples_with_type(
-                    cls, include_zero_dimension=include_zero_dimension,
+                    cls,
+                    include_zero_dimension=include_zero_dimension,
                 )
             )
             > 0
         )
 
     def is_only_model(self, cls) -> bool:
         """
@@ -962,15 +1002,16 @@
         """
         return self.instance_from_unit_vector(
             unit_vector=[0.5] * self.prior_count,
             ignore_prior_limits=ignore_prior_limits,
         )
 
     def log_prior_list_from_vector(
-        self, vector: [float],
+        self,
+        vector: [float],
     ):
         """
         Compute the log priors of every parameter in a vector, using the Prior of every parameter.
         The log prior values are used by Emcee to map the log likelihood to the poserior of the model.
         Parameters
         ----------
         vector : [float]
@@ -1185,35 +1226,47 @@
         d = {prior[1]: self.cls for prior in self.prior_tuples}
         for prior_model in self.prior_model_tuples:
             if not isinstance(prior_model[1], AnnotationPriorModel):
                 d.update(prior_model[1].prior_class_dict)
         return d
 
     def _instance_for_arguments(
-        self, arguments: Dict[Prior, float],
+        self,
+        arguments: Dict[Prior, float],
     ):
         raise NotImplementedError()
 
     def instance_for_arguments(
-        self, arguments,
+        self,
+        arguments: Dict[Prior, float],
+        ignore_assertions: bool = False,
     ):
         """
         Returns an instance of the model for a set of arguments
 
         Parameters
         ----------
-        arguments: {Prior: float}
+        arguments
             Dictionary mapping priors to attribute analysis_path and value pairs
+        ignore_assertions
+            If True, assertions will not be checked
 
         Returns
         -------
             An instance of the class
         """
+        if not (
+            conf.instance["general"]["test"]["exception_override"] or ignore_assertions
+        ):
+            self.check_assertions(arguments)
+
         logger.debug(f"Creating an instance for arguments")
-        return self._instance_for_arguments(arguments,)
+        return self._instance_for_arguments(
+            arguments,
+        )
 
     def path_for_name(self, name: str) -> Tuple[str, ...]:
         """
         Find the path to a prior in the model that matches
         a given name.
 
         For example, name_of_model_name_of_prior could match
@@ -1512,15 +1565,20 @@
         and its number of free parameters
         """
         from .prior_model import Model
 
         formatter = TextFormatter(line_length=info_whitespace())
 
         for t in self.path_instance_tuples_for_class(
-            (Prior, float, tuple,), ignore_children=True
+            (
+                Prior,
+                float,
+                tuple,
+            ),
+            ignore_children=True,
         ):
             for i in range(len(t[0])):
                 path = t[0][:i]
                 obj = self.object_for_path(path)
                 if isinstance(obj, TuplePrior):
                     continue
                 if isinstance(obj, AbstractPriorModel):
```

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior_model/annotation.py` & `autofit-2023.7.7.1/autofit/mapper/prior_model/annotation.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior_model/attribute_pair.py` & `autofit-2023.7.7.1/autofit/mapper/prior_model/attribute_pair.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior_model/collection.py` & `autofit-2023.7.7.1/autofit/mapper/prior_model/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections.abc import Iterable
 
 from autofit.mapper.model import ModelInstance, assert_not_frozen
 from autofit.mapper.prior.abstract import Prior
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
-from autofit.mapper.prior_model.abstract import check_assertions
 
 
 class Collection(AbstractPriorModel):
     def name_for_prior(self, prior: Prior) -> str:
         """
         Construct a name for the prior. This is the path taken
         to get to the prior.
@@ -36,57 +35,47 @@
             return self._dict[item]
         return self.values[item]
 
     def __len__(self):
         return len(self.values)
 
     def __str__(self):
-        return "\n".join(
-            f"{key} = {value}"
-            for key, value
-            in self.items()
-        )
+        return "\n".join(f"{key} = {value}" for key, value in self.items())
 
     def __hash__(self):
         return self.id
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self}>"
 
     @property
     def values(self):
         return list(self._dict.values())
 
     def items(self):
         return self._dict.items()
 
-    def with_prefix(
-            self,
-            prefix: str
-    ):
+    def with_prefix(self, prefix: str):
         """
         Filter members of the collection, only returning those that start
         with a given prefix as a new collection.
         """
-        return Collection({
-            key: value
-            for key, value
-            in self.items()
-            if key.startswith(
-                prefix
-            )
-        })
+        return Collection(
+            {key: value for key, value in self.items() if key.startswith(prefix)}
+        )
 
     def as_model(self):
-        return Collection({
-            key: value.as_model()
-            if isinstance(value, AbstractPriorModel)
-            else value
-            for key, value in self.dict().items()
-        })
+        return Collection(
+            {
+                key: value.as_model()
+                if isinstance(value, AbstractPriorModel)
+                else value
+                for key, value in self.dict().items()
+            }
+        )
 
     def __init__(self, *arguments, **kwargs):
         """
         The object multiple Python classes are input into to create model-components, which has free parameters that
         are fitted by a non-linear search.
 
         Multiple Python classes can be input into a `Collection` in order to compose high dimensional models made of
@@ -194,38 +183,14 @@
                 pass
 
     def remove(self, item):
         for key, value in self.__dict__.copy().items():
             if value == item:
                 del self.__dict__[key]
 
-    @check_assertions
-    def _instance_for_arguments(self, arguments):
-        """
-        Parameters
-        ----------
-        arguments: {Prior: float}
-            A dictionary of arguments
-
-        Returns
-        -------
-        model_instances: [object]
-            A list of instances constructed from the list of prior models.
-        """
-        result = ModelInstance()
-        for key, value in self.__dict__.items():
-            if key.startswith("_"):
-                continue
-            if isinstance(value, AbstractPriorModel):
-                value = value.instance_for_arguments(arguments)
-            elif isinstance(value, Prior):
-                value = arguments[value]
-            setattr(result, key, value)
-        return result
-
     def gaussian_prior_model_for_arguments(self, arguments):
         """
         Create a new collection, updating its priors according to the argument
         dictionary.
 
         Parameters
         ----------
@@ -235,32 +200,47 @@
         Returns
         -------
         A new collection
         """
         collection = Collection()
 
         for key, value in self.items():
-            if key in (
-                    "component_number",
-                    "item_number",
-                    "id"
-            ) or key.startswith(
-                "_"
-            ):
+            if key in ("component_number", "item_number", "id") or key.startswith("_"):
                 continue
 
             if isinstance(value, AbstractPriorModel):
-                collection[key] = value.gaussian_prior_model_for_arguments(
-                    arguments
-                )
+                collection[key] = value.gaussian_prior_model_for_arguments(arguments)
             if isinstance(value, Prior):
                 collection[key] = arguments[value]
 
         return collection
 
+    def _instance_for_arguments(self, arguments):
+        """
+        Parameters
+        ----------
+        arguments: {Prior: float}
+            A dictionary of arguments
+
+        Returns
+        -------
+        model_instances: [object]
+            A list of instances constructed from the list of prior models.
+        """
+        result = ModelInstance()
+        for key, value in self.__dict__.items():
+            if key.startswith("_"):
+                continue
+            if isinstance(value, AbstractPriorModel):
+                value = value.instance_for_arguments(arguments)
+            elif isinstance(value, Prior):
+                value = arguments[value]
+            setattr(result, key, value)
+        return result
+
     @property
     def prior_class_dict(self):
         return {
             **{
                 prior: cls
                 for prior_model in self.direct_prior_model_tuples
                 for prior, cls in prior_model[1].prior_class_dict.items()
```

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior_model/prior_model.py` & `autofit-2023.7.7.1/autofit/mapper/prior_model/prior_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from autoconf.exc import ConfigException
 from autofit.mapper.model import assert_not_frozen
 from autofit.mapper.model_object import ModelObject
 from autofit.mapper.prior.abstract import Prior
 from autofit.mapper.prior.deferred import DeferredInstance
 from autofit.mapper.prior.tuple_prior import TuplePrior
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
-from autofit.mapper.prior_model.abstract import check_assertions
 from autofit.tools.namer import namer
 
 logger = logging.getLogger(__name__)
 
 class_args_dict = dict()
 
 
@@ -283,15 +282,14 @@
         self.__getattribute__(item)
 
     @property
     def is_deferred_arguments(self):
         return len(self.direct_deferred_tuples) > 0
 
     # noinspection PyUnresolvedReferences
-    @check_assertions
     def _instance_for_arguments(self, arguments: {ModelObject: object}):
         """
         Returns an instance of the associated class for a set of arguments
 
         Parameters
         ----------
         arguments: {Prior: float}
@@ -312,15 +310,17 @@
             model_arguments[tuple_prior.name] = tuple_prior.prior.value_for_arguments(
                 arguments
             )
         for prior_model_tuple in self.direct_prior_model_tuples:
             prior_model = prior_model_tuple.prior_model
             model_arguments[
                 prior_model_tuple.name
-            ] = prior_model.instance_for_arguments(arguments,)
+            ] = prior_model.instance_for_arguments(
+                arguments,
+            )
 
         prior_arguments = dict()
 
         for name, prior in self.direct_prior_tuples:
             try:
                 prior_arguments[name] = arguments[prior]
             except KeyError as e:
```

### Comparing `autofit-2023.3.27.1/autofit/mapper/prior_model/recursion.py` & `autofit-2023.7.7.1/autofit/mapper/prior_model/recursion.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/variable.py` & `autofit-2023.7.7.1/autofit/mapper/variable.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mapper/variable_operator.py` & `autofit-2023.7.7.1/autofit/mapper/variable_operator.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/messages/abstract.py` & `autofit-2023.7.7.1/autofit/messages/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,23 @@
             self.parameters = tuple(np.asanyarray(p) for p in parameters)
         else:
             self.parameters = tuple(parameters)
 
     @property
     def broadcast(self):
         return self._broadcast
+    
+    @property
+    def _init_kwargs(self):
+        return dict(
+            log_norm=self.log_norm,
+            id_=self.id,
+            lower_limit=self.lower_limit,
+            upper_limit=self.upper_limit,
+        )
 
     def check_support(self) -> np.ndarray:
         if self._parameter_support is not None:
             return reduce(
                 and_,
                 (
                     (p >= support[0]) & (p <= support[1])
@@ -157,14 +166,17 @@
     @classmethod
     def from_natural_parameters(
         cls, natural_parameters: np.ndarray, **kwargs
     ) -> "AbstractMessage":
         cls_ = cls._projection_class or cls._Base_class or cls
         args = cls_.invert_natural_parameters(natural_parameters)
         return cls_(*args, **kwargs)
+    
+    def zeros_like(self) -> "AbstractMessage":
+        return self ** 0.
 
     @classmethod
     @abstractmethod
     def invert_sufficient_statistics(
         cls, sufficient_statistics: np.ndarray
     ) -> np.ndarray:
         pass
```

### Comparing `autofit-2023.3.27.1/autofit/messages/beta.py` & `autofit-2023.7.7.1/autofit/messages/beta.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/messages/composed_transform.py` & `autofit-2023.7.7.1/autofit/messages/composed_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,7 +300,10 @@
 
     def update_invalid(self, other: "TransformedMessage") -> "MessageInterface":
         return self.with_base(self.base_message.update_invalid(other.base_message))
 
     @property
     def log_base_measure(self):
         return self.base_message.log_base_measure
+
+    def zeros_like(self) -> "MessageInterface":
+        return self ** 0.
```

### Comparing `autofit-2023.3.27.1/autofit/messages/fixed.py` & `autofit-2023.7.7.1/autofit/messages/fixed.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/messages/gamma.py` & `autofit-2023.7.7.1/autofit/messages/gamma.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/messages/interface.py` & `autofit-2023.7.7.1/autofit/messages/interface.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/messages/normal.py` & `autofit-2023.7.7.1/autofit/messages/normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,23 @@
     def __repr__(self):
         return (
             "<NormalMessage id={} mean={} sigma={} "
             "lower_limit={} upper_limit={}>".format(
                 self.id, self.mean, self.sigma, self.lower_limit, self.upper_limit
             )
         )
+    
+    @property
+    def natural(self):
+        return NaturalNormal.from_natural_parameters(
+            self.natural_parameters * 0., **self._init_kwargs
+        )
+
+    def zeros_like(self) -> "AbstractMessage":
+        return self.natural.zeros_like()
 
 
 class NaturalNormal(NormalMessage):
     """
     Identical to the NormalMessage but allows non-normalised values,
     e.g negative or infinite variances
     """
@@ -269,14 +278,20 @@
             precision = covariance.inv().diagonal()
         else:
             mode, variance = cls._get_mean_variance(mode, covariance)
             precision = 1 / variance
 
         return cls(mode * precision, -precision / 2, **kwargs)
 
+    zeros_like = AbstractMessage.zeros_like
+    
+    @property
+    def natural(self):
+        return self
+    
 
 UniformNormalMessage = TransformedMessage(NormalMessage(0, 1), phi_transform)
 
 Log10UniformNormalMessage = TransformedMessage(UniformNormalMessage, log_10_transform)
 
 LogNormalMessage = TransformedMessage(NormalMessage(0, 1), log_transform)
```

### Comparing `autofit-2023.3.27.1/autofit/messages/transform.py` & `autofit-2023.7.7.1/autofit/messages/transform.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/messages/utils.py` & `autofit-2023.7.7.1/autofit/messages/utils.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/mock.py` & `autofit-2023.7.7.1/autofit/mock.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/abstract_search.py` & `autofit-2023.7.7.1/autofit/non_linear/abstract_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from autofit.graphical import (
     MeanField,
     AnalysisFactor,
     _HierarchicalFactor,
     FactorApproximation,
 )
 from autofit.graphical.utils import Status
+from autofit.graphical.utils import Status
 from autofit.mapper.prior_model.collection import Collection
 from autofit.non_linear.initializer import Initializer
 from autofit.non_linear.parallel import SneakyPool
 from autofit.non_linear.paths.abstract import AbstractPaths
 from autofit.non_linear.paths.directory import DirectoryPaths
 from autofit.non_linear.paths.sub_directory_paths import SubDirectoryPaths
 from autofit.non_linear.result import Result
@@ -84,15 +85,15 @@
         """
         Abstract base class for non-linear searches.L
 
         This class sets up the file structure for the non-linear search, which are standardized across all non-linear
         searches.
 
         Parameters
-    ----------
+        ----------
         name
             The name of the search, controlling the last folder results are output.
         path_prefix
             The path of folders prefixing the name folder where results are output.
         unique_tag
             The name of a unique tag for this model-fit, which will be given a unique entry in the sqlite database
             and also acts as the folder after the path prefix and before the search name.
@@ -570,15 +571,22 @@
         self.logger.info("Starting search")
 
         model = analysis.modify_model(model)
         self.paths.model = model
         self.paths.unique_tag = self.unique_tag
         self.paths.restore()
 
-        analysis = analysis.modify_before_fit(paths=self.paths, model=model,)
+        analysis = analysis.modify_before_fit(paths=self.paths, model=model)
+
+        analysis.visualize_before_fit(
+            paths=self.paths, model=model,
+        )
+        analysis.visualize_before_fit_combined(
+            analyses=None, paths=self.paths, model=model,
+        )
 
         if not self.paths.is_complete or self.force_pickle_overwrite:
             self.logger.info("Saving path info")
 
             self.paths.save_all(
                 search_config_dict=self.config_dict_search,
                 info=info,
@@ -764,14 +772,17 @@
         except exc.FitException:
             return samples
 
         self.logger.debug("Visualizing")
         analysis.visualize(
             paths=self.paths, instance=instance, during_analysis=during_analysis
         )
+        analysis.visualize_combined(
+            analyses=None, paths=self.paths, instance=instance, during_analysis=during_analysis
+        )
 
         if self.should_profile:
             self.logger.debug("Profiling Maximum Likelihood Model")
             analysis.profile_log_likelihood_function(
                 paths=self.paths, instance=instance,
             )
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/analysis/analysis.py` & `autofit-2023.7.7.1/autofit/non_linear/analysis/analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import logging
 from abc import ABC
+import os
+
+from autoconf import conf
 
 from autofit.mapper.prior_model.abstract import AbstractPriorModel
 from autofit.non_linear.paths.abstract import AbstractPaths
 from autofit.non_linear.result import Result
 
 logger = logging.getLogger(
     __name__
@@ -34,20 +37,58 @@
         """
         from .model_analysis import ModelAnalysis
         return ModelAnalysis(
             analysis=self,
             model=model
         )
 
+    def should_visualize(self, paths: AbstractPaths) -> bool:
+        """
+        Whether a visualize method should continue and perform visualization, or be terminated early.
+
+        If a model-fit has already completed, the default behaviour is for visualization to be bypassed in order
+        to make model-fits run faster. However, visualization can be forced to run via
+        the `force_visualization_overwrite`, for example if a user wants to plot additional images that were not
+        output on the original run.
+
+        PyAutoFit test mode also disables visualization, irrespective of the `force_visualization_overwite`
+        config input.
+
+        Parameters
+        ----------
+        paths
+            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
+            visualization and the pickled objects used by the aggregator output by this function.
+
+
+        Returns
+        -------
+        A bool determining whether visualization should be performed or not.
+        """
+
+        if os.environ.get("PYAUTOFIT_TEST_MODE") == "1":
+            return False
+
+        return not paths.is_complete or conf.instance["general"]["output"]["force_visualize_overwrite"]
+
     def log_likelihood_function(self, instance):
         raise NotImplementedError()
 
+    def visualize_before_fit(self, paths: AbstractPaths, model: AbstractPriorModel):
+        pass
+
     def visualize(self, paths: AbstractPaths, instance, during_analysis):
         pass
 
+    def visualize_before_fit_combined(self, analyses, paths: AbstractPaths, model: AbstractPriorModel):
+        pass
+
+    def visualize_combined(self, analyses, paths: AbstractPaths, instance, during_analysis):
+        pass
+
     def save_attributes_for_aggregator(self, paths: AbstractPaths):
         pass
 
     def save_results_for_aggregator(self, paths: AbstractPaths, result:Result):
         pass
 
     def modify_before_fit(self, paths: AbstractPaths, model: AbstractPriorModel):
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/analysis/combined.py` & `autofit-2023.7.7.1/autofit/non_linear/analysis/combined.py`

 * *Files 18% similar despite different names*

```diff
@@ -85,17 +85,19 @@
         Parameters
         ----------
         paths
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         model
             The model which is to be fitted.
         """
-        return CombinedAnalysis(
-            *(analysis.modify_before_fit(paths, model) for analysis in self.analyses)
-        )
+
+        def func(child_paths, analysis):
+            return analysis.modify_before_fit(child_paths, model)
+
+        return CombinedAnalysis(*self._for_each_analysis(func, paths))
 
     def modify_after_fit(
         self, paths: AbstractPaths, model: AbstractPriorModel, result: Result
     ):
         """
         Modify the analysis after fitting.
 
@@ -104,19 +106,20 @@
         paths
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         model
             The model which is to be fitted.
         result
             The result of the fit.
         """
+
+        def func(child_paths, analysis, result_):
+            return analysis.modify_after_fit(child_paths, model, result_)
+
         return CombinedAnalysis(
-            *(
-                analysis.modify_after_fit(paths, model, result)
-                for analysis in self.analyses
-            )
+            *self._for_each_analysis(func, paths, result.child_results)
         )
 
     @property
     def n_cores(self):
         return self._n_cores
 
     @n_cores.setter
@@ -151,43 +154,87 @@
         return sum(
             analysis.log_likelihood_function(instance) for analysis in self.analyses
         )
 
     def log_likelihood_function(self, instance):
         return self._log_likelihood_function(instance)
 
-    def _for_each_analysis(self, func, paths, *args):
+    def _for_each_analysis(self, func, paths, *args) -> List[Union[Result, Analysis]]:
         """
         Convenience function to call an underlying function for each
         analysis with a paths object with an integer attached to the
         end.
 
         Parameters
         ----------
         func
             Some function of the analysis class
         paths
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         """
+        results = []
         for (i, analysis), *args in zip(enumerate(self.analyses), *args):
             child_paths = paths.for_sub_analysis(analysis_name=f"analyses/analysis_{i}")
-            func(child_paths, analysis, *args)
+            results.append(func(child_paths, analysis, *args))
+
+        return results
 
     def save_attributes_for_aggregator(self, paths: AbstractPaths):
         def func(child_paths, analysis):
-            analysis.save_attributes_for_aggregator(child_paths,)
+            analysis.save_attributes_for_aggregator(
+                child_paths,
+            )
 
         self._for_each_analysis(func, paths)
 
     def save_results_for_aggregator(self, paths: AbstractPaths, result: Result):
         def func(child_paths, analysis, result_):
             analysis.save_results_for_aggregator(paths=child_paths, result=result_)
 
         self._for_each_analysis(func, paths, result)
 
+    def visualize_before_fit(self, paths: AbstractPaths, model: AbstractPriorModel):
+        """
+        Visualise the model before fitting.
+
+        Visualisation output is distinguished by using an integer suffix
+        for each analysis path.
+
+        Parameters
+        ----------
+        paths
+            An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
+        """
+        def func(child_paths, analysis):
+            analysis.visualize_before_fit(child_paths, model)
+
+        self._for_each_analysis(func, paths)
+
+    def visualize_before_fit_combined(self, analyses, paths: AbstractPaths, model: AbstractPriorModel):
+        """
+        Visualise images and quantities which are shared across all analyses.
+
+        For example, each Analysis may have a different dataset, where the data in each dataset is intended to all
+        be plotted on the same matplotlib subplot. This function can be overwritten to allow the visualization of such
+        a plot.
+
+        Only the first analysis is used to visualize the combined results, where it is assumed that it uses the
+        `analyses` property to access the other analyses and perform visualization.
+
+        Parameters
+        ----------
+        paths
+            An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
+        """
+        self.analyses[0].visualize_before_fit_combined(
+            analyses=self.analyses,
+            paths=paths,
+            model=model,
+        )
+
     def visualize(self, paths: AbstractPaths, instance, during_analysis):
         """
         Visualise the instance according to each analysis.
 
         Visualisation output is distinguished by using an integer suffix
         for each analysis path.
 
@@ -202,16 +249,45 @@
         """
 
         def func(child_paths, analysis):
             analysis.visualize(child_paths, instance, during_analysis)
 
         self._for_each_analysis(func, paths)
 
+    def visualize_combined(self, analyses : List["Analysis"], instance, paths: AbstractPaths, during_analysis):
+        """
+        Visualise the instance using images and quantities which are shared across all analyses.
+
+        For example, each Analysis may have a different dataset, where the fit to each dataset is intended to all
+        be plotted on the same matplotlib subplot. This function can be overwritten to allow the visualization of such
+        a plot.
+
+        Only the first analysis is used to visualize the combined results, where it is assumed that it uses the
+        `analyses` property to access the other analyses and perform visualization.
+
+        Parameters
+        ----------
+        paths
+            An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
+        instance
+            The maximum likelihood instance of the model so far in the non-linear search.
+        during_analysis
+            Is this visualisation during analysis?
+        """
+        self.analyses[0].visualize_combined(
+            analyses=self.analyses,
+            paths=paths,
+            instance=instance,
+            during_analysis=during_analysis
+        )
+
     def profile_log_likelihood_function(
-        self, paths: AbstractPaths, instance,
+        self,
+        paths: AbstractPaths,
+        instance,
     ):
         """
         Profile the log likelihood function of the maximum likelihood model instance using each analysis.
 
         Profiling output is distinguished by using an integer suffix for each analysis path.
 
         Parameters
@@ -220,15 +296,16 @@
             An object describing the paths for saving data (e.g. hard-disk directories or entries in sqlite database).
         instance
             The maximum likliehood instance of the model so far in the non-linear search.
         """
 
         def func(child_paths, analysis):
             analysis.profile_log_likelihood_function(
-                child_paths, instance,
+                child_paths,
+                instance,
             )
 
         self._for_each_analysis(func, paths)
 
     def make_result(self, samples, model, sigma=1.0, use_errors=True, use_widths=False):
         child_results = [
             analysis.make_result(
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/analysis/free_parameter.py` & `autofit-2023.7.7.1/autofit/non_linear/analysis/free_parameter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/analysis/indexed.py` & `autofit-2023.7.7.1/autofit/non_linear/analysis/indexed.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,22 @@
 
     def log_likelihood_function(self, instance):
         """
         Compute the log likelihood by taking the instance at the index
         """
         return self.analysis.log_likelihood_function(instance[self.index])
 
+    # TODO : Add before fit methods here?
+
     def visualize(self, paths: AbstractPaths, instance, during_analysis):
         return self.analysis.visualize(paths, instance[self.index], during_analysis)
 
+    def visualize_combined(self, analyses, paths: AbstractPaths, instance, during_analysis):
+        return self.analysis.visualize_combined(analyses, paths, instance[self.index], during_analysis)
+
     def profile_log_likelihood_function(self, paths: AbstractPaths, instance):
         return self.profile_log_likelihood_function(paths, instance[self.index])
 
     def __getattr__(self, item):
         return getattr(self.analysis, item)
 
     def make_result(self, samples, model, sigma=3.0, use_errors=True, use_widths=True):
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/analysis/model_analysis.py` & `autofit-2023.7.7.1/autofit/non_linear/analysis/model_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/analysis/multiprocessing.py` & `autofit-2023.7.7.1/autofit/non_linear/analysis/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/__init__.py` & `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/__init__.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/job.py` & `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/job.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/result.py` & `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/grid/grid_search/result_builder.py` & `autofit-2023.7.7.1/autofit/non_linear/grid/grid_search/result_builder.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/grid/sensitivity.py` & `autofit-2023.7.7.1/autofit/non_linear/grid/sensitivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,32 +428,37 @@
             instance.perturbation = perturbation_instance
 
             yield self.job_cls(
                 analysis_factory=AnalysisFactory(
                     instance=instance,
                     simulate_function=self.simulate_function,
                     analysis_class=self.analysis_class,
+                    paths=search.paths,
                 ),
                 model=self.model,
                 perturbation_model=perturbation_model,
                 base_instance=self.instance,
                 perturbation_instance=perturbation_instance,
                 search=search,
                 number=number,
             )
 
 
 class AnalysisFactory:
     def __init__(
-        self, instance, simulate_function, analysis_class,
+        self, instance, simulate_function, analysis_class, paths,
     ):
         """
         Callable to delay simulation such that it is performed
         on the Job subprocess
         """
         self.instance = instance
         self.simulate_function = simulate_function
         self.analysis_class = analysis_class
+        self.paths = paths
 
     def __call__(self):
-        dataset = self.simulate_function(self.instance)
+        dataset = self.simulate_function(
+            instance=self.instance,
+            simulate_path=self.paths.image_path.replace("image", "simulate")
+        )
         return self.analysis_class(dataset)
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/grid/simple_grid.py` & `autofit-2023.7.7.1/autofit/non_linear/grid/simple_grid.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/initializer.py` & `autofit-2023.7.7.1/autofit/non_linear/initializer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/abstract_mcmc.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/abstract_mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/auto_correlations.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/auto_correlations.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/emcee.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/emcee.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/plotter.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/emcee/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/emcee/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/plotter.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mcmc/zeus/zeus.py` & `autofit-2023.7.7.1/autofit/non_linear/mcmc/zeus/zeus.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mock/mock_analysis.py` & `autofit-2023.7.7.1/autofit/non_linear/mock/mock_analysis.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mock/mock_result.py` & `autofit-2023.7.7.1/autofit/non_linear/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mock/mock_samples.py` & `autofit-2023.7.7.1/autofit/non_linear/mock/mock_samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/mock/mock_search.py` & `autofit-2023.7.7.1/autofit/non_linear/mock/mock_search.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/abstract_nest.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/abstract_nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/abstract.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/dynamic.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/dynamic.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/plotter.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/dynesty/static.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/dynesty/static.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/plotter.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/nest/ultranest/ultranest.py` & `autofit-2023.7.7.1/autofit/non_linear/nest/ultranest/ultranest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/abstract_optimize.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/abstract_optimize.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/drawer/drawer.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/drawer/drawer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/lbfgs/lbfgs.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/lbfgs.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/lbfgs/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/lbfgs/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/abstract.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/globe.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/globe.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/local.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/local.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/plotter.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/plotter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/optimize/pyswarms/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/optimize/pyswarms/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/parallel/process.py` & `autofit-2023.7.7.1/autofit/non_linear/parallel/process.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/parallel/sneaky.py` & `autofit-2023.7.7.1/autofit/non_linear/parallel/sneaky.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/paths/abstract.py` & `autofit-2023.7.7.1/autofit/non_linear/paths/abstract.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/paths/database.py` & `autofit-2023.7.7.1/autofit/non_linear/paths/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,17 @@
 
         Returns
         -------
         A new paths object
         """
         self.fit.is_grid_search = True
         if self.fit.instance is None:
-            self.fit.instance = self.model.instance_from_prior_medians()
+            self.fit.instance = self.model.instance_from_prior_medians(
+                ignore_prior_limits=True
+            )
         child = type(self)(
             session=self.session,
             name=name or self.name,
             path_prefix=path_prefix or self.path_prefix,
             is_identifier_in_paths=(
                 is_identifier_in_paths
                 if is_identifier_in_paths is not None
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/paths/directory.py` & `autofit-2023.7.7.1/autofit/non_linear/paths/directory.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/paths/null.py` & `autofit-2023.7.7.1/autofit/non_linear/paths/null.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/paths/sub_directory_paths.py` & `autofit-2023.7.7.1/autofit/non_linear/paths/sub_directory_paths.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/result.py` & `autofit-2023.7.7.1/autofit/non_linear/result.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/samples/mcmc.py` & `autofit-2023.7.7.1/autofit/non_linear/samples/mcmc.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/samples/nest.py` & `autofit-2023.7.7.1/autofit/non_linear/samples/nest.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/samples/pdf.py` & `autofit-2023.7.7.1/autofit/non_linear/samples/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,14 +318,18 @@
         """
         The parameter vector of an individual sample of the non-linear search drawn randomly from the PDF, returned as
         a 1D list.
 
         The draw is weighted by the sample weights to ensure that the sample is drawn from the PDF (which is important
         for non-linear searches like nested sampling).
         """
+
+        print(self.sample_list)
+        print(self.weight_list)
+
         sample_index = np.random.choice(a=range(len(self.sample_list)), p=self.weight_list)
 
         return self.parameter_lists[sample_index][:]
 
     @to_instance_input
     def offset_values_via_input_values(self, input_vector: List, as_instance: bool = True) -> Union[List, ModelInstance]:
         """
```

### Comparing `autofit-2023.3.27.1/autofit/non_linear/samples/sample.py` & `autofit-2023.7.7.1/autofit/non_linear/samples/sample.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/samples/samples.py` & `autofit-2023.7.7.1/autofit/non_linear/samples/samples.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/samples/stored.py` & `autofit-2023.7.7.1/autofit/non_linear/samples/stored.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/settings.py` & `autofit-2023.7.7.1/autofit/non_linear/settings.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/non_linear/timer.py` & `autofit-2023.7.7.1/autofit/non_linear/timer.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/plot/output.py` & `autofit-2023.7.7.1/autofit/plot/output.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/plot/samples_plotters.py` & `autofit-2023.7.7.1/autofit/plot/samples_plotters.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/text/formatter.py` & `autofit-2023.7.7.1/autofit/text/formatter.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/text/samples_text.py` & `autofit-2023.7.7.1/autofit/text/samples_text.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/text/text_util.py` & `autofit-2023.7.7.1/autofit/text/text_util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/tools/add_notebook_quotes.py` & `autofit-2023.7.7.1/autofit/tools/add_notebook_quotes.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/tools/update_identifiers.py` & `autofit-2023.7.7.1/autofit/tools/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit/tools/util.py` & `autofit-2023.7.7.1/autofit/tools/util.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/autofit.egg-info/SOURCES.txt` & `autofit-2023.7.7.1/autofit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/Makefile` & `autofit-2023.7.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/_templates/custom-class-template.rst` & `autofit-2023.7.7.1/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/_templates/custom_module_template.rst` & `autofit-2023.7.7.1/docs/_templates/custom_module_template.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/analysis.rst` & `autofit-2023.7.7.1/docs/api/analysis.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/database.rst` & `autofit-2023.7.7.1/docs/api/database.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/model.rst` & `autofit-2023.7.7.1/docs/api/model.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/plot.rst` & `autofit-2023.7.7.1/docs/api/plot.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/priors.rst` & `autofit-2023.7.7.1/docs/api/priors.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/samples.rst` & `autofit-2023.7.7.1/docs/api/samples.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/searches.rst` & `autofit-2023.7.7.1/docs/api/searches.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/api/source.rst` & `autofit-2023.7.7.1/docs/api/source.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/conf.py` & `autofit-2023.7.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/cookbooks/cookbook_1_basics.rst` & `autofit-2023.7.7.1/docs/cookbooks/cookbook_1_basics.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/cookbooks/cookbook_2_collections.rst` & `autofit-2023.7.7.1/docs/cookbooks/cookbook_2_collections.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/cookbooks/cookbook_3_multiple_datasets.rst` & `autofit-2023.7.7.1/docs/cookbooks/cookbook_3_multiple_datasets.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/cookbooks/cookbook_4_multi_level.rst` & `autofit-2023.7.7.1/docs/cookbooks/cookbook_4_multi_level.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/cookbooks/cookbook_5_model_linking.rst` & `autofit-2023.7.7.1/docs/cookbooks/cookbook_5_model_linking.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/database.rst` & `autofit-2023.7.7.1/docs/features/database.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/graphical.rst` & `autofit-2023.7.7.1/docs/features/graphical.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x1_1__low_snr.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x1_1__low_snr.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x1_2__low_snr.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x1_2__low_snr.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x1_3__low_snr.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x1_3__low_snr.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x1_with_feature.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x1_with_feature_fit_feature.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_feature.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x1_with_feature_fit_no_feature.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x2_fit.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x2_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x2_left.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x2_left.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x2_left_fit.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x2_left_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x2_right_fit.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x2_right_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/gaussian_x2_split.png` & `autofit-2023.7.7.1/docs/features/images/gaussian_x2_split.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/sensitivity_data_high.png` & `autofit-2023.7.7.1/docs/features/images/sensitivity_data_high.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/sensitivity_data_high_fit.png` & `autofit-2023.7.7.1/docs/features/images/sensitivity_data_high_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/sensitivity_data_low.png` & `autofit-2023.7.7.1/docs/features/images/sensitivity_data_low.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/images/sensitivity_data_low_fit.png` & `autofit-2023.7.7.1/docs/features/images/sensitivity_data_low_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/search_chaining.rst` & `autofit-2023.7.7.1/docs/features/search_chaining.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/search_grid_search.rst` & `autofit-2023.7.7.1/docs/features/search_grid_search.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/features/sensitivity_mapping.rst` & `autofit-2023.7.7.1/docs/features/sensitivity_mapping.rst`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         """
         Add this noise to the model line to create the line data that is fitted, using the signal-to-noise ratio to compute
         noise-map of our data which is required when evaluating the chi-squared value of the likelihood.
         """
         data = model_line + noise
         noise_map = (1.0 / signal_to_noise_ratio) * np.ones(pixels)
 
-        return Dataset(data=data, noise_map=noise_map)
+        return Imaging(data=data, noise_map=noise_map)
 
 Here are what the two most extreme simulated datasets look like, corresponding to the highest and lowest normalization values
 
 .. image:: https://raw.githubusercontent.com/rhayes777/PyAutoFit/main/docs/features/images/sensitivity_data_low.png
   :width: 600
   :alt: Alternative text
```

### Comparing `autofit-2023.3.27.1/docs/general/adding_a_model_component.rst` & `autofit-2023.7.7.1/docs/general/adding_a_model_component.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/general/citations.rst` & `autofit-2023.7.7.1/docs/general/citations.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/general/configs.rst` & `autofit-2023.7.7.1/docs/general/configs.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/general/roadmap.rst` & `autofit-2023.7.7.1/docs/general/roadmap.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/general/workspace.rst` & `autofit-2023.7.7.1/docs/general/workspace.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/howtofit/chapter_1_introduction.rst` & `autofit-2023.7.7.1/docs/howtofit/chapter_1_introduction.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/howtofit/chapter_database.rst` & `autofit-2023.7.7.1/docs/howtofit/chapter_database.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/howtofit/chapter_graphical_models.rst` & `autofit-2023.7.7.1/docs/howtofit/chapter_graphical_models.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/howtofit/howtofit.rst` & `autofit-2023.7.7.1/docs/howtofit/howtofit.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/images/cornerplot.png` & `autofit-2023.7.7.1/docs/images/cornerplot.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/images/toy_model_fit.png` & `autofit-2023.7.7.1/docs/images/toy_model_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/images/toy_model_fit_x2.png` & `autofit-2023.7.7.1/docs/images/toy_model_fit_x2.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/index.rst` & `autofit-2023.7.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/installation/conda.rst` & `autofit-2023.7.7.1/docs/installation/conda.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/installation/overview.rst` & `autofit-2023.7.7.1/docs/installation/overview.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/installation/pip.rst` & `autofit-2023.7.7.1/docs/installation/pip.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/installation/source.rst` & `autofit-2023.7.7.1/docs/installation/source.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/installation/troubleshooting.rst` & `autofit-2023.7.7.1/docs/installation/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/make.bat` & `autofit-2023.7.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/image/cluster_example.jpg` & `autofit-2023.7.7.1/docs/overview/image/cluster_example.jpg`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/image/lens_model.png` & `autofit-2023.7.7.1/docs/overview/image/lens_model.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/image/lens_model_cluster.png` & `autofit-2023.7.7.1/docs/overview/image/lens_model_cluster.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/model_complex.rst` & `autofit-2023.7.7.1/docs/overview/model_complex.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/model_fit.rst` & `autofit-2023.7.7.1/docs/overview/model_fit.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/multi_datasets.rst` & `autofit-2023.7.7.1/docs/overview/multi_datasets.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/non_linear_search.rst` & `autofit-2023.7.7.1/docs/overview/non_linear_search.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/docs/overview/result.rst` & `autofit-2023.7.7.1/docs/overview/result.rst`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,16 @@
 ------------
 
 **PyAutoFit** includes many visualization tools for plotting the results of a non-linear search, for example we can
 make a corner plot of the probability density function (PDF):
 
 .. code-block:: python
 
-    emcee_plotter = aplt.EmceePlotter(samples=result.samples)
-    emcee_plotter.corner()
+    search_plotter = aplt.EmceePlotter(samples=result.samples)
+    search_plotter.corner()
 
 Here is an example of how a PDF estimated for a model appears:
 
 .. image:: https://raw.githubusercontent.com/rhayes777/PyAutoFit/main/docs/images/cornerplot.png
   :width: 600
   :alt: Alternative text
```

### Comparing `autofit-2023.3.27.1/docs/science_examples/astronomy.rst` & `autofit-2023.7.7.1/docs/science_examples/astronomy.rst`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/citation.tex` & `autofit-2023.7.7.1/files/citation.tex`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/citations.bib` & `autofit-2023.7.7.1/files/citations.bib`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/citations.md` & `autofit-2023.7.7.1/files/citations.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/gaussian_example.png` & `autofit-2023.7.7.1/files/gaussian_example.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/release.sh` & `autofit-2023.7.7.1/files/release.sh`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/to_do_list` & `autofit-2023.7.7.1/files/to_do_list`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/files/toy_model_fit.png` & `autofit-2023.7.7.1/files/toy_model_fit.png`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/paper/paper.bib` & `autofit-2023.7.7.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/paper/paper.json` & `autofit-2023.7.7.1/paper/paper.json`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/paper/paper.md` & `autofit-2023.7.7.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/scripts/update_identifiers.py` & `autofit-2023.7.7.1/scripts/update_identifiers.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/scripts/update_identifiers_from_file.py` & `autofit-2023.7.7.1/scripts/update_identifiers_from_file.py`

 * *Files identical despite different names*

### Comparing `autofit-2023.3.27.1/setup.py` & `autofit-2023.7.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.3.27.1")
+version = environ.get("VERSION", "2023.7.7.1")
 requirements.extend([
     f'autoconf=={version}'
 ])
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
```

### Comparing `autofit-2023.3.27.1/to_do_list` & `autofit-2023.7.7.1/to_do_list`

 * *Files identical despite different names*

