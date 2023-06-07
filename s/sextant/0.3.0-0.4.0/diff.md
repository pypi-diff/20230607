# Comparing `tmp/sextant-0.3.0.tar.gz` & `tmp/sextant-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sextant-0.3.0.tar", last modified: Wed Apr 19 10:43:26 2023, max compression
+gzip compressed data, was "sextant-0.4.0.tar", last modified: Wed Jun  7 06:12:28 2023, max compression
```

## Comparing `sextant-0.3.0.tar` & `sextant-0.4.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.836953 sextant-0.3.0/
--rw-r--r--   0 joe       (1000) joe       (1000)      120 2022-10-17 14:22:50.000000 sextant-0.3.0/.gitignore
--rw-r--r--   0 joe       (1000) joe       (1000)      982 2022-11-10 15:31:15.000000 sextant-0.3.0/.gitlab-ci.yml
--rw-r--r--   0 joe       (1000) joe       (1000)      111 2022-11-10 15:31:15.000000 sextant-0.3.0/.pylintrc
--rw-r--r--   0 joe       (1000) joe       (1000)      281 2023-04-19 10:15:58.000000 sextant-0.3.0/CHANGELOG
--rw-r--r--   0 joe       (1000) joe       (1000)      785 2022-10-17 05:06:58.000000 sextant-0.3.0/LICENSE
--rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-04-19 10:43:26.836953 sextant-0.3.0/PKG-INFO
--rw-r--r--   0 joe       (1000) joe       (1000)     8315 2023-04-19 10:15:44.000000 sextant-0.3.0/README.md
--rw-r--r--   0 joe       (1000) joe       (1000)      322 2022-10-17 05:18:37.000000 sextant-0.3.0/pyproject.toml
--rw-r--r--   0 joe       (1000) joe       (1000)       38 2023-04-19 10:43:26.836953 sextant-0.3.0/setup.cfg
--rw-r--r--   0 joe       (1000) joe       (1000)     1008 2023-04-19 10:15:44.000000 sextant-0.3.0/setup.py
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.828953 sextant-0.3.0/sextant/
--rw-r--r--   0 joe       (1000) joe       (1000)      144 2023-04-19 10:15:44.000000 sextant-0.3.0/sextant/__init__.py
--rw-r--r--   0 joe       (1000) joe       (1000)    10725 2023-04-19 10:15:44.000000 sextant-0.3.0/sextant/cli.py
--rw-r--r--   0 joe       (1000) joe       (1000)     8706 2023-04-19 10:15:44.000000 sextant-0.3.0/sextant/dependency.py
--rw-r--r--   0 joe       (1000) joe       (1000)     4672 2023-04-19 10:15:44.000000 sextant-0.3.0/sextant/module.py
--rw-r--r--   0 joe       (1000) joe       (1000)    13379 2023-04-19 10:15:44.000000 sextant-0.3.0/sextant/scaffold.py
--rw-r--r--   0 joe       (1000) joe       (1000)     1493 2023-01-12 14:50:29.000000 sextant-0.3.0/sextant/semver.py
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/sextant.egg-info/
--rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-04-19 10:43:26.000000 sextant-0.3.0/sextant.egg-info/PKG-INFO
--rw-r--r--   0 joe       (1000) joe       (1000)     1941 2023-04-19 10:43:26.000000 sextant-0.3.0/sextant.egg-info/SOURCES.txt
--rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-04-19 10:43:26.000000 sextant-0.3.0/sextant.egg-info/dependency_links.txt
--rw-r--r--   0 joe       (1000) joe       (1000)       45 2023-04-19 10:43:26.000000 sextant-0.3.0/sextant.egg-info/entry_points.txt
--rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-01-12 14:51:41.000000 sextant-0.3.0/sextant.egg-info/not-zip-safe
--rw-r--r--   0 joe       (1000) joe       (1000)       78 2023-04-19 10:43:26.000000 sextant-0.3.0/sextant.egg-info/requires.txt
--rw-r--r--   0 joe       (1000) joe       (1000)       14 2023-04-19 10:43:26.000000 sextant-0.3.0/sextant.egg-info/top_level.txt
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/
--rw-r--r--   0 joe       (1000) joe       (1000)       93 2022-10-17 06:53:02.000000 sextant-0.3.0/tests/__init__.py
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.828953 sextant-0.3.0/tests/fixtures/
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/bar/
--rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:39:51.000000 sextant-0.3.0/tests/fixtures/bar/beer_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:40:01.000000 sextant-0.3.0/tests/fixtures/bar/beer_2.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)      563 2022-10-12 05:38:33.000000 sextant-0.3.0/tests/fixtures/bar/module.json
--rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:15.000000 sextant-0.3.0/tests/fixtures/bar/stool_0.5.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:27.000000 sextant-0.3.0/tests/fixtures/bar/stool_0.5.1.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:38.000000 sextant-0.3.0/tests/fixtures/bar/stool_1.0.0.tpl
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/baz/
--rw-r--r--   0 joe       (1000) joe       (1000)       20 2022-10-12 05:40:51.000000 sextant-0.3.0/tests/fixtures/baz/drunk-unicorn_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)      437 2022-10-17 14:10:38.000000 sextant-0.3.0/tests/fixtures/baz/module.json
--rw-r--r--   0 joe       (1000) joe       (1000)       23 2022-10-12 05:41:00.000000 sextant-0.3.0/tests/fixtures/baz/sitting-pangolin_1.0.0.tpl
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.828953 sextant-0.3.0/tests/fixtures/charts/
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/charts/bad/
--rw-r--r--   0 joe       (1000) joe       (1000)       59 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/bad/package.json
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/charts/bad/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/bad/templates/.gitkeep
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/charts/good/
--rw-r--r--   0 joe       (1000) joe       (1000)       50 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/good/package.json
--rw-r--r--   0 joe       (1000) joe       (1000)      395 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/charts/good/package.lock
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/charts/good/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/good/templates/.gitkeep
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/charts/other/
--rw-r--r--   0 joe       (1000) joe       (1000)       43 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/other/package.json
--rw-r--r--   0 joe       (1000) joe       (1000)      248 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/other/package.lock
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/charts/other/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/fixtures/charts/other/templates/.gitkeep
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.832953 sextant-0.3.0/tests/fixtures/foo/
--rw-r--r--   0 joe       (1000) joe       (1000)      418 2022-10-12 05:43:41.000000 sextant-0.3.0/tests/fixtures/foo/module.json
--rw-r--r--   0 joe       (1000) joe       (1000)       16 2022-10-12 05:41:58.000000 sextant-0.3.0/tests/fixtures/foo/pangolin_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       15 2022-10-12 05:41:43.000000 sextant-0.3.0/tests/fixtures/foo/unicorn_1.0.0.tpl
--rw-r--r--   0 joe       (1000) joe       (1000)       14 2022-10-12 05:41:53.000000 sextant-0.3.0/tests/fixtures/foo/unicorn_1.1.0.tpl
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.836953 sextant-0.3.0/tests/fixtures/scaffold/
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.836953 sextant-0.3.0/tests/fixtures/scaffold/_skel/
--rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/Chart.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)       44 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/package.json
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.836953 sextant-0.3.0/tests/fixtures/scaffold/_skel/templates/
--rw-r--r--   0 joe       (1000) joe       (1000)       20 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/templates/configmap.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)      523 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)       18 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/templates/service.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)       28 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/templates/spurious.yaml.skel
--rw-r--r--   0 joe       (1000) joe       (1000)      151 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_skel/values.yaml
-drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-04-19 10:43:26.836953 sextant-0.3.0/tests/fixtures/scaffold/_wizard/
--rw-r--r--   0 joe       (1000) joe       (1000)      427 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_wizard/ingress.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)      287 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_wizard/ingress_nginx.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)     1061 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/_wizard/scaffold.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)       77 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/presets.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)      177 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/fixtures/scaffold/questions.yaml
--rw-r--r--   0 joe       (1000) joe       (1000)     1606 2022-11-10 15:31:15.000000 sextant-0.3.0/tests/test_cli.py
--rw-r--r--   0 joe       (1000) joe       (1000)     1120 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/test_dependency.py
--rw-r--r--   0 joe       (1000) joe       (1000)     2167 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/test_module.py
--rw-r--r--   0 joe       (1000) joe       (1000)     3049 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/test_package.py
--rw-r--r--   0 joe       (1000) joe       (1000)     8969 2023-04-19 10:15:44.000000 sextant-0.3.0/tests/test_scaffold.py
--rw-r--r--   0 joe       (1000) joe       (1000)      755 2023-04-19 10:15:44.000000 sextant-0.3.0/tox.ini
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/
+-rw-r--r--   0 joe       (1000) joe       (1000)      120 2022-10-17 14:22:50.000000 sextant-0.4.0/.gitignore
+-rw-r--r--   0 joe       (1000) joe       (1000)      982 2022-11-10 15:31:15.000000 sextant-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0 joe       (1000) joe       (1000)      111 2022-11-10 15:31:15.000000 sextant-0.4.0/.pylintrc
+-rw-r--r--   0 joe       (1000) joe       (1000)      281 2023-04-19 10:15:58.000000 sextant-0.4.0/CHANGELOG
+-rw-r--r--   0 joe       (1000) joe       (1000)      785 2022-10-17 05:06:58.000000 sextant-0.4.0/LICENSE
+-rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-06-07 06:12:28.563573 sextant-0.4.0/PKG-INFO
+-rw-r--r--   0 joe       (1000) joe       (1000)     8459 2023-06-07 06:09:53.000000 sextant-0.4.0/README.md
+-rw-r--r--   0 joe       (1000) joe       (1000)      337 2023-06-06 05:38:31.000000 sextant-0.4.0/pyproject.toml
+-rw-r--r--   0 joe       (1000) joe       (1000)       38 2023-06-07 06:12:28.563573 sextant-0.4.0/setup.cfg
+-rw-r--r--   0 joe       (1000) joe       (1000)     1008 2023-04-19 10:15:44.000000 sextant-0.4.0/setup.py
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/sextant/
+-rw-r--r--   0 joe       (1000) joe       (1000)      224 2023-06-06 05:38:31.000000 sextant-0.4.0/sextant/__init__.py
+-rw-r--r--   0 joe       (1000) joe       (1000)    12923 2023-06-07 06:09:42.000000 sextant-0.4.0/sextant/cli.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     8706 2023-04-19 10:15:44.000000 sextant-0.4.0/sextant/dependency.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     4672 2023-04-19 10:15:44.000000 sextant-0.4.0/sextant/module.py
+-rw-r--r--   0 joe       (1000) joe       (1000)    13379 2023-04-19 10:15:44.000000 sextant-0.4.0/sextant/scaffold.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     1493 2023-01-12 14:50:29.000000 sextant-0.4.0/sextant/semver.py
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/sextant.egg-info/
+-rw-r--r--   0 joe       (1000) joe       (1000)      367 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/PKG-INFO
+-rw-r--r--   0 joe       (1000) joe       (1000)     1979 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/SOURCES.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/dependency_links.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)       45 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/entry_points.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)        1 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/not-zip-safe
+-rw-r--r--   0 joe       (1000) joe       (1000)       78 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/requires.txt
+-rw-r--r--   0 joe       (1000) joe       (1000)       14 2023-06-07 06:12:28.000000 sextant-0.4.0/sextant.egg-info/top_level.txt
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/
+-rw-r--r--   0 joe       (1000) joe       (1000)       93 2022-10-17 06:53:02.000000 sextant-0.4.0/tests/__init__.py
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.555573 sextant-0.4.0/tests/fixtures/
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/bar/
+-rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:39:51.000000 sextant-0.4.0/tests/fixtures/bar/beer_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       11 2022-10-12 05:40:01.000000 sextant-0.4.0/tests/fixtures/bar/beer_2.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)      563 2022-10-12 05:38:33.000000 sextant-0.4.0/tests/fixtures/bar/module.json
+-rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:15.000000 sextant-0.4.0/tests/fixtures/bar/stool_0.5.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:27.000000 sextant-0.4.0/tests/fixtures/bar/stool_0.5.1.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       12 2022-10-12 05:40:38.000000 sextant-0.4.0/tests/fixtures/bar/stool_1.0.0.tpl
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/baz/
+-rw-r--r--   0 joe       (1000) joe       (1000)       20 2022-10-12 05:40:51.000000 sextant-0.4.0/tests/fixtures/baz/drunk-unicorn_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)      437 2022-10-17 14:10:38.000000 sextant-0.4.0/tests/fixtures/baz/module.json
+-rw-r--r--   0 joe       (1000) joe       (1000)       23 2022-10-12 05:41:00.000000 sextant-0.4.0/tests/fixtures/baz/sitting-pangolin_1.0.0.tpl
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.555573 sextant-0.4.0/tests/fixtures/charts/
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/bad/
+-rw-r--r--   0 joe       (1000) joe       (1000)       59 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/bad/package.json
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/bad/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/bad/templates/.gitkeep
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/good/
+-rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-06-06 11:36:44.000000 sextant-0.4.0/tests/fixtures/charts/good/Chart.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)       50 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/good/package.json
+-rw-r--r--   0 joe       (1000) joe       (1000)      395 2023-06-07 05:33:18.000000 sextant-0.4.0/tests/fixtures/charts/good/package.lock
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/good/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/good/templates/.gitkeep
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/other/
+-rw-r--r--   0 joe       (1000) joe       (1000)       43 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/other/package.json
+-rw-r--r--   0 joe       (1000) joe       (1000)      248 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/other/package.lock
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/charts/other/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)        0 2022-11-10 15:31:15.000000 sextant-0.4.0/tests/fixtures/charts/other/templates/.gitkeep
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.559573 sextant-0.4.0/tests/fixtures/foo/
+-rw-r--r--   0 joe       (1000) joe       (1000)      418 2022-10-12 05:43:41.000000 sextant-0.4.0/tests/fixtures/foo/module.json
+-rw-r--r--   0 joe       (1000) joe       (1000)       16 2022-10-12 05:41:58.000000 sextant-0.4.0/tests/fixtures/foo/pangolin_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       15 2022-10-12 05:41:43.000000 sextant-0.4.0/tests/fixtures/foo/unicorn_1.0.0.tpl
+-rw-r--r--   0 joe       (1000) joe       (1000)       14 2022-10-12 05:41:53.000000 sextant-0.4.0/tests/fixtures/foo/unicorn_1.1.0.tpl
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/_skel/
+-rw-r--r--   0 joe       (1000) joe       (1000)       91 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/Chart.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)       44 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/package.json
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/
+-rw-r--r--   0 joe       (1000) joe       (1000)       20 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/configmap.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)      523 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)       18 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/service.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)       28 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/spurious.yaml.skel
+-rw-r--r--   0 joe       (1000) joe       (1000)      151 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_skel/values.yaml
+drwxr-xr-x   0 joe       (1000) joe       (1000)        0 2023-06-07 06:12:28.563573 sextant-0.4.0/tests/fixtures/scaffold/_wizard/
+-rw-r--r--   0 joe       (1000) joe       (1000)      427 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_wizard/ingress.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)      287 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_wizard/ingress_nginx.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)     1061 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/_wizard/scaffold.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)       77 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/presets.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)      177 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/fixtures/scaffold/questions.yaml
+-rw-r--r--   0 joe       (1000) joe       (1000)     3269 2023-06-07 06:09:42.000000 sextant-0.4.0/tests/test_cli.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     1120 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_dependency.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     2167 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_module.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     3049 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_package.py
+-rw-r--r--   0 joe       (1000) joe       (1000)     8969 2023-04-19 10:15:44.000000 sextant-0.4.0/tests/test_scaffold.py
+-rw-r--r--   0 joe       (1000) joe       (1000)      814 2023-06-06 05:38:31.000000 sextant-0.4.0/tox.ini
```

### Comparing `sextant-0.3.0/.gitlab-ci.yml` & `sextant-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/LICENSE` & `sextant-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/README.md` & `sextant-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 A tool to compose and manage helm charts from the wikimedia library of template modules.
 
 It offers multiple functions:
 * `sextant [OPTIONS] vendor [-f] CHART_DIR` allows you to generate the vendored modules bundle for your chart, provided you have a package.json in `CHART_DIR`
 * `sextant [OPTIONS] search CHARTS_DIR NAMESPACE.MODULE:VERSION` finds, within a charts collection, all the ones that depend on a specific module
 * `sextant [OPTIONS] update CHARTS_DIR NAMESPACE.MODULE:VERSION...` allows to update the module dependencies for a chart or multiple ones
 * `sextant [OPTIONS] create-chart CHART_DIR [-s SCAFFOLD_DIR]` allows to create a chart based on templates defined in SCAFFOLD_DIR. See below for details
