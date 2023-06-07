# Comparing `tmp/prettyc-1.0.0.tar.gz` & `tmp/prettyc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.0.tar", last modified: Wed Jun  7 13:14:14 2023, max compression
+gzip compressed data, was "prettyc-1.0.1.tar", last modified: Wed Jun  7 13:56:16 2023, max compression
```

## Comparing `prettyc-1.0.0.tar` & `prettyc-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 13:14:14.348099 prettyc-1.0.0/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.0/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1688 2023-06-07 13:14:14.348099 prettyc-1.0.0/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      753 2023-06-07 13:13:13.000000 prettyc-1.0.0/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 13:14:14.348099 prettyc-1.0.0/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1688 2023-06-07 13:14:14.000000 prettyc-1.0.0/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 13:14:14.000000 prettyc-1.0.0/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 13:14:14.000000 prettyc-1.0.0/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 13:14:14.000000 prettyc-1.0.0/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 13:14:14.000000 prettyc-1.0.0/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   263401 2023-06-07 13:08:19.000000 prettyc-1.0.0/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 13:14:14.348099 prettyc-1.0.0/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.0/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 13:56:16.228129 prettyc-1.0.1/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.1/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1688 2023-06-07 13:56:16.228129 prettyc-1.0.1/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      753 2023-06-07 13:13:13.000000 prettyc-1.0.1/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 13:56:16.228129 prettyc-1.0.1/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1688 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 13:56:16.000000 prettyc-1.0.1/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   261617 2023-06-07 13:54:04.000000 prettyc-1.0.1/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 13:56:16.228129 prettyc-1.0.1/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.1/setup.py
```

### Comparing `prettyc-1.0.0/LICENSE` & `prettyc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.0/PKG-INFO` & `prettyc-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.0/README.md` & `prettyc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.0/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.1/prettyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.0/prettyc.py` & `prettyc-1.0.1/prettyc.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
+__verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
   xrange = range  # Python 3
@@ -236,16 +237,16 @@
      (by default, only files with extensions %s will be assumed to be headers)
 
       Examples:
         --headers=%s
         --headers=hpp,hxx
         --headers=hpp
 
-    prettyc.py supports per-directory configurations specified in PRETTYC.cfg
-    files. PRETTYC.cfg file can contain a number of key=value pairs.
+    prettyc.py supports per-directory configurations specified in .prettyc
+    files. .prettyc file can contain a number of key=value pairs.
     Currently the following options are supported:
 
       set noparent
       filter=+filter1,-filter2,...
       exclude_files=regex
       linelength=80
       root=subdir
@@ -262,20 +263,20 @@
     "exclude_files" allows to specify a regular expression to be matched against
     a file name. If the expression matches, the file is skipped and not run
     through the linter.
 
     "linelength" allows to specify the allowed line length for the project.
 
     The "root" option is similar in function to the --root flag (see example
-    above). Paths are relative to the directory of the PRETTYC.cfg.
+    above). Paths are relative to the directory of the .prettyc.
 
     The "headers" option is similar in function to the --headers flag
     (see example above).
 
-    PRETTYC.cfg has an effect on files in the same directory and all
+    .prettyc has an effect on files in the same directory and all
     sub-directories, unless overridden by a nested configuration file.
 
       Example file:
         filter=-build/include_order,+build/include_alpha
         exclude_files=.*\\.cc
 
     The above example disables build/include_order warning and enables
@@ -323,15 +324,14 @@
     'readability/nul',
     'readability/strings',
     'readability/todo',
     'readability/utf8',
     'runtime/arrays',
     'runtime/casting',
     'runtime/explicit',
-    'runtime/int',
     'runtime/init',
     'runtime/invalid_increment',
     'runtime/member_string_references',
     'runtime/memset',
     'runtime/indentation_namespace',
     'runtime/operator',
     'runtime/printf',
@@ -4287,38 +4287,14 @@
     prevline = GetPreviousNonBlankLine(clean_lines, linenum)[0]
     if (not Search(r'[,;:}{(]\s*$', prevline) and
         not Match(r'\s*#', prevline) and
         not (GetLineWidth(prevline) > _line_length - 2 and '[]' in prevline)):
       error(filename, linenum, 'whitespace/braces', 4,
             '{ should almost always be at the end of the previous line')
 
-  # An else clause should be on the same line as the preceding closing brace.
-  if Match(r'\s*else\b\s*(?:if\b|\{|$)', line):
-    prevline = GetPreviousNonBlankLine(clean_lines, linenum)[0]
-    if Match(r'\s*}\s*$', prevline):
-      error(filename, linenum, 'whitespace/newline', 4,
-            'An else should appear on the same line as the preceding }')
-
-  # If braces come on one side of an else, they should be on both.
-  # However, we have to worry about "else if" that spans multiple lines!
-  if Search(r'else if\s*\(', line):       # could be multi-line if
-    brace_on_left = bool(Search(r'}\s*else if\s*\(', line))
-    # find the ( after the if
-    pos = line.find('else if')
-    pos = line.find('(', pos)
-    if pos > 0:
-      (endline, _, endpos) = CloseExpression(clean_lines, linenum, pos)
-      brace_on_right = endline[endpos:].find('{') != -1
-      if brace_on_left != brace_on_right:    # must be brace after if
-        error(filename, linenum, 'readability/braces', 5,
-              'If an else has a brace on one side, it should have it on both')
-  elif Search(r'}\s*else[^{]*$', line) or Match(r'[^}]*else\s*{', line):
-    error(filename, linenum, 'readability/braces', 5,
-          'If an else has a brace on one side, it should have it on both')
-
   # Likewise, an else should never have the else clause on the same line
   if Search(r'\belse [^\s{]', line) and not Search(r'\belse if\b', line):
     error(filename, linenum, 'whitespace/newline', 4,
           'Else clause should never be on same line as else (use 2 lines)')
 
   # In the same way, a do/while should never be on one line
   if Match(r'\s*do [^\s{]', line):
