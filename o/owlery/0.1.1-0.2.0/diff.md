# Comparing `tmp/owlery-0.1.1.tar.gz` & `tmp/owlery-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlery-0.1.1.tar", last modified: Mon May  8 08:18:03 2023, max compression
+gzip compressed data, was "owlery-0.2.0.tar", last modified: Wed Jun  7 07:08:32 2023, max compression
```

## Comparing `owlery-0.1.1.tar` & `owlery-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,111 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.206782 owlery-0.1.1/
--rw-r--r--   0 michael   (1000) michael   (1000)      143 2023-04-25 07:47:50.000000 owlery-0.1.1/.dockerignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.185782 owlery-0.1.1/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-04-18 12:37:28.000000 owlery-0.1.1/.github/FUNDING.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.187782 owlery-0.1.1/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)      778 2023-05-08 08:10:35.000000 owlery-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      431 2023-04-21 14:13:56.000000 owlery-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-04-21 15:01:49.000000 owlery-0.1.1/.github/workflows/release.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.187782 owlery-0.1.1/.github/workflows/scripts/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1289 2023-04-28 15:25:18.000000 owlery-0.1.1/.github/workflows/scripts/release.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3512 2023-05-06 19:52:58.000000 owlery-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2821 2023-04-18 12:37:44.000000 owlery-0.1.1/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)     1139 2023-05-08 08:10:35.000000 owlery-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      352 2023-04-18 12:37:56.000000 owlery-0.1.1/.readthedocs.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.188782 owlery-0.1.1/.vscode/
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-04-18 12:37:22.000000 owlery-0.1.1/.vscode/settings.json
--rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-05-08 08:14:47.000000 owlery-0.1.1/CHANGELOG.md
--rw-r--r--   0 michael   (1000) michael   (1000)     4718 2023-05-03 13:58:29.000000 owlery-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2179 2023-05-03 09:31:49.000000 owlery-0.1.1/Dockerfile
--rw-r--r--   0 michael   (1000) michael   (1000)     1084 2023-05-08 08:10:35.000000 owlery-0.1.1/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-04-28 15:42:34.000000 owlery-0.1.1/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     1783 2023-05-08 08:18:03.206782 owlery-0.1.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      640 2023-05-08 08:10:35.000000 owlery-0.1.1/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.188782 owlery-0.1.1/changelog.d/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-20 10:32:20.000000 owlery-0.1.1/changelog.d/.gitkeep
--rw-r--r--   0 michael   (1000) michael   (1000)      309 2023-04-20 10:48:15.000000 owlery-0.1.1/changelog.d/template.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.188782 owlery-0.1.1/dev/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-04-28 15:47:21.000000 owlery-0.1.1/dev/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      694 2023-05-08 08:10:35.000000 owlery-0.1.1/docker-compose.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.194782 owlery-0.1.1/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-04-21 11:36:10.000000 owlery-0.1.1/docs/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/api.rst
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-04-21 11:36:10.000000 owlery-0.1.1/docs/changelog.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     4252 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-03 13:19:39.000000 owlery-0.1.1/docs/contributing.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     4247 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/getting-started.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      929 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/installation.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/license.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-04-21 11:36:10.000000 owlery-0.1.1/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-03 09:30:10.000000 owlery-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.194782 owlery-0.1.1/docs/services/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.196782 owlery-0.1.1/docs/services/email/
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/services/email/imap.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3288 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/services/email/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/services/email/pop3.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      195 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/services/email/smtp.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/services/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     2516 2023-05-08 08:10:35.000000 owlery-0.1.1/docs/signals.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-05-06 19:52:58.000000 owlery-0.1.1/docs/spelling-wordlist.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      552 2023-05-08 08:10:35.000000 owlery-0.1.1/dovecot.conf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.197782 owlery-0.1.1/owlery/
--rw-r--r--   0 michael   (1000) michael   (1000)      398 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      160 2023-05-08 08:18:02.000000 owlery-0.1.1/owlery/_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2884 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-19 10:58:50.000000 owlery-0.1.1/owlery/py.typed
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.200782 owlery-0.1.1/owlery/services/
--rw-r--r--   0 michael   (1000) michael   (1000)    14295 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/services/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.201782 owlery-0.1.1/owlery/services/email/
--rw-r--r--   0 michael   (1000) michael   (1000)    11950 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/services/email/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2729 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/services/email/imap.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2543 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/services/email/pop3.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2233 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/services/email/smtp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1836 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/services/misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      286 2023-05-08 08:10:35.000000 owlery-0.1.1/owlery/signals.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.199782 owlery-0.1.1/owlery.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1783 2023-05-08 08:18:03.000000 owlery-0.1.1/owlery.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1627 2023-05-08 08:18:03.000000 owlery-0.1.1/owlery.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-08 08:18:03.000000 owlery-0.1.1/owlery.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       43 2023-05-08 08:18:03.000000 owlery-0.1.1/owlery.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      422 2023-05-08 08:18:03.000000 owlery-0.1.1/owlery.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-05-08 08:18:03.000000 owlery-0.1.1/owlery.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4489 2023-05-08 08:10:35.000000 owlery-0.1.1/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       97 2023-05-02 08:27:39.000000 owlery-0.1.1/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-08 08:18:03.206782 owlery-0.1.1/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.203782 owlery-0.1.1/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-01 18:19:10.000000 owlery-0.1.1/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      576 2023-04-28 15:42:52.000000 owlery-0.1.1/tests/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)       87 2023-05-03 14:44:26.000000 owlery-0.1.1/tests/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.203782 owlery-0.1.1/tests/services/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-01 18:19:10.000000 owlery-0.1.1/tests/services/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.205782 owlery-0.1.1/tests/services/email/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-01 18:19:10.000000 owlery-0.1.1/tests/services/email/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      123 2023-05-01 18:19:10.000000 owlery-0.1.1/tests/services/email/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2540 2023-05-08 08:10:35.000000 owlery-0.1.1/tests/services/email/test_imap.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2535 2023-05-08 08:10:35.000000 owlery-0.1.1/tests/services/email/test_pop3.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1433 2023-05-08 08:10:35.000000 owlery-0.1.1/tests/services/email/test_smtp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1333 2023-05-08 08:10:35.000000 owlery-0.1.1/tests/services/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1859 2023-05-08 08:10:35.000000 owlery-0.1.1/tests/test_signals.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1918 2023-05-06 19:52:58.000000 owlery-0.1.1/tox.ini
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 08:18:03.205782 owlery-0.1.1/typing/
--rw-r--r--   0 michael   (1000) michael   (1000)       62 2023-04-20 12:31:13.000000 owlery-0.1.1/typing/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      143 2023-05-07 18:40:41.000000 owlery-0.2.0/.dockerignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/FUNDING.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)      762 2023-05-11 17:05:09.000000 owlery-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      431 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/workflows/release.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.github/workflows/scripts/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1289 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/workflows/scripts/release.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2750 2023-06-07 07:00:18.000000 owlery-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2821 2023-05-07 18:40:41.000000 owlery-0.2.0/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)     1139 2023-05-07 18:40:41.000000 owlery-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      352 2023-05-07 18:40:41.000000 owlery-0.2.0/.readthedocs.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.vscode/
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-05-07 18:40:41.000000 owlery-0.2.0/.vscode/settings.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      996 2023-06-07 07:05:35.000000 owlery-0.2.0/CHANGELOG.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     4718 2023-05-07 18:40:41.000000 owlery-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2179 2023-05-07 18:40:41.000000 owlery-0.2.0/Dockerfile
+-rw-r--r--   0 michael   (1000) michael   (1000)     1084 2023-05-07 18:40:41.000000 owlery-0.2.0/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-07 18:40:41.000000 owlery-0.2.0/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     1840 2023-06-07 07:08:32.166276 owlery-0.2.0/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      697 2023-06-06 22:32:50.000000 owlery-0.2.0/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/changelog.d/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/changelog.d/.gitkeep
+-rw-r--r--   0 michael   (1000) michael   (1000)      309 2023-05-07 18:40:41.000000 owlery-0.2.0/changelog.d/template.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/dev/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-07 18:40:41.000000 owlery-0.2.0/dev/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-06-07 07:07:49.000000 owlery-0.2.0/docker-compose.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-06-07 07:07:49.000000 owlery-0.2.0/docs/api.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/changelog.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     4252 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/contributing.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     4247 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/getting-started.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      929 2023-06-07 07:07:49.000000 owlery-0.2.0/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/installation.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/integrations/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3591 2023-05-13 13:03:59.000000 owlery-0.2.0/docs/integrations/flask.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-05-07 19:55:42.000000 owlery-0.2.0/docs/license.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/make.bat
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/recipes/
+-rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-05-13 07:31:46.000000 owlery-0.2.0/docs/recipes/celery.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-13 12:58:30.000000 owlery-0.2.0/docs/recipes/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-06-06 21:59:54.000000 owlery-0.2.0/docs/recipes/rq.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/services/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/services/email/
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/email/imap.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3288 2023-05-07 20:01:11.000000 owlery-0.2.0/docs/services/email/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/email/pop3.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      195 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/email/smtp.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3624 2023-06-06 22:32:50.000000 owlery-0.2.0/docs/signals.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/spelling-wordlist.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-06-07 06:25:49.000000 owlery-0.2.0/dovecot.conf
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/
+-rw-r--r--   0 michael   (1000) michael   (1000)      398 2023-05-07 18:40:41.000000 owlery-0.2.0/owlery/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      160 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery/_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2962 2023-05-11 17:05:09.000000 owlery-0.2.0/owlery/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/owlery/py.typed
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/
+-rw-r--r--   0 michael   (1000) michael   (1000)    20845 2023-06-07 06:48:04.000000 owlery-0.2.0/owlery/services/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/email/
+-rw-r--r--   0 michael   (1000) michael   (1000)    16763 2023-06-07 06:56:34.000000 owlery-0.2.0/owlery/services/email/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2812 2023-06-07 06:41:44.000000 owlery-0.2.0/owlery/services/email/imap.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2673 2023-06-07 06:59:11.000000 owlery-0.2.0/owlery/services/email/pop3.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2644 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/email/smtp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1907 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/misc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/mms/
+-rw-r--r--   0 michael   (1000) michael   (1000)     4341 2023-06-07 06:59:57.000000 owlery-0.2.0/owlery/services/mms/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3090 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/mms/twilio.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/sms/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3882 2023-06-07 06:48:04.000000 owlery-0.2.0/owlery/services/sms/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2551 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/sms/twilio.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1614 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/twilio.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/whatsapp/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5366 2023-06-07 06:59:57.000000 owlery-0.2.0/owlery/services/whatsapp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3955 2023-06-07 07:05:29.000000 owlery-0.2.0/owlery/services/whatsapp/twilio.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/signals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-05-13 12:55:55.000000 owlery-0.2.0/owlery/utils.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1840 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     2022 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       43 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      422 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4489 2023-05-07 19:41:49.000000 owlery-0.2.0/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       97 2023-06-06 22:32:50.000000 owlery-0.2.0/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-07 07:08:32.166276 owlery-0.2.0/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      576 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       87 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/tests/services/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/services/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/tests/services/email/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/services/email/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      123 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/services/email/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3259 2023-06-07 06:47:46.000000 owlery-0.2.0/tests/services/email/test_imap.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3384 2023-06-07 06:47:54.000000 owlery-0.2.0/tests/services/email/test_pop3.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2413 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/email/test_smtp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9564 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/test_manager.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1191 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/test_service.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/test_signals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1918 2023-05-07 18:40:41.000000 owlery-0.2.0/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/typing/
+-rw-r--r--   0 michael   (1000) michael   (1000)       62 2023-05-07 18:40:41.000000 owlery-0.2.0/typing/requirements.txt
```

### Comparing `owlery-0.1.1/.github/workflows/docs.yml` & `owlery-0.2.0/.github/workflows/docs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 name: Check documentation
 on:
