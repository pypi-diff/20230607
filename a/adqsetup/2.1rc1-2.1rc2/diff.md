# Comparing `tmp/adqsetup-2.1rc1.tar.gz` & `tmp/adqsetup-2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adqsetup-2.1rc1.tar", last modified: Fri Jun  2 17:37:33 2023, max compression
+gzip compressed data, was "adqsetup-2.1rc2.tar", last modified: Wed Jun  7 18:07:11 2023, max compression
```

## Comparing `adqsetup-2.1rc1.tar` & `adqsetup-2.1rc2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/
--rw-r--r--   0 petersst  (1000) petersst  (1000)     1509 2022-09-28 20:27:20.000000 adqsetup-2.1rc1/LICENSE
--rw-r--r--   0 petersst  (1000) petersst  (1000)       15 2022-09-28 20:27:20.000000 adqsetup-2.1rc1/MANIFEST.in
--rw-r--r--   0 petersst  (1000) petersst  (1000)    10341 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/PKG-INFO
--rw-r--r--   0 petersst  (1000) petersst  (1000)     8175 2023-05-31 18:06:39.000000 adqsetup-2.1rc1/README.md
-drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/adqsetup.egg-info/
--rw-r--r--   0 petersst  (1000) petersst  (1000)    10341 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/PKG-INFO
--rw-r--r--   0 petersst  (1000) petersst  (1000)      244 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/SOURCES.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/dependency_links.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)       45 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/entry_points.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2022-10-07 19:34:57.000000 adqsetup-2.1rc1/adqsetup.egg-info/not-zip-safe
--rw-r--r--   0 petersst  (1000) petersst  (1000)        9 2023-06-02 17:37:33.000000 adqsetup-2.1rc1/adqsetup.egg-info/top_level.txt
--rw-r--r--   0 petersst  (1000) petersst  (1000)   150292 2023-06-02 17:37:26.000000 adqsetup-2.1rc1/adqsetup.py
--rw-r--r--   0 petersst  (1000) petersst  (1000)       38 2023-06-02 17:37:33.120524 adqsetup-2.1rc1/setup.cfg
--rw-r--r--   0 petersst  (1000) petersst  (1000)      667 2023-06-02 17:33:30.000000 adqsetup-2.1rc1/setup.py
+drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2023-06-07 18:07:11.810524 adqsetup-2.1rc2/
+-rw-r--r--   0 petersst  (1000) petersst  (1000)     1509 2022-09-28 20:27:20.000000 adqsetup-2.1rc2/LICENSE
+-rw-r--r--   0 petersst  (1000) petersst  (1000)       15 2022-09-28 20:27:20.000000 adqsetup-2.1rc2/MANIFEST.in
+-rw-r--r--   0 petersst  (1000) petersst  (1000)    10341 2023-06-07 18:07:11.810524 adqsetup-2.1rc2/PKG-INFO
+-rw-r--r--   0 petersst  (1000) petersst  (1000)     8175 2023-05-31 18:06:39.000000 adqsetup-2.1rc2/README.md
+drwxr-xr-x   0 petersst  (1000) petersst  (1000)        0 2023-06-07 18:07:11.810524 adqsetup-2.1rc2/adqsetup.egg-info/
+-rw-r--r--   0 petersst  (1000) petersst  (1000)    10341 2023-06-07 18:07:11.000000 adqsetup-2.1rc2/adqsetup.egg-info/PKG-INFO
+-rw-r--r--   0 petersst  (1000) petersst  (1000)      244 2023-06-07 18:07:11.000000 adqsetup-2.1rc2/adqsetup.egg-info/SOURCES.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2023-06-07 18:07:11.000000 adqsetup-2.1rc2/adqsetup.egg-info/dependency_links.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)       45 2023-06-07 18:07:11.000000 adqsetup-2.1rc2/adqsetup.egg-info/entry_points.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)        1 2022-10-07 19:34:57.000000 adqsetup-2.1rc2/adqsetup.egg-info/not-zip-safe
+-rw-r--r--   0 petersst  (1000) petersst  (1000)        9 2023-06-07 18:07:11.000000 adqsetup-2.1rc2/adqsetup.egg-info/top_level.txt
+-rw-r--r--   0 petersst  (1000) petersst  (1000)   150861 2023-06-07 18:07:11.000000 adqsetup-2.1rc2/adqsetup.py
+-rw-r--r--   0 petersst  (1000) petersst  (1000)       38 2023-06-07 18:07:11.810524 adqsetup-2.1rc2/setup.cfg
+-rw-r--r--   0 petersst  (1000) petersst  (1000)      667 2023-06-07 18:07:08.000000 adqsetup-2.1rc2/setup.py
```

### Comparing `adqsetup-2.1rc1/LICENSE` & `adqsetup-2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `adqsetup-2.1rc1/PKG-INFO` & `adqsetup-2.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adqsetup
-Version: 2.1rc1
+Version: 2.1rc2
 Summary: A pure Python tool and library to setup ADQ for Intel NICs
 Home-page: https://www.intel.com/content/www/us/en/architecture-and-technology/ethernet/adq-resource-center.html
 Author: Intel
 License: BSD-3-Clause
 Description: # adqsetup
         
         _SPDX-License-Identifier: BSD-3-Clause_
```