+* `sextant [OPTIONS] update-version CHART_DIR [-v VERSION]` updates a chart version, either to the next patch level, or to the version provided
 
 The available global options are:
 * `--debug` to print out debug information; useful when reporting bugs (there are many)
 * `--modulepath` to indicate where your modules are located; defaults to `./modules` which is ok if you're running from the root of the deployment-charts repository.
 
 ## Installation
```

### Comparing `sextant-0.3.0/setup.py` & `sextant-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/sextant/cli.py` & `sextant-0.4.0/sextant/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import hashlib
 import logging
 import pathlib
 import shutil
 import sys
 from typing import Generator, List, Optional
 
-from sextant import DEPFILE, dependency, log, module, scaffold
+from sextant import DEPFILE, RE_VERSION, dependency, log, module, scaffold
+from sextant.semver import Semver
 
 
 class ChartsCollection:
     """Manages a charts collection"""
 
     def __init__(self, modules_dir: str, charts_dir: str):
         self.registry = module.registry_from_path(modules_dir)
@@ -61,14 +62,15 @@
     """Manages chart vendorization."""
 
     BUNDLE_DIR = "templates/vendor"
 
     def __init__(self, registry: module.Registry, packagefile: pathlib.Path):
         self.registry = registry
         self.chart_dir = packagefile.parent
