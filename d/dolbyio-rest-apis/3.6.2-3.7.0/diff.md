# Comparing `tmp/dolbyio-rest-apis-3.6.2.tar.gz` & `tmp/dolbyio-rest-apis-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbyio-rest-apis-3.6.2.tar", last modified: Thu Apr  6 22:13:48 2023, max compression
+gzip compressed data, was "dolbyio-rest-apis-3.7.0.tar", last modified: Wed Jun  7 18:07:48 2023, max compression
```

## Comparing `dolbyio-rest-apis-3.6.2.tar` & `dolbyio-rest-apis-3.7.0.tar`

### file list

```diff
@@ -1,148 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:48.003575 dolbyio-rest-apis-3.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/ISSUE_TEMPLATE/report-an-issue.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.github/SECURITY.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.github/workflows/self-smoke-test-action.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/print-hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/requirements/runtime-prerequisites.in
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/requirements/runtime-prerequisites.txt
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/requirements/runtime.in
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/requirements/runtime.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2208 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/twine-upload.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/workflows/build-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.github/workflows/publish-package-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-04-06 22:13:48.003575 dolbyio-rest-apis-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/cli/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/monitor/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/communications/commands/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/enhance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/mastering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/cli/src/dolbyio_rest_apis_cli/media/commands/transcode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/client/
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.991575 dolbyio-rest-apis-3.6.2/client/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.995575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/conference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/internal/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/conferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/http_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/analyze_music.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/analyze_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/enhance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/internal/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/mastering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/analyze_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/diagnose_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/enhance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/mastering_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/result_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/transcode_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:47.999575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:48.003575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/internal/http_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:48.003575 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/publish_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/publish_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/subscribe_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-06 22:13:31.000000 dolbyio-rest-apis-3.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 22:13:48.003575 dolbyio-rest-apis-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.372013 dolbyio-rest-apis-3.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.376013 dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/report-an-issue.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.372013 dolbyio-rest-apis-3.7.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.380013 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.380013 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.in
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/workflows/build-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/workflows/publish-package-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.372013 dolbyio-rest-apis-3.7.0/client/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/conference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/conferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/remix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/mastering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/diagnose_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/enhance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/mastering_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/result_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/transcode_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/http_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/publish_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/publish_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/subscribe_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/setup.cfg
```

### Comparing `dolbyio-rest-apis-3.6.2/.github/ISSUE_TEMPLATE/report-an-issue.md` & `dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/report-an-issue.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.gitignore` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/.pre-commit-config.yaml` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 ---
 ci:
   autoupdate_schedule: quarterly
+  default_language_version: python3.11
 
 repos:
 - repo: https://github.com/asottile/add-trailing-comma.git
-  rev: v2.3.0
+  rev: v2.4.0
   hooks:
   - id: add-trailing-comma
 
 - repo: https://github.com/PyCQA/isort.git
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
     args:
     - --honor-noqa
 
 - repo: https://github.com/Lucas-C/pre-commit-hooks.git
-  rev: v1.3.1
+  rev: v1.5.1
   hooks:
   - id: remove-tabs
 
 - repo: https://github.com/python-jsonschema/check-jsonschema.git
-  rev: 0.18.3
+  rev: 0.22.0
   hooks:
   - id: check-github-actions
   - id: check-github-workflows
   - id: check-jsonschema
     name: Check GitHub Workflows set timeout-minutes
     args:
     - --builtin-schema
     - github-workflows-require-timeout
     files: ^\.github/workflows/[^/]+$
     types:
     - yaml
   - id: check-readthedocs
 
 - repo: https://github.com/pre-commit/pre-commit-hooks.git
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   # Side-effects:
   - id: end-of-file-fixer
   - id: trailing-whitespace
   - id: mixed-line-ending
   # Non-modifying checks:
   - id: name-tests-test
@@ -57,20 +58,20 @@
   - id: detect-private-key
   # Heavy checks:
   - id: check-ast
   - id: debug-statements
     language_version: python3
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.1
+  rev: v2.2.4
   hooks:
   - id: codespell
 
 - repo: https://github.com/adrienverge/yamllint.git
-  rev: v1.28.0
+  rev: v1.30.0
   hooks:
   - id: yamllint
     files: \.(yaml|yml)$
     types:
     - file
     - yaml
     args:
@@ -90,48 +91,50 @@
       D103,
       D107,
       E402,
       E501,
     additional_dependencies:
     - flake8-2020 ~= 1.7.0
     - flake8-pytest-style ~= 1.6.0
-    language_version: python3
 
 - repo: https://github.com/PyCQA/flake8.git
   # NOTE: This is kept at v4 for until WPS starts supporting flake v5.
   rev: 4.0.1  # enforce-version: 4.0.1
   hooks:
   - id: flake8
     alias: flake8-only-wps
     name: flake8 WPS-only
     args:
     - --ignore
+    # NOTE: WPS326: Found implicit string concatenation
+    # NOTE: WPS332: Found walrus operator
     - >-
       WPS102,
       WPS110,
       WPS111,
       WPS305,
+      WPS326,
+      WPS332,
       WPS347,
       WPS360,
       WPS421,
       WPS422,
       WPS432,
       WPS433,
       WPS437,
       WPS440,
       WPS441,
       WPS453,
     - --select
     - WPS
     additional_dependencies:
