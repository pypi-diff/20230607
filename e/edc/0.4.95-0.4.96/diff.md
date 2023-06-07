# Comparing `tmp/edc-0.4.95.tar.gz` & `tmp/edc-0.4.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.95.tar", last modified: Wed May 24 22:36:37 2023, max compression
+gzip compressed data, was "edc-0.4.96.tar", last modified: Wed Jun  7 13:54:47 2023, max compression
```

## Comparing `edc-0.4.95.tar` & `edc-0.4.96.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.509508 edc-0.4.95/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.95/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.95/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.95/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.95/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    39702 2023-05-24 22:36:29.000000 edc-0.4.95/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.95/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.95/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-24 22:36:37.509620 edc-0.4.95/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.95/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.496277 edc-0.4.95/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.499094 edc-0.4.95/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.95/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.95/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.95/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.499766 edc-0.4.95/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.95/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.95/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.95/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.95/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.501034 edc-0.4.95/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.95/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.504871 edc-0.4.95/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.95/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.95/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.95/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.95/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.95/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.95/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.95/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.95/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.95/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.95/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.95/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.95/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.95/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.95/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.95/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.95/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.95/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.95/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.95/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.505756 edc-0.4.95/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-24 22:36:37.000000 edc-0.4.95/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-24 22:36:37.000000 edc-0.4.95/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 22:36:37.000000 edc-0.4.95/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.95/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1923 2023-05-24 22:36:37.000000 edc-0.4.95/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-24 22:36:37.000000 edc-0.4.95/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.505862 edc-0.4.95/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.95/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.95/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.508945 edc-0.4.95/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.95/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.95/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.95/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.95/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.95/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.95/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.95/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.95/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.95/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.95/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.95/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2995 2023-05-24 22:36:37.510033 edc-0.4.95/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 22:36:37.509280 edc-0.4.95/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.95/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.95/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.458735 edc-0.4.96/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.96/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.96/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.96/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.96/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    39972 2023-06-07 13:54:37.000000 edc-0.4.96/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.96/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.96/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-06-07 13:54:47.458843 edc-0.4.96/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.96/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.444782 edc-0.4.96/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.448116 edc-0.4.96/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.96/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.96/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.96/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.448855 edc-0.4.96/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.96/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.96/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.96/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.96/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.450086 edc-0.4.96/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.96/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.454115 edc-0.4.96/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.96/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.96/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.96/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.96/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.96/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.96/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.96/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.96/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.96/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.96/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.96/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.96/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.96/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.96/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.96/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.96/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.96/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.96/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.96/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.455224 edc-0.4.96/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-06-07 13:54:47.000000 edc-0.4.96/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-06-07 13:54:47.000000 edc-0.4.96/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-06-07 13:54:47.000000 edc-0.4.96/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.96/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1923 2023-06-07 13:54:47.000000 edc-0.4.96/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-06-07 13:54:47.000000 edc-0.4.96/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.455352 edc-0.4.96/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.96/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.96/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.458264 edc-0.4.96/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.96/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.96/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.96/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.96/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.96/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.96/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.96/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.96/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.96/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.96/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.96/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2995 2023-06-07 13:54:47.459259 edc-0.4.96/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-06-07 13:54:47.458549 edc-0.4.96/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.96/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.96/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.95/.gitignore` & `edc-0.4.96/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/.pre-commit-config.yaml` & `edc-0.4.96/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/CHANGES` & `edc-0.4.96/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 -------
 
+0.4.96
+------
+- minor fix access id via lookup sep instead of '.' in get_display_appt_type
+  (edc-appointment)
+- use local fields instead of across lookups on admin (edc-subject_visit)
+- add new code for revised HE crf (edc-he)
+- add new code for new QoL CRF (edc-qol)
+
 0.4.95
 ------
 - add model admin mixins (edc-qol)
 
 0.4.94
 ------
 - add mixins for new HE crf (edc-he)