+        self.chart_yaml = self.chart_dir / "Chart.yaml"
         self.vendor_dir = self.chart_dir / self.BUNDLE_DIR
         self.package = dependency.Package(self.registry, str(packagefile))
 
     @classmethod
     def create(cls, registry: module.Registry, chartdir: str, scaffold_dir: str, presets: Optional[str]) -> "Chart":
         """Create a chart directory."""
         chart_dir = pathlib.Path(chartdir)
@@ -85,35 +87,40 @@
     def create_lock(self, force: bool):
         """Create a lockfile to freeze the dependencies."""
         self.package.lock(force)
 
     def _refresh_package(self):
         self.package = dependency.Package(self.registry, str(self.package.path))
 
-    def vendor(self, force: bool):
+    def vendor(self, force: bool, skip_version_bump: bool = False):
         """Creates a bundle of all modules required by the chart, and saves it
         to a vendor directory."""
+        modified = False
         self.vendor_dir.mkdir(exist_ok=True)
         valid_targets: List[pathlib.Path] = []
         for mod in self.package.get(force):
             target = self.vendor_dir / mod.path.parent.name / mod.path.name
             target.parent.mkdir(exist_ok=True)
             valid_targets.append(target)
             if not force and self._is_fresh(target):
                 log.debug("Not updating module %s as the its file is newer than the lockfile.", mod)
                 continue
             if self._copy_if_changed(mod.path, target):
