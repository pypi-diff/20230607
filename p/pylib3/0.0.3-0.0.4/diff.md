# Comparing `tmp/pylib3-0.0.3.tar.gz` & `tmp/pylib3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylib3-0.0.3.tar", last modified: Tue Sep 24 13:58:25 2019, max compression
+gzip compressed data, was "pylib3-0.0.4.tar", last modified: Wed Jun  7 14:28:37 2023, max compression
```

## Comparing `pylib3-0.0.3.tar` & `pylib3-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sbendavi   (510)      600        0 2019-09-24 13:58:25.000000 pylib3-0.0.3/
--rw-r--r--   0 sbendavi   (510)      600     2146 2019-09-24 13:58:25.000000 pylib3-0.0.3/PKG-INFO
-drwxr-xr-x   0 sbendavi   (510)      600        0 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3.egg-info/
--rw-r--r--   0 sbendavi   (510)      600     2146 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3.egg-info/PKG-INFO
--rw-r--r--   0 sbendavi   (510)      600      308 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3.egg-info/SOURCES.txt
--rw-r--r--   0 sbendavi   (510)      600       17 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3.egg-info/requires.txt
--rw-r--r--   0 sbendavi   (510)      600        7 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3.egg-info/top_level.txt
--rw-r--r--   0 sbendavi   (510)      600        1 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3.egg-info/dependency_links.txt
-drwxr-xr-x   0 sbendavi   (510)      600        0 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3/
--rw-r--r--   0 sbendavi   (510)      600        6 2019-09-24 13:56:30.000000 pylib3-0.0.3/pylib3/PYLIB3_VERSION
--rw-r--r--   0 sbendavi   (510)      600     5725 2019-09-02 21:36:27.000000 pylib3-0.0.3/pylib3/__init__.py
-drwxr-xr-x   0 sbendavi   (510)      600        0 2019-09-24 13:58:25.000000 pylib3-0.0.3/pylib3/__pycache__/
--rw-r--r--   0 sbendavi   (510)      600     5513 2019-09-02 22:26:40.000000 pylib3-0.0.3/pylib3/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 sbendavi   (510)      600     6276 2019-09-02 21:43:52.000000 pylib3-0.0.3/pylib3/__init__.pyc
--rw-r--r--   0 sbendavi   (510)      600     1108 2019-09-02 22:11:41.000000 pylib3-0.0.3/LICENSE
--rw-r--r--   0 sbendavi   (510)      600       17 2019-09-02 21:37:24.000000 pylib3-0.0.3/requirements.txt
--rw-r--r--   0 sbendavi   (510)      600       72 2019-09-02 22:15:15.000000 pylib3-0.0.3/MANIFEST.in
--rw-r--r--   0 sbendavi   (510)      600     1205 2019-09-24 13:51:56.000000 pylib3-0.0.3/README.md
--rw-r--r--   0 sbendavi   (510)      600      939 2019-09-02 22:57:06.000000 pylib3-0.0.3/setup.py
--rw-r--r--   0 sbendavi   (510)      600       38 2019-09-24 13:58:25.000000 pylib3-0.0.3/setup.cfg
+drwxr-xr-x   0 sbendavi   (503) staff       (20)        0 2023-06-07 14:28:37.981933 pylib3-0.0.4/
+-rw-r--r--   0 sbendavi   (503) staff       (20)     1108 2023-03-15 06:13:37.000000 pylib3-0.0.4/LICENSE
+-rw-r--r--   0 sbendavi   (503) staff       (20)       72 2023-03-15 06:13:41.000000 pylib3-0.0.4/MANIFEST.in
+-rw-r--r--   0 sbendavi   (503) staff       (20)     1961 2023-06-07 14:28:37.981745 pylib3-0.0.4/PKG-INFO
+-rw-r--r--   0 sbendavi   (503) staff       (20)     1478 2023-06-07 13:55:35.000000 pylib3-0.0.4/README.md
+drwxr-xr-x   0 sbendavi   (503) staff       (20)        0 2023-06-07 14:28:37.979944 pylib3-0.0.4/pylib3/
+-rw-r--r--   0 sbendavi   (503) staff       (20)        6 2023-06-07 13:08:41.000000 pylib3-0.0.4/pylib3/PYLIB3_VERSION
+-rw-r--r--   0 sbendavi   (503) staff       (20)     6408 2023-06-07 13:58:30.000000 pylib3-0.0.4/pylib3/__init__.py
+-rw-r--r--   0 sbendavi   (503) staff       (20)     6276 2023-03-15 06:13:37.000000 pylib3-0.0.4/pylib3/__init__.pyc
+drwxr-xr-x   0 sbendavi   (503) staff       (20)        0 2023-06-07 14:28:37.981397 pylib3-0.0.4/pylib3/__pycache__/
+-rw-r--r--   0 sbendavi   (503) staff       (20)     5513 2023-03-15 06:13:37.000000 pylib3-0.0.4/pylib3/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 sbendavi   (503) staff       (20)     6124 2023-06-07 14:28:37.000000 pylib3-0.0.4/pylib3/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 sbendavi   (503) staff       (20)        0 2023-06-07 14:28:37.980993 pylib3-0.0.4/pylib3.egg-info/
+-rw-r--r--   0 sbendavi   (503) staff       (20)     1961 2023-06-07 14:28:37.000000 pylib3-0.0.4/pylib3.egg-info/PKG-INFO
+-rw-r--r--   0 sbendavi   (503) staff       (20)      351 2023-06-07 14:28:37.000000 pylib3-0.0.4/pylib3.egg-info/SOURCES.txt
+-rw-r--r--   0 sbendavi   (503) staff       (20)        1 2023-06-07 14:28:37.000000 pylib3-0.0.4/pylib3.egg-info/dependency_links.txt
+-rw-r--r--   0 sbendavi   (503) staff       (20)       17 2023-06-07 14:28:37.000000 pylib3-0.0.4/pylib3.egg-info/requires.txt
+-rw-r--r--   0 sbendavi   (503) staff       (20)        7 2023-06-07 14:28:37.000000 pylib3-0.0.4/pylib3.egg-info/top_level.txt
+-rw-r--r--   0 sbendavi   (503) staff       (20)       17 2023-03-15 06:13:37.000000 pylib3-0.0.4/requirements.txt
+-rw-r--r--   0 sbendavi   (503) staff       (20)       38 2023-06-07 14:28:37.982007 pylib3-0.0.4/setup.cfg
+-rw-r--r--   0 sbendavi   (503) staff       (20)      939 2023-03-15 06:13:41.000000 pylib3-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylib3-0.0.3/PKG-INFO` & `pylib3-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 Metadata-Version: 2.1
 Name: pylib3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Shared Library
 Home-page: https://gitlab.com/shlomi.ben.david/pylib3
 Author: Shlomi Ben-David
 Author-email: shlomi.ben.david@gmail.com
