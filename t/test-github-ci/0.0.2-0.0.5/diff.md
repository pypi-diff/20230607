# Comparing `tmp/test-github-ci-0.0.2.tar.gz` & `tmp/test_github_ci-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-github-ci-0.0.2.tar", last modified: Fri Aug 21 08:10:49 2020, max compression
+gzip compressed data, was "test_github_ci-0.0.5.tar", max compression
```

## Comparing `test-github-ci-0.0.2.tar` & `test_github_ci-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      441 2020-08-21 08:10:27.273435 test-github-ci-0.0.2/README.md
--rw-r--r--   0        0        0      612 2020-08-21 08:10:46.949275 test-github-ci-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2020-08-21 08:10:46.981275 test-github-ci-0.0.2/test_github_ci/__init__.py
--rw-r--r--   0        0        0       38 2020-08-21 08:10:27.273435 test-github-ci-0.0.2/test_github_ci/hello.py
--rw-r--r--   0        0        0     1117 2020-08-21 08:10:49.985066 test-github-ci-0.0.2/setup.py
--rw-r--r--   0        0        0      827 2020-08-21 08:10:49.985338 test-github-ci-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      441 2023-06-07 12:04:37.749439 test_github_ci-0.0.5/README.md
+-rw-r--r--   0        0        0      612 2023-06-07 12:05:01.491419 test_github_ci-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-07 12:05:01.491419 test_github_ci-0.0.5/test_github_ci/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-07 12:04:37.749439 test_github_ci-0.0.5/test_github_ci/hello.py
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 test_github_ci-0.0.5/PKG-INFO
```

### Comparing `test-github-ci-0.0.2/pyproject.toml` & `test_github_ci-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-github-ci"
-version = "0.0.2"
+version = "0.0.5"
 description = "This project tests AutoPub with GitHub Actions CI."
 authors = ["BotPub <botpub@autopub.rocks>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `test-github-ci-0.0.2/PKG-INFO` & `test_github_ci-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: test-github-ci
-Version: 0.0.2
+Version: 0.0.5
 Summary: This project tests AutoPub with GitHub Actions CI.
 Author: BotPub
 Author-email: botpub@autopub.rocks
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Test AutoPub & GitHub Actions CI
 
 1. Create repository
 1. Create GitHub and PyPI tokens with appropriate scopes
 1. Add `GH_TOKEN` & `PYPI_PASSWORD` environment variables via repository Settings > Secrets > New secret
```

