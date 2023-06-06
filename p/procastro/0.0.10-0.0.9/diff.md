# Comparing `tmp/procastro-0.0.10.tar.gz` & `tmp/procastro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procastro-0.0.10.tar", last modified: Tue Jun  6 22:59:16 2023, max compression
+gzip compressed data, was "procastro-0.0.9.tar", last modified: Fri May 19 04:40:23 2023, max compression
```

## Comparing `procastro-0.0.10.tar` & `procastro-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:59:16.942602 procastro-0.0.10/
--rw-rw-rw-   0        0        0     1487 2023-05-21 20:58:53.000000 procastro-0.0.10/LICENSE
--rw-rw-rw-   0        0        0     1088 2023-06-06 22:59:16.942602 procastro-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-05-21 20:58:53.000000 procastro-0.0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 22:59:16.937916 procastro-0.0.10/procastro/
--rw-rw-rw-   0        0        0     1227 2023-06-06 22:14:32.000000 procastro-0.0.10/procastro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:59:16.942602 procastro-0.0.10/procastro.egg-info/
--rw-rw-rw-   0        0        0     1088 2023-06-06 22:59:16.000000 procastro-0.0.10/procastro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-06 22:59:16.000000 procastro-0.0.10/procastro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:59:16.000000 procastro-0.0.10/procastro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-06 22:59:16.000000 procastro-0.0.10/procastro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-06 22:59:16.000000 procastro-0.0.10/procastro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1226 2023-06-06 22:51:28.000000 procastro-0.0.10/pyproject.toml
--rw-rw-rw-   0        0        0      180 2023-06-06 22:59:16.942602 procastro-0.0.10/setup.cfg
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.383830 procastro-0.0.9/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1465 2023-05-19 04:36:31.000000 procastro-0.0.9/LICENSE
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    18092 2022-12-10 02:39:32.000000 procastro-0.0.9/LICENSE_old
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      936 2023-05-19 04:42:56.383830 procastro-0.0.9/PKG-INFO
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      615 2023-05-19 01:46:25.000000 procastro-0.0.9/README.md
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.210830 procastro-0.0.9/procastro/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1184 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/__init__.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.231830 procastro-0.0.9/procastro/astro/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      748 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/astro/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    23768 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/astro/astro.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     6395 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/astro/moon.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.236830 procastro-0.0.9/procastro/astro/tests/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        0 1972-04-17 18:10:02.000000 procastro-0.0.9/procastro/astro/tests/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1778 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/astro/tests/test_astro.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.258830 procastro-0.0.9/procastro/core/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1178 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    31231 2023-05-19 01:51:21.000000 procastro-0.0.9/procastro/core/astrodir.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    44821 2023-05-19 01:51:21.000000 procastro-0.0.9/procastro/core/astrofile.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    12333 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/interactive_graphics.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    14706 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/misc_arr.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     2478 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/misc_general.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    14146 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/misc_graph.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     2575 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/misc_math.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.267830 procastro-0.0.9/procastro/core/tests/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        0 1972-04-17 18:10:09.000000 procastro-0.0.9/procastro/core/tests/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     3927 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/tests/test_astrodir.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    10138 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/tests/test_astrofile.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1975 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/core/tests/test_utils.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.278830 procastro-0.0.9/procastro/obsrv/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      897 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/__init__.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.282830 procastro-0.0.9/procastro/obsrv/deprecated/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        0 1972-04-17 18:10:18.000000 procastro-0.0.9/procastro/obsrv/deprecated/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    63326 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/deprecated/available_at.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    24539 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/nightly.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    14116 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/obscalc.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    18945 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/obsrv.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.291830 procastro-0.0.9/procastro/obsrv/tests/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        0 1972-04-17 18:10:23.000000 procastro-0.0.9/procastro/obsrv/tests/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     4801 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/tests/test_obscalc.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1012 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/obsrv/tests/test_obsrv.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.307830 procastro-0.0.9/procastro/photography/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      980 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/photography/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     6005 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/photography/orchestrator.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     5086 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/photography/plotting.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     5711 2023-05-19 02:32:16.000000 procastro-0.0.9/procastro/photography/rawinfo.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.370830 procastro-0.0.9/procastro/tests/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        0 1972-04-17 18:10:46.000000 procastro-0.0.9/procastro/tests/__init__.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      175 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/tests/imshowz_interactive_test.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      116 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/tests/obsrv_test.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1086 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/tests/orch_test.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     3980 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/tests/test_photometry.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1181 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/tests/test_utils.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.375830 procastro-0.0.9/procastro/timeseries/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      788 2023-05-19 01:46:25.000000 procastro-0.0.9/procastro/timeseries/__init__.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.379830 procastro-0.0.9/procastro/timeseries/example/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     4265 2023-05-19 01:46:26.000000 procastro-0.0.9/procastro/timeseries/example/example.py
+-rw-r--r--   0 patobash  (1111) patobash  (1133)    57059 2023-05-19 01:51:21.000000 procastro-0.0.9/procastro/timeseries/photometry.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.381830 procastro-0.0.9/procastro/timeseries/tests/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        0 1972-04-17 18:14:51.000000 procastro-0.0.9/procastro/timeseries/tests/__init__.py
+drwxr-xr-x   0 patobash  (1111) patobash  (1133)        0 2023-05-19 04:42:56.223830 procastro-0.0.9/procastro.egg-info/
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      936 2023-05-19 04:42:56.000000 procastro-0.0.9/procastro.egg-info/PKG-INFO
+-rw-r--r--   0 patobash  (1111) patobash  (1133)     1547 2023-05-19 04:42:56.000000 procastro-0.0.9/procastro.egg-info/SOURCES.txt
+-rw-r--r--   0 patobash  (1111) patobash  (1133)        1 2023-05-19 04:42:56.000000 procastro-0.0.9/procastro.egg-info/dependency_links.txt
+-rw-r--r--   0 patobash  (1111) patobash  (1133)       71 2023-05-19 04:42:56.000000 procastro-0.0.9/procastro.egg-info/requires.txt
+-rw-r--r--   0 patobash  (1111) patobash  (1133)       10 2023-05-19 04:42:56.000000 procastro-0.0.9/procastro.egg-info/top_level.txt
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      570 2023-05-19 04:41:51.000000 procastro-0.0.9/pyproject.toml
+-rw-r--r--   0 patobash  (1111) patobash  (1133)      171 2023-05-19 04:42:56.386830 procastro-0.0.9/setup.cfg
```

### Comparing `procastro-0.0.10/LICENSE` & `procastro-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Copyright 2023 Patricio Rojo
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that
-the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the
- following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the
- following disclaimer in the documentation and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote
- products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED
-WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
-OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGE.
+Copyright 2023 Patricio Rojo
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that
+the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the
+ following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the
+ following disclaimer in the documentation and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote
+ products derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED
+WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
+OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGE.
```

### Comparing `procastro-0.0.10/PKG-INFO` & `procastro-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-Metadata-Version: 2.1
-Name: procastro
-Version: 0.0.10
-Summary: framework to process astronomical data files
-Author-email: Patricio Rojo <pato@das.uchile.cl>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/duckrojo/procastro
-Project-URL: Bug Tracker, https://github.com/duckrojo/procastro/issues
-Keywords: astronomy,data files
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# procastro
-
-## Installation
-
-You can download the current development version by cloning this repository
-
-	$ git clone https://github.com/duckrojo/procastro 
-
-## Testing
-
-Running tests is done by directly calling pytest from the root folder of the project
-	
-	$ pytest
-
-## Documentation
-
-You can compile the autogenerated documentation using the following command from the
-docs directory
-
-	$ cd docs
-	$ make html
-
-## Dependencies
-
-procastro supports python version 3.6 or higher, it currently depends on the following libraries: 
-
-* astropy 
-* numpy 
-* astroquery 0.3.10 or higher 
-* scipy 
-* matplotlib 
-* pyephem
+Metadata-Version: 2.1
+Name: procastro
+Version: 0.0.9
+Summary: framework to process astronomical data files
+Author-email: Patricio Rojo <duckrojo@gmail.com>
+License: BSD-3-Clause
+Keywords: astronomy,data files
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_old
+
+# procastro
+
+## Installation
+
+You can download the current development version by cloning this repository
+
+	$ git clone https://github.com/duckrojo/procastro 
+
+## Testing
+
+Running tests is done by directly calling pytest from the root folder of the project
+	
+	$ pytest
+
+## Documentation
+
+You can compile the autogenerated documentation using the following command from the
+docs directory
+
+	$ cd docs
+	$ make html
+
+## Dependencies
+
+procastro supports python version 3.6 or higher, it currently depends on the following libraries: 
+
+* astropy 
+* numpy 
+* astroquery 0.3.10 or higher 
+* scipy 
+* matplotlib 
+* pyephem
```

### Comparing `procastro-0.0.10/procastro/__init__.py` & `procastro-0.0.9/procastro/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-#
-# procastro - Data processing routines
-#
-# Copyright (C) 2013 Patricio Rojo
-#
-# This program is free software; you can redistribute it and/or
-# modify it under the terms of version 2 of the GNU General
-# Public License as published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin Street, Fifth Floor,
-# Boston, MA  02110-1301, USA.
-#
-#
-
-"""
-Data proc docstring
-"""
-from . import astro
-from . import core
-from .core import *
-#from . import timeseries
-#from . import obsrv
-import logging as _log
-
-
-__all__ = ['astro', 'dplogger']
-__all__ += core.__all__
-
-dplogger = _log.getLogger('procastro')
-_ch = _log.StreamHandler()
-_formatter = _log.Formatter('%(name)s (%(module)s.%(funcName)s) %(levelname)s: %(message)s')
-_ch.setFormatter(_formatter)
-dplogger.addHandler(_ch)
-
-__version__ = "0.0.10"
+#
+# procastro - Data processing routines
+#
+# Copyright (C) 2013 Patricio Rojo
+#
+# This program is free software; you can redistribute it and/or
+# modify it under the terms of version 2 of the GNU General
+# Public License as published by the Free Software Foundation.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program; if not, write to the Free Software
+# Foundation, Inc., 51 Franklin Street, Fifth Floor,
+# Boston, MA  02110-1301, USA.
+#
+#
+
+"""
+Data proc docstring
+"""
+from . import astro
+from . import core
+from .core import *
+#from . import timeseries
+#from . import obsrv
+import logging as _log
+
+
+__all__ = ['astro', 'dplogger']
+__all__ += core.__all__
+
+dplogger = _log.getLogger('procastro')
+_ch = _log.StreamHandler()
+_formatter = _log.Formatter('%(name)s (%(module)s.%(funcName)s) %(levelname)s: %(message)s')
+_ch.setFormatter(_formatter)
+dplogger.addHandler(_ch)
+
+__version__ = "0.0.9"
```

### Comparing `procastro-0.0.10/procastro.egg-info/PKG-INFO` & `procastro-0.0.9/procastro.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-Metadata-Version: 2.1
-Name: procastro
-Version: 0.0.10
-Summary: framework to process astronomical data files
-Author-email: Patricio Rojo <pato@das.uchile.cl>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/duckrojo/procastro
-Project-URL: Bug Tracker, https://github.com/duckrojo/procastro/issues
-Keywords: astronomy,data files
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# procastro
-
-## Installation
-
-You can download the current development version by cloning this repository
-
-	$ git clone https://github.com/duckrojo/procastro 
-
-## Testing
-
-Running tests is done by directly calling pytest from the root folder of the project
-	
-	$ pytest
-
-## Documentation
-
-You can compile the autogenerated documentation using the following command from the
-docs directory
-
-	$ cd docs
-	$ make html
-
-## Dependencies
-
-procastro supports python version 3.6 or higher, it currently depends on the following libraries: 
-
-* astropy 
-* numpy 
-* astroquery 0.3.10 or higher 
-* scipy 
-* matplotlib 
-* pyephem
+Metadata-Version: 2.1
+Name: procastro
+Version: 0.0.9
+Summary: framework to process astronomical data files
+Author-email: Patricio Rojo <duckrojo@gmail.com>
+License: BSD-3-Clause
+Keywords: astronomy,data files
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_old
+
+# procastro
+
+## Installation
+
+You can download the current development version by cloning this repository
+
+	$ git clone https://github.com/duckrojo/procastro 
+
+## Testing
+
+Running tests is done by directly calling pytest from the root folder of the project
+	
+	$ pytest
+
+## Documentation
+
+You can compile the autogenerated documentation using the following command from the
+docs directory
+
+	$ cd docs
+	$ make html
+
+## Dependencies
+
+procastro supports python version 3.6 or higher, it currently depends on the following libraries: 
+
+* astropy 
+* numpy 
+* astroquery 0.3.10 or higher 
+* scipy 
+* matplotlib 
+* pyephem
```

