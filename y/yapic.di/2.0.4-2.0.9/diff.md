# Comparing `tmp/yapic.di-2.0.4.tar.gz` & `tmp/yapic.di-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yapic.di-2.0.4.tar", last modified: Fri Mar  5 16:25:28 2021, max compression
+gzip compressed data, was "yapic.di-2.0.9.tar", last modified: Tue Sep 27 12:22:54 2022, max compression
```

## Comparing `yapic.di-2.0.4.tar` & `yapic.di-2.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1516 2021-03-05 16:25:21.000000 yapic.di-2.0.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2021-03-05 16:25:21.000000 yapic.di-2.0.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5527 2021-03-05 16:25:28.000000 yapic.di-2.0.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3620 2021-03-05 16:25:21.000000 yapic.di-2.0.4/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/yapic.core/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/yapic.core/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/common.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8434 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/module.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/pyptr.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    20393 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/string-builder.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3683 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/thread.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    19507 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/type.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    50584 2021-03-05 16:25:23.000000 yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/typing.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-05 16:25:28.000000 yapic.di-2.0.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4899 2021-03-05 16:25:21.000000 yapic.di-2.0.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3869 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/_di.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/di.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10583 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/di.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/errors.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      759 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/inject.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27647 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/injectable.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6361 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/injector.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2806 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/kwonly.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6532 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/resolver.hpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3125 2021-03-05 16:25:21.000000 yapic.di-2.0.4/src/token.hpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-05 16:25:28.000000 yapic.di-2.0.4/yapic.di.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5527 2021-03-05 16:25:28.000000 yapic.di-2.0.4/yapic.di.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      756 2021-03-05 16:25:28.000000 yapic.di-2.0.4/yapic.di.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-05 16:25:28.000000 yapic.di-2.0.4/yapic.di.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-03-05 16:25:28.000000 yapic.di-2.0.4/yapic.di.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-03-05 16:25:28.000000 yapic.di-2.0.4/yapic.di.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.384820 yapic.di-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-09-27 12:22:45.000000 yapic.di-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-09-27 12:22:45.000000 yapic.di-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-09-27 12:22:54.384820 yapic.di-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3620 2022-09-27 12:22:45.000000 yapic.di-2.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.376820 yapic.di-2.0.9/libs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.376820 yapic.di-2.0.9/libs/yapic.core/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.376820 yapic.di-2.0.9/libs/yapic.core/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.376820 yapic.di-2.0.9/libs/yapic.core/src/yapic/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.376820 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.376820 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.380820 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/
+-rw-r--r--   0 runner    (1001) docker     (121)      783 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/module.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/pyptr.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    20346 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/string-builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/thread.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    19513 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    50965 2022-09-27 12:22:46.000000 yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/typing.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 12:22:54.388820 yapic.di-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-09-27 12:22:45.000000 yapic.di-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.384820 yapic.di-2.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3869 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/_di.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/di.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10584 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/di.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/errors.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/inject.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27646 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/injectable.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6361 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/injector.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/kwonly.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6532 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/resolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-09-27 12:22:45.000000 yapic.di-2.0.9/src/token.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 12:22:54.384820 yapic.di-2.0.9/yapic.di.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-09-27 12:22:54.000000 yapic.di-2.0.9/yapic.di.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-27 12:22:54.000000 yapic.di-2.0.9/yapic.di.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 12:22:54.000000 yapic.di-2.0.9/yapic.di.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-27 12:22:54.000000 yapic.di-2.0.9/yapic.di.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-27 12:22:54.000000 yapic.di-2.0.9/yapic.di.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yapic.di-2.0.4/LICENSE` & `yapic.di-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/PKG-INFO` & `yapic.di-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapic.di
-Version: 2.0.4
+Version: 2.0.9
 Summary: Very fast Dependency Injection library
 Home-page: https://github.com/zozzz/yapic.di
 Author: Zoltán Vetési
 Author-email: vetesi.zoltan@gmail.com
 License: BSD
 Description: Dependency Injector
         ===================