-License: UNKNOWN
-Description: # PYLIB3
-        
-        - The pylib3 is a shared python library, that includes common functions
-          that can be used in any python package.
-        - This package can be used both with python2 and python3
-        
-        ## Usage:
-        - Install the pylib3 package (inside your project virtual environment)
-        ```
-        pip install pylib3
-        ```
-        
-        - To import the pylib3 package
-        ```
-        import pylib3
-        ```
-        
-        - To use one of the common functions from the pylib3 package
-        ```
-        from pylib3 import timer
-        ```
-        
-        ## Common Functions:
-        
-        ```
-        get_version(caller, version_file)
-        ```
-        
-        Gets the version number from the version_file
-        
-        param str caller: source file caller (i.e __file__)
-        param str version_file: a version file to get the version number from
-        returns (str): version number or '0.0.0' if the version_file doesn't exists
-        
-        ```
-        init_logging(log_file, verbose=False, console=False)
-        ```
-        
-        Logger initialization
-        
-        param str log_file: log file name
-        param bool console: if set to True will print logs both to a file and to stdout (console)
-        param bool verbose: if set to True will print more information
-        
-        ```
-        timer(func)
-        ```
-        
-        This function used as a decorator function to print the
-        elapsed time of the passed function
-        
-        param obj func: original function
-        returns (obj): wrapper function
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PYLIB3
+
+- The pylib3 is a shared python library, that includes common functions
+  that can be used in any python package.
+- This package can be used both with python2 and python3
+
+## Usage:
+- Install the pylib3 package (inside your project virtual environment)
+```
+pip install pylib3
+```
+
+- To import the pylib3 package
+```
+import pylib3
+```
+
+- To use one of the common functions from the pylib3 package
+```
+from pylib3 import timer
+```
+
+## Common Functions:
+
+```
+get_version(caller, version_file)
+```
+
+Gets the version number from the version_file
+
+param str caller: source file caller (i.e __file__)
+param str version_file: a version file to get the version number from
+returns (str): version number or '0.0.0' if the version_file doesn't exists
+
+```
+init_logging(log_file, verbose=False, console=False, info='white', debug='blue', warning='yellow', error='red', critical='red')
+```
+
+Logger initialization
+
+param str log_file: log file name
+param bool console: if set to True will print logs both to a file and to stdout (console)
+param bool verbose: if set to True will print more information
+param str info: info messages color
+param str debug: debug messages color
+param str warning: warning messages color
+param str error: error messages color
+param str critical: critical messages color
+
+```
+timer(func)
+```
+
+This function used as a decorator function to print the
+elapsed time of the passed function
+
+param obj func: original function
+returns (obj): wrapper function
+
```

### Comparing `pylib3-0.0.3/pylib3.egg-info/PKG-INFO` & `pylib3-0.0.4/pylib3.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 Metadata-Version: 2.1
 Name: pylib3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Shared Library
 Home-page: https://gitlab.com/shlomi.ben.david/pylib3
 Author: Shlomi Ben-David
 Author-email: shlomi.ben.david@gmail.com