```

### Comparing `edc-0.4.95/LICENSE` & `edc-0.4.96/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/PKG-INFO` & `edc-0.4.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.95
+Version: 0.4.96
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.95/README.rst` & `edc-0.4.96/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/bin/nginx/edc-uat.conf` & `edc-0.4.96/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/bin/nginx/edc.conf` & `edc-0.4.96/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/bin/scripts/dev_repos.sh` & `edc-0.4.96/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/bin/scripts/update_edc.sh` & `edc-0.4.96/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/bin/systemd/celery-uat.service` & `edc-0.4.96/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/bin/systemd/celery.service` & `edc-0.4.96/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/Makefile` & `edc-0.4.96/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/README.rst` & `edc-0.4.96/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/backup.rst` & `edc-0.4.96/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/celery.rst` & `edc-0.4.96/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/conda.rst` & `edc-0.4.96/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/conf.py` & `edc-0.4.96/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/configure_web_services.rst` & `edc-0.4.96/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/deploy_new_droplet.rst` & `edc-0.4.96/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/exporting_encrypted_data.rst` & `edc-0.4.96/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/forms_reference.md` & `edc-0.4.96/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/landing_page.rst` & `edc-0.4.96/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/make.bat` & `edc-0.4.96/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/prepare_database.rst` & `edc-0.4.96/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/printing.rst` & `edc-0.4.96/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/docs/update_deployment.rst` & `edc-0.4.96/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/edc.egg-info/PKG-INFO` & `edc-0.4.96/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.95
+Version: 0.4.96
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.95/edc.egg-info/SOURCES.txt` & `edc-0.4.96/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/edc.egg-info/requires.txt` & `edc-0.4.96/edc.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 django-revision==0.3.6
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
 edc-action-item==0.3.52
 edc-adherence==0.1.21
 edc-adverse-event==0.3.51
-edc-appointment==0.3.71
+edc-appointment==0.3.72
 edc-auth==0.3.60
 edc-consent==0.3.45
 edc-constants==0.3.48
 edc-crf==0.3.42
 edc-dashboard==0.3.45
 edc-data-manager==0.3.53
 edc-device==0.3.11
@@ -87,9 +87,9 @@
 edc-subject-dashboard==0.3.36
 edc-subject-model-wrappers==0.3.15
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
 edc-unblinding==0.1.14
 edc-utils==0.3.20
 edc-visit-schedule==0.3.61
-edc-visit-tracking==0.3.51
+edc-visit-tracking==0.3.52
 edc-vitals==0.1.11
```

### Comparing `edc-0.4.95/image/icon-pycharm.png` & `edc-0.4.96/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/requirements.tests/edc.txt` & `edc-0.4.96/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/requirements.tests/edc_dev.txt` & `edc-0.4.96/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.95/setup.cfg` & `edc-0.4.96/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	django-revision==0.3.6
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
 	edc-action-item==0.3.52
 	edc-adherence==0.1.21
 	edc-adverse-event==0.3.51
-	edc-appointment==0.3.71
+	edc-appointment==0.3.72
 	edc-auth==0.3.60
 	edc-consent==0.3.45
 	edc-constants==0.3.48
 	edc-crf==0.3.42
 	edc-dashboard==0.3.45
 	edc-data-manager==0.3.53
 	edc-device==0.3.11
@@ -116,15 +116,15 @@
 	edc-subject-dashboard==0.3.36
 	edc-subject-model-wrappers==0.3.15
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
 	edc-unblinding==0.1.14
 	edc-utils==0.3.20
 	edc-visit-schedule==0.3.61
-	edc-visit-tracking==0.3.51
+	edc-visit-tracking==0.3.52
 	edc-vitals==0.1.11
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
```

### Comparing `edc-0.4.95/utils/get_edc_requirements.py` & `edc-0.4.96/utils/get_edc_requirements.py`

 * *Files identical despite different names*

