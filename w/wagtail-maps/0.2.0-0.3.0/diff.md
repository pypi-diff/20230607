# Comparing `tmp/wagtail_maps-0.2.0.tar.gz` & `tmp/wagtail_maps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_maps-0.2.0.tar", last modified: Fri Oct 15 13:44:04 2021, max compression
+gzip compressed data, was "wagtail_maps-0.3.0.tar", last modified: Wed Jun  7 10:20:58 2023, max compression
```

## Comparing `wagtail_maps-0.2.0.tar` & `wagtail_maps-0.3.0.tar`

### file list

```diff
@@ -1,85 +1,98 @@
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      128 2021-10-15 09:00:10.000000 wagtail_maps-0.2.0/.babelrc.json
--rw-r--r--   0 jerome    (1000) jerome    (1000)      324 2021-10-04 14:45:24.000000 wagtail_maps-0.2.0/.editorconfig
--rw-r--r--   0 jerome    (1000) jerome    (1000)      166 2021-10-15 09:22:06.000000 wagtail_maps-0.2.0/.eslintrc.json
--rw-r--r--   0 jerome    (1000) jerome    (1000)      272 2021-10-15 08:16:31.000000 wagtail_maps-0.2.0/.gitignore
--rw-r--r--   0 jerome    (1000) jerome    (1000)       83 2021-10-15 09:02:29.000000 wagtail_maps-0.2.0/.prettierrc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      647 2021-10-15 13:42:44.000000 wagtail_maps-0.2.0/CHANGELOG.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)    35149 2021-10-04 14:43:35.000000 wagtail_maps-0.2.0/LICENSE
--rw-r--r--   0 jerome    (1000) jerome    (1000)      121 2021-10-15 08:28:54.000000 wagtail_maps-0.2.0/MANIFEST.in
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1411 2021-10-04 14:52:49.000000 wagtail_maps-0.2.0/Makefile
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5141 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3276 2021-10-14 13:27:31.000000 wagtail_maps-0.2.0/README.md
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.752446 wagtail_maps-0.2.0/examples/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/examples/frontend/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      564 2021-10-14 13:41:06.000000 wagtail_maps-0.2.0/examples/frontend/README.md
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/examples/frontend/js/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      345 2021-10-14 13:31:11.000000 wagtail_maps-0.2.0/examples/frontend/js/main.js
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6177 2021-10-14 13:28:32.000000 wagtail_maps-0.2.0/examples/frontend/js/map.js
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/examples/frontend/scss/
--rw-r--r--   0 jerome    (1000) jerome    (1000)    14143 2021-10-14 13:32:17.000000 wagtail_maps-0.2.0/examples/frontend/scss/_leaflet.scss
--rw-r--r--   0 jerome    (1000) jerome    (1000)   365685 2021-10-15 09:23:58.000000 wagtail_maps-0.2.0/package-lock.json
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1100 2021-10-15 09:23:58.000000 wagtail_maps-0.2.0/package.json
--rw-r--r--   0 jerome    (1000) jerome    (1000)      839 2021-10-04 14:53:26.000000 wagtail_maps-0.2.0/pyproject.toml
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1267 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/setup.cfg
--rw-r--r--   0 jerome    (1000) jerome    (1000)       38 2021-10-04 15:09:00.000000 wagtail_maps-0.2.0/setup.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/tests/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-10-04 20:40:03.000000 wagtail_maps-0.2.0/tests/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      165 2021-10-06 08:09:22.000000 wagtail_maps-0.2.0/tests/conftest.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      662 2021-10-12 16:01:01.000000 wagtail_maps-0.2.0/tests/factories.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2174 2021-10-07 13:44:38.000000 wagtail_maps-0.2.0/tests/settings.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4148 2021-10-12 16:25:35.000000 wagtail_maps-0.2.0/tests/test_admin.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3557 2021-10-12 16:03:44.000000 wagtail_maps-0.2.0/tests/test_api.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2138 2021-10-12 16:13:44.000000 wagtail_maps-0.2.0/tests/test_blocks.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      626 2021-10-06 08:14:52.000000 wagtail_maps-0.2.0/tests/urls.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      473 2021-10-14 13:13:06.000000 wagtail_maps-0.2.0/tox.ini
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/wagtail_maps/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-10-04 15:11:43.000000 wagtail_maps-0.2.0/wagtail_maps/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2124 2021-10-15 08:34:38.000000 wagtail_maps-0.2.0/wagtail_maps/admin.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/api/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-10-04 20:43:55.000000 wagtail_maps-0.2.0/wagtail_maps/api/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1068 2021-10-06 06:42:52.000000 wagtail_maps-0.2.0/wagtail_maps/api/serializers.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      358 2021-10-06 08:07:06.000000 wagtail_maps-0.2.0/wagtail_maps/api/views.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      152 2021-10-04 20:39:45.000000 wagtail_maps-0.2.0/wagtail_maps/apps.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1910 2021-10-12 16:13:37.000000 wagtail_maps-0.2.0/wagtail_maps/blocks.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.752446 wagtail_maps-0.2.0/wagtail_maps/locale/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.752446 wagtail_maps-0.2.0/wagtail_maps/locale/fr/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2756 2021-10-15 13:37:01.000000 wagtail_maps-0.2.0/wagtail_maps/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3710 2021-10-15 13:36:56.000000 wagtail_maps-0.2.0/wagtail_maps/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/migrations/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2708 2021-10-12 07:35:36.000000 wagtail_maps-0.2.0/wagtail_maps/migrations/0001_initial.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-10-07 14:40:35.000000 wagtail_maps-0.2.0/wagtail_maps/migrations/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2812 2021-10-14 14:22:00.000000 wagtail_maps-0.2.0/wagtail_maps/models.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.752446 wagtail_maps-0.2.0/wagtail_maps/static/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.752446 wagtail_maps-0.2.0/wagtail_maps/static/wagtail_maps/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/static/wagtail_maps/css/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      429 2021-10-15 13:32:40.000000 wagtail_maps-0.2.0/wagtail_maps/static/wagtail_maps/css/admin-form.css
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/static/wagtail_maps/js/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1648 2021-10-15 13:42:03.000000 wagtail_maps-0.2.0/wagtail_maps/static/wagtail_maps/js/admin-form.js
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6017 2021-10-15 13:42:03.000000 wagtail_maps-0.2.0/wagtail_maps/static/wagtail_maps/js/admin-form.js.map
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/wagtail_maps/templates/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/wagtail_maps/templates/modeladmin/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.756446 wagtail_maps-0.2.0/wagtail_maps/templates/modeladmin/wagtail_maps/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/templates/modeladmin/wagtail_maps/map/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1193 2021-10-15 13:32:13.000000 wagtail_maps-0.2.0/wagtail_maps/templates/modeladmin/wagtail_maps/map/_geo_modal.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      128 2021-10-14 16:14:45.000000 wagtail_maps-0.2.0/wagtail_maps/templates/modeladmin/wagtail_maps/map/create.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      126 2021-10-14 16:15:21.000000 wagtail_maps-0.2.0/wagtail_maps/templates/modeladmin/wagtail_maps/map/edit.html
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/edit_handlers/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      341 2021-10-14 14:30:40.000000 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/edit_handlers/center_calculate.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      230 2021-10-15 09:38:18.000000 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/edit_handlers/point_from_geo.html
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/icons/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      206 2021-10-15 11:54:10.000000 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/icons/map-pin.svg
--rw-r--r--   0 jerome    (1000) jerome    (1000)      269 2021-10-04 15:55:18.000000 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/icons/map.svg
--rw-r--r--   0 jerome    (1000) jerome    (1000)      269 2021-10-12 16:13:55.000000 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/map_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      448 2021-10-04 20:51:45.000000 wagtail_maps-0.2.0/wagtail_maps/templates/wagtail_maps/popup_content.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      258 2021-10-06 08:06:32.000000 wagtail_maps-0.2.0/wagtail_maps/urls.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      336 2021-10-15 11:54:25.000000 wagtail_maps-0.2.0/wagtail_maps/wagtail_hooks.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-10-15 13:44:04.760446 wagtail_maps-0.2.0/wagtail_maps.egg-info/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5141 2021-10-15 13:44:04.000000 wagtail_maps-0.2.0/wagtail_maps.egg-info/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1772 2021-10-15 13:44:04.000000 wagtail_maps-0.2.0/wagtail_maps.egg-info/SOURCES.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2021-10-15 13:44:04.000000 wagtail_maps-0.2.0/wagtail_maps.egg-info/dependency_links.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)      121 2021-10-15 13:44:04.000000 wagtail_maps-0.2.0/wagtail_maps.egg-info/requires.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       13 2021-10-15 13:44:04.000000 wagtail_maps-0.2.0/wagtail_maps.egg-info/top_level.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)      501 2021-10-15 09:24:04.000000 wagtail_maps-0.2.0/webpack.config.js
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       32 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.babelrc.json
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      328 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.editorconfig
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      432 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.eslintrc.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       94 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.gitattributes
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      285 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.gitignore
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      732 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      716 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       83 2021-10-15 09:02:29.000000 wagtail_maps-0.3.0/.prettierrc
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1366 2023-06-07 10:11:54.000000 wagtail_maps-0.3.0/CHANGELOG.md
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    35149 2021-10-04 14:43:35.000000 wagtail_maps-0.3.0/LICENSE
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      121 2021-10-15 08:28:54.000000 wagtail_maps-0.3.0/MANIFEST.in
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1110 2023-06-07 09:20:50.000000 wagtail_maps-0.3.0/Makefile
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     4547 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/PKG-INFO
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     3533 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/README.md
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.069651 wagtail_maps-0.3.0/client/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.073650 wagtail_maps-0.3.0/client/src/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      400 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/client/src/admin-form.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      412 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/client/src/admin-form_controllers.js
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.073650 wagtail_maps-0.3.0/client/src/controllers/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1067 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/client/src/controllers/geo-coordinates.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1441 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/client/src/controllers/map-center-coordinates.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2680 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/client/src/controllers/map.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      215 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/client/src/map-block.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1674 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/noxfile.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)   179306 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/package-lock.json
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      683 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/package.json
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      790 2023-05-31 13:04:10.000000 wagtail_maps-0.3.0/pyproject.toml
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       42 2023-05-31 13:04:10.000000 wagtail_maps-0.3.0/requirements-dev.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       44 2023-05-31 13:04:10.000000 wagtail_maps-0.3.0/requirements-test.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      632 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/rollup.config.mjs
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1094 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/setup.cfg
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.073650 wagtail_maps-0.3.0/tests/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2023-05-31 13:19:30.000000 wagtail_maps-0.3.0/tests/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      160 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/tests/conftest.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      662 2023-05-31 13:19:30.000000 wagtail_maps-0.3.0/tests/factories.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2169 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/tests/settings.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     3042 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/tests/test_admin.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     3555 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/tests/test_api.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2813 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/tests/test_blocks.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      621 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/tests/urls.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1588 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/admin.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps/api/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/api/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1068 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/api/serializers.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      358 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/api/views.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      152 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/apps.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     3385 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/blocks.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.069651 wagtail_maps-0.3.0/wagtail_maps/locale/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.069651 wagtail_maps-0.3.0/wagtail_maps/locale/fr/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2595 2023-06-07 09:45:23.000000 wagtail_maps-0.3.0/wagtail_maps/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     3405 2023-06-07 09:45:23.000000 wagtail_maps-0.3.0/wagtail_maps/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps/migrations/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2698 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/migrations/0001_initial.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      420 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/migrations/0002_remove_map_max_zoom_remove_map_min_zoom.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/migrations/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2059 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/models.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      576 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/panels.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.069651 wagtail_maps-0.3.0/wagtail_maps/static/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.069651 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/css/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      443 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/css/admin-form.css
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    46129 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/admin-form.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)   143718 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/admin-form.js.map
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    10553 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/admin-form_controllers.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)   100231 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/admin-form_controllers.js.map
+-rw-r--r--   0 jerome    (1000) jerome    (1000)   189737 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/map-block.js
+-rw-r--r--   0 jerome    (1000) jerome    (1000)   814967 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/js/map-block.js.map
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/images/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1259 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/images/layers-2x.png
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      696 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/images/layers.png
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2464 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/images/marker-icon-2x.png
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1466 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/images/marker-icon.png
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      618 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/images/marker-shadow.png
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    14806 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/static/wagtail_maps/vendor/leaflet.css
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.069651 wagtail_maps-0.3.0/wagtail_maps/templates/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/icons/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      272 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/icons/map-pin.svg
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      331 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/icons/map.svg
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      288 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/map_block.html
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.081650 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/panels/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      547 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/panels/map_center_coordinates.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1182 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/panels/point_coordinates.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      279 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/templates/wagtail_maps/popup_content.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      258 2023-05-31 13:19:25.000000 wagtail_maps-0.3.0/wagtail_maps/urls.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      331 2023-06-07 09:20:58.000000 wagtail_maps-0.3.0/wagtail_maps/wagtail_hooks.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-06-07 10:20:58.077650 wagtail_maps-0.3.0/wagtail_maps.egg-info/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     4547 2023-06-07 10:20:58.000000 wagtail_maps-0.3.0/wagtail_maps.egg-info/PKG-INFO
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2440 2023-06-07 10:20:58.000000 wagtail_maps-0.3.0/wagtail_maps.egg-info/SOURCES.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2023-06-07 10:20:58.000000 wagtail_maps-0.3.0/wagtail_maps.egg-info/dependency_links.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       13 2023-06-07 10:20:58.000000 wagtail_maps-0.3.0/wagtail_maps.egg-info/requires.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       13 2023-06-07 10:20:58.000000 wagtail_maps-0.3.0/wagtail_maps.egg-info/top_level.txt
```

### Comparing `wagtail_maps-0.2.0/LICENSE` & `wagtail_maps-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_maps-0.2.0/PKG-INFO` & `wagtail_maps-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,322 +1,285 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7761 6774  : 2.1.Name: wagt
 00000020: 6169 6c5f 6d61 7073 0a56 6572 7369 6f6e  ail_maps.Version
-00000030: 3a20 302e 322e 300a 5375 6d6d 6172 793a  : 0.2.0.Summary:
+00000030: 3a20 302e 332e 300a 5375 6d6d 6172 793a  : 0.3.0.Summary:
 00000040: 2043 7265 6174 6520 616e 6420 6469 7370   Create and disp
 00000050: 6c61 7920 6d61 7073 2077 6974 6820 706f  lay maps with po
 00000060: 696e 7473 2069 6e20 5761 6774 6169 6c0a  ints in Wagtail.
