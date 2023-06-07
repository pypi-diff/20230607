# Comparing `tmp/moneyflow_base-0.0.4.tar.gz` & `tmp/moneyflow_base-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyflow_base-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "moneyflow_base-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `moneyflow_base-0.0.4.tar` & `moneyflow_base-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3090 2023-05-29 05:57:47.185851 moneyflow_base-0.0.4/.gitignore
--rw-r--r--   0        0        0        4 2023-06-03 20:00:36.415875 moneyflow_base-0.0.4/LICENSE
--rw-r--r--   0        0        0     1974 2023-06-03 21:01:04.183510 moneyflow_base-0.0.4/Makefile
--rw-r--r--   0        0        0       90 2023-05-29 05:54:55.382142 moneyflow_base-0.0.4/README.md
--rw-r--r--   0        0        0        6 2023-05-31 06:00:54.518458 moneyflow_base-0.0.4/VERSION
--rw-r--r--   0        0        0     6148 2022-02-16 17:13:36.168907 moneyflow_base-0.0.4/docs/.DS_Store
--rw-r--r--   0        0        0      638 2022-02-14 21:51:19.000000 moneyflow_base-0.0.4/docs/Makefile
--rw-r--r--   0        0        0      804 2022-02-14 21:51:19.000000 moneyflow_base-0.0.4/docs/make.bat
--rw-r--r--   0        0        0     2252 2023-05-30 07:29:16.202817 moneyflow_base-0.0.4/docs/source/conf.py
--rw-r--r--   0        0        0      513 2023-05-30 04:52:49.017528 moneyflow_base-0.0.4/docs/source/index.rst
--rw-r--r--   0        0        0       89 2023-05-30 04:38:20.375048 moneyflow_base-0.0.4/docs/source/mbase/eventlog.rst
--rw-r--r--   0        0        0       80 2023-05-30 04:52:11.924670 moneyflow_base-0.0.4/docs/source/mbase/services.rst
--rw-r--r--   0        0        0       65 2023-05-30 04:49:31.167705 moneyflow_base-0.0.4/docs/source/mbase/utils.rst
--rw-r--r--   0        0        0        0 2023-05-29 05:54:36.692581 moneyflow_base-0.0.4/mbase/__init__.py
--rw-r--r--   0        0        0     7792 2023-05-30 07:32:56.751342 moneyflow_base-0.0.4/mbase/eventlog.py
--rw-r--r--   0        0        0      859 2023-05-29 05:54:36.702787 moneyflow_base-0.0.4/mbase/exceptions.py
--rw-r--r--   0        0        0    21987 2023-05-29 17:52:37.309182 moneyflow_base-0.0.4/mbase/future.py
--rw-r--r--   0        0        0      946 2023-05-31 05:37:13.359364 moneyflow_base-0.0.4/mbase/mlogging.py
--rw-r--r--   0        0        0     7302 2023-05-31 06:00:47.348683 moneyflow_base-0.0.4/mbase/models.py
--rw-r--r--   0        0        0     3144 2023-05-29 18:02:21.856877 moneyflow_base-0.0.4/mbase/services.py
--rw-r--r--   0        0        0    10981 2023-05-31 05:36:39.195619 moneyflow_base-0.0.4/mbase/utils.py
--rw-r--r--   0        0        0      743 2023-06-04 05:45:13.573586 moneyflow_base-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      201 2023-05-30 04:53:44.125364 moneyflow_base-0.0.4/requirements.txt
--rw-r--r--   0        0        0      231 2023-05-30 07:30:16.717215 moneyflow_base-0.0.4/settings.py
--rw-r--r--   0        0        0     1395 2023-05-29 18:25:25.194121 moneyflow_base-0.0.4/setup.py
--rw-r--r--   0        0        0     1840 2023-05-29 05:54:44.625161 moneyflow_base-0.0.4/tests/models_test.py
--rw-r--r--   0        0        0     1491 2023-05-29 18:04:30.312916 moneyflow_base-0.0.4/tests/service_test.py
--rw-r--r--   0        0        0     3775 2023-05-29 06:42:45.874857 moneyflow_base-0.0.4/tests/utils_test.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 moneyflow_base-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3090 2023-05-29 05:57:47.185851 moneyflow_base-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1464 2023-06-07 07:15:23.793906 moneyflow_base-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1980 2023-06-07 07:08:12.487713 moneyflow_base-0.0.5/Makefile
+-rw-r--r--   0        0        0       90 2023-05-29 05:54:55.382142 moneyflow_base-0.0.5/README.md
+-rw-r--r--   0        0        0      540 2023-06-07 07:10:28.613627 moneyflow_base-0.0.5/conftest.py
+-rw-r--r--   0        0        0     6148 2022-02-16 17:13:36.168907 moneyflow_base-0.0.5/docs/.DS_Store
+-rw-r--r--   0        0        0      638 2022-02-14 21:51:19.000000 moneyflow_base-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-02-14 21:51:19.000000 moneyflow_base-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0     2258 2023-06-07 07:05:16.364113 moneyflow_base-0.0.5/docs/source/conf.py
+-rw-r--r--   0        0        0      513 2023-05-30 04:52:49.017528 moneyflow_base-0.0.5/docs/source/index.rst
+-rw-r--r--   0        0        0       89 2023-05-30 04:38:20.375048 moneyflow_base-0.0.5/docs/source/mbase/eventlog.rst
+-rw-r--r--   0        0        0       80 2023-05-30 04:52:11.924670 moneyflow_base-0.0.5/docs/source/mbase/services.rst
+-rw-r--r--   0        0        0       65 2023-05-30 04:49:31.167705 moneyflow_base-0.0.5/docs/source/mbase/utils.rst
+-rw-r--r--   0        0        0        0 2023-05-29 05:54:36.692581 moneyflow_base-0.0.5/mbase/__init__.py
+-rw-r--r--   0        0        0     7792 2023-06-04 19:51:09.378892 moneyflow_base-0.0.5/mbase/eventlog.py
+-rw-r--r--   0        0        0      859 2023-05-29 05:54:36.702787 moneyflow_base-0.0.5/mbase/exceptions.py
+-rw-r--r--   0        0        0    21987 2023-05-29 17:52:37.309182 moneyflow_base-0.0.5/mbase/future.py
+-rw-r--r--   0        0        0     1000 2023-06-04 18:29:05.064172 moneyflow_base-0.0.5/mbase/mlogging.py
+-rw-r--r--   0        0        0     7302 2023-05-31 06:00:47.348683 moneyflow_base-0.0.5/mbase/models.py
+-rw-r--r--   0        0        0     3144 2023-05-29 18:02:21.856877 moneyflow_base-0.0.5/mbase/services.py
+-rw-r--r--   0        0        0    10981 2023-05-31 05:36:39.195619 moneyflow_base-0.0.5/mbase/utils.py
+-rw-r--r--   0        0        0      743 2023-06-07 07:29:34.169215 moneyflow_base-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      138 2023-06-04 20:03:44.109836 moneyflow_base-0.0.5/pytest.ini
+-rw-r--r--   0        0        0      206 2023-06-07 07:05:59.131027 moneyflow_base-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1840 2023-05-29 05:54:44.625161 moneyflow_base-0.0.5/tests/models_test.py
+-rw-r--r--   0        0        0     1452 2023-06-04 18:27:21.796606 moneyflow_base-0.0.5/tests/service_test.py
+-rw-r--r--   0        0        0      233 2023-06-07 07:05:41.757111 moneyflow_base-0.0.5/tests/settings.py
+-rw-r--r--   0        0        0     3775 2023-05-29 06:42:45.874857 moneyflow_base-0.0.5/tests/utils_test.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 moneyflow_base-0.0.5/PKG-INFO
```

### Comparing `moneyflow_base-0.0.4/.gitignore` & `moneyflow_base-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/Makefile` & `moneyflow_base-0.0.5/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 pytest = pytest
 py = $$(if [ -d $(PWD)/'venv' ]; then echo $(PWD)/"venv/bin/python3"; else echo "python3"; fi)
 pip = $(py) -m pip
 
 PY_PATHS := $(PWD)
 pypath := python3 -c 'import sys, pathlib as p; print(":".join([str(p.Path(x).resolve()) for x in sys.argv[1:]]))'
 export PYTHONPATH=$(shell $(pypath) $(PY_PATHS))
