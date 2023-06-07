# Comparing `tmp/pypnusershub-1.6.6.tar.gz` & `tmp/pypnusershub-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnusershub-1.6.6.tar", last modified: Tue Jun  6 20:42:11 2023, max compression
+gzip compressed data, was "pypnusershub-1.6.7.tar", last modified: Wed Jun  7 08:42:08 2023, max compression
```

## Comparing `pypnusershub-1.6.6.tar` & `pypnusershub-1.6.7.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/requirements-common.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/requirements-dependencies.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.326425 pypnusershub-1.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.330425 pypnusershub-1.6.6/src/pypnusershub/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub/db/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/fixtures.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/models_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/db/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs-samples.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.338425 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10925 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/routes_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 20:41:57.000000 pypnusershub-1.6.6/src/pypnusershub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:42:11.334425 pypnusershub-1.6.6/src/pypnusershub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 20:42:11.000000 pypnusershub-1.6.6/src/pypnusershub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/requirements-common.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/requirements-dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.410686 pypnusershub-1.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.418686 pypnusershub-1.6.7/src/pypnusershub/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.422686 pypnusershub-1.6.7/src/pypnusershub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/fixtures.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/models_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.422686 pypnusershub-1.6.7/src/pypnusershub/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.422686 pypnusershub-1.6.7/src/pypnusershub/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs-samples.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10925 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/routes_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/src/pypnusershub/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/test_utilisateurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.418686 pypnusershub-1.6.7/src/pypnusershub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/top_level.txt
```

### Comparing `pypnusershub-1.6.6/LICENSE` & `pypnusershub-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/PKG-INFO` & `pypnusershub-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.6/README.md` & `pypnusershub-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/setup.py` & `pypnusershub-1.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/__main__.py` & `pypnusershub-1.6.7/src/pypnusershub/__main__.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/db/fixtures.sql` & `pypnusershub-1.6.7/src/pypnusershub/db/fixtures.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/db/models.py` & `pypnusershub-1.6.7/src/pypnusershub/db/models.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/db/models_register.py` & `pypnusershub-1.6.7/src/pypnusershub/db/models_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/db/tools.py` & `pypnusershub-1.6.7/src/pypnusershub/db/tools.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/env.py` & `pypnusershub-1.6.7/src/pypnusershub/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs-samples.sql` & `pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs-samples.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/data/utilisateurs.sql` & `pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/env.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py` & `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/routes.py` & `pypnusershub-1.6.7/src/pypnusershub/routes.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/routes_register.py` & `pypnusershub-1.6.7/src/pypnusershub/routes_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/schemas.py` & `pypnusershub-1.6.7/src/pypnusershub/schemas.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub/utils.py` & `pypnusershub-1.6.7/src/pypnusershub/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.6/src/pypnusershub.egg-info/PKG-INFO` & `pypnusershub-1.6.7/src/pypnusershub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.6/src/pypnusershub.egg-info/SOURCES.txt` & `pypnusershub-1.6.7/src/pypnusershub.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -33,8 +33,13 @@
 src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
 src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
 src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
 src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
 src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
 src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
 src/pypnusershub/migrations/versions/__init__.py
-src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+src/pypnusershub/tests/__init__.py
+src/pypnusershub/tests/conftest.py
+src/pypnusershub/tests/fixtures.py
+src/pypnusershub/tests/test_utilisateurs.py
+src/pypnusershub/tests/utils.py
```

