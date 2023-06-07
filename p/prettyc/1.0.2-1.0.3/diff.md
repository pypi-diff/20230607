# Comparing `tmp/prettyc-1.0.2.tar.gz` & `tmp/prettyc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.2.tar", last modified: Wed Jun  7 14:03:34 2023, max compression
+gzip compressed data, was "prettyc-1.0.3.tar", last modified: Wed Jun  7 18:42:20 2023, max compression
```

## Comparing `prettyc-1.0.2.tar` & `prettyc-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 14:03:34.332135 prettyc-1.0.2/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.2/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 14:03:34.332135 prettyc-1.0.2/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.2/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 14:03:34.332135 prettyc-1.0.2/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 14:03:34.000000 prettyc-1.0.2/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   261617 2023-06-07 14:03:02.000000 prettyc-1.0.2/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 14:03:34.332135 prettyc-1.0.2/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.2/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 18:42:20.492029 prettyc-1.0.3/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.3/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 18:42:20.492029 prettyc-1.0.3/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.3/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 18:42:20.492029 prettyc-1.0.3/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 18:42:20.000000 prettyc-1.0.3/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 18:42:20.000000 prettyc-1.0.3/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 18:42:20.000000 prettyc-1.0.3/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 18:42:20.000000 prettyc-1.0.3/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 18:42:20.000000 prettyc-1.0.3/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   260920 2023-06-07 18:41:44.000000 prettyc-1.0.3/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 18:42:20.492029 prettyc-1.0.3/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.3/setup.py
```

### Comparing `prettyc-1.0.2/LICENSE` & `prettyc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.2/PKG-INFO` & `prettyc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.2/README.md` & `prettyc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.2/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.3/prettyc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.2/prettyc.py` & `prettyc-1.0.3/prettyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 __verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
@@ -296,15 +296,14 @@
     'build/c++tr1',
     'build/deprecated',
     'build/endif_comment',
     'build/explicit_make_pair',
     'build/forward_decl',
     'build/header_guard',
     'build/include',
-    'build/include_subdir',
     'build/include_alpha',
     'build/include_order',
     'build/include_what_you_use',
     'build/namespaces_headers',
     'build/namespaces_literals',
     'build/namespaces',
     'build/printf_format',
@@ -5066,28 +5065,14 @@
     linenum: The number of the line to check.
     include_state: An _IncludeState instance in which the headers are inserted.
     error: The function to call with any errors found.
   """
   fileinfo = FileInfo(filename)
   line = clean_lines.lines[linenum]
 
-  # "include" should use the new style "foo/bar.h" instead of just "bar.h"
-  # Only do this check if the included header follows google naming
-  # conventions.  If not, assume that it's a 3rd party API that
-  # requires special include conventions.
-  #
-  # We also make an exception for Lua headers, which follow google
-  # naming convention but not the include convention.
-  match = Match(r'#include\s*"([^/]+\.(.*))"', line)
-  if match:
-    if (IsHeaderExtension(match.group(2)) and
-        not _THIRD_PARTY_HEADERS_PATTERN.match(match.group(1))):
-      error(filename, linenum, 'build/include_subdir', 4,
-            'Include the directory when naming header files')
-
   # we shouldn't include a file more than once. actually, there are a
   # handful of instances where doing so is okay, but in general it's
   # not.
   match = _RE_PATTERN_INCLUDE.search(line)
   if match:
     include = match.group(2)
     used_angle_brackets = match.group(1) == '<'
@@ -6673,15 +6658,15 @@
       # minority, we bias toward LF here since most tools prefer LF.
       for linenum in crlf_lines:
         Error(filename, linenum, 'whitespace/newline', 1,
               'Unexpected \\r (^M) found; better to use only \\n')
 
   # # Suppress printing anything if --quiet was passed unless the error
   # # count has increased after processing this file.
-  if __verbose__ and not _prettyc_state.quiet or old_errors != _prettyc_state.error_count:
+  if __verbose__ and (not _prettyc_state.quiet or old_errors != _prettyc_state.error_count):
     _prettyc_state.PrintInfo('Done processing %s\n' % filename)
   _RestoreFilters()
 
 
 def PrintUsage(message):
   """Prints a brief usage string and exits, optionally with an error message.
```

### Comparing `prettyc-1.0.2/setup.py` & `prettyc-1.0.3/setup.py`

 * *Files identical despite different names*