-    - wemake-python-styleguide ~= 0.16.1
-    language_version: python3
+    - wemake-python-styleguide ~= 0.17.0
 
 - repo: https://github.com/PyCQA/pylint.git
-  rev: v2.15.3
+  rev: v3.0.0a6
   hooks:
   - id: pylint
     args:
     - --disable
     - >-
       import-error,
       invalid-name,
```

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/Dockerfile` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -21,10 +21,11 @@
     pip install --user --upgrade --no-cache-dir --prefer-binary \
       -r requirements/runtime.in
 
 WORKDIR /app
 COPY LICENSE.md .
 COPY twine-upload.sh .
 COPY print-hash.py .
+COPY oidc-exchange.py .
 
 RUN chmod +x twine-upload.sh
 ENTRYPOINT ["/app/twine-upload.sh"]
```

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/LICENSE.md` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/README.md` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,65 +6,93 @@
 # PyPI publish GitHub Action
 
 This action allows you to upload your [Python distribution packages]
 in the `dist/` directory to PyPI.
 This text suggests a minimalistic usage overview. For more detailed
 walkthrough check out the [PyPA guide].
 
+If you have any feedback regarding specific action versions, please leave
+comments in the corresponding [per-release announcement discussions].
+
 
 ## 🌇 `master` branch sunset ❗
 
 The `master` branch version has been sunset. Please, change the GitHub
 Action version you use from `master` to `release/v1` or use an exact
 tag, or a full Git commit SHA.
 
 
 ## Usage
 
-To use the action add the following step to your workflow file (e.g.
-`.github/workflows/main.yml`)
+### Trusted publishing
 
+> **NOTE**: Trusted publishing is sometimes referred to by its
+> underlying technology -- OpenID Connect, or OIDC for short.
+> If you see references to "OIDC publishing" in the context of PyPI,
+> this is what they're referring to.
+
+This example jumps right into the current best practice. If you want to
+use API tokens directly or a less secure username and password, check out
+[how to specify username and password].
+
+This action supports PyPI's [trusted publishing]
+implementation, which allows authentication to PyPI without a manually
+configured API token or username/password combination. To perform
+[trusted publishing] with this action, your project's
+publisher must already be configured on PyPI.
+
+To enter the trusted publishing flow, configure this action's job with the
+`id-token: write` permission and **without** an explicit username or password:
+
+```yaml
+# .github/workflows/ci-cd.yml
+jobs:
+  pypi-publish:
+    name: Upload release to PyPI
+    runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/p/<your-pypi-project-name>
+    permissions:
+      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
+    steps:
+    # retrieve your distributions here
 
-```yml
-- name: Publish a Python distribution to PyPI
-  uses: pypa/gh-action-pypi-publish@release/v1
-  with:
-    password: ${{ secrets.PYPI_API_TOKEN }}
+    - name: Publish package distributions to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
 ```
 
 > **Pro tip**: instead of using branch pointers, like `unstable/v1`, pin
 versions of Actions that you use to tagged versions or sha1 commit identifiers.
 This will make your workflows more secure and better reproducible, saving you
 from sudden and unpleasant surprises.
 
-A common use case is to upload packages only on a tagged commit, to do so add a
-filter to the step:
+Other indices that support trusted publishing can also be used, like TestPyPI:
 
-
-```yml
-  if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+```yaml
+- name: Publish package distributions to TestPyPI
+  uses: pypa/gh-action-pypi-publish@release/v1
+  with:
+    repository-url: https://test.pypi.org/legacy/
 ```
+_(don't forget to update the environment name to `testpypi` or similar!)_
 
-So the full step would look like:
+> **Pro tip**: only set the `id-token: write` permission in the job that does
+> publishing, not globally. Also, try to separate building from publishing
+> — this makes sure that any scripts maliciously injected into the build
+> or test environment won't be able to elevate privileges while flying under
+> the radar.
 
+A common use case is to upload packages only on a tagged commit, to do so add a
+filter to the job:
 
 ```yml
-- name: Publish package
-  if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-  uses: pypa/gh-action-pypi-publish@release/v1
-  with:
-    password: ${{ secrets.PYPI_API_TOKEN }}
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
 ```
 
-The example above uses the new [API token][PyPI API token] feature of
-PyPI, which is recommended to restrict the access the action has.
-
-The secret used in `${{ secrets.PYPI_API_TOKEN }}` needs to be created on the
-settings page of your project on GitHub. See [Creating & using secrets].
-
 
 ## Non-goals
 
 This GitHub Action [has nothing to do with _building package
 distributions_]. Users are responsible for preparing dists for upload
 by putting them into the `dist/` folder prior to running this Action.
 
@@ -92,73 +120,75 @@
 
 
 ## Advanced release management
 
 For best results, figure out what kind of workflow fits your
 project's specific needs.
 
-For example, you could implement a parallel workflow that
+For example, you could implement a parallel job that
 pushes every commit to TestPyPI or your own index server,
 like `devpi`. For this, you'd need to (1) specify a custom
-`repository_url` value and (2) generate a unique version
+`repository-url` value and (2) generate a unique version
 number for each upload so that they'd not create a conflict.
 The latter is possible if you use `setuptools_scm` package but
 you could also invent your own solution based on the distance
 to the latest tagged commit.
 
-You'll need to create another token for a separate host and then
-[save it as a GitHub repo secret][Creating & using secrets].
+You'll need to create another token for a separate host and then [save it as a
+GitHub repo secret][Creating & using secrets] under an environment used in
+your job. Though, passing a password would disable the secretless [trusted
+publishing] so it's better to configure it instead, when publishing to TestPyPI
+and not something custom.
 
 The action invocation in this case would look like:
 ```yml
 - name: Publish package to TestPyPI
   uses: pypa/gh-action-pypi-publish@release/v1
   with:
     password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-    repository_url: https://test.pypi.org/legacy/
