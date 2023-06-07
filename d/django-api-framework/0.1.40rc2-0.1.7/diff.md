# Comparing `tmp/django-api-framework-0.1.40rc2.tar.gz` & `tmp/django-api-framework-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-framework-0.1.40rc2.tar", last modified: Tue Feb 28 03:13:18 2023, max compression
+gzip compressed data, was "django-api-framework-0.1.7.tar", last modified: Tue Oct  4 14:10:12 2022, max compression
```

## Comparing `django-api-framework-0.1.40rc2.tar` & `django-api-framework-0.1.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      192 2022-10-20 14:07:07.934412 django-api-framework-0.1.40rc2/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2022-10-04 15:29:52.313718 django-api-framework-0.1.40rc2/.coveragerc
--rw-r--r--   0        0        0      386 2022-10-13 19:34:07.197850 django-api-framework-0.1.40rc2/.editorconfig
--rw-r--r--   0        0        0      637 2022-10-01 14:16:51.740687 django-api-framework-0.1.40rc2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      564 2022-10-12 09:56:28.872755 django-api-framework-0.1.40rc2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1284 2023-02-27 05:28:56.001666 django-api-framework-0.1.40rc2/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     6387 2022-10-14 03:45:39.464496 django-api-framework-0.1.40rc2/.gitignore
--rw-r--r--   0        0        0       53 2022-10-01 03:44:33.733899 django-api-framework-0.1.40rc2/.isort.cfg
--rw-r--r--   0        0        0      907 2022-10-01 03:44:33.734110 django-api-framework-0.1.40rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      256 2022-10-01 03:44:33.734304 django-api-framework-0.1.40rc2/.pylintrc
--rw-r--r--   0        0        0       13 2022-10-01 03:44:33.734491 django-api-framework-0.1.40rc2/CONTRIBUTORS.txt
--rw-r--r--   0        0        0     1069 2022-09-30 15:01:22.719000 django-api-framework-0.1.40rc2/LICENSE
--rw-r--r--   0        0        0     1273 2023-02-27 06:41:08.702137 django-api-framework-0.1.40rc2/Makefile
--rw-r--r--   0        0        0     6247 2023-02-16 03:53:00.583693 django-api-framework-0.1.40rc2/README.md
--rw-r--r--   0        0        0      936 2022-10-01 03:44:33.735309 django-api-framework-0.1.40rc2/docs/Makefile
--rw-r--r--   0        0        0       81 2022-10-01 03:44:33.735529 django-api-framework-0.1.40rc2/docs/__init__.py
--rw-r--r--   0        0        0     2372 2022-10-01 03:44:33.735752 django-api-framework-0.1.40rc2/docs/conf.py
--rw-r--r--   0        0        0     1275 2022-10-01 03:44:33.735958 django-api-framework-0.1.40rc2/docs/howto.rst
--rw-r--r--   0        0        0   265995 2022-10-04 15:29:52.321872 django-api-framework-0.1.40rc2/docs/images/admin_apis_list.png
--rw-r--r--   0        0        0   296937 2022-10-13 17:37:35.202077 django-api-framework-0.1.40rc2/docs/images/auto_api_demo_2.png
--rw-r--r--   0        0        0   306860 2022-10-13 17:37:35.205842 django-api-framework-0.1.40rc2/docs/images/user_admin_api.png
--rw-r--r--   0        0        0      504 2022-10-01 03:44:33.736168 django-api-framework-0.1.40rc2/docs/index.rst
--rw-r--r--   0        0        0     1012 2022-10-01 03:44:34.127826 django-api-framework-0.1.40rc2/docs/make.bat
--rw-r--r--   0        0        0      177 2023-02-28 03:00:21.733309 django-api-framework-0.1.40rc2/easy/__init__.py
--rw-r--r--   0        0        0       65 2022-10-01 03:44:33.736801 django-api-framework-0.1.40rc2/easy/admin.py
--rw-r--r--   0        0        0      119 2022-10-01 03:44:33.736990 django-api-framework-0.1.40rc2/easy/apps.py
--rw-r--r--   0        0        0        0 2022-10-01 03:44:33.737192 django-api-framework-0.1.40rc2/easy/conf/__init__.py
--rw-r--r--   0        0        0      726 2022-10-20 13:12:47.932488 django-api-framework-0.1.40rc2/easy/conf/settings.py
--rw-r--r--   0        0        0        0 2022-10-01 03:44:33.737539 django-api-framework-0.1.40rc2/easy/controller/__init__.py
--rw-r--r--   0        0        0     2267 2022-10-20 14:07:07.917902 django-api-framework-0.1.40rc2/easy/controller/auto_api.py
--rw-r--r--   0        0        0     1482 2022-10-20 14:07:07.918085 django-api-framework-0.1.40rc2/easy/controller/base.py
--rw-r--r--   0        0        0     7311 2022-10-20 14:07:07.927754 django-api-framework-0.1.40rc2/easy/controller/meta.py
--rw-r--r--   0        0        0     5250 2022-10-17 04:28:48.268092 django-api-framework-0.1.40rc2/easy/controller/meta_conf.py
--rw-r--r--   0        0        0     2428 2022-10-14 21:27:39.464994 django-api-framework-0.1.40rc2/easy/decorators.py
--rw-r--r--   0        0        0      107 2022-10-20 13:12:47.921246 django-api-framework-0.1.40rc2/easy/domain/__init__.py
--rw-r--r--   0        0        0       88 2022-10-20 12:57:53.572689 django-api-framework-0.1.40rc2/easy/domain/base.py
--rw-r--r--   0        0        0      966 2022-10-20 14:07:07.918474 django-api-framework-0.1.40rc2/easy/domain/meta.py
--rw-r--r--   0        0        0     9509 2023-02-28 02:59:39.563746 django-api-framework-0.1.40rc2/easy/domain/orm.py
--rw-r--r--   0        0        0      564 2022-10-13 17:37:35.213418 django-api-framework-0.1.40rc2/easy/exception.py
--rw-r--r--   0        0        0     5479 2022-10-20 14:07:07.928095 django-api-framework-0.1.40rc2/easy/main.py
--rw-r--r--   0        0        0      415 2022-10-04 15:29:52.332695 django-api-framework-0.1.40rc2/easy/permissions/__init__.py
--rw-r--r--   0        0        0     1698 2022-10-17 04:28:48.271606 django-api-framework-0.1.40rc2/easy/permissions/adminsite.py
--rw-r--r--   0        0        0     1252 2022-10-13 17:37:35.215387 django-api-framework-0.1.40rc2/easy/permissions/base.py
--rw-r--r--   0        0        0      646 2022-10-04 15:29:52.334295 django-api-framework-0.1.40rc2/easy/permissions/superuser.py
--rw-r--r--   0        0        0        0 2022-10-01 03:44:33.740655 django-api-framework-0.1.40rc2/easy/renderer/__init__.py
--rw-r--r--   0        0        0      685 2022-10-04 15:29:52.335039 django-api-framework-0.1.40rc2/easy/renderer/json.py
--rw-r--r--   0        0        0     1174 2022-10-20 14:07:07.928309 django-api-framework-0.1.40rc2/easy/response.py
--rw-r--r--   0        0        0       57 2022-10-01 03:44:33.741306 django-api-framework-0.1.40rc2/easy/services/__init__.py
--rw-r--r--   0        0        0      407 2023-02-28 02:59:39.564244 django-api-framework-0.1.40rc2/easy/services/base.py
--rw-r--r--   0        0        0     1339 2023-02-28 02:59:39.564747 django-api-framework-0.1.40rc2/easy/services/crud.py
--rw-r--r--   0        0        0      780 2022-10-04 15:29:52.337178 django-api-framework-0.1.40rc2/easy/services/permission.py
--rw-r--r--   0        0        0       77 2022-10-04 15:29:52.338078 django-api-framework-0.1.40rc2/easy/testing/__init__.py
--rw-r--r--   0        0        0     2555 2022-10-16 03:59:43.878197 django-api-framework-0.1.40rc2/easy/testing/client.py
--rw-r--r--   0        0        0      323 2022-10-04 15:29:52.339168 django-api-framework-0.1.40rc2/easy/utils.py
--rwxr-xr-x   0        0        0     1030 2022-10-13 17:37:35.218971 django-api-framework-0.1.40rc2/manage.py
--rw-r--r--   0        0        0     2478 2023-02-27 05:46:18.238429 django-api-framework-0.1.40rc2/pyproject.toml
--rw-r--r--   0        0        0     2612 2022-11-08 14:38:16.374973 django-api-framework-0.1.40rc2/setup.cfg
--rw-r--r--   0        0        0        0 2022-10-01 03:44:33.743000 django-api-framework-0.1.40rc2/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-10-13 17:37:35.220761 django-api-framework-0.1.40rc2/tests/config/__init__.py
--rw-r--r--   0        0        0     2876 2022-10-20 13:12:47.933176 django-api-framework-0.1.40rc2/tests/config/settings.py
--rw-r--r--   0        0        0     1757 2022-10-17 04:28:48.273098 django-api-framework-0.1.40rc2/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-10-13 17:37:35.221518 django-api-framework-0.1.40rc2/tests/easy_app/__init__.py
--rw-r--r--   0        0        0      347 2022-10-13 17:37:35.221831 django-api-framework-0.1.40rc2/tests/easy_app/apis.py
--rw-r--r--   0        0        0       94 2022-10-13 17:37:35.222048 django-api-framework-0.1.40rc2/tests/easy_app/apps.py
--rw-r--r--   0        0        0      533 2022-10-13 17:37:35.222284 django-api-framework-0.1.40rc2/tests/easy_app/auth.py
--rw-r--r--   0        0        0     6289 2022-10-20 14:07:07.928520 django-api-framework-0.1.40rc2/tests/easy_app/controllers.py
--rw-r--r--   0        0        0      250 2022-10-14 20:44:47.686914 django-api-framework-0.1.40rc2/tests/easy_app/domain.py
--rw-r--r--   0        0        0      315 2023-02-16 04:08:02.794183 django-api-framework-0.1.40rc2/tests/easy_app/factories.py
--rw-r--r--   0        0        0     1461 2022-10-20 14:07:07.918877 django-api-framework-0.1.40rc2/tests/easy_app/models.py
--rw-r--r--   0        0        0      223 2022-10-13 17:37:35.223425 django-api-framework-0.1.40rc2/tests/easy_app/schema.py
--rw-r--r--   0        0        0     1491 2022-10-14 20:23:18.018775 django-api-framework-0.1.40rc2/tests/easy_app/services.py
--rw-r--r--   0        0        0      187 2022-10-14 21:27:39.471187 django-api-framework-0.1.40rc2/tests/easy_app/urls.py
--rw-r--r--   0        0        0     1784 2023-02-16 04:08:02.845615 django-api-framework-0.1.40rc2/tests/test_api_base_response.py
--rw-r--r--   0        0        0     8754 2022-10-18 13:16:09.613525 django-api-framework-0.1.40rc2/tests/test_async_api_permissions.py
--rw-r--r--   0        0        0    10556 2022-10-18 13:16:09.614832 django-api-framework-0.1.40rc2/tests/test_async_auto_crud_apis.py
--rw-r--r--   0        0        0     4324 2022-10-20 14:07:07.928871 django-api-framework-0.1.40rc2/tests/test_async_other_apis.py
--rw-r--r--   0        0        0     3045 2022-10-20 13:12:47.933481 django-api-framework-0.1.40rc2/tests/test_auto_api_creation.py
--rw-r--r--   0        0        0      674 2022-10-13 17:37:35.225467 django-api-framework-0.1.40rc2/tests/test_doc_decorator.py
--rw-r--r--   0        0        0     7940 2022-10-13 17:37:35.225729 django-api-framework-0.1.40rc2/tests/test_exceptions.py
--rw-r--r--   0        0        0      374 2022-10-20 13:12:47.933758 django-api-framework-0.1.40rc2/tests/test_settings.py
--rw-r--r--   0        0        0     9289 1970-01-01 00:00:00.000000 django-api-framework-0.1.40rc2/PKG-INFO
+-rw-r--r--   0        0        0      191 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.coveragerc
+-rw-r--r--   0        0        0    23482 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.dcignore
+-rw-r--r--   0        0        0      127 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.dockerignore
+-rw-r--r--   0        0        0      386 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.editorconfig
+-rw-r--r--   0        0        0       12 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.gitattributes
+-rw-r--r--   0        0        0      637 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      564 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1283 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     6373 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.gitignore
+-rw-r--r--   0        0        0       53 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.isort.cfg
+-rw-r--r--   0        0        0      907 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      256 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/.pylintrc
+-rw-r--r--   0        0        0       13 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/CONTRIBUTORS.txt
+-rw-r--r--   0        0        0     1069 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1265 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/Makefile
+-rw-r--r--   0        0        0     3149 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/README.md
+-rw-r--r--   0        0        0      936 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/docs/Makefile
+-rw-r--r--   0        0        0       81 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/docs/__init__.py
+-rw-r--r--   0        0        0     2372 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/docs/conf.py
+-rw-r--r--   0        0        0     1275 2022-10-04 14:09:31.945891 django-api-framework-0.1.7/docs/howto.rst
+-rw-r--r--   0        0        0   265995 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/docs/images/admin_apis_list.png
+-rw-r--r--   0        0        0   352364 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/docs/images/user_admin_api.png
+-rw-r--r--   0        0        0      504 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/docs/index.rst
+-rw-r--r--   0        0        0     1012 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/docs/make.bat
+-rw-r--r--   0        0        0      172 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/__init__.py
+-rw-r--r--   0        0        0       65 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/admin.py
+-rw-r--r--   0        0        0      119 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/apps.py
+-rw-r--r--   0        0        0        0 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/conf/__init__.py
+-rw-r--r--   0        0        0      744 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/conf/settings.py
+-rw-r--r--   0        0        0        0 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/controller/__init__.py
+-rw-r--r--   0        0        0     1160 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/controller/admin_auto_api.py
+-rw-r--r--   0        0        0      456 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/controller/base.py
+-rw-r--r--   0        0        0     6739 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/controller/meta.py
+-rw-r--r--   0        0        0     2430 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/decorators.py
+-rw-r--r--   0        0        0       55 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/domain/__init__.py
+-rw-r--r--   0        0        0       74 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/domain/base.py
+-rw-r--r--   0        0        0     3348 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/domain/orm.py
+-rw-r--r--   0        0        0     3321 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/domain/serializers.py
+-rw-r--r--   0        0        0      786 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/exception.py
+-rw-r--r--   0        0        0     5539 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/main.py
+-rw-r--r--   0        0        0      415 2022-10-04 14:09:31.949890 django-api-framework-0.1.7/easy/permissions/__init__.py
+-rw-r--r--   0        0        0     3179 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/permissions/adminsite.py
+-rw-r--r--   0        0        0     1179 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/permissions/base.py
+-rw-r--r--   0        0        0      646 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/permissions/superuser.py
+-rw-r--r--   0        0        0        0 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/renderer/__init__.py
+-rw-r--r--   0        0        0      685 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/renderer/json.py
+-rw-r--r--   0        0        0     1192 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/response.py
+-rw-r--r--   0        0        0       57 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/services/__init__.py
+-rw-r--r--   0        0        0      592 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/services/base.py
+-rw-r--r--   0        0        0     1307 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/services/crud.py
+-rw-r--r--   0        0        0      780 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/services/permission.py
+-rw-r--r--   0        0        0       77 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/testing/__init__.py
+-rw-r--r--   0        0        0     1291 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/testing/client.py
+-rw-r--r--   0        0        0      323 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/easy/utils.py
+-rw-r--r--   0        0        0     2307 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       62 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/pytest.ini
+-rw-r--r--   0        0        0     2611 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/setup.cfg
+-rw-r--r--   0        0        0        0 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     2241 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/__init__.py
+-rw-r--r--   0        0        0      374 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/apis.py
+-rw-r--r--   0        0        0       94 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/apps.py
+-rw-r--r--   0        0        0      533 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/auth.py
+-rw-r--r--   0        0        0     1123 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/conftest.py
+-rw-r--r--   0        0        0     3755 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/controllers.py
+-rw-r--r--   0        0        0       77 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/domain.py
+-rw-r--r--   0        0        0      316 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/factories.py
+-rw-r--r--   0        0        0     1012 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/models.py
+-rw-r--r--   0        0        0      223 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/schema.py
+-rw-r--r--   0        0        0     1511 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/services.py
+-rw-r--r--   0        0        0     1781 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_api_base_response.py
+-rw-r--r--   0        0        0     7847 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_async_api_permissions.py
+-rw-r--r--   0        0        0     7881 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_async_auto_crud_apis.py
+-rw-r--r--   0        0        0     3602 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_async_other_apis.py
+-rw-r--r--   0        0        0     1494 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_auto_api_creation.py
+-rw-r--r--   0        0        0      674 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_doc_decorator.py
+-rw-r--r--   0        0        0     6917 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_exceptions.py
+-rw-r--r--   0        0        0      392 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/test_settings.py
+-rw-r--r--   0        0        0      473 2022-10-04 14:09:31.953890 django-api-framework-0.1.7/tests/demo_app/urls.py
+-rw-r--r--   0        0        0     6136 1970-01-01 00:00:00.000000 django-api-framework-0.1.7/PKG-INFO
```

### Comparing `django-api-framework-0.1.40rc2/.github/workflows/publish.yml` & `django-api-framework-0.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/.github/workflows/test.yml` & `django-api-framework-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/.github/workflows/test_full.yml` & `django-api-framework-0.1.7/.github/workflows/test_full.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10']
         django-version: ['>3.1', '<3.2', '<3.3', '<4.1']
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `django-api-framework-0.1.40rc2/.gitignore` & `django-api-framework-0.1.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -385,8 +385,7 @@
 /.idea/inspectionProfiles/Project_Default.xml
 /.idea/.gitignore
 /.idea/django-easy-api.iml
 /.idea/misc.xml
 /.idea/modules.xml
 /.idea/vcs.xml
 /.idea/django-api-framework.iml
-/.idea/shelf/
```

