# Comparing `tmp/python_omnilogic_local-0.8.0.tar.gz` & `tmp/python_omnilogic_local-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.8.0.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.8.1.tar", max compression
```

## Comparing `python_omnilogic_local-0.8.0.tar` & `python_omnilogic_local-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1696 2023-05-31 19:02:53.205971 python_omnilogic_local-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/__init__.py
--rw-r--r--   0        0        0    21453 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0      164 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     8385 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9968 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0    10194 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6338 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5297 2023-05-31 19:02:54.366016 python_omnilogic_local-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 python_omnilogic_local-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1901 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    21453 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0      164 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     8416 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9968 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10194 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6338 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-06-07 17:59:34.205052 python_omnilogic_local-0.8.1/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5297 2023-06-07 17:59:35.373135 python_omnilogic_local-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 python_omnilogic_local-0.8.1/PKG-INFO
```

### Comparing `python_omnilogic_local-0.8.0/README.md` & `python_omnilogic_local-0.8.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 <p align="center">
   <a href="https://pypi.org/project/python-omnilogic-local/">
     <img src="https://img.shields.io/pypi/v/python-omnilogic-local.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
   <img src="https://img.shields.io/pypi/pyversions/python-omnilogic-local.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/python-omnilogic-local.svg?style=flat-square" alt="License">
+  <a href="https://www.buymeacoffee.com/cryptk" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 20px !important;" ></a>
 </p>
 
 A library implementing the UDP XML Local Control api for Hayward OmniLogic and OmniHub pool controllers
 
 ## Installation
 
 This package is published to pypi at https://pypi.org/project/python-omnilogic-local/:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Pyomnilogic Local
-             [PyPI_Version] [Supported Python versions] [License]
+    [PyPI_Version] [Supported Python versions] [License] [Buy_Me_A_Coffee]
 A library implementing the UDP XML Local Control api for Hayward OmniLogic and
 OmniHub pool controllers ## Installation This package is published to pypi at
 https://pypi.org/project/python-omnilogic-local/: `pip install python-
 omnilogic-local` ## Functionality This library is still under development and
 is not yet able to control every function of a Hayward pool controller. The
 implemented functionality is: - Pulling the MSP Config - Polling telemetry -
 Polling a list of active alarms - Polling filter/pump diagnostic information -
```

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/api.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/models/mspconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
                 OmniType.BOW_MSP,
                 OmniType.CHLORINATOR,
                 OmniType.CL_LIGHT,
                 OmniType.FAVORITES,
                 OmniType.FILTER,
                 OmniType.GROUPS,
                 OmniType.HEATER_EQUIP,
+                OmniType.PUMP,
                 OmniType.RELAY,
                 OmniType.SENSOR,
                 OmniType.SCHE,
             ),
         )
         try:
             return MSPConfig.parse_obj(data["MSPConfig"])
```

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyomnilogic_local/types.py` & `python_omnilogic_local-0.8.1/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.8.0/pyproject.toml` & `python_omnilogic_local-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.8.0"
+version = "0.8.1"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.8.0/PKG-INFO` & `python_omnilogic_local-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.8.0
+Version: 0.8.1
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -25,14 +25,15 @@
 
 <p align="center">
   <a href="https://pypi.org/project/python-omnilogic-local/">
     <img src="https://img.shields.io/pypi/v/python-omnilogic-local.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
   <img src="https://img.shields.io/pypi/pyversions/python-omnilogic-local.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/python-omnilogic-local.svg?style=flat-square" alt="License">
+  <a href="https://www.buymeacoffee.com/cryptk" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 20px !important;" ></a>
 </p>
 
 A library implementing the UDP XML Local Control api for Hayward OmniLogic and OmniHub pool controllers
 
 ## Installation
 
 This package is published to pypi at https://pypi.org/project/python-omnilogic-local/:
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.8.0 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.8.1 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries Requires-Dist: pydantic
 (>=1.10.7,<2.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL:
 Repository, https://github.com/cryptk/python-omnilogic-local Description-
 Content-Type: text/markdown # Pyomnilogic Local
-             [PyPI_Version] [Supported Python versions] [License]
+    [PyPI_Version] [Supported Python versions] [License] [Buy_Me_A_Coffee]
 A library implementing the UDP XML Local Control api for Hayward OmniLogic and
 OmniHub pool controllers ## Installation This package is published to pypi at
 https://pypi.org/project/python-omnilogic-local/: `pip install python-
 omnilogic-local` ## Functionality This library is still under development and
 is not yet able to control every function of a Hayward pool controller. The
 implemented functionality is: - Pulling the MSP Config - Polling telemetry -
 Polling a list of active alarms - Polling filter/pump diagnostic information -
```