+    repository-url: https://test.pypi.org/legacy/
 ```
 
 ### Customizing target package dists directory
 
 You can change the default target directory of `dist/`
 to any directory of your liking. The action invocation
 would now look like:
 
 ```yml
 - name: Publish package to PyPI
   uses: pypa/gh-action-pypi-publish@release/v1
   with:
-    password: ${{ secrets.PYPI_API_TOKEN }}
-    packages_dir: custom-dir/
+    packages-dir: custom-dir/
 ```
 
 ### Disabling metadata verification
 
 It is recommended that you run `twine check` just after producing your files,
 but this also runs `twine check` before upload. You can also disable the twine
 check with:
 
 ```yml
    with:
-     verify_metadata: false
+     verify-metadata: false
 ```
 
 ### Tolerating release package file duplicates
 
 Sometimes, when you publish releases from multiple places, your workflow
 may hit race conditions. For example, when publishing from multiple CIs
 or even having workflows with the same steps triggered within GitHub
 Actions CI/CD for different events concerning the same high-level act.
 
-To facilitate this use-case, you may use `skip_existing` (disabled by
+To facilitate this use-case, you may use `skip-existing` (disabled by
 default) setting as follows:
 
 ```yml
    with:
-     skip_existing: true
+     skip-existing: true
 ```
 
 > **Pro tip**: try to avoid enabling this setting where possible. If you
 have steps for publishing to both PyPI and TestPyPI, consider only using
 it for the latter, having the former fail loudly on duplicates.
 
 ### For Debugging
@@ -173,29 +203,41 @@
 ### Showing hash values of files to be uploaded
 
 You may want to verify whether the files on PyPI were automatically uploaded by CI script.
 It will show SHA256, MD5, BLAKE2-256 values of files to be uploaded.
 
 ```yml
   with:
-    print_hash: true
+    print-hash: true
 ```
 
 ### Specifying a different username
 
 The default username value is `__token__`. If you publish to a custom
 registry that does not provide API tokens, like `devpi`, you may need to
 specify a custom username and password pair. This is how it's done.
 
 ```yml
   with:
     user: guido
     password: ${{ secrets.DEVPI_PASSWORD }}
 ```
 
+The secret used in `${{ secrets.DEVPI_PASSWORD }}` needs to be created on the
+environment page under the settings of your project on GitHub.
+See [Creating & using secrets].
+
+In the past, when publishing to PyPI, the most secure way of the access scoping
+for automatic publishing was to use the [API tokens][PyPI API token] feature of
+PyPI. One would make it project-scoped and save as an environment-bound secret
+in their GitHub repository settings, naming it `${{ secrets.PYPI_API_TOKEN }}`,
+for example. See [Creating & using secrets]. While still secure,
+[trusted publishing] is now encouraged over API tokens as a best practice
+on supported platforms (like GitHub).
+
 ## License
 
 The Dockerfile and associated scripts and documentation in this project
 are released under the [BSD 3-clause license](LICENSE.md).
 
 
 [🧪 GitHub Actions CI/CD workflow tests badge]:
@@ -204,20 +246,28 @@
 https://github.com/pypa/gh-action-pypi-publish/actions/workflows/self-smoke-test-action.yml?query=branch%3Aunstable%2Fv1
 
 [pre-commit.ci results page]:
 https://results.pre-commit.ci/latest/github/pypa/gh-action-pypi-publish/unstable/v1
 [pre-commit.ci status badge]:
 https://results.pre-commit.ci/badge/github/pypa/gh-action-pypi-publish/unstable/v1.svg
 
+[per-release announcement discussions]:
+https://github.com/pypa/gh-action-pypi-publish/discussions/categories/announcements
+
 [Creating & using secrets]:
 https://help.github.com/en/actions/automating-your-workflow-with-github-actions/creating-and-using-encrypted-secrets
 [has nothing to do with _building package distributions_]:
 https://github.com/pypa/gh-action-pypi-publish/issues/11#issuecomment-530480449
 [PyPA guide]:
 https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 [PyPI API token]: https://pypi.org/help/#apitoken
 [Python distribution packages]:
 https://packaging.python.org/glossary/#term-Distribution-Package
 [SWUbanner]:
 https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct-single.svg
 [SWUdocs]:
 https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+
+[warehouse#12965]: https://github.com/pypi/warehouse/issues/12965
+[trusted publishing]: https://docs.pypi.org/trusted-publishers/
+
+[how to specify username and password]: #specifying-a-different-username
```

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/print-hash.py` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/.github/actions/gh-action-pypi-publish-1.6.4/requirements/runtime.txt` & `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     # via requests
 commonmark==0.9.1
     # via rich
 cryptography>=39.0.1
     # via secretstorage
 docutils==0.19
     # via readme-renderer
+id==1.0.0
+    # via -r requirements/runtime.in
 idna==3.4
     # via requests
 importlib-metadata==5.1.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
@@ -36,36 +38,42 @@
     # via jaraco-classes
 pkginfo==1.9.2
     # via
     #   -r requirements/runtime.in
     #   twine
 pycparser==2.21
     # via cffi
+pydantic==1.10.6
+    # via id
 pygments==2.13.0
     # via
     #   readme-renderer
     #   rich
 readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests>=2.31.0
     # via
+    #   -r requirements/runtime.in
+    #   id
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==12.6.0
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 twine==4.0.1
     # via -r requirements/runtime.in
+typing-extensions==4.5.0
+    # via pydantic
 urllib3==1.26.13
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
 zipp==3.11.0
```