-  pull_request:
   workflow_call:
 
 jobs:
   docs:
     name: Run documentation tests
     runs-on: ubuntu-latest
     steps:
```

### Comparing `owlery-0.1.1/.github/workflows/scripts/release.py` & `owlery-0.2.0/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/.github/workflows/tests.yml` & `owlery-0.2.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: Run tests
 on:
   pull_request:
-  workflow_dispatch:
+  push:
 
 jobs:
   docs:
     name: Run documentation tests
     uses: ./.github/workflows/docs.yml
   style:
     name: Run linting and style checks
@@ -60,19 +60,18 @@
           python -m pip install -r tests/requirements.txt
           python -m pip install .
           python -m pip install tox-gh-actions
       - name: Setup test suite
         run: tox r -e py${{ matrix.python }} -vv --notest
       - name: Run test suite
         run: tox r -e py${{ matrix.python }} --skip-pkg-install
-      - name: Store code coverage
-        uses: actions/upload-artifact@v3
-        with:
-          name: coverage
-          path: .coverage
+      - name: Publish coveralls.io
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        run: tox r -e coveralls --skip-pkg-install
   typing:
     name: Run typing checks
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python 3.11
         uses: actions/setup-python@v4
@@ -83,31 +82,7 @@
           python -m pip install --upgrade pip setuptools wheel
           python -m pip install -r typing/requirements.txt
           python -m pip install tox tox-gh-actions
       - name: Setup typing checks
         run: tox r -e typing -vv --notest
       - name: Run typing checks
         run: tox r -e typing --skip-pkg-install