-License: UNKNOWN
-Description: # PYLIB3
-        
-        - The pylib3 is a shared python library, that includes common functions
-          that can be used in any python package.
-        - This package can be used both with python2 and python3
-        
-        ## Usage:
-        - Install the pylib3 package (inside your project virtual environment)
-        ```
-        pip install pylib3
-        ```
-        
-        - To import the pylib3 package
-        ```
-        import pylib3
-        ```
-        
-        - To use one of the common functions from the pylib3 package
-        ```
-        from pylib3 import timer
-        ```
-        
-        ## Common Functions:
-        
-        ```
-        get_version(caller, version_file)
-        ```
-        
-        Gets the version number from the version_file
-        
-        param str caller: source file caller (i.e __file__)
-        param str version_file: a version file to get the version number from
-        returns (str): version number or '0.0.0' if the version_file doesn't exists
-        
-        ```
-        init_logging(log_file, verbose=False, console=False)
-        ```
-        
-        Logger initialization
-        
-        param str log_file: log file name
-        param bool console: if set to True will print logs both to a file and to stdout (console)
-        param bool verbose: if set to True will print more information
-        
-        ```
-        timer(func)
-        ```
-        
-        This function used as a decorator function to print the
-        elapsed time of the passed function
-        
-        param obj func: original function
-        returns (obj): wrapper function
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PYLIB3
+
+- The pylib3 is a shared python library, that includes common functions
+  that can be used in any python package.
+- This package can be used both with python2 and python3
+
+## Usage:
+- Install the pylib3 package (inside your project virtual environment)
+```
+pip install pylib3
+```
+
+- To import the pylib3 package
+```
+import pylib3
+```
+
+- To use one of the common functions from the pylib3 package
+```
+from pylib3 import timer
+```
+
+## Common Functions:
+
+```
+get_version(caller, version_file)
+```
+
+Gets the version number from the version_file
+
+param str caller: source file caller (i.e __file__)
+param str version_file: a version file to get the version number from
+returns (str): version number or '0.0.0' if the version_file doesn't exists
+
+```
+init_logging(log_file, verbose=False, console=False, info='white', debug='blue', warning='yellow', error='red', critical='red')
+```
+
+Logger initialization
+
+param str log_file: log file name
+param bool console: if set to True will print logs both to a file and to stdout (console)
+param bool verbose: if set to True will print more information
+param str info: info messages color
+param str debug: debug messages color
+param str warning: warning messages color
+param str error: error messages color
+param str critical: critical messages color
+
+```
+timer(func)
+```
+
+This function used as a decorator function to print the
+elapsed time of the passed function
+
+param obj func: original function
+returns (obj): wrapper function
+
```

### Comparing `pylib3-0.0.3/pylib3/__init__.py` & `pylib3-0.0.4/pylib3/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 file name: __init__.py
 author: Shlomi Ben-David
