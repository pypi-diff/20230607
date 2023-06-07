# Comparing `tmp/datawrapper-0.5.2.tar.gz` & `tmp/datawrapper-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawrapper-0.5.2.tar", last modified: Wed May 31 22:45:01 2023, max compression
+gzip compressed data, was "datawrapper-0.5.3.tar", last modified: Wed Jun  7 21:31:49 2023, max compression
```

## Comparing `datawrapper-0.5.2.tar` & `datawrapper-0.5.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/.stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-31 22:44:48.000000 datawrapper-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-31 22:44:48.000000 datawrapper-0.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-31 22:44:48.000000 datawrapper-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-31 22:44:48.000000 datawrapper-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-31 22:45:01.277543 datawrapper-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 22:44:48.000000 datawrapper-0.5.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    66724 2023-05-31 22:44:48.000000 datawrapper-0.5.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-31 22:44:48.000000 datawrapper-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-31 22:44:48.000000 datawrapper-0.5.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/datawrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 22:44:48.000000 datawrapper-0.5.2/datawrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-31 22:44:48.000000 datawrapper-0.5.2/datawrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 22:44:48.000000 datawrapper-0.5.2/datawrapper/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/datawrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 22:45:01.000000 datawrapper-0.5.2/datawrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/_templates/class.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.273543 datawrapper-0.5.2/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/about/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/static/datawrapper_logo_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/static/datawrapper_logo_light_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/user-guide/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-05-31 22:44:48.000000 datawrapper-0.5.2/docs/user-guide/usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 22:45:01.277543 datawrapper-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-31 22:44:48.000000 datawrapper-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.269543 datawrapper-0.5.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:45:01.277543 datawrapper-0.5.2/tests/test_example/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 22:44:48.000000 datawrapper-0.5.2/tests/test_example/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.669709 datawrapper-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/.stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.669709 datawrapper-0.5.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.669709 datawrapper-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-07 21:31:26.000000 datawrapper-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-07 21:31:26.000000 datawrapper-0.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 21:31:26.000000 datawrapper-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-07 21:31:26.000000 datawrapper-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-07 21:31:49.673709 datawrapper-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 21:31:26.000000 datawrapper-0.5.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    67524 2023-06-07 21:31:26.000000 datawrapper-0.5.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-07 21:31:26.000000 datawrapper-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-07 21:31:26.000000 datawrapper-0.5.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.669709 datawrapper-0.5.3/datawrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-07 21:31:26.000000 datawrapper-0.5.3/datawrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23736 2023-06-07 21:31:26.000000 datawrapper-0.5.3/datawrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-07 21:31:26.000000 datawrapper-0.5.3/datawrapper/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.669709 datawrapper-0.5.3/datawrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-07 21:31:49.000000 datawrapper-0.5.3/datawrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-07 21:31:49.000000 datawrapper-0.5.3/datawrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:31:49.000000 datawrapper-0.5.3/datawrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 21:31:49.000000 datawrapper-0.5.3/datawrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 21:31:49.000000 datawrapper-0.5.3/datawrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/_templates/class.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/about/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/about/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/about/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/about/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/static/datawrapper_logo_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/static/datawrapper_logo_light_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/user-guide/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-06-07 21:31:26.000000 datawrapper-0.5.3/docs/user-guide/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 21:31:49.673709 datawrapper-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-07 21:31:26.000000 datawrapper-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.669709 datawrapper-0.5.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:31:49.673709 datawrapper-0.5.3/tests/test_example/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-07 21:31:26.000000 datawrapper-0.5.3/tests/test_example/test_hello.py
```

### Comparing `datawrapper-0.5.2/.github/.stale.yml` & `datawrapper-0.5.3/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `datawrapper-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `datawrapper-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/.github/PULL_REQUEST_TEMPLATE.md` & `datawrapper-0.5.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/.github/dependabot.yml` & `datawrapper-0.5.3/.github/dependabot.yml`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,37 @@
 
 version: 2
 
 updates:
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
-      interval: "daily"
+      interval: "weekly"
     allow:
       - dependency-type: "all"
+    ignore:
+      - dependency-name: "*"
+        update-types:
+          ["version-update:semver-patch", "version-update:semver-minor"]
     commit-message:
       prefix: ":arrow_up:"
-    open-pull-requests-limit: 50
+    open-pull-requests-limit: 5
 
   - package-ecosystem: "github-actions"
     directory: "/"
     schedule:
-      interval: "daily"
+      interval: "weekly"
     allow:
       - dependency-type: "all"
     commit-message:
       prefix: ":arrow_up:"
-    open-pull-requests-limit: 50
+    open-pull-requests-limit: 5
 
   - package-ecosystem: "docker"
     directory: "/docker"
     schedule:
       interval: "weekly"
     allow:
       - dependency-type: "all"
     commit-message:
       prefix: ":arrow_up:"
-    open-pull-requests-limit: 50
+    open-pull-requests-limit: 5
```

