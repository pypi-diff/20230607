# Comparing `tmp/pytask-0.3.1.tar.gz` & `tmp/pytask-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytask-0.3.1.tar", last modified: Tue Jan 24 23:49:19 2023, max compression
+gzip compressed data, was "pytask-0.3.2.tar", last modified: Wed Jun  7 09:40:51 2023, max compression
```

## Comparing `pytask-0.3.1.tar` & `pytask-0.3.2.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.744739 pytask-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.736739 pytask-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.736739 pytask-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.736739 pytask-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-24 23:49:09.000000 pytask-0.3.1/.github/workflows/update-plugin-list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-24 23:49:09.000000 pytask-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-24 23:49:09.000000 pytask-0.3.1/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-01-24 23:49:09.000000 pytask-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-24 23:49:09.000000 pytask-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-01-24 23:49:19.744739 pytask-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-01-24 23:49:09.000000 pytask-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-01-24 23:49:09.000000 pytask-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-24 23:49:19.744739 pytask-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.736739 pytask-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.744739 pytask-0.3.1/src/_pytask/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-24 23:49:19.000000 pytask-0.3.1/src/_pytask/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    23609 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/click.py
--rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/collect_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/collect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.744739 pytask-0.3.1/src/_pytask/mark/
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/mark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/mark/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/mark/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/mark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/outcomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/parametrize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/parametrize_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/persist.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/resolve_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/skipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/task_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/traceback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-01-24 23:49:09.000000 pytask-0.3.1/src/_pytask/warnings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.744739 pytask-0.3.1/src/pytask/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-01-24 23:49:09.000000 pytask-0.3.1/src/pytask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-24 23:49:09.000000 pytask-0.3.1/src/pytask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:09.000000 pytask-0.3.1/src/pytask/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 23:49:19.744739 pytask-0.3.1/src/pytask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-24 23:49:19.000000 pytask-0.3.1/src/pytask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.422561 pytask-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.414561 pytask-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.414561 pytask-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.414561 pytask-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 09:40:42.000000 pytask-0.3.2/.github/workflows/update-plugin-list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-07 09:40:42.000000 pytask-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-07 09:40:42.000000 pytask-0.3.2/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-07 09:40:42.000000 pytask-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-07 09:40:42.000000 pytask-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-06-07 09:40:51.422561 pytask-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-07 09:40:42.000000 pytask-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-07 09:40:42.000000 pytask-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-07 09:40:51.422561 pytask-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.414561 pytask-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.422561 pytask-0.3.2/src/_pytask/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 09:40:51.000000 pytask-0.3.2/src/_pytask/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23617 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/collect_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/collect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.422561 pytask-0.3.2/src/_pytask/mark/
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/mark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/mark/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/mark/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/mark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/parametrize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/parametrize_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/skipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/task_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/traceback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-07 09:40:42.000000 pytask-0.3.2/src/_pytask/warnings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.422561 pytask-0.3.2/src/pytask/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-07 09:40:42.000000 pytask-0.3.2/src/pytask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 09:40:42.000000 pytask-0.3.2/src/pytask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:42.000000 pytask-0.3.2/src/pytask/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:40:51.422561 pytask-0.3.2/src/pytask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 09:40:51.000000 pytask-0.3.2/src/pytask.egg-info/top_level.txt
```

### Comparing `pytask-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `pytask-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/.github/ISSUE_TEMPLATE/documentation.md` & `pytask-0.3.2/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/.github/ISSUE_TEMPLATE/enhancement.md` & `pytask-0.3.2/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/.github/workflows/main.yml` & `pytask-0.3.2/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     strategy:
       fail-fast: false
       matrix:
         os: ['ubuntu-latest', 'macos-latest', 'windows-latest']
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - uses: conda-incubator/setup-miniconda@v2.2.0
         with:
           auto-update-conda: false
           python-version: ${{ matrix.python-version }}
           channels: conda-forge,nodefaults
           miniforge-variant: Mambaforge
```

### Comparing `pytask-0.3.1/.github/workflows/publish-to-pypi.yml` & `pytask-0.3.2/.github/workflows/publish-to-pypi.yml`

 * *Files 21% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 on: push
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@master
+    - uses: actions/checkout@v3
 
     - name: Set up Python 3.8
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install pypa/build
       run: >-
         python -m
         pip install
```

### Comparing `pytask-0.3.1/.github/workflows/update-plugin-list.yml` & `pytask-0.3.2/.github/workflows/update-plugin-list.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,33 @@
     runs-on: ubuntu-latest
     permissions:
       contents: write
       pull-requests: write
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install packaging requests tabulate[widechars] tqdm
 
       - name: Update Plugin List
         run: python scripts/update_plugin_list.py
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@2455e1596942c2902952003bbb574afbbe2ab2e6
+        uses: peter-evans/create-pull-request@284f54f989303d2699d373481a0cfa13ad5a6666
         with:
           commit-message: '[automated] Update plugin list'
           author: 'Tobias Raabe <tobiasraabe@users.noreply.github.com>'
           branch: update-plugin-list/patch
           delete-branch: true
           branch-suffix: short-commit-hash
           title: '[automated] Update plugin list'
```

### Comparing `pytask-0.3.1/LICENSE` & `pytask-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/PKG-INFO` & `pytask-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytask
-Version: 0.3.1
+Version: 0.3.2
 Summary: In its highest aspirations, pytask tries to be pytest as a build system.
 Home-page: https://pytask-dev.readthedocs.io/en/stable
 Author: Tobias Raabe
 Author-email: raabe@posteo.de
 License: MIT
 Project-URL: Changelog, https://pytask-dev.readthedocs.io/en/stable/changes.html
 Project-URL: Documentation, https://pytask-dev.readthedocs.io/en/stable
```

### Comparing `pytask-0.3.1/README.md` & `pytask-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/pyproject.toml` & `pytask-0.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 
 [tool.ruff]
 target-version = "py37"
 select = ["ALL"]
 fix = true
 extend-ignore = [
+    "TRY",  # ignore tryceratops.
+    "TCH",  # ignore non-guarded type imports.
     # Numpy docstyle
     "D107",
     "D203",
     "D212",
     "D213",
     "D402",
     "D413",
@@ -53,14 +55,17 @@
     "ANN102",  # type annotating cls
     "FBT",  # flake8-boolean-trap
     "EM",  # flake8-errmsg
     "ANN401",  # flake8-annotate typing.Any
     "PD",  # pandas-vet
     "COM812",  # trailing comma missing, but black takes care of that
     "D401",  # imperative mood for first line. too many false-positives.
+    "SLF001",  # access private members.
+    "S603",
+    "S607",
 ]
 
 
 [tool.ruff.per-file-ignores]
 "src/_pytask/capture.py" = ["PGH003"]
 "src/_pytask/hookspecs.py" = ["ARG001"]
 "src/_pytask/outcomes.py" = ["N818"]
@@ -68,7 +73,18 @@
 "tests/*" = ["D", "ANN", "PLR2004"]
 "scripts/*" = ["D", "INP001"]
 "docs/source/conf.py" = ["D401", "INP001"]
 
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
+
+
+[tool.pytest.ini_options]
+testpaths = ["src", "tests"]
+markers = [
+    "wip: Tests that are work-in-progress.",
+    "unit: Flag for unit tests which target mainly a single function.",
+    "integration: Flag for integration tests which may comprise of multiple unit tests.",
+    "end_to_end: Flag for tests that cover the whole program.",
+]
+norecursedirs = [".idea", ".tox"]
```

### Comparing `pytask-0.3.1/setup.cfg` & `pytask-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = In its highest aspirations, pytask tries to be pytest as a build system.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pytask-dev.readthedocs.io/en/stable
 author = Tobias Raabe
 author_email = raabe@posteo.de
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS :: MacOS X
```

### Comparing `pytask-0.3.1/src/_pytask/build.py` & `pytask-0.3.2/src/_pytask/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 @hookimpl(tryfirst=True)
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Extend the command line interface."""
     cli.add_command(build)
 
 
-def main(raw_config: dict[str, Any]) -> Session:  # noqa: C901
+def main(raw_config: dict[str, Any]) -> Session:  # noqa: C901, PLR0912, PLR0915
     """Run pytask.
 
     This is the main command to run pytask which usually receives kwargs from the
     command line interface. It can also be used to run pytask interactively. Pass
     configuration in a dictionary.
 
     Parameters
@@ -109,22 +109,22 @@
         session = Session({}, None)
         session.exit_code = ExitCode.CONFIGURATION_FAILED
 
     else:
         try:
             session.hook.pytask_log_session_header(session=session)
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_resolve_dependencies(session=session)
+            session.hook.pytask_dag(session=session)
             session.hook.pytask_execute(session=session)
 
         except CollectionError:
             session.exit_code = ExitCode.COLLECTION_FAILED
 
         except ResolvingDependenciesError:
-            session.exit_code = ExitCode.RESOLVING_DEPENDENCIES_FAILED
+            session.exit_code = ExitCode.DAG_FAILED
 
         except ExecutionError:
             session.exit_code = ExitCode.FAILED
 
         except Exception:  # noqa: BLE001
             exc_info = sys.exc_info()
             exc_info = remove_internal_traceback_frames_from_exc_info(exc_info)
@@ -168,17 +168,24 @@
     type=bool,
     default=True,
     help=("Choose whether tracebacks should be displayed or not."),
 )
 @click.option(
     "--dry-run", type=bool, is_flag=True, default=False, help="Perform a dry-run."
 )