### Comparing `adqsetup-2.1rc1/README.md` & `adqsetup-2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `adqsetup-2.1rc1/adqsetup.egg-info/PKG-INFO` & `adqsetup-2.1rc2/adqsetup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adqsetup
-Version: 2.1rc1
+Version: 2.1rc2
 Summary: A pure Python tool and library to setup ADQ for Intel NICs
 Home-page: https://www.intel.com/content/www/us/en/architecture-and-technology/ethernet/adq-resource-center.html
 Author: Intel
 License: BSD-3-Clause
 Description: # adqsetup
         
         _SPDX-License-Identifier: BSD-3-Clause_
```

### Comparing `adqsetup-2.1rc1/adqsetup.py` & `adqsetup-2.1rc2/adqsetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # 128 byte mutable buffer
         mask = create_string_buffer(_mask(cpus, 1024))
         size = len(mask)
         if libc.sched_setaffinity(c_uint32(pid), c_size_t(size), byref(mask)):
             raise Exception(os.strerror(get_errno()))
 
 
-_VERSION_ = '2.1rc1'
+_VERSION_ = '2.1rc2'
 
 ## public API
 
 __all__ = [
     'Config', 'ConfigGlobals', 'ConfigSection', 
     'check_interface'
     ]
@@ -1846,23 +1846,25 @@
                 # normalize maps and limit to 16 TCs
                 max_tc = self.TC_QOPT_MAX_QUEUE
                 pmap = pmap[:max_tc]
                 count = count[:len(pmap)]
                 offset = offset[:len(pmap)]
                 if min_rate is not None or max_rate is not None:
                     minrate = array('Q', [0] * 16)
-                    for i in range(len(min_rate)):
-                        pnum = pack("Q", min_rate[i] if min_rate[i] is not None else 0)
-                        num = unpack("Q", pnum)[0] * 125000
-                        minrate[i] = num
+                    if min_rate is not None:
+                        for i in range(len(min_rate)):
+                            pnum = pack("Q", min_rate[i] if min_rate[i] is not None else 0)
+                            num = unpack("Q", pnum)[0] * 125000
+                            minrate[i] = num
                     maxrate = array('Q', [0] * 16)
-                    for i in range(len(max_rate)):
-                        pnum = pack("Q", max_rate[i] if max_rate[i] is not None else 0)
-                        num = unpack("Q", pnum)[0] * 125000
-                        maxrate[i] = num
+                    if max_rate is not None:
+                        for i in range(len(max_rate)):
+                            pnum = pack("Q", max_rate[i] if max_rate[i] is not None else 0)
+                            num = unpack("Q", pnum)[0] * 125000
+                            maxrate[i] = num
                     # nested attrs
                     min_rates = [TCMQAttr(TCMQAttr.TYPE_MINRATE, minrate[i]) for i in range(16)]
                     max_rates = [TCMQAttr(TCMQAttr.TYPE_MAXRATE, maxrate[i]) for i in range(16)]
                     msg.data = msg.data + TCAttr(
                         TCAttr.TYPE_OPTIONS, 
                         pack("B", len(pmap)) + _pack_list(pmap, 'B', max_tc) 
                         + pack("B", 1) + _pack_list(count, 'H', max_tc) 
@@ -3202,21 +3204,28 @@
         for sec in self._sections.values():
             # TODO: check for proper power-of-two queue counts for each TC
             requested += sec.queues
         # if requested > self._queues:
         if requested > 256:
             raise Exception("Not enough queues available")
         
-    def _check_min_rate(self): # type() -> None
+    def _check_rates(self): # type() -> None
+        speed = int(_readfile("/sys/class/net/%s/speed" % self.globals.dev))
         requested = self.globals.min_rate if self.globals.min_rate is not None else 0
         for sec in self._sections.values():
             requested += sec.min_rate if sec.min_rate is not None else 0
-        speed = _readfile("/sys/class/net/%s/speed" % self.globals.dev)
-        if requested > int(speed):
-            raise Exception("Total min_rate exceeds device speed")
+        if requested > speed:
+            raise Exception("Total min_rate exceeds device speed %d" % speed)
+        requested = self.globals.max_rate if self.globals.max_rate is not None else 0
+        if requested > speed:
+            raise Exception("[globals] max_rate exceeds device speed %d" % speed)
+        for name, sec in self._sections.items():
+            requested = sec.max_rate if sec.max_rate is not None else 0
+            if requested > speed:
+                raise Exception("[%s] max_rate exceeds device speed %d" % (name, speed))
 
     def _cleanup(self): # type: () -> None
         '''
         Attempt to cleanup setup from previous run
         '''
         self._printhead("cleanup")
         # turn off napi threads if available
@@ -3546,15 +3555,15 @@
     def apply(self): # type: () -> None
         '''
         Applies the current config to the target system
         '''
         self._log("### cleanup ###")
         self._cleanup()
         self._check_queues()
-        self._check_min_rate()
+        self._check_rates()
         self.settings = Settings(self.globals.dev, self.log)
         self._set_sysctls()
         self._set_interface_flags()
         self._printhead("modifying system and network settings")
         self._log("", "### configuration ###")
         self._print(self.settings)
         self.settings.apply()
```

### Comparing `adqsetup-2.1rc1/setup.py` & `adqsetup-2.1rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='adqsetup',
-    version='2.1rc1',
+    version='2.1rc2',
     description='A pure Python tool and library to setup ADQ for Intel NICs',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',    
     url='https://www.intel.com/content/www/us/en/architecture-and-technology/ethernet/adq-resource-center.html',
     author='Intel',
     license='BSD-3-Clause',
     py_modules=['adqsetup'],
```

