# Comparing `tmp/docstring-inheritance-2.0.0.tar.gz` & `tmp/docstring-inheritance-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring-inheritance-2.0.0.tar", last modified: Wed Jun  7 19:16:18 2023, max compression
+gzip compressed data, was "docstring-inheritance-2.0.0rc0.tar", last modified: Tue Jun  6 19:37:59 2023, max compression
```

## Comparing `docstring-inheritance-2.0.0.tar` & `docstring-inheritance-2.0.0rc0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.768190 docstring-inheritance-2.0.0/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.763190 docstring-inheritance-2.0.0/.github/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.765190 docstring-inheritance-2.0.0/.github/workflows/
--rw-r--r--   0 ad        (1000) ad        (1000)      905 2023-06-07 09:55:33.000000 docstring-inheritance-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 ad        (1000) ad        (1000)       69 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/.gitignore
--rw-r--r--   0 ad        (1000) ad        (1000)     2044 2023-06-07 09:55:33.000000 docstring-inheritance-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 ad        (1000) ad        (1000)     1682 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/CHANGELOG.md
--rw-r--r--   0 ad        (1000) ad        (1000)     1264 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/CREDITS.md
--rw-r--r--   0 ad        (1000) ad        (1000)     1056 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/LICENSE.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.763190 docstring-inheritance-2.0.0/LICENSES/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.765190 docstring-inheritance-2.0.0/LICENSES/headers/
--rw-r--r--   0 ad        (1000) ad        (1000)      284 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/LICENSES/headers/CC-BY-4.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     1056 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/LICENSES/headers/MIT.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     9718 2023-06-07 19:16:18.768190 docstring-inheritance-2.0.0/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     8689 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/README.md
--rw-r--r--   0 ad        (1000) ad        (1000)     1343 2023-06-07 09:55:33.000000 docstring-inheritance-2.0.0/pyproject.toml
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.765190 docstring-inheritance-2.0.0/requirements/
--rw-r--r--   0 ad        (1000) ad        (1000)      605 2023-06-07 09:55:33.000000 docstring-inheritance-2.0.0/requirements/test.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      178 2023-06-07 19:16:18.769190 docstring-inheritance-2.0.0/setup.cfg
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.763190 docstring-inheritance-2.0.0/src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.765190 docstring-inheritance-2.0.0/src/docstring_inheritance/
--rw-r--r--   0 ad        (1000) ad        (1000)     3969 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5703 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/class_docstrings_inheritor.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.767190 docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/
--rw-r--r--   0 ad        (1000) ad        (1000)     1126 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)    12727 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/base.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3205 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/google.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2939 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/numpy.py
--rw-r--r--   0 ad        (1000) ad        (1000)        0 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/src/docstring_inheritance/py.typed
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.766190 docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/
--rw-r--r--   0 ad        (1000) ad        (1000)     9718 2023-06-07 19:16:18.000000 docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     1010 2023-06-07 19:16:18.000000 docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/SOURCES.txt
--rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-06-07 19:16:18.000000 docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/dependency_links.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       38 2023-06-07 19:16:18.000000 docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/requires.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       22 2023-06-07 19:16:18.000000 docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/top_level.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-07 19:16:18.768190 docstring-inheritance-2.0.0/tests/
--rw-r--r--   0 ad        (1000) ad        (1000)     9586 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/tests/test_base_inheritor.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4867 2023-06-07 09:55:33.000000 docstring-inheritance-2.0.0/tests/test_google_inheritor.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3690 2023-03-09 22:15:51.000000 docstring-inheritance-2.0.0/tests/test_inheritance_for_functions.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4320 2023-06-07 19:08:23.000000 docstring-inheritance-2.0.0/tests/test_metaclass_google.py
--rw-r--r--   0 ad        (1000) ad        (1000)     9165 2023-06-07 09:55:33.000000 docstring-inheritance-2.0.0/tests/test_metaclass_numpy.py
--rw-r--r--   0 ad        (1000) ad        (1000)     6869 2023-06-07 12:04:08.000000 docstring-inheritance-2.0.0/tests/test_numpy_inheritor.py
--rw-r--r--   0 ad        (1000) ad        (1000)      772 2023-06-07 19:15:20.000000 docstring-inheritance-2.0.0/tox.ini
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.157869 docstring-inheritance-2.0.0rc0/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.140432 docstring-inheritance-2.0.0rc0/.github/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.146582 docstring-inheritance-2.0.0rc0/.github/workflows/
+-rw-r--r--   0 antoine    (502) staff       (20)      905 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/.github/workflows/tests.yml
+-rw-r--r--   0 antoine    (502) staff       (20)       69 2023-01-15 15:15:57.000000 docstring-inheritance-2.0.0rc0/.gitignore
+-rw-r--r--   0 antoine    (502) staff       (20)     2044 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0 antoine    (502) staff       (20)     1514 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/CHANGELOG.md
+-rw-r--r--   0 antoine    (502) staff       (20)     1264 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/CREDITS.md
+-rw-r--r--   0 antoine    (502) staff       (20)     1056 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/LICENSE.txt
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.140920 docstring-inheritance-2.0.0rc0/LICENSES/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.147691 docstring-inheritance-2.0.0rc0/LICENSES/headers/
+-rw-r--r--   0 antoine    (502) staff       (20)      284 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/LICENSES/headers/CC-BY-4.0.txt
+-rw-r--r--   0 antoine    (502) staff       (20)     1056 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/LICENSES/headers/MIT.txt
+-rw-r--r--   0 antoine    (502) staff       (20)     9721 2023-06-06 19:37:59.158204 docstring-inheritance-2.0.0rc0/PKG-INFO
+-rw-r--r--   0 antoine    (502) staff       (20)     8689 2023-06-05 21:34:25.000000 docstring-inheritance-2.0.0rc0/README.md
+-rw-r--r--   0 antoine    (502) staff       (20)     1343 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/pyproject.toml
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.148146 docstring-inheritance-2.0.0rc0/requirements/
+-rw-r--r--   0 antoine    (502) staff       (20)      605 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/requirements/test.txt
+-rw-r--r--   0 antoine    (502) staff       (20)      178 2023-06-06 19:37:59.159365 docstring-inheritance-2.0.0rc0/setup.cfg
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.141880 docstring-inheritance-2.0.0rc0/src/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.149396 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/
+-rw-r--r--   0 antoine    (502) staff       (20)     3969 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/__init__.py
+-rw-r--r--   0 antoine    (502) staff       (20)     5609 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/class_docstrings_inheritor.py
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.154256 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/
+-rw-r--r--   0 antoine    (502) staff       (20)     1126 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/__init__.py
+-rw-r--r--   0 antoine    (502) staff       (20)    12515 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/base.py
+-rw-r--r--   0 antoine    (502) staff       (20)     3212 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/google.py
+-rw-r--r--   0 antoine    (502) staff       (20)     2892 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/numpy.py
+-rw-r--r--   0 antoine    (502) staff       (20)        0 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/py.typed
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.152145 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/
+-rw-r--r--   0 antoine    (502) staff       (20)     9721 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (502) staff       (20)     1010 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (502) staff       (20)        1 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (502) staff       (20)       38 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/requires.txt
+-rw-r--r--   0 antoine    (502) staff       (20)       22 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/top_level.txt
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.157401 docstring-inheritance-2.0.0rc0/tests/
+-rw-r--r--   0 antoine    (502) staff       (20)     8874 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_base_inheritor.py
+-rw-r--r--   0 antoine    (502) staff       (20)     4867 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_google_inheritor.py
+-rw-r--r--   0 antoine    (502) staff       (20)     3690 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/tests/test_inheritance_for_functions.py
+-rw-r--r--   0 antoine    (502) staff       (20)     3897 2023-06-05 21:34:25.000000 docstring-inheritance-2.0.0rc0/tests/test_metaclass_google.py
+-rw-r--r--   0 antoine    (502) staff       (20)     9165 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_metaclass_numpy.py
+-rw-r--r--   0 antoine    (502) staff       (20)     6885 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_numpy_inheritor.py
+-rw-r--r--   0 antoine    (502) staff       (20)      772 2023-06-06 19:37:11.000000 docstring-inheritance-2.0.0rc0/tox.ini
```

### Comparing `docstring-inheritance-2.0.0/.github/workflows/tests.yml` & `docstring-inheritance-2.0.0rc0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/.pre-commit-config.yaml` & `docstring-inheritance-2.0.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/CHANGELOG.md` & `docstring-inheritance-2.0.0rc0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [2.0.0] - 2023-06
+## [2.0.0rc0] - 2023-06
 ### Changed
 - Docstring inheritance for methods only inherit from the first found parent.