+@click.option(
+    "-f",
+    "--force",
+    is_flag=True,
+    default=False,
+    help="Execute a task even if it succeeded successfully before.",
+)
 def build(**raw_config: Any) -> NoReturn:
     """Collect tasks, execute them and report the results.
 
-    This is pytask's default command. pytask collects tasks from the given paths or the
+    The default command. pytask collects tasks from the given paths or the
     current working directory, executes them and reports the results.
 
     """
     raw_config["command"] = "build"
     session = main(raw_config)
     sys.exit(session.exit_code)
```

### Comparing `pytask-0.3.1/src/_pytask/capture.py` & `pytask-0.3.2/src/_pytask/capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
             self.targetfd_invalid: int | None = os.open(os.devnull, os.O_RDWR)
             os.dup2(self.targetfd_invalid, targetfd)
         else:
             self.targetfd_invalid = None
         self.targetfd_save = os.dup(targetfd)
 
         if targetfd == 0:
-            self.tmpfile = open(os.devnull, encoding="utf-8")  # noqa: SIM115
+            self.tmpfile = open(os.devnull, encoding="utf-8")  # noqa: SIM115, PTH123
             self.syscapture = SysCapture(targetfd)
         else:
             self.tmpfile = EncodedFile(
                 TemporaryFile(buffering=0),
                 encoding="utf-8",
                 errors="replace",
                 newline="",
```

### Comparing `pytask-0.3.1/src/_pytask/clean.py` & `pytask-0.3.2/src/_pytask/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 @click.option(
     "-q",
     "--quiet",
     is_flag=True,
     help="Do not print the names of the removed paths.",
     default=False,
 )
-def clean(**raw_config: Any) -> NoReturn:  # noqa: C901
+def clean(**raw_config: Any) -> NoReturn:  # noqa: C901, PLR0912, PLR0915
     """Clean the provided paths by removing files unknown to pytask."""
     raw_config["command"] = "clean"
 
     try:
         # Duplication of the same mechanism in :func:`pytask.main.main`.
         pm = get_plugin_manager()
         from _pytask import cli
```

### Comparing `pytask-0.3.1/src/_pytask/cli.py` & `pytask-0.3.2/src/_pytask/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return pm
 
 
 def _sort_options_for_each_command_alphabetically(cli: click.Group) -> None:
     """Sort command line options and arguments for each command alphabetically."""
     for command in cli.commands:
         cli.commands[command].params = sorted(
-            cli.commands[command].params, key=lambda x: x.name
+            cli.commands[command].params, key=lambda x: x.opts[0].replace("-", "")
         )
 
 
 @hookimpl
 def pytask_add_hooks(pm: pluggy.PluginManager) -> None:
     """Add hooks."""
     from _pytask import build
@@ -60,19 +60,20 @@
     from _pytask import database
     from _pytask import debugging
     from _pytask import execute
     from _pytask import graph
     from _pytask import live
     from _pytask import logging
     from _pytask import mark
+    from _pytask import nodes
     from _pytask import parameters
     from _pytask import parametrize
     from _pytask import persist
     from _pytask import profile
-    from _pytask import resolve_dependencies
+    from _pytask import dag
     from _pytask import skipping
     from _pytask import task
     from _pytask import warnings
 
     pm.register(build)
     pm.register(capture)
     pm.register(clean)
@@ -82,19 +83,20 @@
     pm.register(database)
     pm.register(debugging)
     pm.register(execute)
     pm.register(graph)
     pm.register(live)
     pm.register(logging)
     pm.register(mark)
+    pm.register(nodes)
     pm.register(parameters)
     pm.register(parametrize)
     pm.register(persist)
     pm.register(profile)
-    pm.register(resolve_dependencies)
+    pm.register(dag)
     pm.register(skipping)
     pm.register(task)
     pm.register(warnings)
 
 
 @click.group(
     cls=ColoredGroup,
```

### Comparing `pytask-0.3.1/src/_pytask/click.py` & `pytask-0.3.2/src/_pytask/click.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 ) -> None:
     """Print options formatted with a table in a panel."""
     highlighter = _OptionHighlighter()
 
     options_table = Table(highlight=True, box=None, show_header=False)
 
     for param in group_or_command.get_params(ctx):
-
         if isinstance(param, click.Argument):
             continue
 
         if getattr(param, "hidden", False):
             continue
 
         # The ordering of -h and --help is not fixed.
@@ -159,21 +158,20 @@
             opt2 = highlighter("--help")
         elif len(param.opts) == 2:  # noqa: PLR2004
             opt1 = highlighter(param.opts[0])
             opt2 = highlighter(param.opts[1])
         elif len(param.opts) == 1 == len(param.secondary_opts):
             opt1 = Text("")
             opt2 = highlighter(param.opts[0] + "/" + param.secondary_opts[0])
+        elif "--" in param.opts[0]:
+            opt1 = Text("")
+            opt2 = highlighter(param.opts[0])
         else:
-            if "--" in param.opts[0]:
-                opt1 = Text("")
-                opt2 = highlighter(param.opts[0])
-            else:
-                opt1 = highlighter(param.opts[0])
-                opt2 = Text("")
+            opt1 = highlighter(param.opts[0])
+            opt2 = Text("")
 
         if param.metavar:
             opt2 += Text(f" {param.metavar}", style="metavar")
         elif isinstance(param.type, click.Choice):
             choices = "[" + "|".join(param.type.choices) + "]"
             opt2 += Text(f" {choices}", style="metavar", overflow="fold")
 
@@ -187,15 +185,17 @@
             title="[bold #f2f2f2]Options[/]",
             title_align="left",
             border_style="grey37",
         )
     )
 
 
-def _format_help_text(param: click.Parameter, ctx: click.Context) -> str:  # noqa: C901
+def _format_help_text(  # noqa: C901, PLR0912, PLR0915
+    param: click.Parameter, ctx: click.Context
+) -> str:
     """Format the help of a click parameter.
 
     A large chunk of the function is copied from
     :meth:`click.core.Option.get_help_record` to support styling, show values of enums,
     etc..
 
     """
```

### Comparing `pytask-0.3.1/src/_pytask/collect.py` & `pytask-0.3.2/src/_pytask/collect.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import inspect
 import itertools
 import os
 import sys
 import time
-from importlib import util as importlib_util
+import warnings
 from pathlib import Path
 from typing import Any
 from typing import Generator
 from typing import Iterable
 
 from _pytask.collect_utils import depends_on
 from _pytask.collect_utils import parse_nodes
@@ -23,14 +23,15 @@
 from _pytask.exceptions import CollectionError
 from _pytask.mark_utils import has_mark
 from _pytask.nodes import FilePathNode
 from _pytask.nodes import Task
 from _pytask.outcomes import CollectionOutcome
 from _pytask.outcomes import count_outcomes
 from _pytask.path import find_case_sensitive_path
+from _pytask.path import import_path
 from _pytask.report import CollectionReport
 from _pytask.session import Session
 from _pytask.shared import find_duplicates
 from _pytask.shared import reduce_node_name
 from _pytask.traceback import render_exc_info
 from rich.text import Text
 
@@ -101,35 +102,45 @@
         ]
 
     session.hook.pytask_collect_file_log(session=session, reports=flat_reports)
 
     return flat_reports
 
 
+_PARAMETRIZE_DEPRECATION_WARNING = """\
+The @pytask.mark.parametrize decorator is deprecated and will be removed in pytask \
+v0.4. Either upgrade your code to the new syntax explained in \
+https://tinyurl.com/pytask-loops or silence the warning by setting \
+`silence_parametrize_deprecation = true` in your pyproject.toml under \
+[tool.pytask.ini_options] and pin pytask to <0.4.
+"""
+
+
 @hookimpl
 def pytask_collect_file(
     session: Session, path: Path, reports: list[CollectionReport]
 ) -> list[CollectionReport] | None:
     """Collect a file."""
     if any(path.match(pattern) for pattern in session.config["task_files"]):
-        spec = importlib_util.spec_from_file_location(path.stem, str(path))
-
-        if spec is None:
-            raise ImportError(f"Can't find module {path.stem!r} at location {path}.")
-
-        mod = importlib_util.module_from_spec(spec)
-        spec.loader.exec_module(mod)
+        mod = import_path(path, session.config["root"])
 
         collected_reports = []
         for name, obj in inspect.getmembers(mod):
             # Ensures that tasks with this decorator are only collected once.
             if has_mark(obj, "task"):
                 continue
 
             if has_mark(obj, "parametrize"):
+                if not session.config.get("silence_parametrize_deprecation", False):
+                    warnings.warn(
+                        message=_PARAMETRIZE_DEPRECATION_WARNING,
+                        category=FutureWarning,
+                        stacklevel=1,
+                    )
+
                 names_and_objects = session.hook.pytask_parametrize_task(
                     session=session, name=name, obj=obj
                 )
             else:
                 names_and_objects = [(name, obj)]
 
             for name_, obj_ in names_and_objects:
```

### Comparing `pytask-0.3.1/src/_pytask/collect_command.py` & `pytask-0.3.2/src/_pytask/collect_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         session.exit_code = ExitCode.CONFIGURATION_FAILED
         console.print_exception()
 
     else:
         try:
             session.hook.pytask_log_session_header(session=session)
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_resolve_dependencies(session=session)
+            session.hook.pytask_dag(session=session)
 
             tasks = _select_tasks_by_expressions_and_marker(session)
 
             common_ancestor = _find_common_ancestor_of_all_nodes(
                 tasks, session.config["paths"], session.config["nodes"]
             )
             dictionary = _organize_tasks(tasks)