-00000070: 486f 6d65 2d70 6167 653a 2055 4e4b 4e4f  Home-page: UNKNO
-00000080: 574e 0a41 7574 686f 723a 2043 6c69 7373  WN.Author: Cliss
-00000090: 2058 5849 0a41 7574 686f 722d 656d 6169   XXI.Author-emai
-000000a0: 6c3a 2063 6f6e 7461 6374 4063 6c69 7373  l: contact@cliss
-000000b0: 3231 2e63 6f6d 0a4c 6963 656e 7365 3a20  21.com.License: 
-000000c0: 4147 504c 7633 2b0a 5072 6f6a 6563 742d  AGPLv3+.Project-
-000000d0: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
-000000e0: 2c20 6874 7470 733a 2f2f 666f 7267 652e  , https://forge.
-000000f0: 636c 6973 7332 312e 6f72 672f 636c 6973  cliss21.org/clis
-00000100: 7332 312f 7761 6774 6169 6c2d 6d61 7073  s21/wagtail-maps
-00000110: 2f69 7373 7565 730a 5072 6f6a 6563 742d  /issues.Project-
-00000120: 5552 4c3a 2053 6f75 7263 6520 436f 6465  URL: Source Code
-00000130: 2c20 6874 7470 733a 2f2f 666f 7267 652e  , https://forge.
-00000140: 636c 6973 7332 312e 6f72 672f 636c 6973  cliss21.org/clis
-00000150: 7332 312f 7761 6774 6169 6c2d 6d61 7073  s21/wagtail-maps
-00000160: 0a44 6573 6372 6970 7469 6f6e 3a20 2320  .Description: # 
-00000170: 7761 6774 6169 6c2d 6d61 7073 0a20 2020  wagtail-maps.   
-00000180: 2020 2020 200a 2020 2020 2020 2020 4372       .        Cr
-00000190: 6561 7465 2061 6e64 2064 6973 706c 6179  eate and display
-000001a0: 206d 6170 7320 7769 7468 2070 6f69 6e74   maps with point
-000001b0: 7320 696e 2057 6167 7461 696c 2e0a 2020  s in Wagtail..  
-000001c0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-000001d0: 2a57 6172 6e69 6e67 212a 2a20 5468 6973  *Warning!** This
-000001e0: 2070 726f 6a65 6374 2069 7320 7374 696c   project is stil
-000001f0: 6c20 6561 726c 7920 6f6e 2069 6e20 6974  l early on in it
-00000200: 7320 6465 7665 6c6f 706d 656e 7420 6c69  s development li
-00000210: 6665 6379 636c 652e 2049 7420 6973 0a20  fecycle. It is. 
-00000220: 2020 2020 2020 2070 6f73 7369 626c 6520         possible 
-00000230: 666f 7220 6272 6561 6b69 6e67 2063 6861  for breaking cha
-00000240: 6e67 6573 2074 6f20 6f63 6375 7220 6265  nges to occur be
-00000250: 7477 6565 6e20 7665 7273 696f 6e73 2075  tween versions u
-00000260: 6e74 696c 2072 6561 6368 696e 6720 6120  ntil reaching a 
-00000270: 7374 6162 6c65 0a20 2020 2020 2020 2031  stable.        1
-00000280: 2e30 2e20 4665 6564 6261 636b 2061 6e64  .0. Feedback and
-00000290: 2070 756c 6c20 7265 7175 6573 7473 2061   pull requests a
-000002a0: 7265 2077 656c 636f 6d65 2e0a 2020 2020  re welcome..    
-000002b0: 2020 2020 0a20 2020 2020 2020 2054 6869      .        Thi
-000002c0: 7320 7061 636b 6167 6520 6578 7465 6e64  s package extend
-000002d0: 2057 6167 7461 696c 2074 6f20 6164 6420   Wagtail to add 
-000002e0: 6120 6e65 7720 4d61 7020 6d6f 6465 6c2c  a new Map model,
-000002f0: 2077 6869 6368 2069 7320 636f 6d70 6f73   which is compos
-00000300: 6564 2062 7920 6f6e 6520 6f72 0a20 2020  ed by one or.   
-00000310: 2020 2020 206d 6f72 6520 706f 696e 7473       more points
-00000320: 2e20 4561 6368 2070 6f69 6e74 206d 6179  . Each point may
-00000330: 2068 6176 6520 6120 7469 746c 652c 2073   have a title, s
-00000340: 6f6d 6520 636f 6e74 656e 7420 616e 6420  ome content and 
-00000350: 6c69 6e6b 2074 6f20 616e 2069 6e74 6572  link to an inter
-00000360: 6e61 6c0a 2020 2020 2020 2020 6f72 2065  nal.        or e
-00000370: 7874 6572 6e61 6c20 5552 4c2e 204f 6e63  xternal URL. Onc
-00000380: 6520 796f 7520 6861 7665 2063 6f6e 6669  e you have confi
-00000390: 6775 7265 6420 796f 7572 206d 6170 2066  gured your map f
-000003a0: 726f 6d20 7468 6520 5761 6774 6169 6c20  rom the Wagtail 
-000003b0: 6164 6d69 6e2c 2079 6f75 0a20 2020 2020  admin, you.     
-000003c0: 2020 2077 696c 6c20 6265 2061 626c 6520     will be able 
-000003d0: 746f 2064 6973 706c 6179 2069 7420 696e  to display it in
-000003e0: 2061 2070 6167 6520 2d20 652e 672e 2061   a page - e.g. a
-000003f0: 7320 6120 5374 7265 616d 4669 656c 6420  s a StreamField 
-00000400: 626c 6f63 6b2e 0a20 2020 2020 2020 200a  block..        .
-00000410: 2020 2020 2020 2020 2323 2052 6571 7569          ## Requi
-00000420: 7265 6d65 6e74 730a 2020 2020 2020 2020  rements.        
-00000430: 0a20 2020 2020 2020 2054 6869 7320 7061  .        This pa
-00000440: 636b 6167 6520 7265 7175 6972 6573 2074  ckage requires t
-00000450: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 2020  he following:.  
-00000460: 2020 2020 2020 2d20 2a2a 5761 6774 6169        - **Wagtai
-00000470: 6c20 3e3d 2032 2e31 342a 2a3a 2075 7073  l >= 2.14**: ups
-00000480: 7472 6561 6d20 7061 7463 6865 7320 6861  tream patches ha
-00000490: 7665 2062 6565 6e20 7375 626d 6974 7465  ve been submitte
-000004a0: 6420 746f 2070 726f 7669 6465 2061 2070  d to provide a p
-000004b0: 726f 7065 720a 2020 2020 2020 2020 2020  roper.          
-000004c0: 696e 7465 6772 6174 696f 6e20 6f66 2074  integration of t
-000004d0: 6869 7320 6578 7465 6e73 696f 6e20 696e  his extension in
-000004e0: 746f 2074 6865 2061 646d 696e 202d 2073  to the admin - s
-000004f0: 6565 205b 2337 3536 325d 2c20 5b23 3735  ee [#7562], [#75
-00000500: 3635 5d20 616e 640a 2020 2020 2020 2020  65] and.        
-00000510: 2020 5b23 3735 3930 5d0a 2020 2020 2020    [#7590].      
-00000520: 2020 2d20 2a2a 446a 616e 676f 2a2a 2028    - **Django** (
-00000530: 332e 312c 2033 2e32 290a 2020 2020 2020  3.1, 3.2).      
-00000540: 2020 2d20 2a2a 5079 7468 6f6e 2033 2a2a    - **Python 3**
-00000550: 2028 332e 372c 2033 2e38 2c20 332e 3929   (3.7, 3.8, 3.9)
-00000560: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000570: 2020 5b23 3735 3632 5d3a 2068 7474 7073    [#7562]: https
-00000580: 3a2f 2f67 6974 6875 622e 636f 6d2f 7761  ://github.com/wa
-00000590: 6774 6169 6c2f 7761 6774 6169 6c2f 7075  gtail/wagtail/pu
-000005a0: 6c6c 2f37 3536 320a 2020 2020 2020 2020  ll/7562.        
-000005b0: 5b23 3735 3635 5d3a 2068 7474 7073 3a2f  [#7565]: https:/
-000005c0: 2f67 6974 6875 622e 636f 6d2f 7761 6774  /github.com/wagt
-000005d0: 6169 6c2f 7761 6774 6169 6c2f 7075 6c6c  ail/wagtail/pull
-000005e0: 2f37 3536 350a 2020 2020 2020 2020 5b23  /7565.        [#
-000005f0: 3735 3930 5d3a 2068 7474 7073 3a2f 2f67  7590]: https://g
-00000600: 6974 6875 622e 636f 6d2f 7761 6774 6169  ithub.com/wagtai
-00000610: 6c2f 7761 6774 6169 6c2f 7075 6c6c 2f37  l/wagtail/pull/7
-00000620: 3539 300a 2020 2020 2020 2020 0a20 2020  590.        .   
-00000630: 2020 2020 2023 2320 496e 7374 616c 6c61       ## Installa
-00000640: 7469 6f6e 0a20 2020 2020 2020 200a 2020  tion.        .  
-00000650: 2020 2020 2020 312e 2049 6e73 7461 6c6c        1. Install
-00000660: 2075 7369 6e67 2060 6070 6970 6060 3a0a   using ``pip``:.
-00000670: 2020 2020 2020 2020 2020 2060 6060 7368             ```sh
-00000680: 656c 6c0a 2020 2020 2020 2020 2020 2070  ell.           p
-00000690: 6970 2069 6e73 7461 6c6c 2077 6167 7461  ip install wagta
-000006a0: 696c 2d6d 6170 730a 2020 2020 2020 2020  il-maps.        
-000006b0: 2020 2060 6060 0a20 2020 2020 2020 2032     ```.        2
-000006c0: 2e20 4164 6420 6060 7761 6774 6169 6c5f  . Add ``wagtail_
-000006d0: 6d61 7073 6060 2074 6f20 796f 7572 2060  maps`` to your `
-000006e0: 6049 4e53 5441 4c4c 4544 5f41 5050 5360  `INSTALLED_APPS`
-000006f0: 6020 7365 7474 696e 673a 0a20 2020 2020  ` setting:.     
-00000700: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00000710: 2020 2020 2020 2020 2020 2049 4e53 5441             INSTA
-00000720: 4c4c 4544 5f41 5050 5320 3d20 5b0a 2020  LLED_APPS = [.  
-00000730: 2020 2020 2020 2020 2020 2020 2023 202e               # .
-00000740: 2e2e 0a20 2020 2020 2020 2020 2020 2020  ...             
-00000750: 2020 2777 6167 7461 696c 5f6d 6170 7327    'wagtail_maps'
-00000760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000770: 2023 202e 2e2e 0a20 2020 2020 2020 2020   # ....         
-00000780: 2020 5d0a 2020 2020 2020 2020 2020 2060    ].           `
-00000790: 6060 0a20 2020 2020 2020 2033 2e20 496e  ``.        3. In
-000007a0: 636c 7564 6520 7468 6520 5552 4c20 6f66  clude the URL of
-000007b0: 202a 7761 6774 6169 6c2d 6d61 7073 2a20   *wagtail-maps* 
-000007c0: 746f 2079 6f75 7220 6060 7572 6c73 2e70  to your ``urls.p
-000007d0: 7960 6020 6669 6c65 3a0a 2020 2020 2020  y`` file:.      
-000007e0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-000007f0: 2020 2020 2020 2020 2020 6672 6f6d 2077            from w
-00000800: 6167 7461 696c 5f6d 6170 7320 696d 706f  agtail_maps impo
-00000810: 7274 2075 726c 7320 6173 2077 6167 7461  rt urls as wagta
-00000820: 696c 6d61 7073 5f75 726c 730a 2020 2020  ilmaps_urls.    
-00000830: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00000840: 7572 6c70 6174 7465 726e 7320 3d20 5b0a  urlpatterns = [.
-00000850: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00000860: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00000870: 2020 2020 7061 7468 2827 6d61 7073 2f27      path('maps/'
-00000880: 2c20 696e 636c 7564 6528 7761 6774 6169  , include(wagtai
-00000890: 6c6d 6170 735f 7572 6c73 2929 2c0a 2020  lmaps_urls)),.  
-000008a0: 2020 2020 2020 2020 2020 2020 2023 202e               # .
-000008b0: 2e2e 0a20 2020 2020 2020 2020 2020 5d0a  ...           ].
-000008c0: 2020 2020 2020 2020 2020 2060 6060 0a20             ```. 
-000008d0: 2020 2020 2020 2034 2e20 5275 6e20 6060         4. Run ``
-000008e0: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
-000008f0: 206d 6967 7261 7465 6060 2074 6f20 6372   migrate`` to cr
-00000900: 6561 7465 2074 6865 206d 6f64 656c 730a  eate the models.
-00000910: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000920: 2023 2320 5573 6167 650a 2020 2020 2020   ## Usage.      
-00000930: 2020 0a20 2020 2020 2020 2041 2053 7472    .        A Str
-00000940: 6561 6d46 6965 6c64 2062 6c6f 636b 2060  eamField block `
-00000950: 7761 6774 6169 6c5f 6d61 7073 2e62 6c6f  wagtail_maps.blo
-00000960: 636b 732e 4d61 7042 6c6f 636b 6020 6361  cks.MapBlock` ca
-00000970: 6e20 6265 2075 7365 6420 746f 2064 6973  n be used to dis
-00000980: 706c 6179 2061 0a20 2020 2020 2020 206d  play a.        m
-00000990: 6170 202d 2063 686f 6f73 656e 2066 726f  ap - choosen fro
-000009a0: 6d20 7468 6520 6375 7272 656e 7420 6f6e  m the current on
-000009b0: 6573 202d 2069 6e20 796f 7572 2070 6167  es - in your pag
-000009c0: 652e 2054 6865 204a 6176 6153 6372 6970  e. The JavaScrip
-000009d0: 7420 636f 6465 2061 6e64 2074 6865 0a20  t code and the. 
-000009e0: 2020 2020 2020 204c 6561 666c 6574 2070         Leaflet p
-000009f0: 6163 6b61 6765 2069 7320 6375 7272 656e  ackage is curren
-00000a00: 746c 7920 6e6f 7420 7368 6970 7065 642c  tly not shipped,
-00000a10: 2062 7574 2079 6f75 2063 616e 2066 696e   but you can fin
-00000a20: 6420 616e 2065 7861 6d70 6c65 2069 6e0a  d an example in.
-00000a30: 2020 2020 2020 2020 5b65 7861 6d70 6c65          [example
-00000a40: 732f 6672 6f6e 7465 6e64 2f5d 2865 7861  s/frontend/](exa
-00000a50: 6d70 6c65 732f 6672 6f6e 7465 6e64 2f29  mples/frontend/)
-00000a60: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00000a70: 2020 2023 2320 4465 7665 6c6f 706d 656e     ## Developmen
-00000a80: 740a 2020 2020 2020 2020 2323 2320 5175  t.        ### Qu
-00000a90: 6963 6b20 7374 6172 740a 2020 2020 2020  ick start.      
-00000aa0: 2020 0a20 2020 2020 2020 2054 6f20 7365    .        To se
-00000ab0: 7420 7570 2061 2064 6576 656c 6f70 6d65  t up a developme
-00000ac0: 6e74 2065 6e76 6972 6f6e 6d65 6e74 2c20  nt environment, 
-00000ad0: 656e 7375 7265 2074 6861 7420 5079 7468  ensure that Pyth
-00000ae0: 6f6e 2033 2069 7320 696e 7374 616c 6c65  on 3 is installe
-00000af0: 6420 6f6e 2079 6f75 720a 2020 2020 2020  d on your.      
-00000b00: 2020 7379 7374 656d 2e20 5468 656e 3a0a    system. Then:.
-00000b10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000b20: 2031 2e20 436c 6f6e 6520 7468 6973 2072   1. Clone this r
-00000b30: 6570 6f73 6974 6f72 790a 2020 2020 2020  epository.      
-00000b40: 2020 322e 2043 7265 6174 6520 6120 7669    2. Create a vi
-00000b50: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
-00000b60: 7420 616e 6420 6163 7469 7661 7465 2069  t and activate i
-00000b70: 743a 0a20 2020 2020 2020 2020 2020 6060  t:.           ``
-00000b80: 6073 6865 6c6c 0a20 2020 2020 2020 2020  `shell.         
-00000b90: 2020 7079 7468 6f6e 3320 2d6d 2076 656e    python3 -m ven
-00000ba0: 7620 7665 6e76 0a20 2020 2020 2020 2020  v venv.         
-00000bb0: 2020 736f 7572 6365 2076 656e 762f 6269    source venv/bi
-00000bc0: 6e2f 6163 7469 7661 7465 0a20 2020 2020  n/activate.     
-00000bd0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000be0: 2020 332e 2049 6e73 7461 6c6c 2074 6869    3. Install thi
-00000bf0: 7320 7061 636b 6167 6520 696e 2064 6576  s package in dev
-00000c00: 656c 6f70 206d 6f64 6520 7769 7468 2065  elop mode with e
-00000c10: 7874 7261 2072 6571 7569 7265 6d65 6e74  xtra requirement
-00000c20: 733a 0a20 2020 2020 2020 2020 2020 6060  s:.           ``
-00000c30: 6073 6865 6c6c 0a20 2020 2020 2020 2020  `shell.         
-00000c40: 2020 7069 7020 696e 7374 616c 6c20 2d65    pip install -e
-00000c50: 202e 5b74 6573 745d 0a20 2020 2020 2020   .[test].       
-00000c60: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000c70: 0a20 2020 2020 2020 2023 2323 2043 6f6e  .        ### Con
-00000c80: 7472 6962 7574 696e 670a 2020 2020 2020  tributing.      
-00000c90: 2020 0a20 2020 2020 2020 2054 6865 2050    .        The P
-00000ca0: 7974 686f 6e20 636f 6465 2069 7320 666f  ython code is fo
-00000cb0: 726d 6174 7465 6420 616e 6420 6c69 6e74  rmatted and lint
-00000cc0: 6564 2074 6861 6e6b 7320 746f 205b 666c  ed thanks to [fl
-00000cd0: 616b 6538 5d2c 205b 6973 6f72 745d 2061  ake8], [isort] a
-00000ce0: 6e64 205b 626c 6163 6b5d 2e0a 2020 2020  nd [black]..    
-00000cf0: 2020 2020 546f 2065 6173 6520 7468 6520      To ease the 
-00000d00: 7573 6520 6f66 2074 6869 7320 746f 6f6c  use of this tool
-00000d10: 732c 2074 6865 2066 6f6c 6c6f 7769 6e67  s, the following
-00000d20: 2063 6f6d 6d61 6e64 7320 6172 6520 6176   commands are av
-00000d30: 6169 6c61 626c 653a 0a20 2020 2020 2020  ailable:.       
-00000d40: 202d 2060 6d61 6b65 206c 696e 7460 3a20   - `make lint`: 
-00000d50: 6368 6563 6b20 7468 6520 5079 7468 6f6e  check the Python
-00000d60: 2063 6f64 6520 7379 6e74 6178 2061 6e64   code syntax and
-00000d70: 2069 6d70 6f72 7473 206f 7264 6572 0a20   imports order. 
-00000d80: 2020 2020 2020 202d 2060 6d61 6b65 2066         - `make f
-00000d90: 6f72 6d61 7460 3a20 6669 7820 7468 6520  ormat`: fix the 
-00000da0: 5079 7468 6f6e 2063 6f64 6520 7379 6e74  Python code synt
-00000db0: 6178 2061 6e64 2069 6d70 6f72 7473 206f  ax and imports o
-00000dc0: 7264 6572 0a20 2020 2020 2020 200a 2020  rder.        .  
-00000dd0: 2020 2020 2020 5468 6520 7465 7374 7320        The tests 
-00000de0: 6172 6520 7772 6974 7465 6e20 7769 7468  are written with
-00000df0: 205b 7079 7465 7374 5d20 616e 6420 636f   [pytest] and co
-00000e00: 6465 2063 6f76 6572 6167 6520 6973 206d  de coverage is m
-00000e10: 6561 7375 7265 6420 7769 7468 205b 636f  easured with [co
-00000e20: 7665 7261 6765 5d2e 0a20 2020 2020 2020  verage]..       
-00000e30: 2059 6f75 2063 616e 2075 7365 2074 6865   You can use the
-00000e40: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000e50: 6e64 7320 666f 7220 7468 6174 3a0a 2020  nds for that:.  
-00000e60: 2020 2020 2020 2d20 6060 6d61 6b65 2074        - ``make t
-00000e70: 6573 7460 603a 2072 756e 2074 6865 2074  est``: run the t
-00000e80: 6573 7473 2061 6e64 206f 7574 7075 7420  ests and output 
-00000e90: 6120 7175 6963 6b20 7265 706f 7274 206f  a quick report o
-00000ea0: 6620 636f 6465 2063 6f76 6572 6167 650a  f code coverage.
-00000eb0: 2020 2020 2020 2020 2d20 6060 6d61 6b65          - ``make
-00000ec0: 2063 6f76 6572 6167 6560 603a 2072 756e   coverage``: run
-00000ed0: 2074 6865 2074 6573 7473 2061 6e64 2070   the tests and p
-00000ee0: 726f 6475 6365 2061 6e20 4854 4d4c 2072  roduce an HTML r
-00000ef0: 6570 6f72 7420 6f66 2063 6f64 6520 636f  eport of code co
-00000f00: 7665 7261 6765 0a20 2020 2020 2020 200a  verage.        .
-00000f10: 2020 2020 2020 2020 5768 656e 2073 7562          When sub
-00000f20: 6d69 7474 696e 6720 6120 7075 6c6c 2d72  mitting a pull-r
-00000f30: 6571 7565 7374 2c20 706c 6561 7365 2065  equest, please e
-00000f40: 6e73 7572 6520 7468 6174 2074 6865 2063  nsure that the c
-00000f50: 6f64 6520 6973 2077 656c 6c20 666f 726d  ode is well form
-00000f60: 6174 7465 640a 2020 2020 2020 2020 616e  atted.        an
-00000f70: 6420 636f 7665 7265 642c 2061 6e64 2074  d covered, and t
-00000f80: 6861 7420 616c 6c20 7468 6520 6f74 6865  hat all the othe
-00000f90: 7220 7465 7374 7320 7061 7373 2e0a 2020  r tests pass..  
-00000fa0: 2020 2020 2020 0a20 2020 2020 2020 205b        .        [
-00000fb0: 666c 616b 6538 5d3a 2068 7474 7073 3a2f  flake8]: https:/
-00000fc0: 2f66 6c61 6b65 382e 7079 6371 612e 6f72  /flake8.pycqa.or
-00000fd0: 672f 0a20 2020 2020 2020 205b 6973 6f72  g/.        [isor
-00000fe0: 745d 3a20 6874 7470 733a 2f2f 7079 6371  t]: https://pycq
-00000ff0: 612e 6769 7468 7562 2e69 6f2f 6973 6f72  a.github.io/isor
-00001000: 742f 0a20 2020 2020 2020 205b 626c 6163  t/.        [blac
-00001010: 6b5d 3a20 6874 7470 733a 2f2f 626c 6163  k]: https://blac
-00001020: 6b2e 7265 6164 7468 6564 6f63 732e 696f  k.readthedocs.io
-00001030: 2f0a 2020 2020 2020 2020 5b70 7974 6573  /.        [pytes
-00001040: 745d 3a20 6874 7470 733a 2f2f 646f 6373  t]: https://docs
-00001050: 2e70 7974 6573 742e 6f72 672f 0a20 2020  .pytest.org/.   
-00001060: 2020 2020 205b 636f 7665 7261 6765 5d3a       [coverage]:
-00001070: 2068 7474 7073 3a2f 2f63 6f76 6572 6167   https://coverag
-00001080: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00001090: 2f0a 2020 2020 2020 2020 0a20 2020 2020  /.        .     
-000010a0: 2020 2023 2320 4c69 6365 6e73 650a 2020     ## License.  
-000010b0: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
-000010c0: 6869 7320 6578 7465 6e73 696f 6e20 6973  his extension is
-000010d0: 206d 6169 6e6c 7920 6465 7665 6c6f 7065   mainly develope
-000010e0: 6420 6279 205b 436c 6973 7320 5858 495d  d by [Cliss XXI]
-000010f0: 2868 7474 7073 3a2f 2f77 7777 2e63 6c69  (https://www.cli
-00001100: 7373 3231 2e63 6f6d 2920 616e 640a 2020  ss21.com) and.  
-00001110: 2020 2020 2020 6c69 6365 6e73 6564 2075        licensed u
-00001120: 6e64 6572 2074 6865 205b 4147 504c 7633  nder the [AGPLv3
-00001130: 2b5d 284c 4943 454e 5345 292e 2041 6e79  +](LICENSE). Any
-00001140: 2063 6f6e 7472 6962 7574 696f 6e20 6973   contribution is
-00001150: 2077 656c 636f 6d65 210a 2020 2020 2020   welcome!.      
-00001160: 2020 0a4b 6579 776f 7264 733a 2077 6167    .Keywords: wag
-00001170: 7461 696c 2c6d 6170 2c6c 6561 666c 6574  tail,map,leaflet
-00001180: 0a50 6c61 7466 6f72 6d3a 2055 4e4b 4e4f  .Platform: UNKNO
-00001190: 574e 0a43 6c61 7373 6966 6965 723a 2044  WN.Classifier: D
-000011a0: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-000011b0: 7320 3a3a 2033 202d 2041 6c70 6861 0a43  s :: 3 - Alpha.C
-000011c0: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
-000011d0: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
-000011e0: 7669 726f 6e6d 656e 740a 436c 6173 7369  vironment.Classi
-000011f0: 6669 6572 3a20 4672 616d 6577 6f72 6b20  fier: Framework 
-00001200: 3a3a 2044 6a61 6e67 6f0a 436c 6173 7369  :: Django.Classi
-00001210: 6669 6572 3a20 4672 616d 6577 6f72 6b20  fier: Framework 
-00001220: 3a3a 2057 6167 7461 696c 0a43 6c61 7373  :: Wagtail.Class
-00001230: 6966 6965 723a 2046 7261 6d65 776f 726b  ifier: Framework
-00001240: 203a 3a20 5761 6774 6169 6c20 3a3a 2032   :: Wagtail :: 2
-00001250: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-00001260: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00001270: 3a20 4465 7665 6c6f 7065 7273 0a43 6c61  : Developers.Cla
-00001280: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-00001290: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000012a0: 203a 3a20 474e 5520 4166 6665 726f 2047   :: GNU Affero G
-000012b0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-000012c0: 6365 6e73 6520 7633 0a43 6c61 7373 6966  cense v3.Classif
-000012d0: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-000012e0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000012f0: 7065 6e64 656e 740a 436c 6173 7369 6669  pendent.Classifi
-00001300: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00001310: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00001320: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
-00001330: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00001340: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00001350: 6f6e 203a 3a20 332e 370a 436c 6173 7369  on :: 3.7.Classi
-00001360: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00001370: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00001380: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
-00001390: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000013a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000013b0: 5079 7468 6f6e 203a 3a20 332e 390a 5265  Python :: 3.9.Re
-000013c0: 7175 6972 6573 2d50 7974 686f 6e3a 203c  quires-Python: <
-000013d0: 342c 3e3d 332e 370a 4465 7363 7269 7074  4,>=3.7.Descript
-000013e0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000013f0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00001400: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00001410: 7465 7374 0a                             test.
+00000070: 4175 7468 6f72 3a20 436c 6973 7320 5858  Author: Cliss XX
+00000080: 490a 4175 7468 6f72 2d65 6d61 696c 3a20  I.Author-email: 
+00000090: 636f 6e74 6163 7440 636c 6973 7332 312e  contact@cliss21.
+000000a0: 636f 6d0a 4c69 6365 6e73 653a 2041 4750  com.License: AGP
+000000b0: 4c76 332b 0a50 726f 6a65 6374 2d55 524c  Lv3+.Project-URL
+000000c0: 3a20 4275 6720 5472 6163 6b65 722c 2068  : Bug Tracker, h
+000000d0: 7474 7073 3a2f 2f66 7261 6d61 6769 742e  ttps://framagit.
+000000e0: 6f72 672f 636c 6973 7332 312f 7761 6774  org/cliss21/wagt
+000000f0: 6169 6c2d 6d61 7073 2f2d 2f69 7373 7565  ail-maps/-/issue
+00000100: 730a 5072 6f6a 6563 742d 5552 4c3a 2053  s.Project-URL: S
+00000110: 6f75 7263 6520 436f 6465 2c20 6874 7470  ource Code, http
+00000120: 733a 2f2f 6672 616d 6167 6974 2e6f 7267  s://framagit.org
+00000130: 2f63 6c69 7373 3231 2f77 6167 7461 696c  /cliss21/wagtail
+00000140: 2d6d 6170 730a 4b65 7977 6f72 6473 3a20  -maps.Keywords: 
+00000150: 7761 6774 6169 6c2c 6d61 702c 6c65 6166  wagtail,map,leaf
+00000160: 6c65 740a 436c 6173 7369 6669 6572 3a20  let.Classifier: 
+00000170: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000180: 7573 203a 3a20 3320 2d20 416c 7068 610a  us :: 3 - Alpha.
+00000190: 436c 6173 7369 6669 6572 3a20 456e 7669  Classifier: Envi
+000001a0: 726f 6e6d 656e 7420 3a3a 2057 6562 2045  ronment :: Web E
+000001b0: 6e76 6972 6f6e 6d65 6e74 0a43 6c61 7373  nvironment.Class
+000001c0: 6966 6965 723a 2046 7261 6d65 776f 726b  ifier: Framework
+000001d0: 203a 3a20 446a 616e 676f 0a43 6c61 7373   :: Django.Class
+000001e0: 6966 6965 723a 2046 7261 6d65 776f 726b  ifier: Framework
+000001f0: 203a 3a20 5761 6774 6169 6c0a 436c 6173   :: Wagtail.Clas
+00000200: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
+00000210: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000220: 656c 6f70 6572 730a 436c 6173 7369 6669  elopers.Classifi
+00000230: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+00000240: 5349 2041 7070 726f 7665 6420 3a3a 2047  SI Approved :: G
+00000250: 4e55 2041 6666 6572 6f20 4765 6e65 7261  NU Affero Genera
+00000260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00000270: 2076 330a 436c 6173 7369 6669 6572 3a20   v3.Classifier: 
+00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000290: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000002a0: 6e74 0a43 6c61 7373 6966 6965 723a 2050  nt.Classifier: P
+000002b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002d0: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
+000002e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000300: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000310: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000320: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000330: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000340: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000350: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000360: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+00000370: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000380: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000390: 7468 6f6e 203a 3a20 332e 3131 0a52 6571  thon :: 3.11.Req
+000003a0: 7569 7265 732d 5079 7468 6f6e 3a20 3c34  uires-Python: <4
+000003b0: 2c3e 3d33 2e38 0a44 6573 6372 6970 7469  ,>=3.8.Descripti
+000003c0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+000003d0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
+000003e0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+000003f0: 454e 5345 0a0a 2320 7761 6774 6169 6c2d  ENSE..# wagtail-
+00000400: 6d61 7073 0a0a 4372 6561 7465 2061 6e64  maps..Create and
+00000410: 2064 6973 706c 6179 206d 6170 7320 7769   display maps wi
+00000420: 7468 2070 6f69 6e74 7320 696e 2057 6167  th points in Wag
+00000430: 7461 696c 2e0a 0a2a 2a57 6172 6e69 6e67  tail...**Warning
+00000440: 212a 2a20 5468 6973 2070 726f 6a65 6374  !** This project
+00000450: 2069 7320 7374 696c 6c20 6561 726c 7920   is still early 
+00000460: 6f6e 2069 6e20 6974 7320 6465 7665 6c6f  on in its develo
+00000470: 706d 656e 7420 6c69 6665 6379 636c 652e  pment lifecycle.
+00000480: 2049 7420 6973 0a70 6f73 7369 626c 6520   It is.possible 
+00000490: 666f 7220 6272 6561 6b69 6e67 2063 6861  for breaking cha
+000004a0: 6e67 6573 2074 6f20 6f63 6375 7220 6265  nges to occur be
+000004b0: 7477 6565 6e20 7665 7273 696f 6e73 2075  tween versions u
+000004c0: 6e74 696c 2072 6561 6368 696e 6720 6120  ntil reaching a 
+000004d0: 7374 6162 6c65 0a31 2e30 2e20 4665 6564  stable.1.0. Feed
+000004e0: 6261 636b 2061 6e64 2070 756c 6c20 7265  back and pull re
+000004f0: 7175 6573 7473 2061 7265 2077 656c 636f  quests are welco
+00000500: 6d65 2e0a 0a54 6869 7320 7061 636b 6167  me...This packag
+00000510: 6520 6578 7465 6e64 2057 6167 7461 696c  e extend Wagtail
+00000520: 2074 6f20 6164 6420 6120 6e65 7720 4d61   to add a new Ma
+00000530: 7020 6d6f 6465 6c2c 2077 6869 6368 2069  p model, which i
+00000540: 7320 636f 6d70 6f73 6564 2062 7920 6f6e  s composed by on
+00000550: 6520 6f72 0a6d 6f72 6520 706f 696e 7473  e or.more points
+00000560: 2e20 4561 6368 2070 6f69 6e74 206d 6179  . Each point may
+00000570: 2068 6176 6520 6120 7469 746c 652c 2073   have a title, s
+00000580: 6f6d 6520 636f 6e74 656e 7420 616e 6420  ome content and 
+00000590: 6c69 6e6b 2074 6f20 616e 2069 6e74 6572  link to an inter
+000005a0: 6e61 6c0a 6f72 2065 7874 6572 6e61 6c20  nal.or external 
+000005b0: 5552 4c2e 204f 6e63 6520 796f 7520 6861  URL. Once you ha
+000005c0: 7665 2063 6f6e 6669 6775 7265 6420 796f  ve configured yo
+000005d0: 7572 206d 6170 2066 726f 6d20 7468 6520  ur map from the 
+000005e0: 5761 6774 6169 6c20 6164 6d69 6e2c 2079  Wagtail admin, y
+000005f0: 6f75 0a77 696c 6c20 6265 2061 626c 6520  ou.will be able 
+00000600: 746f 2064 6973 706c 6179 2069 7420 696e  to display it in
+00000610: 2061 2070 6167 6520 2d20 652e 672e 2061   a page - e.g. a
+00000620: 7320 6120 5374 7265 616d 4669 656c 6420  s a StreamField 
+00000630: 626c 6f63 6b2e 0a0a 2323 2052 6571 7569  block...## Requi
+00000640: 7265 6d65 6e74 730a 0a54 6869 7320 7061  rements..This pa
+00000650: 636b 6167 6520 7265 7175 6972 6573 2074  ckage requires t
+00000660: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 2d20  he following:.- 
+00000670: 2a2a 5761 6774 6169 6c2a 2a20 2834 2e31  **Wagtail** (4.1
+00000680: 204c 5453 2c20 352e 3029 0a2d 202a 2a44   LTS, 5.0).- **D
+00000690: 6a61 6e67 6f2a 2a20 2833 2e32 204c 5453  jango** (3.2 LTS
+000006a0: 2c20 342e 3220 4c54 5329 0a2d 202a 2a50  , 4.2 LTS).- **P
+000006b0: 7974 686f 6e20 332a 2a20 2833 2e38 2c20  ython 3** (3.8, 
+000006c0: 332e 392c 2033 2e31 302c 2033 2e31 3129  3.9, 3.10, 3.11)
+000006d0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+000006e0: 6e0a 0a31 2e20 496e 7374 616c 6c20 7573  n..1. Install us
+000006f0: 696e 6720 6060 7069 7060 603a 0a20 2020  ing ``pip``:.   
+00000700: 6060 6073 6865 6c6c 0a20 2020 7069 7020  ```shell.   pip 
+00000710: 696e 7374 616c 6c20 7761 6774 6169 6c2d  install wagtail-
+00000720: 6d61 7073 0a20 2020 6060 600a 322e 2041  maps.   ```.2. A
+00000730: 6464 2060 6077 6167 7461 696c 5f6d 6170  dd ``wagtail_map
+00000740: 7360 6020 746f 2079 6f75 7220 6060 494e  s`` to your ``IN
+00000750: 5354 414c 4c45 445f 4150 5053 6060 2073  STALLED_APPS`` s
+00000760: 6574 7469 6e67 3a0a 2020 2060 6060 7079  etting:.   ```py
+00000770: 7468 6f6e 0a20 2020 494e 5354 414c 4c45  thon.   INSTALLE
+00000780: 445f 4150 5053 203d 205b 0a20 2020 2020  D_APPS = [.     
+00000790: 2020 2320 2e2e 2e0a 2020 2020 2020 2027    # ....       '
+000007a0: 7761 6774 6169 6c5f 6d61 7073 272c 0a20  wagtail_maps',. 
+000007b0: 2020 2020 2020 2320 2e2e 2e0a 2020 205d        # ....   ]
+000007c0: 0a20 2020 6060 600a 332e 2049 6e63 6c75  .   ```.3. Inclu
+000007d0: 6465 2074 6865 2055 524c 206f 6620 2a77  de the URL of *w
+000007e0: 6167 7461 696c 2d6d 6170 732a 2074 6f20  agtail-maps* to 
+000007f0: 796f 7572 2060 6075 726c 732e 7079 6060  your ``urls.py``
+00000800: 2066 696c 653a 0a20 2020 6060 6070 7974   file:.   ```pyt
+00000810: 686f 6e0a 2020 2066 726f 6d20 7761 6774  hon.   from wagt
+00000820: 6169 6c5f 6d61 7073 2069 6d70 6f72 7420  ail_maps import 
+00000830: 7572 6c73 2061 7320 7761 6774 6169 6c6d  urls as wagtailm
+00000840: 6170 735f 7572 6c73 0a0a 2020 2075 726c  aps_urls..   url
+00000850: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
+00000860: 2020 2020 2320 2e2e 2e0a 2020 2020 2020      # ....      
+00000870: 2070 6174 6828 276d 6170 732f 272c 2069   path('maps/', i
+00000880: 6e63 6c75 6465 2877 6167 7461 696c 6d61  nclude(wagtailma
+00000890: 7073 5f75 726c 7329 292c 0a20 2020 2020  ps_urls)),.     
+000008a0: 2020 2320 2e2e 2e0a 2020 205d 0a20 2020    # ....   ].   
+000008b0: 6060 600a 342e 2052 756e 2060 6070 7974  ```.4. Run ``pyt
+000008c0: 686f 6e20 6d61 6e61 6765 2e70 7920 6d69  hon manage.py mi
+000008d0: 6772 6174 6560 6020 746f 2063 7265 6174  grate`` to creat
+000008e0: 6520 7468 6520 6d6f 6465 6c73 0a0a 2323  e the models..##
+000008f0: 2055 7361 6765 0a0a 4120 5374 7265 616d   Usage..A Stream
+00000900: 4669 656c 6420 626c 6f63 6b20 6077 6167  Field block `wag
+00000910: 7461 696c 5f6d 6170 732e 626c 6f63 6b73  tail_maps.blocks
+00000920: 2e4d 6170 426c 6f63 6b60 2063 616e 2062  .MapBlock` can b
+00000930: 6520 7573 6564 2074 6f20 6469 7370 6c61  e used to displa
+00000940: 7920 610a 6769 7665 6e20 604d 6170 6020  y a.given `Map` 
+00000950: 6f62 6a65 6374 2077 6974 6820 6974 7320  object with its 
+00000960: 706f 696e 7473 2069 6e20 796f 7572 2070  points in your p
+00000970: 6167 652e 2054 6f20 7265 6e64 6572 2074  age. To render t
+00000980: 6869 7320 626c 6f63 6b20 696e 2079 6f75  his block in you
+00000990: 720a 6672 6f6e 7465 6e64 2c20 796f 7520  r.frontend, you 
+000009a0: 7769 6c6c 2068 6176 6520 746f 2069 6e63  will have to inc
+000009b0: 6c75 6465 2074 6865 2066 6f6c 6c6f 7769  lude the followi
+000009c0: 6e67 2061 7373 6574 7320 696e 2074 6865  ng assets in the
+000009d0: 2074 656d 706c 6174 6573 2077 6869 6368   templates which
+000009e0: 0a63 616e 2063 6f6e 7461 696e 2069 7420  .can contain it 
+000009f0: 2d20 6f72 2069 6e20 796f 7572 2062 6173  - or in your bas
+00000a00: 6520 7465 6d70 6c61 7465 3a0a 0a2a 2074  e template:..* t
+00000a10: 6865 204a 6176 6153 6372 6970 7420 636f  he JavaScript co
+00000a20: 6465 2074 6861 7420 7265 6e64 6572 7320  de that renders 
+00000a30: 7468 6520 6d61 7020 7769 7468 205b 4c65  the map with [Le
+00000a40: 6166 6c65 745d 2074 6861 6e6b 7320 746f  aflet] thanks to
+00000a50: 2061 0a20 205b 5374 696d 756c 7573 5d20   a.  [Stimulus] 
+00000a60: 636f 6e74 726f 6c6c 6572 3a0a 2020 6060  controller:.  ``
+00000a70: 6064 6a61 6e67 6f0a 2020 3c73 6372 6970  `django.  <scrip
+00000a80: 7420 7372 633d 227b 2520 7374 6174 6963  t src="{% static
+00000a90: 2022 7761 6774 6169 6c5f 6d61 7073 2f6a   "wagtail_maps/j
+00000aa0: 732f 6d61 702d 626c 6f63 6b2e 6a73 2220  s/map-block.js" 
+00000ab0: 257d 223e 3c2f 7363 7269 7074 3e0a 2020  %}"></script>.  
+00000ac0: 6060 600a 2a20 7468 6520 6465 6661 756c  ```.* the defaul
+00000ad0: 7420 4c65 6166 6c65 7420 7374 796c 6573  t Leaflet styles
+00000ae0: 6865 6574 2069 6620 796f 7520 646f 6e27  heet if you don'
+00000af0: 7420 7072 6f76 6964 6520 796f 7572 206f  t provide your o
+00000b00: 776e 3a0a 2020 6060 6064 6a61 6e67 6f0a  wn:.  ```django.
+00000b10: 2020 3c6c 696e 6b20 7265 6c3d 2273 7479    <link rel="sty
+00000b20: 6c65 7368 6565 7422 2068 7265 663d 227b  lesheet" href="{
+00000b30: 2520 7374 6174 6963 2022 7761 6774 6169  % static "wagtai
+00000b40: 6c5f 6d61 7073 2f76 656e 646f 722f 6c65  l_maps/vendor/le
+00000b50: 6166 6c65 742e 6373 7322 2025 7d22 3e0a  aflet.css" %}">.
+00000b60: 2020 6060 600a 0a5b 4c65 6166 6c65 745d    ```..[Leaflet]
+00000b70: 3a20 6874 7470 733a 2f2f 6c65 6166 6c65  : https://leafle
+00000b80: 746a 732e 636f 6d2f 0a5b 5374 696d 756c  tjs.com/.[Stimul
+00000b90: 7573 5d3a 2068 7474 7073 3a2f 2f73 7469  us]: https://sti
+00000ba0: 6d75 6c75 732e 686f 7477 6972 6564 2e64  mulus.hotwired.d
+00000bb0: 6576 2f0a 0a23 2320 4465 7665 6c6f 706d  ev/..## Developm
+00000bc0: 656e 740a 2323 2320 5175 6963 6b20 7374  ent.### Quick st
+00000bd0: 6172 740a 0a54 6f20 7365 7420 7570 2061  art..To set up a
+00000be0: 2064 6576 656c 6f70 6d65 6e74 2065 6e76   development env
+00000bf0: 6972 6f6e 6d65 6e74 2c20 656e 7375 7265  ironment, ensure
+00000c00: 2074 6861 7420 5079 7468 6f6e 2033 2069   that Python 3 i
+00000c10: 7320 696e 7374 616c 6c65 6420 6f6e 2079  s installed on y
+00000c20: 6f75 720a 7379 7374 656d 2e20 5468 656e  our.system. Then
+00000c30: 3a0a 0a31 2e20 436c 6f6e 6520 7468 6973  :..1. Clone this
+00000c40: 2072 6570 6f73 6974 6f72 790a 322e 2043   repository.2. C
+00000c50: 7265 6174 6520 6120 7669 7274 7561 6c20  reate a virtual 
+00000c60: 656e 7669 726f 6e6d 656e 7420 616e 6420  environment and 
+00000c70: 6163 7469 7661 7465 2069 743a 0a20 2020  activate it:.   
+00000c80: 6060 6073 6865 6c6c 0a20 2020 7079 7468  ```shell.   pyth
+00000c90: 6f6e 3320 2d6d 2076 656e 7620 7665 6e76  on3 -m venv venv
+00000ca0: 0a20 2020 736f 7572 6365 2076 656e 762f  .   source venv/
+00000cb0: 6269 6e2f 6163 7469 7661 7465 0a20 2020  bin/activate.   
+00000cc0: 6060 600a 332e 2049 6e73 7461 6c6c 2074  ```.3. Install t
+00000cd0: 6869 7320 7061 636b 6167 6520 616e 6420  his package and 
+00000ce0: 6974 7320 7265 7175 6972 656d 656e 7473  its requirements
+00000cf0: 3a0a 2020 2060 6060 7368 656c 6c0a 2020  :.   ```shell.  
+00000d00: 2028 7665 6e76 2924 2070 6970 2069 6e73   (venv)$ pip ins
+00000d10: 7461 6c6c 202d 7220 7265 7175 6972 656d  tall -r requirem
+00000d20: 656e 7473 2d64 6576 2e74 7874 0a20 2020  ents-dev.txt.   
+00000d30: 6060 600a 0a23 2323 2043 6f6e 7472 6962  ```..### Contrib
+00000d40: 7574 696e 670a 0a54 6865 2074 6573 7473  uting..The tests
+00000d50: 2061 7265 2077 7269 7474 656e 2077 6974   are written wit
+00000d60: 6820 5b70 7974 6573 745d 2061 6e64 2063  h [pytest] and c
+00000d70: 6f64 6520 636f 7665 7261 6765 2069 7320  ode coverage is 
+00000d80: 6d65 6173 7572 6564 2077 6974 6820 5b63  measured with [c
+00000d90: 6f76 6572 6167 655d 2e0a 596f 7520 6361  overage]..You ca
+00000da0: 6e20 7573 6520 7468 6520 666f 6c6c 6f77  n use the follow
+00000db0: 696e 6720 636f 6d6d 616e 6473 2077 6869  ing commands whi
+00000dc0: 6c65 2064 6576 656c 6f70 696e 673a 0a2d  le developing:.-
+00000dd0: 2060 606d 616b 6520 7465 7374 6060 3a20   ``make test``: 
+00000de0: 7275 6e20 7468 6520 7465 7374 7320 616e  run the tests an
+00000df0: 6420 6f75 7470 7574 2061 2071 7569 636b  d output a quick
+00000e00: 2072 6570 6f72 7420 6f66 2063 6f64 6520   report of code 
+00000e10: 636f 7665 7261 6765 0a2d 2060 606d 616b  coverage.- ``mak
+00000e20: 6520 7465 7374 2d77 6970 6060 3a20 6f6e  e test-wip``: on
+00000e30: 6c79 2072 756e 2074 6865 2074 6573 7473  ly run the tests
+00000e40: 206d 6172 6b65 6420 6173 2027 7769 7027   marked as 'wip'
+00000e50: 0a2d 2060 606d 616b 6520 7465 7374 2d61  .- ``make test-a
+00000e60: 6c6c 6060 3a20 7275 6e20 7468 6520 7465  ll``: run the te
+00000e70: 7374 7320 6f6e 2061 6c6c 2073 7570 706f  sts on all suppo
+00000e80: 7274 6564 2076 6572 7369 6f6e 7320 6f66  rted versions of
+00000e90: 2044 6a61 6e67 6f20 616e 640a 2020 5761   Django and.  Wa
+00000ea0: 6774 6169 6c20 7769 7468 205b 6e6f 785d  gtail with [nox]
+00000eb0: 0a0a 5468 6520 5079 7468 6f6e 2063 6f64  ..The Python cod
+00000ec0: 6520 6973 2066 6f72 6d61 7474 6564 2061  e is formatted a
+00000ed0: 6e64 206c 696e 7465 6420 7468 616e 6b73  nd linted thanks
+00000ee0: 2074 6f20 5b66 6c61 6b65 385d 2c20 5b69   to [flake8], [i
+00000ef0: 736f 7274 5d20 616e 6420 5b62 6c61 636b  sort] and [black
+00000f00: 5d2e 0a41 6c6c 206f 6620 7468 6573 6520  ]..All of these 
+00000f10: 746f 6f6c 7320 6172 6520 636f 6e66 6967  tools are config
+00000f20: 7572 6564 2069 6e20 5b70 7265 2d63 6f6d  ured in [pre-com
+00000f30: 6d69 745d 2061 6e64 2079 6f75 2073 686f  mit] and you sho
+00000f40: 756c 6420 636f 6e73 6964 6572 2074 6f0a  uld consider to.
+00000f50: 696e 7374 616c 6c20 6974 7320 6769 7420  install its git 
+00000f60: 686f 6f6b 2073 6372 6970 7473 2062 7920  hook scripts by 
+00000f70: 7275 6e6e 696e 673a 0a60 6060 7368 656c  running:.```shel
+00000f80: 6c0a 2876 656e 7629 2420 7072 652d 636f  l.(venv)$ pre-co
+00000f90: 6d6d 6974 2069 6e73 7461 6c6c 0a60 6060  mmit install.```
+00000fa0: 0a0a 5768 656e 2073 7562 6d69 7474 696e  ..When submittin
+00000fb0: 6720 6120 7075 6c6c 2d72 6571 7565 7374  g a pull-request
+00000fc0: 2c20 706c 6561 7365 2065 6e73 7572 6520  , please ensure 
+00000fd0: 7468 6174 2074 6865 2063 6f64 6520 6973  that the code is
+00000fe0: 2077 656c 6c20 666f 726d 6174 7465 640a   well formatted.
+00000ff0: 616e 6420 636f 7665 7265 642c 2061 6e64  and covered, and
+00001000: 2074 6861 7420 616c 6c20 7468 6520 7465   that all the te
+00001010: 7374 7320 7061 7373 2e0a 0a5b 7079 7465  sts pass...[pyte
+00001020: 7374 5d3a 2068 7474 7073 3a2f 2f64 6f63  st]: https://doc
+00001030: 732e 7079 7465 7374 2e6f 7267 2f0a 5b63  s.pytest.org/.[c
+00001040: 6f76 6572 6167 655d 3a20 6874 7470 733a  overage]: https:
+00001050: 2f2f 636f 7665 7261 6765 2e72 6561 6474  //coverage.readt
+00001060: 6865 646f 6373 2e69 6f2f 0a5b 6e6f 785d  hedocs.io/.[nox]
+00001070: 3a20 6874 7470 733a 2f2f 6e6f 782e 7468  : https://nox.th
+00001080: 6561 2e63 6f64 6573 2f0a 5b66 6c61 6b65  ea.codes/.[flake
+00001090: 385d 3a20 6874 7470 733a 2f2f 666c 616b  8]: https://flak
+000010a0: 6538 2e70 7963 7161 2e6f 7267 2f0a 5b69  e8.pycqa.org/.[i
+000010b0: 736f 7274 5d3a 2068 7474 7073 3a2f 2f70  sort]: https://p
+000010c0: 7963 7161 2e67 6974 6875 622e 696f 2f69  ycqa.github.io/i
+000010d0: 736f 7274 2f0a 5b62 6c61 636b 5d3a 2068  sort/.[black]: h
+000010e0: 7474 7073 3a2f 2f62 6c61 636b 2e72 6561  ttps://black.rea
+000010f0: 6474 6865 646f 6373 2e69 6f2f 0a5b 7072  dthedocs.io/.[pr
+00001100: 652d 636f 6d6d 6974 5d3a 2068 7474 7073  e-commit]: https
+00001110: 3a2f 2f70 7265 2d63 6f6d 6d69 742e 636f  ://pre-commit.co
+00001120: 6d2f 0a0a 2323 204c 6963 656e 7365 0a0a  m/..## License..
+00001130: 5468 6973 2065 7874 656e 7369 6f6e 2069  This extension i
+00001140: 7320 6d61 696e 6c79 2064 6576 656c 6f70  s mainly develop
+00001150: 6564 2062 7920 5b43 6c69 7373 2058 5849  ed by [Cliss XXI
+00001160: 5d28 6874 7470 733a 2f2f 7777 772e 636c  ](https://www.cl
+00001170: 6973 7332 312e 636f 6d29 2061 6e64 0a6c  iss21.com) and.l
+00001180: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00001190: 6520 5b41 4750 4c76 332b 5d28 4c49 4345  e [AGPLv3+](LICE
+000011a0: 4e53 4529 2e20 416e 7920 636f 6e74 7269  NSE). Any contri
+000011b0: 6275 7469 6f6e 2069 7320 7765 6c63 6f6d  bution is welcom
+000011c0: 6521 0a                                  e!.
```

### Comparing `wagtail_maps-0.2.0/README.md` & `wagtail_maps-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -34,172 +34,188 @@
 00000210: 706c 6179 2069 7420 696e 2061 2070 6167  play it in a pag
 00000220: 6520 2d20 652e 672e 2061 7320 6120 5374  e - e.g. as a St
 00000230: 7265 616d 4669 656c 6420 626c 6f63 6b2e  reamField block.
 00000240: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
 00000250: 730a 0a54 6869 7320 7061 636b 6167 6520  s..This package 
 00000260: 7265 7175 6972 6573 2074 6865 2066 6f6c  requires the fol
 00000270: 6c6f 7769 6e67 3a0a 2d20 2a2a 5761 6774  lowing:.- **Wagt
-00000280: 6169 6c20 3e3d 2032 2e31 342a 2a3a 2075  ail >= 2.14**: u
-00000290: 7073 7472 6561 6d20 7061 7463 6865 7320  pstream patches 
-000002a0: 6861 7665 2062 6565 6e20 7375 626d 6974  have been submit
-000002b0: 7465 6420 746f 2070 726f 7669 6465 2061  ted to provide a
-000002c0: 2070 726f 7065 720a 2020 696e 7465 6772   proper.  integr
-000002d0: 6174 696f 6e20 6f66 2074 6869 7320 6578  ation of this ex
-000002e0: 7465 6e73 696f 6e20 696e 746f 2074 6865  tension into the
-000002f0: 2061 646d 696e 202d 2073 6565 205b 2337   admin - see [#7
-00000300: 3536 325d 2c20 5b23 3735 3635 5d20 616e  562], [#7565] an
-00000310: 640a 2020 5b23 3735 3930 5d0a 2d20 2a2a  d.  [#7590].- **
-00000320: 446a 616e 676f 2a2a 2028 332e 312c 2033  Django** (3.1, 3
-00000330: 2e32 290a 2d20 2a2a 5079 7468 6f6e 2033  .2).- **Python 3
-00000340: 2a2a 2028 332e 372c 2033 2e38 2c20 332e  ** (3.7, 3.8, 3.
-00000350: 3929 0a0a 5b23 3735 3632 5d3a 2068 7474  9)..[#7562]: htt
-00000360: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000370: 7761 6774 6169 6c2f 7761 6774 6169 6c2f  wagtail/wagtail/
-00000380: 7075 6c6c 2f37 3536 320a 5b23 3735 3635  pull/7562.[#7565
-00000390: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-000003a0: 622e 636f 6d2f 7761 6774 6169 6c2f 7761  b.com/wagtail/wa
-000003b0: 6774 6169 6c2f 7075 6c6c 2f37 3536 350a  gtail/pull/7565.
-000003c0: 5b23 3735 3930 5d3a 2068 7474 7073 3a2f  [#7590]: https:/
-000003d0: 2f67 6974 6875 622e 636f 6d2f 7761 6774  /github.com/wagt
-000003e0: 6169 6c2f 7761 6774 6169 6c2f 7075 6c6c  ail/wagtail/pull
-000003f0: 2f37 3539 300a 0a23 2320 496e 7374 616c  /7590..## Instal
-00000400: 6c61 7469 6f6e 0a0a 312e 2049 6e73 7461  lation..1. Insta
-00000410: 6c6c 2075 7369 6e67 2060 6070 6970 6060  ll using ``pip``
-00000420: 3a0a 2020 2060 6060 7368 656c 6c0a 2020  :.   ```shell.  
-00000430: 2070 6970 2069 6e73 7461 6c6c 2077 6167   pip install wag
-00000440: 7461 696c 2d6d 6170 730a 2020 2060 6060  tail-maps.   ```
-00000450: 0a32 2e20 4164 6420 6060 7761 6774 6169  .2. Add ``wagtai
-00000460: 6c5f 6d61 7073 6060 2074 6f20 796f 7572  l_maps`` to your
-00000470: 2060 6049 4e53 5441 4c4c 4544 5f41 5050   ``INSTALLED_APP
-00000480: 5360 6020 7365 7474 696e 673a 0a20 2020  S`` setting:.   
-00000490: 6060 6070 7974 686f 6e0a 2020 2049 4e53  ```python.   INS
-000004a0: 5441 4c4c 4544 5f41 5050 5320 3d20 5b0a  TALLED_APPS = [.
-000004b0: 2020 2020 2020 2023 202e 2e2e 0a20 2020         # ....   
-000004c0: 2020 2020 2777 6167 7461 696c 5f6d 6170      'wagtail_map
-000004d0: 7327 2c0a 2020 2020 2020 2023 202e 2e2e  s',.       # ...
-000004e0: 0a20 2020 5d0a 2020 2060 6060 0a33 2e20  .   ].   ```.3. 
-000004f0: 496e 636c 7564 6520 7468 6520 5552 4c20  Include the URL 
-00000500: 6f66 202a 7761 6774 6169 6c2d 6d61 7073  of *wagtail-maps
-00000510: 2a20 746f 2079 6f75 7220 6060 7572 6c73  * to your ``urls
-00000520: 2e70 7960 6020 6669 6c65 3a0a 2020 2060  .py`` file:.   `
-00000530: 6060 7079 7468 6f6e 0a20 2020 6672 6f6d  ``python.   from
-00000540: 2077 6167 7461 696c 5f6d 6170 7320 696d   wagtail_maps im
-00000550: 706f 7274 2075 726c 7320 6173 2077 6167  port urls as wag
-00000560: 7461 696c 6d61 7073 5f75 726c 730a 0a20  tailmaps_urls.. 
-00000570: 2020 7572 6c70 6174 7465 726e 7320 3d20    urlpatterns = 
-00000580: 5b0a 2020 2020 2020 2023 202e 2e2e 0a20  [.       # .... 
-00000590: 2020 2020 2020 7061 7468 2827 6d61 7073        path('maps
-000005a0: 2f27 2c20 696e 636c 7564 6528 7761 6774  /', include(wagt
-000005b0: 6169 6c6d 6170 735f 7572 6c73 2929 2c0a  ailmaps_urls)),.
-000005c0: 2020 2020 2020 2023 202e 2e2e 0a20 2020         # ....   
-000005d0: 5d0a 2020 2060 6060 0a34 2e20 5275 6e20  ].   ```.4. Run 
-000005e0: 6060 7079 7468 6f6e 206d 616e 6167 652e  ``python manage.
-000005f0: 7079 206d 6967 7261 7465 6060 2074 6f20  py migrate`` to 
-00000600: 6372 6561 7465 2074 6865 206d 6f64 656c  create the model
-00000610: 730a 0a23 2320 5573 6167 650a 0a41 2053  s..## Usage..A S
-00000620: 7472 6561 6d46 6965 6c64 2062 6c6f 636b  treamField block
-00000630: 2060 7761 6774 6169 6c5f 6d61 7073 2e62   `wagtail_maps.b
-00000640: 6c6f 636b 732e 4d61 7042 6c6f 636b 6020  locks.MapBlock` 
-00000650: 6361 6e20 6265 2075 7365 6420 746f 2064  can be used to d
-00000660: 6973 706c 6179 2061 0a6d 6170 202d 2063  isplay a.map - c
-00000670: 686f 6f73 656e 2066 726f 6d20 7468 6520  hoosen from the 
-00000680: 6375 7272 656e 7420 6f6e 6573 202d 2069  current ones - i
-00000690: 6e20 796f 7572 2070 6167 652e 2054 6865  n your page. The
-000006a0: 204a 6176 6153 6372 6970 7420 636f 6465   JavaScript code
-000006b0: 2061 6e64 2074 6865 0a4c 6561 666c 6574   and the.Leaflet
-000006c0: 2070 6163 6b61 6765 2069 7320 6375 7272   package is curr
-000006d0: 656e 746c 7920 6e6f 7420 7368 6970 7065  ently not shippe
-000006e0: 642c 2062 7574 2079 6f75 2063 616e 2066  d, but you can f
-000006f0: 696e 6420 616e 2065 7861 6d70 6c65 2069  ind an example i
-00000700: 6e0a 5b65 7861 6d70 6c65 732f 6672 6f6e  n.[examples/fron
-00000710: 7465 6e64 2f5d 2865 7861 6d70 6c65 732f  tend/](examples/
-00000720: 6672 6f6e 7465 6e64 2f29 2e0a 0a23 2320  frontend/)...## 
-00000730: 4465 7665 6c6f 706d 656e 740a 2323 2320  Development.### 
-00000740: 5175 6963 6b20 7374 6172 740a 0a54 6f20  Quick start..To 
-00000750: 7365 7420 7570 2061 2064 6576 656c 6f70  set up a develop
-00000760: 6d65 6e74 2065 6e76 6972 6f6e 6d65 6e74  ment environment
-00000770: 2c20 656e 7375 7265 2074 6861 7420 5079  , ensure that Py
-00000780: 7468 6f6e 2033 2069 7320 696e 7374 616c  thon 3 is instal
-00000790: 6c65 6420 6f6e 2079 6f75 720a 7379 7374  led on your.syst
-000007a0: 656d 2e20 5468 656e 3a0a 0a31 2e20 436c  em. Then:..1. Cl
-000007b0: 6f6e 6520 7468 6973 2072 6570 6f73 6974  one this reposit
-000007c0: 6f72 790a 322e 2043 7265 6174 6520 6120  ory.2. Create a 
-000007d0: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
-000007e0: 656e 7420 616e 6420 6163 7469 7661 7465  ent and activate
-000007f0: 2069 743a 0a20 2020 6060 6073 6865 6c6c   it:.   ```shell
-00000800: 0a20 2020 7079 7468 6f6e 3320 2d6d 2076  .   python3 -m v
-00000810: 656e 7620 7665 6e76 0a20 2020 736f 7572  env venv.   sour
-00000820: 6365 2076 656e 762f 6269 6e2f 6163 7469  ce venv/bin/acti
-00000830: 7661 7465 0a20 2020 6060 600a 332e 2049  vate.   ```.3. I
-00000840: 6e73 7461 6c6c 2074 6869 7320 7061 636b  nstall this pack
-00000850: 6167 6520 696e 2064 6576 656c 6f70 206d  age in develop m
-00000860: 6f64 6520 7769 7468 2065 7874 7261 2072  ode with extra r
-00000870: 6571 7569 7265 6d65 6e74 733a 0a20 2020  equirements:.   
-00000880: 6060 6073 6865 6c6c 0a20 2020 7069 7020  ```shell.   pip 
-00000890: 696e 7374 616c 6c20 2d65 202e 5b74 6573  install -e .[tes
-000008a0: 745d 0a20 2020 6060 600a 0a23 2323 2043  t].   ```..### C
-000008b0: 6f6e 7472 6962 7574 696e 670a 0a54 6865  ontributing..The
-000008c0: 2050 7974 686f 6e20 636f 6465 2069 7320   Python code is 
-000008d0: 666f 726d 6174 7465 6420 616e 6420 6c69  formatted and li
-000008e0: 6e74 6564 2074 6861 6e6b 7320 746f 205b  nted thanks to [
-000008f0: 666c 616b 6538 5d2c 205b 6973 6f72 745d  flake8], [isort]
-00000900: 2061 6e64 205b 626c 6163 6b5d 2e0a 546f   and [black]..To
-00000910: 2065 6173 6520 7468 6520 7573 6520 6f66   ease the use of
-00000920: 2074 6869 7320 746f 6f6c 732c 2074 6865   this tools, the
-00000930: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000940: 6e64 7320 6172 6520 6176 6169 6c61 626c  nds are availabl
-00000950: 653a 0a2d 2060 6d61 6b65 206c 696e 7460  e:.- `make lint`
-00000960: 3a20 6368 6563 6b20 7468 6520 5079 7468  : check the Pyth
-00000970: 6f6e 2063 6f64 6520 7379 6e74 6178 2061  on code syntax a
-00000980: 6e64 2069 6d70 6f72 7473 206f 7264 6572  nd imports order
-00000990: 0a2d 2060 6d61 6b65 2066 6f72 6d61 7460  .- `make format`
-000009a0: 3a20 6669 7820 7468 6520 5079 7468 6f6e  : fix the Python
-000009b0: 2063 6f64 6520 7379 6e74 6178 2061 6e64   code syntax and
-000009c0: 2069 6d70 6f72 7473 206f 7264 6572 0a0a   imports order..
-000009d0: 5468 6520 7465 7374 7320 6172 6520 7772  The tests are wr
-000009e0: 6974 7465 6e20 7769 7468 205b 7079 7465  itten with [pyte
-000009f0: 7374 5d20 616e 6420 636f 6465 2063 6f76  st] and code cov
-00000a00: 6572 6167 6520 6973 206d 6561 7375 7265  erage is measure
-00000a10: 6420 7769 7468 205b 636f 7665 7261 6765  d with [coverage
-00000a20: 5d2e 0a59 6f75 2063 616e 2075 7365 2074  ]..You can use t
-00000a30: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00000a40: 6d61 6e64 7320 666f 7220 7468 6174 3a0a  mands for that:.
-00000a50: 2d20 6060 6d61 6b65 2074 6573 7460 603a  - ``make test``:
-00000a60: 2072 756e 2074 6865 2074 6573 7473 2061   run the tests a
-00000a70: 6e64 206f 7574 7075 7420 6120 7175 6963  nd output a quic
-00000a80: 6b20 7265 706f 7274 206f 6620 636f 6465  k report of code
-00000a90: 2063 6f76 6572 6167 650a 2d20 6060 6d61   coverage.- ``ma
-00000aa0: 6b65 2063 6f76 6572 6167 6560 603a 2072  ke coverage``: r
-00000ab0: 756e 2074 6865 2074 6573 7473 2061 6e64  un the tests and
-00000ac0: 2070 726f 6475 6365 2061 6e20 4854 4d4c   produce an HTML
-00000ad0: 2072 6570 6f72 7420 6f66 2063 6f64 6520   report of code 
-00000ae0: 636f 7665 7261 6765 0a0a 5768 656e 2073  coverage..When s
-00000af0: 7562 6d69 7474 696e 6720 6120 7075 6c6c  ubmitting a pull
-00000b00: 2d72 6571 7565 7374 2c20 706c 6561 7365  -request, please
-00000b10: 2065 6e73 7572 6520 7468 6174 2074 6865   ensure that the
-00000b20: 2063 6f64 6520 6973 2077 656c 6c20 666f   code is well fo
-00000b30: 726d 6174 7465 640a 616e 6420 636f 7665  rmatted.and cove
-00000b40: 7265 642c 2061 6e64 2074 6861 7420 616c  red, and that al
-00000b50: 6c20 7468 6520 6f74 6865 7220 7465 7374  l the other test
-00000b60: 7320 7061 7373 2e0a 0a5b 666c 616b 6538  s pass...[flake8
-00000b70: 5d3a 2068 7474 7073 3a2f 2f66 6c61 6b65  ]: https://flake
-00000b80: 382e 7079 6371 612e 6f72 672f 0a5b 6973  8.pycqa.org/.[is
-00000b90: 6f72 745d 3a20 6874 7470 733a 2f2f 7079  ort]: https://py
-00000ba0: 6371 612e 6769 7468 7562 2e69 6f2f 6973  cqa.github.io/is
-00000bb0: 6f72 742f 0a5b 626c 6163 6b5d 3a20 6874  ort/.[black]: ht
-00000bc0: 7470 733a 2f2f 626c 6163 6b2e 7265 6164  tps://black.read
-00000bd0: 7468 6564 6f63 732e 696f 2f0a 5b70 7974  thedocs.io/.[pyt
-00000be0: 6573 745d 3a20 6874 7470 733a 2f2f 646f  est]: https://do
-00000bf0: 6373 2e70 7974 6573 742e 6f72 672f 0a5b  cs.pytest.org/.[
-00000c00: 636f 7665 7261 6765 5d3a 2068 7474 7073  coverage]: https
-00000c10: 3a2f 2f63 6f76 6572 6167 652e 7265 6164  ://coverage.read
-00000c20: 7468 6564 6f63 732e 696f 2f0a 0a23 2320  thedocs.io/..## 
-00000c30: 4c69 6365 6e73 650a 0a54 6869 7320 6578  License..This ex
-00000c40: 7465 6e73 696f 6e20 6973 206d 6169 6e6c  tension is mainl
-00000c50: 7920 6465 7665 6c6f 7065 6420 6279 205b  y developed by [
-00000c60: 436c 6973 7320 5858 495d 2868 7474 7073  Cliss XXI](https
-00000c70: 3a2f 2f77 7777 2e63 6c69 7373 3231 2e63  ://www.cliss21.c
-00000c80: 6f6d 2920 616e 640a 6c69 6365 6e73 6564  om) and.licensed
-00000c90: 2075 6e64 6572 2074 6865 205b 4147 504c   under the [AGPL
-00000ca0: 7633 2b5d 284c 4943 454e 5345 292e 2041  v3+](LICENSE). A
-00000cb0: 6e79 2063 6f6e 7472 6962 7574 696f 6e20  ny contribution 
-00000cc0: 6973 2077 656c 636f 6d65 210a            is welcome!.
+00000280: 6169 6c2a 2a20 2834 2e31 204c 5453 2c20  ail** (4.1 LTS, 
+00000290: 352e 3029 0a2d 202a 2a44 6a61 6e67 6f2a  5.0).- **Django*
+000002a0: 2a20 2833 2e32 204c 5453 2c20 342e 3220  * (3.2 LTS, 4.2 
+000002b0: 4c54 5329 0a2d 202a 2a50 7974 686f 6e20  LTS).- **Python 
+000002c0: 332a 2a20 2833 2e38 2c20 332e 392c 2033  3** (3.8, 3.9, 3
+000002d0: 2e31 302c 2033 2e31 3129 0a0a 2323 2049  .10, 3.11)..## I
+000002e0: 6e73 7461 6c6c 6174 696f 6e0a 0a31 2e20  nstallation..1. 
+000002f0: 496e 7374 616c 6c20 7573 696e 6720 6060  Install using ``
+00000300: 7069 7060 603a 0a20 2020 6060 6073 6865  pip``:.   ```she
+00000310: 6c6c 0a20 2020 7069 7020 696e 7374 616c  ll.   pip instal
+00000320: 6c20 7761 6774 6169 6c2d 6d61 7073 0a20  l wagtail-maps. 
+00000330: 2020 6060 600a 322e 2041 6464 2060 6077    ```.2. Add ``w
+00000340: 6167 7461 696c 5f6d 6170 7360 6020 746f  agtail_maps`` to
+00000350: 2079 6f75 7220 6060 494e 5354 414c 4c45   your ``INSTALLE
+00000360: 445f 4150 5053 6060 2073 6574 7469 6e67  D_APPS`` setting
+00000370: 3a0a 2020 2060 6060 7079 7468 6f6e 0a20  :.   ```python. 
+00000380: 2020 494e 5354 414c 4c45 445f 4150 5053    INSTALLED_APPS
+00000390: 203d 205b 0a20 2020 2020 2020 2320 2e2e   = [.       # ..
+000003a0: 2e0a 2020 2020 2020 2027 7761 6774 6169  ..       'wagtai
+000003b0: 6c5f 6d61 7073 272c 0a20 2020 2020 2020  l_maps',.       
+000003c0: 2320 2e2e 2e0a 2020 205d 0a20 2020 6060  # ....   ].   ``
+000003d0: 600a 332e 2049 6e63 6c75 6465 2074 6865  `.3. Include the
+000003e0: 2055 524c 206f 6620 2a77 6167 7461 696c   URL of *wagtail
+000003f0: 2d6d 6170 732a 2074 6f20 796f 7572 2060  -maps* to your `
+00000400: 6075 726c 732e 7079 6060 2066 696c 653a  `urls.py`` file:
+00000410: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
+00000420: 2066 726f 6d20 7761 6774 6169 6c5f 6d61   from wagtail_ma
+00000430: 7073 2069 6d70 6f72 7420 7572 6c73 2061  ps import urls a
+00000440: 7320 7761 6774 6169 6c6d 6170 735f 7572  s wagtailmaps_ur
+00000450: 6c73 0a0a 2020 2075 726c 7061 7474 6572  ls..   urlpatter
+00000460: 6e73 203d 205b 0a20 2020 2020 2020 2320  ns = [.       # 
+00000470: 2e2e 2e0a 2020 2020 2020 2070 6174 6828  ....       path(
+00000480: 276d 6170 732f 272c 2069 6e63 6c75 6465  'maps/', include
+00000490: 2877 6167 7461 696c 6d61 7073 5f75 726c  (wagtailmaps_url
+000004a0: 7329 292c 0a20 2020 2020 2020 2320 2e2e  s)),.       # ..
+000004b0: 2e0a 2020 205d 0a20 2020 6060 600a 342e  ..   ].   ```.4.
+000004c0: 2052 756e 2060 6070 7974 686f 6e20 6d61   Run ``python ma
+000004d0: 6e61 6765 2e70 7920 6d69 6772 6174 6560  nage.py migrate`
+000004e0: 6020 746f 2063 7265 6174 6520 7468 6520  ` to create the 
+000004f0: 6d6f 6465 6c73 0a0a 2323 2055 7361 6765  models..## Usage
+00000500: 0a0a 4120 5374 7265 616d 4669 656c 6420  ..A StreamField 
+00000510: 626c 6f63 6b20 6077 6167 7461 696c 5f6d  block `wagtail_m
+00000520: 6170 732e 626c 6f63 6b73 2e4d 6170 426c  aps.blocks.MapBl
+00000530: 6f63 6b60 2063 616e 2062 6520 7573 6564  ock` can be used
+00000540: 2074 6f20 6469 7370 6c61 7920 610a 6769   to display a.gi
+00000550: 7665 6e20 604d 6170 6020 6f62 6a65 6374  ven `Map` object
+00000560: 2077 6974 6820 6974 7320 706f 696e 7473   with its points
+00000570: 2069 6e20 796f 7572 2070 6167 652e 2054   in your page. T
+00000580: 6f20 7265 6e64 6572 2074 6869 7320 626c  o render this bl
+00000590: 6f63 6b20 696e 2079 6f75 720a 6672 6f6e  ock in your.fron
+000005a0: 7465 6e64 2c20 796f 7520 7769 6c6c 2068  tend, you will h
+000005b0: 6176 6520 746f 2069 6e63 6c75 6465 2074  ave to include t
+000005c0: 6865 2066 6f6c 6c6f 7769 6e67 2061 7373  he following ass
+000005d0: 6574 7320 696e 2074 6865 2074 656d 706c  ets in the templ
+000005e0: 6174 6573 2077 6869 6368 0a63 616e 2063  ates which.can c
+000005f0: 6f6e 7461 696e 2069 7420 2d20 6f72 2069  ontain it - or i
+00000600: 6e20 796f 7572 2062 6173 6520 7465 6d70  n your base temp
+00000610: 6c61 7465 3a0a 0a2a 2074 6865 204a 6176  late:..* the Jav
+00000620: 6153 6372 6970 7420 636f 6465 2074 6861  aScript code tha
+00000630: 7420 7265 6e64 6572 7320 7468 6520 6d61  t renders the ma
+00000640: 7020 7769 7468 205b 4c65 6166 6c65 745d  p with [Leaflet]
+00000650: 2074 6861 6e6b 7320 746f 2061 0a20 205b   thanks to a.  [
+00000660: 5374 696d 756c 7573 5d20 636f 6e74 726f  Stimulus] contro
+00000670: 6c6c 6572 3a0a 2020 6060 6064 6a61 6e67  ller:.  ```djang
+00000680: 6f0a 2020 3c73 6372 6970 7420 7372 633d  o.  <script src=
+00000690: 227b 2520 7374 6174 6963 2022 7761 6774  "{% static "wagt
+000006a0: 6169 6c5f 6d61 7073 2f6a 732f 6d61 702d  ail_maps/js/map-
+000006b0: 626c 6f63 6b2e 6a73 2220 257d 223e 3c2f  block.js" %}"></
+000006c0: 7363 7269 7074 3e0a 2020 6060 600a 2a20  script>.  ```.* 
+000006d0: 7468 6520 6465 6661 756c 7420 4c65 6166  the default Leaf
+000006e0: 6c65 7420 7374 796c 6573 6865 6574 2069  let stylesheet i
+000006f0: 6620 796f 7520 646f 6e27 7420 7072 6f76  f you don't prov
+00000700: 6964 6520 796f 7572 206f 776e 3a0a 2020  ide your own:.  
+00000710: 6060 6064 6a61 6e67 6f0a 2020 3c6c 696e  ```django.  <lin
+00000720: 6b20 7265 6c3d 2273 7479 6c65 7368 6565  k rel="styleshee
+00000730: 7422 2068 7265 663d 227b 2520 7374 6174  t" href="{% stat
+00000740: 6963 2022 7761 6774 6169 6c5f 6d61 7073  ic "wagtail_maps
+00000750: 2f76 656e 646f 722f 6c65 6166 6c65 742e  /vendor/leaflet.
+00000760: 6373 7322 2025 7d22 3e0a 2020 6060 600a  css" %}">.  ```.
+00000770: 0a5b 4c65 6166 6c65 745d 3a20 6874 7470  .[Leaflet]: http
+00000780: 733a 2f2f 6c65 6166 6c65 746a 732e 636f  s://leafletjs.co
+00000790: 6d2f 0a5b 5374 696d 756c 7573 5d3a 2068  m/.[Stimulus]: h
+000007a0: 7474 7073 3a2f 2f73 7469 6d75 6c75 732e  ttps://stimulus.
+000007b0: 686f 7477 6972 6564 2e64 6576 2f0a 0a23  hotwired.dev/..#
+000007c0: 2320 4465 7665 6c6f 706d 656e 740a 2323  # Development.##
+000007d0: 2320 5175 6963 6b20 7374 6172 740a 0a54  # Quick start..T
+000007e0: 6f20 7365 7420 7570 2061 2064 6576 656c  o set up a devel
+000007f0: 6f70 6d65 6e74 2065 6e76 6972 6f6e 6d65  opment environme
+00000800: 6e74 2c20 656e 7375 7265 2074 6861 7420  nt, ensure that 
+00000810: 5079 7468 6f6e 2033 2069 7320 696e 7374  Python 3 is inst
+00000820: 616c 6c65 6420 6f6e 2079 6f75 720a 7379  alled on your.sy
+00000830: 7374 656d 2e20 5468 656e 3a0a 0a31 2e20  stem. Then:..1. 
+00000840: 436c 6f6e 6520 7468 6973 2072 6570 6f73  Clone this repos
+00000850: 6974 6f72 790a 322e 2043 7265 6174 6520  itory.2. Create 
+00000860: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
+00000870: 6e6d 656e 7420 616e 6420 6163 7469 7661  nment and activa
+00000880: 7465 2069 743a 0a20 2020 6060 6073 6865  te it:.   ```she
+00000890: 6c6c 0a20 2020 7079 7468 6f6e 3320 2d6d  ll.   python3 -m
+000008a0: 2076 656e 7620 7665 6e76 0a20 2020 736f   venv venv.   so
+000008b0: 7572 6365 2076 656e 762f 6269 6e2f 6163  urce venv/bin/ac
+000008c0: 7469 7661 7465 0a20 2020 6060 600a 332e  tivate.   ```.3.
+000008d0: 2049 6e73 7461 6c6c 2074 6869 7320 7061   Install this pa
+000008e0: 636b 6167 6520 616e 6420 6974 7320 7265  ckage and its re
+000008f0: 7175 6972 656d 656e 7473 3a0a 2020 2060  quirements:.   `
+00000900: 6060 7368 656c 6c0a 2020 2028 7665 6e76  ``shell.   (venv
+00000910: 2924 2070 6970 2069 6e73 7461 6c6c 202d  )$ pip install -
+00000920: 7220 7265 7175 6972 656d 656e 7473 2d64  r requirements-d
+00000930: 6576 2e74 7874 0a20 2020 6060 600a 0a23  ev.txt.   ```..#
+00000940: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000950: 0a54 6865 2074 6573 7473 2061 7265 2077  .The tests are w
+00000960: 7269 7474 656e 2077 6974 6820 5b70 7974  ritten with [pyt
+00000970: 6573 745d 2061 6e64 2063 6f64 6520 636f  est] and code co
+00000980: 7665 7261 6765 2069 7320 6d65 6173 7572  verage is measur
+00000990: 6564 2077 6974 6820 5b63 6f76 6572 6167  ed with [coverag
+000009a0: 655d 2e0a 596f 7520 6361 6e20 7573 6520  e]..You can use 
+000009b0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+000009c0: 6d6d 616e 6473 2077 6869 6c65 2064 6576  mmands while dev
+000009d0: 656c 6f70 696e 673a 0a2d 2060 606d 616b  eloping:.- ``mak
+000009e0: 6520 7465 7374 6060 3a20 7275 6e20 7468  e test``: run th
+000009f0: 6520 7465 7374 7320 616e 6420 6f75 7470  e tests and outp
+00000a00: 7574 2061 2071 7569 636b 2072 6570 6f72  ut a quick repor
+00000a10: 7420 6f66 2063 6f64 6520 636f 7665 7261  t of code covera
+00000a20: 6765 0a2d 2060 606d 616b 6520 7465 7374  ge.- ``make test
+00000a30: 2d77 6970 6060 3a20 6f6e 6c79 2072 756e  -wip``: only run
+00000a40: 2074 6865 2074 6573 7473 206d 6172 6b65   the tests marke
+00000a50: 6420 6173 2027 7769 7027 0a2d 2060 606d  d as 'wip'.- ``m
+00000a60: 616b 6520 7465 7374 2d61 6c6c 6060 3a20  ake test-all``: 
+00000a70: 7275 6e20 7468 6520 7465 7374 7320 6f6e  run the tests on
+00000a80: 2061 6c6c 2073 7570 706f 7274 6564 2076   all supported v
+00000a90: 6572 7369 6f6e 7320 6f66 2044 6a61 6e67  ersions of Djang
+00000aa0: 6f20 616e 640a 2020 5761 6774 6169 6c20  o and.  Wagtail 
+00000ab0: 7769 7468 205b 6e6f 785d 0a0a 5468 6520  with [nox]..The 
+00000ac0: 5079 7468 6f6e 2063 6f64 6520 6973 2066  Python code is f
+00000ad0: 6f72 6d61 7474 6564 2061 6e64 206c 696e  ormatted and lin
+00000ae0: 7465 6420 7468 616e 6b73 2074 6f20 5b66  ted thanks to [f
+00000af0: 6c61 6b65 385d 2c20 5b69 736f 7274 5d20  lake8], [isort] 
+00000b00: 616e 6420 5b62 6c61 636b 5d2e 0a41 6c6c  and [black]..All
+00000b10: 206f 6620 7468 6573 6520 746f 6f6c 7320   of these tools 
+00000b20: 6172 6520 636f 6e66 6967 7572 6564 2069  are configured i
+00000b30: 6e20 5b70 7265 2d63 6f6d 6d69 745d 2061  n [pre-commit] a
+00000b40: 6e64 2079 6f75 2073 686f 756c 6420 636f  nd you should co
+00000b50: 6e73 6964 6572 2074 6f0a 696e 7374 616c  nsider to.instal
+00000b60: 6c20 6974 7320 6769 7420 686f 6f6b 2073  l its git hook s
+00000b70: 6372 6970 7473 2062 7920 7275 6e6e 696e  cripts by runnin
+00000b80: 673a 0a60 6060 7368 656c 6c0a 2876 656e  g:.```shell.(ven
+00000b90: 7629 2420 7072 652d 636f 6d6d 6974 2069  v)$ pre-commit i
+00000ba0: 6e73 7461 6c6c 0a60 6060 0a0a 5768 656e  nstall.```..When
+00000bb0: 2073 7562 6d69 7474 696e 6720 6120 7075   submitting a pu
+00000bc0: 6c6c 2d72 6571 7565 7374 2c20 706c 6561  ll-request, plea
+00000bd0: 7365 2065 6e73 7572 6520 7468 6174 2074  se ensure that t
+00000be0: 6865 2063 6f64 6520 6973 2077 656c 6c20  he code is well 
+00000bf0: 666f 726d 6174 7465 640a 616e 6420 636f  formatted.and co
+00000c00: 7665 7265 642c 2061 6e64 2074 6861 7420  vered, and that 
+00000c10: 616c 6c20 7468 6520 7465 7374 7320 7061  all the tests pa
+00000c20: 7373 2e0a 0a5b 7079 7465 7374 5d3a 2068  ss...[pytest]: h
+00000c30: 7474 7073 3a2f 2f64 6f63 732e 7079 7465  ttps://docs.pyte
+00000c40: 7374 2e6f 7267 2f0a 5b63 6f76 6572 6167  st.org/.[coverag
+00000c50: 655d 3a20 6874 7470 733a 2f2f 636f 7665  e]: https://cove
+00000c60: 7261 6765 2e72 6561 6474 6865 646f 6373  rage.readthedocs
+00000c70: 2e69 6f2f 0a5b 6e6f 785d 3a20 6874 7470  .io/.[nox]: http
+00000c80: 733a 2f2f 6e6f 782e 7468 6561 2e63 6f64  s://nox.thea.cod
+00000c90: 6573 2f0a 5b66 6c61 6b65 385d 3a20 6874  es/.[flake8]: ht
+00000ca0: 7470 733a 2f2f 666c 616b 6538 2e70 7963  tps://flake8.pyc
+00000cb0: 7161 2e6f 7267 2f0a 5b69 736f 7274 5d3a  qa.org/.[isort]:
+00000cc0: 2068 7474 7073 3a2f 2f70 7963 7161 2e67   https://pycqa.g
+00000cd0: 6974 6875 622e 696f 2f69 736f 7274 2f0a  ithub.io/isort/.
+00000ce0: 5b62 6c61 636b 5d3a 2068 7474 7073 3a2f  [black]: https:/
+00000cf0: 2f62 6c61 636b 2e72 6561 6474 6865 646f  /black.readthedo
+00000d00: 6373 2e69 6f2f 0a5b 7072 652d 636f 6d6d  cs.io/.[pre-comm
+00000d10: 6974 5d3a 2068 7474 7073 3a2f 2f70 7265  it]: https://pre
+00000d20: 2d63 6f6d 6d69 742e 636f 6d2f 0a0a 2323  -commit.com/..##
+00000d30: 204c 6963 656e 7365 0a0a 5468 6973 2065   License..This e
+00000d40: 7874 656e 7369 6f6e 2069 7320 6d61 696e  xtension is main
+00000d50: 6c79 2064 6576 656c 6f70 6564 2062 7920  ly developed by 
+00000d60: 5b43 6c69 7373 2058 5849 5d28 6874 7470  [Cliss XXI](http
+00000d70: 733a 2f2f 7777 772e 636c 6973 7332 312e  s://www.cliss21.
+00000d80: 636f 6d29 2061 6e64 0a6c 6963 656e 7365  com) and.license
+00000d90: 6420 756e 6465 7220 7468 6520 5b41 4750  d under the [AGP
+00000da0: 4c76 332b 5d28 4c49 4345 4e53 4529 2e20  Lv3+](LICENSE). 
+00000db0: 416e 7920 636f 6e74 7269 6275 7469 6f6e  Any contribution
+00000dc0: 2069 7320 7765 6c63 6f6d 6521 0a          is welcome!.
```

### Comparing `wagtail_maps-0.2.0/pyproject.toml` & `wagtail_maps-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 [build-system]
-requires = ["setuptools >=42", "wheel", "setuptools_scm[toml] >=3.4"]
-build-backend = "setuptools.build_meta"
+requires = ['setuptools >=45', 'wheel', 'setuptools_scm[toml] >=6.2']
+build-backend = 'setuptools.build_meta'
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 80
 skip-string-normalization = true
-exclude = '''
-/(
-   \.git
-   | venv
-   | migrations
-)/
-'''
+extend-exclude = '/migrations/'
 
 [tool.isort]
 profile = 'black'
 line_length = 80
 known_django = 'django'
 known_wagtail = 'wagtail'
 sections = [
   'FUTURE', 'STDLIB', 'DJANGO', 'WAGTAIL', 'THIRDPARTY', 'FIRSTPARTY', 'LOCALFOLDER'
 ]
 skip_glob = '**/migrations/*.py'
 
 [tool.pytest.ini_options]
-addopts = '--ds=tests.settings'
-python_files = ['test_*.py']
+pythonpath = '.'
 testpaths = ['tests']
 markers = ['wip: mark a test as a work in progress']
+DJANGO_SETTINGS_MODULE = 'tests.settings'
 
 [tool.coverage.run]
 branch = true
 source = ['wagtail_maps']
 
 [tool.coverage.report]
 exclude_lines = ['# pragma: no cover', 'raise NotImplementedError']
-show_missing = true
```

### Comparing `wagtail_maps-0.2.0/setup.cfg` & `wagtail_maps-0.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -3,54 +3,40 @@
 description = Create and display maps with points in Wagtail
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Cliss XXI
 author_email = contact@cliss21.com
 license = AGPLv3+
 project_urls = 
-	Bug Tracker = https://forge.cliss21.org/cliss21/wagtail-maps/issues
-	Source Code = https://forge.cliss21.org/cliss21/wagtail-maps
+	Bug Tracker = https://framagit.org/cliss21/wagtail-maps/-/issues
+	Source Code = https://framagit.org/cliss21/wagtail-maps
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Wagtail
-	Framework :: Wagtail :: 2
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Affero General Public License v3
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 keywords = 
 	wagtail
 	map
 	leaflet
 
 [options]
-include_package_data = True
-install_requires = 
-	wagtail >=2.14
 packages = wagtail_maps
-python_requires = >=3.7, <4
-setup_requires = 
-	setuptools_scm
-
-[options.extras_require]
-test = 
-	pytest
-	pytest-cov
-	pytest-django
-	factory-boy
-	black
-	flake8 >=3.5
-	flake8-black
-	flake8-isort
-	isort >=5.0
+install_requires = 
+	wagtail >=4.1
+python_requires = >=3.8, <4
+include_package_data = True
 
 [flake8]
 exclude = 
 	*/migrations/*
 max-line-length = 80
 
 [egg_info]
```

### Comparing `wagtail_maps-0.2.0/tests/factories.py` & `wagtail_maps-0.3.0/tests/factories.py`

 * *Files identical despite different names*

### Comparing `wagtail_maps-0.2.0/tests/settings.py` & `wagtail_maps-0.3.0/tests/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     'wagtail.contrib.modeladmin',
     'wagtail.sites',
     'wagtail.users',
     'wagtail.documents',
     'wagtail.images',
     'wagtail.search',
     'wagtail.admin',
-    'wagtail.core',
+    'wagtail',
     'modelcluster',
     'taggit',
     # wagtail_maps
     'wagtail_maps',
     'tests',
 ]
```

### Comparing `wagtail_maps-0.2.0/tests/test_api.py` & `wagtail_maps-0.3.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             content='<p>Lorem <a id="{}" linktype="page">ipsum</a></p>'.format(
                 root_page.id
             ),
             map_id=map_example.id,
         )
         points = self.get_detail_response(map_example.id).json()['points']
         content = BeautifulSoup(points[-1]['content'], 'html5lib')
-        assert content.select_one('span', text='Point title')
+        assert content.select_one('h5', text='Point title')
         assert content.select_one('p', text='Lorem')
         link = content.select_one('a', tex_t='ipsum')
         assert link['href'] == root_page.url
 
     def test_detail_content_with_url(self, map_example):
         PointFactory(
             title='Point with link',
```

### Comparing `wagtail_maps-0.2.0/tests/test_blocks.py` & `wagtail_maps-0.3.0/tests/test_blocks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.core.exceptions import ValidationError
+
 import pytest
 from pytest_django.asserts import assertHTMLEqual
 
 from wagtail_maps.blocks import MapBlock
 
 from .factories import MapFactory
 
@@ -25,50 +27,71 @@
     @pytest.mark.parametrize('value', ('', None, '10'))
     def test_form_response_map_none(self, value):
         MapFactory.create_batch(2)
 
         value = self.block.value_from_datadict({'p-map': value}, {}, 'p')
         assert value['map'] is None
 
+    def test_get_form_state(self):
+        assert self.block.get_form_state(
+            {'map': 1, 'height': 400, 'zoom': 1}
+        ) == {'height': '400', 'map': ['1'], 'zoom': '1'}
+
     def test_render(self):
         assertHTMLEqual(
             self.render(
                 {
                     'map': MapFactory(
                         center_latitude=0.0, center_longitude=1.0
                     ).id
                 }
             ),
             """
-            <div class="map" data-map
-              data-map-api-url="/maps/api/v1/1/"
-              data-map-center-lat="0.0000"
-              data-map-center-lng="1.0000">
+            <div class="map" data-controller="map"
+              data-map-api-url-value="/maps/api/v1/1/"
+              data-map-center-value="[0.0, 1.0]">
             </div>
             """,
         )
 
     def test_render_with_attrs(self):
         assertHTMLEqual(
             self.render(
                 {
                     'map': MapFactory(
-                        center_latitude=0.0, center_longitude=1.0, min_zoom=2
+                        center_latitude=0.0, center_longitude=1.0
                     ).id,
+                    'min_zoom': '2',
+                    'max_zoom': '10',
                     'zoom': '1',
                     'height': '10',
                 }
             ),
             """
-            <div class="map" data-map
-              data-map-api-url="/maps/api/v1/1/"
-              data-map-center-lat="0.0000"
-              data-map-center-lng="1.0000"
-              data-map-height="10"
-              data-map-min-zoom="2"
-              data-map-zoom="1">
+            <div class="map" data-controller="map"
+              data-map-api-url-value="/maps/api/v1/1/"
+              data-map-center-value="[0.0, 1.0]"
+              data-map-height-value="10"
+              data-map-min-zoom-value="2"
+              data-map-max-zoom-value="10"
+              data-map-zoom-value="1">
             </div>
             """,
         )
 
     def test_render_unknown(self):
         assert self.render({'map': '100'}) == ''
+
+    def test_clean_min_max_zoom(self):
+        data = {'map': MapFactory().id}
+
+        self.block.clean(data)
+
+        data['min_zoom'] = 10
+        self.block.clean(data)
+
+        data['max_zoom'] = 15
+        self.block.clean(data)
+
+        with pytest.raises(ValidationError):
+            data['max_zoom'] = 5
+            self.block.clean(data)
```

### Comparing `wagtail_maps-0.2.0/tests/urls.py` & `wagtail_maps-0.3.0/tests/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 from django.urls import include, path
 
+from wagtail import urls as wagtail_urls
 from wagtail.admin import urls as wagtailadmin_urls
-from wagtail.core import urls as wagtail_urls
 from wagtail.documents import urls as wagtaildocs_urls
 
 from wagtail_maps import urls as wagtailmaps_urls
 
 urlpatterns = [
     path('admin/', include(wagtailadmin_urls)),
     path('documents/', include(wagtaildocs_urls)),
```

### Comparing `wagtail_maps-0.2.0/wagtail_maps/api/serializers.py` & `wagtail_maps-0.3.0/wagtail_maps/api/serializers.py`

 * *Files identical despite different names*

### Comparing `wagtail_maps-0.2.0/wagtail_maps/locale/fr/LC_MESSAGES/django.po` & `wagtail_maps-0.3.0/wagtail_maps/locale/fr/LC_MESSAGES/django.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,170 +1,153 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: wagtail-maps\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-10-15 15:33+0200\n"
-"PO-Revision-Date: 2021-10-15 15:36+0200\n"
+"POT-Creation-Date: 2023-06-07 11:40+0200\n"
+"PO-Revision-Date: 2023-06-07 11:42+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: admin.py:29
+#: admin.py:26
 msgid "Latitude"
 msgstr "Latitude"
 
-#: admin.py:30
+#: admin.py:27
 msgid "Longitude"
 msgstr "Longitude"
 
-#: admin.py:37
+#: admin.py:29
 msgid "Center of the map"
 msgstr "Centre de la carte"
 
-#: admin.py:43
-msgid "Minimum"
-msgstr "Minimum"
-
-#: admin.py:44
-msgid "Maximum"
-msgstr "Maximum"
-
-#: admin.py:48
-msgid "Zoom levels"
-msgstr "Niveaux de zoom"
-
-#: admin.py:64 admin.py:73
+#: admin.py:42 admin.py:51
 msgid "Points"
 msgstr "Points"
 
-#: admin.py:65
+#: admin.py:43
 msgid "Point"
 msgstr "Point"
 
-#: blocks.py:19 blocks.py:51
+#: blocks.py:25 blocks.py:72
 msgid "Map"
 msgstr "Carte"
 
-#: blocks.py:38
+#: blocks.py:47
 msgid "Height (px)"
 msgstr "Hauteur (px)"
 
-#: blocks.py:43
+#: blocks.py:52
 msgid "Initial zoom"
 msgstr "Zoom initial"
 
-#: models.py:19
+#: blocks.py:58
+msgid "Minimum zoom level"
+msgstr "Niveau de zoom minimum"
+
+#: blocks.py:64
+msgid "Maximum zoom level"
+msgstr "Niveau de zoom maximum"
+
+#: blocks.py:88
+msgid "Minimum zoom level must be smaller than maximum."
+msgstr "Le niveau de zoom minimum doit être plus petit que le maximum."
+
+#: models.py:13
 msgid "name"
 msgstr "nom"
 
-#: models.py:22
+#: models.py:16
 msgid "center point's latitude"
 msgstr "latitude du point central"
 
-#: models.py:27
+#: models.py:21
 msgid "center point's longitude"
 msgstr "longitude du point central"
 
-#: models.py:32
-msgid "minimum zoom level"
-msgstr "niveau de zoom minimum"
-
-#: models.py:38
-msgid "maximum zoom level"
-msgstr "niveau de zoom maximum"
-
-#: models.py:45
+#: models.py:27
 msgid "map"
 msgstr "carte"
 
-#: models.py:46
+#: models.py:28
 msgid "maps"
 msgstr "cartes"
 
-#: models.py:53
-msgid "Minimum zoom level must be smaller than maximum."
-msgstr "Le niveau de zoom minimum doit être plus petit que le maximum."
-
-#: models.py:58
+#: models.py:35
 msgid "title"
 msgstr "Titre"
 
-#: models.py:60
+#: models.py:37
 msgid "content"
 msgstr "Contenu"
 
-#: models.py:66
+#: models.py:43
 msgid "link to a page"
 msgstr "lien vers une page"
 
-#: models.py:73
+#: models.py:50
 msgid "link to an URL"
 msgstr "lien vers une URL"
 
-#: models.py:78
+#: models.py:55
 msgid "latitude"
 msgstr "latitude"
 
-#: models.py:83
+#: models.py:60
 msgid "longitude"
 msgstr "longitude"
 
-#: models.py:91
+#: models.py:68
 msgid "point"
 msgstr "point"
 
-#: models.py:92
+#: models.py:69
 msgid "points"
 msgstr "points"
 
-#: models.py:96
+#: models.py:73
 msgid "Choose between a link to a page or an URL."
 msgstr "Choisissez entre un lien vers une page ou une URL."
 
-#: templates/modeladmin/wagtail_maps/map/_geo_modal.html:6
-#: templates/wagtail_maps/popup_content.html:9
-msgid "Close"
-msgstr "Fermer"
+#: templates/wagtail_maps/panels/map_center_coordinates.html:7
+msgid "Calculate from the points"
+msgstr "Calculer à partir des points"
 
-#: templates/modeladmin/wagtail_maps/map/_geo_modal.html:9
+#: templates/wagtail_maps/panels/map_center_coordinates.html:11
+msgid ""
+"Unable to calculate the geometric center of the points. Verify that you have "
+"at least one point with valid latitude and longitude."
+msgstr ""
+"Impossible de calculer le centre géographique des points. Vérifiez qu'au "
+"moins un point est défini avec une latitude et longitude valides."
+
+#: templates/wagtail_maps/panels/point_coordinates.html:5
+msgid "Coordinates from geo URI…"
+msgstr "Coordonnées depuis une URI géo…"
+
+#: templates/wagtail_maps/panels/point_coordinates.html:8
 msgid "Coordinates of the point"
 msgstr "Coordonnées du point"
 
-#: templates/modeladmin/wagtail_maps/map/_geo_modal.html:12
+#: templates/wagtail_maps/panels/point_coordinates.html:11
 msgid ""
 "Enter the geo URI of your point to set its latitude and longitude "
 "accordingly."
 msgstr ""
-"Entrez l'URI géo du point pour définir sa latitude et sa longitude "
-"en conséquence."
+"Entrez l'URI géo du point pour définir sa latitude et sa longitude en "
+"conséquence."
 
-#: templates/modeladmin/wagtail_maps/map/_geo_modal.html:17
+#: templates/wagtail_maps/panels/point_coordinates.html:14
 msgid "Set coordinates"
 msgstr "Définir les coordonnées"
 
-#: templates/modeladmin/wagtail_maps/map/_geo_modal.html:20
+#: templates/wagtail_maps/panels/point_coordinates.html:17
 msgid ""
 "Unable to parse the geo URI. Verify that it is in the form of "
 "<code>geo:1.0,2.0</code>."
 msgstr ""
 "Impossible d'analyser l'URI géo. Vérifiez qu'elle est de la forme "
 "<code>geo:1.0,2.0</code>."
-
-#: templates/wagtail_maps/edit_handlers/center_calculate.html:3
-msgid "Calculate from the points"
-msgstr "Calculer à partir des points"
-
-#: templates/wagtail_maps/edit_handlers/center_calculate.html:7
-msgid ""
-"Unable to calculate the geometric center of the points. Verify that you have "
-"at least one point with valid latitude and longitude."
-msgstr ""
-"Impossible de calculer le centre géographique des points. Vérifiez qu'au "
-"moins un point est défini avec une latitude et longitude valides."
-
-#: templates/wagtail_maps/edit_handlers/point_from_geo.html:3
-msgid "Coordinates from geo URI…"
-msgstr "Coordonnées depuis une URI géo…"
```

### Comparing `wagtail_maps-0.2.0/wagtail_maps/migrations/0001_initial.py` & `wagtail_maps-0.3.0/wagtail_maps/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by Django 3.2.7 on 2021-10-12 07:35
 
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 import modelcluster.fields
-import wagtail.core.fields
+import wagtail.fields
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -32,15 +32,15 @@
             },
         ),
         migrations.CreateModel(
             name='Point',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('title', models.CharField(max_length=50, verbose_name='title')),
-                ('content', wagtail.core.fields.RichTextField(blank=True, verbose_name='content')),
+                ('content', wagtail.fields.RichTextField(blank=True, verbose_name='content')),
                 ('external_link', models.URLField(blank=True, verbose_name='link to an URL')),
                 ('latitude', models.DecimalField(decimal_places=4, max_digits=7, verbose_name='latitude')),
                 ('longitude', models.DecimalField(decimal_places=4, max_digits=7, verbose_name='longitude')),
                 ('map', modelcluster.fields.ParentalKey(on_delete=django.db.models.deletion.CASCADE, related_name='points', to='wagtail_maps.map')),
                 ('page_link', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to='wagtailcore.page', verbose_name='link to a page')),
             ],
             options={
```

### Comparing `wagtail_maps-0.2.0/wagtail_maps/models.py` & `wagtail_maps-0.3.0/wagtail_maps/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,39 @@
 from django.core.exceptions import ValidationError
-from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
 
-from wagtail.core.fields import RichTextField
+from wagtail.fields import RichTextField
 
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
 
-zoom_validators = [
-    MinValueValidator(1),
-    MaxValueValidator(20),
-]
-
 
 class Map(ClusterableModel):
     name = models.CharField(verbose_name=_("name"), max_length=30)
 
     center_latitude = models.DecimalField(
         verbose_name=_("center point's latitude"),
         max_digits=7,
         decimal_places=4,
     )
     center_longitude = models.DecimalField(
         verbose_name=_("center point's longitude"),
         max_digits=7,
         decimal_places=4,
     )
-    min_zoom = models.PositiveSmallIntegerField(
-        verbose_name=_("minimum zoom level"),
-        blank=True,
-        null=True,
-        validators=zoom_validators,
-    )
-    max_zoom = models.PositiveSmallIntegerField(
-        verbose_name=_("maximum zoom level"),
-        blank=True,
-        null=True,
-        validators=zoom_validators,
-    )
 
     class Meta:
         verbose_name = _("map")
         verbose_name_plural = _("maps")
 
     def __str__(self):
         return self.name
 
-    def clean(self):
-        if self.min_zoom and self.max_zoom and self.min_zoom > self.max_zoom:
-            msg = gettext("Minimum zoom level must be smaller than maximum.")
-            raise ValidationError({'min_zoom': msg, 'max_zoom': msg})
-
 
 class Point(models.Model):
     title = models.CharField(verbose_name=_("title"), max_length=50)
     content = RichTextField(
         verbose_name=_("content"),
         blank=True,
         features=['bold', 'italic', 'ol', 'ul', 'link'],
```

### Comparing `wagtail_maps-0.2.0/wagtail_maps.egg-info/SOURCES.txt` & `wagtail_maps-0.3.0/wagtail_maps.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 .babelrc.json
 .editorconfig
-.eslintrc.json
+.eslintrc.js
+.gitattributes
 .gitignore
+.gitlab-ci.yml
+.pre-commit-config.yaml
 .prettierrc
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
+noxfile.py
 package-lock.json
 package.json
 pyproject.toml
+requirements-dev.txt
+requirements-test.txt
+rollup.config.mjs
 setup.cfg
-setup.py
-tox.ini
-webpack.config.js
-examples/frontend/README.md
-examples/frontend/js/main.js
-examples/frontend/js/map.js
-examples/frontend/scss/_leaflet.scss
+client/src/admin-form.js
+client/src/admin-form_controllers.js
+client/src/map-block.js
+client/src/controllers/geo-coordinates.js
+client/src/controllers/map-center-coordinates.js
+client/src/controllers/map.js
 tests/__init__.py
 tests/conftest.py
 tests/factories.py
 tests/settings.py
 tests/test_admin.py
 tests/test_api.py
 tests/test_blocks.py
 tests/urls.py
 wagtail_maps/__init__.py
 wagtail_maps/admin.py
 wagtail_maps/apps.py
 wagtail_maps/blocks.py
 wagtail_maps/models.py
+wagtail_maps/panels.py
 wagtail_maps/urls.py
 wagtail_maps/wagtail_hooks.py
 wagtail_maps.egg-info/PKG-INFO
 wagtail_maps.egg-info/SOURCES.txt
 wagtail_maps.egg-info/dependency_links.txt
 wagtail_maps.egg-info/requires.txt
 wagtail_maps.egg-info/top_level.txt
 wagtail_maps/api/__init__.py
 wagtail_maps/api/serializers.py
 wagtail_maps/api/views.py
 wagtail_maps/locale/fr/LC_MESSAGES/django.mo
 wagtail_maps/locale/fr/LC_MESSAGES/django.po
 wagtail_maps/migrations/0001_initial.py
+wagtail_maps/migrations/0002_remove_map_max_zoom_remove_map_min_zoom.py
 wagtail_maps/migrations/__init__.py
 wagtail_maps/static/wagtail_maps/css/admin-form.css
 wagtail_maps/static/wagtail_maps/js/admin-form.js
 wagtail_maps/static/wagtail_maps/js/admin-form.js.map
-wagtail_maps/templates/modeladmin/wagtail_maps/map/_geo_modal.html
-wagtail_maps/templates/modeladmin/wagtail_maps/map/create.html
-wagtail_maps/templates/modeladmin/wagtail_maps/map/edit.html
+wagtail_maps/static/wagtail_maps/js/admin-form_controllers.js
+wagtail_maps/static/wagtail_maps/js/admin-form_controllers.js.map
+wagtail_maps/static/wagtail_maps/js/map-block.js
+wagtail_maps/static/wagtail_maps/js/map-block.js.map
+wagtail_maps/static/wagtail_maps/vendor/leaflet.css
+wagtail_maps/static/wagtail_maps/vendor/images/layers-2x.png
+wagtail_maps/static/wagtail_maps/vendor/images/layers.png
+wagtail_maps/static/wagtail_maps/vendor/images/marker-icon-2x.png
+wagtail_maps/static/wagtail_maps/vendor/images/marker-icon.png
+wagtail_maps/static/wagtail_maps/vendor/images/marker-shadow.png
 wagtail_maps/templates/wagtail_maps/map_block.html
 wagtail_maps/templates/wagtail_maps/popup_content.html
-wagtail_maps/templates/wagtail_maps/edit_handlers/center_calculate.html
-wagtail_maps/templates/wagtail_maps/edit_handlers/point_from_geo.html
 wagtail_maps/templates/wagtail_maps/icons/map-pin.svg
-wagtail_maps/templates/wagtail_maps/icons/map.svg
+wagtail_maps/templates/wagtail_maps/icons/map.svg
+wagtail_maps/templates/wagtail_maps/panels/map_center_coordinates.html
+wagtail_maps/templates/wagtail_maps/panels/point_coordinates.html
```

