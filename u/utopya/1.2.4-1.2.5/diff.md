# Comparing `tmp/utopya-1.2.4.tar.gz` & `tmp/utopya-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utopya-1.2.4.tar", last modified: Tue Apr  4 16:40:28 2023, max compression
+gzip compressed data, was "utopya-1.2.5.tar", last modified: Wed Jun  7 09:29:25 2023, max compression
```

## Comparing `utopya-1.2.4.tar` & `utopya-1.2.5.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.244458 utopya-1.2.4/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-04-04 16:40:14.000000 utopya-1.2.4/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     7633 2023-04-04 16:40:14.000000 utopya-1.2.4/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)     3148 2023-04-04 16:40:28.243458 utopya-1.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-04 16:40:14.000000 utopya-1.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-04-04 16:40:14.000000 utopya-1.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 16:40:28.244458 utopya-1.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5684 2023-04-04 16:40:14.000000 utopya-1.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.204455 utopya-1.2.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.209455 utopya-1.2.4/tests/_gen_figures/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/_gen_figures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/_gen_figures/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/_gen_figures/test_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.211455 utopya-1.2.4/tests/backend/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8239 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/backend/test_benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)    10242 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/backend/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/backend/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.213455 utopya-1.2.4/tests/cli/
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test__shell_complete.py
--rw-rw-rw-   0 root         (0) root         (0)     2810 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test__to_migrate.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test_batch.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15337 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6936 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test_run_and_eval.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/cli/test_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.215455 utopya-1.2.4/tests/eval/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9145 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/eval/test_containers.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/eval/test_datamanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/eval/test_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     6444 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/eval/test_plot_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    45409 2023-04-04 16:40:14.000000 utopya-1.2.4/tests/eval/test_plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.222456 utopya-1.2.4/utopya/
--rw-rw-rw-   0 root         (0) root         (0)     3255 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3340 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_cluster.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_import_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_signal.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.225456 utopya-1.2.4/utopya/_yaml_registry/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_yaml_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_yaml_registry/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    10242 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/_yaml_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    18565 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.227456 utopya-1.2.4/utopya/cfg/
--rw-rw-rw-   0 root         (0) root         (0)    20229 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/cfg/base_cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)    13771 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/cfg/base_plots.yml
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/cfg/btm_cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/cfg/user_cfg_header.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/cfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.230457 utopya-1.2.4/utopya/eval/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6936 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/_plot_func_resolver.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/containers.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/data_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     3079 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/datamanager.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plotcreators.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plothelper.py
--rw-rw-rw-   0 root         (0) root         (0)     9048 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plotmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.234457 utopya-1.2.4/utopya/eval/plots/
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7502 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/_attractor.py
--rw-rw-rw-   0 root         (0) root         (0)    72342 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/_mpl.py
--rw-rw-rw-   0 root         (0) root         (0)    12091 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    58799 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/abm.py
--rw-rw-rw-   0 root         (0) root         (0)    25571 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/attractor.py
--rw-rw-rw-   0 root         (0) root         (0)    62459 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/ca.py
--rw-rw-rw-   0 root         (0) root         (0)     6924 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/distributions.py
--rw-rw-rw-   0 root         (0) root         (0)    24529 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     9451 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/snsplot.py
--rw-rw-rw-   0 root         (0) root         (0)     3193 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/plots/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/eval/transform.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23144 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.236457 utopya-1.2.4/utopya/model_registry/
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model_registry/_registration.py
--rw-rw-rw-   0 root         (0) root         (0)    16777 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model_registry/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    15927 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model_registry/info_bundle.py
--rw-rw-rw-   0 root         (0) root         (0)    11936 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/model_registry/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    70507 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/multiverse.py
--rw-rw-rw-   0 root         (0) root         (0)    19695 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    12146 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/project_registry.py
--rw-rw-rw-   0 root         (0) root         (0)    54018 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)    13652 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/stop_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)    52862 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/testtools.py
--rw-rw-rw-   0 root         (0) root         (0)     9031 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/tools.py
--rw-rw-rw-   0 root         (0) root         (0)    41450 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/workermanager.py
--rw-rw-rw-   0 root         (0) root         (0)     5421 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.224456 utopya-1.2.4/utopya.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3148 2023-04-04 16:40:28.000000 utopya-1.2.4/utopya.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2762 2023-04-04 16:40:28.000000 utopya-1.2.4/utopya.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 16:40:28.000000 utopya-1.2.4/utopya.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-04 16:40:28.000000 utopya-1.2.4/utopya.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-04 16:40:28.000000 utopya-1.2.4/utopya.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-04 16:40:28.000000 utopya-1.2.4/utopya.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.238457 utopya-1.2.4/utopya_backend/
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17418 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.238457 utopya-1.2.4/utopya_backend/io/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.239457 utopya-1.2.4/utopya_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18987 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/model/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8082 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/model/step.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/signal.py
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_backend/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 16:40:28.243458 utopya-1.2.4/utopya_cli/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18051 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/_copy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     9861 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/_shared.py
--rw-rw-rw-   0 root         (0) root         (0)    15347 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5722 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    17756 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/eval.py
--rw-rw-rw-   0 root         (0) root         (0)    24141 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7872 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/projects.py
--rw-rw-rw-   0 root         (0) root         (0)     6753 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/run.py
--rw-rw-rw-   0 root         (0) root         (0)     2627 2023-04-04 16:40:14.000000 utopya-1.2.4/utopya_cli/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.941450 utopya-1.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-07 09:29:14.000000 utopya-1.2.5/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2023-06-07 09:29:14.000000 utopya-1.2.5/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-06-07 09:29:25.940450 utopya-1.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-06-07 09:29:14.000000 utopya-1.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-07 09:29:14.000000 utopya-1.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 09:29:25.941450 utopya-1.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2023-06-07 09:29:14.000000 utopya-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.917450 utopya-1.2.5/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.920450 utopya-1.2.5/tests/_gen_figures/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/_gen_figures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/_gen_figures/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/_gen_figures/test_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.921450 utopya-1.2.5/tests/backend/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8239 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/backend/test_benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)    10242 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/backend/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/backend/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.923450 utopya-1.2.5/tests/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test__shell_complete.py
+-rw-rw-rw-   0 root         (0) root         (0)     2810 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test__to_migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test_batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4804 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15337 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6936 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test_run_and_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/cli/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.924450 utopya-1.2.5/tests/eval/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9145 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/eval/test_containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/eval/test_datamanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/eval/test_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     6444 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/eval/test_plot_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    45409 2023-06-07 09:29:14.000000 utopya-1.2.5/tests/eval/test_plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.928450 utopya-1.2.5/utopya/
+-rw-rw-rw-   0 root         (0) root         (0)     3255 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_import_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_signal.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.930450 utopya-1.2.5/utopya/_yaml_registry/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_yaml_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_yaml_registry/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    10242 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/_yaml_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    18565 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.930450 utopya-1.2.5/utopya/cfg/
+-rw-rw-rw-   0 root         (0) root         (0)    20229 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/cfg/base_cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13771 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/cfg/base_plots.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/cfg/btm_cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/cfg/user_cfg_header.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/cfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.932450 utopya-1.2.5/utopya/eval/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6936 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/_plot_func_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/data_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/datamanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plotcreators.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plothelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9048 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plotmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.935450 utopya-1.2.5/utopya/eval/plots/
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7502 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/_attractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    72342 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/_mpl.py
+-rw-rw-rw-   0 root         (0) root         (0)    12091 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    58799 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/abm.py
+-rw-rw-rw-   0 root         (0) root         (0)    25571 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/attractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    62459 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/ca.py
+-rw-rw-rw-   0 root         (0) root         (0)     6924 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24529 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     9451 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/snsplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/plots/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/eval/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23144 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.936450 utopya-1.2.5/utopya/model_registry/
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model_registry/_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)    16777 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model_registry/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    15927 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model_registry/info_bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)    11936 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/model_registry/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    70544 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/multiverse.py
+-rw-rw-rw-   0 root         (0) root         (0)    19695 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    12146 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/project_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    54018 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)    13652 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/stop_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)    52862 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/testtools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9031 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    41450 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/workermanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5421 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.929450 utopya-1.2.5/utopya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-06-07 09:29:25.000000 utopya-1.2.5/utopya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-06-07 09:29:25.000000 utopya-1.2.5/utopya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:29:25.000000 utopya-1.2.5/utopya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-07 09:29:25.000000 utopya-1.2.5/utopya.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-07 09:29:25.000000 utopya-1.2.5/utopya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-07 09:29:25.000000 utopya-1.2.5/utopya.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.937450 utopya-1.2.5/utopya_backend/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17418 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.937450 utopya-1.2.5/utopya_backend/io/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.938450 utopya-1.2.5/utopya_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18987 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/model/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8082 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/model/step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_backend/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:29:25.940450 utopya-1.2.5/utopya_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18051 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/_copy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     9861 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/_shared.py
+-rw-rw-rw-   0 root         (0) root         (0)    15347 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/eval.py
+-rw-rw-rw-   0 root         (0) root         (0)    24141 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7872 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     6753 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-06-07 09:29:14.000000 utopya-1.2.5/utopya_cli/test.py
```

### Comparing `utopya-1.2.4/COPYING` & `utopya-1.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/COPYING.LESSER` & `utopya-1.2.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/PKG-INFO` & `utopya-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utopya
-Version: 1.2.4
+Version: 1.2.5
 Summary: A simulation management and evaluation framework
 Home-page: https://gitlab.com/utopia-project/utopya
 Author: utopya developers
 Author-email: Benjamin Herdeanu <Benjamin.Herdeanu@iup.uni-heidelberg.de>, Yunus Sevinchan <yunus.sevinchan@hu-berlin.de>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `utopya-1.2.4/README.md` & `utopya-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/pyproject.toml` & `utopya-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/setup.py` & `utopya-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/_gen_figures/__init__.py` & `utopya-1.2.5/tests/_gen_figures/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/_gen_figures/test_plots.py` & `utopya-1.2.5/tests/_gen_figures/test_plots.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/backend/test_benchmark.py` & `utopya-1.2.5/tests/backend/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/backend/test_model.py` & `utopya-1.2.5/tests/backend/test_model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/backend/test_tools.py` & `utopya-1.2.5/tests/backend/test_tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test__shell_complete.py` & `utopya-1.2.5/tests/cli/test__shell_complete.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test__to_migrate.py` & `utopya-1.2.5/tests/cli/test__to_migrate.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test_batch.py` & `utopya-1.2.5/tests/cli/test_batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test_config.py` & `utopya-1.2.5/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test_models.py` & `utopya-1.2.5/tests/cli/test_models.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test_projects.py` & `utopya-1.2.5/tests/cli/test_projects.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test_run_and_eval.py` & `utopya-1.2.5/tests/cli/test_run_and_eval.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/cli/test_test.py` & `utopya-1.2.5/tests/cli/test_test.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/eval/test_containers.py` & `utopya-1.2.5/tests/eval/test_containers.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/eval/test_datamanager.py` & `utopya-1.2.5/tests/eval/test_datamanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/eval/test_groups.py` & `utopya-1.2.5/tests/eval/test_groups.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/eval/test_plot_utils.py` & `utopya-1.2.5/tests/eval/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/tests/eval/test_plotting.py` & `utopya-1.2.5/tests/eval/test_plotting.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/__init__.py` & `utopya-1.2.5/utopya/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 utopya as its frontend.
 For model implementations, the :py:mod:`utopya_backend` package can assist in
 building Python-based models that use :py:mod:`utopya` as a frontend.
 
 Also visit :ref:`the user manual front page <welcome>` for more information.
 """
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 """The :py:mod:`utopya` package version"""
 
 # .. Logging ..................................................................
 # TODO Consider setting up logging elsewhere -- but needs to be done first!
 from dantro.logging import REMARK as _DEFAULT_LOG_LEVEL
 from dantro.logging import getLogger as _getLogger
```

