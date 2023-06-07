# Comparing `tmp/jira2branch-0.1.9.tar.gz` & `tmp/jira2branch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira2branch-0.1.9.tar", last modified: Thu Sep 23 13:35:39 2021, max compression
+gzip compressed data, was "jira2branch-0.2.0.tar", max compression
```

## Comparing `jira2branch-0.1.9.tar` & `jira2branch-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,8 @@
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1833 2021-09-23 13:35:39.155202 jira2branch-0.1.9/PKG-INFO
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1418 2021-09-23 11:13:26.000000 jira2branch-0.1.9/README.md
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/jira2branch/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       74 2021-09-23 13:10:10.000000 jira2branch-0.1.9/jira2branch/__init__.py
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)    10236 2021-09-23 13:35:22.000000 jira2branch-0.1.9/jira2branch/__main__.py
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/jira2branch/tests/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-09 15:20:22.000000 jira2branch-0.1.9/jira2branch/tests/__init__.py
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)      838 2021-09-09 15:18:35.000000 jira2branch-0.1.9/jira2branch/tests/test_main.py
-drwxr-xr-x   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        0 2021-09-23 13:35:39.155202 jira2branch-0.1.9/jira2branch.egg-info/
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1833 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/PKG-INFO
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)      339 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/SOURCES.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)        1 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/dependency_links.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       58 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/entry_points.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       36 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/requires.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       12 2021-09-23 13:35:39.000000 jira2branch-0.1.9/jira2branch.egg-info/top_level.txt
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)       38 2021-09-23 13:35:39.155202 jira2branch-0.1.9/setup.cfg
--rw-r--r--   0 tiagoafpereira  (1000) tiagoafpereira  (1000)     1052 2021-09-23 13:10:10.000000 jira2branch-0.1.9/setup.py
+-rw-r--r--   0        0        0     1070 2023-05-19 17:01:56.796560 jira2branch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1638 2023-05-24 15:25:44.402088 jira2branch-0.2.0/README.md
+-rw-r--r--   0        0        0       75 2023-05-19 17:00:08.394276 jira2branch-0.2.0/jira2branch/__init__.py
+-rw-r--r--   0        0        0    20610 2023-06-07 14:24:28.539445 jira2branch-0.2.0/jira2branch/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:00:08.394276 jira2branch-0.2.0/jira2branch/tests/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-19 17:00:08.394276 jira2branch-0.2.0/jira2branch/tests/test_main.py
+-rw-r--r--   0        0        0      655 2023-06-07 14:25:38.869526 jira2branch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 jira2branch-0.2.0/PKG-INFO
```

### Comparing `jira2branch-0.1.9/PKG-INFO` & `jira2branch-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,46 @@
-Metadata-Version: 2.1
-Name: jira2branch
-Version: 0.1.9
-Summary: Takes a JIRA issue and creates a git branch
-Home-page: UNKNOWN
-Author: Tiago Pereira
-Author-email: tiago.pereira@infraspeak.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
 # JIRA 2 Branch
 
 Takes a JIRA issue and creates a git branch
 
 ```
-Usage: jira2branch [OPTIONS] ISSUE_ID_OR_URL
+Usage: jira2branch [OPTIONS] ISSUE_ID_OR_URL SOURCE_BRANCH
 
   Simple program that takes a JIRA issue ID and creates a new local and
   tracking remote branch
 
 Options:
-  -n, --name-only    Generates the branch name and prints it, no actual branch
-                     will be created (default is False)
-  -p, --push         Push newly created branch to remote (default is False)
-  -t, --target PATH  Target repository (default is current directory)
-  --help             Show this message and exit.
+  -n, --name-only      Generates the branch name and prints it, no actual
+                       branch will be created (default is False)
+  -p, --push           Push newly created branch to remote (default is False)
+  -t, --target PATH    Target repository (default is current directory)
+  -r, --merge-request  Create merge request. Requires --push. (default is
+                       False)
+  --help               Show this message and exit.
 ```
 
 - Branch naming format is as follows:
   - {CONVENTIONAL_COMMIT_PREFIX}/{ISSUE_ID}_{ISSUE_TITLE}
 
 ## Requirements
 
 Requires Python 3.8
 
 ### Dev env
 
 ```
-pip install pipenv
-pipenv install
-virtualenv venv
-. venv/bin/activate
-pip install --editable .
+pip install poetry
+poetry install
+pip install dist/jira2branch-[VERSION]-py3-none-any.whl
 ```
 
 Afterwards, your command should be available:
 
 ```
-$ jira2branch WT3-227
+$ jira2branch WT3-227 develop
 fix/WT3-227_some-jira-issue
 ```
 
 ### Credentials
 
 JIRA credentials will be fetched from `[USER HOME]/.j2b/secrets.ini` with the following format:
 
@@ -64,24 +50,24 @@
 # url = 
 # email = 
 # username = 
 # password = 
 # token = 
 ```
 
+WIP: GitLab credentials will also be required for automatic MR creation
+
 #### Required fields
 
 `url` and `email` are required.
 
 Use either `username` + `password` or `token` depending on how access is configured
 
 ## Usage
 
 `python main.py [JIRA_ISSUE_ID|JIRA_ISSUE_URL]`
 
 ### Examples
 
-`python main.py WT3-227`
-
-`python main.py https://company.atlassian.net/browse/WT3-227`
-
+`python main.py WT3-227 develop`
 
+`python main.py https://company.atlassian.net/browse/WT3-227 develop`
```