-file version: 0.0.1
+file version: 0.0.2
 """
 import os
 import sys
 import time
 import logging
 
 COLOR_STREAM = False
@@ -17,16 +17,21 @@
     COLOR_STREAM = True
 except ImportError:
     pass
 
 
 class ColoredStreamHandler(logging.StreamHandler):
     """ Colored Logger Stream Handler class """
-    def __init__(self, stream):
+    def __init__(self, stream, info='white', debug='blue', warning='yellow', error='red', critical='red'):
         logging.StreamHandler.__init__(self, stream)
+        self.info = info
+        self.debug = debug
+        self.warning = warning
+        self.error = error
+        self.critical = critical
 
     def format(self, record):
         """
         Format the specified record.
 
         If a formatter is set, use it. Otherwise, use the default formatter
         for the module.
@@ -46,19 +51,19 @@
         """
         if self.formatter:
             fmt = self.formatter
         else:
             fmt = logging.Formatter()
 
         level_to_color_mapper = {
-            'INFO': 'white',
-            'DEBUG': 'blue',
-            'WARNING': 'yellow',
-            'ERROR': 'red',
-            'CRITICAL': 'red',
+            'INFO': self.info or 'white',
+            'DEBUG': self.debug or 'blue',
+            'WARNING': self.warning or 'yellow',
+            'ERROR': self.error or 'red',
+            'CRITICAL': self.critical or 'red',
         }
 
         color = level_to_color_mapper.get(record.levelname) or 'white'
         setattr(record, 'msg', colored(record.msg, color))
 
         return fmt.format(record)
 
@@ -85,22 +90,28 @@
     if not os.path.exists(version_path):
         return '0.0.0'
 
     with open(version_path, 'r') as ifile:
         return ifile.read().strip()
 
 
-def init_logging(log_file, verbose=False, console=False):
+def init_logging(
+    log_file, verbose=False, console=False, info='white', debug='blue', warning='yellow', error='red', critical='red'
+):
     """
     Logger initialization
 
     :param str log_file: log file name
-    :param bool console: if set to True will print logs both to a file
-        and to stdout
+    :param bool console: if set to True will print logs both to a file and to stdout
     :param bool verbose: if set to True will print more information
+    :param str info: info messages color
+    :param str debug: debug messages color
+    :param str warning: warning messages color
+    :param str error: error messages color
+    :param str critical: critical messages color
 
     NOTE: The bellow snippet taken from the logging Formatter class
 
     %(name)s            Name of the logger (logging channel)
     %(levelno)s         Numeric logging level for the message (DEBUG, INFO,
                         WARNING, ERROR, CRITICAL)
     %(levelname)s       Text logging level for the message ("DEBUG", "INFO",
@@ -141,15 +152,17 @@
 
     if COLOR_STREAM:
         StreamHandler = ColoredStreamHandler
     else:
         StreamHandler = logging.StreamHandler
 
     if console:
-        console_handler = StreamHandler(sys.stdout)
+        console_handler = StreamHandler(
+            sys.stdout, info=info, debug=debug, warning=warning, error=error, critical=critical
+        )
         console_handler.setFormatter(console_log_formatter)
         logger.addHandler(console_handler)
 
 
 def timer(func):
     """
     This function used as a decorator function to check
```

### Comparing `pylib3-0.0.3/pylib3/__pycache__/__init__.cpython-37.pyc` & `pylib3-0.0.4/pylib3/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pylib3-0.0.3/pylib3/__init__.pyc` & `pylib3-0.0.4/pylib3/__init__.pyc`

 * *Files identical despite different names*

### Comparing `pylib3-0.0.3/LICENSE` & `pylib3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylib3-0.0.3/README.md` & `pylib3-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,22 +29,27 @@
 Gets the version number from the version_file
 
 param str caller: source file caller (i.e __file__)
 param str version_file: a version file to get the version number from
 returns (str): version number or '0.0.0' if the version_file doesn't exists
 
 ```
-init_logging(log_file, verbose=False, console=False)
+init_logging(log_file, verbose=False, console=False, info='white', debug='blue', warning='yellow', error='red', critical='red')
 ```
 
 Logger initialization
 
 param str log_file: log file name
 param bool console: if set to True will print logs both to a file and to stdout (console)
 param bool verbose: if set to True will print more information
+param str info: info messages color
+param str debug: debug messages color
+param str warning: warning messages color
+param str error: error messages color
+param str critical: critical messages color
 
 ```
 timer(func)
 ```
 
 This function used as a decorator function to print the
 elapsed time of the passed function
```

### Comparing `pylib3-0.0.3/setup.py` & `pylib3-0.0.4/setup.py`

 * *Files identical despite different names*