### Comparing `django-api-framework-0.1.40rc2/.pre-commit-config.yaml` & `django-api-framework-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/LICENSE` & `django-api-framework-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/Makefile` & `django-api-framework-0.1.7/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .PHONY: help docs
 .DEFAULT_GOAL := help
 
 help:
 	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 clean: ## Removing cached python compiled files
-	find . -name \*pyc  | xargs  rm -rfv
+	find . -name \*pyc  | xargs  rm -fv
 	find . -name \*pyo | xargs  rm -fv
 	find . -name \*~  | xargs  rm -fv
 	find . -name __pycache__  | xargs  rm -rfv
 
 install: ## Install dependencies
 	make clean
 	flit install --deps develop --symlink
@@ -24,15 +24,15 @@
 
 fmt format: ## Run code formatters
 	autoflake --in-place --remove-all-unused-imports --remove-unused-variables --ignore-init-module-imports  -r easy tests
 	isort easy tests
 	black easy tests
 
 test: ## Run tests
-	pytest -s -vv
+	pytest
 
 test-cov: ## Run tests with coverage
 	pytest --cov=easy --cov-report term
 
 test-cov-full: ## Run tests with coverage term-missing
 	pytest --cov=easy --cov-report term-missing tests
```

### Comparing `django-api-framework-0.1.40rc2/docs/Makefile` & `django-api-framework-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/docs/conf.py` & `django-api-framework-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/docs/howto.rst` & `django-api-framework-0.1.7/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/docs/images/admin_apis_list.png` & `django-api-framework-0.1.7/docs/images/admin_apis_list.png`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/docs/make.bat` & `django-api-framework-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/easy/controller/auto_api.py` & `django-api-framework-0.1.7/easy/controller/admin_auto_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,47 @@
 import logging
-from typing import Optional, Type, Union
+from typing import Type, Union
 
 from django.db import models
 from ninja_extra import ControllerBase, api_controller
-from ninja_extra.permissions import BasePermission
 
 from easy.controller.base import CrudAPIController
-from easy.controller.meta_conf import (
-    GENERATE_CRUD_ATTR,
-    MODEL_EXCLUDE_ATTR,
-    MODEL_FIELDS_ATTR,
-    MODEL_JOIN_ATTR,
-    MODEL_RECURSIVE_ATTR,
-    SENSITIVE_FIELDS_ATTR,
-    ModelOptions,
-)
-from easy.permissions import AdminSitePermission, BaseApiPermission
+from easy.permissions import AdminSitePermission
 
 logger = logging.getLogger(__name__)
 
 
-def create_api_controller(
-    model: models.Model,
-    app_name: str,
-    permission_class: Type[BasePermission] = BaseApiPermission,
-    controller_name_prefix: Optional[str] = None,
-) -> Union[Type[ControllerBase], Type]:
-    """Create APIController class dynamically, with specified permission class"""
-    model_name = model.__name__  # type:ignore
+class AdminClass(object):
+    auto_import = True
 
-    model_opts: ModelOptions = ModelOptions.get_model_options(
-        getattr(model, "APIMeta", None)
-    )
 
-    APIMeta = type(
-        "APIMeta",
+def create_admin_controller(
+    model: models.Model, app_name: str
+) -> Union[Type[ControllerBase], Type]:
+    """Create AdminAPI class dynamically, permission class set to AdminSitePermission"""
+    model_name = model.__name__  # type:ignore
+    Meta = type(
+        "Meta",
         (object,),
-        {
-            "model": model,
-            GENERATE_CRUD_ATTR: model_opts.generate_crud,
-            MODEL_EXCLUDE_ATTR: model_opts.model_exclude,
-            MODEL_FIELDS_ATTR: model_opts.model_fields,
-            MODEL_RECURSIVE_ATTR: model_opts.model_recursive,
-            MODEL_JOIN_ATTR: model_opts.model_join,
-            SENSITIVE_FIELDS_ATTR: model_opts.model_fields,
-        },
+        {"model": model, "fields": "__all__"},
     )
 
-    class_name = f"{model_name}{controller_name_prefix}APIController"
+    class_name = f"{model_name}AdminAPIController"
 
     auto_cls = type.__new__(
         type,
         class_name,
-        (CrudAPIController,),
+        (
+            CrudAPIController,
+            AdminClass,
+        ),
         {
-            "APIMeta": APIMeta,
+            "Meta": Meta,
         },
     )
 
+    logger.debug(f"Creating Admin API for f{model.__dict__.items()}")
     return api_controller(
         f"/{app_name}/{model_name.lower()}",
-        tags=[f"{model_name} {controller_name_prefix}API"],
-        permissions=[permission_class],
+        tags=[f"{model_name} AdminAPI"],
+        permissions=[AdminSitePermission],
     )(auto_cls)
-
-
-def create_admin_controller(
-    model: models.Model, app_name: str
-) -> Union[Type[ControllerBase], Type]:
-    """Create AdminAPI class dynamically, permission class set to AdminSitePermission"""
-    return create_api_controller(
-        model=model,
-        app_name=app_name,
-        permission_class=AdminSitePermission,
-        controller_name_prefix="Admin",
-    )
```