-  finish:
-    name: Publish coverage
-    needs: tests
-    if: ${{ always() }}
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - name: Setup Python 3.11
-        uses: actions/setup-python@v4
-        with:
-          python-version: '3.11'
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip setuptools wheel
-          python -m pip install -r typing/requirements.txt
-          python -m pip install tox tox-gh-actions
-      - name: Download code coverage
-        uses: actions/download-artifact@v3
-        with:
-          name: coverage
-      - name: Publish coveralls.io
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        run: tox r -e coveralls --skip-pkg-install
```

### Comparing `owlery-0.1.1/.gitignore` & `owlery-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/.pre-commit-config.yaml` & `owlery-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/.vscode/settings.json` & `owlery-0.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/CHANGELOG.md` & `owlery-0.2.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,30 @@
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [towncrier](https://towncrier.readthedocs.io/) and the changes for the upcoming release can be found
 in the ``changelog.d/`` folder.
 
 <!-- towncrier release notes start -->
 
+## [0.2.0](https://github.com/COUR4G3/owlery/tree/0.2.0) - 2023-06-07
+
+
+### Features
+
+- Set message status on send, and store exception on error.
+- Support for SMS text, MMS multimedia and WhatsApp messages.
+- Added Twilio as a provider (for SMS, MMS and WhatsApp).
+
+
+### Fixed
+
+- Various fixes to services.
+- Fixed documentation and tests.
+
+
 ## [0.1.1](https://github.com/COUR4G3/owlery/tree/0.1.1) - 2023-05-08
 
 
 ### Fixed
 
 - Fixed documentation and tests.
```

### Comparing `owlery-0.1.1/CONTRIBUTING.md` & `owlery-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/Dockerfile` & `owlery-0.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/LICENSE` & `owlery-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/PKG-INFO` & `owlery-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlery
-Version: 0.1.1
+Version: 0.2.0
 Summary: Uniform messaging service for Python applications.
 Author-email: Michael de Villiers <michael@devilears.co.za>
 Maintainer-email: Michael de Villiers <michael@devilears.co.za>
 License: MIT
 Project-URL: Homepage, https://github.com/COUR4G3/owlery/
 Project-URL: Documentation, https://owlery-messaging.readthedocs.io/
 Project-URL: Changes, https://owlery-messaging.readthedocs.io/en/latest/changelog.html
@@ -25,17 +25,18 @@
 Provides-Extra: tests
 Provides-Extra: typing
 License-File: LICENSE
 
 Owlery
 ======
 
-Uniform messaging service for Python applications supporting a variety of messaging services and vendors, allowing easy
-substitution and drop-in of services and vendors during runtime, configuration, development cycle or application
-evolution - even sending different messages through different vendors based on rules.
+Uniform messaging service supporting a variety of messaging services and vendors easily integrated with your Python
+applications or usable from your command-line, allowing easy substitution and drop-in of services and vendors during
+runtime, configuration, development cycle or application evolution - even sending different messages through different
+vendors based on rules.
 
 
 ## Links
 
 - Documentation: <https://owlery-messaging.readthedocs.io/>
 - Changes: <https://owlery-messaging.readthedocs.io/en/latest/changes.html>
 - Releases: <https://pypi.org/project/owlery/>
```

### Comparing `owlery-0.1.1/README.md` & `owlery-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Owlery
 ======
 
-Uniform messaging service for Python applications supporting a variety of messaging services and vendors, allowing easy
-substitution and drop-in of services and vendors during runtime, configuration, development cycle or application
-evolution - even sending different messages through different vendors based on rules.
+Uniform messaging service supporting a variety of messaging services and vendors easily integrated with your Python
+applications or usable from your command-line, allowing easy substitution and drop-in of services and vendors during
+runtime, configuration, development cycle or application evolution - even sending different messages through different
+vendors based on rules.
 
 
 ## Links
 
 - Documentation: <https://owlery-messaging.readthedocs.io/>
 - Changes: <https://owlery-messaging.readthedocs.io/en/latest/changes.html>
 - Releases: <https://pypi.org/project/owlery/>
```

### Comparing `owlery-0.1.1/docker-compose.yml` & `owlery-0.2.0/docker-compose.yml`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     volumes:
       - ./:/opt/owlery
     restart: unless-stopped
   imap:
     image: dovecot/dovecot:latest
     ports:
       - 143:143
+      - 465:465
+      - 587:587
       - 993:993
     volumes:
       - ./dovecot.conf:/etc/dovecot/dovecot.conf:ro
     restart: unless-stopped
   pop3:
     image: dovecot/dovecot:latest
     ports:
```

### Comparing `owlery-0.1.1/docs/Makefile` & `owlery-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/docs/conf.py` & `owlery-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/docs/getting-started.rst` & `owlery-0.2.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/docs/index.rst` & `owlery-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/docs/installation.rst` & `owlery-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/docs/make.bat` & `owlery-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/docs/services/email/index.rst` & `owlery-0.2.0/docs/services/email/index.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/owlery/exceptions.py` & `owlery-0.2.0/owlery/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,38 +64,44 @@
         super().__init__(exc_info, exc_info=exc_info)
 
 
 class ServiceNotRegistered(OwleryException):
     """Service not registered on a service manager."""
 
     def __init__(self, name: t.Optional[str] = None):
+        self.name = name
+
         if name:
             description = f"Service '{name}' not registered on this manager"
         else:
             description = "No service registered on this manager"
 
         super().__init__(description, name)
 
 
 class ServiceReceiveCapabilityError(OwleryException):
     """Service cannot receive messages."""
 
     def __init__(self, name: t.Optional[str] = None):
+        self.name = name
+
         if name:
             description = f"Service '{name}' cannot receive messages"
         else:
             description = "No service registered to receive on this manager"
 
         super().__init__(description, name)
 
 
 class ServiceSendCapabilityError(OwleryException):
     """Service cannot send messages."""
 
     def __init__(self, name: t.Optional[str] = None):
+        self.name = name
+
         if name:
             description = f"Service '{name}' cannot send messages"
         else:
             description = "No service registered to send on this manager"
 
         super().__init__(description, name)
```

### Comparing `owlery-0.1.1/owlery/services/__init__.py` & `owlery-0.2.0/owlery/services/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import dataclasses
+import datetime as dt
+import logging
 import platform
 import random
 import typing as t
 
-from collections import UserList
+from collections import UserDict, UserList
 from contextlib import contextmanager
 
 from .. import __version__
 from ..exceptions import (
     ServiceNotRegistered,
     ServiceReceiveCapabilityError,
     ServiceSendCapabilityError,
 )
 from ..signals import (
     on_after_send,
     on_before_send,
     on_close_session,
     on_open_session,
     on_receive_message,
+    on_receive_status_callback,
+    on_register_service,
+    on_unregister_service,
 )
 
 USER_AGENT = (
     f"owlery/{__version__} "
     f"{platform.python_implementation()}/{platform.python_version()}"
 )
 
@@ -36,156 +41,306 @@
 
     """
 
     data: t.Union[bytes, t.IO[bytes]]
     mimetype: str = "application/octet-stream"
 
 
+MessageStatus = t.Literal[
+    "draft",
+    "queued",
+    "sent",
+    "received",
+    "read",
+    "cancelled",
+    "error",
+]
+
+
 @dataclasses.dataclass
 class Message:
-    """A representation for a received messages."""
+    """A representation for a received messages.
+
+    :param id: The message unique identifier.
+    :param reply_id: The message identifier this message is replied to.
+    :param date: The date the message was sent/received.
+    :param raw: The raw data response from service.
+    :param status: The message status.
+    :param exc: The exception object if an error occured.
+    :param service: Service to use for sending, replies and fowarding.
+
+    """
+
+    id: t.Optional[str] = None
+    reply_id: t.Optional[str] = None
+    date: t.Optional[dt.datetime] = None
+    raw: t.Any = None
+    status: MessageStatus = "draft"
+    exc: t.Optional[Exception] = None
+    service: t.Optional["Service"] = None
+
+    def as_dict(self):
+        return dataclasses.asdict(self)
+
+    def send(self, service=None):
+        if not service:
+            service = self.service
+        if not service:
+            raise ValueError("No service to send this message")
+
+        return service.send_message(self)
+
+
+class MessageBuilder(UserDict):
+    def __init__(self, dict=None, service=None, **kwargs):
+        self.service = service
+
+        super().__init__(dict, **kwargs)
+
+    def _replace(self, **kwargs):
+        message = self.copy()
+        message.update(**kwargs)
+
+        return message
+
+    def send(self):
+        service = self.service
+        if not service:
+            raise ValueError("No service to send this message")
+
+        return service.send(**self.data)
 
 
 class Outbox(UserList):
     """Outbox containing captured messages.
 
     :param suppress: Do not send messages when released.
 
     """
 
-    def __init__(self, suppress=False):
+    def __init__(self, service, suppress=False):
+        self.service = service
         self.suppress = suppress
 
         super().__init__()
 
-    def __enter__(self):
-        return self
+    def append(self, item):
+        super().append(item)
 
-    def __exit__(self, exc_type, exc_value, exc_tb):
-        if exc_type:
-            self.discard()
-        else:
-            self.release()
+        self.service.logger.debug("Enqueued a message in outbox:\n%r", item)
+
+    def clear(self):
+        count = len(self.data)
+
+        super().clear()
+
+        self.service.logger.debug("Discarded %d messages from outbox", count)
 
     def discard(self):
         """Discard all messages."""
-        self.data.clear()
+        self.clear()
 
     def release(self):
         """Release messages to be sent, unless :data:``suppress`` is set."""
-        if self.suppress:
-            self.data.clear()
+        # if self.suppress:
+        #     self.data.clear()
+
+        count = len(self.data)
 
         with on_before_send.muted():
             while self.data:
                 service, message = self.data.pop()
                 service.send(**message)
 
+        self.service.logger.debug("Released %d messages from outbox", count)
+
 
 class Service:
     """Base class for all services."""
 
     name: str
+
     can_receive: bool = False
     can_send: bool = False
 
+    has_receive_webhook = False
+    has_receive_webhook_methods = ["POST"]
+
+    has_status_callback = False
+    has_status_callback_methods = ["POST"]
+
     def __init__(self, suppress=False, **kwargs):
         self.opened = False
         """Whether a connection or session has been started."""
 
         self.suppress = suppress
         """Suppress sending of messages."""
 
+        self._media_helper = None
+
         self._wrap_methods()
 
+        self.logger = logging.getLogger(__name__)
+
+    def _on_receive_message(self, message):
+        message.status = "received"
+
+        on_receive_message.send(self, message=message)
+
+        self.logger.debug("Received message:\n%r", message)
+
     def _wrap_close(self):
         # wrap the close method:
         # - dispatch the `on_session_close` signals.
         # - unset the ``opened`` flag.
+        # - log a message.
         original_close = self.close
 
         def close(self):
             original_close()
 
             on_close_session.send(self)
 
+            self.logger.debug("Closed session")
+
             self.opened = False
 
         self.close = close.__get__(self, Service)
         self._close = original_close
 
     def _wrap_methods(self):
         # wrap all methods
         self._wrap_close()
         self._wrap_open()
         self._wrap_receive()
+        self._wrap_receive_webhook()
         self._wrap_send()
+        self._wrap_status_callback()
 
     def _wrap_open(self):
         # wrap the open method:
         # - dispatch `on_session_open` signals.
         # - set the ``opened`` flag.
+        # - log a message.
 
         original_open = self.open
 
         def open(self):
             original_open()
 
             on_open_session.send(self)
 
+            self.logger.debug("Opened session")
+
             self.opened = True
 
         self.open = open.__get__(self, Service)
         self._open = original_open
 
     def _wrap_receive(self):
         # wrap the receive method:
         # - dispatch `on_receive_message` signals.
         # - open the connection or session if ``opened`` flag not set.
+        # - log messages.
 
         original_receive = self.receive
 
         def receive(self, **kwargs):
             if not self.opened:
                 self.open()
 
+            count = 0
             for message in original_receive(**kwargs):
-                on_receive_message.send(self, message=message)
+                self._on_receive_message(message)
 
                 yield message
+                count += 1
+
+            self.logger.info("Received %d messages", count)
 
         self.receive = receive.__get__(self, Service)
         self._receive = original_receive
 
+    def _wrap_receive_webhook(self):
+        # wrap the receive_webhook method:
+        # - dispatch `on_receive_message` signals.
+        # - log messages.
+
+        original_receive = self.receive_webhook
+
+        def receive_webhook(self, request):
+            count = 0
+            for message in original_receive(request):
+                self._on_receive_message(message)
+
+                yield message
+                count += 1
+
+            self.logger.info("Received %d messages from webhook", count)
+
+        self.receive_webhook = receive_webhook.__get__(self, Service)
+        self._receive_webhook = original_receive
+
     def _wrap_send(self):
         # wrap the send method:
         # - dispatch ``on_before_send`` and ``on_after_send`` signals.
         # - open the connection or session if ``opened`` flag not set.
         # - silently discard the message if ``suppress`` flag is set.
+        # - log messages.
 
         original_send = self.send
 
         def send(self, **kwargs):
             on_before_send.send(self, message=kwargs)
 
             if self.suppress:
                 return
 
             if not self.opened:
                 self.open()
 
-            results = original_send(**kwargs)
+            message = original_send(**kwargs)
 
-            on_after_send.send(self, message=kwargs)
+            on_after_send.send(self, message=message)
 
-            return results
+            # self.logger.info("Sent message %s", message.id)
+            # self.logger.debug("%r", message)
+
+            return message
 
         self.send = send.__get__(self, Service)
         self._send = original_send
 
+    def _wrap_status_callback(self):
+        # wrap the status_callback method:
+        # - dispatch ``on_receive_status_callback`` signals.
+        # - log messages.
+
+        original_status = self.status_callback
+
+        def status_callback(self, request):
+            message_id, status, raw = original_status(request)
+            on_receive_status_callback.send(
+                self,
+                message_id=message_id,
+                status=status,
+                raw=raw,
+            )
+
+            self.logger.info(
+                "Received message status: %s, %s",
+                message_id,
+                status,
+            )
+
+            return message_id, status, raw
+
+        self.status_callback = status_callback.__get__(self, Service)
+        self._status_callback = original_status
+
     def __enter__(self):
         if not self.opened:
             self.open()
 
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
@@ -199,26 +354,38 @@
 
         This is called at the end of a context manager, otherwise must be
         called manually.
 
         """
         return
 
+    def generate_media_urls(self, attachments: t.List[Attachment]):
+        """Generate URLs for services that require external media URLs."""
+        urls = []
+        for attachment in attachments:
+            url = self._media_helper(attachment)
+            urls.append(url)
+        return urls
+
     def open(self):
         """Open or prepare a connection or session.
 
         Developers SHOULD implement this method if they need to setup or
         configure a connection.
 
         This is called on first send and called at the start of a context
         manager.
 
         """
         return
 
+    def media_helper(self, f):
+        """Register a function to help with external media."""
+        self._media_helper = f
+
     @contextmanager
     def outbox(self):
         """Capture outgoing messages.
 
         On exit, the messages will be released and sent.
 
         You can call the :meth:`release` method manually:
@@ -239,30 +406,35 @@
                 service.send(...)
 
                 outbox.discard()  # all messages are discarded
 
             # nothing is sent
 
         """
-        outbox = Outbox(suppress=self.suppress)
+        outbox = Outbox(self, suppress=self.suppress)
 
         def capture(this, kwargs):
             outbox.append((this, kwargs))
 
-        on_before_send.connect(capture, self)
+        on_before_send.connect(capture)
 
         original_suppress = self.suppress
         self.suppress = True
 
         try:
             yield outbox
+        except Exception:
+            outbox.discard()
+            raise
         finally:
-            on_before_send.disconnect(capture, self)
+            on_before_send.disconnect(capture)
             self.suppress = original_suppress
 
+        outbox.release()
+
     def receive(
         self,
         limit: int = 100,
         **kwargs,
     ) -> t.Generator[Message, None, None]:
         """Receive messages.
 
@@ -275,28 +447,63 @@
         :return: A received message.
         :rtype: Message
 
         """
         name = self.__class__.__name__
         raise ServiceReceiveCapabilityError(name=name)
 
+    def receive_webhook(self, request):
+        """Receive messages from a webhook.
+
+        Developers SHOULD implement this method.
+
+        :param request: The request to parse.
+
+        :raises ServiceReceiveCapabilityError: Receiving not supported.
+
+        """
+        name = self.__class__.__name__
+        raise ServiceReceiveCapabilityError(name=name)
+
     def send(self, *args, **kwargs):
         """Send a message.
 
         Developers MUST implement this method.
 
         :raises ServiceSendCapabilityError: Sending messages not supported.
 
         """
         name = self.__class__.__name__
         raise ServiceSendCapabilityError(name=name)
 
+    def send_message(self, message: Message):
+        """Send a message from a message object.
+
+        :param message: A :class:`Message` message object.
+
+        """
+        data = message.as_dict()
+        data["service"] = self
+        return message.send(**data)
+
+    def status_callback(self, request):
+        """Receive sent message status callback from a webhook.
+
+        Developers SHOULD implement this method.
+
+        :param request: The request to parse.
+
+        :raises NotImplementedError: Status callback not supported.
+
+        """
+        raise NotImplementedError()
+
     @contextmanager
     def suppressed(self):
-        """suppress outgoing messages for duration of the context manager."""
+        """Suppress outgoing messages for duration of the context manager."""
         original_suppress = self.suppress
         self.suppress = True
 
         try:
             yield
         finally:
             self.suppress = original_suppress
@@ -333,28 +540,34 @@
 
         def receive(self, limit=100, via=None, **kwargs):
             services = []
             if via:
                 try:
                     service = self.services[via]
                 except KeyError:
-                    raise RuntimeError(f"No service '{via}' registered")
+                    raise ServiceNotRegistered(via)
                 else:
                     services.append(service)
             else:
                 # get all services in a random order to prevent a single
                 # service from blocking all other services
                 services = list(
                     s for s in self.services.values() if s.can_receive
                 )
-                services = random.shuffle(services)
+                random.shuffle(services)
+
+            if not services:
+                raise ServiceReceiveCapabilityError()
 
             for service in services:
                 for message in service.receive(limit=limit, **kwargs):
-                    on_receive_message(self, message=message)
+                    # if service cannot send replies, set to manager
+                    if not service.can_send:
+                        message.service = self
+                    on_receive_message.send(self, message=message)
                     yield message
                     limit -= 1
 
         self.receive = receive.__get__(self, ServiceManager)
 
     def _update_send(self):
         # update the send method:: bool = False
@@ -368,25 +581,25 @@
             if self._via and not via:
                 via = self._via(self, **kwargs)
 
             if via:
                 try:
                     service = self.services[via]
                 except KeyError:
-                    raise RuntimeError(f"No service '{via}' registered")
+                    raise ServiceNotRegistered(via)
 
             if not service:
                 try:
                     service = list(
                         s for s in self.services.values() if s.can_send
                     )[0]
                 except IndexError:
-                    raise RuntimeError("No sending services registered")
+                    raise ServiceSendCapabilityError()
 
-            on_before_send.send(self, kwargs=kwargs)
+            on_before_send.send(service, kwargs=kwargs)
 
             if self.suppress:
                 return
 
             result = service.send(**kwargs)
 
             on_after_send.send(self, kwargs=kwargs)
@@ -447,14 +660,21 @@
                     found_send = True
 
             if receive and not found_receive:
                 raise ServiceReceiveCapabilityError()
             if send and not found_send:
                 raise ServiceSendCapabilityError()
 
+    def media_helper(self, f):
+        """Register a function to help with external media."""
+        super().media_helper(f)
+
+        for service in self.services.values():
+            service.media_helper(f)
+
     def register(
         self,
         service_cls,
         *args,
         name=None,
         overwrite=False,
         **kwargs,
@@ -468,33 +688,43 @@
                      service.
         :param overwrite: Overwrite an existing service with ``name``, defaults
                           to ``False``.
         :param \*\*kwargs: Keyword-arguments to pass to the service on
                            initialisation.
 
         """
+        if not name:
+            name = service_cls.name
         if name in self.services and not overwrite:
             raise KeyError(f"Service '{name}' already exists")
 
         service = service_cls(*args, **kwargs)
+
+        if self._media_helper:
+            service.media_helper(self._media_helper)
+
         self.services[name] = service
 
+        on_register_service.send(self, service=service)
+
+        self.logger.info("Registered a service: %s", service.name)
+
         return service
 
     def unregister(self, service, ignore_missing=False):
         """Unregister a service.
 
         :param service: The service or service name to unregister.
         :param ignore_missing: Do not raise an exception if service does not
                                exist on manager, defaults to ``False``.
 
         """
         if isinstance(service, str):
             try:
-                return self.services.pop(service)
+                service = self.services.pop(service)
             except KeyError:
                 if ignore_missing:
                     return
                 raise KeyError(f"Service '{service}' does not exist")
         else:
             name = None
             for name, service_ in self.services.items():
@@ -502,15 +732,19 @@
                     name = name
                     break
             else:
                 if ignore_missing:
                     return
                 raise KeyError(f"Service '{service!r}' does not exist")
 
-            return self.services.pop(name)
+            service = self.services.pop(name)
+
+        on_unregister_service.send(self, service=service)
+
+        self.logger.info("Unregistered a service: %s", service.name)
 
     def via(
         self,
         f: t.Callable[
             ["ServiceManager", "t.ParamSpecKwargs"],
             t.Optional[str],
         ],
```

### Comparing `owlery-0.1.1/owlery/services/email/__init__.py` & `owlery-0.2.0/owlery/services/email/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 import dataclasses
-import datetime as dt
 import typing as t
 
 from collections import UserDict
+from email import (
+    message_from_binary_file,
+    message_from_bytes,
+    message_from_file,
+    message_from_string,
+)
 from email.message import EmailMessage as PyEmailMessage
-from email.utils import format_datetime, make_msgid
+from email.utils import (
+    format_datetime,
+    make_msgid,
+    parseaddr,
+    parsedate_to_datetime,
+)
 
 from .. import USER_AGENT, Attachment, Message, Service, ServiceManager
 
+try:
+    import envelope
+except ImportError:
+    ENVELOPE_AVAILABLE = False
+else:
+    ENVELOPE_AVAILABLE = True
+
 AddressType = t.Union[str, t.Tuple[t.Optional[str], str]]
 AddressesType = t.Iterable[AddressType]
 
 
 @dataclasses.dataclass
 class EmailAttachment(Attachment):
     """A representation of an email attachment.
@@ -38,37 +55,117 @@
                           (https://amp.dev/about/email)
     :param cc: A list of carbon-copy recipients.
     :param bcc: A list of blind carbon-copy recipients.
     :param reply_to: An optional address to send replies to.
     :param from\\_: The from address of the email message.
     :param attachments: A list of attachments.
     :param headers: A list of additional messages headers.
+    :param encrypted: Email message is encrypted with GPG, PGP or S/MIME
+    :param verified: Email message integrity has been verified.
     :param service: Service to use for sending, reply etc.
 
     """
 
-    to: AddressesType
-    subject: str
-    body: str
+    to: t.Optional[AddressesType] = None
+    subject: t.Optional[str] = None
+    body: t.Optional[str] = None
     html_body: t.Optional[str] = None
     amp_html_body: t.Optional[str] = None
     cc: AddressesType = dataclasses.field(default_factory=list)
     bcc: AddressesType = dataclasses.field(default_factory=list)
     reply_to: t.Optional[AddressType] = None
     from_: t.Optional[AddressType] = None
     attachments: t.List[EmailAttachment] = dataclasses.field(
         default_factory=list,
     )
     headers: t.Dict[str, str] = dataclasses.field(default_factory=dict)
+    encrypted: bool = False
+    signed: bool = False
+    verified: bool = False
+    raw: t.Any = None
     service: t.Optional["Email"] = None
 
+    def as_bytes(self):
+        message = self.as_email_message()
+        return message.as_bytes()
+
+    def as_email_message(self):
+        message = PyEmailMessage()
+
+        if self.date:
+            message["Date"] = format_datetime(self.date)
+
+        if not self.id:
+            self.id = make_msgid()
+        message["Message-ID"] = self.id
+
+        if self.from_:
+            message["From"] = self.from_
+
+        if self.to:
+            message["To"] = self.to
+
+        if self.cc:
+            message["Cc"] = self.cc
+
+        if self.reply_to:
+            message["Reply-To"] = self.reply_to
+
+        if self.subject:
+            message["Subject"] = self.subject
+
+        message.set_content(self.body, subtype="plain")
+
+        if self.amp_html_body:
+            message.add_alternative(self.amp_html_body, subtype="x-amp-html")
+
+        if self.html_body:
+            message.add_alternative(self.html_body, subtype="html")
+
+        message["User-Agent"] = message["X-Mailer"] = USER_AGENT
+
+        if self.headers:
+            for name, value in self.headers.items():
+                message[name] = value
+
+        return message
+
+    def as_string(self):
+        message = self.as_email_message()
+        return message.as_string()
+
     @classmethod
     def build(self, **kwargs):
         return EmailMessageBuilder(**kwargs)
 
+    def _check_encrypted_and_signed(self):
+        message = self.as_email_message()
+        encrypted = signed = False
+        for part in message.walk():
+            if part.get_content_type() == "multipart/encrypted":
+                encrypted = True
+            elif part.get_content_type() == "multipart/signed":
+                signed = True
+        return encrypted, signed
+
+    def decrypt(self):
+        """Decrypt the message.
+
+        Requires the `envelope` library to be installed.
+
+        """
+        if not ENVELOPE_AVAILABLE:
+            raise RuntimeError("envelope library not available")
+
+        message = self.as_email_message()
+
+        env = envelope.Envelope.load(message)
+
+        return self.from_email_message(env.as_message())
+
     def forward(
         self,
         to: AddressesType,
         quote: bool = True,
         service: t.Optional["Email"] = None,
         **kwargs,
     ):
@@ -85,14 +182,78 @@
         if not service:
             return
 
         body = self.body
 
         service.send(to, body, attachments=self.attachments, **kwargs)
 
+    @classmethod
+    def from_binary_file(cls, fp: t.IO[bytes]):
+        msg = message_from_binary_file(fp, PyEmailMessage)
+        return cls.from_email_message(msg)  # type: ignore
+
+    @classmethod
+    def from_bytes(cls, s: bytes):
+        msg = message_from_bytes(s, PyEmailMessage)
+        return cls.from_email_message(msg)  # type: ignore
+
+    @classmethod
+    def from_email_message(cls, message: PyEmailMessage):
+        to = [parseaddr(t.strip()) for t in message.get("To", "").split(",")]
+        from_ = parseaddr(message.get("From", ""))
+        subject = message.get("Subject", "")
+        body = message.get_body(("plain",))
+        html_body = message.get_body(("html",))
+        cc = [parseaddr(c.strip()) for c in message.get("Cc", "").split(",")]
+        reply_to = parseaddr(message.get("Reply-To", ""))
+        date = message.get("Date", None)
+        if date:
+            date = parsedate_to_datetime(date)
+        id = message.get("Message-ID")
+
+        headers = {}
+        for name, value in message.items():
+            if name in (
+                "From",
+                "Subject",
+                "To",
+                "Cc",
+                "Reply-To",
+                "Date",
+                "Message-ID",
+            ):
+                continue
+            headers[name] = value
+
+        headers = dict(message.items())
+
+        return cls(
+            to=to,
+            subject=subject,
+            body=body and body.get_payload() or "",
+            html_body=html_body and html_body.get_payload() or None,
+            cc=cc,
+            reply_to=reply_to,
+            from_=from_,
+            headers=headers,
+            date=date,
+            id=id,
+            raw=message,
+        )
+
+    @classmethod
+    def from_file(cls, fp: t.IO[str]):
+        msg = message_from_file(fp, PyEmailMessage)
+        return cls.from_email_message(msg)  # type: ignore
+
+    @classmethod
+    def from_string(cls, s: str):
+        msg = message_from_string(s, PyEmailMessage)
+        return cls.from_email_message(msg)  # type: ignore
+
     def reply(
         self,
         quote: bool = True,
         service: t.Optional["Email"] = None,
         **kwargs,
     ):
         r"""Reply to this message.
@@ -129,14 +290,49 @@
         if not service:
             return
 
         body = self.body
 
         service.send(self.to, body, cc=self.cc, **kwargs)
 
+    def verify(self):
+        """Verify the message integrity.
+
+        Requires the `envelope` library to be installed.
+
+        :returns: message integrity verification
+        :rtype: bool
+
+        """
+        if not ENVELOPE_AVAILABLE:
+            raise RuntimeError("envelope library not available")
+
+        message = self.as_email_message()
+
+        env = envelope.Envelope.load(message)
+
+        sig = data = None
+        for part in message.walk():
+            if part.get_content_type() == "multipart/signed":
+                for subpart in part.walk():
+                    if (
+                        subpart.get_content_type()
+                        == "application/pgp-signature"
+                    ):
+                        sig = part.get_payload().encode()
+                    else:
+                        data = part.get_payload().encode()
+
+        if sig and data:
+            result = env._gpg_verify(sig, data)
+            self.verified = result
+            return result
+
+        return False
+
 
 class EmailMessageBuilder(UserDict):
     """A builder for email messages.
 
     :param to: A list of recipient addresses.
     :param subject: The email subject.
     :param body: The text body of the email.
@@ -162,14 +358,16 @@
         amp_html_body: t.Optional[str] = None,
         cc: t.Optional[AddressesType] = None,
         bcc: t.Optional[AddressesType] = None,
         reply_to: t.Optional[AddressType] = None,
         from_: t.Optional[AddressType] = None,
         attachments: t.Optional[t.Iterable[EmailAttachment]] = None,
         headers: t.Optional[t.Dict[str, str]] = None,
+        encrypt: bool = False,
+        sign: bool = False,
         service: t.Optional["Email"] = None,
     ):
         self.service = service
 
         super().__init__(
             {
                 "to": to,
@@ -179,23 +377,28 @@
                 "bcc": bcc,
                 "headers": headers,
                 "html_body": html_body,
                 "amp_html_body": amp_html_body,
                 "reply_to": reply_to,
                 "from_": from_,
                 "attachments": attachments,
+                "encrypt": encrypt,
+                "sign": sign,
             },
         )
 
     def amp_html_body(self, amp_html_body: t.Optional[str] = None):
         if not amp_html_body:
             return self.data["amp_html_body"]
 
         return self.replace(amp_html_body=amp_html_body)
 
+    def as_message(self):
+        return EmailMessage(**self.data)
+
     def attach(
         self,
         data: t.Union[bytes, t.IO[bytes]],
         filename: t.Optional[str] = None,
         mimetype: str = "application/octet-stream",
     ):
         """Attach a file to the message.
@@ -242,62 +445,22 @@
 
     def from_(self, from_: t.Optional[AddressType] = None):
         if not from_:
             return self.data["from_"]
 
         return self.replace(from_=from_)
 
-    def format_message(self) -> PyEmailMessage:
-        message = PyEmailMessage()
-
-        date = self.get("date")
-        if not date:
-            date = dt.datetime.now()
-        message["Date"] = format_datetime(date)
-
-        message["Message-ID"] = self.get("id", make_msgid())
-
-        from_ = self.get("from_")
-        if from_:
-            message["From"] = from_
-
-        to = self.get("to")
-        if to:
-            message["To"] = to
-
-        cc = self.get("cc")
-        if cc:
-            message["Cc"] = cc
-
-        reply_to = self.get("reply_to")
-        if reply_to:
-            message["Reply-To"] = reply_to
-
-        subject = self.get("subject")
-        if subject:
-            message["Subject"] = subject
-
-        message.set_content(self["body"], subtype="plain")
-
-        amp_html_body = self.get("amp_html_body")
-        if amp_html_body:
-            message.add_alternative(amp_html_body, subtype="x-amp-html")
-
-        html_body = self.get("html_body")
-        if html_body:
-            message.add_alternative(html_body, subtype="html")
-
-        message["User-Agent"] = message["X-Mailer"] = USER_AGENT
+    def encrypt(self):
+        """Encrypt the message.
 
-        headers = self.get("headers")
-        if headers:
-            for name, value in headers.items():
-                message[name] = value
+        Requires the `envelope` library to be installed.
 
-        return message
+        """
+        if not ENVELOPE_AVAILABLE:
+            raise RuntimeError("envelope library not available")
 
     def html_body(self, html_body: t.Optional[str] = None):
         if not html_body:
             return self.data["html_body"]
 
         return self.replace(html_body=html_body)
 
@@ -315,14 +478,23 @@
 
     def send(self):
         """Send the email message."""
         if not self.service:
             raise NotImplementedError()
         return self.service.send_message(self.format_message())
 
+    def sign(self):
+        """Sign the message.
+
+        Requires the `envelope` library to be installed.
+
+        """
+        if not ENVELOPE_AVAILABLE:
+            raise RuntimeError("envelope library not available")
+
     def subject(self, subject: t.Optional[str] = None):
         if not subject:
             return self.data["subject"]
 
         return self.replace(subject=subject)
 
     def to(self, to: t.Optional[AddressesType] = None):
@@ -385,14 +557,10 @@
         :param from\\_: The from address of the email message.
         :param attachments: A list of attachments.
         :param headers: A list of additional messages headers.
 
         """
         ...
 
-    def send_message(self, message: EmailMessage):
-        """Send an email message from :class:`EmailMessage`."""
-        return self.send(**dataclasses.asdict(message))
-
 
 class EmailManager(Email, ServiceManager):
     """Service manager for email messaging services."""
```

### Comparing `owlery-0.1.1/owlery/services/email/imap.py` & `owlery-0.2.0/owlery/services/email/imap.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing as t
 
 from ...exceptions import (
     ServiceAuthFailed,
     ServiceConnectError,
     ServiceTimeoutError,
 )
-from . import Email
+from . import Email, EmailMessage
 
 if t.TYPE_CHECKING:
     import ssl
 
 
 class IMAP(Email):
     """Service to receive email messages from an IMAP server mailbox.
@@ -22,14 +22,18 @@
     :param folder: Folder to check for messages, defaults to ``'INBOX'``.
     :param starttls: Use STARTTLS encryption.
     :param ssl: Use SSL encryption.
     :param ssl_context: SSL context, see :class:`ssl.SSLContext`.
 
     """
 
+    name = "imap"
+
+    can_receive = True
+
     def __init__(
         self,
         host: str = "localhost",
         port: t.Optional[int] = None,
         user: t.Optional[str] = None,
         password: t.Optional[str] = None,
         folder: str = "INBOX",
@@ -70,15 +74,15 @@
         if self.starttls:
             self.session.starttls(ssl_context=self.ssl_context)
 
         try:
             self.session.login(self.user, self.password or "")
         except imaplib.IMAP4.error as e:
             if "[AUTHENTICATIONFAILED]" in str(e):
-                raise ServiceAuthFailed()
+                raise ServiceAuthFailed(e)
             raise
 
     @property
     def port(self) -> int:
         port = self._port
         if not port:
             if self.ssl and not self.starttls:
@@ -90,10 +94,10 @@
 
     def receive(self, limit: int = 100, **kwargs):
         self.session.select(self.folder, readonly=True)
 
         res, data = self.session.search("UTF-8", "UNSEEN")
         for num in data[0].split():
             res, data = self.session.fetch(num, "(RFC822)")
-            yield data[0][1]
+            yield EmailMessage.from_bytes(data[0][1])
 
         self.session.close()
```

### Comparing `owlery-0.1.1/owlery/services/email/pop3.py` & `owlery-0.2.0/owlery/services/email/pop3.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing as t
 
 from ...exceptions import (
     ServiceAuthFailed,
     ServiceConnectError,
     ServiceTimeoutError,
 )
-from . import Email
+from . import Email, EmailMessage
 
 if t.TYPE_CHECKING:
     import ssl
 
 
 class POP3(Email):
     """Service to receive email messages from an POP3 server mailbox.
@@ -21,14 +21,18 @@
     :param password: Password to login.
     :param starttls: Use STARTTLS encryption.
     :param ssl: Use SSL encryption.
     :param ssl_context: SSL context, see :class:`ssl.SSLContext`.
 
     """
 
+    name = "pop3"
+
+    can_receive = True
+
     def __init__(
         self,
         host: str = "localhost",
         port: t.Optional[int] = None,
         user: t.Optional[str] = None,
         password: t.Optional[str] = None,
         starttls: bool = False,
@@ -68,15 +72,15 @@
             self.session.stls(context=self.ssl_context)
 
         try:
             self.session.user(self.user or "")
             self.session.pass_(self.password or "")
         except poplib.error_proto as e:
             if "[AUTH] Authentication failed" in str(e):
-                raise ServiceAuthFailed()
+                raise ServiceAuthFailed(e)
             raise
 
     @property
     def port(self) -> int:
         port = self._port
         if not port:
             if self.ssl and not self.starttls:
@@ -88,8 +92,9 @@
 
     def receive(self, limit: int = 100, **kwargs):
         res, data, size = self.session.list()
         count = len(data)
 
         for i in range(1, min(count, limit) + 1):
             res, data, octets = self.session.retr(i)
-            yield data
+            yield EmailMessage.from_bytes(b"\r\n".join(data))
+            self.session.dele(i)
```

### Comparing `owlery-0.1.1/owlery/services/email/smtp.py` & `owlery-0.2.0/owlery/services/email/smtp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import smtplib
 import typing as t
 
-from ...exceptions import ServiceConnectError, ServiceTimeoutError
-from . import Email
+from ...exceptions import ServiceAuthFailed, ServiceConnectError
+from . import Email, EmailMessage
 
 if t.TYPE_CHECKING:
     import ssl
 
 
 class SMTP(Email):
     """Service to send email messages from an SMTP server.
@@ -19,14 +19,16 @@
     :param ssl: Use SSL encryption.
     :param ssl_context: SSL context, see :class:`ssl.SSLContext`.
 
     """
 
     name = "smtp"
 
+    can_send = True
+
     def __init__(
         self,
         host: str = "localhost",
         port: t.Optional[int] = None,
         user: t.Optional[str] = None,
         password: t.Optional[str] = None,
         starttls: bool = False,
@@ -44,32 +46,36 @@
 
         self.session: t.Union[smtplib.SMTP, smtplib.SMTP_SSL]
         if ssl:
             self.session = smtplib.SMTP_SSL(context=ssl_context)
         else:
             self.session = smtplib.SMTP()
 
+        # this is required for ssl support
+        self.session._host = host  # type: ignore
+
         super().__init__(**kwargs)
 
     def close(self):
         self.session.quit()
 
     def open(self):
         try:
             self.session.connect(self.host, self.port)
-        except TimeoutError as e:
-            raise ServiceTimeoutError(e)
-        except ConnectionError as e:
+        except (smtplib.SMTPConnectError, smtplib.SMTPServerDisconnected) as e:
             raise ServiceConnectError(e)
 
         if self.starttls:
             self.session.starttls(context=self.ssl_context)
 
         if self.user:
-            self.session.login(self.user, self.password or "")
+            try:
+                self.session.login(self.user, self.password or "")
+            except smtplib.SMTPAuthenticationError as e:
+                raise ServiceAuthFailed(e)
 
     @property
     def port(self) -> int:
         port = self._port
         if not port:
             if self.starttls:
                 port = 587
@@ -77,9 +83,18 @@
                 port = 465
             else:
                 port = 25
 
         return port
 
     def send(self, **kwargs):
-        message = self.Message(**kwargs).format_message()
-        return self.session.send_message(message)
+        message = EmailMessage(**kwargs)
+
+        try:
+            self.session.send_message(message.as_email_message())
+        except smtplib.SMTPException as e:
+            message.exc = e
+            message.status = "error"
+        else:
+            message.status = "sent"
+
+        return message
```

### Comparing `owlery-0.1.1/owlery/services/misc.py` & `owlery-0.2.0/owlery/services/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import typing as t
 
-from . import Service
+from . import Message, Service
 
 
 class Logger(Service):
     """Service that logs sent messages to a logger.
 
     :param logger: Name of the logger, defaults to root logger.
     :param level: Level of logging message, defaults to ``logging.INFO`` (or
@@ -21,34 +21,36 @@
     def __init__(
         self,
         logger: t.Optional[str] = None,
         level: int = logging.INFO,
         message: str = "Message sent %s",
         **kwargs,
     ):
-        self.logger = logging.getLogger(logger)
+        self.message_logger = logging.getLogger(logger)
         self.level = level
         self.message = message
 
         super().__init__(**kwargs)
 
         self.suppress = False
 
     def send(self, **kwargs):
-        self.logger.log(self.level, self.message, kwargs, extra=kwargs)
+        self.message_logger.log(self.level, self.message, kwargs, extra=kwargs)
+
+        return Message(raw=kwargs)
 
 
 class Null(Service):
     """Service that silently discards messages."""
 
     name = "null"
     can_send = True
 
     def send(self, **kwargs):
-        return
+        return Message()
 
 
 class ReceiveFunction(Service):
     """Service to call a function to receive messages.
 
     :param func: Function to call.
```

### Comparing `owlery-0.1.1/owlery.egg-info/PKG-INFO` & `owlery-0.2.0/owlery.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlery
-Version: 0.1.1
+Version: 0.2.0
 Summary: Uniform messaging service for Python applications.
 Author-email: Michael de Villiers <michael@devilears.co.za>
 Maintainer-email: Michael de Villiers <michael@devilears.co.za>
 License: MIT
 Project-URL: Homepage, https://github.com/COUR4G3/owlery/
 Project-URL: Documentation, https://owlery-messaging.readthedocs.io/
 Project-URL: Changes, https://owlery-messaging.readthedocs.io/en/latest/changelog.html
@@ -25,17 +25,18 @@
 Provides-Extra: tests
 Provides-Extra: typing
 License-File: LICENSE
 
 Owlery
 ======
 
-Uniform messaging service for Python applications supporting a variety of messaging services and vendors, allowing easy
-substitution and drop-in of services and vendors during runtime, configuration, development cycle or application
-evolution - even sending different messages through different vendors based on rules.
+Uniform messaging service supporting a variety of messaging services and vendors easily integrated with your Python
+applications or usable from your command-line, allowing easy substitution and drop-in of services and vendors during
+runtime, configuration, development cycle or application evolution - even sending different messages through different
+vendors based on rules.
 
 
 ## Links
 
 - Documentation: <https://owlery-messaging.readthedocs.io/>
 - Changes: <https://owlery-messaging.readthedocs.io/en/latest/changes.html>
 - Releases: <https://pypi.org/project/owlery/>
```

### Comparing `owlery-0.1.1/owlery.egg-info/SOURCES.txt` & `owlery-0.2.0/owlery.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -32,41 +32,55 @@
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/signals.rst
 docs/spelling-wordlist.txt
+docs/integrations/flask.rst
+docs/recipes/celery.rst
+docs/recipes/index.rst
+docs/recipes/rq.rst
 docs/services/index.rst
 docs/services/email/imap.rst
 docs/services/email/index.rst
 docs/services/email/pop3.rst
 docs/services/email/smtp.rst
 owlery/__init__.py
 owlery/_version.py
 owlery/exceptions.py
 owlery/py.typed
 owlery/signals.py
+owlery/utils.py
 owlery.egg-info/PKG-INFO
 owlery.egg-info/SOURCES.txt
 owlery.egg-info/dependency_links.txt
 owlery.egg-info/entry_points.txt
 owlery.egg-info/requires.txt
 owlery.egg-info/top_level.txt
 owlery/services/__init__.py
 owlery/services/misc.py
+owlery/services/twilio.py
 owlery/services/email/__init__.py
 owlery/services/email/imap.py
 owlery/services/email/pop3.py
 owlery/services/email/smtp.py
+owlery/services/mms/__init__.py
+owlery/services/mms/twilio.py
+owlery/services/sms/__init__.py
+owlery/services/sms/twilio.py
+owlery/services/whatsapp/__init__.py
+owlery/services/whatsapp/twilio.py
 tests/__init__.py
 tests/conftest.py
 tests/requirements.txt
 tests/test_signals.py
 tests/services/__init__.py
+tests/services/test_manager.py
 tests/services/test_misc.py
+tests/services/test_service.py
 tests/services/email/__init__.py
 tests/services/email/conftest.py
 tests/services/email/test_imap.py
 tests/services/email/test_pop3.py
 tests/services/email/test_smtp.py
 typing/requirements.txt
```

### Comparing `owlery-0.1.1/pyproject.toml` & `owlery-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/tests/conftest.py` & `owlery-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `owlery-0.1.1/tests/services/email/test_imap.py` & `owlery-0.2.0/tests/services/email/test_imap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,40 @@
+import imaplib
+import time
+
+from email.utils import make_msgid
+
 import pytest
 
 from owlery.exceptions import ServiceAuthFailed
+from owlery.services.email import EmailMessage
 from owlery.services.email.imap import IMAP
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture()
 def message():
-    return {
-        "body": "This is a test message",
-        "from_": "test@example.com",
-        "subject": "Test message",
-        "to": ["test@example.com"],
-    }
+    message = EmailMessage(
+        to=["user"],
+        subject="Test message",
+        body="This is a test message.",
+        from_="test@example.com",
+        id=make_msgid(),
+    )
+
+    with imaplib.IMAP4(host="localhost", port=143) as imap:
+        imap.login("user", "pass")
+
+        imap.append(
+            "INBOX",
+            (),
+            time.time(),
+            message.as_bytes(),
+        )
+
+    return message
 
 
 @pytest.fixture(scope="session")
 def imap():
     return IMAP(host="localhost", port=143, user="user", password="pass")
 
 
@@ -99,31 +118,35 @@
 def test_specified_port():
     imap = IMAP(port=144)
     assert imap.port == 144
 
 
 @pytest.mark.integration
 def test_receive(imap, message):
-    for _ in imap.receive(limit=10):
-        pass
+    for received_message in imap.receive(limit=10):
+        received_message = received_message
     imap.close()
+    assert received_message.id == message.id
 
 
 @pytest.mark.integration
 def test_receive_contextmanager(imap, message):
     with imap:
-        for _ in imap.receive(limit=10):
-            pass
+        for received_message in imap.receive(limit=10):
+            received_message = received_message
+    assert received_message.id == message.id
 
 
 @pytest.mark.integration
 def test_receive_with_manager(manager_with_imap, message):
-    for _ in manager_with_imap.receive(limit=10):
-        pass
+    for received_message in manager_with_imap.receive(limit=10):
+        received_message = received_message
     manager_with_imap.close()
+    assert received_message.id == message.id
 
 
 @pytest.mark.integration
 def test_receive_with_manager_contextmanager(manager_with_imap, message):
     with manager_with_imap:
-        for _ in manager_with_imap.receive(limit=10):
-            pass
+        for received_message in manager_with_imap.receive(limit=10):
+            received_message = received_message
+    assert received_message.id == message.id
```

### Comparing `owlery-0.1.1/tests/services/email/test_pop3.py` & `owlery-0.2.0/tests/services/email/test_pop3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,38 @@
+import imaplib
+import secrets
+import time
+
 import pytest
 
 from owlery.exceptions import ServiceAuthFailed
+from owlery.services.email import EmailMessage
 from owlery.services.email.pop3 import POP3
 
 
-@pytest.fixture(scope="session")
+@pytest.fixture()
 def message():
-    return {
-        "body": "This is a test message",
-        "from_": "test@example.com",
-        "subject": "Test message",
-        "to": ["test@example.com"],
-    }
+    message = EmailMessage(
+        to=["user"],
+        subject=f"Test message {secrets.token_hex(8)}",
+        body="This is a test message.",
+        from_="test@example.com",
+    )
+
+    with imaplib.IMAP4(host="localhost", port=144) as imap:
+        imap.login("user", "pass")
+
+        imap.append(
+            "INBOX",
+            (),
+            time.time(),
+            message.as_bytes(),
+        )
+
+    return message
 
 
 @pytest.fixture(scope="session")
 def pop3():
     return POP3(host="localhost", port=110, user="user", password="pass")
 
 
@@ -103,31 +120,39 @@
 def test_specified_port():
     pop3 = POP3(port=111)
     assert pop3.port == 111
 
 
 @pytest.mark.integration
 def test_receive(pop3, message):
-    for _ in pop3.receive(limit=10):
-        pass
+    received_message = None
+    for received_message in pop3.receive(limit=10):
+        received_message = received_message
     pop3.close()
+    assert received_message.subject == message.subject
 
 
 @pytest.mark.integration
 def test_receive_contextmanager(pop3, message):
+    received_message = None
     with pop3:
-        for _ in pop3.receive(limit=10):
-            pass
+        for received_message in pop3.receive(limit=10):
+            received_message = received_message
+    assert received_message.subject == message.subject
 
 
 @pytest.mark.integration
 def test_receive_with_manager(manager_with_pop3, message):
-    for _ in manager_with_pop3.receive(limit=10):
-        pass
+    received_message = None
+    for received_message in manager_with_pop3.receive(limit=10):
+        received_message = received_message
     manager_with_pop3.close()
+    assert received_message.subject == message.subject
 
 
 @pytest.mark.integration
 def test_receive_with_manager_contextmanager(manager_with_pop3, message):
+    received_message = None
     with manager_with_pop3:
-        for _ in manager_with_pop3.receive(limit=10):
-            pass
+        for received_message in manager_with_pop3.receive(limit=10):
+            received_message = received_message
+    assert received_message.subject == message.subject
```

### Comparing `owlery-0.1.1/tests/services/test_misc.py` & `owlery-0.2.0/tests/services/test_misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,34 +19,26 @@
     service.send(foo="bar")
 
     assert caplog.records[0].levelno == service.level
     assert caplog.records[0].msg == service.message
     assert caplog.records[0].foo == "bar"
 
 
-def test_null(mocker):
+def test_null():
     service = Null()
 
-    spy = mocker.spy(service, "send")
-
-    service.send(foo="bar")
-
-    assert spy.call_count == 1
-    assert spy.spy_return is None
+    message = service.send(foo="bar")
+    assert message.raw is None
 
 
-def test_null_with_manager(manager, mocker):
+def test_null_with_manager(manager):
     manager.register(Null)
 
-    spy = mocker.spy(manager, "send")
-
-    manager.send(foo="bar")
-
-    assert spy.call_count == 1
-    assert spy.spy_return is None
+    message = manager.send(foo="bar")
+    assert message.raw is None
 
 
 def test_receive_function(mocker):
     stub = mocker.stub(name="receive_function")
 
     limit = 10
```

### Comparing `owlery-0.1.1/tests/test_signals.py` & `owlery-0.2.0/tests/test_signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from owlery import signals
+from owlery.services import Message
 from owlery.services.misc import Null, ReceiveFunction
 
 
 @pytest.fixture
 def message():
     return {
         "foo": "bar",
@@ -22,15 +23,15 @@
     def capture(service, message):
         captured.append((service, message))
 
     with signals.on_after_send.connected_to(capture):
         service.send(**message)
 
         assert captured[0][0] is service
-        assert captured[0][1] == message
+        assert captured[0][1].raw is None
 
 
 def test_on_before_send(service, message):
     captured = []
 
     def capture(service, message):
         captured.append((service, message))
@@ -70,17 +71,17 @@
 def test_on_receive_message(message):
     captured = []
 
     def capture(service, message):
         captured.append((service, message))
 
     def receive(**kwargs):
-        return [message]
+        return [Message(raw=message)]
 
     service = ReceiveFunction(receive)
 
     with signals.on_receive_message.connected_to(capture):
         for _ in service.receive():
             pass
 
         assert captured[0][0] is service
-        assert captured[0][1] == message
+        assert captured[0][1].raw == message
```

### Comparing `owlery-0.1.1/tox.ini` & `owlery-0.2.0/tox.ini`

 * *Files identical despite different names*