### Comparing `datawrapper-0.5.2/.github/workflows/continuous-deployment.yml` & `datawrapper-0.5.3/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/.gitignore` & `datawrapper-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/.pre-commit-config.yaml` & `datawrapper-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/CODE_OF_CONDUCT.md` & `datawrapper-0.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/LICENSE` & `datawrapper-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/PKG-INFO` & `datawrapper-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawrapper
-Version: 0.5.2
+Version: 0.5.3
 Summary: A light-weight python wrapper for the Datawrapper API
 Home-page: https://github.com/chekos/datawrapper
 Author: chekos
 Author-email: chekos@tacosdedatos.com
 License: MIT
 Project-URL: Maintainer, https://github.com/chekos/
 Project-URL: Source, https://github.com/chekos/datawrapper
```

### Comparing `datawrapper-0.5.2/Pipfile.lock` & `datawrapper-0.5.3/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973118279569894%*

 * *Differences: {"'develop'": "{'coverage': {'hashes': "*

 * *              "['sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f', "*

 * *              "'sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2', "*

 * *              "'sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a', "*

 * *              "'sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a', "*

 * *              "'sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01', "*

 * *           […]*

```diff
@@ -578,108 +578,117 @@
             "version": "==3.1.0"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
-                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
-                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
-                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
-                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
-                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
-                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
-                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
-                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
-                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
-                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
-                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
-                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
-                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
-                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
-                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
-                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
-                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
-                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
-                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
-                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
-                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
-                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
-                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
-                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
-                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
-                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
-                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
-                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
-                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
-                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
-                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
-                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
-                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
-                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
-                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
-                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
-                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
-                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
-                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
-                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
-                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
-                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
-                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
-                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
-                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
-                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
-                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
-                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
-                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
-                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.5"
+            "version": "==7.2.7"
         },
         "cryptography": {
             "hashes": [
-                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
-                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
-                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
-                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
-                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
-                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
-                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
-                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
-                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
-                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
-                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
-                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
-                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
-                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
-                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
-                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
-                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
-                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
-                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==40.0.2"
+            "index": "pypi",
+            "version": "==41.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
-                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.20"
+            "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
@@ -1048,19 +1057,19 @@
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==3.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
-                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.7.2"
+            "version": "==67.8.0"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
                 "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
@@ -1110,19 +1119,19 @@
                 "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
                 "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
             ],
             "version": "==1.26.25.13"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c",
+                "sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.5.0"
+            "version": "==4.6.2"
         },
         "urllib3": {
             "hashes": [
                 "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
                 "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `datawrapper-0.5.2/README.md` & `datawrapper-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/SECURITY.md` & `datawrapper-0.5.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/datawrapper/__init__.py` & `datawrapper-0.5.3/datawrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/datawrapper/__main__.py` & `datawrapper-0.5.3/datawrapper/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
     def create_chart(
         self,
         title: str = "New Chart",
         chart_type: str = "d3-bars-stacked",
         data: Union[pd.DataFrame, None] = None,
         folder_id: str = "",
+        organization_id: str = "",
         metadata: Optional[Dict[Any, Any]] = None,
     ) -> Union[Dict[Any, Any], None, Any]:
         """Creates a new Datawrapper chart, table or map.
 
         You can pass a pandas DataFrame as a `data` argument to upload data.
 
         Returns the created chart's information.
@@ -143,14 +144,16 @@
             Title for new chart, table or map, by default "New Chart"
         chart_type : str, optional
             Chart type to be created. See https://developer.datawrapper.de/docs/chart-types, by default "d3-bars-stacked"
         data : [type], optional
             A pandas DataFrame containing the data to be added, by default None
         folder_id : str, optional
             ID of folder in Datawrapper.de for the chart, table or map to be created in, by default ""
+        organization_id : str, optional
+            ID of the team where the chart should be created. The authenticated user must have access to this team.
         metadata: dict, optional
             A Python dictionary of properties to add.
 
         Returns
         -------
         dict
             A dictionary containing the created chart's information.
@@ -159,14 +162,16 @@
         _header = self._auth_header
         _header["content-type"] = "application/json"
 
         _data = {"title": title, "type": chart_type}
 
         if folder_id:
             _data["folderId"] = folder_id
+        if organization_id:
+            _data["organizationId"] = organization_id
         if metadata:
             _data["metadata"] = metadata  # type: ignore
 
         new_chart_response = r.post(
             url=self._CHARTS_URL, headers=_header, data=json.dumps(_data)
         )
 
@@ -632,16 +637,17 @@
     def get_charts(
         self,
         user_id: str = "",
         published: str = "true",
         search: str = "",
         order: str = "DESC",
         order_by: str = "createdAt",
-        folder_id: str = "",
         limit: int = 25,
+        folder_id: str = "",
+        team_id: str = "",
     ) -> Union[None, List[Any]]:
         """Retrieves a list of charts by User
 
         Parameters
         ----------
         user_id : str, optional
             ID of the user to fetch charts for, by default ""
@@ -649,18 +655,20 @@
             Flag to filter resutls by publish status, by default "true"
         search : str, optional
             Search for charts with a specific title, by default ""
         order : str, optional
             Result order (ascending or descending), by default "DESC"
         order_by : str, optional
             Attribute to order by. One of createdAt, email, id, or name, by default "createdAt"
-        folder_id: str, optional
-            ID of the folder to search charts in, by default ""
         limit : int, optional
             Maximum items to fetch, by default 25
+        folder_id : str, optional
+            ID of folder in Datawrapper.de where to list charts, by default ""
+        team_id : str, optional
+            ID of the team where to list charts. The authenticated user must have access to this team, by default ""
 
         Returns
         -------
         list
             List of charts.
         """
 
@@ -674,18 +682,20 @@
             _query["published"] = published
         if search:
             _query["search"] = search
         if order:
             _query["order"] = order
         if order_by:
             _query["orderBy"] = order_by
-        if folder_id:
-            _query["folderId"] = folder_id
         if limit:
             _query["limit"] = str(limit)
+        if folder_id:
+            _query["folderId"] = folder_id
+        if team_id:
+            _query["teamId"] = team_id
 
         get_charts_response = r.get(url=_url, headers=_header, params=_query)
 
         if get_charts_response.status_code == 200:
             return get_charts_response.json()["list"]  # type: ignore
         else:
             logger.error("Could not retrieve charts at this moment.")
```

### Comparing `datawrapper-0.5.2/datawrapper.egg-info/PKG-INFO` & `datawrapper-0.5.3/datawrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawrapper
-Version: 0.5.2
+Version: 0.5.3
 Summary: A light-weight python wrapper for the Datawrapper API
 Home-page: https://github.com/chekos/datawrapper
 Author: chekos
 Author-email: chekos@tacosdedatos.com
 License: MIT
 Project-URL: Maintainer, https://github.com/chekos/
 Project-URL: Source, https://github.com/chekos/datawrapper
```

### Comparing `datawrapper-0.5.2/datawrapper.egg-info/SOURCES.txt` & `datawrapper-0.5.3/datawrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/Makefile` & `datawrapper-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/conf.py` & `datawrapper-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/make.bat` & `datawrapper-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/static/datawrapper_logo_light.png` & `datawrapper-0.5.3/docs/static/datawrapper_logo_light.png`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/static/datawrapper_logo_light_small.png` & `datawrapper-0.5.3/docs/static/datawrapper_logo_light_small.png`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/user-guide/installation.md` & `datawrapper-0.5.3/docs/user-guide/installation.md`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/docs/user-guide/usage.ipynb` & `datawrapper-0.5.3/docs/user-guide/usage.ipynb`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/setup.py` & `datawrapper-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `datawrapper-0.5.2/tests/test_example/test_hello.py` & `datawrapper-0.5.3/tests/test_example/test_hello.py`

 * *Files identical despite different names*

