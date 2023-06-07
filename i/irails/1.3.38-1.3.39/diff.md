# Comparing `tmp/irails-1.3.38.tar.gz` & `tmp/irails-1.3.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.38.tar", last modified: Tue Jun  6 12:28:48 2023, max compression
+gzip compressed data, was "irails-1.3.39.tar", last modified: Wed Jun  7 14:00:27 2023, max compression
```

## Comparing `irails-1.3.38.tar` & `irails-1.3.39.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.108225 irails-1.3.38/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.38/MANIFEST.in
--rw-rw-rw-   0        0        0     4956 2023-06-06 12:28:48.107247 irails-1.3.38/PKG-INFO
--rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.38/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:47.992402 irails-1.3.38/irails/
--rw-rw-rw-   0        0        0      307 2023-06-06 12:28:14.000000 irails-1.3.38/irails/__init__.py
--rw-rw-rw-   0        0        0     5099 2023-06-06 11:40:15.000000 irails-1.3.38/irails/_i18n.py
--rw-rw-rw-   0        0        0     4450 2023-06-01 06:04:06.000000 irails-1.3.38/irails/_loader.py
--rw-rw-rw-   0        0        0     6271 2023-06-06 11:58:47.000000 irails-1.3.38/irails/_utils.py
--rw-rw-rw-   0        0        0    15351 2023-05-30 10:30:31.000000 irails-1.3.38/irails/auth.py
--rw-rw-rw-   0        0        0    13396 2023-06-06 11:05:31.000000 irails-1.3.38/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.004370 irails-1.3.38/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.006363 irails-1.3.38/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9337 2023-05-31 14:37:50.000000 irails-1.3.38/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.38/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10665 2023-05-31 14:37:46.000000 irails-1.3.38/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.38/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.38/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.38/irails/controller_utils.py
--rw-rw-rw-   0        0        0    26975 2023-06-06 12:15:32.000000 irails-1.3.38/irails/core.py
--rw-rw-rw-   0        0        0    21544 2023-06-06 12:23:20.000000 irails-1.3.38/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.38/irails/log.py
--rw-rw-rw-   0        0        0     8910 2023-06-05 12:15:01.000000 irails-1.3.38/irails/midware.py
--rw-rw-rw-   0        0        0     9175 2023-06-01 06:44:57.000000 irails-1.3.38/irails/midware_session.py
--rw-rw-rw-   0        0        0     4336 2023-06-01 06:22:43.000000 irails-1.3.38/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.021323 irails-1.3.38/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.38/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.38/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.38/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.38/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.38/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.38/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.38/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.38/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.38/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     5750 2023-05-29 06:31:52.000000 irails-1.3.38/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.38/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:47.953506 irails-1.3.38/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.034289 irails-1.3.38/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.38/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.38/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.38/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.38/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.38/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.38/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.38/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.38/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.38/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.037284 irails-1.3.38/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.38/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.039276 irails-1.3.38/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.38/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.054375 irails-1.3.38/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.38/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.38/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.38/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.073321 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.38/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.38/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.38/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.38/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.38/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:47.957497 irails-1.3.38/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.078336 irails-1.3.38/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.38/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.38/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.38/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.38/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.085288 irails-1.3.38/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.38/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.38/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.090290 irails-1.3.38/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:47.963481 irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.094264 irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.101254 irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.38/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.38/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:47.964478 irails-1.3.38/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.103254 irails-1.3.38/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.38/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.38/irails/scripts/tpls/project/public/vue_home.html
--rw-rw-rw-   0        0        0     1731 2023-05-29 05:12:03.000000 irails-1.3.38/irails/unit_test.py
--rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.38/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:28:48.001376 irails-1.3.38/irails.egg-info/
--rw-rw-rw-   0        0        0     4956 2023-06-06 12:28:47.000000 irails-1.3.38/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3209 2023-06-06 12:28:47.000000 irails-1.3.38/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 12:28:47.000000 irails-1.3.38/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-06 12:28:47.000000 irails-1.3.38/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-06-06 12:28:47.000000 irails-1.3.38/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 12:28:47.000000 irails-1.3.38/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 12:28:48.108225 irails-1.3.38/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.244583 irails-1.3.39/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.39/MANIFEST.in
+-rw-rw-rw-   0        0        0     4979 2023-06-07 14:00:27.242588 irails-1.3.39/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.39/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.094717 irails-1.3.39/irails/
+-rw-rw-rw-   0        0        0      307 2023-06-07 13:59:55.000000 irails-1.3.39/irails/__init__.py
+-rw-rw-rw-   0        0        0     7048 2023-06-07 13:53:06.000000 irails-1.3.39/irails/_i18n.py
+-rw-rw-rw-   0        0        0     4450 2023-06-01 06:04:06.000000 irails-1.3.39/irails/_loader.py
+-rw-rw-rw-   0        0        0     6271 2023-06-06 11:58:47.000000 irails-1.3.39/irails/_utils.py
+-rw-rw-rw-   0        0        0    15361 2023-06-07 11:59:43.000000 irails-1.3.39/irails/auth.py
+-rw-rw-rw-   0        0        0    13554 2023-06-07 13:24:34.000000 irails-1.3.39/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.102690 irails-1.3.39/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.104683 irails-1.3.39/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9337 2023-05-31 14:37:50.000000 irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10665 2023-05-31 14:37:46.000000 irails-1.3.39/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.39/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.39/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.39/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    26975 2023-06-06 12:15:32.000000 irails-1.3.39/irails/core.py
+-rw-rw-rw-   0        0        0    21544 2023-06-06 12:23:20.000000 irails-1.3.39/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.39/irails/log.py
+-rw-rw-rw-   0        0        0     8910 2023-06-05 12:15:01.000000 irails-1.3.39/irails/midware.py
+-rw-rw-rw-   0        0        0     9175 2023-06-01 06:44:57.000000 irails-1.3.39/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4336 2023-06-01 06:22:43.000000 irails-1.3.39/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.116530 irails-1.3.39/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.39/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.39/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.39/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.39/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.39/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.39/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.39/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.39/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.39/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     5750 2023-05-29 06:31:52.000000 irails-1.3.39/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.39/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.066143 irails-1.3.39/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.128502 irails-1.3.39/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.39/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.39/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.39/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.39/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.39/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.39/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.39/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.39/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.39/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.130492 irails-1.3.39/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.39/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.131491 irails-1.3.39/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.39/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.186344 irails-1.3.39/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.39/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.39/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.39/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.202301 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.39/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.39/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.39/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.39/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.39/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.069121 irails-1.3.39/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.208286 irails-1.3.39/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.39/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.39/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.39/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.39/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.214269 irails-1.3.39/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.39/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.39/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.218260 irails-1.3.39/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.071117 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.226709 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.235109 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.072115 irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.237998 irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.39/irails/scripts/tpls/project/public/vue_home.html
+-rw-rw-rw-   0        0        0     1731 2023-05-29 05:12:03.000000 irails-1.3.39/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.39/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:00:27.100693 irails-1.3.39/irails.egg-info/
+-rw-rw-rw-   0        0        0     4979 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3209 2023-06-07 14:00:27.000000 irails-1.3.39/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 14:00:26.000000 irails-1.3.39/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:00:27.244583 irails-1.3.39/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.39/setup.py
```

### Comparing `irails-1.3.38/PKG-INFO` & `irails-1.3.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.38
+Version: 1.3.39
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -83,7 +84,9 @@
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
 * `irails migrate`       --run database migrations
