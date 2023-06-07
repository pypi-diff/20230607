# Comparing `tmp/nsqdriver-0.2.7.tar.gz` & `tmp/nsqdriver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsqdriver-0.2.7.tar", last modified: Mon Jun  5 04:24:03 2023, max compression
+gzip compressed data, was "nsqdriver-0.3.0.tar", last modified: Wed Jun  7 06:20:56 2023, max compression
```

## Comparing `nsqdriver-0.2.7.tar` & `nsqdriver-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.766407 nsqdriver-0.2.7/nsqdriver/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/NS_CST.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/NS_MCI.py
--rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/NS_QSYNC.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/nsqdriver/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/AWG_ADC.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/BD_NSMCI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/ND_NSMCI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/nsqdriver/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/nsqdriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 04:24:03.000000 nsqdriver-0.2.7/nsqdriver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:24:03.770407 nsqdriver-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_cy_gen_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_demod_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_driver_info_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_init_device.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_mixer_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_param_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_rfskit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-05 04:23:58.000000 nsqdriver-0.2.7/tests/test_rpc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/nsqdriver/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/NS_CST.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19542 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/NS_MCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23281 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/NS_QSYNC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/nsqdriver/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/compiler/ns_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/compiler/py_wave_asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/nsqdriver/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/wrapper/AWG_ADC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/wrapper/BD_NSMCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/wrapper/ND_NSMCI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/nsqdriver/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/nsqdriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 06:20:56.000000 nsqdriver-0.3.0/nsqdriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-07 06:20:56.000000 nsqdriver-0.3.0/nsqdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:20:56.000000 nsqdriver-0.3.0/nsqdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 06:20:56.000000 nsqdriver-0.3.0/nsqdriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 06:20:56.000000 nsqdriver-0.3.0/nsqdriver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:20:56.603514 nsqdriver-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_cy_gen_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_demod_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_driver_info_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_init_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_ins_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_mixer_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_param_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_rfskit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-07 06:20:52.000000 nsqdriver-0.3.0/tests/test_rpc_parser.py
```

### Comparing `nsqdriver-0.2.7/README.md` & `nsqdriver-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/nsqdriver/NS_CST.py` & `nsqdriver-0.3.0/nsqdriver/NS_CST.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/nsqdriver/NS_MCI.py` & `nsqdriver-0.3.0/nsqdriver/NS_MCI.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,31 @@
 from xmlrpc.client import Transport
 from multiprocessing import shared_memory
 from functools import wraps
 
 import numpy as np
 import waveforms
 
-from .common import BaseDriver, Quantity, get_coef
+try:
+    from .common import BaseDriver, Quantity, get_coef
+except ImportError as e:
+    class BaseDriver:
+        def __init__(self, addr, timeout, **kw):
+            self.addr = addr
+            self.timeout = timeout
+
+
+    class Quantity(object):
+        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
+            self.name = name
+            self.default = dict(value=value, ch=ch, unit=unit)
+
+
+    def get_coef(*args):
+        return '', '', '', ''
 
 DEBUG_PRINT = False
 
 
 def print_debug(*args, **kwargs):
     if DEBUG_PRINT:
         print(*args, **kwargs)
```

### Comparing `nsqdriver-0.2.7/nsqdriver/NS_QSYNC.py` & `nsqdriver-0.3.0/nsqdriver/NS_QSYNC.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,34 @@
 import pickle
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import wait as wait_futures
 from multiprocessing import shared_memory
 from functools import lru_cache, wraps
 from typing import Union, TYPE_CHECKING, Tuple, Iterable
 
-from .common import BaseDriver, Quantity, QInteger
+try:
+    from .common import BaseDriver, Quantity, QInteger
+except ImportError as e:
+    class BaseDriver:
+        def __init__(self, addr, timeout, **kw):
+            self.addr = addr
+            self.timeout = timeout
+
+
+    class Quantity(object):
+        def __init__(self, name: str, value=None, ch: int = 1, unit: str = ''):
+            self.name = name
+            self.default = dict(value=value, ch=ch, unit=unit)
+
+
+    class QInteger:
+        def __init__(self, name, value=None, unit='', ch=None,
+                     get_cmd='', set_cmd='', ):
+            self.name = name
+
 
 if TYPE_CHECKING:
     from backend.board_parser import MCIBoard
     from concurrent.futures import Future
 
 THREAD_POOL = ThreadPoolExecutor(max_workers=10)
 _scanning_lock = threading.Lock()
```

### Comparing `nsqdriver-0.2.7/nsqdriver/wrapper/AWG_ADC.py` & `nsqdriver-0.3.0/nsqdriver/wrapper/AWG_ADC.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/nsqdriver/wrapper/BD_NSMCI.py` & `nsqdriver-0.3.0/nsqdriver/wrapper/BD_NSMCI.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/nsqdriver/wrapper/ND_NSMCI.py` & `nsqdriver-0.3.0/nsqdriver/wrapper/ND_NSMCI.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/nsqdriver.egg-info/SOURCES.txt` & `nsqdriver-0.3.0/nsqdriver.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 nsqdriver/common.py
 nsqdriver/setup.py
 nsqdriver.egg-info/PKG-INFO
 nsqdriver.egg-info/SOURCES.txt
 nsqdriver.egg-info/dependency_links.txt
 nsqdriver.egg-info/requires.txt
 nsqdriver.egg-info/top_level.txt
+nsqdriver/compiler/__init__.py
+nsqdriver/compiler/ns_wave.py
+nsqdriver/compiler/py_wave_asm.py
 nsqdriver/wrapper/AWG_ADC.py
 nsqdriver/wrapper/BD_NSMCI.py
 nsqdriver/wrapper/ND_NSMCI.py
 nsqdriver/wrapper/__init__.py
 tests/test_cy_gen_wave.py
 tests/test_demod_speed.py
 tests/test_driver_info_memory.py
 tests/test_init_device.py
+tests/test_ins_channel.py
 tests/test_mixer_simulator.py
 tests/test_param_memory.py
 tests/test_rfskit_base.py
 tests/test_rpc_parser.py
```

### Comparing `nsqdriver-0.2.7/tests/test_cy_gen_wave.py` & `nsqdriver-0.3.0/tests/test_cy_gen_wave.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/tests/test_demod_speed.py` & `nsqdriver-0.3.0/tests/test_demod_speed.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/tests/test_driver_info_memory.py` & `nsqdriver-0.3.0/tests/test_driver_info_memory.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/tests/test_param_memory.py` & `nsqdriver-0.3.0/tests/test_param_memory.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/tests/test_rfskit_base.py` & `nsqdriver-0.3.0/tests/test_rfskit_base.py`

 * *Files identical despite different names*

### Comparing `nsqdriver-0.2.7/tests/test_rpc_parser.py` & `nsqdriver-0.3.0/tests/test_rpc_parser.py`

 * *Files identical despite different names*

