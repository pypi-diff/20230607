# Comparing `tmp/invenio-drafts-resources-1.4.0.tar.gz` & `tmp/invenio-drafts-resources-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-drafts-resources-1.4.0.tar", last modified: Tue Apr 25 08:00:38 2023, max compression
+gzip compressed data, was "dist/invenio-drafts-resources-1.4.1.tar", last modified: Wed Jun  7 14:03:26 2023, max compression
```

## Comparing `invenio-drafts-resources-1.4.0.tar` & `invenio-drafts-resources-1.4.1.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/systemfields/parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/systemfields/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/mock_module/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/records/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/resources/test_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/resources/test_resource_links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:00:38.000000 invenio-drafts-resources-1.4.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/test_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/test_record_service_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/test_record_service_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/test_record_service_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 08:00:32.000000 invenio-drafts-resources-1.4.0/tests/services/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/mock_module/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/records/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/test_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/resources/test_resource_links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:03:25.000000 invenio-drafts-resources-1.4.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_record_service_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-07 14:03:19.000000 invenio-drafts-resources-1.4.1/tests/services/utils.py
```

### Comparing `invenio-drafts-resources-1.4.0/.editorconfig` & `invenio-drafts-resources-1.4.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/.github/workflows/i18n-pull.yml` & `invenio-drafts-resources-1.4.1/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/.github/workflows/i18n-push.yml` & `invenio-drafts-resources-1.4.1/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/.github/workflows/pypi-publish.yml` & `invenio-drafts-resources-1.4.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/.github/workflows/tests.yml` & `invenio-drafts-resources-1.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/.tx/config` & `invenio-drafts-resources-1.4.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/CHANGES.rst` & `invenio-drafts-resources-1.4.1/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 1.4.1 (2023-06-06)
+
+- fix permission check for managing files
+
 Version 1.4.0 (2023-04-25)
 
 - upgrade invenio-records-resources
 - ensure testing of file indexing
 
 Version 1.3.0 (2023-04-20)
```

### Comparing `invenio-drafts-resources-1.4.0/CONTRIBUTING.rst` & `invenio-drafts-resources-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/LICENSE` & `invenio-drafts-resources-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/MANIFEST.in` & `invenio-drafts-resources-1.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/PKG-INFO` & `invenio-drafts-resources-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.4.0
+Version: 1.4.1
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,18 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.4.1 (2023-06-06)
+        
+        - fix permission check for managing files
+        
         Version 1.4.0 (2023-04-25)
         
         - upgrade invenio-records-resources
         - ensure testing of file indexing
         
         Version 1.3.0 (2023-04-20)
```

### Comparing `invenio-drafts-resources-1.4.0/README.rst` & `invenio-drafts-resources-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/babel.ini` & `invenio-drafts-resources-1.4.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/docs/Makefile` & `invenio-drafts-resources-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/docs/conf.py` & `invenio-drafts-resources-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/docs/index.rst` & `invenio-drafts-resources-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/docs/make.bat` & `invenio-drafts-resources-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/__init__.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/api.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/models.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/systemfields/parent.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/records/systemfields/versions.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/records/systemfields/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/args.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/config.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/errors.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/resources/records/resource.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/__init__.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/base.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/files.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
         NOTE: `record` actually refers to the draft
               (this interface is used in records-resources and rdm-records)
         """
         draft = record
         enabled = data.get("files", {}).get("enabled", True)
 
         if draft.files.enabled != enabled:
-            if not self.service.check_permission(identity, "manage_files"):
+            if not self.service.check_permission(
+                identity, "manage_files", record=draft
+            ):
                 errors.append(
                     {
                         "field": "files.enabled",
                         "messages": [
                             _("You don't have permissions to manage files options.")
                         ],
                     }
@@ -59,15 +61,17 @@
               (this interface is used in records-resources and rdm-records)
         """
         draft = record
         enabled = data.get("files", {}).get("enabled", True)
         default_preview = data.get("files", {}).get("default_preview")
 
         if draft.files.enabled != enabled:
