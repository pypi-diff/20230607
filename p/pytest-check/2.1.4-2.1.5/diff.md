# Comparing `tmp/pytest-check-2.1.4.tar.gz` & `tmp/pytest_check-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-check-2.1.4.tar", last modified: Mon Feb 13 15:16:58 2023, max compression
+gzip compressed data, was "pytest_check-2.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest-check-2.1.4.tar` & `pytest_check-2.1.5.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0     1079 2023-02-13 15:16:49.023448 pytest-check-2.1.4/LICENSE.txt
--rw-r--r--   0        0        0     8651 2023-02-13 15:16:49.023448 pytest-check-2.1.4/README.md
--rw-r--r--   0        0        0     8176 2023-02-13 15:16:49.023448 pytest-check-2.1.4/changelog.md
--rw-r--r--   0        0        0      564 2023-02-13 15:16:49.023448 pytest-check-2.1.4/examples/test_example_alt_names.py
--rw-r--r--   0        0        0      535 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_any_failures.py
--rw-r--r--   0        0        0      187 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_check_and_assert.py
--rw-r--r--   0        0        0      269 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_check_check.py
--rw-r--r--   0        0        0      519 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_check_func_decorator.py
--rw-r--r--   0        0        0      483 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_check_not_in_test.py
--rw-r--r--   0        0        0      724 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_context_functions.py
--rw-r--r--   0        0        0      521 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_context_manager_fail.py
--rw-r--r--   0        0        0      325 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_context_manager_pass.py
--rw-r--r--   0        0        0      331 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_fail_in_fixture.py
--rw-r--r--   0        0        0     1536 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_functions_fail.py
--rw-r--r--   0        0        0     1718 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_functions_pass.py
--rw-r--r--   0        0        0      358 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_helpers.py
--rw-r--r--   0        0        0      772 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_httpx.py
--rw-r--r--   0        0        0     1175 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_logging.py
--rw-r--r--   0        0        0      769 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_maxfail.py
--rw-r--r--   0        0        0      185 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_message.py
--rw-r--r--   0        0        0      413 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_mix_checks_and_assertions.py
--rw-r--r--   0        0        0      118 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_multiple_failures.py
--rw-r--r--   0        0        0      487 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_raises.py
--rw-r--r--   0        0        0      208 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_simple.py
--rw-r--r--   0        0        0      421 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_speedup_funcs.py
--rw-r--r--   0        0        0      604 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_stop_on_fail.py
--rw-r--r--   0        0        0      358 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_tb_style.py
--rw-r--r--   0        0        0     1101 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_traceback.py
--rw-r--r--   0        0        0      502 2023-02-13 15:16:49.027448 pytest-check-2.1.4/examples/test_example_xfail.py
--rw-r--r--   0        0        0      857 2023-02-13 15:16:49.027448 pytest-check-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     1519 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/__init__.py
--rw-r--r--   0        0        0     5081 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/check_functions.py
--rw-r--r--   0        0        0     1602 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/check_log.py
--rw-r--r--   0        0        0     3831 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/check_raises.py
--rw-r--r--   0        0        0     1551 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/context_manager.py
--rw-r--r--   0        0        0     3363 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/plugin.py
--rw-r--r--   0        0        0     1432 2023-02-13 15:16:49.027448 pytest-check-2.1.4/src/pytest_check/pseudo_traceback.py
--rw-r--r--   0        0        0        0 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/conftest.py
--rw-r--r--   0        0        0      600 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_alt_names.py
--rw-r--r--   0        0        0      986 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_any_failures.py
--rw-r--r--   0        0        0      229 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_check_and_assert.py
--rw-r--r--   0        0        0      179 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_check_check.py
--rw-r--r--   0        0        0     1061 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_check_context_manager.py
--rw-r--r--   0        0        0       53 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_check_fixture.py
--rw-r--r--   0        0        0      740 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_check_func_decorator.py
--rw-r--r--   0        0        0      536 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_fail_in_fixture.py
--rw-r--r--   0        0        0      392 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_functions.py
--rw-r--r--   0        0        0     1522 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_helpers.py
--rw-r--r--   0        0        0     1352 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_logging.py
--rw-r--r--   0        0        0     1036 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_maxfail.py
--rw-r--r--   0        0        0      505 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_message.py
--rw-r--r--   0        0        0     1018 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_not_in_test.py
--rw-r--r--   0        0        0     5413 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_raises.py
--rw-r--r--   0        0        0      860 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_red.py
--rw-r--r--   0        0        0     2500 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_speedup_flags.py
--rw-r--r--   0        0        0     2647 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_speedup_functions.py
--rw-r--r--   0        0        0      924 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_stop_on_fail.py
--rw-r--r--   0        0        0      713 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_tb_style.py
--rw-r--r--   0        0        0     1018 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tests/test_xfail.py
--rw-r--r--   0        0        0      867 2023-02-13 15:16:49.027448 pytest-check-2.1.4/tox.ini
--rw-r--r--   0        0        0     9266 1970-01-01 00:00:00.000000 pytest-check-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-06 21:59:29.997499 pytest_check-2.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     8651 2023-06-06 21:59:29.997499 pytest_check-2.1.5/README.md
+-rw-r--r--   0        0        0     8369 2023-06-06 21:59:29.997499 pytest_check-2.1.5/changelog.md
+-rw-r--r--   0        0        0      564 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_alt_names.py
+-rw-r--r--   0        0        0      535 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_any_failures.py
+-rw-r--r--   0        0        0      187 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_and_assert.py
+-rw-r--r--   0        0        0      269 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_check.py
+-rw-r--r--   0        0        0      519 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_func_decorator.py
+-rw-r--r--   0        0        0      483 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_check_not_in_test.py
+-rw-r--r--   0        0        0      724 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_context_functions.py
+-rw-r--r--   0        0        0      521 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_context_manager_fail.py
+-rw-r--r--   0        0        0      325 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_context_manager_pass.py
+-rw-r--r--   0        0        0      331 2023-06-06 21:59:29.997499 pytest_check-2.1.5/examples/test_example_fail_in_fixture.py
+-rw-r--r--   0        0        0      448 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_fail_in_thread.py
+-rw-r--r--   0        0        0     1536 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_functions_fail.py
+-rw-r--r--   0        0        0     1718 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_functions_pass.py
+-rw-r--r--   0        0        0      358 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_helpers.py
+-rw-r--r--   0        0        0      772 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_httpx.py
+-rw-r--r--   0        0        0     1175 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_logging.py
+-rw-r--r--   0        0        0      769 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_maxfail.py
+-rw-r--r--   0        0        0      185 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_message.py
+-rw-r--r--   0        0        0      413 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_mix_checks_and_assertions.py
+-rw-r--r--   0        0        0      118 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_multiple_failures.py
+-rw-r--r--   0        0        0      384 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_pass_in_thread.py
+-rw-r--r--   0        0        0      487 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_raises.py
+-rw-r--r--   0        0        0      208 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_simple.py
+-rw-r--r--   0        0        0      421 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_speedup_funcs.py
+-rw-r--r--   0        0        0      604 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_stop_on_fail.py
+-rw-r--r--   0        0        0      358 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_tb_style.py
+-rw-r--r--   0        0        0     1101 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_traceback.py
+-rw-r--r--   0        0        0      502 2023-06-06 21:59:30.001499 pytest_check-2.1.5/examples/test_example_xfail.py
+-rw-r--r--   0        0        0      685 2023-06-06 21:59:30.001499 pytest_check-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/__init__.py
+-rw-r--r--   0        0        0     5081 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/check_functions.py
+-rw-r--r--   0        0        0     1602 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/check_log.py
+-rw-r--r--   0        0        0     3831 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/check_raises.py
+-rw-r--r--   0        0        0     1551 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/context_manager.py
+-rw-r--r--   0        0        0     3363 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/plugin.py
+-rw-r--r--   0        0        0     1493 2023-06-06 21:59:30.001499 pytest_check-2.1.5/src/pytest_check/pseudo_traceback.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      600 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_alt_names.py
+-rw-r--r--   0        0        0      986 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_any_failures.py
+-rw-r--r--   0        0        0      229 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_and_assert.py
+-rw-r--r--   0        0        0      179 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_check.py
+-rw-r--r--   0        0        0     1061 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_context_manager.py
+-rw-r--r--   0        0        0       53 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_fixture.py
+-rw-r--r--   0        0        0      740 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_check_func_decorator.py
+-rw-r--r--   0        0        0      536 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_fail_in_fixture.py
+-rw-r--r--   0        0        0      392 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_functions.py
+-rw-r--r--   0        0        0     1522 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_helpers.py
+-rw-r--r--   0        0        0     1352 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_logging.py
+-rw-r--r--   0        0        0     1036 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_maxfail.py
+-rw-r--r--   0        0        0      505 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_message.py
+-rw-r--r--   0        0        0     1018 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_not_in_test.py
+-rw-r--r--   0        0        0     5413 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_raises.py
+-rw-r--r--   0        0        0      860 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_red.py
+-rw-r--r--   0        0        0     2500 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_speedup_flags.py
+-rw-r--r--   0        0        0     2647 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_speedup_functions.py
+-rw-r--r--   0        0        0      924 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_stop_on_fail.py
+-rw-r--r--   0        0        0      713 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_tb_style.py
+-rw-r--r--   0        0        0      508 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_thread.py
+-rw-r--r--   0        0        0     1018 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tests/test_xfail.py
+-rw-r--r--   0        0        0      859 2023-06-06 21:59:30.001499 pytest_check-2.1.5/tox.ini
+-rw-r--r--   0        0        0     9018 1970-01-01 00:00:00.000000 pytest_check-2.1.5/PKG-INFO
```

### Comparing `pytest-check-2.1.4/LICENSE.txt` & `pytest_check-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/README.md` & `pytest_check-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/changelog.md` & `pytest_check-2.1.5/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 - nothing so far
 
 ### Changed
 
 - nothing so far
 
 -->