+
+
```

### Comparing `irails-1.3.38/README.md` & `irails-1.3.39/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/_i18n.py` & `irails-1.3.39/irails/_i18n.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,28 @@
  
 import gettext
 import importlib  
 
 import os,sys
 import gettext
+
+from typing import Callable
  
 
 _default_localedir = os.path.join(sys.base_prefix, 'share', 'locale')
  
 
 def load_module(module_name:str,module_path:str):
-    if module_name in sys.modules:
-        return sys.modules[module_name]
+    # if module_name in sys.modules:
+    #     return sys.modules[module_name]
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
-        sys.modules[module_name] = module
+        # sys.modules[module_name] = module
         return module
     return None
 def check_compile_po(localedir,lang): 
     po_file = os.path.join(localedir, f'{lang}.po') 
     mo_file = os.path.join(localedir, f'{lang}.mo')
     def do_mfgmft():
          
@@ -34,19 +36,60 @@
     if os.path.exists(po_file): 
         if os.path.exists(mo_file):
             mod_time =  (os.stat(mo_file).st_mtime)
         else:
             mod_time = 0
         pod_time =  (os.stat(po_file).st_mtime) 
         if pod_time>mod_time: 
+            try:
+                if os.path.exists(mo_file):
+                    os.remove(mo_file)
+            except Exception as e:
+                pass
+            key = (gettext.GNUTranslations,mo_file)
+            if key in gettext._translations:
+                del gettext._translations[key]
             do_mfgmft()
  
 __all_trans = {}          
 default_langs = ['en','zh'] 
 