-- For the Numpy style, the section `OtherParameters` is no longer processed against the arguments of the signature.
 ### Fixed
 - Docstring inheritance for methods with no argument descriptions.
 - Format of the arguments provided with the default description for the Numpy style.
-- Docstring inheritance for methods with no arguments.
 
 ## [1.1.1] - 2023-01
 ### Fixed
 - Docstring inheritance for methods with multiple parents.
 
 ## [1.1.0] - 2023-01
 ### Added
```

### Comparing `docstring-inheritance-2.0.0/CREDITS.md` & `docstring-inheritance-2.0.0rc0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/LICENSE.txt` & `docstring-inheritance-2.0.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/LICENSES/headers/MIT.txt` & `docstring-inheritance-2.0.0rc0/LICENSES/headers/MIT.txt`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/PKG-INFO` & `docstring-inheritance-2.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstring-inheritance
-Version: 2.0.0
+Version: 2.0.0rc0
 Summary: Avoid writing and maintaining duplicated docstrings.
 Author: Antoine Dechaume
 License: MIT
 Project-URL: Documentation, https://antoined.github.io/docstring-inheritance
 Project-URL: Homepage, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Source, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Tracker, https://github.com/AntoineD/docstring-inheritance/issues
```

### Comparing `docstring-inheritance-2.0.0/README.md` & `docstring-inheritance-2.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/pyproject.toml` & `docstring-inheritance-2.0.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/requirements/test.txt` & `docstring-inheritance-2.0.0rc0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance/__init__.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/__init__.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance/class_docstrings_inheritor.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/class_docstrings_inheritor.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,14 @@
                 if parent_method is not None:
                     parent_doc = parent_method.__doc__
                     if parent_doc is not None:
                         self._docstring_inheritor(parent_doc, attr)
                         # As opposed to the class docstring inheritance, and following
                         # the MRO for methods, we inherit only from the first found parent.
                         break
