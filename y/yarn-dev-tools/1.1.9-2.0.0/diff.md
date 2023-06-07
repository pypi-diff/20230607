# Comparing `tmp/yarn-dev-tools-1.1.9.tar.gz` & `tmp/yarn-dev-tools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yarn-dev-tools-1.1.9.tar", max compression
+gzip compressed data, was "yarn-dev-tools-2.0.0.tar", max compression
```

## Comparing `yarn-dev-tools-1.1.9.tar` & `yarn-dev-tools-2.0.0.tar`

### file list

```diff
@@ -1,80 +1,102 @@
--rwxr-xr-x   0        0        0     1286 2020-08-18 18:59:10.000000 yarn-dev-tools-1.1.9/LICENSE
--rwxr-xr-x   0        0        0     8577 2023-06-07 15:17:38.331261 yarn-dev-tools-1.1.9/README.md
--rw-r--r--   0        0        0     1459 2023-06-07 15:28:08.844514 yarn-dev-tools-1.1.9/pyproject.toml
--rw-r--r--   0        0        0        8 2022-01-06 12:10:58.591525 yarn-dev-tools-1.1.9/yarndevtools/.gitignore
--rw-r--r--   0        0        0        0 2020-08-18 19:22:37.000000 yarn-dev-tools-1.1.9/yarndevtools/__init__.py
--rw-r--r--   0        0        0     3484 2023-06-07 15:17:38.343055 yarn-dev-tools-1.1.9/yarndevtools/argparser.py
--rw-r--r--   0        0        0       62 2022-01-06 12:10:58.593052 yarn-dev-tools-1.1.9/yarndevtools/cdsw/.gitignore
--rw-r--r--   0        0        0      540 2022-10-07 15:04:39.588060 yarn-dev-tools-1.1.9/yarndevtools/cdsw/Dockerfile
--rw-r--r--   0        0        0        0 2022-01-06 12:10:58.594830 yarn-dev-tools-1.1.9/yarndevtools/cdsw/__init__.py
--rw-r--r--   0        0        0    12326 2023-06-07 15:17:38.343925 yarn-dev-tools-1.1.9/yarndevtools/cdsw/cdsw_common.py
--rw-r--r--   0        0        0    22084 2023-06-07 15:17:38.345103 yarn-dev-tools-1.1.9/yarndevtools/cdsw/cdsw_config.py
--rw-r--r--   0        0        0    16485 2023-06-07 15:17:38.346473 yarn-dev-tools-1.1.9/yarndevtools/cdsw/cdsw_runner.py
--rw-r--r--   0        0        0     3138 2023-06-07 15:17:38.347591 yarn-dev-tools-1.1.9/yarndevtools/cdsw/constants.py
--rw-r--r--   0        0        0        0 2022-01-28 12:46:19.326799 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/__init__.py
--rw-r--r--   0        0        0     3688 2022-03-25 07:44:59.852898 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py
--rw-r--r--   0        0        0     2710 2022-11-14 14:38:31.676456 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py
--rw-r--r--   0        0        0     2577 2022-03-25 07:44:59.854589 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py
--rw-r--r--   0        0        0     2501 2022-03-25 07:44:59.855487 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/reviewsync_job_config.py
--rw-r--r--   0        0        0     4730 2023-06-07 15:17:38.348154 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_job_config.py
--rw-r--r--   0        0        0     5215 2023-04-05 01:43:33.240085 yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:38.991565 yarn-dev-tools-1.1.9/yarndevtools/cdsw/libreloader/__init__.py
--rw-r--r--   0        0        0     6288 2022-10-08 15:30:26.829864 yarn-dev-tools-1.1.9/yarndevtools/cdsw/libreloader/reload_dependencies.py
--rw-r--r--   0        0        0     9397 2022-01-06 12:12:38.994617 yarn-dev-tools-1.1.9/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt
--rw-r--r--   0        0        0     2493 2022-01-28 12:46:19.333950 yarn-dev-tools-1.1.9/yarndevtools/cdsw/restarter.py
--rwxr-xr-x   0        0        0     1145 2023-01-17 14:25:07.393686 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/clone_downstream_repos.sh
--rwxr-xr-x   0        0        0      893 2023-01-17 14:25:07.408136 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/clone_upstream_repos.sh
--rw-r--r--   0        0        0      980 2022-01-06 12:10:58.607176 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh
--rwxr-xr-x   0        0        0      734 2022-01-06 12:10:58.607369 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/exit-test.py
--rwxr-xr-x   0        0        0      806 2022-01-06 12:10:58.607585 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/exit-test2.py
--rwxr-xr-x   0        0        0      149 2022-01-06 12:10:58.607845 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/test.py
--rwxr-xr-x   0        0        0       56 2022-01-06 12:10:58.608064 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/test.sh
--rw-r--r--   0        0        0     4243 2022-09-23 12:01:04.799569 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh
--rw-r--r--   0        0        0      491 2022-10-07 15:05:52.226372 yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/install-requirements.sh
--rw-r--r--   0        0        0     2167 2022-11-12 11:48:51.946677 yarn-dev-tools-1.1.9/yarndevtools/cdsw/start_job.py
--rw-r--r--   0        0        0      516 2022-01-20 21:40:52.794108 yarn-dev-tools-1.1.9/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt
--rw-r--r--   0        0        0     2731 2021-03-26 06:41:50.421000 yarn-dev-tools-1.1.9/yarndevtools/cdsw_compat.py
--rw-r--r--   0        0        0        0 2020-08-16 20:16:33.000000 yarn-dev-tools-1.1.9/yarndevtools/commands/__init__.py
--rw-r--r--   0        0        0    11806 2023-06-07 15:17:38.348988 yarn-dev-tools-1.1.9/yarndevtools/commands/backporter.py
--rw-r--r--   0        0        0        0 2021-04-20 19:49:58.360499 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/__init__.py
--rw-r--r--   0        0        0    16114 2023-06-07 15:17:38.350769 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/branch_comparator.py
--rw-r--r--   0        0        0     5844 2021-04-20 19:49:58.361481 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/common.py
--rw-r--r--   0        0        0    17597 2022-03-25 07:44:59.858949 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/common_representation.py
--rw-r--r--   0        0        0    34636 2022-01-06 12:12:39.004030 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/group_matching.py
--rw-r--r--   0        0        0     4589 2021-05-05 17:23:20.255448 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/legacy_script.py
--rw-r--r--   0        0        0    22649 2023-06-07 15:17:38.352489 yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/simple_matching.py
--rw-r--r--   0        0        0     4954 2022-03-25 07:44:59.859747 yarn-dev-tools-1.1.9/yarndevtools/commands/format_patch_saver.py
--rw-r--r--   0        0        0     6268 2022-03-25 07:44:59.861044 yarn-dev-tools-1.1.9/yarndevtools/commands/patch_saver.py
--rw-r--r--   0        0        0     4847 2022-03-25 07:44:59.861741 yarn-dev-tools-1.1.9/yarndevtools/commands/review_branch_creator.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.005164 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/__init__.py
--rw-r--r--   0        0        0     1357 2022-02-23 14:40:39.023806 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/common.py
--rw-r--r--   0        0        0    11076 2022-03-25 07:44:59.862561 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/representation.py
--rw-r--r--   0        0        0     9083 2022-03-25 07:44:59.863362 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py
--rwxr-xr-x   0        0        0     2499 2022-01-06 12:12:39.005969 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/README.md
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.006124 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/__init__.py
--rw-r--r--   0        0        0      482 2022-01-06 12:12:39.006438 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/common.py
--rw-r--r--   0        0        0    10819 2022-01-06 12:12:39.006765 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/jira_wrapper.py
--rw-r--r--   0        0        0    10904 2022-03-25 07:44:59.864473 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/representation.py
--rwxr-xr-x   0        0        0    16327 2022-06-21 17:12:39.479946 yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/reviewsync.py
--rw-r--r--   0        0        0     5274 2022-03-25 07:44:59.865969 yarn-dev-tools-1.1.9/yarndevtools/commands/send_latest_command_data_in_mail.py
--rw-r--r--   0        0        0        0 2022-01-06 12:10:58.625913 yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultaggregator/__init__.py
--rw-r--r--   0        0        0     3260 2023-06-07 15:17:38.353851 yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultaggregator/common.py
--rw-r--r--   0        0        0    32944 2023-06-07 15:17:38.354693 yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultaggregator/representation.py
--rw-r--r--   0        0        0    45593 2023-06-07 15:27:51.090645 yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultaggregator/unit_test_result_aggregator.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.010105 yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultfetcher/__init__.py
--rwxr-xr-x   0        0        0    56119 2023-06-07 15:17:38.357221 yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultfetcher/unit_test_result_fetcher.py
--rw-r--r--   0        0        0     5163 2022-03-25 07:44:59.870797 yarn-dev-tools-1.1.9/yarndevtools/commands/upstream_jira_patch_differ.py
--rw-r--r--   0        0        0     4427 2022-03-25 07:44:59.871519 yarn-dev-tools-1.1.9/yarndevtools/commands/upstream_pr_fetcher.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.011215 yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/__init__.py
--rw-r--r--   0        0        0     3116 2022-01-06 12:12:39.011504 yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/common.py
--rw-r--r--   0        0        0    11072 2022-03-25 07:44:59.872666 yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/representation.py
--rw-r--r--   0        0        0    30282 2022-10-07 15:04:28.669991 yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py
--rw-r--r--   0        0        0     5549 2022-03-25 07:44:59.874359 yarn-dev-tools-1.1.9/yarndevtools/commands/zip_latest_command_data.py
--rw-r--r--   0        0        0    20858 2023-06-07 15:17:38.358492 yarn-dev-tools-1.1.9/yarndevtools/commands_common.py
--rw-r--r--   0        0        0        0 2022-01-06 12:10:58.634134 yarn-dev-tools-1.1.9/yarndevtools/common/__init__.py
--rw-r--r--   0        0        0    12377 2023-06-07 15:17:38.359251 yarn-dev-tools-1.1.9/yarndevtools/common/shared_command_utils.py
--rw-r--r--   0        0        0     1518 2022-10-07 15:04:28.706599 yarn-dev-tools-1.1.9/yarndevtools/constants.py
--rwxr-xr-x   0        0        0     5001 2023-06-07 15:17:38.360005 yarn-dev-tools-1.1.9/yarndevtools/yarn_dev_tools.py
--rw-r--r--   0        0        0      178 2022-03-25 07:44:59.878538 yarn-dev-tools-1.1.9/yarndevtools/yarn_dev_tools_config.py
--rw-r--r--   0        0        0    10247 1970-01-01 00:00:00.000000 yarn-dev-tools-1.1.9/setup.py
--rw-r--r--   0        0        0     9385 1970-01-01 00:00:00.000000 yarn-dev-tools-1.1.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1286 2020-08-18 18:59:10.000000 yarn-dev-tools-2.0.0/LICENSE
+-rwxr-xr-x   0        0        0     8774 2023-04-05 01:08:00.058196 yarn-dev-tools-2.0.0/README.md
+-rw-r--r--   0        0        0     1516 2023-04-05 01:08:06.458083 yarn-dev-tools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        8 2022-01-06 12:10:58.591525 yarn-dev-tools-2.0.0/yarndevtools/.gitignore
+-rw-r--r--   0        0        0        0 2020-08-18 19:22:37.000000 yarn-dev-tools-2.0.0/yarndevtools/__init__.py
+-rw-r--r--   0        0        0     4427 2023-04-05 01:08:00.070672 yarn-dev-tools-2.0.0/yarndevtools/argparser.py
+-rw-r--r--   0        0        0       62 2022-01-06 12:10:58.593052 yarn-dev-tools-2.0.0/yarndevtools/cdsw/.gitignore
+-rw-r--r--   0        0        0      540 2022-10-07 15:04:39.588060 yarn-dev-tools-2.0.0/yarndevtools/cdsw/Dockerfile
+-rw-r--r--   0        0        0        0 2022-01-06 12:10:58.594830 yarn-dev-tools-2.0.0/yarndevtools/cdsw/__init__.py
+-rw-r--r--   0        0        0    12351 2023-04-05 01:08:00.071605 yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_common.py
+-rw-r--r--   0        0        0    22094 2023-04-05 01:08:00.072542 yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_config.py
+-rw-r--r--   0        0        0    16493 2023-04-05 01:08:00.073523 yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_runner.py
+-rw-r--r--   0        0        0     3067 2023-04-05 01:08:00.074554 yarn-dev-tools-2.0.0/yarndevtools/cdsw/constants.py
+-rw-r--r--   0        0        0        0 2022-01-28 12:46:19.326799 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/__init__.py
+-rw-r--r--   0        0        0     3688 2022-03-25 07:44:59.852898 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py
+-rw-r--r--   0        0        0     2710 2022-11-14 14:38:31.676456 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py
+-rw-r--r--   0        0        0     2577 2022-03-25 07:44:59.854589 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py
+-rw-r--r--   0        0        0     2501 2022-03-25 07:44:59.855487 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/reviewsync_job_config.py
+-rw-r--r--   0        0        0     4733 2023-04-05 01:08:00.075302 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_email_job_config.py
+-rw-r--r--   0        0        0     5037 2022-01-28 12:46:19.330150 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:38.991565 yarn-dev-tools-2.0.0/yarndevtools/cdsw/libreloader/__init__.py
+-rw-r--r--   0        0        0     6288 2022-10-08 15:30:26.829864 yarn-dev-tools-2.0.0/yarndevtools/cdsw/libreloader/reload_dependencies.py
+-rw-r--r--   0        0        0     9397 2022-01-06 12:12:38.994617 yarn-dev-tools-2.0.0/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt
+-rw-r--r--   0        0        0     2493 2022-01-28 12:46:19.333950 yarn-dev-tools-2.0.0/yarndevtools/cdsw/restarter.py
+-rwxr-xr-x   0        0        0     1145 2023-01-17 14:25:07.393686 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_downstream_repos.sh
+-rwxr-xr-x   0        0        0      893 2023-01-17 14:25:07.408136 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_upstream_repos.sh
+-rw-r--r--   0        0        0      980 2022-01-06 12:10:58.607176 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh
+-rwxr-xr-x   0        0        0      734 2022-01-06 12:10:58.607369 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test.py
+-rwxr-xr-x   0        0        0      806 2022-01-06 12:10:58.607585 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test2.py
+-rwxr-xr-x   0        0        0      149 2022-01-06 12:10:58.607845 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/test.py
+-rwxr-xr-x   0        0        0       56 2022-01-06 12:10:58.608064 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/test.sh
+-rw-r--r--   0        0        0     4243 2022-09-23 12:01:04.799569 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh
+-rw-r--r--   0        0        0      491 2022-10-07 15:05:52.226372 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/install-requirements.sh
+-rw-r--r--   0        0        0     2167 2022-11-12 11:48:51.946677 yarn-dev-tools-2.0.0/yarndevtools/cdsw/start_job.py
+-rw-r--r--   0        0        0      516 2022-01-20 21:40:52.794108 yarn-dev-tools-2.0.0/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt
+-rw-r--r--   0        0        0     2731 2021-03-26 06:41:50.421000 yarn-dev-tools-2.0.0/yarndevtools/cdsw_compat.py
+-rw-r--r--   0        0        0        0 2020-08-16 20:16:33.000000 yarn-dev-tools-2.0.0/yarndevtools/commands/__init__.py
+-rw-r--r--   0        0        0    11904 2023-04-05 01:08:00.076368 yarn-dev-tools-2.0.0/yarndevtools/commands/backporter.py
+-rw-r--r--   0        0        0        0 2021-04-20 19:49:58.360499 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/__init__.py
+-rw-r--r--   0        0        0    16165 2023-04-05 01:08:00.077338 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/branch_comparator.py
+-rw-r--r--   0        0        0     5844 2021-04-20 19:49:58.361481 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common.py
+-rw-r--r--   0        0        0    17597 2022-03-25 07:44:59.858949 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common_representation.py
+-rw-r--r--   0        0        0    34636 2022-01-06 12:12:39.004030 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/group_matching.py
+-rw-r--r--   0        0        0     4589 2021-05-05 17:23:20.255448 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/legacy_script.py
+-rw-r--r--   0        0        0    23360 2023-04-05 01:08:00.078314 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/simple_matching.py
+-rw-r--r--   0        0        0     4954 2022-03-25 07:44:59.859747 yarn-dev-tools-2.0.0/yarndevtools/commands/format_patch_saver.py
+-rw-r--r--   0        0        0     6268 2022-03-25 07:44:59.861044 yarn-dev-tools-2.0.0/yarndevtools/commands/patch_saver.py
+-rw-r--r--   0        0        0     4847 2022-03-25 07:44:59.861741 yarn-dev-tools-2.0.0/yarndevtools/commands/review_branch_creator.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.005164 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/__init__.py
+-rw-r--r--   0        0        0     1357 2022-02-23 14:40:39.023806 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/common.py
+-rw-r--r--   0        0        0    11076 2022-03-25 07:44:59.862561 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/representation.py
+-rw-r--r--   0        0        0     9083 2022-03-25 07:44:59.863362 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py
+-rwxr-xr-x   0        0        0     2499 2022-01-06 12:12:39.005969 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/README.md
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.006124 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/__init__.py
+-rw-r--r--   0        0        0      482 2022-01-06 12:12:39.006438 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/common.py
+-rw-r--r--   0        0        0    10819 2022-01-06 12:12:39.006765 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/jira_wrapper.py
+-rw-r--r--   0        0        0    10904 2022-03-25 07:44:59.864473 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/representation.py
+-rwxr-xr-x   0        0        0    16327 2022-06-21 17:12:39.479946 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/reviewsync.py
+-rw-r--r--   0        0        0     5274 2022-03-25 07:44:59.865969 yarn-dev-tools-2.0.0/yarndevtools/commands/send_latest_command_data_in_mail.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:10:58.625913 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 01:08:00.078483 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/__init__.py
+-rw-r--r--   0        0        0    30693 2023-04-05 01:08:00.079967 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/aggregation.py
+-rw-r--r--   0        0        0    16485 2023-04-05 01:08:00.080474 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/model.py
+-rw-r--r--   0        0        0     3393 2023-04-05 01:08:00.081501 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/parser.py
+-rw-r--r--   0        0        0      948 2023-04-05 01:08:00.082455 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/constants.py
+-rw-r--r--   0        0        0     7395 2023-04-05 01:08:00.083377 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/aggregation.py
+-rw-r--r--   0        0        0     1422 2023-04-05 01:08:00.083694 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/model.py
+-rw-r--r--   0        0        0      245 2023-04-05 01:08:00.084499 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/parser.py
+-rw-r--r--   0        0        0     2977 2023-04-05 01:08:00.084837 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/persistence.py
+-rw-r--r--   0        0        0        0 2023-04-05 01:08:00.084984 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/__init__.py
+-rw-r--r--   0        0        0     7695 2023-04-05 01:08:00.085978 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/config.py
+-rw-r--r--   0        0        0     2106 2023-04-05 01:08:00.086633 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/parser.py
+-rw-r--r--   0        0        0     6173 2023-04-05 01:08:00.087520 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/processor.py
+-rw-r--r--   0        0        0     3263 2023-04-05 01:08:00.088492 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/gsheet.py
+-rw-r--r--   0        0        0    33662 2023-04-05 01:08:00.090043 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/representation.py
+-rw-r--r--   0        0        0     4787 2023-04-05 01:08:00.091411 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/unit_test_result_aggregator.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.010105 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/__init__.py
+-rw-r--r--   0        0        0    20068 2023-04-05 01:08:00.092008 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/cache.py
+-rw-r--r--   0        0        0     2235 2023-04-05 01:08:00.092400 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/common.py
+-rw-r--r--   0        0        0     8475 2023-04-05 01:08:00.092749 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/db.py
+-rw-r--r--   0        0        0     4344 2023-04-05 01:08:00.093106 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/email.py
+-rw-r--r--   0        0        0     8528 2023-04-05 01:08:00.093705 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/jenkins.py
+-rw-r--r--   0        0        0     5591 2023-04-05 01:08:00.094084 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/model.py
+-rw-r--r--   0        0        0     6924 2023-04-05 01:08:00.094695 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/parser.py
+-rwxr-xr-x   0        0        0    20496 2023-04-05 01:08:00.096137 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/unit_test_result_fetcher.py
+-rw-r--r--   0        0        0     5163 2022-03-25 07:44:59.870797 yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_jira_patch_differ.py
+-rw-r--r--   0        0        0     4427 2022-03-25 07:44:59.871519 yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_pr_fetcher.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.011215 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/__init__.py
+-rw-r--r--   0        0        0     3116 2022-01-06 12:12:39.011504 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/common.py
+-rw-r--r--   0        0        0    11072 2022-03-25 07:44:59.872666 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/representation.py
+-rw-r--r--   0        0        0    30282 2022-10-07 15:04:28.669991 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py
+-rw-r--r--   0        0        0     5549 2022-03-25 07:44:59.874359 yarn-dev-tools-2.0.0/yarndevtools/commands/zip_latest_command_data.py
+-rw-r--r--   0        0        0    21980 2023-04-05 01:08:00.097596 yarn-dev-tools-2.0.0/yarndevtools/commands_common.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:10:58.634134 yarn-dev-tools-2.0.0/yarndevtools/common/__init__.py
+-rw-r--r--   0        0        0     9647 2023-04-05 01:08:00.098260 yarn-dev-tools-2.0.0/yarndevtools/common/common_model.py
+-rw-r--r--   0        0        0     7921 2023-04-05 01:08:00.099136 yarn-dev-tools-2.0.0/yarndevtools/common/db.py
+-rw-r--r--   0        0        0    12378 2023-04-05 01:08:00.100462 yarn-dev-tools-2.0.0/yarndevtools/common/shared_command_utils.py
+-rw-r--r--   0        0        0     1518 2022-10-07 15:04:28.706599 yarn-dev-tools-2.0.0/yarndevtools/constants.py
+-rwxr-xr-x   0        0        0     6349 2023-04-05 01:08:00.101778 yarn-dev-tools-2.0.0/yarndevtools/yarn_dev_tools.py
+-rw-r--r--   0        0        0      178 2022-03-25 07:44:59.878538 yarn-dev-tools-2.0.0/yarndevtools/yarn_dev_tools_config.py
+-rw-r--r--   0        0        0    10651 1970-01-01 00:00:00.000000 yarn-dev-tools-2.0.0/setup.py
+-rw-r--r--   0        0        0     9587 1970-01-01 00:00:00.000000 yarn-dev-tools-2.0.0/PKG-INFO
```

### Comparing `yarn-dev-tools-1.1.9/LICENSE` & `yarn-dev-tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/README.md` & `yarn-dev-tools-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,44 +32,43 @@
 
 TODO
 
 # Getting started
 
 In order to use this tool, you need to have at least Python 3.8 installed.
 