### Comparing `dolbyio-rest-apis-3.6.2/.github/workflows/build-package.yml` & `dolbyio-rest-apis-3.7.0/.github/workflows/build-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,13 @@
           python3 -m pip install --upgrade pip
           # Install the requirements
           python3 -m pip install -r requirements.txt
 
       - name: Run PyLint 🔧
         run: |
           # Run PyLint
-          python3 -m pylint client/src/dolbyio_rest_apis cli/src/dolbyio_rest_apis_cli
+          python3 -m pylint client/src/dolbyio_rest_apis
 
       - name: Build the packages 🔧
         run: |
           # Build the Python packages
           python3 client/setup.py sdist bdist_wheel
-          python3 cli/setup.py sdist bdist_wheel
```

### Comparing `dolbyio-rest-apis-3.6.2/.github/workflows/codeql-analysis.yml` & `dolbyio-rest-apis-3.7.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/.github/workflows/publish-package-to-pypi.yml` & `dolbyio-rest-apis-3.7.0/.github/workflows/publish-package-to-pypi.yml`

 * *Files 9% similar despite different names*

```diff
@@ -19,20 +19,19 @@
           python3 -m pip install --upgrade pip
           # Install the requirements
           python3 -m pip install -r requirements.txt
 
       - name: Run PyLint 🔧
         run: |
           # Run PyLint
-          python3 -m pylint client/src/dolbyio_rest_apis cli/src/dolbyio_rest_apis_cli
+          python3 -m pylint client/src/dolbyio_rest_apis
 
       - name: Build the packages 🔧
         run: |
           # Build the Python packages
           python3 client/setup.py sdist bdist_wheel
-          python3 cli/setup.py sdist bdist_wheel
 
       - name: Deploy to PyPI 🚀
-        uses: ./.github/actions/gh-action-pypi-publish-1.6.4
+        uses: ./.github/actions/gh-action-pypi-publish-1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `dolbyio-rest-apis-3.6.2/.gitignore` & `dolbyio-rest-apis-3.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/.pylintrc` & `dolbyio-rest-apis-3.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/LICENSE` & `dolbyio-rest-apis-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/PKG-INFO` & `dolbyio-rest-apis-3.7.0/client/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: dolbyio-rest-apis
-Version: 3.6.2
-Summary: A Python wrapper for the Dolby.io REST APIs.
-Home-page: https://github.com/dolbyio/dolbyio-rest-apis-client-python
-Author: Dolby.io
-Author-email: fabien.lavocat@dolby.com
-License: MIT
-Project-URL: Documentation, https://docs.dolby.io/communications-apis/reference
-Project-URL: Source, https://github.com/dolbyio/dolbyio-rest-apis-client-python
-Project-URL: Bug Tracker, https://github.com/dolbyio/dolbyio-rest-apis-client-python/issues
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Dolby.io REST APIs Client for Python
 
 Python wrapper for the dolby.io REST [Communications](https://docs.dolby.io/communications-apis/reference/authentication-api), [Streaming](https://docs.dolby.io/streaming-apis/reference) and [Media](https://docs.dolby.io/media-processing/reference/media-enhance-overview) APIs.
 
 ## Install this project
 
 Check the [dolbyio-rest-apis](https://pypi.org/project/dolbyio-rest-apis/) package on PyPI. To install the latest stable python package run the following command: 
@@ -67,46 +41,71 @@
 
 task = authentication.get_api_token(APP_KEY, APP_SECRET)
 at = loop.run_until_complete(task)
 
 print(f'API Token: {at.access_token}')
 ```
 