-                    # TODO: else WARN that no dosctring is defined and none can be inherited.
 
     @staticmethod
     def _create_dummy_func_with_doc(docstring: str | None) -> Callable[..., Any]:
         """Create a dummy function with a given docstring.
 
         Args:
             docstring: The docstring to be assigned.
```

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/__init__.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/__init__.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/base.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
         "See Also",
         "Notes",
         "References",
         "Examples",
     ]
     """Names of the sections."""
 
-    _ARGS_SECTION_NAME: ClassVar[str]
-    """The name of the section for method and function arguments."""
+    _ARGS_SECTION_NAMES: ClassVar[set[str]]
+    """Names of the sections for method and function arguments."""
 
     _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]]
-    """Names of all the sections with items, including `_ARGS_SECTION_NAME`."""
+    """Names of the sections with items."""
 
     MISSING_ARG_DESCRIPTION: ClassVar[str] = "The description is missing."
     """Fall back description for an argument without a given description."""
 
     def __call__(self, parent_doc: str | None, child_func: Callable[..., Any]) -> None:
         """
         Args:
@@ -265,23 +265,19 @@
             temp_section_items.update(
                 cast(Dict[str, str], child_sections[section_name])
             )
 
             temp_sections[section_name] = temp_section_items
 
         # Args section shall be filtered.
-        args_section = cls._filter_args_section(
-            child_func,
-            cast(Dict[str, str], temp_sections.get(cls._ARGS_SECTION_NAME, {})),
-        )
-        if args_section:
-            temp_sections[cls._ARGS_SECTION_NAME] = args_section
-        elif cls._ARGS_SECTION_NAME in temp_sections:
-            # The args section is empty, there is nothing to document.
-            del temp_sections[cls._ARGS_SECTION_NAME]
+        for section_name in temp_sections.keys() & cls._ARGS_SECTION_NAMES:
+            temp_sections[section_name] = cls._filter_args_section(
+                child_func,
+                cast(Dict[str, str], temp_sections[section_name]),
+            )
 
         # Reorder the standard sections.
         new_child_sections = {
             section_name: temp_sections.pop(section_name)
             for section_name in cls._SECTION_NAMES
             if section_name in temp_sections
         }
```

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/google.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/google.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     """A class for inheriting docstrings in Google format."""
 
     _SECTION_NAMES: ClassVar[list[str | None]] = list(
         AbstractDocstringInheritor._SECTION_NAMES
     )
     _SECTION_NAMES[1] = "Args"
 
-    _ARGS_SECTION_NAME: ClassVar[str] = "Args"
+    _ARGS_SECTION_NAMES: ClassVar[set[str]] = {"Args"}
 
-    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]] = {_ARGS_SECTION_NAME} | {
+    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]] = _ARGS_SECTION_NAMES | {
         "Attributes",
         "Methods",
     }
 
     MISSING_ARG_DESCRIPTION = f": {AbstractDocstringInheritor.MISSING_ARG_DESCRIPTION}"
 
     @classmethod
```

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance/docstring_inheritors/numpy.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/numpy.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
 from .base import AbstractDocstringInheritor
 
 
 class NumpyDocstringInheritor(AbstractDocstringInheritor):
     """A class for inheriting docstrings in Numpy format."""
 