+                modified = True
                 log.info("Copied %s => %s", mod.path, target)
-            shutil.copy(str(mod.path), str(target))
+
         # Now remove stale files
         for path in self.vendor_dir.glob("**/*.tpl"):
             if path in valid_targets:
                 continue
             log.info("Pruning stale file %s", path)
+            modified = True
             path.unlink()
+        if modified and not skip_version_bump:
+            self.bump_chart_version()
 
     def _is_fresh(self, target: pathlib.Path) -> bool:
         return target.exists() and self.package.lockfile.stat().st_mtime <= target.stat().st_mtime
 
     def _copy_if_changed(self, src: pathlib.Path, dst: pathlib.Path) -> bool:
         if dst.exists():
             src_md5sum = hashlib.md5(src.read_bytes()).hexdigest()
@@ -124,26 +131,48 @@
         shutil.copy(str(src), str(dst))
         return True
 
     def __str__(self) -> str:
         """String representation"""
         return self.chart_dir.name
 
-    def depends_on(self, query: str) -> bool:
+    def depends_on(self, query: str, strict_match: bool = True) -> bool:
         """Checks if the chart depends on a module, directly or indirectly."""
-        for mod in self.package.get():
-            if str(mod) == query:
-                return True
-        return False
+        if strict_match:
+            return any(str(m) == query for m in self.package.get())
+        return any(m.matches(query) for m in self.package.get())
 
     def update_dependency(self, slug: str) -> bool:
         """Update a dependency in package.json."""
         # If the update needs to happen in package.json, or if
         # we have an implicit dependency on it, force a re-vendoring.