+To request a particular scope for this access token:
+
+```python
+task = authentication.get_api_token(APP_KEY, APP_SECRET, scope=['comms:*'])
+at = loop.run_until_complete(task)
+
+print(f'API Token: {at.access_token}')
+print(f'Scope: {at.scope}')
+```
+
 ## Communications Examples
 
 ### Get a client access token
 
 To get an access token that will be used by the client SDK for an end user to open a session against dolby.io, use the following code:
 
 ```python
 import asyncio
+from dolbyio_rest_apis import authentication as auth
 from dolbyio_rest_apis.communications import authentication
 
 APP_KEY = 'YOUR_APP_KEY'
 APP_SECRET = 'YOUR_APP_SECRET'
 
 loop = asyncio.get_event_loop()
 
-task = authentication.get_api_token(APP_KEY, APP_SECRET)
-at = loop.run_until_complete(task)
+# Request an API Token
+task = auth.get_api_token(APP_KEY, APP_SECRET, scope=['comms:client_access_token:create'])
+api_token = loop.run_until_complete(task)
+
+print(f'API Token: {api_token.access_token}')
+
+# Request the Client Access Token
+task = authentication.get_client_access_token_v2(api_token.access_token, ['*'])
+cat = loop.run_until_complete(task)
 
-print(f'Access Token: {at.access_token}')
+print(f'Client Access Token: {cat.access_token}')
 ```
 
 Because most of the APIs are asynchronous, you can write an async function like that:
 
 ```python
+from dolbyio_rest_apis import authentication as auth
 from dolbyio_rest_apis.communications import authentication
 
 APP_KEY = 'YOUR_APP_KEY'
 APP_SECRET = 'YOUR_APP_SECRET'
 
 async def get_client_access_token():
-    at = await authentication.get_client_access_token(APP_KEY, APP_SECRET)
-    print(f'Access Token: {at.access_token}')
+    # Request an API Token
+    api_token = await auth.get_api_token(APP_KEY, APP_SECRET, scope=['comms:client_access_token:create'])
+
+    # Request the Client Access Token
+    cat = await authentication.get_client_access_token_v2(api_token.access_token, ['*'])
+    print(f'Client Access Token: {cat.access_token}')
+    
+    return cat.access_token
 
 ```
 
 ### Create a conference
 
 To create a Dolby Voice conference, you first must retrieve an API Access Token, then use the following code to create the conference.
 
@@ -126,17 +125,18 @@
     Participant('hostA', [Permission.JOIN, Permission.SEND_AUDIO, Permission.SEND_VIDEO], notify=True),
     Participant('listener1', [Permission.JOIN], notify=False),
 ]
 
 loop = asyncio.get_event_loop()
 
 # Request an API token
-task = authentication.get_api_token(APP_KEY, APP_SECRET)
+task = authentication.get_api_token(APP_KEY, APP_SECRET, scope=['comms:conf:create'])
 at = loop.run_until_complete(task)
 
+# Create the conference
 task = conference.create_conference(
     at.access_token,
     owner_id,
     alias,
     video_codec=VideoCodec.VP8,
     participants=participants
 )
@@ -316,9 +316,7 @@
 task = io.download_file(
     access_token=at.access_token,
     dlb_url=output_url,
     file_path=OUT_FILE_PATH,
 )
 loop.run_until_complete(task)
 ```
-
-
```