-    # The section OtherParameters is not processed for the arguments.
-    _ARGS_SECTION_NAME: ClassVar[str] = "Parameters"
+    _ARGS_SECTION_NAMES: ClassVar[set[str]] = {
+        "Parameters",
+        "Other Parameters",
+    }
 
-    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]] = {_ARGS_SECTION_NAME} | {
-        "OtherParameters",
+    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]] = _ARGS_SECTION_NAMES | {
         "Attributes",
         "Methods",
     }
 
     MISSING_ARG_DESCRIPTION: ClassVar[
         str
     ] = f"\n    {AbstractDocstringInheritor.MISSING_ARG_DESCRIPTION}"
```

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/PKG-INFO` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docstring-inheritance
-Version: 2.0.0
+Version: 2.0.0rc0
 Summary: Avoid writing and maintaining duplicated docstrings.
 Author: Antoine Dechaume
 License: MIT
 Project-URL: Documentation, https://antoined.github.io/docstring-inheritance
 Project-URL: Homepage, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Source, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Tracker, https://github.com/AntoineD/docstring-inheritance/issues
```

### Comparing `docstring-inheritance-2.0.0/src/docstring_inheritance.egg-info/SOURCES.txt` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/tests/test_base_inheritor.py` & `docstring-inheritance-2.0.0rc0/tests/test_base_inheritor.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from __future__ import annotations
 
 import textwrap
-from typing import Generator
 
 import pytest
 
 from docstring_inheritance.docstring_inheritors.base import AbstractDocstringInheritor
 
 
 def _test_parse_sections(parse_sections, unindented_docstring, expected_sections):
@@ -100,20 +99,20 @@
 
 
 def func_all(arg1, arg2=None, *varargs, **varkw):
     pass
 
 
 @pytest.fixture(scope="module")
-def concrete_inheritor() -> Generator[type[AbstractDocstringInheritor], None, None]:
+def concrete_inheritor() -> type[AbstractDocstringInheritor]:
     """Return a concrete enough AbstractDocstringInheritor."""
-    AbstractDocstringInheritor._ARGS_SECTION_NAME = "Args"
+    AbstractDocstringInheritor._ARGS_SECTION_NAMES = {"Args"}
     AbstractDocstringInheritor._SECTION_NAMES_WITH_ITEMS = {"Args", "Methods"}
     yield AbstractDocstringInheritor
-    delattr(AbstractDocstringInheritor, "_ARGS_SECTION_NAME")
+    delattr(AbstractDocstringInheritor, "_ARGS_SECTION_NAMES")
     delattr(AbstractDocstringInheritor, "_SECTION_NAMES_WITH_ITEMS")
 
 
 @pytest.mark.parametrize(
     "parent_section,child_section,func,expected",
     [
         ({}, {}, func_none, {}),
@@ -154,58 +153,33 @@
             {"Methods": {"method": "parent"}},
             {"Methods": {"method": "child"}},
             func_none,
             {"Methods": {"method": "child"}},
         ),
         # Sections with args items.
         # Non-existing section in child for function without args.
-        ({"Args": {"parent_a": ""}}, {}, func_none, {}),
+        ({"Args": {"parent_a": ""}}, {}, func_none, {"Args": {}}),
         # Non-existing section in parent for function without args.
-        ({}, {"Args": {"child_a": ""}}, func_none, {}),
+        ({}, {"Args": {"child_a": ""}}, func_none, {"Args": {}}),
         # Missing argument description.
-        ({}, {}, func_args, {"Args": {"arg": "The description is missing."}}),
-        (
-            {},
-            {"Args": {"child_a": ""}},
-            func_args,
-            {"Args": {"arg": "The description is missing."}},
-        ),
-        (
-            {"Args": {"parent_a": ""}},
-            {},
-            func_args,
-            {"Args": {"arg": "The description is missing."}},
-        ),
         (
             {"Args": {"parent_a": ""}},
             {"Args": {"child_a": ""}},
             func_args,
             {"Args": {"arg": "The description is missing."}},
         ),
         # Argument description in parent.
         (
             {"Args": {"arg": "parent"}},
-            {},
-            func_args,
-            {"Args": {"arg": "parent"}},
-        ),
-        (
-            {"Args": {"arg": "parent"}},
             {"Args": {"child_a": ""}},
             func_args,
             {"Args": {"arg": "parent"}},
         ),
         # Argument description in child.
         (
-            {},
-            {"Args": {"arg": "child"}},
-            func_args,
-            {"Args": {"arg": "child"}},
-        ),
-        (
             {"Args": {"parent_a": ""}},
             {"Args": {"arg": "child"}},
             func_args,
             {"Args": {"arg": "child"}},
         ),
         # Argument description in both parent and child.
         (
```