-        return self.package.update(slug) or self.depends_on(slug)
+        return self.package.update(slug) or self.depends_on(slug, strict_match=False)
+
+    def bump_chart_version(self, specific_version="") -> Semver:
+        """Bump the chart version after a vendor update."""
+        with self.chart_yaml.open() as yaml:
+            content = yaml.read()
+        match = RE_VERSION.search(content)
+        if not match:
+            raise KeyError(f"Chart version could not be determined from {self.chart_yaml}")
+        if specific_version != "":
+            version = Semver(specific_version)
+            cur_version = Semver(match[2])
+            if version < cur_version:
+                raise ValueError(
+                    f"Chart version is currently '{cur_version}', which is newer than the requested '{version}'"
+                )
+        else:
+            version = Semver(match[2])
+            version.patch += 1
+        content = RE_VERSION.sub(rf"\g<1>{str(version)}", content)
+        with self.chart_yaml.open("w") as yaml:
+            yaml.write(content)
+
+        return version
 
 
 def argparser():
     """Get the argument parser for the command line"""
     parser = argparse.ArgumentParser(prog="sextant", description="Tool to manage template libraries for helm charts")
     parser.add_argument("--modulepath", default="./modules", help="the directory where the modules are located.")
     parser.add_argument("--debug", action="store_true", help="output debug logging.")