-export DJANGO_SETTINGS_MODULE=settings
+export DJANGO_SETTINGS_MODULE=tests.settings
 
 .PHONY: test-pypath
 test-pypath: export PYTHONPATH = $(shell $(pypath) $(PY_PATHS))
 test-pypath:
 	@python3 -c 'import sys; print(sys.path)'
```

### Comparing `moneyflow_base-0.0.4/docs/.DS_Store` & `moneyflow_base-0.0.5/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/docs/Makefile` & `moneyflow_base-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/docs/make.bat` & `moneyflow_base-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/docs/source/conf.py` & `moneyflow_base-0.0.5/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 import os
 import sys
 
 import django
 
 sys.path.insert(0, os.path.abspath("../mbase/"))
-os.environ["DJANGO_SETTINGS_MODULE"] = "settings"
+os.environ["DJANGO_SETTINGS_MODULE"] = "tests.settings"
 django.setup()
 
 
 # -- Project information -----------------------------------------------------
 
 project = "Moneyflow Base utilities"
 copyright = "2023"
```

### Comparing `moneyflow_base-0.0.4/docs/source/index.rst` & `moneyflow_base-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/mbase/eventlog.py` & `moneyflow_base-0.0.5/mbase/eventlog.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/mbase/exceptions.py` & `moneyflow_base-0.0.5/mbase/exceptions.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/mbase/future.py` & `moneyflow_base-0.0.5/mbase/future.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/mbase/mlogging.py` & `moneyflow_base-0.0.5/mbase/mlogging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import structlog
-from django.conf import settings
+# from django.conf import settings
 
 
 def mf_get_logger(name):
     if name is None:
         name = "mlog"
     module_name = name.split(".")[0]