+
+## [2.1.5] - 2023-June-6
+
+### Fixed
+
+- Fix [127](https://github.com/okken/pytest-check/issues/127) IndexError when running a check in a thread -  Thanks [fperrin](https://github.com/fperrin)
+
 ## [2.1.4] - 2023-Feb-13
 
 ### Added
 
 - include tests an examples in sdist -  [pr 121](https://github.com/okken/pytest-check/pull/121)
 
 ## [2.1.3] - 2023-Feb-9
```

### Comparing `pytest-check-2.1.4/examples/test_example_alt_names.py` & `pytest_check-2.1.5/examples/test_example_alt_names.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_any_failures.py` & `pytest_check-2.1.5/examples/test_example_any_failures.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_check_func_decorator.py` & `pytest_check-2.1.5/examples/test_example_check_func_decorator.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_context_functions.py` & `pytest_check-2.1.5/examples/test_example_context_functions.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_context_manager_fail.py` & `pytest_check-2.1.5/examples/test_example_context_manager_fail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_functions_fail.py` & `pytest_check-2.1.5/examples/test_example_functions_fail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_functions_pass.py` & `pytest_check-2.1.5/examples/test_example_functions_pass.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_httpx.py` & `pytest_check-2.1.5/examples/test_example_httpx.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_logging.py` & `pytest_check-2.1.5/examples/test_example_logging.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_maxfail.py` & `pytest_check-2.1.5/examples/test_example_maxfail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_stop_on_fail.py` & `pytest_check-2.1.5/examples/test_example_stop_on_fail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/examples/test_example_traceback.py` & `pytest_check-2.1.5/examples/test_example_traceback.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/src/pytest_check/__init__.py` & `pytest_check-2.1.5/src/pytest_check/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-"""A pytest plugin that allows multiple failures per test."""
-__version__ = "2.1.4"
-
 import pytest
 
 # make sure assert rewriting happens
 pytest.register_assert_rewrite("pytest_check.check_functions")
 
 # allow for top level helper function access:
 # import pytest_check
```

### Comparing `pytest-check-2.1.4/src/pytest_check/check_functions.py` & `pytest_check-2.1.5/src/pytest_check/check_functions.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/src/pytest_check/check_log.py` & `pytest_check-2.1.5/src/pytest_check/check_log.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/src/pytest_check/check_raises.py` & `pytest_check-2.1.5/src/pytest_check/check_raises.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/src/pytest_check/context_manager.py` & `pytest_check-2.1.5/src/pytest_check/context_manager.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/src/pytest_check/plugin.py` & `pytest_check-2.1.5/src/pytest_check/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/src/pytest_check/pseudo_traceback.py` & `pytest_check-2.1.5/src/pytest_check/pseudo_traceback.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 
 _traceback_style = "auto"
 
 
-def get_full_context(level):
-    (_, filename, line, funcname, contextlist) = inspect.stack()[level][0:5]
+def get_full_context(frame):
+    (_, filename, line, funcname, contextlist) = frame[0:5]
     try:
         filename = os.path.relpath(filename)
     except ValueError:  # pragma: no cover
         # this is necessary if we're tracing to a different drive letter
         # such as C: to D:
         #
         # Turning off coverage for abspath, for now,
@@ -24,23 +24,23 @@
     """
     built traceback styles for better error message
     only supports no
     """
     if _traceback_style == "no":
         return ""
 
-    level = 4
+    skip_own_frames = 3
     pseudo_trace = []
     func = ""
-    while "test_" not in func:
-        (file, line, func, context) = get_full_context(level)
+    context_stack = inspect.stack()[skip_own_frames:]
+    while "test_" not in func and context_stack:
+        (file, line, func, context) = get_full_context(context_stack.pop(0))
         # we want to trace through user code, not 3rd party or builtin libs
         if "site-packages" in file:
             break
         # if called outside of a test, we might hit this
         if "<module>" in func:
             break
         line = f"{file}:{line} in {func}() -> {context}"
         pseudo_trace.append(line)
-        level += 1
 
     return "\n".join(reversed(pseudo_trace)) + "\n"
```

### Comparing `pytest-check-2.1.4/tests/test_alt_names.py` & `pytest_check-2.1.5/tests/test_alt_names.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_any_failures.py` & `pytest_check-2.1.5/tests/test_any_failures.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_check_context_manager.py` & `pytest_check-2.1.5/tests/test_check_context_manager.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_check_func_decorator.py` & `pytest_check-2.1.5/tests/test_check_func_decorator.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_fail_in_fixture.py` & `pytest_check-2.1.5/tests/test_fail_in_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_helpers.py` & `pytest_check-2.1.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_logging.py` & `pytest_check-2.1.5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_maxfail.py` & `pytest_check-2.1.5/tests/test_maxfail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_not_in_test.py` & `pytest_check-2.1.5/tests/test_not_in_test.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_raises.py` & `pytest_check-2.1.5/tests/test_raises.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_red.py` & `pytest_check-2.1.5/tests/test_red.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_speedup_flags.py` & `pytest_check-2.1.5/tests/test_speedup_flags.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_speedup_functions.py` & `pytest_check-2.1.5/tests/test_speedup_functions.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_stop_on_fail.py` & `pytest_check-2.1.5/tests/test_stop_on_fail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_tb_style.py` & `pytest_check-2.1.5/tests/test_tb_style.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/tests/test_xfail.py` & `pytest_check-2.1.5/tests/test_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest-check-2.1.4/PKG-INFO` & `pytest_check-2.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: pytest-check
-Version: 2.1.4
+Version: 2.1.5
 Summary: A pytest plugin that allows multiple failures per test.
 Author: Brian Okken
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
-Classifier: Topic :: Software Development :: Testing
 Requires-Dist: pytest
 Project-URL: Home, https://github.com/okken/pytest-check
 
 # pytest-check
 
 A pytest plugin that allows multiple failures per test.
```