### Comparing `docstring-inheritance-2.0.0/tests/test_google_inheritor.py` & `docstring-inheritance-2.0.0rc0/tests/test_google_inheritor.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/tests/test_inheritance_for_functions.py` & `docstring-inheritance-2.0.0rc0/tests/test_inheritance_for_functions.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/tests/test_metaclass_google.py` & `docstring-inheritance-2.0.0rc0/tests/test_metaclass_google.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from __future__ import annotations
 
-import textwrap
-
 import pytest
 
 from docstring_inheritance import GoogleDocstringInheritanceInitMeta
 from docstring_inheritance import GoogleDocstringInheritanceMeta
 
 parametrize_inheritance = pytest.mark.parametrize(
     "inheritance_class",
@@ -48,24 +46,24 @@
     class Child(Parent):
         def method(self, xx, x, *args, yy=None, y=None, **kwargs):
             """
             Args:
                 xx: int
             """
 
-    expected = """
+    excepted = """
 Args:
     xx: int
     x: int
     *args: int
     yy: The description is missing.
     y: float
     **kwargs: int"""
 
-    assert Child.method.__doc__ == expected
+    assert Child.method.__doc__ == excepted
 
 
 @parametrize_inheritance
 def test_class_doc_inheritance(inheritance_class):
     class GrandParent(metaclass=inheritance_class):
         """Class GrandParent.
 
@@ -96,15 +94,15 @@
             a: From Child.
             c : From Child.
 
         Note:
             From Child.
         """
 
-    expected = """\
+    excepted = """\
 Class Child.
 
 Attributes:
     a: From Child.
     b: From Parent.
     c : From Child.
 
@@ -112,15 +110,15 @@
     a: From GrandParent.
     b: From Parent.
 
 Note:
     From Child.\
 """
 
-    assert Child.__doc__ == expected
+    assert Child.__doc__ == excepted
 
 
 @parametrize_inheritance
 def test_do_not_inherit_from_object(inheritance_class):
     class Parent(metaclass=inheritance_class):
         def __init__(self):
             pass
@@ -149,39 +147,20 @@
         Note:
             From Child.
         """
 
         def __init__(self, b, c):
             pass
 
-    expected = """\
+    excepted = """\
 Class Child.
 
 Args:
     b: b from Parent.
     c: c from Child.
 
 Note:
     From Child.\
 """
 
-    assert Child.__doc__ == expected
+    assert Child.__doc__ == excepted
     assert Child.__init__.__doc__ is None
-
-
-def test_class_doc_inheritance_with_empty_parent_doc():
-    class Parent(metaclass=GoogleDocstringInheritanceInitMeta):
-        def __init__(self, a, b):
-            pass
-
-    class Child(Parent):
-        def __init__(self, b, c):
-            """
-            Args:
-                b: n
-            """
-
-    expected = """
-Args:
-    b: n
-"""
-    assert textwrap.dedent(Child.__init__.__doc__) == expected
```

### Comparing `docstring-inheritance-2.0.0/tests/test_metaclass_numpy.py` & `docstring-inheritance-2.0.0rc0/tests/test_metaclass_numpy.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-2.0.0/tests/test_numpy_inheritor.py` & `docstring-inheritance-2.0.0rc0/tests/test_numpy_inheritor.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             {"Methods": {1: 0}},
             {"Methods": {0: 0, 1: 0}},
         ),
         # Merge section_items with common items that are args.
         (
             {"Parameters": {}},
             {"Parameters": {}},
-            {},
+            {"Parameters": {}},
         ),
         # Standard section_items names come before non-standard ones.
         ({0: 0, "Notes": 0}, {}, {"Notes": 0, 0: 0}),
     ],
 )
 def test_inherit_sections(parent_sections, child_sections, expected_sections):
     new_child_sections = NumpyDocstringInheritor._inherit_sections(
```

### Comparing `docstring-inheritance-2.0.0/tox.ini` & `docstring-inheritance-2.0.0rc0/tox.ini`

 * *Files identical despite different names*

