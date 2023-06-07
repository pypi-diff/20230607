# Comparing `tmp/escapyde-0.2.2.tar.gz` & `tmp/escapyde-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escapyde-0.2.2.tar", max compression
+gzip compressed data, was "escapyde-0.2.3.tar", max compression
```

## Comparing `escapyde-0.2.2.tar` & `escapyde-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     4199 2023-06-01 20:39:50.043884 escapyde-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-06-01 20:39:50.043884 escapyde-0.2.2/LICENSE
--rw-r--r--   0        0        0      754 2023-06-01 20:39:50.043884 escapyde-0.2.2/README.md
--rw-r--r--   0        0        0      124 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/__init__.py
--rw-r--r--   0        0        0     2550 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/ansi.py
--rw-r--r--   0        0        0     2434 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/colours.py
--rw-r--r--   0        0        0        0 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/examples/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-01 20:39:50.043884 escapyde-0.2.2/escapyde/examples/text.py
--rw-r--r--   0        0        0     3640 2023-06-01 20:39:50.043884 escapyde-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 escapyde-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5155 2023-06-07 13:27:18.292448 escapyde-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-07 13:27:18.292448 escapyde-0.2.3/LICENSE
+-rw-r--r--   0        0        0      754 2023-06-07 13:27:18.292448 escapyde-0.2.3/README.md
+-rw-r--r--   0        0        0      124 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/__init__.py
+-rw-r--r--   0        0        0     2623 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/ansi.py
+-rw-r--r--   0        0        0     2434 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/colours.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/examples/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/examples/text.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:27:18.292448 escapyde-0.2.3/py.typed
+-rw-r--r--   0        0        0     4515 2023-06-07 13:27:18.292448 escapyde-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 escapyde-0.2.3/PKG-INFO
```

### Comparing `escapyde-0.2.2/CHANGELOG.md` & `escapyde-0.2.3/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -45,31 +45,62 @@
 - Updated localisation files
 
 -->
 
 <!--
 _______________________________________________________________________________
 
-## [0.2.2] - 2023-06-01
+## [0.2.3] - 2023-06-07
 
-Updated dependencies, and added `py.typed` to show the package
-is type-hinted.
+Remembered to include `py.typed` in the package, and fixed a bug with the
+`escape_format` function. Furthermore, identified a major bug with chained
+escapes, which will be fixed in the next major update as it may require breaking
+changes.
 
 ### Added
 
-- Added `py.typed`
+- Added `py.typed` - this time for real
+- Added unit tests
 
 ### Changed
 
 - Updated dependencies
 
+### Fixed
+
+- Fixed a bug where `escape_format` was forcing any replaced substrings to be
+  lowercase. The casing in the output now matches the input.
+
 -->
 
 _______________________________________________________________________________
 
+## [0.2.3] - 2023-06-07
+
+Remembered to include `py.typed` in the package, and fixed a bug with the
+`escape_format` function. Furthermore, identified a major bug with chained
+escapes, which will be fixed in the next major update as it may require breaking
+changes.
+
+### Added
+
+- Added `py.typed` - this time for real
+- Added unit tests
+
+### Changed
+
+- Updated dependencies
+
+### Fixed
+
+- Fixed a bug where `escape_format` was forcing any replaced substrings to be
+  lowercase. The casing in the output now matches the input.
+
+_______________________________________________________________________________
+
 ## [0.2.2] - 2023-06-01
 
 Updated dependencies, and added `py.typed` to show the package
 is type-hinted.
 
 ### Added
```

### Comparing `escapyde-0.2.2/LICENSE` & `escapyde-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.2/README.md` & `escapyde-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.2/escapyde/ansi.py` & `escapyde-0.2.3/escapyde/ansi.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,17 +70,20 @@
     for line_idx, line in enumerate(lines):
 
         words = line.split(' ')
         for substring, escape in escape_map.items():
 
             for idx, word in enumerate(words):
 
+                temp_word = word
+                temp_substring = substring
+
                 if not case_sensitive:
-                    substring = substring.lower()  # noqa: PLW2901
-                    word = word.lower()  # noqa: PLW2901
+                    temp_substring = temp_substring.lower()
+                    temp_word = temp_word.lower()
 
-                if word.startswith(substring):
+                if temp_word.startswith(temp_substring):
                     words[idx] = f'{escape | word[:len(substring)]}{word[len(substring):]}'
 
         lines[line_idx] = ' '.join(words)
 
     return '\n'.join(lines)
```

### Comparing `escapyde-0.2.2/escapyde/colours.py` & `escapyde-0.2.3/escapyde/colours.py`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.2/escapyde/examples/text.py` & `escapyde-0.2.3/escapyde/examples/text.py`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.2/PKG-INFO` & `escapyde-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escapyde
-Version: 0.2.2
+Version: 0.2.3
 Summary: Yet another ANSI escape sequence library for Python - now modernised!
 Home-page: https://pypi.org/project/escapyde/
 License: MIT
 Keywords: ansi,console,terminal,escape,sequence,colour,color
 Author: Lari Liuhamo
 Author-email: lari.liuhamo+pypi@gmail.com
 Maintainer: Lari Liuhamo
@@ -16,15 +16,14 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: IronPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: Stackless
 Classifier: Topic :: Artistic Software
```