-## Use yarn-dev-tools from package (recommended)
+## Use yarn-dev-tools from package (Recommended)
 If you don't want to tinker with the source code, you can download [yarn-dev-tools](https://pypi.org/project/yarn-dev-tools/#history) from PyPi as well.
 This is probably the easiest way to use it.
-
-
-Please check the [initial_setup.sh](initial_setup.sh) script.
-It has a `setup-vars` function at the beginning that define some environment variables:
+You don't need to install anything manually as I created a [script](initial_setup.sh) that performs the installation automatically.
+The script has a `setup-vars` function at the beginning that defines some environment variables:
 
 These are the following:
-- `YARNDEVTOOLS_ROOT`: specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.
-- `HADOOP_DEV_DIR` should be set to the upstream Hadoop repository root, e.g.: "/Users/snemeth/development/apache/hadoop/"
-- `CLOUDERA_HADOOP_ROOT` should be set to the downstream Hadoop repository root, e.g.: "/Users/snemeth/development/cloudera/hadoop/"
+- `YARNDEVTOOLS_ROOT`: Specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.
+- `HADOOP_DEV_DIR` Should be set to the upstream Hadoop repository root, e.g.: "~/development/apache/hadoop/"
+- `CLOUDERA_HADOOP_ROOT` Should be set to the downstream Hadoop repository root, e.g.: "~/development/cloudera/hadoop/"
 