+from .config import config
+is_debug = config.get("debug")
+if is_debug: #watch locale dir file change
+    from watchdog.observers import Observer
+    from watchdog.events import FileSystemEventHandler
+    import time
+    class PoFileHandler(FileSystemEventHandler):
+        def __init__(self,hash,handler:Callable ) -> None:
+            self.hash = hash
+            self.handler = handler
+            self.observer:Observer=None
+            super().__init__()
+        def on_modified(self, event):
+            if not event.is_directory and callable(self.handler):
+                 
+                if self.is_recently_modified(event.src_path):
+                    print(f"{event.src_path} has been modified") 
+                    self.handler(self.hash,self.observer)
+
+        def is_recently_modified(self, file_name:str, seconds=1):  
+            if not file_name.endswith(".po"):
+                return False
+            modified_time = os.path.getmtime(file_name)
+            current_time = time.time()
+            return current_time - modified_time < seconds
+
+    def handler(hash,observer:Observer):
+        if hash in __all_trans:
+            del __all_trans[hash]
+         
+        observer.stop()
+        observer.unschedule_all()
+
 def set_module_i18n(obj, module_name ):
      
     module = sys.modules[module_name]
     module_package = module.__package__ 
       
     if module_package:
         if module_package in sys.modules:
@@ -62,14 +105,15 @@
             setattr(obj,"__app_package__",".".join(app_dirs))
             app_dir = os.path.dirname(service_package_path)
             # auto set the i18n locales to the `app_name/locales`
             t = load_app_translations(app_dir)
             # setattr(obj,"_",t) #modify object
             setattr(module,'_',t.gettext)
 
+
 def load_app_translations(module_dir,lan=None) -> gettext.GNUTranslations: 
     global __all_trans
     
     if  not lan:
         from .config import config
         cfg = config.get('i18n')
         if not cfg:
@@ -79,36 +123,49 @@
         if not isinstance(lan,list):
             lan=[lan]
     
 
     key = f"{module_dir}@{lan}"
     if key in __all_trans:
         return __all_trans[key]
-    # 加载翻译文件
+     
     locales_dir = os.path.join(module_dir, "locales")
+
+
+        # observer.join()
     ret = None
     try:
         
         ret = gettext.translation("messages", locales_dir, languages=lan) 
-        ret.install()
+        # ret.install()
+        
+        if is_debug:
+            event_handler = PoFileHandler(key,handler=handler )
+            observer = Observer()
+            observer.schedule(event_handler=event_handler,path=locales_dir) 
+            observer.start()
+            event_handler.observer = observer
     except Exception as e:
          
         ret = gettext
     
     #cache item
     __all_trans[key] = ret