```

### Comparing `yapic.di-2.0.4/README.rst` & `yapic.di-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/common.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/common.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/module.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/module.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/pyptr.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/pyptr.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/string-builder.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/string-builder.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,14 @@
 	static inline void AppendAscii(Memory& mem, Input ch) {
 		assert(ch <= 127);
 		*(mem.cursor++) = ch;
 	}
 
 	template<typename Memory, typename Input>
 	static inline void AppendChar(Memory& mem, Input ch) {
-		assert(sizeof(Memory::DT) >= sizeof(Input));
 		*(mem.cursor++) = ch;
 	}
 
 	template<typename Memory, typename Mc>
 	static inline bool AppendString(Memory& mem, PyObject* obj, Mc& maxchar) {
 		unsigned int kind = (unsigned int)PyUnicode_KIND(obj);
 		maxchar |= PyUnicode_MAX_CHAR_VALUE(obj);
```

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/thread.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/thread.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/type.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/type.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -393,15 +393,15 @@
 			static inline const PyTypeObject* PyType() {
 				static const PyTypeObject type = {
 					PyVarObject_HEAD_INIT(NULL, 0)
 					/* tp_name */ 			Self::Name(),
 					/* tp_basicsize */ 		sizeof(Self),
 					/* tp_itemsize */ 		static_cast<Py_ssize_t>(0),
 					/* tp_dealloc */ 		(destructor) Yapic_GetTypeMethod(Self, __dealloc__),
-					/* tp_print */ 			NULL,
+					/* tp_vectorcall_offset */ 0,
 					/* tp_getattr */ 		Yapic_GetTypeMethod(Self, __getattr__),
 					/* tp_setattr */ 		Yapic_GetTypeMethod(Self, __setattr__),
 					/* tp_as_async */ 		NULL,
 					/* tp_repr */ 			Yapic_GetTypeMethod(Self, __repr__),
 					/* tp_as_number */ 		Yapic_TypeHasNumberMethods(Self) ? Self::_NumberMethods() : NULL,
 					/* tp_as_sequence */ 	Yapic_TypeHasSequenceMethods(Self) ? Self::_SequenceMethods() : NULL,
 					/* tp_as_mapping */ 	Yapic_TypeHasMappingMethods(Self) ? Self::_MappingMethods() : NULL,
```

### Comparing `yapic.di-2.0.4/libs/yapic.core/src/yapic/core/include/yapic/typing.hpp` & `yapic.di-2.0.9/libs/yapic.core/src/yapic/core/include/yapic/typing.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #define D57C95BE_1134_1461_11A3_990B2EDF5491
 
 #include <Python.h>
 #include <memory>
 #include "./pyptr.hpp"
 
 
-#define YapicTyping_REPR(o) (((PyObject*)o) == NULL ? "<NULL>" : ((char*) PyUnicode_DATA(PyObject_Repr(((PyObject*)o)))))
+#define YapicTyping_REPR(o) (((PyObject*)o) == NULL ? "<NULL>" : ((char*) PyUnicode_DATA(PyObject_ASCII(((PyObject*)o)))))
 #define YapicTyping_DUMP(o) printf(#o " = %s\n", YapicTyping_REPR(o))
 
 
 #define Yapic_Typing_ImportFromTyping(into, name) \
     into = PyObject_GetAttrString(_typing, name); \
     if (into == NULL) { \
         return false; \
@@ -1044,18 +1044,27 @@
                 }
 
                 PyPtr<PyTupleObject> result(PyTuple_New(2));
                 if (result.IsNull()) {
                     return NULL;
                 }
 
-                PyObject* annots = PyFunction_GET_ANNOTATIONS(func);
-                if (annots != NULL) {
-                    assert(PyDict_CheckExact(annots));
-                }
+                // version >= 3.10
+                #if PY_VERSION_HEX >= 0x030A0000
+                    // Már tuple nem dict
+                    PyPtr<> annots = PyObject_GetAttr((PyObject*) func, __annotations__);
+                    if (annots.IsNull()) {
+                        return NULL;
+                    }
+                #else
+                    PyObject* annots = PyFunction_GET_ANNOTATIONS(func);
+                    if (annots != NULL) {
+                        assert(PyDict_CheckExact(annots));
+                    }
+                #endif
 
                 PyPtr<PyTupleObject> args;
                 PyPtr<PyTupleObject> keywords;
                 PyObject* defaults;
                 PyObject* argName;
                 PyObject* argType;
                 PyObject* argDef;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yapic.di-2.0.4/setup.py` & `yapic.di-2.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-#!/usr/bin/env python3
-
-import os
 import sys
 from glob import glob
 from os import path
 from pathlib import Path
-from setuptools import setup, Extension
+
+from setuptools import Command, Extension, setup
 from setuptools.command.test import test as TestCommand
-from setuptools import Command
 
-VERSION = "2.0.4"
+VERSION = "2.0.9"
 
 define_macros = {
     "YAPIC_DI_VERSION_MAJOR": VERSION.split(".")[0],
     "YAPIC_DI_VERSION_MINOR": VERSION.split(".")[1],
-    "YAPIC_DI_VERSION_PATCH": VERSION.split(".")[2]
+    "YAPIC_DI_VERSION_PATCH": VERSION.split(".")[2],
 }
 undef_macros = []
 extra_compile_args = []  # -flto
 
 subcommand_args = []
 if "--" in sys.argv:
-    subcommand_args = sys.argv[sys.argv.index("--") + 1:]
-    del sys.argv[sys.argv.index("--"):]
+    subcommand_args = sys.argv[sys.argv.index("--") + 1 :]  # noqa
+    del sys.argv[sys.argv.index("--") :]  # noqa
 
 if sys.platform == "win32":
     define_macros["UNICODE"] = "1"
 
     DEVELOP = sys.executable.endswith("python_d.exe")
     if DEVELOP:
         define_macros["_DEBUG"] = "1"
@@ -109,14 +106,15 @@
             yield dist.tests_require
 
         cmd_prerun(self, requirements)
         self.run_tests()
 
     def run_tests(self):
         import pytest
+
         errno = pytest.main(subcommand_args)
         sys.exit(errno)
 
 
 class Benchmark(Command):
     user_options = [
         ("file=", "f", "File to run"),
@@ -132,15 +130,17 @@
 
     def run(self):
         def requirements(dist):
             yield dist.extras_require["benchmark"]
 
         cmd_prerun(self, requirements)
         import shlex
+
         import pytest
+
         errno = pytest.main(shlex.split(self.pytest_args))
         sys.exit(errno)
 
 
 # typing: https://github.com/python/typing/issues/84
 setup(
     name="yapic.di",
@@ -154,18 +154,15 @@
     packages=["yapic.di"],
     package_dir={"yapic.di": "src"},
     package_data={"yapic.di": ["_di.pyi"]},
     ext_modules=[cpp_ext],
     tests_require=["pytest", "pytest-leaks"],
     python_requires=">=3.7",
     extras_require={"benchmark": ["pytest", "pytest-benchmark"]},
-    cmdclass={
-        "test": PyTest,
-        "bench": Benchmark
-    },
+    cmdclass={"test": PyTest, "bench": Benchmark},
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
         "Programming Language :: C++",
         "Programming Language :: Python :: 3.7",
```

### Comparing `yapic.di-2.0.4/src/_di.pyi` & `yapic.di-2.0.9/src/_di.pyi`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/src/di.hpp` & `yapic.di-2.0.9/src/di.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #define YAPIC_DI_VERSION \
 	YapicDI_STR(YAPIC_DI_VERSION_MAJOR) "." \
 	YapicDI_STR(YAPIC_DI_VERSION_MINOR) "." \
 	YapicDI_STR(YAPIC_DI_VERSION_PATCH)
 
 // USE ONLY FOR DEBUGGING
-#define YapicDI_REPR(o) (((PyObject*)o) == NULL ? "<NULL>" : ((char*) PyUnicode_DATA(PyObject_Repr(((PyObject*)o)))))
+#define YapicDI_REPR(o) (((PyObject*)o) == NULL ? "<NULL>" : ((char*) PyUnicode_DATA(PyObject_ASCII(((PyObject*)o)))))
 #define YapicDI_DUMP(o) printf(#o " = %s\n", YapicDI_REPR(o))
 
 #define YapicDI_MAX_RECURSION 1000
 
 #ifdef _MSC_VER
 #	define FORCEINLINE __forceinline
 #elif defined(__GNUC__)
```

### Comparing `yapic.di-2.0.4/src/errors.hpp` & `yapic.di-2.0.9/src/errors.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/src/inject.py` & `yapic.di-2.0.9/src/inject.py`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/src/injectable.hpp` & `yapic.di-2.0.9/src/injectable.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 		static PyObject* Arguments(PyObject* hints) {
 			Py_ssize_t l = PyTuple_GET_SIZE(hints);
 			PyPtr<PyTupleObject> args = PyTuple_New(l);
 			if (!args) {
 				return NULL;
 			}
 
-
 			PyObject* entry;
 			PyObject* argName;
 			PyObject* argType;
 			PyObject* argDef;
 			PyObject* resolver;
 			for (Py_ssize_t i = 0; i < l; ++i) {
 				entry = PyTuple_GET_ITEM(hints, i);
```

### Comparing `yapic.di-2.0.4/src/injector.hpp` & `yapic.di-2.0.9/src/injector.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/src/kwonly.hpp` & `yapic.di-2.0.9/src/kwonly.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/src/resolver.hpp` & `yapic.di-2.0.9/src/resolver.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/src/token.hpp` & `yapic.di-2.0.9/src/token.hpp`

 * *Files identical despite different names*

### Comparing `yapic.di-2.0.4/yapic.di.egg-info/PKG-INFO` & `yapic.di-2.0.9/yapic.di.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapic.di
-Version: 2.0.4
+Version: 2.0.9
 Summary: Very fast Dependency Injection library
 Home-page: https://github.com/zozzz/yapic.di
 Author: Zoltán Vetési
 Author-email: vetesi.zoltan@gmail.com
 License: BSD
 Description: Dependency Injector
         ===================
```

### Comparing `yapic.di-2.0.4/yapic.di.egg-info/SOURCES.txt` & `yapic.di-2.0.9/yapic.di.egg-info/SOURCES.txt`

 * *Files identical despite different names*