-The latter 2 environment variables is better to be added to your bashrc file to keep them between the shells.
+The latter two environment variables is better to be added to your bashrc / zshrc file (depending on what shell you are using) to keep them between the shells.
 
 ## Use yarn-dev-tools from source
 If you want to use yarn-dev-tools from source, first you need to install its dependencies.
 The project root contains a pyproject.toml file that has all the dependencies listed.
 The project uses Poetry to resolve the dependencies so you need to [install poetry](https://python-poetry.org/docs/#installation) as well.
 Simply go to the root of this project and execute `poetry install --without localdev`.
 Alternatively, you can run `make` from the root of the project.
 
 ## Setting up handy aliases to use yarn-dev-tools
 If you completed the installation (either by source or by package), you may want to define some shell aliases to use the tool more easily.
+In my system, I have [these](
+https://github.com/szilard-nemeth/linux-env/blob/master/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).
+Please make sure to source this script so that the command 'yarndevtools' will be available since it's defined as a function.
+It is important to specify `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` as mentioned above, before sourcing the script.
 
+After these steps, you will have a basic set of aliases that is enough to get you started.
 
-So, you are ready to set up some aliases. 
-In my system, I have [these aliases](
-https://github.com/szilard-nemeth/linux-env/blob/94748d92ef32689805e89724948dd024a9936d59/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).
-If you run this script (with `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` specified as mentioned above), you will have a basic set of aliases that is enough to get you started.
 
 # Setting up yarn-dev-tools with Cloudera CDSW
 
 ## Initial setup
 1. Upload the initial setup scripts to the CDSW files, to the root directory (/home/cdsw)
 - [initial-cdsw-setup.sh](yarndevtools/cdsw/scripts/initial-cdsw-setup.sh)
 - [install-requirements.sh](yarndevtools/cdsw/scripts/install-requirements.sh)
@@ -153,15 +152,16 @@
 where REVIEWER_LIST is in this format: "r=user1,r=user2,r=user3,..."
 
 
 # Contributing
 
 ## Setup of pre-commit
 
-Configure precommit as described in this blogpost: https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/
+Configure precommit as described in [this blogpost](https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/).
+
 Commands:
 1. Install precommit: `pip install pre-commit`
 2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: 
    `$HOME/Library/Python/3.8/bin/pre-commit`.
 2. Execute `pre-commit install` to install git hooks in your `.git/` directory.
 
 ## Running the tests
@@ -174,8 +174,9 @@
 In case you're facing a similar issue:
 ```
 An error has occurred: InvalidManifestError: 
 =====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist
 Check the log at /<userhome>/.cache/pre-commit/pre-commit.log
 ```
 , please run: `pre-commit autoupdate`
-More info here: https://github.com/pre-commit/pre-commit/issues/577
+
+More info can be found [here](https://github.com/pre-commit/pre-commit/issues/577).
```

### Comparing `yarn-dev-tools-1.1.9/pyproject.toml` & `yarn-dev-tools-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "yarn-dev-tools"
-version = "1.1.9"
+version = "2.0.0"
 description = ""
 authors = ["Szilard Nemeth <szilard.nemeth88@gmail.com>"]
 keywords = ["YARN", "development", "dev environment"]
 readme = "README.md"
 homepage = "https://github.com/szilard-nemeth/yarn-dev-tools"
 repository = "https://github.com/szilard-nemeth/yarn-dev-tools"
 packages = [{include = "yarndevtools"}]
@@ -31,31 +31,34 @@
 
 # TODO Verify if this is required
 [tool.setuptools.package-data]
 yarndevtools = ["cdsw/unit-test-result-aggregator/*.txt", "cdsw/scripts/*.sh"]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
-python-common-lib = "1.0.4"
-google-api-wrapper2 = "1.0.4"
+python = "^3.8.12"
+python-common-lib = "1.0.6"
+google-api-wrapper2 = "1.0.5"
 gitpython = "*"
 humanize = "*"
 bs4 = "*"
 jira = "*"
 dataclasses-json = "*"
 dacite = "*"
+pymongo = "*"
+marshmallow = "*"
 
 
 [tool.poetry.group.dev.dependencies]
 requests = "*"
-flake8 = "*"
+flake8 = "6.0.0"
 pytest = "*"
 pytest-html = "*"
 pytest-cov = "*"
+mongomock = "4.1.2"
 pre-commit = "*"
 coolname = "*"
 httpretty = "*"
 black = "*"
 autopep8 = "*"
 
 [tool.poetry.group.localdev.dependencies]
@@ -69,16 +72,14 @@
 
 
 
 
 
 
 
-
-
 
 
 
 
 
 [tool.poetry.scripts]
 exec-yarndevtools = "yarndevtools.yarn_dev_tools:run"
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/argparser.py` & `yarn-dev-tools-2.0.0/yarndevtools/argparser.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 from yarndevtools.commands.branchcomparator.branch_comparator import BranchComparator
 from yarndevtools.commands.format_patch_saver import FormatPatchSaver
 from yarndevtools.commands.patch_saver import PatchSaver
 from yarndevtools.commands.review_branch_creator import ReviewBranchCreator
 from yarndevtools.commands.reviewsheetbackportupdater.review_sheet_backport_updater import ReviewSheetBackportUpdater
 from yarndevtools.commands.reviewsync.reviewsync import ReviewSync
 from yarndevtools.commands.send_latest_command_data_in_mail import SendLatestCommandDataInEmail
-from yarndevtools.commands.unittestresultaggregator.unit_test_result_aggregator import (
-    UnitTestResultAggregator,
-)
+from yarndevtools.commands.unittestresultaggregator.unit_test_result_aggregator import UnitTestResultAggregator
+
+# TODO
+# from yarndevtools.commands.unittestresultaggregator.db.unit_test_result_aggregator_db import (
+#     DatabaseUnitTestResultAggregator
+# )
 from yarndevtools.commands.unittestresultfetcher.unit_test_result_fetcher import (
     UnitTestResultFetcher,
 )
 from yarndevtools.commands.upstream_jira_patch_differ import UpstreamJiraPatchDiffer
 from yarndevtools.commands.upstream_pr_fetcher import UpstreamPRFetcher
 from yarndevtools.commands.upstreamumbrellafetcher.upstream_jira_umbrella_fetcher import UpstreamJiraUmbrellaFetcher
 from yarndevtools.commands.zip_latest_command_data import ZipLatestCommandData
@@ -69,20 +72,50 @@
             action="store_true",
             dest="verbose",
             default=None,
             required=False,
             help="More verbose log (including gitpython verbose logs)",
         )
         parser.add_argument(
-            "-d",
+            "-lt",
+            "--trace",
+            action="store_true",
+            dest="logging_trace",
+            default=False,
+            required=False,
+            help="Set log level to TRACE",
+        )
+
+        parser.add_argument(
+            "-ld",
             "--debug",
             action="store_true",
-            dest="debug",
+            dest="logging_debug",
+            default=False,
+            required=False,
+            help="Set log level to DEBUG",
+        )
+
+        parser.add_argument(
+            "-lp",
+            "--logging-pythoncommons",
+            dest="logging_level_pythoncommons",
+            type=str,
+            default=None,
+            required=False,
+            help="Set log level of pythoncommons",
+        )
+
+        parser.add_argument(
+            "-lg",
+            "--logging-googleapiwrapper",
+            dest="logging_level_googleapiwrapper",
+            type=str,
             default=None,
             required=False,
-            help="Turn on console debug level logs",
+            help="Set log level of google api wrapper",
         )
 
         args = parser.parse_args()
         if args.verbose:
             print("Args: " + str(args))
         return args, parser
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/Dockerfile` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/Dockerfile`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/cdsw_common.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ProjectRootDeterminationStrategy,
     PROJECTS_BASEDIR,
     PROJECTS_BASEDIR_NAME,
 )
 from yarndevtools.cdsw.constants import (
     CdswEnvVar,
     PROJECT_NAME,
-    UnitTestResultAggregatorEnvVar,
+    UnitTestResultAggregatorEmailEnvVar,
     SECRET_PROJECTS_DIR,
 )
 
 from yarndevtools.common.shared_command_utils import CommandType
 from yarndevtools.constants import YARNDEVTOOLS_MODULE_NAME, UPSTREAM_JIRA_BASE_URL
 
 # MAKE SURE THIS PRECEDES IMPORT TO pythoncommons
@@ -237,34 +237,34 @@
 
     @classmethod
     def determine_lines_to_skip(cls) -> List[str]:
         skip_lines_starting_with: List[str] = cls.DEFAULT_SKIP_LINES_STARTING_WITH
         # If env var "SKIP_AGGREGATION_RESOURCE_FILE" is specified, try to read file
         # The file takes precedence over the default list of DEFAULT_SKIP_LINES_STARTING_WITH
         skip_aggregation_res_file = OsUtils.get_env_value(
-            UnitTestResultAggregatorEnvVar.SKIP_AGGREGATION_RESOURCE_FILE.value
+            UnitTestResultAggregatorEmailEnvVar.SKIP_AGGREGATION_RESOURCE_FILE.value
         )
         skip_aggregation_res_file_auto_discovery_str = OsUtils.get_env_value(
-            UnitTestResultAggregatorEnvVar.SKIP_AGGREGATION_RESOURCE_FILE_AUTO_DISCOVERY.value
+            UnitTestResultAggregatorEmailEnvVar.SKIP_AGGREGATION_RESOURCE_FILE_AUTO_DISCOVERY.value
         )
         LOG.info(
             "Value of env var '%s': %s",
-            UnitTestResultAggregatorEnvVar.SKIP_AGGREGATION_RESOURCE_FILE_AUTO_DISCOVERY.value,
+            UnitTestResultAggregatorEmailEnvVar.SKIP_AGGREGATION_RESOURCE_FILE_AUTO_DISCOVERY.value,
             skip_aggregation_res_file_auto_discovery_str,
         )
 
         # TODO Bool parsing should be done in get_env_value
         if skip_aggregation_res_file_auto_discovery_str in ("True", "true", "1"):
             skip_aggregation_res_file_auto_discovery = True
         elif skip_aggregation_res_file_auto_discovery_str in ("False", "false", "0"):
             skip_aggregation_res_file_auto_discovery = False
         else:
             raise ValueError(
                 "Invalid value for environment variable '{}': {}".format(
-                    UnitTestResultAggregatorEnvVar.SKIP_AGGREGATION_RESOURCE_FILE_AUTO_DISCOVERY.value,
+                    UnitTestResultAggregatorEmailEnvVar.SKIP_AGGREGATION_RESOURCE_FILE_AUTO_DISCOVERY.value,
                     skip_aggregation_res_file_auto_discovery_str,
                 )
             )
 
         if skip_aggregation_res_file_auto_discovery:
             found_with_auto_discovery = cls._auto_discover_skip_aggregation_result_file()
             if found_with_auto_discovery:
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/cdsw_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pythoncommons.date_utils import DateUtils
 from pythoncommons.string_utils import auto_str
 
 from yarndevtools.cdsw.constants import (
     JiraUmbrellaFetcherEnvVar,
     BranchComparatorEnvVar,
     UnitTestResultFetcherEnvVar,
-    UnitTestResultAggregatorEnvVar,
+    UnitTestResultAggregatorEmailEnvVar,
     ReviewSheetBackportUpdaterEnvVar,
     ReviewSyncEnvVar,
     CdswEnvVar,
 )
 from yarndevtools.common.shared_command_utils import CommandType
 
 YARN_DEV_TOOLS_VAR_OVERRIDE_TEMPLATE = "Found argument in yarn_dev_tools_arguments and runconfig.yarn_dev_tools_arguments: '%s'. The latter will take predence."
@@ -283,15 +283,15 @@
 
 @auto_str
 class CdswJobConfigReader:
     command_to_env_var_class = {
         CommandType.JIRA_UMBRELLA_DATA_FETCHER: JiraUmbrellaFetcherEnvVar,
         CommandType.BRANCH_COMPARATOR: BranchComparatorEnvVar,
         CommandType.UNIT_TEST_RESULT_FETCHER: UnitTestResultFetcherEnvVar,
-        CommandType.UNIT_TEST_RESULT_AGGREGATOR: UnitTestResultAggregatorEnvVar,
+        CommandType.UNIT_TEST_RESULT_AGGREGATOR: UnitTestResultAggregatorEmailEnvVar,
         CommandType.REVIEW_SHEET_BACKPORT_UPDATER: ReviewSheetBackportUpdaterEnvVar,
         CommandType.REVIEWSYNC: ReviewSyncEnvVar,
     }
 
     @staticmethod
     def read_from_file(file):
         if not file:
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/cdsw_runner.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
     args, parser = ArgParser.parse_args()
     # TODO Temporarily removed
     # ProjectUtils.get_output_basedir(CDSW_PROJECT)
     # logging_config: SimpleLoggingSetupConfig = SimpleLoggingSetup.init_logger(
     #     project_name=CDSW_PROJECT,
     #     logger_name_prefix=CDSW_PROJECT,
     #     execution_mode=ExecutionMode.PRODUCTION,
-    #     console_debug=args.debug,
+    #     console_debug=args.logging_debug,
     #     postfix=args.cmd_type,
     #     verbose_git_log=args.verbose,
     # )
     # LOG.info("Logging to files: %s", logging_config.log_file_paths)
 
     config = CdswRunnerConfig(parser, args, CdswConfigReaderAdapter())
     cdsw_runner = CdswRunner(config)
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/constants.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 # TODO Add default value of all env vars to enum
 # TODO Move all EnvVar classes to commands?
 class CdswEnvVar(Enum):
     MAIL_ACC_PASSWORD = "MAIL_ACC_PASSWORD"
     MAIL_ACC_USER = "MAIL_ACC_USER"
     MAIL_RECIPIENTS = "MAIL_RECIPIENTS"
-    JENKINS_USER = "JENKINS_USER"
-    JENKINS_PASSWORD = "JENKINS_PASSWORD"
     CLOUDERA_HADOOP_ROOT = YarnDevToolsEnvVar.ENV_CLOUDERA_HADOOP_ROOT.value
     HADOOP_DEV_DIR = YarnDevToolsEnvVar.ENV_HADOOP_DEV_DIR.value
     PYTHONPATH = "PYTHONPATH"
     TEST_EXECUTION_MODE = "TEST_EXEC_MODE"
     PYTHON_MODULE_MODE = "PYTHON_MODULE_MODE"
     ENABLE_GOOGLE_DRIVE_INTEGRATION = "ENABLE_GOOGLE_DRIVE_INTEGRATION"
     INSTALL_REQUIREMENTS = "INSTALL_REQUIREMENTS"
@@ -57,15 +55,15 @@
     GSHEET_WORKSHEET = "GSHEET_WORKSHEET"
     GSHEET_JIRA_COLUMN = "GSHEET_JIRA_COLUMN"
     GSHEET_UPDATE_DATE_COLUMN = "GSHEET_UPDATE_DATE_COLUMN"
     GSHEET_STATUS_INFO_COLUMN = "GSHEET_STATUS_INFO_COLUMN"
     BRANCHES = "BRANCHES"
 
 
-class UnitTestResultAggregatorEnvVar(Enum):
+class UnitTestResultAggregatorEmailEnvVar(Enum):
     GSHEET_CLIENT_SECRET = "GSHEET_CLIENT_SECRET"
     GSHEET_SPREADSHEET = "GSHEET_SPREADSHEET"
     GSHEET_WORKSHEET = "GSHEET_WORKSHEET"
     REQUEST_LIMIT = "REQUEST_LIMIT"
     MATCH_EXPRESSION = "MATCH_EXPRESSION"
 
     # OPTIONALS
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/reviewsync_job_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/reviewsync_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_job_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_email_job_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from yarndevtools.cdsw.cdsw_common import (
     UnitTestResultAggregatorCdswUtils,
     GenericCdswConfigUtils,
 )
 from yarndevtools.cdsw.cdsw_config import Include
 from yarndevtools.cdsw.constants import CdswEnvVar
-from yarndevtools.commands.unittestresultaggregator.common import OperationMode
+from yarndevtools.commands.unittestresultaggregator.constants import OperationMode
 from yarndevtools.common.shared_command_utils import CommandType
 from yarndevtools.constants import ReportFile
 
 config = {
     "job_name": "Unit test result aggregator",
     "command_type": CommandType.UNIT_TEST_RESULT_AGGREGATOR,
     "env_sanitize_exceptions": ["MATCH_EXPRESSION", "GSHEET_COMPARE_WITH_JIRA_TABLE", "AGGREGATE_FILTERS"],
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 )
 from yarndevtools.common.shared_command_utils import CommandType
 
 config = {
     "job_name": "Unit test result fetcher",
     "command_type": CommandType.UNIT_TEST_RESULT_FETCHER,
     "env_sanitize_exceptions": [],
-    "mandatory_env_vars": ["MAIL_ACC_USER", "MAIL_ACC_PASSWORD", "JENKINS_USER", "JENKINS_PASSWORD"],
+    "mandatory_env_vars": ["MAIL_ACC_USER", "MAIL_ACC_PASSWORD"],
     "optional_env_vars": ["BUILD_PROCESSING_LIMIT", "FORCE_SENDING_MAIL", "RESET_JOB_BUILD_DATA"],
     "yarn_dev_tools_arguments": [
         lambda conf: f"{Include.when(conf.var('debugMode'), '--debug', '')}",
         f"{CommandType.UNIT_TEST_RESULT_FETCHER.name}",
         lambda conf: f"--smtp_server {conf.var('smtp_server')}",
         lambda conf: f"--smtp_port {conf.var('smtp_port')}",
         lambda conf: f"--account_user {conf.env('MAIL_ACC_USER')}",
         lambda conf: f"--account_password {conf.env('MAIL_ACC_PASSWORD')}",
-        lambda conf: f"--jenkins-user {conf.env('JENKINS_USER')}",
-        lambda conf: f"--jenkins-password {conf.env('JENKINS_PASSWORD')}",
         lambda conf: f"--sender {conf.var('sender')}",
         lambda conf: f"--recipients {conf.var('recipients')}",
         lambda conf: f"--mode {conf.var('mode')}",
         lambda conf: f"--testcase-filter {conf.var('testcase_filters')}",
         lambda conf: f"--request-limit {conf.var('buildProcessingLimit')}",
         lambda conf: f"--num-builds {JENKINS_BUILDS_EXAMINE_UNLIMITIED_VAL}",
         lambda conf: f"{Include.when(conf.var('omitJobSummary'), '--omit-job-summary', '')}",
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/libreloader/reload_dependencies.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/libreloader/reload_dependencies.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/restarter.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/restarter.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/clone_downstream_repos.sh` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_downstream_repos.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/clone_upstream_repos.sh` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_upstream_repos.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/exit-test.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/experiments/exit-test2.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test2.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/start_job.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/start_job.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/cdsw_compat.py` & `yarn-dev-tools-2.0.0/yarndevtools/cdsw_compat.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/backporter.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/backporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 GERRIT_REVIEWER_LIST = "r=snemeth,r=bteke,r=tdomok,r=rkhandelwal,r=susheel.gupta"
 DEFAULT_MAVEN_COMMAND = "mvn clean install -Pdist -DskipTests -Pnoshade  -Dmaven.javadoc.skip=true"
 WARNING_MESSAGE = (
     "!! Remember to build project to verify the backported commit compiles !!"
     f"Run this command to build the project: {DEFAULT_MAVEN_COMMAND}"
 )
-DEFAULT_REMOTE = "cauldron"
+DEFAULT_REMOTE = "gerrit"
 
 LOG = logging.getLogger(__name__)
 
 
 class Backporter(CommandAbs):
     """
     A class used to backport changes from an upstream repository to a downstream repository, having an assumption
@@ -62,14 +62,15 @@
         self.downstream_jira_id = self.args.downstream_jira_id
         self.downstream_branch = self.args.downstream_branch
         self.upstream_jira_id = self.args.upstream_jira_id
         self.upstream_branch = self.args.upstream_branch
         self.fetch_repos: bool = not self.args.no_fetch
         self.upstream_repo = upstream_repo
         self.downstream_repo: GitWrapper = downstream_repo
+        # TODO Make remote configurable with CLI switch (search for: "DEFAULT_REMOTE" in this file)
 
         gerrit_push_cmd = (
             "Run this command to push to gerrit: "
             f"git push {DEFAULT_REMOTE} HEAD:refs/for/{args.downstream_branch}%{GERRIT_REVIEWER_LIST}"
         )
 
         # A branch that is the base of the newly created downstream branch for this backport.
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/branch_comparator.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/branch_comparator.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,14 +332,16 @@
             YarnDevToolsConfig.PROJECT_OUT_ROOT,
         )
         branch_comparator.run()
 
     def run(self):
         self.config.full_cmd = OsUtils.determine_full_command()
         LOG.info(f"Starting Branch comparator... \n{str(self.config)}")
+
+        # TODO fetch here before doing validation
         self.validate_branches()
         # TODO Make fetching optional, argparse argument
         # self.repo.fetch(all=True)
         self.matching_result = self.compare()
         if self.config.run_legacy_script:
             LegacyScriptRunner.start(self.config, self.branches, self.repo.repo_path, self.matching_result)
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/common.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/common_representation.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common_representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/group_matching.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/group_matching.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/legacy_script.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/legacy_script.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/branchcomparator/simple_matching.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/simple_matching.py`

 * *Files 3% similar despite different names*

```diff
@@ -449,31 +449,49 @@
         color_conf = ColorizeConfig(
             [
                 ColorDescriptor(bool, True, Color.GREEN, MatchType.ALL, (0, row_len), (0, row_len)),
                 ColorDescriptor(bool, False, Color.RED, MatchType.ANY, (0, row_len), (0, row_len)),
             ],
             eval_method=EvaluationMethod.ALL,
         )
-        self._add_all_comits_table(header, all_commits, colorize_conf=color_conf)
-        self._add_all_comits_table(header, all_commits, colorize_conf=None)
+        self._add_all_comits_table(header, all_commits, colorize_conf=color_conf, row_number_in_header=True)
+        self._add_all_comits_table(header, all_commits, colorize_conf=None, row_number_in_header=True)
 
-    def _add_all_comits_table(self, header, all_commits, colorize_conf: ColorizeConfig = None):
+    def _add_all_comits_table(
+        self, header, all_commits, colorize_conf: ColorizeConfig = None, row_number_in_header: bool = False
+    ):
         table_type = BranchComparatorTableType.ALL_COMMITS_MERGED
         colorize = True if colorize_conf else False
 
         render_conf = TableRenderingConfig(
             row_callback=lambda row: row,
             print_result=False,
             max_width=100,
             max_width_separator=" ",
-            add_row_numbers=False,
+            add_row_numbers=True,
             tabulate_formats=DEFAULT_TABLE_FORMATS,
             bool_conversion_config=BoolConversionConfig(),
             colorize_config=colorize_conf,
         )
+
+        first_row = all_commits[0]
+        actual_columns = len(first_row)
+        expected_columns = len(header)
+        if row_number_in_header:
+            expected_columns = expected_columns - 1
+
+        if expected_columns != actual_columns:
+            raise ValueError(
+                "Header is misaligned! \n"
+                "Expected columns: {}, "
+                "Actual columns: {} \n"
+                "Row number in header: {} \n"
+                "Header: {} \n"
+                "First row: {}".format(expected_columns, actual_columns, row_number_in_header, header, first_row)
+            )
         gen_tables = ResultPrinter.print_tables(data=all_commits, header=header, render_conf=render_conf)
         for table_fmt, table in gen_tables.items():
             self.add_table(
                 table_type,
                 BranchComparatorTable(
                     table_type.header, header, all_commits, table, table_fmt=table_fmt, colorized=colorize
                 ),
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/format_patch_saver.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/format_patch_saver.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/patch_saver.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/patch_saver.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/review_branch_creator.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/review_branch_creator.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/common.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/representation.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/README.md` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/README.md`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/jira_wrapper.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/jira_wrapper.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/representation.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/reviewsync/reviewsync.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/reviewsync.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/send_latest_command_data_in_mail.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/send_latest_command_data_in_mail.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/unittestresultaggregator/representation.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,29 @@
     GenericTableWithHeader,
     ResultPrinter,
     DEFAULT_TABLE_FORMATS,
     TableRenderingConfig,
 )
 from pythoncommons.string_utils import StringUtils, auto_str
 
-from yarndevtools.commands.unittestresultaggregator.common import (
-    get_key_by_testcase_filter,
+from yarndevtools.commands.unittestresultaggregator.constants import (
     OperationMode,
     SummaryMode,
-    TestCaseFilter,
-    FailedTestCase,
-    FailedTestCaseAggregated,
+)
+from yarndevtools.commands.unittestresultaggregator.common.model import (
     BuildComparisonResult,
+    FailedTestCaseAggregated,
+    TestCaseFilter,
+    FailedTestCaseAbs,
+    TestCaseFilters,
+    AggregatedFailurePropertyFilter,
+    FailedBuildFromEmail,
 )
+from yarndevtools.commands.unittestresultaggregator.common.aggregation import AggregationResults
+from yarndevtools.commands.unittestresultaggregator.db.model import EmailContent
 from yarndevtools.constants import (
     ReportFile,
 )
 
 LOG = logging.getLogger(__name__)
 
 
@@ -57,24 +63,24 @@
         self.header = header_value
 
 
 @dataclass
 class OutputFormatRules:
     truncate_length: bool
     abbrev_tc_package: str or None
-    truncate_subject_with: str or None
+    truncate_origin_with: str or None
 
 
-# TODO Get rid of this later?
 @auto_str
 class UnitTestResultAggregatorTableRenderingConfig(TableRenderingConfig):
+    # TODO refactor: Get rid of this class later?
     def __init__(
         self,
         data_type: TableDataType = None,
-        testcase_filters: List[TestCaseFilter] or None = None,
+        testcase_filters: TestCaseFilters or None = None,
         header: List[str] = None,
         table_types: List[TableOutputFormat] = None,
         out_fmt: OutputFormatRules or None = None,
         row_callback=None,
         tabulate_formats: List[TabulateTableFormat] = DEFAULT_TABLE_FORMATS,
         simple_mode=False,
         max_width=200,
@@ -83,20 +89,21 @@
         print_result=False,
     ):
         super().__init__(row_callback, tabulate_formats=tabulate_formats)
         self.print_result = print_result
         self.add_row_numbers = add_row_numbers
         self.max_width_separator = max_width_separator
         self.max_width = max_width
-        self.testcase_filters = [] if not testcase_filters else testcase_filters
+        self.testcase_filters = TestCaseFilters.create_empty() if not testcase_filters else testcase_filters
         self.header = header
         self.data_type = data_type
         self.table_types = table_types
         self.out_fmt = out_fmt
         self.simple_mode = simple_mode
+        # TODO refactor: Debug when these can be None: self.data_type, self.testcase_filters
         LOG.info(
             f"Testcase filters for data type '{self.data_type}': {[tcf.short_str() for tcf in self.testcase_filters]}"
         )
 
 
 class SummaryGenerator:
     jira_crosscheck_headers = ["Known failure?", "Reoccurred failure?"]
@@ -114,66 +121,66 @@
         self._callback_dict: Dict[TableOutputFormat, Callable] = {
             TableOutputFormat.REGULAR: self._regular_table,
             TableOutputFormat.REGULAR_WITH_COLORS: self._colorized_table,
             TableOutputFormat.HTML: self._html_table,
         }
 
     @classmethod
-    def process_testcase_filter_results(
-        cls, tc_filter_results, query_result: ThreadQueryResults, config, output_manager
+    def process_aggregation_results(
+        cls, aggr_results: AggregationResults, query_result: ThreadQueryResults, config, output_manager
     ):
         if config.summary_mode != SummaryMode.NONE.value:
             # TODO fix
             # truncate = self.config.operation_mode == OperationMode.PRINT
             truncate = True if config.summary_mode == SummaryMode.TEXT.value else False
 
             # We apply the specified truncation / abbreviation rules only for TEXT based tables
             # HTML / Gsheet output is just fine with longer names.
             # If SummaryMode.ALL is used, we leave all values intact for simplicity.
-            if config.abbrev_tc_package or config.truncate_subject_with:
+            if config.abbrev_tc_package or config.truncate_origin_with:
                 if config.summary_mode in [SummaryMode.ALL.value, SummaryMode.HTML.value]:
                     LOG.warning(
-                        f"Either abbreviate package or truncate subject is enabled "
+                        f"Either abbreviate package or truncate origin is enabled "
                         f"but SummaryMode is set to '{config.summary_mode}'. "
                         "Leaving all data intact so truncate / abbreviate options are ignored."
                     )
                     config.abbrev_tc_package = None
-                    config.truncate_subject_with = None
+                    config.truncate_origin_with = None
 
             data_dict: Dict[TableDataType, Callable[[TestCaseFilter, OutputFormatRules], List[List[str]]]] = {
                 TableDataType.MATCHED_LINES: lambda tcf, out_fmt: DataConverter.convert_data_to_rows(
-                    tc_filter_results.get_failed_testcases_by_filter(tcf),
+                    aggr_results.get_failures(tcf),
                     out_fmt,
                 ),
                 TableDataType.MATCHED_LINES_AGGREGATED: lambda tcf, out_fmt: DataConverter.render_aggregated_rows_table(
-                    tc_filter_results.get_aggregated_testcases_by_filter(tcf),
+                    aggr_results.get_aggregated_testcases_by_filters(tcf),
                     out_fmt,
                 ),
                 TableDataType.MAIL_SUBJECTS: lambda tcf, out_fmt: DataConverter.convert_email_subjects(query_result),
                 TableDataType.UNIQUE_MAIL_SUBJECTS: lambda tcf, out_fmt: DataConverter.convert_unique_email_subjects(
                     query_result
                 ),
                 TableDataType.LATEST_FAILURES: lambda tcf, out_fmt: DataConverter.render_latest_failures_table(
-                    tc_filter_results.get_latest_failed_testcases_by_filter(tcf)
+                    aggr_results.get_latest_failures(tcf)
                 ),
                 TableDataType.BUILD_COMPARISON: lambda tcf, out_fmt: DataConverter.render_build_comparison_table(
-                    tc_filter_results.get_build_comparison_result_by_filter(tcf)
+                    aggr_results.get_build_comparison(tcf)
                 ),
                 TableDataType.UNKNOWN_FAILURES: lambda tcf, out_fmt: DataConverter.render_aggregated_rows_table(
-                    tc_filter_results.get_aggregated_testcases_by_filter(tcf, filter_unknown=True),
+                    aggr_results.get_aggregated_testcases_by_filters(tcf, AggregatedFailurePropertyFilter.UNKNOWN),
                     out_fmt,
                     basic_mode=True,
                 ),
                 TableDataType.REOCCURRED_FAILURES: lambda tcf, out_fmt: DataConverter.render_aggregated_rows_table(
-                    tc_filter_results.get_aggregated_testcases_by_filter(tcf, filter_reoccurred=True),
+                    aggr_results.get_aggregated_testcases_by_filters(tcf, AggregatedFailurePropertyFilter.REOCCURRED),
                     out_fmt,
                     basic_mode=True,
                 ),
                 TableDataType.TESTCASES_TO_JIRAS: lambda tcf, out_fmt: DataConverter.render_aggregated_rows_table(
-                    tc_filter_results.get_aggregated_testcases_by_filter(tcf), out_fmt
+                    aggr_results.get_aggregated_testcases_by_filters(tcf), out_fmt
                 ),
             }
 
             detailed_render_confs = cls.detailed_render_confs(config, truncate)
             short_render_confs = cls.short_render_confs(config, truncate)
             detailed_report_files: Dict[SummaryMode, str] = {
                 SummaryMode.HTML: ReportFile.DETAILED_HTML.value,
@@ -193,22 +200,22 @@
             # These should be written to files regardless of the SummaryMode setting
             output_manager.process_rendered_table_data(table_renderer, TableDataType.MAIL_SUBJECTS)
             output_manager.process_rendered_table_data(table_renderer, TableDataType.UNIQUE_MAIL_SUBJECTS)
 
         if config.operation_mode == OperationMode.GSHEET:
             # We need to re-generate all the data here, as table renderer might rendered truncated data.
             LOG.info("Updating Google sheet with data...")
-            for tcf in config.testcase_filters.get_non_aggregate_filters():
-                failed_testcases = tc_filter_results.get_failed_testcases_by_filter(tcf)
+            for tcf in config.testcase_filter_defs.get_non_aggregate_filters():
+                failed_testcases = aggr_results.get_failures(tcf)
                 table_data = DataConverter.convert_data_to_rows(failed_testcases, OutputFormatRules(False, None, None))
                 SummaryGenerator._write_to_sheet(
                     config, "data", cls.matched_testcases_all_header, output_manager, table_data, tcf
                 )
-            for tcf in config.testcase_filters.get_aggregate_filters():
-                failed_testcases = tc_filter_results.get_aggregated_testcases_by_filter(tcf)
+            for tcf in config.testcase_filter_defs.get_aggregate_filters():
+                failed_testcases = aggr_results.get_aggregated_testcases_by_filters(tcf)
                 table_data = DataConverter.render_aggregated_rows_table(
                     failed_testcases, OutputFormatRules(False, None, None)
                 )
                 SummaryGenerator._write_to_sheet(
                     config,
                     f"aggregated data for aggregation filter {tcf}",
                     cls.matched_testcases_aggregated_header_full,
@@ -238,35 +245,35 @@
 
     @classmethod
     def short_render_confs(cls, config, truncate) -> List[UnitTestResultAggregatorTableRenderingConfig]:
         return [
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.BUILD_COMPARISON,
                 header=["Testcase", "Still failing", "Fixed", "New failure"],
-                testcase_filters=config.testcase_filters.LATEST_FAILURE_FILTERS,
+                testcase_filters=config.testcase_filter_defs.LATEST_FAILURE_FILTERS,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
-                out_fmt=OutputFormatRules(truncate, config.abbrev_tc_package, config.truncate_subject_with),
+                out_fmt=OutputFormatRules(truncate, config.abbrev_tc_package, config.truncate_origin_with),
             ),
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.UNKNOWN_FAILURES,
-                testcase_filters=config.testcase_filters.get_match_expression_aggregate_filters(),
+                testcase_filters=config.testcase_filter_defs.get_match_expression_aggregate_filters(),
                 header=cls.matched_testcases_aggregated_header_basic,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
                 out_fmt=OutputFormatRules(False, config.abbrev_tc_package, None),
             ),
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.REOCCURRED_FAILURES,
-                testcase_filters=config.testcase_filters.get_match_expression_aggregate_filters(),
+                testcase_filters=config.testcase_filter_defs.get_match_expression_aggregate_filters(),
                 header=cls.matched_testcases_aggregated_header_basic,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
                 out_fmt=OutputFormatRules(False, config.abbrev_tc_package, None),
             ),
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.TESTCASES_TO_JIRAS,
-                testcase_filters=config.testcase_filters.get_match_expression_aggregate_filters(),
+                testcase_filters=config.testcase_filter_defs.get_match_expression_aggregate_filters(),
                 header=cls.matched_testcases_aggregated_header_full,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
                 out_fmt=OutputFormatRules(False, config.abbrev_tc_package, None),
             ),
         ]
 
     @classmethod
@@ -287,24 +294,24 @@
         # Failed testcases_MR_Aggregated_CDPD-7.1.x (2)
         # Failed testcases_MR_Aggregated_CDPD-7.x (2)
         return [
             # Render tables for all match expressions + ALL values
             # --> 3 tables in case of 2 match expressions
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.MATCHED_LINES,
-                testcase_filters=config.testcase_filters.get_non_aggregate_filters(),
+                testcase_filters=config.testcase_filter_defs.get_non_aggregate_filters(),
                 header=cls.matched_testcases_all_header,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
-                out_fmt=OutputFormatRules(truncate, config.abbrev_tc_package, config.truncate_subject_with),
+                out_fmt=OutputFormatRules(truncate, config.abbrev_tc_package, config.truncate_origin_with),
             ),
             # Render tables for all match expressions AND all aggregation filters
             # --> 4 tables in case of 2 match expressions and 2 aggregate filters
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.MATCHED_LINES_AGGREGATED,
-                testcase_filters=config.testcase_filters.get_aggregate_filters(),
+                testcase_filters=config.testcase_filter_defs.get_aggregate_filters(),
                 header=cls.matched_testcases_aggregated_header_full,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
                 out_fmt=OutputFormatRules(False, config.abbrev_tc_package, None),
             ),
             UnitTestResultAggregatorTableRenderingConfig(
                 simple_mode=True,
                 header=["Subject", "Thread ID"],
@@ -320,17 +327,17 @@
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
                 testcase_filters=None,
                 out_fmt=None,
             ),
             UnitTestResultAggregatorTableRenderingConfig(
                 data_type=TableDataType.LATEST_FAILURES,
                 header=["Testcase", "Failure date", "Subject"],
-                testcase_filters=config.testcase_filters.LATEST_FAILURE_FILTERS,
+                testcase_filters=config.testcase_filter_defs.LATEST_FAILURE_FILTERS,
                 table_types=[TableOutputFormat.REGULAR, TableOutputFormat.HTML],
-                out_fmt=OutputFormatRules(truncate, config.abbrev_tc_package, config.truncate_subject_with),
+                out_fmt=OutputFormatRules(truncate, config.abbrev_tc_package, config.truncate_origin_with),
             ),
         ] + SummaryGenerator.short_render_confs(config, truncate)
 
     @staticmethod
     def _write_to_sheet(config, data_descriptor, header, output_manager, table_data, tcf):
         worksheet_name: str = config.get_worksheet_name(tcf)
         LOG.info(
@@ -373,15 +380,15 @@
 
     def generate_summary(
         self, render_confs: List[UnitTestResultAggregatorTableRenderingConfig], table_output_format: TableOutputFormat
     ) -> str:
         tables: List[GenericTableWithHeader] = []
         for conf in render_confs:
             for tcf in conf.testcase_filters:
-                alias = get_key_by_testcase_filter(tcf)
+                alias = tcf.key()
                 rendered_table = self._callback_dict[table_output_format](conf.data_type, alias=alias)
                 tables.append(rendered_table)
             if conf.simple_mode:
                 rendered_table = self._callback_dict[table_output_format](conf.data_type, alias=None)
                 tables.append(rendered_table)
 
         if table_output_format in [TableOutputFormat.REGULAR, TableOutputFormat.REGULAR_WITH_COLORS]:
@@ -410,15 +417,15 @@
             .append_html_tables(
                 table_tuples, separator=html_sep, header_type="h1", additional_separator_at_beginning=True
             )
             .render()
         )
 
 
-# TODO Try to extract this to common class (pythoncommons?), BranchComparator should move to this implementation later.
+# TODO refactor: Try to extract this to common class (pythoncommons?), BranchComparator should move to this implementation later.
 class TableRenderer:
     def __init__(self):
         self._tables: Dict[str, List[GenericTableWithHeader]] = {}
 
     def render_by_config(
         self,
         conf: UnitTestResultAggregatorTableRenderingConfig,
@@ -428,15 +435,15 @@
             self._render_tables(
                 header=conf.header,
                 data=data_callable(None, conf.out_fmt),
                 dtype=conf.data_type,
                 formats=conf.tabulate_formats,
             )
         for tcf in conf.testcase_filters:
-            key = get_key_by_testcase_filter(tcf)
+            key = tcf.key()
             self._render_tables(
                 header=conf.header,
                 data=data_callable(tcf, conf.out_fmt),
                 dtype=conf.data_type,
                 formats=conf.tabulate_formats,
                 append_to_header_title=f"_{key}",
                 table_alias=key,
@@ -587,75 +594,83 @@
             data,
             clear_range=True,
             worksheet_name=worksheet_name,
             create_not_existing_worksheet=create_not_existing,
         )
 
 
-# TODO This should be a simple renderer class without any data business logic
+# TODO refactor: This should be a simple renderer class without any data business logic
 class DataConverter:
-    SUBJECT_MAX_LENGTH = 50
+    ORIGIN_MAX_LENGTH = 50
     LINE_MAX_LENGTH = 80
 
     @staticmethod
-    def convert_data_to_rows(failed_testcases: List[FailedTestCase], out_fmt: OutputFormatRules) -> List[List[str]]:
+    def convert_data_to_rows(failed_testcases: List[FailedTestCaseAbs], out_fmt: OutputFormatRules) -> List[List[str]]:
         data_table: List[List[str]] = []
-        truncate_subject_by_length: bool = out_fmt.truncate_length
+        truncate_origin_by_length: bool = out_fmt.truncate_length
         truncate_testcase_by_length: bool = out_fmt.truncate_length
 
         for testcase in failed_testcases:
-            subject, testcase_name = DataConverter._apply_truncate_rules(
-                out_fmt, testcase, truncate_subject_by_length, truncate_testcase_by_length
+            origin, testcase_name = DataConverter._apply_truncate_rules(
+                out_fmt, testcase, truncate_origin_by_length, truncate_testcase_by_length
             )
+
+            # TODO yarndevtoolsv2 DB: dirty hack to get email fields
+            message_id, thread_id = "", ""
+            failed_build: FailedBuildFromEmail = getattr(testcase, "_failed_build")
+            if isinstance(failed_build, FailedBuildFromEmail):
+                email_content: EmailContent = getattr(failed_build, "_email_content")
+                message_id, thread_id = email_content.msg_id, email_content.thread_id
+
             data_table.append(
                 [
-                    str(testcase.email_meta.date),
-                    subject,
+                    str(testcase.date()),
+                    origin,
                     testcase_name,
-                    testcase.email_meta.message_id,
-                    testcase.email_meta.thread_id,
+                    message_id,
+                    thread_id,
                 ]
             )
         return data_table
 
     @staticmethod
-    def _apply_truncate_rules(out_fmt, testcase, truncate_subject_by_length, truncate_testcase_by_length):
+    def _apply_truncate_rules(out_fmt, testcase, truncate_origin_by_length, truncate_testcase_by_length):
         # Don't touch the original MatchObject data.
-        # It's not memory efficient to copy subject / TC name but we need the
+        # It's not memory efficient to copy origin / TC name but we need the
         # untruncated / original fields later.
-        subject = copy.copy(testcase.email_meta.subject)
-        testcase_name = copy.copy(testcase.full_name)
-        if out_fmt.truncate_subject_with:
-            subject = DataConverter._truncate_subject(subject, out_fmt.truncate_subject_with)
+        origin = copy.copy(testcase.origin())
+        testcase_name = copy.copy(testcase.full_name())
+        if out_fmt.truncate_origin_with:
+            origin = DataConverter._truncate_origin(origin, out_fmt.truncate_origin_with)
         if out_fmt.abbrev_tc_package:
             testcase_name = DataConverter._abbreviate_package_name(out_fmt.abbrev_tc_package, testcase_name)
 
         # Check length-based truncate, if still necessary
-        if truncate_subject_by_length and len(subject) > DataConverter.SUBJECT_MAX_LENGTH:
-            subject = DataConverter._truncate_str(subject, DataConverter.SUBJECT_MAX_LENGTH, "subject")
+        if truncate_origin_by_length and len(origin) > DataConverter.ORIGIN_MAX_LENGTH:
+            origin = DataConverter._truncate_str(origin, DataConverter.ORIGIN_MAX_LENGTH, "origin")
         if truncate_testcase_by_length:
             testcase_name = DataConverter._truncate_str(testcase_name, DataConverter.LINE_MAX_LENGTH, "testcase")
-        return subject, testcase_name
+        return origin, testcase_name
 
     @staticmethod
     def _abbreviate_package_name(abbrev_tc_package, testcase_name):
         if abbrev_tc_package in testcase_name:
             replacement = ".".join([p[0] for p in abbrev_tc_package.split(".")])
             new_testcase_name = f"{replacement}{testcase_name.split(abbrev_tc_package)[1]}"
             LOG.debug(f"Abbreviated testcase name: '{testcase_name}' -> {new_testcase_name}")
             testcase_name = new_testcase_name
         return testcase_name
 
     @staticmethod
-    def _truncate_subject(subject, truncate_subject_with):
-        if truncate_subject_with in subject:
-            new_subject = "".join([s for s in subject.split(truncate_subject_with) if s])
-            LOG.debug(f"Truncated subject: '{subject}' -> {new_subject}")
-            subject = new_subject
-        return subject
+    def _truncate_origin(origin, truncate_origin_with):
+        if truncate_origin_with in origin:
+            new_origin = "".join([s for s in origin.split(truncate_origin_with) if s])
+            LOG.debug(f"Truncated origin: '{origin}' -> {new_origin}")
+            origin = new_origin
+        return origin
 
     @staticmethod
     def render_aggregated_rows_table(
         failed_testcases: List[FailedTestCaseAggregated], out_fmt: OutputFormatRules = None, basic_mode=False
     ) -> List[List[str]]:
         data_table: List[List[str]] = []
         for testcase in failed_testcases:
@@ -670,29 +685,29 @@
         tc_name = testcase.simple_name
         if out_fmt.abbrev_tc_package:
             tc_name = DataConverter._abbreviate_package_name(out_fmt.abbrev_tc_package, tc_name)
         tc_param = "" if not testcase.parameter else testcase.parameter
         return [tc_name, tc_param, testcase.failure_freq, str(testcase.latest_failure)]
 
     @staticmethod
-    def render_latest_failures_table(failed_testcases: List[FailedTestCase]) -> List[List[str]]:
+    def render_latest_failures_table(failed_testcases: List[FailedTestCaseAbs]) -> List[List[str]]:
         data_table: List[List[str]] = []
         for testcase in failed_testcases:
-            data_table.append([testcase.full_name, testcase.email_meta.date, testcase.email_meta.subject])
+            data_table.append([testcase.full_name, testcase.date(), testcase.origin()])
         return data_table
 
     @classmethod
     def render_build_comparison_table(cls, result: BuildComparisonResult):
         data_table: List[List[str]] = []
         for tc in result.still_failing:
-            data_table.append([tc.full_name, True, False, False])
+            data_table.append([tc.full_name(), True, False, False])
         for tc in result.fixed:
-            data_table.append([tc.full_name, False, True, False])
-        for tc in result.new_failures:
-            data_table.append([tc.full_name, False, False, True])
+            data_table.append([tc.full_name(), False, True, False])
+        for tc in result.new:
+            data_table.append([tc.full_name(), False, False, True])
         return data_table
 
     @staticmethod
     def convert_email_subjects(query_result: ThreadQueryResults) -> List[List[str]]:
         data_table: List[List[str]] = []
         for tup in query_result.subjects_and_ids:
             data_table.append(list(tup))
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/upstream_jira_patch_differ.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_jira_patch_differ.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/upstream_pr_fetcher.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_pr_fetcher.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/common.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/representation.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands/zip_latest_command_data.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands/zip_latest_command_data.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/commands_common.py` & `yarn-dev-tools-2.0.0/yarndevtools/commands_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pythoncommons.git_constants import (
     COMMIT_FIELD_SEPARATOR,
     REVERT,
 )
 from pythoncommons.git_wrapper import GitLogLineFormat
 from pythoncommons.string_utils import auto_str
 
-from yarndevtools.commands.unittestresultaggregator.common import MATCH_EXPRESSION_PATTERN
+from yarndevtools.commands.unittestresultaggregator.constants import MATCH_EXPRESSION_PATTERN
 from yarndevtools.constants import (
     YARN_JIRA_ID_PATTERN,
 )
 
 LOG = logging.getLogger(__name__)
 
 
@@ -43,14 +43,61 @@
 
     @staticmethod
     @abstractmethod
     def execute(args, parser=None):
         pass
 
 
+class MongoArguments:
+    @staticmethod
+    def add_mongo_arguments(parser):
+        mongo_group = parser.add_argument_group("mongo", "Arguments for MongoDB integration")
+
+        parser.add_argument(
+            "-mhost",
+            "--mongo-hostname",
+            type=str,
+            dest="mongo.hostname",
+            help="MongoDB hostname",
+        )
+
+        parser.add_argument(
+            "-mport",
+            "--mongo-port",
+            type=str,
+            dest="mongo.port",
+            help="MongoDB port",
+        )
+        parser.add_argument(
+            "-muser",
+            "--mongo-user",
+            type=str,
+            dest="mongo.user",
+            help="MongoDB username",
+        )
+
+        parser.add_argument(
+            "-mpass",
+            "--mongo-password",
+            type=str,
+            dest="mongo.password",
+            help="MongoDB password",
+        )
+
+        parser.add_argument(
+            "-mdbname",
+            "--mongo-db-name",
+            type=str,
+            dest="mongo.db_name",
+            help="MongoDB DB name",
+        )
+
+        return mongo_group
+
+
 class GSheetArguments:
     @staticmethod
     def add_gsheet_arguments(parser):
         # Arguments for Google sheet integration
         gsheet_group = parser.add_argument_group("google-sheet", "Arguments for Google sheet integration")
 
         gsheet_group.add_argument(
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/common/shared_command_utils.py` & `yarn-dev-tools-2.0.0/yarndevtools/common/shared_command_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,14 +217,15 @@
         True,
         "latest-session-jira-umbrella-data-fetcher",
     )
     BRANCH_COMPARATOR = ("branch_comparator", "branch-comparator", True, "latest-session-branchcomparator")
     ZIP_LATEST_COMMAND_DATA = ("zip_latest_command_data", "zip-latest-command-data", False)
     SEND_LATEST_COMMAND_DATA = ("send_latest_command_data", "send-latest-command-data", False)
     UNIT_TEST_RESULT_FETCHER = ("unit_test_result_fetcher", "unit-test-result-fetcher", False)
+
     UNIT_TEST_RESULT_AGGREGATOR = (
         "unit_test_result_aggregator",
         "unit-test-result-aggregator",
         True,
         "latest-session-unit-test-result-aggregator",
     )
     REVIEW_SHEET_BACKPORT_UPDATER = (
```

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/constants.py` & `yarn-dev-tools-2.0.0/yarndevtools/constants.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-1.1.9/yarndevtools/yarn_dev_tools.py` & `yarn-dev-tools-2.0.0/yarndevtools/yarn_dev_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -79,33 +79,76 @@
     global args, cmd_type
     start_time = time.time()
     # TODO Revisit all exception handling: ValueError vs. exit() calls
     # Methods should throw exceptions, exit should be handled in this method
     YarnDevTools()
     # Parse args, commands will be mapped to YarnDevTools functions in ArgParser.parse_args
     args, parser = ArgParser.parse_args()
-    logging_config: SimpleLoggingSetupConfig = SimpleLoggingSetup.init_logger(
-        project_name=YARNDEVTOOLS_MODULE_NAME,
-        logger_name_prefix=YARNDEVTOOLS_MODULE_NAME,
-        execution_mode=ExecutionMode.PRODUCTION,
-        console_debug=args.debug,
-        postfix=args.command,
-        repos=[YarnDevToolsConfig.UPSTREAM_REPO.repo, YarnDevToolsConfig.DOWNSTREAM_REPO.repo],
-        verbose_git_log=args.verbose,
-    )
-    LOG.info("Logging to files: %s", logging_config.log_file_paths)
+
+    logging_config = configure_logging(args)
+
     cmd_type = CommandType.from_str(args.command)
     if cmd_type not in IGNORE_LATEST_SYMLINK_COMMANDS:
         for log_level, log_file_path in logging_config.log_file_paths.items():
             log_level_name = logging.getLevelName(log_level)
             link_name = cmd_type.log_link_name + "-" + log_level_name
             FileUtils.create_symlink_path_dir(link_name, log_file_path, YarnDevToolsConfig.PROJECT_OUT_ROOT)
     else:
         LOG.info(f"Skipping to re-create symlink as command is: {args.command}")
+
     # Call the handler function
     args.func(args, parser=parser)
     end_time = time.time()
     LOG.info("Execution of script took %d seconds", end_time - start_time)
 
 
+def configure_logging(args):
+    # TODO use this value later with SimpleLoggingSetup.init_logger instead of passing bool flags
+    # log_level = determine_logging_level(args)
+    debug = getattr(args, "logging_debug", False)
+    trace = getattr(args, "logging_trace", False)
+    logging_config: SimpleLoggingSetupConfig = SimpleLoggingSetup.init_logger(
+        project_name=YARNDEVTOOLS_MODULE_NAME,
+        logger_name_prefix=YARNDEVTOOLS_MODULE_NAME,
+        execution_mode=ExecutionMode.PRODUCTION,
+        # TODO find 'console_debug' in project and rename
+        console_debug=debug,
+        trace=trace,
+        postfix=args.command,
+        repos=[YarnDevToolsConfig.UPSTREAM_REPO.repo, YarnDevToolsConfig.DOWNSTREAM_REPO.repo],
+        verbose_git_log=args.verbose,
+        with_trace_level=True,
+    )
+    # LOG.trace("test trace")
+    LOG.info("Logging to files: %s", logging_config.log_file_paths)
+    configure_loggers(args)
+
+    return logging_config
+
+
+def configure_loggers(args):
+    googleapiwrapper_level = getattr(args, "logging_level_googleapiwrapper", None)
+    pythoncommons_level = getattr(args, "logging_level_pythoncommons", None)
+
+    if googleapiwrapper_level:
+        logging.getLogger("googleapiwrapper").setLevel(googleapiwrapper_level)
+    if pythoncommons_level:
+        logging.getLogger("pythoncommons").setLevel(pythoncommons_level)
+
+
+def determine_logging_level(args):
+    log_levels = {
+        logging.DEBUG: getattr(args, "logging_debug", False),
+        # TODO
+        # logging.TRACE: getattr(args, "logging_trace", False),
+        logging.INFO: True,  # Info is always on
+    }
+    val = 99999
+    for level_value, enabled in log_levels.items():
+        if level_value < val and enabled:
+            val = level_value
+
+    return logging.getLevelName(val)
+
+
 if __name__ == "__main__":
     run()
```

### Comparing `yarn-dev-tools-1.1.9/setup.py` & `yarn-dev-tools-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,17 @@
  'yarndevtools.cdsw.libreloader',
  'yarndevtools.cdsw.scripts.experiments',
  'yarndevtools.commands',
  'yarndevtools.commands.branchcomparator',
  'yarndevtools.commands.reviewsheetbackportupdater',
  'yarndevtools.commands.reviewsync',
  'yarndevtools.commands.unittestresultaggregator',
+ 'yarndevtools.commands.unittestresultaggregator.common',
+ 'yarndevtools.commands.unittestresultaggregator.db',
+ 'yarndevtools.commands.unittestresultaggregator.email',
  'yarndevtools.commands.unittestresultfetcher',
  'yarndevtools.commands.upstreamumbrellafetcher',
  'yarndevtools.common']
 
 package_data = \
 {'': ['*'],
  'yarndevtools.cdsw': ['resources/*',
@@ -23,34 +26,36 @@
                        'unit-test-result-aggregator/*']}
 
 install_requires = \
 ['bs4',
  'dacite',
  'dataclasses-json',
  'gitpython',
- 'google-api-wrapper2==1.0.4',
+ 'google-api-wrapper2==1.0.5',
  'humanize',
  'jira',
- 'python-common-lib==1.0.4']
+ 'marshmallow',
+ 'pymongo',
+ 'python-common-lib==1.0.6']
 
 entry_points = \
 {'console_scripts': ['exec-yarndevtools = yarndevtools.yarn_dev_tools:run']}
 
 setup_kwargs = {
     'name': 'yarn-dev-tools',
-    'version': '1.1.9',
+    'version': '2.0.0',
     'description': '',
-    'long_description': '[![CI for YARN dev tools (pip)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml)\n[![codecov](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools/branch/master/graph/badge.svg?token=OQD6FIFF7I)](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![GitHub language count](https://img.shields.io/github/languages/count/szilard-nemeth/yarn-dev-tools)\n\n\n# YARN-dev-tools\n\nThis project contains various developer helper scripts in order to simplify every day tasks related to Apache Hadoop YARN development.\n\n## Main dependencies\n\n* [gitpython](https://gitpython.readthedocs.io/en/stable/) - GitPython is a python library used to interact with git repositories, high-level like git-porcelain, or low-level like git-plumbing.\n* [tabulate](https://pypi.org/project/tabulate/) - python-tabulate: Pretty-print tabular data in Python, a library and a command-line utility.\n* [bs4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - Beautiful Soup is a Python library for pulling data out of HTML and XML files.\n\n* TODO: Missing dependencies\n\n## Contributing\n\nTODO \n\n## Authors\n\n* **Szilard Nemeth** - *Initial work* - [Szilard Nemeth](https://github.com/szilard-nemeth)\n\n## License\n\nTODO \n\n## Acknowledgments\n\nTODO\n\n# Getting started\n\nIn order to use this tool, you need to have at least Python 3.8 installed.\n\n## Use yarn-dev-tools from package (recommended)\nIf you don\'t want to tinker with the source code, you can download [yarn-dev-tools](https://pypi.org/project/yarn-dev-tools/#history) from PyPi as well.\nThis is probably the easiest way to use it.\n\n\nPlease check the [initial_setup.sh](initial_setup.sh) script.\nIt has a `setup-vars` function at the beginning that define some environment variables:\n\nThese are the following:\n- `YARNDEVTOOLS_ROOT`: specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.\n- `HADOOP_DEV_DIR` should be set to the upstream Hadoop repository root, e.g.: "/Users/snemeth/development/apache/hadoop/"\n- `CLOUDERA_HADOOP_ROOT` should be set to the downstream Hadoop repository root, e.g.: "/Users/snemeth/development/cloudera/hadoop/"\n\nThe latter 2 environment variables is better to be added to your bashrc file to keep them between the shells.\n\n## Use yarn-dev-tools from source\nIf you want to use yarn-dev-tools from source, first you need to install its dependencies.\nThe project root contains a pyproject.toml file that has all the dependencies listed.\nThe project uses Poetry to resolve the dependencies so you need to [install poetry](https://python-poetry.org/docs/#installation) as well.\nSimply go to the root of this project and execute `poetry install --without localdev`.\nAlternatively, you can run `make` from the root of the project.\n\n## Setting up handy aliases to use yarn-dev-tools\nIf you completed the installation (either by source or by package), you may want to define some shell aliases to use the tool more easily.\n\n\nSo, you are ready to set up some aliases. \nIn my system, I have [these aliases](\nhttps://github.com/szilard-nemeth/linux-env/blob/94748d92ef32689805e89724948dd024a9936d59/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).\nIf you run this script (with `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` specified as mentioned above), you will have a basic set of aliases that is enough to get you started.\n\n# Setting up yarn-dev-tools with Cloudera CDSW\n\n## Initial setup\n1. Upload the initial setup scripts to the CDSW files, to the root directory (/home/cdsw)\n- [initial-cdsw-setup.sh](yarndevtools/cdsw/scripts/initial-cdsw-setup.sh)\n- [install-requirements.sh](yarndevtools/cdsw/scripts/install-requirements.sh)\n\n2. Create a new CDSW session.\nWait for the session to be launched and open up a terminal by Clicking "Terminal access" on the top menu bar.\n\n\n3. Execute this command:\n```\n~/initial-cdsw-setup.sh user cloudera\n```\n\n\nThe script performs the following actions: \n1. Downloads the scripts that are cloning the upstream and downstream Hadoop repositories + installing yarndevtools itself as a python module.\nThe download location is: `/home/cdsw/scripts`<br>\nPlease note that the files will be downloaded from the GitHub master branch of this repository!\n- [clone_downstream_repos.sh](yarndevtools/cdsw/scripts/clone_downstream_repos.sh)\n- [clone_upstream_repos.sh](yarndevtools/cdsw/scripts/clone_upstream_repos.sh)\n\n2. Executes the script described in step 2. \nThis can take some time, especially cloning Hadoop.\nNote: The individual CDSW jobs should make sure for themselves to clone the repositories.\n\n3. Copies the [python-based job configs](yarndevtools/cdsw/job_configs) for all jobs to `/home/cdsw/jobs`\n\n4. All you have to do in CDSW is to set up the projects and their starter scripts like this:\n\n| Project                                                                | Starter script location         | Arguments for script          |\n|------------------------------------------------------------------------|---------------------------------|-------------------------------|\n| Jira umbrella data fetcher (Formerly: Jira umbrella checker reporting) | scripts/start_job.py            | jira-umbrella-data-fetcher    |\n| Unit test result aggregator                                            | scripts/start_job.py            | unit-test-result-aggregator   |\n| Unit test result fetcher (Formerly: Unit test result reporting)        | scripts/start_job.py            | unit-test-result-fetcher      |\n| Branch comparator (Formerly: Downstream branchdiff reporting)          | scripts/start_job.py            | branch-comparator             |\n| Review sheet backport updater                                          | scripts/start_job.py | review-sheet-backport-updater |\n| Reviewsync                                                             | scripts/start_job.py | reviewsync                    |\n\n# Use-cases\n\n\n### Examples for YARN backporter\nTo backport YARN-6221 to 2 branches, run these commands:\n```\nyarn-backport YARN-6221 COMPX-6664 cdpd-master\nyarn-backport YARN-6221 COMPX-6664 CDH-7.1-maint --no-fetch\n```\nThe first argument is the upstream Jira ID<br>\nThe second argument is the downstream Jira ID.<br>\nThe third argument is the downstream branch.<br>\nThe `--no-fetch` option is a means to skip git fetch on both repos.\n\n### How to backport to an already existing relation chain?\n1. Go to Gerrit UI and download the patch.\nFor example: \n```\ngit fetch "https://gerrit.sjc.cloudera.com/cdh/hadoop" refs/changes/29/156429/5 && git checkout FETCH_HEAD\n```\n2. Checkout a new branch\n```\ngit checkout -b my-relation-chain \n```\n\n3. Run backporter with: \n```\nyarn-backport YARN-10314 COMPX-7855 CDH-7.1.7.1000 --no-fetch --downstream_base_ref my-relation-chain\n```\nwhere:<br>\nThe first argument is the upstream Jira ID<br>\nThe second argument is the downstream Jira ID.<br>\nThe third argument is the downstream branch.<br>\nThe `--no-fetch` option is a means to skip git fetch on both repos.<br>\nThe `--downstream_base_ref <local-branch` is a way to use a local branch to base the backport on so the Git remote name won\'t be prepended.\n\n\nFinally, I set up two aliases for pushing the changes to the downstream repo:\n```\nalias git-push-to-cdpdmaster="git push <REMOTE> HEAD:refs/for/cdpd-master%<REVIEWER_LIST>"\nalias git-push-to-cdh71maint="git push <REMOTE> HEAD:refs/for/CDH-7.1-maint%<REVIEWER_LIST>"\n```\nwhere REVIEWER_LIST is in this format: "r=user1,r=user2,r=user3,..."\n\n\n# Contributing\n\n## Setup of pre-commit\n\nConfigure precommit as described in this blogpost: https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/\nCommands:\n1. Install precommit: `pip install pre-commit`\n2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: \n   `$HOME/Library/Python/3.8/bin/pre-commit`.\n2. Execute `pre-commit install` to install git hooks in your `.git/` directory.\n\n## Running the tests\n\nTODO\n\n## Troubleshooting\n\n### Installation issues\nIn case you\'re facing a similar issue:\n```\nAn error has occurred: InvalidManifestError: \n=====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist\nCheck the log at /<userhome>/.cache/pre-commit/pre-commit.log\n```\n, please run: `pre-commit autoupdate`\nMore info here: https://github.com/pre-commit/pre-commit/issues/577',
+    'long_description': '[![CI for YARN dev tools (pip)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml)\n[![codecov](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools/branch/master/graph/badge.svg?token=OQD6FIFF7I)](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![GitHub language count](https://img.shields.io/github/languages/count/szilard-nemeth/yarn-dev-tools)\n\n\n# YARN-dev-tools\n\nThis project contains various developer helper scripts in order to simplify every day tasks related to Apache Hadoop YARN development.\n\n## Main dependencies\n\n* [gitpython](https://gitpython.readthedocs.io/en/stable/) - GitPython is a python library used to interact with git repositories, high-level like git-porcelain, or low-level like git-plumbing.\n* [tabulate](https://pypi.org/project/tabulate/) - python-tabulate: Pretty-print tabular data in Python, a library and a command-line utility.\n* [bs4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - Beautiful Soup is a Python library for pulling data out of HTML and XML files.\n\n* TODO: Missing dependencies\n\n## Contributing\n\nTODO \n\n## Authors\n\n* **Szilard Nemeth** - *Initial work* - [Szilard Nemeth](https://github.com/szilard-nemeth)\n\n## License\n\nTODO \n\n## Acknowledgments\n\nTODO\n\n# Getting started\n\nIn order to use this tool, you need to have at least Python 3.8 installed.\n\n## Use yarn-dev-tools from package (Recommended)\nIf you don\'t want to tinker with the source code, you can download [yarn-dev-tools](https://pypi.org/project/yarn-dev-tools/#history) from PyPi as well.\nThis is probably the easiest way to use it.\nYou don\'t need to install anything manually as I created a [script](initial_setup.sh) that performs the installation automatically.\nThe script has a `setup-vars` function at the beginning that defines some environment variables:\n\nThese are the following:\n- `YARNDEVTOOLS_ROOT`: Specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.\n- `HADOOP_DEV_DIR` Should be set to the upstream Hadoop repository root, e.g.: "~/development/apache/hadoop/"\n- `CLOUDERA_HADOOP_ROOT` Should be set to the downstream Hadoop repository root, e.g.: "~/development/cloudera/hadoop/"\n\nThe latter two environment variables is better to be added to your bashrc / zshrc file (depending on what shell you are using) to keep them between the shells.\n\n## Use yarn-dev-tools from source\nIf you want to use yarn-dev-tools from source, first you need to install its dependencies.\nThe project root contains a pyproject.toml file that has all the dependencies listed.\nThe project uses Poetry to resolve the dependencies so you need to [install poetry](https://python-poetry.org/docs/#installation) as well.\nSimply go to the root of this project and execute `poetry install --without localdev`.\nAlternatively, you can run `make` from the root of the project.\n\n## Setting up handy aliases to use yarn-dev-tools\nIf you completed the installation (either by source or by package), you may want to define some shell aliases to use the tool more easily.\nIn my system, I have [these](\nhttps://github.com/szilard-nemeth/linux-env/blob/master/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).\nPlease make sure to source this script so that the command \'yarndevtools\' will be available since it\'s defined as a function.\nIt is important to specify `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` as mentioned above, before sourcing the script.\n\nAfter these steps, you will have a basic set of aliases that is enough to get you started.\n\n\n# Setting up yarn-dev-tools with Cloudera CDSW\n\n## Initial setup\n1. Upload the initial setup scripts to the CDSW files, to the root directory (/home/cdsw)\n- [initial-cdsw-setup.sh](yarndevtools/cdsw/scripts/initial-cdsw-setup.sh)\n- [install-requirements.sh](yarndevtools/cdsw/scripts/install-requirements.sh)\n\n2. Create a new CDSW session.\nWait for the session to be launched and open up a terminal by Clicking "Terminal access" on the top menu bar.\n\n\n3. Execute this command:\n```\n~/initial-cdsw-setup.sh user cloudera\n```\n\n\nThe script performs the following actions: \n1. Downloads the scripts that are cloning the upstream and downstream Hadoop repositories + installing yarndevtools itself as a python module.\nThe download location is: `/home/cdsw/scripts`<br>\nPlease note that the files will be downloaded from the GitHub master branch of this repository!\n- [clone_downstream_repos.sh](yarndevtools/cdsw/scripts/clone_downstream_repos.sh)\n- [clone_upstream_repos.sh](yarndevtools/cdsw/scripts/clone_upstream_repos.sh)\n\n2. Executes the script described in step 2. \nThis can take some time, especially cloning Hadoop.\nNote: The individual CDSW jobs should make sure for themselves to clone the repositories.\n\n3. Copies the [python-based job configs](yarndevtools/cdsw/job_configs) for all jobs to `/home/cdsw/jobs`\n\n4. All you have to do in CDSW is to set up the projects and their starter scripts like this:\n\n| Project                                                                | Starter script location         | Arguments for script          |\n|------------------------------------------------------------------------|---------------------------------|-------------------------------|\n| Jira umbrella data fetcher (Formerly: Jira umbrella checker reporting) | scripts/start_job.py            | jira-umbrella-data-fetcher    |\n| Unit test result aggregator                                            | scripts/start_job.py            | unit-test-result-aggregator   |\n| Unit test result fetcher (Formerly: Unit test result reporting)        | scripts/start_job.py            | unit-test-result-fetcher      |\n| Branch comparator (Formerly: Downstream branchdiff reporting)          | scripts/start_job.py            | branch-comparator             |\n| Review sheet backport updater                                          | scripts/start_job.py | review-sheet-backport-updater |\n| Reviewsync                                                             | scripts/start_job.py | reviewsync                    |\n\n# Use-cases\n\n\n### Examples for YARN backporter\nTo backport YARN-6221 to 2 branches, run these commands:\n```\nyarn-backport YARN-6221 COMPX-6664 cdpd-master\nyarn-backport YARN-6221 COMPX-6664 CDH-7.1-maint --no-fetch\n```\nThe first argument is the upstream Jira ID<br>\nThe second argument is the downstream Jira ID.<br>\nThe third argument is the downstream branch.<br>\nThe `--no-fetch` option is a means to skip git fetch on both repos.\n\n### How to backport to an already existing relation chain?\n1. Go to Gerrit UI and download the patch.\nFor example: \n```\ngit fetch "https://gerrit.sjc.cloudera.com/cdh/hadoop" refs/changes/29/156429/5 && git checkout FETCH_HEAD\n```\n2. Checkout a new branch\n```\ngit checkout -b my-relation-chain \n```\n\n3. Run backporter with: \n```\nyarn-backport YARN-10314 COMPX-7855 CDH-7.1.7.1000 --no-fetch --downstream_base_ref my-relation-chain\n```\nwhere:<br>\nThe first argument is the upstream Jira ID<br>\nThe second argument is the downstream Jira ID.<br>\nThe third argument is the downstream branch.<br>\nThe `--no-fetch` option is a means to skip git fetch on both repos.<br>\nThe `--downstream_base_ref <local-branch` is a way to use a local branch to base the backport on so the Git remote name won\'t be prepended.\n\n\nFinally, I set up two aliases for pushing the changes to the downstream repo:\n```\nalias git-push-to-cdpdmaster="git push <REMOTE> HEAD:refs/for/cdpd-master%<REVIEWER_LIST>"\nalias git-push-to-cdh71maint="git push <REMOTE> HEAD:refs/for/CDH-7.1-maint%<REVIEWER_LIST>"\n```\nwhere REVIEWER_LIST is in this format: "r=user1,r=user2,r=user3,..."\n\n\n# Contributing\n\n## Setup of pre-commit\n\nConfigure precommit as described in [this blogpost](https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/).\n\nCommands:\n1. Install precommit: `pip install pre-commit`\n2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: \n   `$HOME/Library/Python/3.8/bin/pre-commit`.\n2. Execute `pre-commit install` to install git hooks in your `.git/` directory.\n\n## Running the tests\n\nTODO\n\n## Troubleshooting\n\n### Installation issues\nIn case you\'re facing a similar issue:\n```\nAn error has occurred: InvalidManifestError: \n=====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist\nCheck the log at /<userhome>/.cache/pre-commit/pre-commit.log\n```\n, please run: `pre-commit autoupdate`\n\nMore info can be found [here](https://github.com/pre-commit/pre-commit/issues/577).',
     'author': 'Szilard Nemeth',
     'author_email': 'szilard.nemeth88@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/szilard-nemeth/yarn-dev-tools',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8.12,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `yarn-dev-tools-1.1.9/PKG-INFO` & `yarn-dev-tools-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: yarn-dev-tools
-Version: 1.1.9
+Version: 2.0.0
 Summary: 
 Home-page: https://github.com/szilard-nemeth/yarn-dev-tools
 Keywords: YARN,development,dev environment
 Author: Szilard Nemeth
 Author-email: szilard.nemeth88@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bs4
 Requires-Dist: dacite
 Requires-Dist: dataclasses-json
 Requires-Dist: gitpython
-Requires-Dist: google-api-wrapper2 (==1.0.4)
+Requires-Dist: google-api-wrapper2 (==1.0.5)
 Requires-Dist: humanize
 Requires-Dist: jira
-Requires-Dist: python-common-lib (==1.0.4)
+Requires-Dist: marshmallow
+Requires-Dist: pymongo
+Requires-Dist: python-common-lib (==1.0.6)
 Project-URL: Repository, https://github.com/szilard-nemeth/yarn-dev-tools
 Description-Content-Type: text/markdown
 
 [![CI for YARN dev tools (pip)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools/branch/master/graph/badge.svg?token=OQD6FIFF7I)](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![GitHub language count](https://img.shields.io/github/languages/count/szilard-nemeth/yarn-dev-tools)
@@ -56,44 +57,43 @@
 
 TODO
 
 # Getting started
 
 In order to use this tool, you need to have at least Python 3.8 installed.
 
-## Use yarn-dev-tools from package (recommended)
+## Use yarn-dev-tools from package (Recommended)
 If you don't want to tinker with the source code, you can download [yarn-dev-tools](https://pypi.org/project/yarn-dev-tools/#history) from PyPi as well.
 This is probably the easiest way to use it.
-
-
-Please check the [initial_setup.sh](initial_setup.sh) script.
-It has a `setup-vars` function at the beginning that define some environment variables:
+You don't need to install anything manually as I created a [script](initial_setup.sh) that performs the installation automatically.
+The script has a `setup-vars` function at the beginning that defines some environment variables:
 
 These are the following:
-- `YARNDEVTOOLS_ROOT`: specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.
-- `HADOOP_DEV_DIR` should be set to the upstream Hadoop repository root, e.g.: "/Users/snemeth/development/apache/hadoop/"
-- `CLOUDERA_HADOOP_ROOT` should be set to the downstream Hadoop repository root, e.g.: "/Users/snemeth/development/cloudera/hadoop/"
+- `YARNDEVTOOLS_ROOT`: Specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.
+- `HADOOP_DEV_DIR` Should be set to the upstream Hadoop repository root, e.g.: "~/development/apache/hadoop/"
+- `CLOUDERA_HADOOP_ROOT` Should be set to the downstream Hadoop repository root, e.g.: "~/development/cloudera/hadoop/"
 
-The latter 2 environment variables is better to be added to your bashrc file to keep them between the shells.
+The latter two environment variables is better to be added to your bashrc / zshrc file (depending on what shell you are using) to keep them between the shells.
 
 ## Use yarn-dev-tools from source
 If you want to use yarn-dev-tools from source, first you need to install its dependencies.
 The project root contains a pyproject.toml file that has all the dependencies listed.
 The project uses Poetry to resolve the dependencies so you need to [install poetry](https://python-poetry.org/docs/#installation) as well.
 Simply go to the root of this project and execute `poetry install --without localdev`.
 Alternatively, you can run `make` from the root of the project.
 
 ## Setting up handy aliases to use yarn-dev-tools
 If you completed the installation (either by source or by package), you may want to define some shell aliases to use the tool more easily.
+In my system, I have [these](
+https://github.com/szilard-nemeth/linux-env/blob/master/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).
+Please make sure to source this script so that the command 'yarndevtools' will be available since it's defined as a function.
+It is important to specify `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` as mentioned above, before sourcing the script.
 
+After these steps, you will have a basic set of aliases that is enough to get you started.
 
-So, you are ready to set up some aliases. 
-In my system, I have [these aliases](
-https://github.com/szilard-nemeth/linux-env/blob/94748d92ef32689805e89724948dd024a9936d59/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).
-If you run this script (with `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` specified as mentioned above), you will have a basic set of aliases that is enough to get you started.
 
 # Setting up yarn-dev-tools with Cloudera CDSW
 
 ## Initial setup
 1. Upload the initial setup scripts to the CDSW files, to the root directory (/home/cdsw)
 - [initial-cdsw-setup.sh](yarndevtools/cdsw/scripts/initial-cdsw-setup.sh)
 - [install-requirements.sh](yarndevtools/cdsw/scripts/install-requirements.sh)
@@ -177,15 +177,16 @@
 where REVIEWER_LIST is in this format: "r=user1,r=user2,r=user3,..."
 
 
 # Contributing
 
 ## Setup of pre-commit
 
-Configure precommit as described in this blogpost: https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/
+Configure precommit as described in [this blogpost](https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/).
+
 Commands:
 1. Install precommit: `pip install pre-commit`
 2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: 
    `$HOME/Library/Python/3.8/bin/pre-commit`.
 2. Execute `pre-commit install` to install git hooks in your `.git/` directory.
 
 ## Running the tests
@@ -198,8 +199,9 @@
 In case you're facing a similar issue:
 ```
 An error has occurred: InvalidManifestError: 
 =====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist
 Check the log at /<userhome>/.cache/pre-commit/pre-commit.log
 ```
 , please run: `pre-commit autoupdate`
-More info here: https://github.com/pre-commit/pre-commit/issues/577
+
+More info can be found [here](https://github.com/pre-commit/pre-commit/issues/577).
```