### Comparing `django-api-framework-0.1.40rc2/easy/controller/meta.py` & `django-api-framework-0.1.7/easy/controller/meta.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,192 +1,192 @@
 import json
 import logging
-import re
 import uuid
-from abc import ABC, ABCMeta
-from collections import ChainMap
-from typing import Any, List, Match, Optional, Tuple, Type
+from abc import ABCMeta
+from typing import Any, Optional, Tuple, Type, Union
 
+from django.db import models
 from django.http import HttpRequest
 from ninja import ModelSchema
 from ninja_extra import ControllerBase, http_delete, http_get, http_patch, http_put
-from ninja_extra.exceptions import ValidationError
 from ninja_extra.pagination import paginate
 
-from easy.controller.meta_conf import MODEL_FIELDS_ATTR_DEFAULT, ModelOptions
-from easy.domain.meta import CrudModel
-from easy.response import BaseAPIResponse
+from easy.domain.orm import CrudModel
 from easy.services import BaseService
 from easy.utils import copy_func
 
 logger = logging.getLogger(__name__)
 
 
-class CrudAPI(CrudModel, ABC):
+class CrudAPI(CrudModel):
     # Never add type note to service, it will cause injection error
     def __init__(self, service=None):  # type: ignore
-        # Critical to set __Meta
-        self.service = service
-
-        _model_opts: ModelOptions = ModelOptions.get_model_options(self.APIMeta)
-        if self.model and _model_opts:
-            ModelOptions.set_model_meta(self.model, _model_opts)
-
         if not service:
             self.service = BaseService(model=self.model)
+        else:
+            self.service = service
         super().__init__(model=self.model)
 
+    # Define Controller APIs for auto generation
+    async def get_obj(self, request: HttpRequest, id: int) -> Any:
+        """
+        GET /{id}
+        Retrieve a single Object
+        """
+        return await self.service.get_obj(id)
+
+    async def del_obj(self, request: HttpRequest, id: int) -> Any:
+        """
+        DELETE /objects/{id}
+        Delete a single Object
+        """
+        return await self.service.del_obj(id)
+
+    @paginate
+    async def get_objs(
+        self, request: HttpRequest, maximum: int = None, filters: str = None
+    ) -> Any:
+        """
+        GET /get_all
+        Retrieve multiple Object
+        """
+        if filters:
+            return await self.service.get_objs(maximum, **json.loads(filters))
+        return await self.service.get_objs(maximum)
+
+    @paginate
+    async def filter_objs(
+        self, request: HttpRequest, filters: Union[str, bytes]
+    ) -> Any:
+        """
+        GET /filter/?filters={filters_dict}
+        Filter Objects
+        """
+        return await self.service.filter_objs(**json.loads(filters))
+
+    @paginate
+    async def filter_exclude_objs(self, filters: Union[str, bytes]) -> Any:
+        """
+        GET /filter_exclude/?filters={filters_dict}
+        Filter exclude Objects
+        """
+        return await self.service.filter_exclude_objs(**json.loads(filters))
+
+    # async def bulk_create_objs(self, request):
+    #     """
+    #     POST /bulk_create
+    #     Create multiple Object
+    #     """
+    #     return await self.service.bulk_create_objs()
+    #
+    # async def recover_obj(self, request):
+    #     """
+    #     PATCH /{id}/recover
+    #     Recover one Object
+    #     """
+    #     return await self.service.recover_obj()
+
 
-class CrudAPIMetaclass(ABCMeta):
+class CrudApiMetaclass(ABCMeta):
     def __new__(mcs, name: str, bases: Tuple[Type[Any], ...], attrs: dict) -> Any:
-        # Get configs from APIMeta
-        attrs_meta = attrs.get("APIMeta", None)
-        model_opts: ModelOptions = ModelOptions.get_model_options(attrs_meta)
-
-        # Get all attrs from parents excluding private ones
-        def is_private_attrs(attr_name: str) -> Optional[Match[str]]:
-            return re.match(r"^__[^\d\W]\w*\Z__$", attr_name, re.UNICODE)
-
-        parent_attrs = ChainMap(
-            *[attrs]
-            + [
-                {k: v for (k, v) in vars(base).items() if not (is_private_attrs(k))}
-                for base in bases
-            ]
+        # Get configs from Meta
+        temp_base: Type = type.__new__(type, "object", (), {})
+        temp_cls: Type = super(CrudApiMetaclass, mcs).__new__(
+            mcs, name, (temp_base,), attrs
         )
-        base_cls_attrs: dict = {}
-        base_cls_attrs.update(parent_attrs)
-
-        # Define Controller APIs for auto generation
-        async def get_obj(self, request: HttpRequest, id: int) -> Any:  # type: ignore
-            """
-            GET /{id}
-            Retrieve a single Object
-            """
-            try:
-                qs = await self.service.get_obj(id)
-            except Exception as e:  # pragma: no cover
-                logger.error(f"Get Error - {e}", exc_info=True)
-                return BaseAPIResponse(str(e), message="Get Failed", code=500)
-            if qs:
-                return qs
-            else:
-                return BaseAPIResponse(message="Not Found", code=404)
-
-        async def del_obj(self, request: HttpRequest, id: int) -> Any:  # type: ignore
-            """
-            DELETE /{id}
-            Delete a single Object
-            """
-            if await self.service.del_obj(id):
-                return BaseAPIResponse("Deleted.", code=204)
-            else:
-                return BaseAPIResponse("Not Found.", code=404)
-
-        @paginate
-        async def get_objs(self, request: HttpRequest, filters: Optional[str] = None) -> Any:  # type: ignore
-            """
-            GET /?filters={filters_dict}
-            Retrieve multiple Object (optional: django filters)
-            """
-            if filters:
-                try:
-                    _filters = json.loads(filters)
-                except Exception as exc:  # pragma: no cover
-                    raise ValidationError(
-                        detail=f"Bad filter, please check carefully. {exc}",
-                        code=402,
-                    )
-                return await self.service.get_objs(**_filters)
-            return await self.service.get_objs()
+        temp_opts: ModelOptions = ModelOptions(getattr(temp_cls, "Meta", None))
+        opts_fields_exclude: Optional[Union[str]] = temp_opts.exclude
+        opts_fields: Optional[Union[str]] = temp_opts.fields
+        opts_model: Optional[Type[models.Model]] = temp_opts.model
+        opts_recursive: Optional[Union[bool]] = temp_opts.recursive
+
+        base_cls_attrs = {
+            "get_obj": http_get("/", summary="Get")(
+                copy_func(CrudAPI.get_obj)  # type: ignore
+            ),
+            "del_obj": http_delete("/", summary="Delete")(
+                copy_func(CrudAPI.del_obj)  # type: ignore
+            ),
+            "get_all": http_get("/get_all", summary="Get All")(
+                copy_func(CrudAPI.get_objs)  # type: ignore
+            ),
+            "filter_objs": http_get("/filter", summary="Filter")(
+                copy_func(CrudAPI.filter_objs)  # type: ignore
+            ),
+            "filter_exclude_objs": http_get(
+                "/filter_exclude", summary="Filter exclude"
+            )(
+                copy_func(CrudAPI.filter_exclude_objs)  # type: ignore
+            ),
+        }
 
-        if model_opts.generate_crud and model_opts.model:
-            base_cls_attrs.update(
-                {
-                    "get_obj": http_get("/{id}", summary="Get a single object")(
-                        copy_func(get_obj)  # type: ignore
-                    ),
-                    "del_obj": http_delete("/{id}", summary="Delete a single object")(
-                        copy_func(del_obj)  # type: ignore
-                    ),
-                    "get_objs": http_get("/", summary="Get multiple objects")(
-                        copy_func(get_objs)  # type: ignore
-                    ),
-                }
-            )
+        if opts_model:
 
             class DataSchema(ModelSchema):
                 class Config:
-                    model = model_opts.model
-                    model_exclude: List = []
-                    if model_opts.model_exclude:
-                        model_exclude.extend(model_opts.model_exclude)
-                        # Remove pk(id) from Create/Update Schema
-                        model_exclude.extend([model._meta.pk.name])  # type: ignore
+                    model = opts_model
+                    if opts_fields_exclude:
+                        model_exclude = opts_fields_exclude
                     else:
-                        if model_opts.model_fields == MODEL_FIELDS_ATTR_DEFAULT:
-                            # Remove pk(id) from Create/Update Schema
-                            model_exclude.extend([model._meta.pk.name])  # type: ignore
+                        if opts_fields == ["__all__"]:
+                            model_fields = "__all__"
                         else:
-                            model_fields = (
-                                model_opts.model_fields
-                                if model_opts.model_fields
-                                else MODEL_FIELDS_ATTR_DEFAULT
-                            )
+                            model_fields = opts_fields if opts_fields else "__all__"
+                    recursive = temp_opts.recursive
 
             async def add_obj(  # type: ignore
                 self, request: HttpRequest, data: DataSchema
             ) -> Any:
                 """
                 PUT /
                 Create a single Object
                 """
-                obj_id = await self.service.add_obj(**data.dict())
-                if obj_id:
-                    return BaseAPIResponse({"id": obj_id}, code=201, message="Created.")
-                else:
-                    return BaseAPIResponse(
-                        code=204, message="Add failed."
-                    )  # pragma: no cover
+                return await self.service.add_obj(**data.dict())
 
             async def patch_obj(  # type: ignore
                 self, request: HttpRequest, id: int, data: DataSchema
             ) -> Any:
                 """
-                PATCH /{id}
-                Update a single object
+                PATCH /?id={id}
+                Update a single field for a Object
                 """
-                if await self.service.patch_obj(id=id, payload=data.dict()):
-                    return BaseAPIResponse(message="Updated.")
-                else:
-                    return BaseAPIResponse(code=400, message="Updated Failed")
+                return await self.service.patch_obj(id=id, payload=data.dict())
 
             DataSchema.__name__ = (
-                f"{model_opts.model.__name__}__AutoSchema({str(uuid.uuid4())[:4]})"
+                f"{opts_model.__name__}__AutoSchema({str(uuid.uuid4())[:4]})"
             )
 
+            setattr(CrudAPI, "add_obj", classmethod(add_obj))
+            setattr(CrudAPI, "patch_obj", classmethod(patch_obj))
             base_cls_attrs.update(
                 {
-                    "patch_obj": http_patch("/{id}", summary="Patch a single object")(
-                        copy_func(patch_obj)  # type: ignore
+                    "patch_obj": http_patch("/", summary="Patch/Update")(
+                        copy_func(CrudAPI.patch_obj)  # type: ignore
                     ),
                     "add_obj": http_put("/", summary="Create")(
-                        copy_func(add_obj)  # type: ignore
+                        copy_func(CrudAPI.add_obj)  # type: ignore
                     ),
                 }
             )
 
-        new_cls: Type = super().__new__(
-            mcs,
-            name,
-            (
-                ControllerBase,
-                CrudAPI,
-            ),
-            base_cls_attrs,
+        new_base: Type = type.__new__(
+            type, name, (ControllerBase, CrudAPI), base_cls_attrs
+        )
+        new_cls: Type = super(CrudApiMetaclass, mcs).__new__(
+            mcs, name, (new_base,), attrs
         )
 
-        if model_opts.model:
-            ModelOptions.set_model_meta(model_opts.model, model_opts)
-            setattr(new_cls, "model", model_opts.model)
+        new_cls.model = opts_model
+        new_cls.fields_exclude = opts_fields_exclude
+        new_cls.fields = opts_fields
+        new_cls.recursive = opts_recursive
 
         return new_cls
+
+
+class ModelOptions:
+    def __init__(self, options: object = None):
+        self.model: Optional[Type[models.Model]] = getattr(options, "model", None)
+        self.service: Optional[Any] = getattr(options, "service", None)
+        self.fields: Optional[Union[str]] = getattr(options, "fields", None)
+        self.exclude: Optional[Union[str]] = getattr(options, "exclude", None)
+        self.recursive: Optional[Union[bool]] = getattr(options, "recursive", False)
```

### Comparing `django-api-framework-0.1.40rc2/easy/decorators.py` & `django-api-framework-0.1.7/easy/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,14 @@
     login_url: str = "admin:login",
 ) -> Any:
     """
     Decorator for views that checks that the user is logged in and is a staff
     member, redirecting to the login page if necessary.
     """
     actual_decorator = request_passes_test(
-        lambda r: (r.user.is_active and r.user.is_staff),
+        lambda r: ((r.user.is_active and r.user.is_staff)),
         login_url=login_url,
         redirect_field_name=redirect_field_name,
     )
     if view_func:
         return actual_decorator(view_func)
     return actual_decorator  # pragma: no cover
```

### Comparing `django-api-framework-0.1.40rc2/easy/main.py` & `django-api-framework-0.1.7/easy/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 from django.utils.module_loading import module_has_submodule
 from ninja.constants import NOT_SET, NOT_SET_TYPE
 from ninja.parser import Parser
 from ninja.renderers import BaseRenderer
 from ninja.types import TCallable
 from ninja_extra import NinjaExtraAPI
 
-from easy.controller.auto_api import create_admin_controller
-from easy.domain.orm import django_serializer
+from easy.controller.admin_auto_api import create_admin_controller
+from easy.domain import serializers
 from easy.renderer.json import EasyJSONRenderer
-from easy.response import BaseAPIResponse
+from easy.response import BaseApiResponse
 
 logger = logging.getLogger(__name__)
 
 
 class EasyAPI(NinjaExtraAPI):
     """
     EasyAPI, extensions:
     -Add 2 init params
         Easy_extra: bool = True,
             Can serialize queryset or model, and support pagination
         Easy_output: bool = True,
             If True, will be encapsulated in BaseAPIResponse
     -renderer, default to EasyJSONRenderer
+    -API docs default to docs_permission_required，only logged in Staff users can visit
     -Auto generate AdminAPIs, it will read the following settings:
-        CRUD_API_ENABLED_ALL_APPS
-        CRUD_API_EXCLUDE_APPS
-        CRUD_API_INCLUDE_APPS
+        AUTO_ADMIN_ENABLED_ALL_APPS
+        AUTO_ADMIN_EXCLUDE_APPS
+        AUTO_ADMIN_INCLUDE_APPS
     """
 
     def __init__(
         self,
         *,
         title: str = "Easy API",
         version: str = "1.0.0",
@@ -71,25 +72,25 @@
         self.app_name = app_name
         self.easy_extra = easy_extra
         self.easy_output = easy_output
 
     def auto_create_admin_controllers(self, version: str = None) -> None:
         for app_module in self.get_installed_apps():
             # If not all
-            if not settings.CRUD_API_ENABLED_ALL_APPS:  # type:ignore
+            if not settings.AUTO_ADMIN_ENABLED_ALL_APPS:  # type:ignore
                 # Only generate for this included apps
-                if settings.CRUD_API_INCLUDE_APPS is not None:  # type:ignore
+                if settings.AUTO_ADMIN_INCLUDE_APPS is not None:  # type:ignore
                     if (
                         app_module.name
-                        not in settings.CRUD_API_INCLUDE_APPS  # type:ignore
+                        not in settings.AUTO_ADMIN_INCLUDE_APPS  # type:ignore
                     ):
                         continue
 
             # Exclude list
-            if app_module.name in settings.CRUD_API_EXCLUDE_APPS:  # type:ignore
+            if app_module.name in settings.AUTO_ADMIN_EXCLUDE_APPS:  # type:ignore
                 continue
 
             try:
                 app_module_ = import_module(app_module.name)
                 final = []
                 if module_has_submodule(app_module_, "models"):
                     # Auto generate AdminAPI
@@ -109,51 +110,45 @@
 
         return [
             v
             for k, v in apps.app_configs.items()
             if not v.name.startswith("django.") and (not v.name == "easy.api")
         ]
 
+    def process_data(self, data: Any) -> Any:
+        data_to_render = data
+        if self.easy_extra:
+            # TODO: need to protect sensitive fields
+            # Queryset
+            if serializers.is_queryset(data):
+                data_to_render = serializers.serialize_queryset(data)
+            # Model
+            elif serializers.is_model_instance(data):
+                data_to_render = serializers.serialize_model_instance(data)
+            # Add limit_off pagination support
+            elif serializers.is_paginated(data):
+                data_to_render = serializers.serialize_queryset(data.get("items"))
+
+        if self.easy_output:
+            if not serializers.is_base_response(data_to_render):
+                data_to_render = serializers.serialize_base_response(data_to_render)
+
+        return data_to_render
+
     def create_response(
         self,
         request: HttpRequest,
         data: Any,
         *,
         status: int = None,
         temporal_response: HttpResponse = None,
     ) -> HttpResponse:
-        if self.easy_extra:
-            try:
-                data = django_serializer.serialize_data(data)
-            except Exception as e:  # pragma: no cover
-                logger.error(f"Creat Response Error - {e}", exc_info=True)
-                return BaseAPIResponse(str(e), code=500)
+        data_to_render = self.process_data(data)
 
-        if self.easy_output:
-            if temporal_response:
-                status = temporal_response.status_code
-            assert status
-
-            _temp = BaseAPIResponse(
-                data, status=status, content_type=self.get_content_type()
-            )
-
-            if temporal_response:
-                response = temporal_response
-                response.content = _temp.content
-            else:
-                response = _temp
-
-        else:
-            response = super().create_response(
-                request,
-                data,
-                status=status,
-                temporal_response=temporal_response,
-            )
-        return response
-
-    def create_temporal_response(self, request: HttpRequest) -> HttpResponse:
-        if self.easy_output:
-            return BaseAPIResponse("", content_type=self.get_content_type())
-        else:
-            return super().create_temporal_response(request)
+        if isinstance(data_to_render, BaseApiResponse):
+            return data_to_render
+        return super(EasyAPI, self).create_response(
+            request=request,
+            data=data_to_render,
+            status=status,
+            temporal_response=temporal_response,
+        )  # pragma: no cover
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-api-framework-0.1.40rc2/easy/permissions/base.py` & `django-api-framework-0.1.7/easy/permissions/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 if TYPE_CHECKING:
     from ninja_extra.controllers.base import ControllerBase  # pragma: no cover
 
 
 class BaseApiPermission(permissions.BasePermission):
     """
-    Base permission class that all Permission Class should inherit from.
-    This will call service.check_permission for extra check.
+    Base permission class, only active user will have access
     """
 
     def has_permission(
         self, request: HttpRequest, controller: "ControllerBase"
     ) -> bool:
         """
         Return `True` if permission is granted, `False` otherwise.
```

### Comparing `django-api-framework-0.1.40rc2/easy/permissions/superuser.py` & `django-api-framework-0.1.7/easy/permissions/superuser.py`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/easy/renderer/json.py` & `django-api-framework-0.1.7/easy/renderer/json.py`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/easy/response.py` & `django-api-framework-0.1.7/easy/response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import json
-from typing import Any, Dict, List, Union
+from typing import Any, Type, Union
 
-from django.db.models import QuerySet
 from django.http.response import JsonResponse
 
 from easy.renderer.json import EasyJSONEncoder
 
-CODE_SUCCESS = 0
+ERRNO_SUCCESS = 0
 SUCCESS_MESSAGE = "success"
+UNKNOWN_ERROR_MSG = "system error"
 
 
-class BaseAPIResponse(JsonResponse):
+class BaseApiResponse(JsonResponse):
     """
     Base for all API responses
     """
 
     def __init__(
         self,
-        data: Union[Dict, str, bool, List[Any], QuerySet] = None,
-        code: int = None,
+        data: Union[dict, str] = None,
+        errno: int = None,
         message: str = None,
         **kwargs: Any
     ):
-        if code:
-            message = message or str(code)
+        if errno:
+            message = message or UNKNOWN_ERROR_MSG
         else:
-            message = message or SUCCESS_MESSAGE
-            code = CODE_SUCCESS
+            message = SUCCESS_MESSAGE
+            errno = ERRNO_SUCCESS
 
-        _data: Union[Dict, str] = {
-            "code": code,
+        _data: Union[dict, str] = {
+            "code": errno,
             "message": message,
             "data": data if data is not None else {},
         }
-
-        super().__init__(data=_data, encoder=EasyJSONEncoder, **kwargs)
+        _encoder: Type[json.JSONEncoder] = EasyJSONEncoder
+        super().__init__(data=_data, encoder=_encoder, **kwargs)
 
     @property
     def json_data(self) -> Any:
         """
         Get json data
         """
         return json.loads(self.content)
 
-    def update_content(self, data: Dict) -> None:
+    def update_content(self, data: dict) -> None:
         """
         Update content with new data
         """
         self.content = json.dumps(data)
```

### Comparing `django-api-framework-0.1.40rc2/easy/services/crud.py` & `django-api-framework-0.1.7/easy/services/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
-from typing import Any, Optional, Type
+from typing import Any
 
 from asgiref.sync import sync_to_async
 from django.db import models
 
-from easy.domain.orm import DjangoOrmModel
+from easy.domain.orm import CrudModel
 
 logger = logging.getLogger(__name__)
 
 
-class CrudService(DjangoOrmModel):
-    def __init__(self, model: Optional[Type[models.Model]] = None):
+class CrudService(CrudModel):
+    def __init__(self, model: models.Model):
         super().__init__(model)
         self.model = model
 
     async def get_obj(self, id: int) -> Any:
-        return await sync_to_async(self.crud_get_obj)(id)
+        return await sync_to_async(self._crud_get_obj)(id)
 
-    async def get_objs(self, **filters: Any) -> Any:
-        return await sync_to_async(self.crud_get_objs_all)(**filters)
+    async def get_objs(self, maximum: int = None, **filters: Any) -> Any:
+        return await sync_to_async(self._crud_get_objs_all)(maximum, **filters)
 
     async def patch_obj(self, id: int, payload: Any) -> Any:
-        return await sync_to_async(self.crud_update_obj)(id, payload)
+        return await sync_to_async(self._crud_update_obj)(id, payload)
 
     async def del_obj(self, id: int) -> Any:
-        return await sync_to_async(self.crud_del_obj)(id)
+        return await sync_to_async(self._crud_del_obj)(id)
 
     async def add_obj(self, **payload: Any) -> Any:
-        return await sync_to_async(self.crud_add_obj)(**payload)
+        return await sync_to_async(self._crud_add_obj)(**payload)
 
     async def filter_objs(self, **payload: Any) -> Any:
-        return await sync_to_async(self.crud_filter)(**payload)  # pragma: no cover
+        return await sync_to_async(self._crud_filter)(**payload)
 
     async def filter_exclude_objs(self, **payload: Any) -> Any:
-        return await sync_to_async(self.crud_filter_exclude)(**payload)
+        return await sync_to_async(self._crud_filter_exclude)(**payload)
 
     # async def bulk_create_objs(self):
     #     ...
     #
     # async def recover_obj(self):
     #     ...
```

### Comparing `django-api-framework-0.1.40rc2/easy/services/permission.py` & `django-api-framework-0.1.7/easy/services/permission.py`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/pyproject.toml` & `django-api-framework-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,28 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Framework :: Django",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 requires = [
     "Django >= 3.1",
-    "django-ninja-extra >= 0.16.0",
+    "django-ninja-extra >= 0.15.0",
 ]
 description-file = "README.md"
 requires-python = ">=3.6"
 
 
 [tool.flit.metadata.urls]
 Documentation = "https://github.com/freemindcore/django-api-framework"
@@ -60,15 +59,15 @@
     "isort",
     "injector == 0.19.0",
     "flake8",
     "mypy==0.931",
     "django-stubs",
     "factory-boy==3.2.1",
     "django_coverage_plugin",
-    "django-ninja-extra >= 0.16.0",
+    "django-ninja-extra >= 0.15.0",
     "django-ninja-jwt",
     "Django >= 3.1",
 ]
 dev = [
     "autoflake",
     "pre_commit",
     "bumpversion==0.6.0",
@@ -76,12 +75,7 @@
 doc = [
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=7.1.9,<8.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
     "markdown-include"
 ]
-
-[tool.pytest.ini_options]
-DJANGO_SETTINGS_MODULE = "tests.config.settings"
-asyncio_mode = "auto"
-addopts = "--nomigrations"
```

### Comparing `django-api-framework-0.1.40rc2/setup.cfg` & `django-api-framework-0.1.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 max-complexity = 10
 
 [pycodestyle]
 max-line-length = 88
 exclude = .tox,.git,*/migrations/*,*/static/CACHE/*,docs,node_modules,venv
 
 [mypy]
-python_version = 3.11
+python_version = 3.8
 ignore_missing_imports = True
 warn_unused_configs = True
 plugins = mypy_django_plugin.main
 
 show_column_numbers = True
 
 follow_imports = normal
@@ -80,15 +80,15 @@
 warn_unused_ignores = True
 
 disallow_untyped_defs = True
 check_untyped_defs = True
 no_implicit_reexport = True
 
 [mypy.plugins.django-stubs]
-django_settings_module = "tests.easy_app"
+django_settings_module = "tests.demo_app"
 
 [mypy-*.migrations.*]
 # Django migrations should not produce any errors:
 ignore_errors = True
 
 [mypy-tests.*]
 ignore_errors = True
```

### Comparing `django-api-framework-0.1.40rc2/tests/conftest.py` & `django-api-framework-0.1.7/tests/demo_app/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import copy
-from typing import Callable, Type, Union
 
 import pytest
 from django.contrib.auth import get_user_model
-from ninja_extra import ControllerBase, Router
 
-from easy import EasyAPI
+from easy.controller.base import CrudAPIController
 from easy.testing import EasyTestClient
-
-from .easy_app.auth import JWTAuthAsync, jwt_auth_async
-from .easy_app.factories import UserFactory
+from tests.demo_app.auth import JWTAuthAsync, jwt_auth_async
+from tests.demo_app.factories import UserFactory
 
 User = get_user_model()
 
 
 @pytest.fixture(autouse=True)
 def media_storage(settings, tmpdir):
     settings.MEDIA_ROOT = tmpdir.strpath
@@ -21,45 +18,28 @@
 
 @pytest.fixture
 def user(db) -> User:
     return UserFactory()
 
 
 @pytest.fixture
-def easy_api_client(user) -> Callable:
+def easy_api_client(user) -> EasyTestClient:
     orig_func = copy.deepcopy(JWTAuthAsync.__call__)
 
+    async def mock_func(self, request):
+        setattr(request, "user", user)
+        return True
+
+    setattr(JWTAuthAsync, "__call__", mock_func)
+
     def create_client(
-        api: Union[EasyAPI, Router, Type[ControllerBase]],
-        api_user=None,  # type: ignore
+        api: CrudAPIController,
         is_staff: bool = False,
         is_superuser: bool = False,
-        has_perm: bool = False,
-    ) -> "EasyTestClient":
-        if api_user is None:
-            api_user = user
-        setattr(api_user, "is_staff", is_staff)
-        setattr(api_user, "is_superuser", is_superuser)
-
-        def mock_has_perm_true(*args, **kwargs):
-            return True
-
-        def mock_has_perm_false(*args, **kwargs):
-            return False
-
-        async def mock_func(self, request):
-            setattr(request, "user", api_user)
-            return True
-
-        setattr(JWTAuthAsync, "__call__", mock_func)
-
-        if is_superuser:
-            setattr(api_user, "is_staff", True)
-        if has_perm:
-            setattr(api_user, "has_perm", mock_has_perm_true)
-        else:
-            setattr(api_user, "has_perm", mock_has_perm_false)
+    ):
+        setattr(user, "is_staff", is_staff)
+        setattr(user, "is_superuser", is_superuser)
         client = EasyTestClient(api, auth=jwt_auth_async)
         return client
 
     yield create_client
     setattr(JWTAuthAsync, "__call__", orig_func)
```

### Comparing `django-api-framework-0.1.40rc2/tests/easy_app/auth.py` & `django-api-framework-0.1.7/tests/demo_app/auth.py`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/tests/easy_app/services.py` & `django-api-framework-0.1.7/tests/demo_app/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import TYPE_CHECKING, Any
 
 from django.http import HttpRequest
 
-from .domain import EventBiz
+from tests.demo_app.models import Event
 
 if TYPE_CHECKING:
     from ninja_extra.controllers.base import ControllerBase  # pragma: no cover
 
 from easy.services import BaseService
 
 
 class EventService(BaseService):
-    def __init__(self, biz=EventBiz()):
-        super().__init__(biz.model)
+    def __init__(self, model=Event):
+        super().__init__(model=model)
 
     @staticmethod
     async def prepare_create_event_data(data):
         """Helper func for unit testing"""
         object_data = data.copy()
         object_data.update(title=f"{object_data['title']}_create")
         return object_data
 
     async def get_event_objs_demo(self):
         """Demo API for unit testing"""
-        return await self.get_objs()
+        return await self.get_objs(maximum=10)
 
     async def get_identity_demo(self, word):
         """Demo API for unit testing"""
         return dict(says=word)
 
     def check_permission(
         self, request: HttpRequest, controller: "ControllerBase"
```

### Comparing `django-api-framework-0.1.40rc2/tests/test_api_base_response.py` & `django-api-framework-0.1.7/tests/demo_app/test_api_base_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 import json
 
 import pytest
 
-from easy.response import BaseAPIResponse
+from easy.response import BaseApiResponse
 
 
 def test_base_api_result_base():
-    assert BaseAPIResponse("").json_data["data"] == ""
 
-    assert BaseAPIResponse("1").json_data["data"] == "1"
+    assert BaseApiResponse("").json_data["data"] == ""
 
-    assert BaseAPIResponse("0").json_data["data"] == "0"
-    assert BaseAPIResponse().json_data["data"] == {}
-    assert BaseAPIResponse([]).json_data["data"] == []
-    assert BaseAPIResponse(True).json_data["data"] is True
-    assert BaseAPIResponse(False).json_data["data"] is False
-    assert BaseAPIResponse([1, 2, 3]).json_data["data"] == [1, 2, 3]
+    assert BaseApiResponse("1").json_data["data"] == "1"
+
+    assert BaseApiResponse("0").json_data["data"] == "0"
+    assert BaseApiResponse().json_data["data"] == {}
+    assert BaseApiResponse([]).json_data["data"] == []
+    assert BaseApiResponse(True).json_data["data"] is True
+    assert BaseApiResponse(False).json_data["data"] is False
+    assert BaseApiResponse([1, 2, 3]).json_data["data"] == [1, 2, 3]
 
 
 def test_base_api_result_dict():
-    assert BaseAPIResponse({"a": 1, "b": 2}).json_data["data"] == {
+
+    assert BaseApiResponse({"a": 1, "b": 2}).json_data["data"] == {
         "a": 1,
         "b": 2,
     }
 
-    assert (BaseAPIResponse({"code": 2, "im": 14})).json_data["data"]["im"] == 14
-    assert (BaseAPIResponse({"code": 2, "im": 14})).json_data["data"]["code"] == 2
+    assert (BaseApiResponse({"code": 2, "im": 14})).json_data["data"]["im"] == 14
+    assert (BaseApiResponse({"code": 2, "im": 14})).json_data["data"]["code"] == 2
 
 
 def test_base_api_result_message():
     assert (
-        BaseAPIResponse(code=-1, message="error test").json_data["message"]
+        BaseApiResponse(errno=-1, message="error test").json_data["message"]
         == "error test"
     )
-    assert BaseAPIResponse().json_data["message"]
+    assert BaseApiResponse().json_data["message"]
 
 
 def test_base_api_edit():
-    orig_resp = BaseAPIResponse(
+    orig_resp = BaseApiResponse(
         {"item_id": 2, "im": 14},
-        code=0,
+        errno=0,
     )
 
     with pytest.raises(KeyError):
-        print(orig_resp.json_data["detail"])
+        orig_resp.json_data["detail"]
 
     data = orig_resp.json_data
 
     data["detail"] = "Edited!!!"
     orig_resp.content = json.dumps(data)
 
     assert orig_resp.json_data["detail"] == "Edited!!!"
```

### Comparing `django-api-framework-0.1.40rc2/tests/test_async_api_permissions.py` & `django-api-framework-0.1.7/tests/demo_app/test_async_api_permissions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,167 +1,160 @@
 from datetime import datetime, timedelta
 
 import django
 import pytest
 from asgiref.sync import sync_to_async
 
-from .easy_app.controllers import (
+from tests.demo_app.controllers import (
     AdminSitePermissionAPIController,
     AutoGenCrudAPIController,
     PermissionAPIController,
 )
-from .easy_app.models import Client, Event, Type
-from .test_async_other_apis import dummy_data
+from tests.demo_app.models import Client, Event
+from tests.demo_app.test_async_other_apis import dummy_data
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
 @pytest.mark.django_db
 class TestPermissionController:
     async def test_demo(self, easy_api_client):
         client = easy_api_client(PermissionAPIController)
 
         response = await client.get(
-            "/must_be_authenticated/?word=authenticated",
-            content_type="application/json",
+            "/must_be_authenticated?word=authenticated", content_type="application/json"
         )
         assert response.status_code == 200
         assert response.json().get("data")["says"] == "authenticated"
 
         client = easy_api_client(PermissionAPIController)
         response = await client.get(
-            "/must_be_admin_user/?word=admin",
+            "/must_be_admin_user?word=admin",
         )
-        assert response.status_code == 403
+        assert response.status_code == 200
         with pytest.raises(KeyError):
             assert response.json().get("data")["says"] == "admin"
 
         client = easy_api_client(PermissionAPIController, is_staff=True)
         response = await client.get(
-            "/must_be_admin_user/?word=admin",
+            "/must_be_admin_user?word=admin",
         )
         assert response.status_code == 200
         assert response.json().get("data")["says"] == "admin"
 
         client = easy_api_client(PermissionAPIController)
         response = await client.get(
-            "/must_be_super_user/?word=superuser",
+            "/must_be_super_user?word=superuser",
         )
-        assert response.status_code == 403
+        assert response.status_code == 200
         with pytest.raises(KeyError):
             assert response.json().get("data")["says"] == "superuser"
 
         client = easy_api_client(PermissionAPIController, is_superuser=True)
         response = await client.get(
-            "/must_be_super_user/?word=superuser",
+            "/must_be_super_user?word=superuser",
         )
         assert response.status_code == 200
         assert response.json().get("data")["says"] == "superuser"
 
     async def test_perm(self, transactional_db, easy_api_client):
         client = easy_api_client(PermissionAPIController)
-        response = await client.get("/test_perm/", query=dict(word="normal"))
+        response = await client.get("/test_perm", query=dict(word="normal"))
         assert response.status_code == 200
         assert response.json().get("data")["says"] == "normal"
         client = easy_api_client(PermissionAPIController, is_staff=True)
-        response = await client.get("/test_perm/", query=dict(word="staff"))
+        response = await client.get("/test_perm", query=dict(word="staff"))
         assert response.status_code == 200
         assert response.json().get("data")["says"] == "staff"
 
     async def test_perm_only_super(self, transactional_db, easy_api_client):
         client = easy_api_client(PermissionAPIController)
-        response = await client.get("/test_perm_only_super/")
-        assert response.status_code == 403
+        response = await client.get("/test_perm_only_super")
+        assert response.status_code == 200
         assert response.json().get("data") == {
             "detail": "You do not have permission to perform this action."
         }
 
         client = easy_api_client(PermissionAPIController)
-        response = await client.get("/test_perm_only_super/")
-        assert response.status_code == 403
+        response = await client.get("/test_perm_only_super")
+        assert response.status_code == 200
         assert response.json().get("data") == {
             "detail": "You do not have permission to perform this action."
         }
 
         client = easy_api_client(PermissionAPIController, is_superuser=True)
-        response = await client.get("/test_perm_only_super/")
+        response = await client.get("/test_perm_only_super")
         assert response.status_code == 200
         assert response.json().get("data")["title"] == "test_event_title"
 
     async def test_perm_admin_site(self, transactional_db, easy_api_client):
         # None-admin users
         client = easy_api_client(PermissionAPIController)
         response = await client.get(
-            "/test_perm_admin_site/", query=dict(word="non-admin")
+            "/test_perm_admin_site", query=dict(word="non-admin")
         )
-        assert response.status_code == 403
+        assert response.status_code == 200
         assert response.json().get("data") == {
             "detail": "You do not have permission to perform this action."
         }
 
         # Staff users
-        client = easy_api_client(PermissionAPIController, is_staff=True, has_perm=True)
-        response = await client.get("/test_perm_admin_site/", query=dict(word="staff"))
+        client = easy_api_client(PermissionAPIController, is_staff=True)
+        response = await client.get("/test_perm_admin_site", query=dict(word="staff"))
         assert response.status_code == 200
-        assert response.json()["data"]["says"] == "staff"
-
+        assert response.json().get("data")["says"] == "staff"
 
-@pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
-@pytest.mark.django_db
-class TestAdminSitePermissionController:
     async def test_perm_auto_apis_delete(self, transactional_db, easy_api_client):
         client = easy_api_client(AdminSitePermissionAPIController)
         # Test delete
         object_data = dummy_data.copy()
         object_data.update(title=f"{object_data['title']}_get")
         event = await sync_to_async(Event.objects.create)(**object_data)
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
-        assert response.status_code == 403
+        assert response.status_code == 200
 
         response = await client.delete(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
-        assert response.status_code == 403
+        assert response.status_code == 200
         assert response.json().get("data") == {
             "detail": "You do not have permission to perform this action."
         }
 
         # Super users
         client = easy_api_client(AutoGenCrudAPIController, is_superuser=True)
-        response = await client.delete(
-            f"/{event.id}",
+        await client.delete(
+            f"/?id={event.id}",
         )
 
-        assert response.status_code == 200
-
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
         assert response.status_code == 200
-        assert response.json().get("code") == 404
+        assert response.json().get("data") == {}
 
     async def test_perm_auto_apis_patch(self, transactional_db, easy_api_client):
         client = easy_api_client(AdminSitePermissionAPIController)
 
         object_data = dummy_data.copy()
         event = await sync_to_async(Event.objects.create)(**object_data)
 
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
-        assert response.status_code == 403
+        assert response.status_code == 200
         assert response.json().get("data") == {
             "detail": "You do not have permission to perform this action."
         }
 
         # Staff users
         client = easy_api_client(AutoGenCrudAPIController, is_staff=True)
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
         assert response.json().get("data")["title"] == f"{object_data['title']}"
 
         client_g = await sync_to_async(Client.objects.create)(
             name="Client G for Unit Testings", key="G"
         )
 
@@ -175,53 +168,34 @@
             start_date=str((datetime.now() + timedelta(days=10)).date()),
             end_date=str((datetime.now() + timedelta(days=20)).date()),
             owner=[client_g.id, client_h.id],
         )
 
         client = easy_api_client(AdminSitePermissionAPIController)
         response = await client.patch(
-            f"/{event.id}", json=new_data, content_type="application/json"
+            f"/?id={event.id}", json=new_data, content_type="application/json"
         )
 
-        assert response.status_code == 403
+        assert response.status_code == 200
         assert response.json().get("data") == {
             "detail": "You do not have permission to perform this action."
         }
 
         # Super users
         client = easy_api_client(AutoGenCrudAPIController, is_superuser=True)
         response = await client.patch(
-            f"/{event.id}", json=new_data, content_type="application/json"
+            f"/?id={event.id}", json=new_data, content_type="application/json"
         )
-        assert response.json().get("message") == "Updated."
+        assert response.json().get("data")["id"] == event.id
+        assert response.json().get("data")["created"] is False
 
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
         assert response.status_code == 200
         assert response.json().get("data")["title"] == "AsyncAPIEvent_patch"
         assert response.json().get("data")["start_date"] == str(
             (datetime.now() + timedelta(days=10)).date()
         )
         assert response.json().get("data")["end_date"] == str(
             (datetime.now() + timedelta(days=20)).date()
         )
-
-    async def test_perm_auto_apis_add(self, transactional_db, easy_api_client):
-        client = easy_api_client(AdminSitePermissionAPIController)
-        type = await sync_to_async(Type.objects.create)(name="TypeForCreating")
-
-        object_data = dummy_data.copy()
-        object_data.update(title=f"{object_data['title']}_create")
-        object_data.update(type_id=type.id)
-
-        response = await client.put(
-            "/", json=object_data, content_type="application/json"
-        )
-        assert response.status_code == 403
-
-        client = easy_api_client(AdminSitePermissionAPIController, is_superuser=True)
-
-        response = await client.put(
-            "/", json=object_data, content_type="application/json"
-        )
-        assert response.status_code == 200
```

### Comparing `django-api-framework-0.1.40rc2/tests/test_async_auto_crud_apis.py` & `django-api-framework-0.1.7/tests/demo_app/test_async_auto_crud_apis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,27 @@
 import json
 from datetime import datetime, timedelta
 
 import django
 import pytest
 from asgiref.sync import sync_to_async
 
-from .easy_app.controllers import (
-    AutoGenCrudAPIController,
-    AutoGenCrudNoJoinAPIController,
-    AutoGenCrudSomeFieldsAPIController,
-    EventSchema,
-    InheritedRecursiveAPIController,
-    NoCrudAPIController,
-    NoCrudInheritedAPIController,
-    RecursiveAPIController,
-)
-from .easy_app.models import Category, Client, Event, Type
+from tests.demo_app.controllers import AutoGenCrudAPIController, EventSchema
+from tests.demo_app.models import Category, Client, Event, Type
 
 dummy_data = dict(
     title="AsyncAdminAPIEvent",
     start_date=str(datetime.now().date()),
     end_date=str((datetime.now() + timedelta(days=5)).date()),
 )
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
 @pytest.mark.django_db
 class TestAutoCrudAdminAPI:
-    async def test_crud_generate_or_not(self, transactional_db, easy_api_client):
-        client = easy_api_client(NoCrudAPIController)
-
-        object_data = dummy_data.copy()
-        object_data.update(title=f"{object_data['title']}_get")
-
-        event = await sync_to_async(Event.objects.create)(**object_data)
-
-        with pytest.raises(Exception):
-            await client.get(
-                f"/{event.id}",
-            )
-
-        client = easy_api_client(NoCrudInheritedAPIController, is_superuser=True)
-
-        object_data = dummy_data.copy()
-        object_data.update(title=f"{object_data['title']}_get")
-
-        event = await sync_to_async(Event.objects.create)(**object_data)
-
-        response = await client.get(
-            f"/{event.id}",
-        )
-        assert response.status_code == 200
-        with pytest.raises(Exception):
-            print(response.json()["data"]["start_date"])
-
     async def test_crud_default_get_all(self, transactional_db, easy_api_client):
         client = easy_api_client(AutoGenCrudAPIController)
 
         object_data = dummy_data.copy()
         object_data.update(title=f"{object_data['title']}_get_all")
 
         event = await sync_to_async(Event.objects.create)(**object_data)
@@ -73,66 +37,40 @@
         )
         event.category = category
         event.type = type
         await sync_to_async(event.save)()
         await sync_to_async(event.owner.set)([client_a, client_b])
 
         response = await client.get(
-            "/", query=dict(maximum=100, filters=json.dumps(dict(id__gte=1)))
+            "/get_all", query=dict(maximum=100, filters=json.dumps(dict(id__gte=1)))
         )
         assert response.status_code == 200
 
         data = response.json().get("data")
         assert data[0]["title"] == "AsyncAdminAPIEvent_get_all"
         assert data[0]["type"] == type.id
 
         event_schema = json.loads(EventSchema.from_orm(event).json())
         assert event_schema["start_date"] == data[0]["start_date"]
 
-        # Recursive = True
-        client = easy_api_client(RecursiveAPIController)
-        response = await client.get(
-            "/", query=dict(maximum=100, filters=json.dumps(dict(id__gte=1)))
-        )
-        assert response.status_code == 200
-
-        data = response.json().get("data")
-        assert data[0]["title"] == "AsyncAdminAPIEvent_get_all"
-
-        assert data[0]["type"]["id"] == type.id
-        assert data[0]["category"]["status"] == 1
-
-        # Recursive = True, inherited class
-        client = easy_api_client(InheritedRecursiveAPIController)
         response = await client.get(
-            "/", query=dict(maximum=100, filters=json.dumps(dict(id__gte=1)))
-        )
-        assert response.status_code == 200
-
-        data = response.json().get("data")
-        assert data[0]["title"] == "AsyncAdminAPIEvent_get_all"
-
-        assert data[0]["type"]["id"] == type.id
-        assert data[0]["category"]["status"] == 1
-
-        # Back to AutoGenCrudAPIController
-        client = easy_api_client(AutoGenCrudAPIController)
-
-        response = await client.get(
-            "/",
+            "/get_all",
+            query=dict(
+                maximum=100,
+            ),
         )
         assert response.status_code == 200
 
         data = response.json().get("data")
         assert data[0]["title"] == "AsyncAdminAPIEvent_get_all"
 
         event_schema = json.loads(EventSchema.from_orm(event).json())
         assert event_schema["start_date"] == data[0]["start_date"]
 
-        response = await client.get("/")
+        response = await client.get("/get_all")
         assert response.status_code == 200
 
         data = response.json().get("data")
         assert data[0]["title"] == "AsyncAdminAPIEvent_get_all"
 
         event_schema = json.loads(EventSchema.from_orm(event).json())
         assert event_schema["start_date"] == data[0]["start_date"]
@@ -142,164 +80,140 @@
 
         object_data = dummy_data.copy()
         object_data.update(title=f"{object_data['title']}_get")
 
         event = await sync_to_async(Event.objects.create)(**object_data)
 
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
         assert response.status_code == 200
 
         data = response.json().get("data")
         assert data["title"] == "AsyncAdminAPIEvent_get"
 
         event_schema = json.loads(EventSchema.from_orm(event).json())
         assert event_schema["end_date"] == data["end_date"]
 
         await client.delete(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
 
         response = await client.get(
-            f"/{event.id}",
+            f"/?id={event.id}",
         )
         assert response.status_code == 200
-        assert response.json().get("code") == 404
-
-        response = await client.delete("/20000")
-        assert response.status_code == 200
-        assert response.json().get("data") == "Not Found."
+        assert response.json().get("data") == {}
 
     async def test_crud_default_create(self, transactional_db, easy_api_client):
         client = easy_api_client(AutoGenCrudAPIController)
 
         client_c = await sync_to_async(Client.objects.create)(
             name="Client C for Unit Testings", key="C"
         )
 
         client_d = await sync_to_async(Client.objects.create)(
             name="Client D for Unit Testings", key="D"
         )
 
-        type = await sync_to_async(Type.objects.create)(name="TypeForCreating")
-
         object_data = dummy_data.copy()
         object_data.update(title=f"{object_data['title']}_create")
         object_data.update(owner=[client_c.id, client_d.id])
-        object_data.update(lead_owner=[client_d.id])
-        object_data.update(type_id=type.id)
 
         response = await client.put(
             "/", json=object_data, content_type="application/json"
         )
         assert response.status_code == 200
-        assert response.json().get("code") == 201
-        assert response.json().get("message") == "Created."
 
         event_id = response.json().get("data")["id"]
 
         response = await client.get(
-            f"/{event_id}",
+            f"/?id={event_id}",
         )
-
         assert response.status_code == 200
         assert response.json().get("data")["title"] == "AsyncAdminAPIEvent_create"
 
-    async def test_crud_default_create_some_fields(
-        self, transactional_db, easy_api_client
-    ):
-        client = easy_api_client(AutoGenCrudSomeFieldsAPIController)
-
-        category = await sync_to_async(Category.objects.create)(
-            title="Category for Unit Testings"
-        )
-
-        client_type = await sync_to_async(Client.objects.create)(
-            name="Client for Unit Testings",
-            key="Type",
-            category=category,
-            password="DUMMY_PASSWORD",
-        )
-
-        response = await client.get(
-            f"/{client_type.id}",
-        )
-
-        assert response.status_code == 200
-        assert response.json()["data"]["key"] == "Type"
-        with pytest.raises(KeyError):
-            print(response.json()["data"]["password"])
-        with pytest.raises(KeyError):
-            print(response.json()["data"]["category"])
-
     async def test_crud_default_patch(self, transactional_db, easy_api_client):
         client = easy_api_client(AutoGenCrudAPIController)
 
         object_data = dummy_data.copy()
         event = await sync_to_async(Event.objects.create)(**object_data)
 
         response = await client.get(
-            f"/{event.pk}",
+            f"/?id={event.id}",
         )
         assert response.status_code == 200
         assert response.json().get("data")["title"] == f"{object_data['title']}"
 
         client_e = await sync_to_async(Client.objects.create)(
             name="Client E for Unit Testings", key="E"
         )
 
         client_f = await sync_to_async(Client.objects.create)(
             name="Client F for Unit Testings", key="F"
         )
 
-        category = await sync_to_async(Category.objects.create)(
-            title="Category for Unit Testings", status=2
-        )
-
         new_data = dict(
-            id=event.pk,
+            id=event.id,
             title=f"{object_data['title']}_patch",
             start_date=str((datetime.now() + timedelta(days=10)).date()),
             end_date=str((datetime.now() + timedelta(days=20)).date()),
-            owner=[client_e.pk, client_f.pk],
-            category=category.pk,
+            owner=[client_e.id, client_f.id],
         )
 
         response = await client.patch(
-            "/20000", json=new_data, content_type="application/json"
+            f"/?id={event.id}", json=new_data, content_type="application/json"
         )
 
         assert response.status_code == 200
-        assert response.json()["code"] == 400
+        assert response.json().get("data")["id"] == event.id
+        assert response.json().get("data")["created"] is False
 
-        response = await client.patch(
-            f"/{event.pk}", json=new_data, content_type="application/json"
+        response = await client.get(
+            f"/?id={event.id}",
         )
-
         assert response.status_code == 200
-        assert response.json().get("message") == "Updated."
+        assert response.json().get("data")["title"] == "AsyncAdminAPIEvent_patch"
+        assert response.json().get("data")["start_date"] == str(
+            (datetime.now() + timedelta(days=10)).date()
+        )
+        assert response.json().get("data")["end_date"] == str(
+            (datetime.now() + timedelta(days=20)).date()
+        )
+
+    async def test_default_filter(self, transactional_db, easy_api_client):
+        object_data = dummy_data.copy()
+        object_data.update(title=f"{object_data['title']}_filter")
+
+        event = await sync_to_async(Event.objects.create)(**object_data)
+
+        client = easy_api_client(AutoGenCrudAPIController)
 
         response = await client.get(
-            f"/{event.pk}",
+            "/filter", query=dict(filters=json.dumps(dict(id__gte=1)))
         )
         assert response.status_code == 200
+
         data = response.json().get("data")
+        assert data[0]["title"] == "AsyncAdminAPIEvent_filter"
 
-        assert len(data["owner"]) == 2
-        assert len(data["lead_owner"]) == 0
-        assert data["owner"][0]["name"] == "Client E for Unit Testings"
-        assert data["owner"][1]["name"] == "Client F for Unit Testings"
-
-        assert data["title"] == "AsyncAdminAPIEvent_patch"
-        assert data["start_date"] == str((datetime.now() + timedelta(days=10)).date())
-        assert data["end_date"] == str((datetime.now() + timedelta(days=20)).date())
+        event_schema = json.loads(EventSchema.from_orm(event).json())
+        assert event_schema["end_date"] == data[0]["end_date"]
 
-        client = easy_api_client(AutoGenCrudNoJoinAPIController)
+    async def test_crud_filter_exclude(self, transactional_db, easy_api_client):
+        object_data = dummy_data.copy()
+        object_data.update(title=f"{object_data['title']}_exclude")
+
+        event = await sync_to_async(Event.objects.create)(**object_data)
+
+        client = easy_api_client(AutoGenCrudAPIController)
 
-        # No auto join
         response = await client.get(
-            f"/{event.pk}",
+            "/filter_exclude", query=dict(filters=json.dumps(dict(id__lt=1)))
         )
         assert response.status_code == 200
+
         data = response.json().get("data")
-        assert data["owner"] == [8, 9]
+        assert data[0]["title"] == "AsyncAdminAPIEvent_exclude"
+
+        event_schema = json.loads(EventSchema.from_orm(event).json())
+        assert event_schema["end_date"] == data[0]["end_date"]
```

### Comparing `django-api-framework-0.1.40rc2/tests/test_async_other_apis.py` & `django-api-framework-0.1.7/tests/demo_app/test_async_other_apis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from datetime import datetime, timedelta
 
 import django
 import pytest
 from asgiref.sync import sync_to_async
 
-from .easy_app.controllers import EasyCrudAPIController
-from .easy_app.models import Event, Type
-from .easy_app.schema import EventSchema
-from .easy_app.services import EventService
+from tests.demo_app.controllers import EasyCrudAPIController
+from tests.demo_app.models import Event, Type
+from tests.demo_app.schema import EventSchema
+from tests.demo_app.services import EventService
 
 dummy_data = dict(
     title="AsyncAPIEvent",
     start_date=str(datetime.now().date()),
     end_date=str((datetime.now() + timedelta(days=5)).date()),
 )
 
@@ -26,49 +26,48 @@
         object_data = await EventService.prepare_create_event_data(dummy_data)
 
         response = await client.put(
             "/", json=object_data, content_type="application/json"
         )
         assert response.status_code == 200
 
-        assert response.json().get("code") == 201
         event_id = response.json().get("data")["id"]
 
         response = await client.get(
-            f"/{event_id}",
+            f"/?id={event_id}",
         )
         assert response.status_code == 200
         assert response.json().get("data")["title"] == "AsyncAPIEvent_create"
 
-        response = await client.get("/")
+        response = await client.get("/get_all")
         assert response.status_code == 200
         assert response.json().get("data")[0]["title"] == "AsyncAPIEvent_create"
 
     async def test_base_response(self, transactional_db, easy_api_client):
         client = easy_api_client(EasyCrudAPIController)
 
         response = await client.get(
-            "/base_response/",
+            "/base_response",
         )
         assert response.status_code == 200
-        assert response.json().get("data")["data"] == "This is a BaseAPIResponse."
+        assert response.json().get("data")["data"] == "This is a BaseApiResponse."
 
     async def test_qs_paginated(self, transactional_db, easy_api_client):
         client = easy_api_client(EasyCrudAPIController)
 
         object_data = await EventService.prepare_create_event_data(dummy_data)
 
         response = await client.put(
             "/", json=object_data, content_type="application/json"
         )
         assert response.status_code == 200
-        assert response.json().get("code") == 201
+
         event_id = response.json().get("data")["id"]
         response = await client.get(
-            "/qs_paginated/",
+            "/qs_paginated",
         )
         assert response.status_code == 200
         assert response.json().get("data")[0]["id"] == event_id
 
     async def test_qs_list(self, transactional_db, easy_api_client):
         client = easy_api_client(EasyCrudAPIController)
 
@@ -82,37 +81,21 @@
 
         type = await sync_to_async(Type.objects.create)(name="Test-Type-88")
         object_data = await EventService.prepare_create_event_data(dummy_data)
         object_data.update(title=f"{object_data['title']}_qs_list_88", type=type)
         event = await sync_to_async(Event.objects.create)(**object_data)
 
         response = await client.get(
-            "/qs_list/",
+            "/qs_list",
         )
         assert response.status_code == 200
 
         data = response.json().get("data")
 
         assert data[0]["title"] == "AsyncAPIEvent_create_qs_list_0"
 
         event_schema = json.loads(EventSchema.from_orm(event).json())
         assert (
             event_schema["title"]
             == data[4]["title"]
             == "AsyncAPIEvent_create_qs_list_88"
         )
-
-    async def test_qs_(self, transactional_db, easy_api_client):
-        client = easy_api_client(EasyCrudAPIController)
-
-        for i in range(4):
-            type = await sync_to_async(Type.objects.create)(name=f"Test-Type-{i}")
-            object_data = await EventService.prepare_create_event_data(dummy_data)
-            object_data.update(title=f"{object_data['title']}_qs_{i}", type=type.id)
-            await client.put("/", json=object_data)
-
-        response = await client.get(
-            "/qs/",
-        )
-        assert response.status_code == 200
-
-        assert response.json().get("data")[0]["title"] == "AsyncAPIEvent_create_qs_0"
```

### Comparing `django-api-framework-0.1.40rc2/tests/test_doc_decorator.py` & `django-api-framework-0.1.7/tests/demo_app/test_doc_decorator.py`

 * *Files identical despite different names*

### Comparing `django-api-framework-0.1.40rc2/tests/test_exceptions.py` & `django-api-framework-0.1.7/tests/demo_app/test_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 from django.test import RequestFactory
 from django.utils.translation import gettext_lazy as _
-from ninja_extra import exceptions
+from ninja_extra import NinjaExtraAPI, exceptions, testing
 
-from easy import EasyAPI, testing
 from easy.exception import APIAuthException, BaseAPIException
 
-api = EasyAPI(urls_namespace="exception")
+api = NinjaExtraAPI(urls_namespace="exception")
 
 
 @api.get("/list_exception")
-async def list_exception(request):
+def list_exception(request):
     raise BaseAPIException(
         [
             "some error 1",
             "some error 2",
         ]
     )
 
 
 @api.get("/list_exception_full_detail")
-async def list_exception_full(request):
+def list_exception_full(request):
     exception = BaseAPIException(
         [
             "some error 1",
             "some error 2",
         ]
     )
     return exception.get_full_details()
 
 
 @api.get("/dict_exception")
-async def dict_exception(request):
+def dict_exception(request):
     raise BaseAPIException(dict(error="error 1"))
 
 
 @api.get("/dict_exception_full_detail")
-async def dict_exception_full_detail(request):
+def dict_exception_full_detail(request):
     exception = BaseAPIException(dict(error="error 1"))
     return exception.get_full_details()
 
 
 @api.get("/dict_exception_code_detail")
-async def dict_exception_code_detail(request):
+def dict_exception_code_detail(request):
     exception = BaseAPIException(dict(error="error 1"))
     return exception.get_codes()
 
 
 @api.get("/list_exception_code_detail")
-async def list_exception_code_detail(request):
+def list_exception_code_detail(request):
     exception = BaseAPIException(["some error"])
     return exception.get_codes()
 
 
-client = testing.EasyTestClient(api)
+client = testing.TestClient(api)
 
 
 class TestException:
-    async def test_get_error_details(self):
+    def test_get_error_details(self):
         example = "string"
         lazy_example = _(example)
 
         assert exceptions._get_error_details(lazy_example) == example
 
         assert isinstance(
             exceptions._get_error_details(lazy_example), exceptions.ErrorDetail
@@ -80,106 +79,101 @@
         assert isinstance(
             exceptions._get_error_details([[lazy_example]])[0][0],
             exceptions.ErrorDetail,
         )
 
 
 class TestErrorDetail:
-    async def test_eq(self):
+    def test_eq(self):
         assert exceptions.ErrorDetail("msg") == exceptions.ErrorDetail("msg")
         assert exceptions.ErrorDetail("msg", "code") == exceptions.ErrorDetail(
             "msg", code="code"
         )
 
         assert exceptions.ErrorDetail("msg") == "msg"
         assert exceptions.ErrorDetail("msg", "code") == "msg"
 
-    async def test_ne(self):
+    def test_ne(self):
         assert exceptions.ErrorDetail("msg1") != exceptions.ErrorDetail("msg2")
         assert exceptions.ErrorDetail("msg") != exceptions.ErrorDetail(
             "msg", code="invalid"
         )
 
         assert exceptions.ErrorDetail("msg1") != "msg2"
         assert exceptions.ErrorDetail("msg1", "code") != "msg2"
 
-    async def test_repr(self):
+    def test_repr(self):
         assert repr(
             exceptions.ErrorDetail("msg1")
         ) == "ErrorDetail(string={!r}, code=None)".format("msg1")
         assert repr(
             exceptions.ErrorDetail("msg1", "code")
         ) == "ErrorDetail(string={!r}, code={!r})".format("msg1", "code")
 
-    async def test_str(self):
+    def test_str(self):
         assert str(exceptions.ErrorDetail("msg1")) == "msg1"
         assert str(exceptions.ErrorDetail("msg1", "code")) == "msg1"
 
-    async def test_hash(self):
+    def test_hash(self):
         assert hash(exceptions.ErrorDetail("msg")) == hash("msg")
         assert hash(exceptions.ErrorDetail("msg", "code")) == hash("msg")
 
 
-async def test_server_error():
+def test_server_error():
     request = RequestFactory().get("/")
     response = exceptions.server_error(request)
     assert response.status_code == 500
     assert response["content-type"] == "application/json"
 
 
-async def test_bad_request():
+def test_bad_request():
     request = RequestFactory().get("/")
     exception = Exception("Something went wrong — Not used")
     response = exceptions.bad_request(request, exception)
     assert response.status_code == 400
     assert response["content-type"] == "application/json"
 
 
-async def test_exception_with_list_details():
-    res = await client.get("list_exception")
+def test_exception_with_list_details():
+    res = client.get("list_exception")
     assert res.status_code == 500
-    assert res.json()["data"] == {
-        "detail": "[ErrorDetail(string='some error 1', code='error'), "
-        "ErrorDetail(string='some error 2', code='error')]",
-    }
+    assert res.json() == ["some error 1", "some error 2"]
 
 
-async def test_exception_with_list_full_details():
-    res = await client.get("list_exception_full_detail")
+def test_exception_with_list_full_details():
+    res = client.get("list_exception_full_detail")
     assert res.status_code == 200
-    assert res.json()["data"] == [
+    assert res.json() == [
         {"message": "some error 1", "code": "error"},
         {"message": "some error 2", "code": "error"},
     ]
 
 
-async def test_exception_with_dict_details():
-    res = await client.get("dict_exception")
+def test_exception_with_dict_details():
+    res = client.get("dict_exception")
     assert res.status_code == 500
-    assert res.json()["data"] == {
-        "detail": "{'error': ErrorDetail(string='error 1', code='error')}"
-    }
+    assert res.json() == dict(error="error 1")
 
 
-async def test_exception_with_full_details():
-    res = await client.get("dict_exception_full_detail")
+def test_exception_with_full_details():
+    res = client.get("dict_exception_full_detail")
     assert res.status_code == 200
-    assert res.json()["data"] == {"error": {"message": "error 1", "code": "error"}}
+    assert res.json() == {"error": {"message": "error 1", "code": "error"}}
 
 
-async def test_exception_dict_exception_code_detail():
-    res = await client.get("dict_exception_code_detail")
+def test_exception_dict_exception_code_detail():
+    res = client.get("dict_exception_code_detail")
     assert res.status_code == 200
-    assert res.json()["data"] == {"error": "error"}
+    assert res.json() == {"error": "error"}
 
 
-async def test_exception_with_list_exception_code_detail():
-    res = await client.get("list_exception_code_detail")
+def test_exception_with_list_exception_code_detail():
+    res = client.get("list_exception_code_detail")
     assert res.status_code == 200
-    assert res.json()["data"] == ["error"]
+    assert res.json() == ["error"]
 
 
 def test_validation_error():
     exception = exceptions.ValidationError()
     assert exception.detail == [
         exceptions.ErrorDetail(
             string=exceptions.ValidationError.default_detail,
@@ -199,56 +193,31 @@
     )
     assert exception.get_codes() == exceptions.MethodNotAllowed.default_code
 
     exception = exceptions.MethodNotAllowed("get", ["errors"])
     assert exception.detail == ["errors"]
 
 
-async def test_method_not_allowed_accepted_error():
+def test_method_not_allowed_accepted_error():
     exception = exceptions.NotAcceptable()
     assert exception.detail == exceptions.NotAcceptable.default_detail
     assert exception.get_codes() == exceptions.NotAcceptable.default_code
 
     exception = exceptions.NotAcceptable(["errors"])
     assert exception.detail == ["errors"]
 
 
-async def test_unsupported_media_type_allowed_error():
+def test_unsupported_media_type_allowed_error():
     exception = exceptions.UnsupportedMediaType("whatever/type")
     assert exception.detail == exceptions.UnsupportedMediaType.default_detail.format(
         media_type="whatever/type"
     )
     assert exception.get_codes() == exceptions.UnsupportedMediaType.default_code
 
     exception = exceptions.UnsupportedMediaType("whatever/type", ["errors"])
     assert exception.detail == ["errors"]
 
 
-async def test_api_exception_code():
-    exception = APIAuthException("Unexpected error")
+def test_api_exception_code():
+    exception = APIAuthException("Unexpected error", code=503)
     assert exception.detail == "Unexpected error"
-    assert exception.status_code == 401
-
-
-api_default = EasyAPI(urls_namespace="exception_default", easy_output=False)
-
-
-@api_default.get("/list_exception")
-async def list_exception_default(request):
-    raise BaseAPIException(
-        [
-            "some error 1",
-            "some error 2",
-        ]
-    )
-
-
-client_default = testing.EasyTestClient(api_default)
-
-
-async def test_exception_with_list_details_default():
-    res = await client_default.get("list_exception")
-    assert res.status_code == 500
-    assert res.json() == {
-        "detail": "[ErrorDetail(string='some error 1', code='error'), "
-        "ErrorDetail(string='some error 2', code='error')]",
-    }
+    assert exception.status_code == 503
```