### Comparing `dolbyio-rest-apis-3.6.2/README.md` & `dolbyio-rest-apis-3.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Publish Package](https://github.com/DolbyIO/dolbyio-rest-apis-client-python/actions/workflows/publish-package-to-pypi.yml/badge.svg)](https://github.com/DolbyIO/dolbyio-rest-apis-client-python/actions/workflows/publish-package-to-pypi.yml)
 ![PyPI](https://img.shields.io/pypi/v/dolbyio-rest-apis)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dolbyio-rest-apis)
 [![License](https://img.shields.io/github/license/DolbyIO/dolbyio-rest-apis-client-python)](LICENSE)
 
 # Dolby.io REST APIs Client for Python
 
-Python wrapper for the dolby.io REST [Communications](https://docs.dolby.io/communications-apis/reference/authentication-api), [Streaming](https://docs.dolby.io/streaming-apis/reference) and [Media](https://docs.dolby.io/media-processing/reference/media-enhance-overview) APIs. It also contains a Command Line Interface utility.
+Python wrapper for the dolby.io REST [Communications](https://docs.dolby.io/communications-apis/reference/authentication-api), [Streaming](https://docs.dolby.io/streaming-apis/reference) and [Media](https://docs.dolby.io/media-processing/reference/media-enhance-overview) APIs.
 
 ## Build the builder
 
 Install the package dependencies to build the installers:
 
 ```bash
 python3 -m pip install -r requirements.txt
@@ -26,30 +26,14 @@
 
 Build this project wheel:
 
 ```bash
 python3 client/setup.py sdist bdist_wheel
 ```
 
-## Build the CLI project
-
-Install the package dependencies to build and run this project:
-
-```bash
-python3 -m pip install -r cli/requirements.txt
-```
-
-Build this project wheel:
-
-```bash
-python3 cli/setup.py sdist bdist_wheel
-```
-
 ## Run PyLint on the code
 
 Run the following [pylint](https://pylint.org/) command:
 
 ```bash
-python3 -m pylint \
-    client/src/dolbyio_rest_apis \
-    cli/src/dolbyio_rest_apis_cli
+python3 -m pylint client/src/dolbyio_rest_apis
 ```
```

### Comparing `dolbyio-rest-apis-3.6.2/cli/setup.py` & `dolbyio-rest-apis-3.7.0/client/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,35 +11,29 @@
 with open(os.path.join(current_path, 'README.md'), 'r', encoding='UTF-8') as f:
     long_description = f.read()
 
 with open(os.path.join(current_path, 'requirements.txt'), 'r', encoding='UTF-8') as f:
     requirements = f.readlines()
 
 setuptools.setup(
-    name='dolbyio-rest-apis-cli',
+    name='dolbyio-rest-apis',
     author='Dolby.io',
     author_email='fabien.lavocat@dolby.com',
-    description='A command line wrapper for the Dolby.io REST APIs.',
+    description='A Python wrapper for the Dolby.io REST APIs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/dolbyio/dolbyio-rest-apis-client-python',
     project_urls={
         'Documentation': 'https://docs.dolby.io/communications-apis/reference',
         'Source': 'https://github.com/dolbyio/dolbyio-rest-apis-client-python',
         'Bug Tracker': 'https://github.com/dolbyio/dolbyio-rest-apis-client-python/issues',
     },
     package_dir={'': os.path.join(current_path, 'src')},
     packages=setuptools.find_packages(where=os.path.join(current_path, 'src')),
-    entry_points={
-        'console_scripts': [
-            'communications=dolbyio_rest_apis_cli.communications.cli:cli',
-            'media=dolbyio_rest_apis_cli.media.cli:cli',
-        ],
-    },
     python_requires='>=3.7',
     use_scm_version= {
         'local_scheme': 'no-local-version',
         'version_scheme': 'release-branch-semver',
     },
     setup_requires=[
         'setuptools_scm',
```

### Comparing `dolbyio-rest-apis-3.6.2/client/README.md` & `dolbyio-rest-apis-3.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: dolbyio-rest-apis
+Version: 3.7.0
+Summary: A Python wrapper for the Dolby.io REST APIs.
+Home-page: https://github.com/dolbyio/dolbyio-rest-apis-client-python
+Author: Dolby.io
+Author-email: fabien.lavocat@dolby.com
+License: MIT
+Project-URL: Documentation, https://docs.dolby.io/communications-apis/reference
+Project-URL: Source, https://github.com/dolbyio/dolbyio-rest-apis-client-python
+Project-URL: Bug Tracker, https://github.com/dolbyio/dolbyio-rest-apis-client-python/issues
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Dolby.io REST APIs Client for Python
 
 Python wrapper for the dolby.io REST [Communications](https://docs.dolby.io/communications-apis/reference/authentication-api), [Streaming](https://docs.dolby.io/streaming-apis/reference) and [Media](https://docs.dolby.io/media-processing/reference/media-enhance-overview) APIs.
 
 ## Install this project
 
 Check the [dolbyio-rest-apis](https://pypi.org/project/dolbyio-rest-apis/) package on PyPI. To install the latest stable python package run the following command: 
@@ -41,46 +67,71 @@
 
 task = authentication.get_api_token(APP_KEY, APP_SECRET)
 at = loop.run_until_complete(task)
 
 print(f'API Token: {at.access_token}')
 ```
 
+To request a particular scope for this access token:
+
+```python
+task = authentication.get_api_token(APP_KEY, APP_SECRET, scope=['comms:*'])
+at = loop.run_until_complete(task)
+
+print(f'API Token: {at.access_token}')
+print(f'Scope: {at.scope}')
+```
+
 ## Communications Examples
 
 ### Get a client access token
 
 To get an access token that will be used by the client SDK for an end user to open a session against dolby.io, use the following code:
 
 ```python
 import asyncio
+from dolbyio_rest_apis import authentication as auth
 from dolbyio_rest_apis.communications import authentication
 
 APP_KEY = 'YOUR_APP_KEY'
 APP_SECRET = 'YOUR_APP_SECRET'
 
 loop = asyncio.get_event_loop()
 
-task = authentication.get_api_token(APP_KEY, APP_SECRET)
-at = loop.run_until_complete(task)
+# Request an API Token
+task = auth.get_api_token(APP_KEY, APP_SECRET, scope=['comms:client_access_token:create'])
+api_token = loop.run_until_complete(task)
+
+print(f'API Token: {api_token.access_token}')
+
+# Request the Client Access Token
+task = authentication.get_client_access_token_v2(api_token.access_token, ['*'])
+cat = loop.run_until_complete(task)
 
-print(f'Access Token: {at.access_token}')
+print(f'Client Access Token: {cat.access_token}')
 ```
 
 Because most of the APIs are asynchronous, you can write an async function like that:
 
 ```python
+from dolbyio_rest_apis import authentication as auth
 from dolbyio_rest_apis.communications import authentication
 
 APP_KEY = 'YOUR_APP_KEY'
 APP_SECRET = 'YOUR_APP_SECRET'
 
 async def get_client_access_token():
-    at = await authentication.get_client_access_token(APP_KEY, APP_SECRET)
-    print(f'Access Token: {at.access_token}')
+    # Request an API Token
+    api_token = await auth.get_api_token(APP_KEY, APP_SECRET, scope=['comms:client_access_token:create'])
+
+    # Request the Client Access Token
+    cat = await authentication.get_client_access_token_v2(api_token.access_token, ['*'])
+    print(f'Client Access Token: {cat.access_token}')
+    
+    return cat.access_token
 
 ```
 
 ### Create a conference
 
 To create a Dolby Voice conference, you first must retrieve an API Access Token, then use the following code to create the conference.
 
@@ -100,17 +151,18 @@
     Participant('hostA', [Permission.JOIN, Permission.SEND_AUDIO, Permission.SEND_VIDEO], notify=True),
     Participant('listener1', [Permission.JOIN], notify=False),
 ]
 
 loop = asyncio.get_event_loop()
 
 # Request an API token
-task = authentication.get_api_token(APP_KEY, APP_SECRET)
+task = authentication.get_api_token(APP_KEY, APP_SECRET, scope=['comms:conf:create'])
 at = loop.run_until_complete(task)
 
+# Create the conference
 task = conference.create_conference(
     at.access_token,
     owner_id,
     alias,
     video_codec=VideoCodec.VP8,
     participants=participants
 )
@@ -290,7 +342,9 @@
 task = io.download_file(
     access_token=at.access_token,
     dlb_url=output_url,
     file_path=OUT_FILE_PATH,
 )
 loop.run_until_complete(task)
 ```
+
+
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/conference.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/conference.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/internal/http_context.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/http_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 
     async def _requests_post_put(
             self,
             access_token: str,
             url: str,
             method: str,
             payload: Any=None,
+            extra_headers: Dict[str, str]=None,
         ) -> Any or None:
         r"""
         Sends a POST or PUT request.
 
         Args:
             access_token: The Access Token to use for authentication.
             url: Where to send the request to.
             method: HTTP method, POST or PUT.
             payload: (Optional) Content of the request.
+            extra_headers: (Optional) Add extra HTTP headers in the request.
 
         Returns:
             The JSON response if any or None.
 
         Raises:
             HttpRequestError: If a client error one occurred.
             HTTPError: If one occurred.
@@ -47,14 +49,17 @@
 
         headers = {
             'Accept': 'application/json',
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {access_token}',
         }
 
+        if extra_headers is not None:
+            headers.update(extra_headers)
+
         if payload is None:
             payload = '{}' # The REST APIs don't support an empty payload
         else:
             payload = json.dumps(payload, indent=4)
 
         return await self._send_request(
             method=method,
@@ -93,36 +98,39 @@
         )
 
     async def requests_post(
             self,
             access_token: str,
             url: str,
             payload: Any=None,
+            extra_headers: Dict[str, str]=None,
         ) -> Any or None:
         r"""
         Sends a POST request.
 
         Args:
             access_token: The Access Token to use for authentication.
             url: Where to send the request to.
             payload: (Optional) Content of the request.
+            extra_headers: (Optional) Add extra HTTP headers in the request.
 
         Returns:
             The JSON response if any or None.
 
         Raises:
             HttpRequestError: If a client error one occurred.
             HTTPError: If one occurred.
         """
 
         return await self._requests_post_put(
             access_token=access_token,
             url=url,
             method='POST',
-            payload=payload
+            payload=payload,
+            extra_headers=extra_headers,
         )
 
     async def requests_post_basic_auth(
             self,
             app_key: str,
             app_secret: str,
             url: str,
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/models.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/models.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/conferences.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/conferences.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/models.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/models.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/recordings.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/recordings.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/recording.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/recording.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/remix.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/remix.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/communications/streaming.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/streaming.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/helpers.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/helpers.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/http_context.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/http_request_error.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_request_error.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/rate_limiter.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/core/urls.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 
 This module contains the URLs to use to call the REST APIs.
 """
 
 API_URL = 'api.dolby.io'
 
 COMMS_URL = 'comms.api.dolby.io'
-COMMS_SESSION_URL = 'session.voxeet.com/v1'
+COMMS_SESSION_URL = 'session.voxeet.com'
 
 SAPI_URL = 'api.millicast.com'
 
 MAPI_URL = 'api.dolby.com'
 
 def get_api_url() -> str:
     return f'https://{API_URL}/v1'
 
+def get_comms_url_v1() -> str:
+    return f'https://{COMMS_URL}/v1'
+
 def get_comms_monitor_url() -> str:
-    return f'https://{COMMS_URL}/v1/monitor'
+    return f'{get_comms_url_v1()}/monitor'
 
 def get_comms_url_v2(region: str = None) -> str:
     if region is None:
         return f'https://{COMMS_URL}/v2'
     return f'https://{region}.{COMMS_URL}/v2'
 
 def get_comms_session_url() -> str:
-    return f'https://{COMMS_SESSION_URL}'
+    return f'https://{COMMS_SESSION_URL}/v1'
 
 def get_rts_url() -> str:
     return f'https://{SAPI_URL}'
 
 def get_mapi_url() -> str:
     return f'https://{MAPI_URL}'
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/analyze.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/analyze_music.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_music.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/analyze_speech.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_speech.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/diagnose.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/diagnose.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/enhance.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/enhance.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/internal/http_context.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/io.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/io.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/jobs.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/jobs.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/mastering.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/mastering.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """
-dolbyio_rest_apis.media.models.analyze_music_response
+dolbyio_rest_apis.media.models.analyze_speech_response
 ~~~~~~~~~~~~~~~
 
-This module contains the Analyze Music model.
+This module contains the Analyze Speech model.
 """
 
 from .job_response import JobResponse
 
-class AnalyzeMusicJobResult(dict):
-    """The :class:`AnalyzeMusicJobResult` object, which represents the result for an analyze music job."""
+class AnalyzeSpeechJobResult(dict):
+    """The :class:`AnalyzeSpeechJobResult` object, which represents the result for an analyze speech job."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        if 'media_info' in dictionary:
-            self.media_info = dictionary['media_info']
-        if 'processed_region' in dictionary:
-            self.media_info = dictionary['processed_region']
-
-class AnalyzeMusicJob(JobResponse):
-    """The :class:`AnalyzeMusicJob` object, which represents the result for an analyze music job."""
+class AnalyzeSpeechJob(JobResponse):
+    """The :class:`AnalyzeSpeechJob` object, which represents the result for an analyze speech job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = AnalyzeMusicJobResult(dictionary)
+            self.result = AnalyzeSpeechJobResult(dictionary['result'])
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/analyze_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/enhance_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """
-dolbyio_rest_apis.media.models.analyze_response
+dolbyio_rest_apis.media.models.enhance_response
 ~~~~~~~~~~~~~~~
 
-This module contains the Analyze models.
+This module contains the Enhance Response model.
 """
 
+from dolbyio_rest_apis.core.helpers import get_value_or_default
 from .job_response import JobResponse
 
-class AnalyzeJobResult(dict):
-    """The :class:`AnalyzeJobResult` object, which represents the result for an analyze job."""
+class EnhanceJobResult(dict):
+    """The :class:`EnhanceJobResult` object, which represents the result for an enhance job."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        if 'media_info' in dictionary:
-            self.media_info = dictionary['media_info']
-        if 'processed_region' in dictionary:
-            self.media_info = dictionary['processed_region']
+        self.version = get_value_or_default(dictionary, 'version', None)
 
-class AnalyzeJobResponse(JobResponse):
-    """The :class:`AnalyzeJobResponse` object, which represents the result for an analyze job."""
+class EnhanceJob(JobResponse):
+    """The :class:`EnhanceJob` object, which represents the result for an enhance job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = AnalyzeJobResult(dictionary)
+            self.result = EnhanceJobResult(dictionary['result'])
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/diagnose_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/diagnose_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 class DiagnoseJob(JobResponse):
     """The :class:`DiagnoseJob` object, which represents the result for a diagnose job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = DiagnoseJobResult(dictionary)
+            self.result = DiagnoseJobResult(dictionary['result'])
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/enhance_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """
-dolbyio_rest_apis.media.models.enhance_response
+dolbyio_rest_apis.media.models.analyze_response
 ~~~~~~~~~~~~~~~
 
-This module contains the Enhance Response model.
+This module contains the Analyze models.
 """
 
-from dolbyio_rest_apis.core.helpers import get_value_or_default
 from .job_response import JobResponse
 
-class EnhanceJobResult(dict):
-    """The :class:`EnhanceJobResult` object, which represents the result for an enhance job."""
+class AnalyzeJobResult(dict):
+    """The :class:`AnalyzeJobResult` object, which represents the result for an analyze job."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        self.version = get_value_or_default(dictionary, 'version', None)
-
-class EnhanceJob(JobResponse):
-    """The :class:`EnhanceJob` object, which represents the result for an enhance job."""
+class AnalyzeJobResponse(JobResponse):
+    """The :class:`AnalyzeJobResponse` object, which represents the result for an analyze job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = EnhanceJobResult(dictionary)
+            self.result = AnalyzeJobResult(dictionary['result'])
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/job_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/job_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/jobs_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/jobs_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/mastering_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/mastering_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class MasteringPreviewJob(JobResponse):
     """The :class:`MasteringPreviewJob` object, which represents the result for a mastering preview job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = MasteringPreviewJobResult(dictionary)
+            self.result = MasteringPreviewJobResult(dictionary['result'])
 
 class MasteringJobResult(MasteringPreviewJobResult):
     """The :class:`MasteringJobResult` object, which represents the result for a mastering job."""
 
     def __init__(self, dictionary: dict):
         MasteringPreviewJobResult.__init__(self, dictionary)
 
@@ -36,8 +36,8 @@
 class MasteringJob(JobResponse):
     """The :class:`MasteringJob` object, which represents the result for a mastering job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = MasteringJobResult(dictionary)
+            self.result = MasteringJobResult(dictionary['result'])
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/result_error.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/result_error.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/transcode_response.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/transcode_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 class TranscodeJob(JobResponse):
     """The :class:`TranscodeJob` object, which represents the result for a transcode job."""
 
     def __init__(self, job_id, dictionary: dict):
         JobResponse.__init__(self, job_id, dictionary)
 
         if 'result' in dictionary:
-            self.result = TranscodeJobResult(dictionary)
+            self.result = TranscodeJobResult(dictionary['result'])
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/models/webhook.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/webhook.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/transcode.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/transcode.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/media/webhooks.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/webhooks.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/models.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,7 +13,8 @@
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
         self.token_type = get_value_or_default(self, 'token_type', None)
         self.access_token = get_value_or_default(self, 'access_token', None)
         self.refresh_token = get_value_or_default(self, 'refresh_token', None)
         self.expires_in_val = get_value_or_default(self, 'expires_in', 0)
+        self.scope = get_value_or_default(self, 'scope', None)
```

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/cluster.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/cluster.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/internal/http_context.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/cluster.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/cluster.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/core.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/core.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/publish_token.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/publish_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/publish_token.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/publish_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/stream.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/stream.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.6.2/client/src/dolbyio_rest_apis/streaming/subscribe_token.py` & `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/subscribe_token.py`

 * *Files identical despite different names*

