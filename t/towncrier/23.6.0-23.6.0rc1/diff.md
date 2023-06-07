# Comparing `tmp/towncrier-23.6.0.tar.gz` & `tmp/towncrier-23.6.0rc1.tar.gz`

## Comparing `towncrier-23.6.0.tar` & `towncrier-23.6.0rc1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 towncrier-23.6.0/.flake8
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 towncrier-23.6.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 towncrier-23.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 towncrier-23.6.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 towncrier-23.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 towncrier-23.6.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0    21741 2020-02-02 00:00:00.000000 towncrier-23.6.0/NEWS.rst
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 towncrier-23.6.0/RELEASE.rst
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 towncrier-23.6.0/noxfile.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 towncrier-23.6.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 towncrier-23.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 towncrier-23.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/__main__.py
--rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_builder.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_git.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_project.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_shell.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_version.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_writer.py
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/build.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/check.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/create.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_settings/__init__.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_settings/fragment_types.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/_settings/load.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/templates/default.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/templates/default.rst
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/templates/hr-between-versions.rst
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/templates/single-file-no-bullets.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/__init__.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/helpers.py
--rw-r--r--   0        0        0    42541 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_build.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_builder.py
--rw-r--r--   0        0        0    10636 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_check.py
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_create.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_format.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_git.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_packaging.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_project.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_settings.py
--rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 towncrier-23.6.0/src/towncrier/test/test_write.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 towncrier-23.6.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 towncrier-23.6.0/LICENSE
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 towncrier-23.6.0/README.rst
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 towncrier-23.6.0/pyproject.toml
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 towncrier-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.flake8
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    21747 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/NEWS.rst
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/RELEASE.rst
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/noxfile.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/__main__.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_builder.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_git.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_project.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_shell.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_version.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_writer.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/build.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/check.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/create.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_settings/__init__.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_settings/fragment_types.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/_settings/load.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/default.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/default.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/hr-between-versions.rst
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/templates/single-file-no-bullets.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/__init__.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/helpers.py
+-rw-r--r--   0        0        0    42541 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_build.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_builder.py
+-rw-r--r--   0        0        0    10636 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_check.py
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_create.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_format.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_git.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_packaging.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_project.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_settings.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/src/towncrier/test/test_write.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/README.rst
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 towncrier-23.6.0rc1/PKG-INFO
```

### Comparing `towncrier-23.6.0/.pre-commit-config.yaml` & `towncrier-23.6.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/CODE_OF_CONDUCT.md` & `towncrier-23.6.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/CONTRIBUTING.rst` & `towncrier-23.6.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/NEWS.rst` & `towncrier-23.6.0rc1/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Release notes
 #############
 
 ``towncrier`` issues are filed on `GitHub <https://github.com/twisted/towncrier/issues>`_, and each ticket number here corresponds to a closed GitHub issue.
 
 .. towncrier release notes start
 
-towncrier 23.6.0 (2023-06-06)
-=============================
+towncrier 23.6.0rc1 (2023-06-05)
+================================
 
 This is the last release to support Python 3.7.
 
 
 Features
 --------
```

### Comparing `towncrier-23.6.0/RELEASE.rst` & `towncrier-23.6.0rc1/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/noxfile.py` & `towncrier-23.6.0rc1/noxfile.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `towncrier-23.6.0rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/.github/workflows/ci.yml` & `towncrier-23.6.0rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/__init__.py` & `towncrier-23.6.0rc1/src/towncrier/__init__.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_builder.py` & `towncrier-23.6.0rc1/src/towncrier/_builder.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_git.py` & `towncrier-23.6.0rc1/src/towncrier/_git.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_project.py` & `towncrier-23.6.0rc1/src/towncrier/_project.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_shell.py` & `towncrier-23.6.0rc1/src/towncrier/_shell.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_writer.py` & `towncrier-23.6.0rc1/src/towncrier/_writer.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/build.py` & `towncrier-23.6.0rc1/src/towncrier/build.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/check.py` & `towncrier-23.6.0rc1/src/towncrier/check.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/create.py` & `towncrier-23.6.0rc1/src/towncrier/create.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_settings/__init__.py` & `towncrier-23.6.0rc1/src/towncrier/_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_settings/fragment_types.py` & `towncrier-23.6.0rc1/src/towncrier/_settings/fragment_types.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/_settings/load.py` & `towncrier-23.6.0rc1/src/towncrier/_settings/load.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/templates/default.md` & `towncrier-23.6.0rc1/src/towncrier/templates/default.md`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/templates/default.rst` & `towncrier-23.6.0rc1/src/towncrier/templates/default.rst`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/templates/hr-between-versions.rst` & `towncrier-23.6.0rc1/src/towncrier/templates/hr-between-versions.rst`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/templates/single-file-no-bullets.rst` & `towncrier-23.6.0rc1/src/towncrier/templates/single-file-no-bullets.rst`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/helpers.py` & `towncrier-23.6.0rc1/src/towncrier/test/helpers.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_build.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_build.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_builder.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_builder.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_check.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_check.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_create.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_create.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_format.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_format.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_packaging.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_packaging.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_project.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_project.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_settings.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/src/towncrier/test/test_write.py` & `towncrier-23.6.0rc1/src/towncrier/test/test_write.py`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/LICENSE` & `towncrier-23.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/README.rst` & `towncrier-23.6.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/pyproject.toml` & `towncrier-23.6.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `towncrier-23.6.0/PKG-INFO` & `towncrier-23.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towncrier
-Version: 23.6.0
+Version: 23.6.0rc1
 Summary: Building newsfiles for your project.
 Project-URL: Documentation, https://towncrier.readthedocs.io/
 Project-URL: Chat, https://web.libera.chat/?channels=%23twisted
 Project-URL: Mailing list, https://mail.python.org/mailman3/lists/twisted.python.org/
 Project-URL: Issues, https://github.com/twisted/towncrier/issues
 Project-URL: Repository, https://github.com/twisted/towncrier
 Project-URL: Tests, https://github.com/twisted/towncrier/actions?query=branch%3Atrunk
```