### Comparing `utopya-1.2.4/utopya/_cluster.py` & `utopya-1.2.5/utopya/_cluster.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/_import_tools.py` & `utopya-1.2.5/utopya/_import_tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/_yaml_registry/entry.py` & `utopya-1.2.5/utopya/_yaml_registry/entry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/_yaml_registry/registry.py` & `utopya-1.2.5/utopya/_yaml_registry/registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/batch.py` & `utopya-1.2.5/utopya/batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/cfg/base_cfg.yml` & `utopya-1.2.5/utopya/cfg/base_cfg.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/cfg/base_plots.yml` & `utopya-1.2.5/utopya/cfg/base_plots.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/cfg/btm_cfg.yml` & `utopya-1.2.5/utopya/cfg/btm_cfg.yml`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/cfg.py` & `utopya-1.2.5/utopya/cfg.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/_plot_func_resolver.py` & `utopya-1.2.5/utopya/eval/_plot_func_resolver.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/containers.py` & `utopya-1.2.5/utopya/eval/containers.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/data_ops.py` & `utopya-1.2.5/utopya/eval/data_ops.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/datamanager.py` & `utopya-1.2.5/utopya/eval/datamanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/groups.py` & `utopya-1.2.5/utopya/eval/groups.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plotcreators.py` & `utopya-1.2.5/utopya/eval/plotcreators.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plothelper.py` & `utopya-1.2.5/utopya/eval/plothelper.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plotmanager.py` & `utopya-1.2.5/utopya/eval/plotmanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/_attractor.py` & `utopya-1.2.5/utopya/eval/plots/_attractor.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/_graph.py` & `utopya-1.2.5/utopya/eval/plots/_graph.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/_mpl.py` & `utopya-1.2.5/utopya/eval/plots/_mpl.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/_utils.py` & `utopya-1.2.5/utopya/eval/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/abm.py` & `utopya-1.2.5/utopya/eval/plots/abm.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/attractor.py` & `utopya-1.2.5/utopya/eval/plots/attractor.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/ca.py` & `utopya-1.2.5/utopya/eval/plots/ca.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/distributions.py` & `utopya-1.2.5/utopya/eval/plots/distributions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/graph.py` & `utopya-1.2.5/utopya/eval/plots/graph.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/snsplot.py` & `utopya-1.2.5/utopya/eval/plots/snsplot.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/plots/time_series.py` & `utopya-1.2.5/utopya/eval/plots/time_series.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/eval/transform.py` & `utopya-1.2.5/utopya/eval/transform.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/exceptions.py` & `utopya-1.2.5/utopya/exceptions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model.py` & `utopya-1.2.5/utopya/model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model_registry/__init__.py` & `utopya-1.2.5/utopya/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model_registry/_registration.py` & `utopya-1.2.5/utopya/model_registry/_registration.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model_registry/entry.py` & `utopya-1.2.5/utopya/model_registry/entry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model_registry/info_bundle.py` & `utopya-1.2.5/utopya/model_registry/info_bundle.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model_registry/registry.py` & `utopya-1.2.5/utopya/model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/model_registry/utils.py` & `utopya-1.2.5/utopya/model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/multiverse.py` & `utopya-1.2.5/utopya/multiverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1070,16 +1070,17 @@
                 f"Expected file at:  {execpath}"
             )
 
         elif not os.access(execpath, os.X_OK):
             raise PermissionError(
                 f"The specified executable path for model '{self.model_name}' "
                 "does not point to an executable file. Did you set the "
-                f"correct access rights? Use chmod to adjust access rights.\n"
-                "Executable path:  {execpath}"
+                f"correct access rights?\n"
+                "Use the chmod command to mark the file as executable:\n\n"
+                f"  chmod +x {execpath}\n"
             )
 
         if run_from_tmpdir:
             self._tmpdir = TemporaryDirectory(prefix=self.model_name)
             tmp_execpath = os.path.join(
                 self._tmpdir.name, os.path.basename(execpath)
             )