@@ -5073,15 +5049,14 @@
       target_first_component.group(0) ==
       include_first_component.group(0)):
     return _POSSIBLE_MY_HEADER
 
   return _OTHER_HEADER
 
 
-
 def CheckIncludeLine(filename, clean_lines, linenum, include_state, error):
   """Check rules that are applicable to #include lines.
 
   Strings on #include lines are NOT removed from elided line, to make
   certain tasks easier. However, to prevent false positives, checks
   applicable to #include lines in CheckLanguage must be put here.
 
@@ -5300,26 +5275,14 @@
     # TODO(unknown): check that 1-arg constructors are explicit.
     #                How to tell it's a constructor?
     #                (handled in CheckForNonStandardConstructs for now)
     # TODO(unknown): check that classes declare or disable copy/assign
     #                (level 1 error)
     pass
 
-  # Check if people are using the verboten C basic types.  The only exception
-  # we regularly allow is "unsigned short port" for port.
-  if Search(r'\bshort port\b', line):
-    if not Search(r'\bunsigned short port\b', line):
-      error(filename, linenum, 'runtime/int', 4,
-            'Use "unsigned short" for ports, not "short"')
-  else:
-    match = Search(r'\b(short|long(?! +double)|long long)\b', line)
-    if match:
-      error(filename, linenum, 'runtime/int', 4,
-            'Use int16/int64/etc, rather than the C type %s' % match.group(1))
-
   # Check if some verboten operator overloading is going on
   # TODO(unknown): catch out-of-line unary operator&:
   #   class X {};
   #   int operator&(const X& x) { return 42; }  // unary operator&
   # The trick is it's hard to tell apart from binary operator&:
   #   class Y { int operator&(const Y& x) { return 23; } }; // binary operator&
   if Search(r'\boperator\s*&\s*\(\s*\)', line):
@@ -6550,15 +6513,15 @@
   cfg_filters = []
   keep_looking = True
   while keep_looking:
     abs_path, base_name = os.path.split(abs_filename)
     if not base_name:
       break  # Reached the root directory.
 
-    cfg_file = os.path.join(abs_path, "PRETTYC.cfg")
+    cfg_file = os.path.join(abs_path, ".prettyc")
     abs_filename = abs_path
     if not os.path.isfile(cfg_file):
       continue
 
     try:
       with codecs.open(cfg_file, 'r', 'utf8', 'replace') as file_handle:
         for line in file_handle:
@@ -6573,39 +6536,40 @@
             keep_looking = False
           elif name == 'filter':
             cfg_filters.append(val)
           elif name == 'exclude_files':
             # When matching exclude_files pattern, use the base_name of
             # the current file name or the directory name we are processing.
             # For example, if we are checking for lint errors in /foo/bar/baz.cc
-            # and we found the .cfg file at /foo/PRETTYC.cfg, then the config
+            # and we found the .cfg file at /foo/.prettyc, then the config
             # file's "exclude_files" filter is meant to be checked against "bar"
             # and not "baz" nor "bar/baz.cc".
             if base_name:
               pattern = re.compile(val)
               if pattern.match(base_name):
                 if _prettyc_state.quiet:
                   # Suppress "Ignoring file" warning when using --quiet.
                   return False
-                _prettyc_state.PrintInfo('Ignoring "%s": file excluded by "%s". '
-                                 'File path component "%s" matches '
-                                 'pattern "%s"\n' %
-                                 (filename, cfg_file, base_name, val))
+                if __verbose__:
+                    _prettyc_state.PrintInfo('Ignoring "%s": file excluded by "%s". '
+                                     'File path component "%s" matches '
+                                     'pattern "%s"\n' %
+                                     (filename, cfg_file, base_name, val))
                 return False
           elif name == 'linelength':
             global _line_length
             try:
               _line_length = int(val)
             except ValueError:
               _prettyc_state.PrintError('Line length must be numeric.')
           elif name == 'extensions':
             ProcessExtensionsOption(val)
           elif name == 'root':
             global _root
-            # root directories are specified relative to PRETTYC.cfg dir.
+            # root directories are specified relative to .prettyc dir.
             _root = os.path.join(os.path.dirname(cfg_file), val)
           elif name == 'headers':
             ProcessHppHeadersOption(val)
           elif name == 'includeorder':
             ProcessIncludeOrderOption(val)
           else:
             _prettyc_state.PrintError(
@@ -6709,16 +6673,16 @@
       # minority, we bias toward LF here since most tools prefer LF.
       for linenum in crlf_lines:
         Error(filename, linenum, 'whitespace/newline', 1,
               'Unexpected \\r (^M) found; better to use only \\n')
 
   # # Suppress printing anything if --quiet was passed unless the error
   # # count has increased after processing this file.
-  # if not _prettyc_state.quiet or old_errors != _prettyc_state.error_count:
-  #   _prettyc_state.PrintInfo('Done processing %s\n' % filename)
+  if __verbose__ and not _prettyc_state.quiet or old_errors != _prettyc_state.error_count:
+    _prettyc_state.PrintInfo('Done processing %s\n' % filename)
   _RestoreFilters()
 
 
 def PrintUsage(message):
   """Prints a brief usage string and exits, optionally with an error message.
 
   Args:
```

### Comparing `prettyc-1.0.0/setup.py` & `prettyc-1.0.1/setup.py`

 * *Files identical despite different names*