@@ -153,14 +182,20 @@
     bundle.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Re-create the lockfile and the bundle even if not necessary.",
     )
     bundle.add_argument(
+        "--no-version-bump",
+        "-b",
+        action="store_true",
+        help="Do not bump the chart version unless strictly necessary.",
+    )
+    bundle.add_argument(
         "chartdir",
         metavar="CHART_DIRECTORY",
         help="the directory where the chart's package.json file is located.",
     )
     # Command 2: search modules in charts
     search = action.add_parser(
         "search",
@@ -185,14 +220,24 @@
     )
     create.add_argument(
         "--scaffold", "-s", help="relative path to the scaffolding template.", default="_scaffold/sextant"
     )
     create.add_argument(
         "--presets", "-p", help="YAML file containing selections of components and answers", default=None
     )
+    # Comand 5: change a chart version
+    chart_version = action.add_parser("update-version", help="Updates the version of a chart")
+    chart_version.add_argument(
+        "--version", "-v", help="Optionally define a specific version to bump the chart to.", default=""
+    )
+    chart_version.add_argument(
+        "chartdir",
+        metavar="CHART_DIRECTORY",
+        help="the directory where the chart's package.json file is located.",
+    )
     return parser
 
 
 def main(args: Optional[List[str]] = None):
     """The main entrypoint."""
 
     if args is None:
@@ -200,15 +245,15 @@
     params = argparser().parse_args(args)
     if params.debug:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO)
 
     what = params.action.replace("-", "_")
-    if what in ["vendor", "create_chart"]:
+    if what in ["vendor", "create_chart", "update_version"]:
         chartsdir = str(pathlib.Path(params.chartdir).parent)
     elif what is not None:
         chartsdir = params.chartdir
 
     charts = ChartsCollection(params.modulepath, chartsdir)
 
     try:
@@ -218,22 +263,22 @@
         log.exception(exc)
         sys.exit(1)
 
 
 def run_vendor(params: argparse.Namespace, charts: ChartsCollection):
     """Vendor dependencies."""
     chart_path = pathlib.Path(params.chartdir)