```

### Comparing `utopya-1.2.4/utopya/parameter.py` & `utopya-1.2.5/utopya/parameter.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/plotting.py` & `utopya-1.2.5/utopya/plotting.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/project_registry.py` & `utopya-1.2.5/utopya/project_registry.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/reporter.py` & `utopya-1.2.5/utopya/reporter.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/stop_conditions.py` & `utopya-1.2.5/utopya/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/task.py` & `utopya-1.2.5/utopya/task.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/testtools.py` & `utopya-1.2.5/utopya/testtools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/tools.py` & `utopya-1.2.5/utopya/tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/workermanager.py` & `utopya-1.2.5/utopya/workermanager.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya/yaml.py` & `utopya-1.2.5/utopya/yaml.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya.egg-info/PKG-INFO` & `utopya-1.2.5/utopya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utopya
-Version: 1.2.4
+Version: 1.2.5
 Summary: A simulation management and evaluation framework
 Home-page: https://gitlab.com/utopia-project/utopya
 Author: utopya developers
 Author-email: Benjamin Herdeanu <Benjamin.Herdeanu@iup.uni-heidelberg.de>, Yunus Sevinchan <yunus.sevinchan@hu-berlin.de>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `utopya-1.2.4/utopya.egg-info/SOURCES.txt` & `utopya-1.2.5/utopya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/benchmark.py` & `utopya-1.2.5/utopya_backend/benchmark.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/logging.py` & `utopya-1.2.5/utopya_backend/logging.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/model/__init__.py` & `utopya-1.2.5/utopya_backend/model/__init__.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/model/base.py` & `utopya-1.2.5/utopya_backend/model/base.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/model/step.py` & `utopya-1.2.5/utopya_backend/model/step.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/signal.py` & `utopya-1.2.5/utopya_backend/signal.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_backend/tools.py` & `utopya-1.2.5/utopya_backend/tools.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/_copy_model.py` & `utopya-1.2.5/utopya_cli/_copy_model.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/_shared.py` & `utopya-1.2.5/utopya_cli/_shared.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/_utils.py` & `utopya-1.2.5/utopya_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/batch.py` & `utopya-1.2.5/utopya_cli/batch.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/cli.py` & `utopya-1.2.5/utopya_cli/cli.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/config.py` & `utopya-1.2.5/utopya_cli/config.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/eval.py` & `utopya-1.2.5/utopya_cli/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 #
 #
 #
 @click.pass_context
 def evaluate(ctx, **params):
     """Invokes a model simulation run and subsequent evaluation"""
     import utopya
-    from utopya.exceptions import ValidationError
     from utopya.tools import pformat
 
     _log = utopya._getLogger("utopya")  # TODO How best to do this?!
 
     # Preparations . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
     _log.info("Parsing additional command line arguments ...")
     update_dict, update_plots_cfg = parse_update_dicts(_mode="eval", **params)
@@ -131,14 +130,16 @@
     *,
     ctx,
     mv: Union["Multiverse", "FrozenMultiverse"],
     _log=log,
     **params,
 ):
     """Wrapper that takes care of loading and evaluating"""
+    from utopya.tools import pformat
+
     _log.progress(
         "Beginning evaluation: loading data and starting PlotManager ...\n"
     )
 
     # Loading data into the data tree and (optionally) showing it .............
     if not params["use_data_tree_cache"]:
         mv.dm.load_from_cfg()
```

### Comparing `utopya-1.2.4/utopya_cli/models.py` & `utopya-1.2.5/utopya_cli/models.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/projects.py` & `utopya-1.2.5/utopya_cli/projects.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/run.py` & `utopya-1.2.5/utopya_cli/run.py`

 * *Files identical despite different names*

### Comparing `utopya-1.2.4/utopya_cli/test.py` & `utopya-1.2.5/utopya_cli/test.py`

 * *Files identical despite different names*