-            if not self.service.check_permission(identity, "manage_files"):
+            if not self.service.check_permission(
+                identity, "manage_files", record=draft
+            ):
                 errors.append(
                     {
                         "field": "files.enabled",
                         "messages": [
                             _("You don't have permissions to manage files options.")
                         ],
                     }
```

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/metadata.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/pid.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/pid.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,12 @@
             record.register()
 
     def delete_draft(self, identity, draft=None, record=None, force=False):
         """Unregister persistent identifiers for unpublished drafts."""
         if force:
             draft.__class__.pid.session_merge(draft)
             draft.pid.delete()
-            draft.parent.__class__.pid.session_merge(draft.parent)
-            draft.parent.pid.delete()
+
+            # Only delete parent PID if there are no other versions
+            if draft.versions.latest_index == 1:
+                draft.parent.__class__.pid.session_merge(draft.parent)
+                draft.parent.pid.delete()
```

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/components/relations.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/config.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/permissions.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/schema.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/search_params.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/search_params.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/service.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/services/records/tasks.py` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/services/records/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/messages.pot` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/PKG-INFO` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.4.0
+Version: 1.4.1
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,18 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.4.1 (2023-06-06)
+        
+        - fix permission check for managing files
+        
         Version 1.4.0 (2023-04-25)
         
         - upgrade invenio-records-resources
         - ensure testing of file indexing
         
         Version 1.3.0 (2023-04-20)
```

### Comparing `invenio-drafts-resources-1.4.0/invenio_drafts_resources.egg-info/SOURCES.txt` & `invenio-drafts-resources-1.4.1/invenio_drafts_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/run-tests.sh` & `invenio-drafts-resources-1.4.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/setup.cfg` & `invenio-drafts-resources-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/conftest.py` & `invenio-drafts-resources-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/api.py` & `invenio-drafts-resources-1.4.1/tests/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.4.1/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/models.py` & `invenio-drafts-resources-1.4.1/tests/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/permissions.py` & `invenio-drafts-resources-1.4.1/tests/mock_module/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/resource.py` & `invenio-drafts-resources-1.4.1/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/schemas.py` & `invenio-drafts-resources-1.4.1/tests/mock_module/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/mock_module/service.py` & `invenio-drafts-resources-1.4.1/tests/mock_module/service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/records/conftest.py` & `invenio-drafts-resources-1.4.1/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/records/test_api.py` & `invenio-drafts-resources-1.4.1/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/resources/conftest.py` & `invenio-drafts-resources-1.4.1/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/resources/test_files_resource.py` & `invenio-drafts-resources-1.4.1/tests/resources/test_files_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/resources/test_record_resource.py` & `invenio-drafts-resources-1.4.1/tests/resources/test_record_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/resources/test_resource_links.py` & `invenio-drafts-resources-1.4.1/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/services/conftest.py` & `invenio-drafts-resources-1.4.1/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/services/test_record_service.py` & `invenio-drafts-resources-1.4.1/tests/services/test_record_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -275,14 +275,68 @@
     assert record_2.id
     assert record_2._record.pid.status == PIDStatus.REGISTERED
     assert record_2._record.parent.pid.status == PIDStatus.REGISTERED
     assert record_2._record.revision_id == 1
     assert record_2["id"] != record["id"]
 
 
+def test_multi_version_delete_draft(app, service, identity_simple, input_data):
+    """Test deleting drafts of a multi-version record.
+
+    Both individual version PIDs and parent PID should stay 'REGISTERED' when deleting
+    drafts of a multi-version record.
+    """
+    record = create_and_publish(service, identity_simple, input_data)
+    recid_v1 = record.id
+
+    def assert_record_pids_status(recid):
+        record = service.read(identity_simple, recid)
+        assert record._record.pid.status == PIDStatus.REGISTERED
+        assert record._record.parent.pid.status == PIDStatus.REGISTERED
+
+    # Edit record v1
+    draft = service.edit(identity_simple, recid_v1)
+    assert_record_pids_status(recid_v1)
+
+    # Delete edit draft of record v1
+    service.delete_draft(identity_simple, draft.id)
+    assert_record_pids_status(recid_v1)
+
+    # Create new version (v2)
+    draft = service.new_version(identity_simple, recid_v1)
+    assert_record_pids_status(recid_v1)
+
+    # Delete new version (v2) draft
+    service.delete_draft(identity_simple, draft.id)
+    assert_record_pids_status(recid_v1)
+
+    # Create new version (v2) and publish
+    draft = service.new_version(identity_simple, recid_v1)
+    record_v2 = service.publish(identity_simple, draft.id)
+    recid_v2 = record_v2.id
+    assert_record_pids_status(recid_v1)
+    assert_record_pids_status(recid_v2)
+
+    # Edit both record v1 and v2
+    draft_v1 = service.edit(identity_simple, recid_v1)
+    draft_v2 = service.edit(identity_simple, recid_v2)
+    assert_record_pids_status(recid_v1)
+    assert_record_pids_status(recid_v2)
+
+    # Delete draft v1
+    service.delete_draft(identity_simple, draft_v1.id)
+    assert_record_pids_status(recid_v1)
+    assert_record_pids_status(recid_v2)
+
+    # Delete draft v2
+    service.delete_draft(identity_simple, draft_v2.id)
+    assert_record_pids_status(recid_v1)
+    assert_record_pids_status(recid_v2)
+
+
 def test_read_latest_version(app, service, identity_simple, input_data):
     """Test read the latest version of a record.
 
     This tests the `read_latest` service method.
     """
     record = create_and_publish(service, identity_simple, input_data)
     recid = record.id
```

### Comparing `invenio-drafts-resources-1.4.0/tests/services/test_record_service_files.py` & `invenio-drafts-resources-1.4.1/tests/services/test_record_service_files.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/services/test_record_service_search.py` & `invenio-drafts-resources-1.4.1/tests/services/test_record_service_search.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/services/test_record_service_tasks.py` & `invenio-drafts-resources-1.4.1/tests/services/test_record_service_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/services/test_services.py` & `invenio-drafts-resources-1.4.1/tests/services/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.0/tests/services/utils.py` & `invenio-drafts-resources-1.4.1/tests/services/utils.py`

 * *Files identical despite different names*