@@ -91,15 +91,15 @@
             console.print()
             console.rule(style="neutral")
 
         except CollectionError:
             session.exit_code = ExitCode.COLLECTION_FAILED
 
         except ResolvingDependenciesError:
-            session.exit_code = ExitCode.RESOLVING_DEPENDENCIES_FAILED
+            session.exit_code = ExitCode.DAG_FAILED
 
         except Exception:  # noqa: BLE001
             session.exit_code = ExitCode.FAILED
             console.print_exception()
             console.rule(style="failed")
 
     sys.exit(session.exit_code)
```

### Comparing `pytask-0.3.1/src/_pytask/collect_utils.py` & `pytask-0.3.2/src/_pytask/collect_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def depends_on(
     objects: Any | Iterable[Any] | dict[Any, Any]
 ) -> Any | Iterable[Any] | dict[Any, Any]:
     """Specify dependencies for a task.
 
     Parameters
     ----------
-    objects : Any | Iterable[Any] | dict[Any, Any]
+    objects
         Can be any valid Python object or an iterable of any Python objects. To be
         valid, it must be parsed by some hook implementation for the
         :func:`_pytask.hookspecs.pytask_collect_node` entry-point.
 
     """
     return objects
 
@@ -45,15 +45,15 @@
 def produces(
     objects: Any | Iterable[Any] | dict[Any, Any]
 ) -> Any | Iterable[Any] | dict[Any, Any]:
     """Specify products of a task.
 
     Parameters
     ----------
-    objects : Any | Iterable[Any] | dict[Any, Any]
+    objects
         Can be any valid Python object or an iterable of any Python objects. To be
         valid, it must be parsed by some hook implementation for the
         :func:`_pytask.hookspecs.pytask_collect_node` entry-point.
 
     """
     return objects
 
@@ -197,27 +197,26 @@
 def _collect_node(
     session: Session, path: Path, name: str, node: str | Path
 ) -> dict[str, MetaNode]:
     """Collect nodes for a task.
 
     Parameters
     ----------
-    session : _pytask.session.Session
+    session
         The session.
-    path : Path
+    path
         The path to the task whose nodes are collected.
-    name : str
+    name
         The name of the task.
-    nodes : Dict[str, Union[str, Path]]
+    nodes
         A dictionary of nodes parsed from the ``depends_on`` or ``produces`` markers.
 
     Returns
     -------
-    Dict[str, MetaNode]
-        A dictionary of node names and their paths.
+    A dictionary of node names and their paths.
 
     Raises
     ------
     NodeNotCollectedError
         If the node could not collected.
 
     """
```

### Comparing `pytask-0.3.1/src/_pytask/compat.py` & `pytask-0.3.2/src/_pytask/compat.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,50 +26,50 @@
     """Get version from a package."""
     version = getattr(module, "__version__", None)
     if version is None:
         raise ImportError(f"Can't determine version for {module.__name__}")
     return version
 
 