-    return structlog.get_logger(f"{settings.SYSTEM_NAME}.{module_name}")
+    # return structlog.get_logger(f"{settings.SYSTEM_NAME}.{module_name}")
+    return structlog.get_logger(f"{module_name}")
 
 
 def trace_logging(*included_safe_kwargs):
     """
     Usage: Decorate your function with
      @trace_logging("is_payer", "amount")
```

### Comparing `moneyflow_base-0.0.4/mbase/models.py` & `moneyflow_base-0.0.5/mbase/models.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/mbase/services.py` & `moneyflow_base-0.0.5/mbase/services.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/mbase/utils.py` & `moneyflow_base-0.0.5/mbase/utils.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/pyproject.toml` & `moneyflow_base-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "moneyflow-base"
-version = "0.0.4"
+version = "0.0.5"
 description = "Moneyflow Base"
 authors = [
   { name = "Team Moneyflow", email = "infrastructure@moneyflow.io" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `moneyflow_base-0.0.4/tests/models_test.py` & `moneyflow_base-0.0.5/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/tests/service_test.py` & `moneyflow_base-0.0.5/tests/service_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-print("PP=", os.environ['PYTHONPATH'])
 
 from mbase.services import BaseService, ObservableMixin, BaseObserver
 from mbase.mlogging import mf_get_logger
 
 logger = mf_get_logger(__name__)
```

### Comparing `moneyflow_base-0.0.4/tests/utils_test.py` & `moneyflow_base-0.0.5/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `moneyflow_base-0.0.4/PKG-INFO` & `moneyflow_base-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyflow-base
-Version: 0.0.4
+Version: 0.0.5
 Summary: Moneyflow Base
 Author-email: Team Moneyflow <infrastructure@moneyflow.io>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