+
+
     return ret
  
  
 def __init_load_i18n():
 
     _dir = os.path.dirname(__file__)
     # Locate a .mo file using the gettext strategy
     def __new_find(domain, localedir=None, languages=None, all=False):
         # Get some reasonable defaults for arguments that were not supplied
+        # all = False
         if localedir is None:
             localedir = _default_localedir
         if languages is None:
             languages = []
             for envar in ('LANGUAGE', 'LC_ALL', 'LC_MESSAGES', 'LANG'):
                 val = os.environ.get(envar)
                 if val:
```

### Comparing `irails-1.3.38/irails/_loader.py` & `irails-1.3.39/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/_utils.py` & `irails-1.3.39/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/auth.py` & `irails-1.3.39/irails/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,14 +352,15 @@
             "domain": user.domain
         }
 
         request: Request = kwargs['request']
 
         access_token = jwt.encode(
             auth_user_obj, self.secret_key, self.algorithm)
+        
         auth_user_obj.update({"token": access_token})
         request.session[_session_name] = auth_user_obj
         return access_token
```

### Comparing `irails-1.3.38/irails/base_controller.py` & `irails-1.3.39/irails/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,25 +61,29 @@
         url_path = "/"+"/".join(pairs)  + "/"
     return url_path.lower() + url.strip()
 
 class BaseController:
  
     @property
     def _(self):
+        if hasattr(self,"__cached_i18n__"):
+            return getattr(self,'__cached_i18n__').gettext
+        
         m = getattr(self,'__appdir__') 
         languages = None
         if 'lang' in self._session:
             languages = self._session['lang']
         else:
             language_header = self._request.headers.get('accept-language')
             if language_header:
                 languages = language_header.split(',')
                 if languages:
                     languages = [languages[0]]
         t = load_app_translations(module_dir=m,lan=languages)
+        setattr(self,'__cached_i18n__',t)
         return t.gettext
     @property
     def log(self)->Logger:
         return _log
     @property 
     def cookies(self)->Dict[str,str]: 
         """
```

### Comparing `irails-1.3.38/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.39/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.39/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/cbv.py` & `irails-1.3.39/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/config.py` & `irails-1.3.39/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/controller_utils.py` & `irails-1.3.39/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/core.py` & `irails-1.3.39/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/database.py` & `irails-1.3.39/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/log.py` & `irails-1.3.39/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/midware.py` & `irails-1.3.39/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/midware_session.py` & `irails-1.3.39/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/mvc_router.py` & `irails-1.3.39/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_app.py` & `irails-1.3.39/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_controller.py` & `irails-1.3.39/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_i18n.py` & `irails-1.3.39/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_migrate.py` & `irails-1.3.39/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_model.py` & `irails-1.3.39/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_project.py` & `irails-1.3.39/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_run.py` & `irails-1.3.39/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_shell.py` & `irails-1.3.39/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/_test.py` & `irails-1.3.39/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/main.py` & `irails-1.3.39/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.39/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/app/home.tpl` & `irails-1.3.39/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/app/model.jinja` & `irails-1.3.39/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.39/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.39/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.39/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.39/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.39/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.39/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.39/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.39/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.39/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.39/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/scripts/tpls/project/public/vue_home.html` & `irails-1.3.39/irails/scripts/tpls/project/public/vue_home.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/unit_test.py` & `irails-1.3.39/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails/view.py` & `irails-1.3.39/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/irails.egg-info/PKG-INFO` & `irails-1.3.39/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.38
+Version: 1.3.39
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -83,7 +84,9 @@
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
 * `irails migrate`       --run database migrations
+
+
```

### Comparing `irails-1.3.38/irails.egg-info/SOURCES.txt` & `irails-1.3.39/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.38/setup.py` & `irails-1.3.39/setup.py`

 * *Files identical despite different names*