-def import_optional_dependency(  # noqa: C901
+def import_optional_dependency(
     name: str,
     extra: str = "",
     errors: str = "raise",
     min_version: str | None = None,
     caller: str = "pytask",
 ) -> types.ModuleType | None:
     """Import an optional dependency.
 
     By default, if a dependency is missing an ImportError with a nice message will be
     raised. If a dependency is present, but too old, we raise.
 
     Parameters
     ----------
-    name : str
+    name
         The module name.
-    extra : str
+    extra
         Additional text to include in the ImportError message.
-    errors : str {'raise', 'warn', 'ignore'}
+    errors
         What to do when a dependency is not found or its version is too old.
 
         * raise : Raise an ImportError
         * warn : Only applicable when a module's version is to old. Warns that the
           version is too old and returns None
         * ignore: If the module is not installed, return None, otherwise, return the
           module, even if the version is too old. It's expected that users validate the
           version locally when using ``errors="ignore"`` (see. ``io/html.py``)
-    min_version : str, default None
+    min_version
         Specify a minimum version that is different from the global pandas minimum
         version required.
-    caller : str, default "pytask"
+    caller
         The caller of the function.
 
     Returns
     -------
-    maybe_module : Optional[ModuleType]
+    types.ModuleType | None
         The imported module, when found and the version is correct. None is returned
         when the package is not found and `errors` is False, or when the package's
         version is too old and `errors` is ``'warn'``.
 
     """
     if errors not in ("warn", "raise", "ignore"):  # pragma: no cover
         raise ValueError("'errors' must be one of 'warn', 'raise' or 'ignore'.")
@@ -104,15 +104,15 @@
         version = _get_version(module_to_get)
         if parse_version(version) < parse_version(minimum_version):
             msg = (
                 f"{caller} requires version {minimum_version!r} or newer of "
                 f"{parent!r} (version {version!r} currently installed)."
             )
             if errors == "warn":
-                warnings.warn(msg, UserWarning)
+                warnings.warn(msg, UserWarning, stacklevel=2)
                 return None
             if errors == "raise":
                 raise ImportError(msg)
 
     return module
 
 
@@ -132,10 +132,10 @@
 
     program_exists = shutil.which(name) is not None
 
     if not program_exists:
         if errors == "raise":
             raise RuntimeError(msg)
         if errors == "warn":
-            warnings.warn(msg, UserWarning)
+            warnings.warn(msg, UserWarning, stacklevel=2)
 
     return program_exists
```

### Comparing `pytask-0.3.1/src/_pytask/config.py` & `pytask-0.3.2/src/_pytask/config.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/config_utils.py` & `pytask-0.3.2/src/_pytask/config_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         context.default_map = {}
     context.default_map.update(config_from_file)
     context.params.update(config_from_file)
 
     return context.params["config"]
 
 
-def _find_project_root_and_config(paths: list[Path]) -> tuple[Path, Path]:  # noqa: C901
+def _find_project_root_and_config(paths: list[Path]) -> tuple[Path, Path]:
     """Find the project root and configuration file from a list of paths.
 
     The process is as follows:
 
     1. Find the common base directory of all paths passed to pytask (default to the
        current working directory).
     2. Starting from this directory, look at all parent directories, and return the file
```

### Comparing `pytask-0.3.1/src/_pytask/console.py` & `pytask-0.3.2/src/_pytask/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         "option": "bold #F4C041",
         "switch": "bold #D54523",
         "metavar": "bold #FFFF00",
     }
 )
 
 
-console = Console(theme=theme, color_system=_COLOR_SYSTEM)
+console: Console = Console(theme=theme, color_system=_COLOR_SYSTEM)
 
 
 def render_to_string(
     text: str | Text,
     *,
     console: Console | None = None,
     strip_styles: bool = False,
```

### Comparing `pytask-0.3.1/src/_pytask/dag.py` & `pytask-0.3.2/src/_pytask/dag_utils.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/database.py` & `pytask-0.3.2/src/_pytask/database.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/debugging.py` & `pytask-0.3.2/src/_pytask/debugging.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
                 # Handle --pdbcls=pdb:pdb.Pdb (useful e.g. with pdbpp).
                 parts = classname.split(".")
                 pdb_cls = getattr(mod, parts[0])
                 for part in parts[1:]:
                     pdb_cls = getattr(pdb_cls, part)
             except Exception as exc:  # noqa: BLE001
-                value = ":".join((modname, classname))
+                value = f"{modname}:{classname}"
                 raise ValueError(
                     f"--pdbcls: could not import {value!r}: {exc}."
                 ) from exc
         else:
             import pdb  # noqa: T100
 
             pdb_cls = pdb.Pdb
@@ -165,14 +165,15 @@
         return wrapped_cls
 
     @classmethod
     def _get_pdb_wrapper_class(  # noqa: C901
         cls, pdb_cls: type[pdb.Pdb], capman: CaptureManager, live_manager: LiveManager
     ) -> type[pdb.Pdb]:
         """Create a pdf wrapper class."""
+
         # Type ignored because mypy doesn't support "dynamic"
         # inheritance like this.
         class PytaskPdbWrapper(pdb_cls):  # type: ignore[valid-type,misc]
             _pytask_capman = capman
             _pytask_live_manager = live_manager
             _continued = False
```

### Comparing `pytask-0.3.1/src/_pytask/exceptions.py` & `pytask-0.3.2/src/_pytask/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/execute.py` & `pytask-0.3.2/src/_pytask/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from _pytask.config import hookimpl
 from _pytask.console import console
 from _pytask.console import create_summary_panel
 from _pytask.console import create_url_style_for_task
 from _pytask.console import format_strings_as_flat_tree
 from _pytask.console import format_task_id
 from _pytask.console import unify_styles
-from _pytask.dag import descending_tasks
-from _pytask.dag import TopologicalSorter
+from _pytask.dag_utils import descending_tasks
+from _pytask.dag_utils import TopologicalSorter
 from _pytask.database_utils import update_states_in_database
 from _pytask.enums import ShowCapture
 from _pytask.exceptions import ExecutionError
 from _pytask.exceptions import NodeNotFoundError
 from _pytask.mark import Mark
 from _pytask.mark_utils import has_mark
 from _pytask.nodes import FilePathNode
@@ -117,19 +117,17 @@
 
     1. Check whether all dependencies of a task are available.
     2. Create the directory where the product will be placed.
 
     """
     for dependency in session.dag.predecessors(task.name):
         node = session.dag.nodes[dependency]["node"]
-        try:
-            node.state()
-        except NodeNotFoundError as e:
+        if not node.state():
             msg = f"{node.name} is missing and required for {task.name}."
-            raise NodeNotFoundError(msg) from e
+            raise NodeNotFoundError(msg)
 
     # Create directory for product if it does not exist. Maybe this should be a `setup`
     # method for the node classes.
     for product in session.dag.successors(task.name):
         node = session.dag.nodes[product]["node"]
         if isinstance(node, FilePathNode):
             node.path.parent.mkdir(parents=True, exist_ok=True)
@@ -139,15 +137,15 @@
         raise WouldBeExecuted
 
 
 @hookimpl(trylast=True)
 def pytask_execute_task(session: Session, task: Task) -> bool:
     """Execute task."""
     if session.config["dry_run"]:
-        raise WouldBeExecuted()
+        raise WouldBeExecuted
 
     kwargs = {**task.kwargs}
 
     func_arg_names = set(inspect.signature(task.function).parameters)
     for arg_name in ("depends_on", "produces"):
         if arg_name in func_arg_names:
             attribute = getattr(task, arg_name)
@@ -159,20 +157,16 @@
 
 @hookimpl
 def pytask_execute_task_teardown(session: Session, task: Task) -> None:
     """Check if :class:`_pytask.nodes.FilePathNode` are produced by a task."""
     missing_nodes = []
     for product in session.dag.successors(task.name):
         node = session.dag.nodes[product]["node"]
-        if isinstance(node, FilePathNode):
-
-            try:
-                node.state()
-            except NodeNotFoundError:
-                missing_nodes.append(node)
+        if not node.state():
+            missing_nodes.append(node)
 
     if missing_nodes:
         paths = [reduce_node_name(i, session.config["paths"]) for i in missing_nodes]
         formatted = format_strings_as_flat_tree(
             paths, "The task did not produce the following files:\n", ""
         )
         raise NodeNotFoundError(formatted)
@@ -186,15 +180,15 @@
 
     If a task failed, skip all subsequent tasks. Else, update the states of related
     nodes in the database.
 
     """
     task = report.task
     if report.outcome == TaskOutcome.SUCCESS:
-        update_states_in_database(session.dag, task.name)
+        update_states_in_database(session, task.name)
     elif report.exc_info and isinstance(report.exc_info[1], WouldBeExecuted):
         report.outcome = TaskOutcome.WOULD_BE_EXECUTED
 
         for descending_task_name in descending_tasks(task.name, session.dag):
             descending_task = session.dag.nodes[descending_task_name]["task"]
             descending_task.markers.append(
                 Mark(
```

### Comparing `pytask-0.3.1/src/_pytask/git.py` & `pytask-0.3.2/src/_pytask/git.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/graph.py` & `pytask-0.3.2/src/_pytask/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,23 +106,23 @@
             import_optional_dependency("pygraphviz")
             check_for_optional_program(
                 session.config["layout"],
                 extra="The layout program is part of the graphviz package which you "
                 "can install with conda.",
             )
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_resolve_dependencies(session=session)
+            session.hook.pytask_dag(session=session)
             dag = _refine_dag(session)
             _write_graph(dag, session.config["output_path"], session.config["layout"])
 
         except CollectionError:
             session.exit_code = ExitCode.COLLECTION_FAILED
 
         except ResolvingDependenciesError:
-            session.exit_code = ExitCode.RESOLVING_DEPENDENCIES_FAILED
+            session.exit_code = ExitCode.DAG_FAILED
 
         except Exception:  # noqa: BLE001
             session.exit_code = ExitCode.FAILED
             exc_info = remove_internal_traceback_frames_from_exc_info(sys.exc_info())
             console.print()
             console.print(Traceback.from_exception(*exc_info))
             console.rule(style="failed")
@@ -210,15 +210,15 @@
             import_optional_dependency("pygraphviz")
             check_for_optional_program(
                 session.config["layout"],
                 extra="The layout program is part of the graphviz package that you "
                 "can install with conda.",
             )
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_resolve_dependencies(session=session)
+            session.hook.pytask_dag(session=session)
             dag = _refine_dag(session)
 
         except Exception:
             raise
 
         else:
             return dag
```

### Comparing `pytask-0.3.1/src/_pytask/hookspecs.py` & `pytask-0.3.2/src/_pytask/hookspecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 At each of the entry-points, a plugin can register a hook implementation which receives
 the message send by the host and may send a response.
 
 """
 from __future__ import annotations
 
-from pathlib import Path
+import pathlib
 from typing import Any
 from typing import Callable
 from typing import TYPE_CHECKING
 
 import click
-import networkx as nx
+import networkx
 import pluggy
 
 
 if TYPE_CHECKING:
     from _pytask.session import Session
     from _pytask.nodes import MetaNode
     from _pytask.nodes import Task
     from _pytask.outcomes import CollectionOutcome
     from _pytask.outcomes import TaskOutcome
     from _pytask.reports import CollectionReport
     from _pytask.reports import ExecutionReport
-    from _pytask.reports import ResolveDependencyReport
+    from _pytask.reports import DagReport
 
 
 hookspec = pluggy.HookspecMarker("pytask")
 
 
 @hookspec
 def pytask_add_hooks(pm: pluggy.PluginManager) -> None:
@@ -113,15 +113,15 @@
     The main hook implementation which controls the collection and calls subordinated
     hooks.
 
     """
 
 
 @hookspec(firstresult=True)
-def pytask_ignore_collect(path: Path, config: dict[str, Any]) -> bool:
+def pytask_ignore_collect(path: pathlib.Path, config: dict[str, Any]) -> bool:
     """Ignore collected path.
 
     This hook is indicates for each directory and file whether it should be ignored.
     This speeds up the collection.
 
     """
 
@@ -133,27 +133,27 @@
     This hook can be used to deselect tasks when they match a certain keyword or mark.
 
     """
 
 
 @hookspec(firstresult=True)
 def pytask_collect_file_protocol(
-    session: Session, path: Path, reports: list[CollectionReport]
+    session: Session, path: pathlib.Path, reports: list[CollectionReport]
 ) -> list[CollectionReport]:
     """Start protocol to collect files.
 
     The protocol calls the subordinate hook :func:`pytask_collect_file` which might
     error if the file has a :class:`SyntaxError`.
 
     """
 
 
 @hookspec
 def pytask_collect_file(
-    session: Session, path: Path, reports: list[CollectionReport]
+    session: Session, path: pathlib.Path, reports: list[CollectionReport]
 ) -> list[CollectionReport] | None:
     """Collect tasks from a file.
 
     If you want to collect tasks from other files, modify this hook.
 
     """
 
@@ -161,43 +161,45 @@
 @hookspec
 def pytask_collect_file_log(session: Session, reports: list[CollectionReport]) -> None:
     """Perform logging at the end of collecting a file."""
 
 
 @hookspec(firstresult=True)
 def pytask_collect_task_protocol(
-    session: Session, path: Path, name: str, obj: Any
+    session: Session, path: pathlib.Path, name: str, obj: Any
 ) -> CollectionReport | None:
     """Start protocol to collect tasks."""
 
 
 @hookspec
 def pytask_collect_task_setup(
-    session: Session, path: Path, name: str, obj: Any
+    session: Session, path: pathlib.Path, name: str, obj: Any
 ) -> None:
     """Steps before collecting a task."""
 
 
 @hookspec(firstresult=True)
-def pytask_collect_task(session: Session, path: Path, name: str, obj: Any) -> Task:
+def pytask_collect_task(
+    session: Session, path: pathlib.Path, name: str, obj: Any
+) -> Task:
     """Collect a single task."""
 
 
 @hookspec
 def pytask_collect_task_teardown(session: Session, task: Task) -> None:
     """Perform tear-down operations when a task was collected.
 
     Use this hook specification to, for example, perform checks on the collected task.
 
     """
 
 
 @hookspec(firstresult=True)
 def pytask_collect_node(
-    session: Session, path: Path, node: MetaNode
+    session: Session, path: pathlib.Path, node: MetaNode
 ) -> MetaNode | None:
     """Collect a node which is a dependency or a product of a task."""
 
 
 @hookspec(firstresult=True)
 def pytask_collect_log(
     session: Session, reports: list[CollectionReport], tasks: list[Task]
@@ -230,71 +232,77 @@
     """
 
 
 # Hooks for resolving dependencies.
 
 
 @hookspec(firstresult=True)
-def pytask_resolve_dependencies(session: Session) -> None:
-    """Resolve dependencies.
+def pytask_dag(session: Session) -> None:
+    """Create a DAG.
 
     The main hook implementation which controls the resolution of dependencies and calls
     subordinated hooks.
 
     """
 
 
 @hookspec(firstresult=True)
-def pytask_resolve_dependencies_create_dag(
-    session: Session, tasks: list[Task]
-) -> nx.DiGraph:
+def pytask_dag_create_dag(session: Session, tasks: list[Task]) -> networkx.DiGraph:
     """Create the DAG.
 
     This hook creates the DAG from tasks, dependencies and products. The DAG can be used
     by a scheduler to find an execution order.
 
     """
 
 
 @hookspec
-def pytask_resolve_dependencies_modify_dag(session: Session, dag: nx.DiGraph) -> None:
+def pytask_dag_modify_dag(session: Session, dag: networkx.DiGraph) -> None:
     """Modify the DAG.
 
     This hook allows to make some changes to the DAG before it is validated and tasks
     are selected.
 
     """
 
 
 @hookspec(firstresult=True)
-def pytask_resolve_dependencies_validate_dag(session: Session, dag: nx.DiGraph) -> None:
+def pytask_dag_validate_dag(session: Session, dag: networkx.DiGraph) -> None:
     """Validate the DAG.
 
     This hook validates the DAG. For example, there can be cycles in the DAG if tasks,
     dependencies and products have been misspecified.
 
     """
 
 
 @hookspec
-def pytask_resolve_dependencies_select_execution_dag(
-    session: Session, dag: nx.DiGraph
+def pytask_dag_select_execution_dag(session: Session, dag: networkx.DiGraph) -> None:
+    """Select the subgraph which needs to be executed.
+
+    This hook determines which of the tasks have to be re-run because something has
+    changed.
+
+    """
+
+
+@hookspec(firstresult=True)
+def pytask_dag_has_node_changed(
+    session: Session, dag: networkx.DiGraph, node: MetaNode, task_name: str
 ) -> None:
     """Select the subgraph which needs to be executed.
 
     This hook determines which of the tasks have to be re-run because something has
     changed.
 
     """
 
 
 @hookspec
-def pytask_resolve_dependencies_log(
-    session: Session, report: ResolveDependencyReport
-) -> None:
+def pytask_dag_log(session: Session, report: DagReport) -> None:
     """Log errors during resolving dependencies."""
 
 
 # Hooks for running tasks.
 
 
 @hookspec(firstresult=True)
```

### Comparing `pytask-0.3.1/src/_pytask/live.py` & `pytask-0.3.2/src/_pytask/live.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/logging.py` & `pytask-0.3.2/src/_pytask/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Parse configuration."""
     if config["editor_url_scheme"] not in ("no_link", "file") and IS_WINDOWS_TERMINAL:
         config["editor_url_scheme"] = "file"
         warnings.warn(
             "Windows Terminal does not support url schemes to applications, yet."
             "See https://github.com/pytask-dev/pytask/issues/171 for more information. "
-            "Resort to `editor_url_scheme='file'`."
+            "Resort to `editor_url_scheme='file'`.",
+            stacklevel=1,
         )
 
 
 @hookimpl
 def pytask_log_session_header(session: Session) -> None:
     """Log the header of a pytask session."""
     console.rule("Start pytask session", style=None)
@@ -123,15 +124,15 @@
             i for i in duration_tuples if i[1] not in ("second", "seconds")
         ]
 
     formatted_duration = ", ".join([" ".join(map(str, i)) for i in duration_tuples])
     return formatted_duration
 
 
-def _humanize_time(  # noqa: C901
+def _humanize_time(  # noqa: C901, PLR0912
     amount: int | float, unit: str, short_label: bool = False
 ) -> list[tuple[float, str]]:
     """Humanize the time.
 
     Examples
     --------
     >>> _humanize_time(173, "hours")
```

### Comparing `pytask-0.3.1/src/_pytask/mark/__init__.py` & `pytask-0.3.2/src/_pytask/mark/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING
 
 import click
 import networkx as nx
 from _pytask.click import ColoredCommand
 from _pytask.config import hookimpl
 from _pytask.console import console
-from _pytask.dag import task_and_preceding_tasks
+from _pytask.dag_utils import task_and_preceding_tasks
 from _pytask.exceptions import ConfigurationError
 from _pytask.mark.expression import Expression
 from _pytask.mark.expression import ParseError
 from _pytask.mark.structures import Mark
 from _pytask.mark.structures import MARK_GEN
 from _pytask.mark.structures import MarkDecorator
 from _pytask.mark.structures import MarkGenerator
@@ -217,15 +217,15 @@
     """Deselect tasks."""
     for task in session.tasks:
         if task.name not in remaining:
             task.markers.append(mark)
 
 
 @hookimpl
-def pytask_resolve_dependencies_modify_dag(session: Session, dag: nx.DiGraph) -> None:
+def pytask_dag_modify_dag(session: Session, dag: nx.DiGraph) -> None:
     """Modify the tasks which are executed with expressions and markers."""
     remaining = select_by_keyword(session, dag)
     if remaining is not None:
         _deselect_others_with_mark(
             session, remaining, Mark("skip", (), {"reason": "Deselected by keyword."})
         )
     remaining = select_by_mark(session, dag)
```

### Comparing `pytask-0.3.1/src/_pytask/mark/expression.py` & `pytask-0.3.2/src/_pytask/mark/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,18 +189,18 @@
     def __init__(self, matcher: Callable[[str], bool]) -> None:
         self.matcher = matcher
 
     def __getitem__(self, key: str) -> bool:
         return self.matcher(key[len(IDENT_PREFIX) :])
 
     def __iter__(self) -> Iterator[str]:
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def __len__(self) -> int:
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 class Expression:
     """A compiled match expression as used by -k and -m.
 
     The expression can be evaluated against different matchers.
```

### Comparing `pytask-0.3.1/src/_pytask/mark/structures.py` & `pytask-0.3.2/src/_pytask/mark/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,17 @@
         # If the name is not in the set of known marks after updating,
         # then it really is time to issue a warning or an error.
         if self.config is not None and name not in self.config["markers"]:
             if self.config["strict_markers"]:
                 raise ValueError(f"Unknown pytask.mark.{name}.")
             # Raise a specific error for common misspellings of "parametrize".
             if name in ("parameterize", "parametrise", "parameterise"):
-                warnings.warn(f"Unknown {name!r} mark, did you mean 'parametrize'?")
+                warnings.warn(
+                    f"Unknown {name!r} mark, did you mean 'parametrize'?", stacklevel=1
+                )
 
             warnings.warn(
                 f"Unknown pytask.mark.{name} - is this a typo? You can register "
                 "custom marks to avoid this warning.",
                 stacklevel=2,
             )
```

### Comparing `pytask-0.3.1/src/_pytask/mark_utils.py` & `pytask-0.3.2/src/_pytask/mark_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,18 @@
     return marks
 
 
 def set_marks(obj_or_task: Any | Task, marks: list[Mark]) -> Any | Task:
     """Set marks on a callable or task."""
     if isinstance(obj_or_task, Task):
         obj_or_task.markers = marks
+    elif hasattr(obj_or_task, "pytask_meta"):
+        obj_or_task.pytask_meta.markers = marks
     else:
-        if hasattr(obj_or_task, "pytask_meta"):
-            obj_or_task.pytask_meta.markers = marks
-        else:
-            obj_or_task.pytask_meta = CollectionMetadata(markers=marks)
+        obj_or_task.pytask_meta = CollectionMetadata(markers=marks)
     return obj_or_task
 
 
 def get_marks(obj_or_task: Any | Task, marker_name: str) -> list[Mark]:
     """Get marks from callable or task."""
     marks = get_all_marks(obj_or_task)
     return [mark for mark in marks if mark.name == marker_name]
```

### Comparing `pytask-0.3.1/src/_pytask/models.py` & `pytask-0.3.2/src/_pytask/models.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/nodes.py` & `pytask-0.3.2/src/_pytask/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from abc import ABCMeta
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import TYPE_CHECKING
 
-from _pytask.exceptions import NodeNotFoundError
 from attrs import define
 from attrs import field
 
 
 if TYPE_CHECKING:
     from _pytask.mark import Mark
 
@@ -21,92 +20,91 @@
 __all__ = ["FilePathNode", "MetaNode", "Task"]
 
 
 class MetaNode(metaclass=ABCMeta):
     """Meta class for nodes."""
 
     name: str
-    path: Path
+    """str: The name of node that must be unique."""
 
     @abstractmethod
-    def state(self) -> str | None:
-        """Check the state of the node."""
+    def state(self) -> Any:
         ...
 
 
 @define(kw_only=True)
-class Task:
+class Task(MetaNode):
     """The class for tasks which are Python functions."""
 
     base_name: str
-    """str: The base name of the task."""
+    """The base name of the task."""
     path: Path
-    """pathlib.Path: Path to the file where the task was defined."""
+    """Path to the file where the task was defined."""
     function: Callable[..., Any]
-    """Callable[..., Any]: The task function."""
+    """The task function."""
+    name: str | None = field(default=None, init=False)
+    """The name of the task."""
     short_name: str | None = field(default=None, init=False)
-    """str: The shortest uniquely identifiable name for task for display."""
+    """The shortest uniquely identifiable name for task for display."""
     depends_on: dict[str, MetaNode] = field(factory=dict)
-    """Dict[str, MetaNode]: A list of dependencies of task."""
+    """A list of dependencies of task."""
     produces: dict[str, MetaNode] = field(factory=dict)
-    """Dict[str, MetaNode]: A list of products of task."""
+    """A list of products of task."""
     markers: list[Mark] = field(factory=list)
-    """Optional[List[Mark]]: A list of markers attached to the task function."""
+    """A list of markers attached to the task function."""
     kwargs: dict[str, Any] = field(factory=dict)
-    """Dict[str, Any]: A dictionary with keyword arguments supplied to the task."""
+    """A dictionary with keyword arguments supplied to the task."""
     _report_sections: list[tuple[str, str, str]] = field(factory=list)
-    """List[Tuple[str, str, str]]: Reports with entries for when, what, and content."""
+    """Reports with entries for when, what, and content."""
     attributes: dict[Any, Any] = field(factory=dict)
-    """Dict[Any, Any]: A dictionary to store additional information of the task."""
+    """A dictionary to store additional information of the task."""
 
     def __attrs_post_init__(self: Task) -> None:
         """Change class after initialization."""
+        if self.name is None:
+            self.name = self.path.as_posix() + "::" + self.base_name
+
         if self.short_name is None:
             self.short_name = self.name
 
-    @property
-    def name(self) -> str:
-        """Return the name of the task."""
-        return self.path.as_posix() + "::" + self.base_name
+    def state(self) -> str | None:
+        if self.path.exists():
+            return str(self.path.stat().st_mtime)
+        return None
 
     def execute(self, **kwargs: Any) -> None:
         """Execute the task."""
         self.function(**kwargs)
 
-    def state(self) -> str:
-        """Return the last modified date of the file where the task is defined."""
-        return str(self.path.stat().st_mtime)
-
     def add_report_section(self, when: str, key: str, content: str) -> None:
         """Add sections which will be displayed in report like stdout or stderr."""
         if content:
             self._report_sections.append((when, key, content))
 
 
-@define
+@define(kw_only=True)
 class FilePathNode(MetaNode):
     """The class for a node which is a path."""
 
     name: str
     """str: Name of the node which makes it identifiable in the DAG."""
     value: Path
     """Any: Value passed to the decorator which can be requested inside the function."""
     path: Path
     """pathlib.Path: Path to the FilePathNode."""
 
+    def state(self) -> str | None:
+        if self.path.exists():
+            return str(self.path.stat().st_mtime)
+        return None
+
     @classmethod
     @functools.lru_cache()
     def from_path(cls, path: Path) -> FilePathNode:
         """Instantiate class from path to file.
 
         The `lru_cache` decorator ensures that the same object is not collected twice.
 
         """
         if not path.is_absolute():
             raise ValueError("FilePathNode must be instantiated from absolute path.")
-        return cls(path.as_posix(), path, path)
-
-    def state(self) -> str | None:
-        """Return the last modified date for file path."""
-        if not self.path.exists():
-            raise NodeNotFoundError
-        return str(self.path.stat().st_mtime)
+        return cls(name=path.as_posix(), value=path, path=path)
```

### Comparing `pytask-0.3.1/src/_pytask/outcomes.py` & `pytask-0.3.2/src/_pytask/outcomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,19 +195,19 @@
     """Failed while executing tasks."""
 
     CONFIGURATION_FAILED = 2
 
     COLLECTION_FAILED = 3
     """Failed while collecting tasks."""
 
-    RESOLVING_DEPENDENCIES_FAILED = 4
-    """Failed while resolving dependencies."""
+    DAG_FAILED = 4
+    """Failed while building the DAG."""
 
 
-class PytaskOutcome(Exception):  # noqa: N818
+class PytaskOutcome(Exception):
     """Base outcome of a task."""
 
 
 class Skipped(PytaskOutcome):
     """Outcome if task is skipped."""
 
 
@@ -223,15 +223,15 @@
     """Outcome if task should persist."""
 
 
 class WouldBeExecuted(PytaskOutcome):
     """Outcome if a task would be executed."""
 
 
-class Exit(Exception):  # noqa: N818
+class Exit(Exception):
     """Raised for immediate program exits (no tracebacks/summaries)."""
 
     def __init__(
         self, msg: str = "unknown reason", returncode: int | None = None
     ) -> None:
         self.msg = msg
         self.returncode = returncode
```

### Comparing `pytask-0.3.1/src/_pytask/parameters.py` & `pytask-0.3.2/src/_pytask/parameters.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 _IGNORE_OPTION = click.Option(
     ["--ignore"],
     type=str,
     multiple=True,
     help=(
-        "A pattern to ignore files or directories. For example, task_example.py or "
-        "src/*."
+        "A pattern to ignore files or directories. Refer to pathlib.Path.match for "
+        "more info."
     ),
     default=[],
 )
 """click.Option: An option for the --ignore flag."""
 
 
 _PATH_ARGUMENT = click.Argument(
```

### Comparing `pytask-0.3.1/src/_pytask/parametrize.py` & `pytask-0.3.2/src/_pytask/parametrize.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/parametrize_utils.py` & `pytask-0.3.2/src/_pytask/parametrize_utils.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/persist.py` & `pytask-0.3.2/src/_pytask/persist.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Implement the ability for tasks to persist."""
 from __future__ import annotations
 
 from typing import Any
 from typing import TYPE_CHECKING
 
 from _pytask.config import hookimpl
-from _pytask.dag import node_and_neighbors
+from _pytask.dag_utils import node_and_neighbors
 from _pytask.database_utils import update_states_in_database
-from _pytask.exceptions import NodeNotFoundError
 from _pytask.mark_utils import has_mark
 from _pytask.outcomes import Persisted
 from _pytask.outcomes import TaskOutcome
 
 
 if TYPE_CHECKING:
     from _pytask.session import Session
@@ -35,25 +34,20 @@
 def pytask_execute_task_setup(session: Session, task: Task) -> None:
     """Exit persisting tasks early.
 
     The decorator needs to be set and all nodes need to exist.
 
     """
     if has_mark(task, "persist"):
-        try:
-            for name in node_and_neighbors(session.dag, task.name):
-                node = (
-                    session.dag.nodes[name].get("task")
-                    or session.dag.nodes[name]["node"]
-                )
-                node.state()
-        except NodeNotFoundError:
-            all_nodes_exist = False
-        else:
-            all_nodes_exist = True
+        all_nodes_exist = all(
+            (
+                session.dag.nodes[name].get("task") or session.dag.nodes[name]["node"]
+            ).state()
+            for name in node_and_neighbors(session.dag, task.name)
+        )
 
         if all_nodes_exist:
             raise Persisted
 
 
 @hookimpl
 def pytask_execute_task_process_report(
@@ -62,10 +56,10 @@
     """Set task status to success.
 
     Do not return ``True`` so that states will be updated in database.
 
     """
     if report.exc_info and isinstance(report.exc_info[1], Persisted):
         report.outcome = TaskOutcome.PERSISTENCE
-        update_states_in_database(session.dag, report.task.name)
+        update_states_in_database(session, report.task.name)
         return True
     return None
```

### Comparing `pytask-0.3.1/src/_pytask/profile.py` & `pytask-0.3.2/src/_pytask/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         ] = sys.exc_info()
         console.print(render_exc_info(*exc_info, show_locals=config["show_locals"]))
 
     else:
         try:
             session.hook.pytask_log_session_header(session=session)
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_resolve_dependencies(session=session)
+            session.hook.pytask_dag(session=session)
 
             profile: dict[str, dict[str, Any]] = {
                 task.name: {} for task in session.tasks
             }
             session.hook.pytask_profile_add_info_on_task(
                 session=session, tasks=session.tasks, profile=profile
             )
```

### Comparing `pytask-0.3.1/src/_pytask/report.py` & `pytask-0.3.2/src/_pytask/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,21 +38,21 @@
         node: MetaNode | None = None,
     ) -> CollectionReport:
         exc_info = remove_internal_traceback_frames_from_exc_info(exc_info)
         return cls(outcome=outcome, node=node, exc_info=exc_info)
 
 
 @define
-class ResolvingDependenciesReport:
-    """A report for an error while resolving dependencies."""
+class DagReport:
+    """A report for an error during the creation of the DAG."""
 
     exc_info: ExceptionInfo
 
     @classmethod
-    def from_exception(cls, exc_info: ExceptionInfo) -> ResolvingDependenciesReport:
+    def from_exception(cls, exc_info: ExceptionInfo) -> DagReport:
         exc_info = remove_internal_traceback_frames_from_exc_info(exc_info)
         return cls(exc_info)
 
 
 @define
 class ExecutionReport:
     """A report for an executed task."""
```

### Comparing `pytask-0.3.1/src/_pytask/resolve_dependencies.py` & `pytask-0.3.2/src/_pytask/dag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 """This module contains code related to resolving dependencies."""
 from __future__ import annotations
 
+import hashlib
 import itertools
 import sys
 
 import networkx as nx
 from _pytask.config import hookimpl
 from _pytask.config import IS_FILE_SYSTEM_CASE_SENSITIVE
 from _pytask.console import ARROW_DOWN_ICON
 from _pytask.console import console
 from _pytask.console import FILE_ICON
 from _pytask.console import render_to_string
 from _pytask.console import TASK_ICON
-from _pytask.dag import node_and_neighbors
-from _pytask.dag import task_and_descending_tasks
-from _pytask.dag import TopologicalSorter
+from _pytask.dag_utils import node_and_neighbors
+from _pytask.dag_utils import task_and_descending_tasks
+from _pytask.dag_utils import TopologicalSorter
 from _pytask.database_utils import State
-from _pytask.exceptions import NodeNotFoundError
 from _pytask.exceptions import ResolvingDependenciesError
 from _pytask.mark import Mark
 from _pytask.mark_utils import get_marks
 from _pytask.mark_utils import has_mark
+from _pytask.nodes import FilePathNode
 from _pytask.nodes import MetaNode
 from _pytask.nodes import Task
 from _pytask.path import find_common_ancestor_of_nodes
-from _pytask.report import ResolvingDependenciesReport
+from _pytask.report import DagReport
 from _pytask.session import Session
 from _pytask.shared import reduce_names_of_multiple_nodes
 from _pytask.shared import reduce_node_name
 from _pytask.traceback import render_exc_info
 from pony import orm
 from pybaum import tree_map
 from rich.text import Text
 from rich.tree import Tree
 
 
 @hookimpl
-def pytask_resolve_dependencies(session: Session) -> bool | None:
+def pytask_dag(session: Session) -> bool | None:
     """Create a directed acyclic graph (DAG) capturing dependencies between functions.
 
     Parameters
     ----------
     session : _pytask.session.Session
         Dictionary containing tasks.
 
     """
     try:
-        session.dag = session.hook.pytask_resolve_dependencies_create_dag(
+        session.dag = session.hook.pytask_dag_create_dag(
             session=session, tasks=session.tasks
         )
-        session.hook.pytask_resolve_dependencies_modify_dag(
-            session=session, dag=session.dag
-        )
-        session.hook.pytask_resolve_dependencies_validate_dag(
-            session=session, dag=session.dag
-        )
-        session.hook.pytask_resolve_dependencies_select_execution_dag(
-            session=session, dag=session.dag
-        )
+        session.hook.pytask_dag_modify_dag(session=session, dag=session.dag)
+        session.hook.pytask_dag_validate_dag(session=session, dag=session.dag)
+        session.hook.pytask_dag_select_execution_dag(session=session, dag=session.dag)
 
     except Exception:  # noqa: BLE001
-        report = ResolvingDependenciesReport.from_exception(sys.exc_info())
-        session.hook.pytask_resolve_dependencies_log(session=session, report=report)
+        report = DagReport.from_exception(sys.exc_info())
+        session.hook.pytask_dag_log(session=session, report=report)
         session.resolving_dependencies_report = report
 
         raise ResolvingDependenciesError from None
 
     else:
         return True
 
 
 @hookimpl
-def pytask_resolve_dependencies_create_dag(tasks: list[Task]) -> nx.DiGraph:
+def pytask_dag_create_dag(tasks: list[Task]) -> nx.DiGraph:
     """Create the DAG from tasks, dependencies and products."""
     dag = nx.DiGraph()
 
     for task in tasks:
         dag.add_node(task.name, task=task)
 
         tree_map(lambda x: dag.add_node(x.name, node=x), task.depends_on)
@@ -88,62 +83,83 @@
 
     _check_if_dag_has_cycles(dag)
 
     return dag
 
 
 @hookimpl
-def pytask_resolve_dependencies_select_execution_dag(dag: nx.DiGraph) -> None:
+def pytask_dag_select_execution_dag(session: Session, dag: nx.DiGraph) -> None:
     """Select the tasks which need to be executed."""
     scheduler = TopologicalSorter.from_dag(dag)
-    visited_nodes = []
+    visited_nodes: set[str] = set()
 
     for task_name in scheduler.static_order():
         if task_name not in visited_nodes:
-            have_changed = _have_task_or_neighbors_changed(task_name, dag)
+            task = dag.nodes[task_name]["task"]
+            have_changed = _have_task_or_neighbors_changed(session, dag, task)
             if have_changed:
-                visited_nodes += list(task_and_descending_tasks(task_name, dag))
+                visited_nodes.update(task_and_descending_tasks(task_name, dag))
             else:
                 dag.nodes[task_name]["task"].markers.append(
                     Mark("skip_unchanged", (), {})
                 )
 
 
 @hookimpl
-def pytask_resolve_dependencies_validate_dag(dag: nx.DiGraph) -> None:
+def pytask_dag_validate_dag(dag: nx.DiGraph) -> None:
     """Validate the DAG."""
     _check_if_root_nodes_are_available(dag)
     _check_if_tasks_have_the_same_products(dag)
 
 
-def _have_task_or_neighbors_changed(task_name: str, dag: nx.DiGraph) -> bool:
+def _have_task_or_neighbors_changed(
+    session: Session, dag: nx.DiGraph, task: Task
+) -> bool:
     """Indicate whether dependencies or products of a task have changed."""
     return any(
-        _has_node_changed(task_name, dag.nodes[node])
-        for node in node_and_neighbors(dag, task_name)
+        session.hook.pytask_dag_has_node_changed(
+            session=session,
+            dag=dag,
+            task_name=task.name,
+            node=dag.nodes[node_name].get("task") or dag.nodes[node_name].get("node"),
+        )
+        for node_name in node_and_neighbors(dag, task.name)
     )
 
 
 @orm.db_session
-def _has_node_changed(task_name: str, node_dict: dict[str, MetaNode | Task]) -> bool:
+@hookimpl(trylast=True)
+def pytask_dag_has_node_changed(node: MetaNode, task_name: str) -> bool:
     """Indicate whether a single dependency or product has changed."""
-    node = node_dict.get("task") or node_dict["node"]
-    try:
-        state = node.state()
-    except NodeNotFoundError:
-        out = True
-    else:
+    if isinstance(node, (FilePathNode, Task)):
+        # If node does not exist, we receive None.
+        file_state = node.state()
+        if file_state is None:
+            return True
+
+        # If the node is not in the database.
         try:
-            state_in_db = State[task_name, node.name].state  # type: ignore[misc]
+            name = node.name
+            db_state = State[task_name, name]  # type: ignore[type-arg, valid-type]
         except orm.ObjectNotFound:
-            out = True
-        else:
-            out = state != state_in_db
+            return True
 
-    return out
+        # If the modification times match, the node has not been changed.
+        if file_state == db_state.modification_time:
+            return False
+
+        # If the modification time changed, quickly return for non-tasks.
+        if isinstance(node, FilePathNode):
+            return True
+
+        # When modification times changed, we are still comparing the hash of the file
+        # to avoid unnecessary and expensive reexecutions of tasks.
+        file_hash = hashlib.sha256(node.path.read_bytes()).hexdigest()
+        return file_hash != db_state.file_hash
+    return node.state()
 
 
 def _check_if_dag_has_cycles(dag: nx.DiGraph) -> None:
     """Check if DAG has cycles."""
     try:
         cycles = nx.algorithms.cycles.find_cycle(dag)
     except nx.NetworkXNoCycle:
@@ -186,18 +202,16 @@
         is_node = "node" in dag.nodes[node]
         is_without_parents = len(list(dag.predecessors(node))) == 0
         if is_node and is_without_parents:
             are_all_tasks_skipped, is_task_skipped = _check_if_tasks_are_skipped(
                 node, dag, is_task_skipped
             )
             if not are_all_tasks_skipped:
-                try:
-                    dag.nodes[node]["node"].state()
-                except NodeNotFoundError:
-                    # Shorten node names for better printing.
+                node_exists = dag.nodes[node]["node"].state()
+                if not node_exists:
                     missing_root_nodes.append(node)
 
     if missing_root_nodes:
         all_names = missing_root_nodes + [
             successor
             for node in missing_root_nodes
             for successor in dag.successors(node)
@@ -297,17 +311,15 @@
             "There are some tasks which produce the same output. See the following "
             "tree which shows which products are produced by multiple tasks."
             f"\n\n{text}"
         )
 
 
 @hookimpl
-def pytask_resolve_dependencies_log(
-    session: Session, report: ResolvingDependenciesReport
-) -> None:
+def pytask_dag_log(session: Session, report: DagReport) -> None:
     """Log errors which happened while resolving dependencies."""
     console.print()
     console.rule(
         Text("Failures during resolving dependencies", style="failed"),
         style="failed",
     )
```

### Comparing `pytask-0.3.1/src/_pytask/session.py` & `pytask-0.3.2/src/_pytask/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,50 +16,50 @@
 except ImportError:
     from pluggy.hooks import _HookRelay
 
 
 if TYPE_CHECKING:
     from _pytask.report import CollectionReport
     from _pytask.report import ExecutionReport
-    from _ptytask.report import ResolvingDependenciesReport
+    from _ptytask.report import DagReport
     from _pytask.nodes import Task
 
 
 @define
 class Session:
     """The session of pytask."""
 
     config: dict[str, Any] = field(factory=dict)
-    """Dict[str, Any]: Configuration of the session."""
+    """Configuration of the session."""
     hook: _HookRelay | None = None
-    """pluggy.hooks._HookRelay | None: Holds all hooks collected by pytask."""
+    """Holds all hooks collected by pytask."""
     collection_reports: list[CollectionReport] = field(factory=list)
-    """list[CollectionReport]: Reports for collected items.
+    """Reports for collected items.
 
     The reports capture errors which happened while collecting tasks.
 
     """
     tasks: list[Task] = field(factory=list)
-    """list[Task]: List of collected tasks."""
+    """List of collected tasks."""
     dag: nx.DiGraph | None = None
-    resolving_dependencies_report: ResolvingDependenciesReport | None = None
-    """ResolvingDependenciesReport | None: Reports for resolving dependencies failed."""
+    resolving_dependencies_report: DagReport | None = None
+    """Reports for resolving dependencies failed."""
     execution_reports: list[ExecutionReport] = field(factory=list)
-    """list[ExecutionReport]: Reports for executed tasks."""
+    """Reports for executed tasks."""
     exit_code: ExitCode = ExitCode.OK
 
     collection_start: float | None = None
     collection_end: float | None = None
     execution_start: float | None = None
     execution_end: float | None = None
 
     n_tasks_failed: int = 0
-    """int | None: Number of tests which have failed."""
+    """Number of tests which have failed."""
     scheduler: Any = None
     should_stop: bool = False
-    """bool | None: Indicates whether the session should be stopped."""
+    """Indicates whether the session should be stopped."""
     warnings: list[WarningReport] = field(factory=list)
 
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> Session:
         """Construct the class from a config."""
         return cls(config, config["pm"].hook)
```

### Comparing `pytask-0.3.1/src/_pytask/shared.py` & `pytask-0.3.2/src/_pytask/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any
 from typing import Iterable
 from typing import Sequence
 
 import click
 import networkx as nx
 from _pytask.console import format_task_id
+from _pytask.nodes import FilePathNode
 from _pytask.nodes import MetaNode
 from _pytask.nodes import Task
 from _pytask.path import find_closest_ancestor
 from _pytask.path import find_common_ancestor
 from _pytask.path import relative_to
 
 
@@ -62,27 +63,28 @@
     The whole name of the node - which includes the drive letter - can be very long
     when using nested folder structures in bigger projects.
 
     Thus, the part of the name which contains the path is replaced by the relative
     path from one path in ``session.config["paths"]`` to the node.
 
     """
-    ancestor = find_closest_ancestor(node.path, paths)
-    if ancestor is None:
-        try:
-            ancestor = find_common_ancestor(node.path, *paths)
-        except ValueError:
-            ancestor = node.path.parents[-1]
+    if isinstance(node, (Task, FilePathNode)):
+        ancestor = find_closest_ancestor(node.path, paths)
+        if ancestor is None:
+            try:
+                ancestor = find_common_ancestor(node.path, *paths)
+            except ValueError:
+                ancestor = node.path.parents[-1]
 
-    if isinstance(node, MetaNode):
-        name = relative_to(node.path, ancestor).as_posix()
-    else:
-        raise TypeError(f"Unknown node {node} with type {type(node)!r}.")
-
-    return name
+        if isinstance(node, MetaNode):
+            name = relative_to(node.path, ancestor).as_posix()
+        else:
+            raise TypeError(f"Unknown node {node} with type {type(node)!r}.")
+        return name
+    return node.name
 
 
 def reduce_names_of_multiple_nodes(
     names: list[str], dag: nx.DiGraph, paths: Sequence[str | Path]
 ) -> list[str]:
     """Reduce the names of multiple nodes in the DAG."""
     short_names = []
@@ -92,15 +94,15 @@
         if isinstance(node, Task):
             short_name = format_task_id(
                 node, editor_url_scheme="no_link", short_name=True
             )
         elif isinstance(node, MetaNode):
             short_name = reduce_node_name(node, paths)
         else:
-            raise TypeError(f"Requires 'Task' or 'MetaNode' and not {type(node)!r}.")
+            raise TypeError(f"Requires 'Task' or 'Node' and not {type(node)!r}.")
 
         short_names.append(short_name)
 
     return short_names
 
 
 def find_duplicates(x: Iterable[Any]) -> set[Any]:
```

### Comparing `pytask-0.3.1/src/_pytask/skipping.py` & `pytask-0.3.2/src/_pytask/skipping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module contains everything related to skipping tasks."""
 from __future__ import annotations
 
 from typing import Any
 from typing import TYPE_CHECKING
 
 from _pytask.config import hookimpl
-from _pytask.dag import descending_tasks
+from _pytask.dag_utils import descending_tasks
 from _pytask.mark import Mark
 from _pytask.mark_utils import get_marks
 from _pytask.mark_utils import has_mark
 from _pytask.outcomes import Skipped
 from _pytask.outcomes import SkippedAncestorFailed
 from _pytask.outcomes import SkippedUnchanged
 from _pytask.outcomes import TaskOutcome
@@ -43,20 +43,20 @@
         "executed and have not been changed.",
         "skipif": "Skip a task and all its dependent tasks if a condition is met.",
     }
     config["markers"] = {**config["markers"], **markers}
 
 
 @hookimpl
-def pytask_execute_task_setup(task: Task) -> None:
+def pytask_execute_task_setup(session: Session, task: Task) -> None:
     """Take a short-cut for skipped tasks during setup with an exception."""
     is_unchanged = has_mark(task, "skip_unchanged") and not has_mark(
         task, "would_be_executed"
     )
-    if is_unchanged:
+    if is_unchanged and not session.config["force"]:
         raise SkippedUnchanged
 
     ancestor_failed_marks = get_marks(task, "skip_ancestor_failed")
     if ancestor_failed_marks:
         message = "\n".join(
             skip_ancestor_failed(*mark.args, **mark.kwargs)
             for mark in ancestor_failed_marks
```

### Comparing `pytask-0.3.1/src/_pytask/task.py` & `pytask-0.3.2/src/_pytask/task.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/task_utils.py` & `pytask-0.3.2/src/_pytask/task_utils.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/traceback.py` & `pytask-0.3.2/src/_pytask/traceback.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/warnings.py` & `pytask-0.3.2/src/_pytask/warnings.py`

 * *Files identical despite different names*

### Comparing `pytask-0.3.1/src/_pytask/warnings_utils.py` & `pytask-0.3.2/src/_pytask/warnings_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 class WarningReport(NamedTuple):
     message: str
     fs_location: tuple[str, int]
     id_: str | None
 
 
 @functools.lru_cache(maxsize=50)
-def parse_warning_filter(  # noqa: C901
+def parse_warning_filter(  # noqa: PLR0912
     arg: str, *, escape: bool
 ) -> tuple[warnings._ActionKind, str, type[Warning], str, int]:
     """Parse a warnings filter string.
 
     This is copied from warnings._setoption with the following changes:
 
     - Does not apply the filter.
@@ -151,16 +151,15 @@
 def catch_warnings_for_item(
     session: Session,
     task: Task | None = None,
     when: str | None = None,
 ) -> Generator[None, None, None]:
     """Context manager that catches warnings generated in the contained execution block.
 
-    ``item`` can be None if we are not in the context of an item execution. Each warning
-    captured triggers the ``pytest_warning_recorded`` hook.
+    ``item`` can be None if we are not in the context of an item execution.
 
     """
     with warnings.catch_warnings(record=True) as log:
         # mypy can't infer that record=True means log is not None; help it.
         assert log is not None
 
         for arg in session.config["filterwarnings"]:
```

### Comparing `pytask-0.3.1/src/pytask/__init__.py` & `pytask-0.3.2/src/pytask/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from _pytask.collect_utils import depends_on
 from _pytask.collect_utils import parse_nodes
 from _pytask.collect_utils import produces
 from _pytask.compat import check_for_optional_program
 from _pytask.compat import import_optional_dependency
 from _pytask.config import hookimpl
 from _pytask.console import console
+from _pytask.database_utils import db
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import ConfigurationError
 from _pytask.exceptions import ExecutionError
 from _pytask.exceptions import NodeNotCollectedError
 from _pytask.exceptions import NodeNotFoundError
 from _pytask.exceptions import PytaskError
 from _pytask.exceptions import ResolvingDependenciesError
@@ -40,16 +41,16 @@
 from _pytask.outcomes import ExitCode
 from _pytask.outcomes import Persisted
 from _pytask.outcomes import Skipped
 from _pytask.outcomes import SkippedAncestorFailed
 from _pytask.outcomes import SkippedUnchanged
 from _pytask.outcomes import TaskOutcome
 from _pytask.report import CollectionReport
+from _pytask.report import DagReport
 from _pytask.report import ExecutionReport
-from _pytask.report import ResolvingDependenciesReport
 from _pytask.session import Session
 from _pytask.traceback import format_exception_without_traceback
 from _pytask.traceback import remove_internal_traceback_frames_from_exc_info
 from _pytask.traceback import remove_traceback_from_exc_info
 from _pytask.traceback import render_exc_info
 from _pytask.warnings_utils import parse_warning_filter
 from _pytask.warnings_utils import warning_record_to_str
@@ -79,28 +80,29 @@
     "MarkGenerator",
     "MetaNode",
     "NodeNotCollectedError",
     "NodeNotFoundError",
     "Persisted",
     "PytaskError",
     "ResolvingDependenciesError",
-    "ResolvingDependenciesReport",
+    "DagReport",
     "Session",
     "Skipped",
     "SkippedAncestorFailed",
     "SkippedUnchanged",
     "Task",
     "TaskOutcome",
     "WarningReport",
     "__version__",
     "build_dag",
     "check_for_optional_program",
     "cli",
     "console",
     "count_outcomes",
+    "db",
     "depends_on",
     "format_exception_without_traceback",
     "get_all_marks",
     "get_marks",
     "has_mark",
     "hookimpl",
     "import_optional_dependency",
```

### Comparing `pytask-0.3.1/src/pytask.egg-info/PKG-INFO` & `pytask-0.3.2/src/pytask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytask
-Version: 0.3.1
+Version: 0.3.2
 Summary: In its highest aspirations, pytask tries to be pytest as a build system.
 Home-page: https://pytask-dev.readthedocs.io/en/stable
 Author: Tobias Raabe
 Author-email: raabe@posteo.de
 License: MIT
 Project-URL: Changelog, https://pytask-dev.readthedocs.io/en/stable/changes.html
 Project-URL: Documentation, https://pytask-dev.readthedocs.io/en/stable
```

### Comparing `pytask-0.3.1/src/pytask.egg-info/SOURCES.txt` & `pytask-0.3.2/src/pytask.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 CITATION
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+.github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/documentation.md
 .github/ISSUE_TEMPLATE/enhancement.md
 .github/ISSUE_TEMPLATE/question.md
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
@@ -24,14 +25,15 @@
 src/_pytask/collect_command.py
 src/_pytask/collect_utils.py
 src/_pytask/compat.py
 src/_pytask/config.py
 src/_pytask/config_utils.py
 src/_pytask/console.py
 src/_pytask/dag.py
+src/_pytask/dag_utils.py
 src/_pytask/database.py
 src/_pytask/database_utils.py
 src/_pytask/debugging.py
 src/_pytask/enums.py
 src/_pytask/exceptions.py
 src/_pytask/execute.py
 src/_pytask/git.py
@@ -48,15 +50,14 @@
 src/_pytask/parametrize_utils.py
 src/_pytask/path.py
 src/_pytask/persist.py
 src/_pytask/pluginmanager.py
 src/_pytask/profile.py
 src/_pytask/py.typed
 src/_pytask/report.py
-src/_pytask/resolve_dependencies.py
 src/_pytask/session.py
 src/_pytask/shared.py
 src/_pytask/skipping.py
 src/_pytask/task.py
 src/_pytask/task_utils.py
 src/_pytask/traceback.py
 src/_pytask/warnings.py
```