-    charts.chart(chart_path.name).vendor(params.force)
+    charts.chart(chart_path.name).vendor(params.force, params.no_version_bump)
 
 
 def run_create_chart(params: argparse.Namespace, charts: ChartsCollection):
     """Create a new chart"""
     chart = Chart.create(charts.registry, params.chartdir, params.scaffold, params.presets)
     print(f"Chart {chart} created, now vendoring dependencies.")
-    chart.vendor(False)
+    chart.vendor(False, skip_version_bump=True)
 
 
 def run_search(params: argparse.Namespace, charts: ChartsCollection):
     """Run search"""
     results = charts.query(params.query)
     if not results:
         print(f"The query for {params.query} returned no results.")
@@ -270,7 +315,13 @@
     for chart in charts.charts():
         to_vendor = False
         for slug in updated_modules:
             if chart.update_dependency(slug):
                 to_vendor = True
         if to_vendor:
             chart.vendor(True)
+
+
+def run_update_version(params: argparse.Namespace, charts: ChartsCollection):
+    """Bump chart version."""
+    chart_path = pathlib.Path(params.chartdir)
+    charts.chart(chart_path.name).bump_chart_version(params.version)
```

### Comparing `sextant-0.3.0/sextant/dependency.py` & `sextant-0.4.0/sextant/dependency.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/sextant/module.py` & `sextant-0.4.0/sextant/module.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/sextant/scaffold.py` & `sextant-0.4.0/sextant/scaffold.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/sextant/semver.py` & `sextant-0.4.0/sextant/semver.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/sextant.egg-info/SOURCES.txt` & `sextant-0.4.0/sextant.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 tests/fixtures/bar/stool_0.5.1.tpl
 tests/fixtures/bar/stool_1.0.0.tpl
 tests/fixtures/baz/drunk-unicorn_1.0.0.tpl
 tests/fixtures/baz/module.json
 tests/fixtures/baz/sitting-pangolin_1.0.0.tpl
 tests/fixtures/charts/bad/package.json
 tests/fixtures/charts/bad/templates/.gitkeep
+tests/fixtures/charts/good/Chart.yaml
 tests/fixtures/charts/good/package.json
 tests/fixtures/charts/good/package.lock
 tests/fixtures/charts/good/templates/.gitkeep
 tests/fixtures/charts/other/package.json
 tests/fixtures/charts/other/package.lock
 tests/fixtures/charts/other/templates/.gitkeep
 tests/fixtures/foo/module.json
```

### Comparing `sextant-0.3.0/tests/fixtures/bar/module.json` & `sextant-0.4.0/tests/fixtures/bar/module.json`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel` & `sextant-0.4.0/tests/fixtures/scaffold/_skel/templates/deployment.yaml.skel`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tests/fixtures/scaffold/_wizard/scaffold.yaml` & `sextant-0.4.0/tests/fixtures/scaffold/_wizard/scaffold.yaml`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tests/test_dependency.py` & `sextant-0.4.0/tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tests/test_module.py` & `sextant-0.4.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tests/test_package.py` & `sextant-0.4.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tests/test_scaffold.py` & `sextant-0.4.0/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `sextant-0.3.0/tox.ini` & `sextant-0.4.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tox]
 minversion = 2.5.0
-envlist = py{37,38,39,310}-{style,tests,lint}
+envlist = py{37,38,39,310,311}-{style,tests,lint}
 skip_missing_interpreters = True
 
 [testenv]
 usedevelop = True
 basepython =
     py39: python3.9
     py310: python3.10
+    py311: python3.11
 description =
     style: Style consistency checker
     tests: Run all tests
     py39: (Python 3,9)
     py310: (Python 3,10)
+    py311: (Python 3,11)
 commands =
     lint: mypy  sextant
     lint: pylint --rcfile .pylintrc sextant
     style: flake8
     style: black  --check .
     tests: py.test --strict-markers tests {posargs}
 # Use install_requires and the additional extras_require[tests] from setup.py
@@ -24,8 +26,8 @@
     lint: mypy
     lint: pylint
     lint: types-PyYAML
 
 [flake8]
 max-line-length = 120
 statistics = True
-exclude = .git,build,dist,__pycache__,.tox,.venv,.mypy_cache,.eggs
+exclude = .git,build,dist,__pycache__,.tox,.venv,.mypy_cache,.eggs,.direnv
```

