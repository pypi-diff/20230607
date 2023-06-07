# Comparing `tmp/hbp_validation_framework-0.8.1.tar.gz` & `tmp/hbp_validation_framework-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbp_validation_framework-0.8.1.tar", last modified: Fri Jan 20 15:09:37 2023, max compression
+gzip compressed data, was "hbp_validation_framework-0.8.2.tar", last modified: Wed Jun  7 15:55:42 2023, max compression
```

## Comparing `hbp_validation_framework-0.8.1.tar` & `hbp_validation_framework-0.8.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.187197 hbp_validation_framework-0.8.1/
--rw-r--r--   0 adavison   (502) staff       (20)     1523 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/LICENSE.txt
--rw-r--r--   0 adavison   (502) staff       (20)      179 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/MANIFEST.in
--rw-r--r--   0 adavison   (502) staff       (20)      455 2023-01-20 15:09:37.187061 hbp_validation_framework-0.8.1/PKG-INFO
--rw-r--r--   0 adavison   (502) staff       (20)      822 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/README.md
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.179190 hbp_validation_framework-0.8.1/hbp_validation_framework/
--rw-r--r--   0 adavison   (502) staff       (20)   116341 2023-01-20 15:07:51.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)    15481 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/datastores.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.183545 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/
--rw-r--r--   0 adavison   (502) staff       (20)     1220 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/CHANGELOG.md
--rw-r--r--   0 adavison   (502) staff       (20)     1110 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/LICENSE
--rw-r--r--   0 adavison   (502) staff       (20)     2747 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/README.md
--rw-r--r--   0 adavison   (502) staff       (20)     2557 2023-01-20 14:52:00.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/data.js
--rw-r--r--   0 adavison   (502) staff       (20)      815 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/document.json
--rw-r--r--   0 adavison   (502) staff       (20)     1150 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/favicon.ico
--rw-r--r--   0 adavison   (502) staff       (20)     6785 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/index.htm
--rw-r--r--   0 adavison   (502) staff       (20)     5045 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/jsonTreeViewer.js
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.174250 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.184641 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/
--rw-r--r--   0 adavison   (502) staff       (20)     7644 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/App.js
--rw-r--r--   0 adavison   (502) staff       (20)     2194 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/README.md
--rw-r--r--   0 adavison   (502) staff       (20)     6163 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/app.css
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.185203 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/docs/
--rw-r--r--   0 adavison   (502) staff       (20)     9615 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/docs/index.htm
--rw-r--r--   0 adavison   (502) staff       (20)     1557 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/docs/main.css
--rw-r--r--   0 adavison   (502) staff       (20)     1072 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/reset.css
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.186240 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/
--rw-r--r--   0 adavison   (502) staff       (20)      867 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/icons.svg
--rw-r--r--   0 adavison   (502) staff       (20)     2504 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.css
--rw-r--r--   0 adavison   (502) staff       (20)    24674 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.js
--rw-r--r--   0 adavison   (502) staff       (20)     1056 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/sample.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.186755 hbp_validation_framework-0.8.1/hbp_validation_framework/templates/
--rw-r--r--   0 adavison   (502) staff       (20)    23558 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/templates/report_template.html
--rw-r--r--   0 adavison   (502) staff       (20)    56458 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/utils.py
--rw-r--r--   0 adavison   (502) staff       (20)      734 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/hbp_validation_framework/versioning.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-01-20 15:09:37.180713 hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/
--rw-r--r--   0 adavison   (502) staff       (20)      455 2023-01-20 15:09:37.000000 hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/PKG-INFO
--rw-r--r--   0 adavison   (502) staff       (20)     1506 2023-01-20 15:09:37.000000 hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 adavison   (502) staff       (20)        1 2023-01-20 15:09:37.000000 hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 adavison   (502) staff       (20)      103 2023-01-20 15:09:37.000000 hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/requires.txt
--rw-r--r--   0 adavison   (502) staff       (20)       25 2023-01-20 15:09:37.000000 hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/top_level.txt
--rw-r--r--   0 adavison   (502) staff       (20)       31 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.1/requirements.txt
--rw-r--r--   0 adavison   (502) staff       (20)       38 2023-01-20 15:09:37.187249 hbp_validation_framework-0.8.1/setup.cfg
--rw-r--r--   0 adavison   (502) staff       (20)     1151 2023-01-20 15:07:31.000000 hbp_validation_framework-0.8.1/setup.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.602871 hbp_validation_framework-0.8.2/
+-rw-r--r--   0 adavison   (502) staff       (20)     1523 2023-06-07 15:54:23.000000 hbp_validation_framework-0.8.2/LICENSE.txt
+-rw-r--r--   0 adavison   (502) staff       (20)      179 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/MANIFEST.in
+-rw-r--r--   0 adavison   (502) staff       (20)      455 2023-06-07 15:55:42.602701 hbp_validation_framework-0.8.2/PKG-INFO
+-rw-r--r--   0 adavison   (502) staff       (20)      822 2023-06-07 15:54:42.000000 hbp_validation_framework-0.8.2/README.md
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.589891 hbp_validation_framework-0.8.2/hbp_validation_framework/
+-rw-r--r--   0 adavison   (502) staff       (20)   117520 2023-06-07 15:54:36.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)    15879 2023-06-07 14:36:57.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/datastores.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.598403 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/
+-rw-r--r--   0 adavison   (502) staff       (20)     1220 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/CHANGELOG.md
+-rw-r--r--   0 adavison   (502) staff       (20)     1110 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/LICENSE
+-rw-r--r--   0 adavison   (502) staff       (20)     2747 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/README.md
+-rw-r--r--   0 adavison   (502) staff       (20)     2557 2023-01-20 14:52:00.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/data.js
+-rw-r--r--   0 adavison   (502) staff       (20)      815 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/document.json
+-rw-r--r--   0 adavison   (502) staff       (20)     1150 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/favicon.ico
+-rw-r--r--   0 adavison   (502) staff       (20)     6785 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/index.htm
+-rw-r--r--   0 adavison   (502) staff       (20)     5045 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/jsonTreeViewer.js
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.584432 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.599911 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/
+-rw-r--r--   0 adavison   (502) staff       (20)     7644 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/App.js
+-rw-r--r--   0 adavison   (502) staff       (20)     2194 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/README.md
+-rw-r--r--   0 adavison   (502) staff       (20)     6163 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/app.css
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.600648 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/docs/
+-rw-r--r--   0 adavison   (502) staff       (20)     9615 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/docs/index.htm
+-rw-r--r--   0 adavison   (502) staff       (20)     1557 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/docs/main.css
+-rw-r--r--   0 adavison   (502) staff       (20)     1072 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/reset.css
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.601847 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/
+-rw-r--r--   0 adavison   (502) staff       (20)      867 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/icons.svg
+-rw-r--r--   0 adavison   (502) staff       (20)     2504 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.css
+-rw-r--r--   0 adavison   (502) staff       (20)    24674 2022-03-11 10:38:17.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.js
+-rw-r--r--   0 adavison   (502) staff       (20)     1056 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/sample.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.602435 hbp_validation_framework-0.8.2/hbp_validation_framework/templates/
+-rw-r--r--   0 adavison   (502) staff       (20)    23558 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/templates/report_template.html
+-rw-r--r--   0 adavison   (502) staff       (20)    56458 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/utils.py
+-rw-r--r--   0 adavison   (502) staff       (20)      734 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.2/hbp_validation_framework/versioning.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-06-07 15:55:42.595004 hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/
+-rw-r--r--   0 adavison   (502) staff       (20)      455 2023-06-07 15:55:42.000000 hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 adavison   (502) staff       (20)     1506 2023-06-07 15:55:42.000000 hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 adavison   (502) staff       (20)        1 2023-06-07 15:55:42.000000 hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 adavison   (502) staff       (20)      103 2023-06-07 15:55:42.000000 hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/requires.txt
+-rw-r--r--   0 adavison   (502) staff       (20)       25 2023-06-07 15:55:42.000000 hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/top_level.txt
+-rw-r--r--   0 adavison   (502) staff       (20)       31 2023-01-19 14:35:06.000000 hbp_validation_framework-0.8.2/requirements.txt
+-rw-r--r--   0 adavison   (502) staff       (20)       38 2023-06-07 15:55:42.602934 hbp_validation_framework-0.8.2/setup.cfg
+-rw-r--r--   0 adavison   (502) staff       (20)     1151 2023-06-07 15:53:39.000000 hbp_validation_framework-0.8.2/setup.py
```

### Comparing `hbp_validation_framework-0.8.1/LICENSE.txt` & `hbp_validation_framework-0.8.2/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2022, Shailesh Appukuttan, CNRS; Andrew P. Davison, CNRS
+Copyright (c) 2017-2023, Shailesh Appukuttan, CNRS; Andrew P. Davison, CNRS
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 * Neither the names of the copyright holders nor the names of the contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

### Comparing `hbp_validation_framework-0.8.1/README.md` & `hbp_validation_framework-0.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 A Python package for working with the EBRAINS/Human Brain Project Model Validation Framework
 ============================================================================================
 
-Andrew Davison and Shailesh Appukuttan, CNRS, 2017-2022
+Andrew Davison and Shailesh Appukuttan, CNRS, 2017-2023
 
 Documentation: http://hbp-validation-client.readthedocs.io
 
 Licence: BSD 3-clause, see LICENSE.txt
 
 <div><img src="https://raw.githubusercontent.com/HumanBrainProject/hbp-validation-client/master/eu_logo.jpg" alt="EU Logo" width="15%" align="right"></div>
```

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/__init__.py` & `hbp_validation_framework-0.8.2/hbp_validation_framework/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 A Python package for working with the EBRAINS / Human Brain Project Model Validation Framework.
 
-Andrew Davison and Shailesh Appukuttan, CNRS, 2017-2022
+Andrew Davison and Shailesh Appukuttan, CNRS, 2017-2023
 
 License: BSD 3-clause, see LICENSE.txt
 
 """
 
 import os
 import re
 import getpass
 import json
+from datetime import datetime
 
 import platform
 import socket
 from importlib import import_module
 from pathlib import Path
 from urllib.error import URLError
 from urllib.parse import urlparse, urlunparse, parse_qs, urljoin, urlencode, quote
@@ -30,15 +31,15 @@
     from clb_nb_utils import oauth
 
     have_collab_token_handler = True
 except ImportError:
     have_collab_token_handler = False
 
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 
 TOKENFILE = os.path.expanduser("~/.hbptoken")
 
 
 class ResponseError(Exception):
     pass
@@ -665,16 +666,31 @@
         module_name = ".".join(path_parts[:-1])
         test_module = import_module(module_name)
         test_cls = getattr(test_module, cls_name)
 
         # Load the reference data ("observations")
         observation_data = self._load_reference_data(test_json["data_location"])
 
+        # Combine parameters from test definition with locally-defined parameters
+        if test_instance_json["parameters"]:
+            response = requests.get(test_instance_json["parameters"])
+            if response.status_code == 200:
+                all_parameters = response.json()
+            else:
+                raise Exception(
+                    f"Unable to retrieve parameter file at {test_instance_json['parameters']}"
+                )
+        else:
+            all_parameters = {}
+        all_parameters.update(params)
+
         # Create the :class:`sciunit.Test` instance
-        test_instance = test_cls(observation=observation_data, **params)
+        test_instance = test_cls(
+            observation=observation_data, name=test_json["name"], **all_parameters
+        )
         test_instance.uuid = test_instance_json["id"]
         return test_instance
 
     def list_tests(self, size=1000000, from_index=0, **filters):
         """Retrieve a list of test definitions satisfying specified filters.
 
         The filters may specify one or more attributes that belong
@@ -1441,14 +1457,16 @@
     def _load_reference_data(self, uri_list):
         # Load the reference data ("observations").
         observation_data = []
         return_single = False
         if not isinstance(uri_list, list):
             uri_list = [uri_list]
             return_single = True
+        elif len(uri_list) == 1:
+            return_single = True
         for uri in uri_list:
             parse_result = urlparse(uri)
             datastore = URI_SCHEME_MAP[parse_result.scheme](auth=self.auth)
             observation_data.append(datastore.load_data(uri))
         if return_single:
             return observation_data[0]
         else:
@@ -1600,16 +1618,25 @@
 
         Examples
         --------
         >>> score = test.judge(model)
         >>> response = test_library.register_result(test_result=score)
         """
 
+        if hasattr(test_result, "exec_timestamp"):
+            timestamp = test_result.exec_timestamp
+        elif "timestamp" in test_result.related_data:
+            timestamp = test_result.related_data["timestamp"]
+        else:
+            timestamp = datetime.now()
+
         if collab_id is None:
             collab_id = test_result.related_data.get("collab_id", None)
+            if collab_id is None and data_store:
+                collab_id = data_store.collab_id
         if collab_id is None:
             raise Exception(
                 "Don't know where to register this result. Please specify `collab_id`!"
             )
 
         model_catalog = ModelCatalog.from_existing(self)
         model_instance_uuid = model_catalog.find_model_instance_else_add(
@@ -1626,36 +1653,42 @@
                 # the data store before passing to `register()`
             if data_store.collab_id is None:
                 data_store.collab_id = collab_id
             files_to_upload = []
             if "figures" in test_result.related_data:
                 files_to_upload.extend(test_result.related_data["figures"])
             if files_to_upload:
-                list_dict_files_to_upload = [
+                list_dict_files_uploaded = [
                     {"download_url": f["filepath"], "size": f["filesize"]}
                     for f in data_store.upload_data(files_to_upload)
                 ]
-                results_storage.extend(list_dict_files_to_upload)
+                results_storage.extend(list_dict_files_uploaded)
 
         url = self.url + "/results/"
         result_json = {
             "model_instance_id": model_instance_uuid,
             "test_instance_id": test_result.test.uuid,
             "results_storage": results_storage,
-            "score": int(test_result.score)
-            if isinstance(test_result.score, bool)
-            else test_result.score,
-            "passed": None
-            if "passed" not in test_result.related_data
-            else test_result.related_data["passed"],
-            # "platform": str(self._get_platform()), # not currently supported in v2
+            "score": (
+                int(test_result.score)
+                if isinstance(test_result.score, bool)
+                else test_result.score
+            ),
+            "passed": (
+                None
+                if "passed" not in test_result.related_data
+                else test_result.related_data["passed"]
+            ),
+            "timestamp": timestamp.isoformat(),
             "project_id": collab_id,
-            "normalized_score": int(test_result.score)
-            if isinstance(test_result.score, bool)
-            else test_result.score,
+            "normalized_score": (
+                int(test_result.score)
+                if isinstance(test_result.score, bool)
+                else test_result.score
+            ),
         }
 
         headers = {"Content-type": "application/json"}
         response = requests.post(
             url,
             data=json.dumps(result_json),
             auth=self.auth,
@@ -1916,14 +1949,15 @@
         * cell_type
         * model_scope
         * abstraction_level
         * author
         * owner
         * organization
         * collab_id
+        * format
         * private
 
         Parameters
         ----------
         size : positive integer
             Max number of models to be returned; default is set to 1000000.
         from_index : positive integer
@@ -1951,14 +1985,15 @@
             "cell_type",
             "model_scope",
             "abstraction_level",
             "author",
             "owner",
             "organization",
             "collab_id",
+            "format",
             "private",
         ]
         params = locals()["filters"]
         for filter in params:
             if filter not in valid_filters:
                 raise ValueError(
                     "The specified filter '{}' is an invalid filter!\nValid filters are: {}".format(
```

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/datastores.py` & `hbp_validation_framework-0.8.2/hbp_validation_framework/datastores.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,17 +197,24 @@
         for local_path, relative_path in zip(file_paths, relative_paths):
             remote_path = os.path.join(self.base_folder, relative_path)
             if not overwrite:
                 if remote_path in existing_files:
                     warn(f"File {remote_path} already exists and you have set overwrite=False")
 
             self.bucket.upload(local_path, remote_path)
+
+            # try to resolve the data-proxy path
+            remote_url = f"https://data-proxy.ebrains.eu/api/v1/buckets/{self.collab_id}/{remote_path}"
+            response = requests.get(remote_url, allow_redirects=False)
+            if response.status_code == 307:
+                remote_url = response.headers["location"]
+
             uploaded_file_paths.append(
                 {
-                    "filepath": f"https://data-proxy.ebrains.eu/api/v1/buckets/{self.collab_id}/{self.base_folder}/{remote_path}",
+                    "filepath": remote_url,
                     "filesize": os.stat(local_path).st_size,
                 }
             )
         return uploaded_file_paths
 
 
 class HTTPDataStore(object):
@@ -235,37 +242,39 @@
                         "https://senselab.med.yale.edu/modeldb/"
                     ) and url.endswith("&mime=application/zip"):
                         filename = req.headers["Content-Disposition"].split(
                             "filename="
                         )[1]
                     else:
                         filename = url.split("/")[-1]
-                local_path = os.path.join(local_directory, filename)
-                # local_path = os.path.join(local_directory, os.path.basename(urlparse(url).path))
-                if os.path.exists(local_path):
-                    raise FileExistsError(
-                        "Target file path `{}` already exists!\nSet `overwrite=True` if you wish overwrite existing files!".format(
-                            local_path
+                    local_path = os.path.join(local_directory, filename)
+                    # local_path = os.path.join(local_directory, os.path.basename(urlparse(url).path))
+                    if os.path.exists(local_path):
+                        raise FileExistsError(
+                            "Target file path `{}` already exists!\nSet `overwrite=True` if you wish overwrite existing files!".format(
+                                local_path
+                            )
                         )
-                    )
 
         for url in remote_paths:
             req = requests.head(url)
             if req.status_code == 200:
                 if url.startswith(
                     "https://senselab.med.yale.edu/modeldb/"
                 ) and url.endswith("&mime=application/zip"):
                     filename = req.headers["Content-Disposition"].split("filename=")[1]
                 else:
                     filename = url.split("/")[-1]
-            local_path = os.path.join(local_directory, filename)
-            # local_path = os.path.join(local_directory, os.path.basename(urlparse(url).path))
-            Path(os.path.dirname(local_path)).mkdir(parents=True, exist_ok=True)
-            filename, headers = urlretrieve(url, local_path)
-            local_paths.append(filename)
+                local_path = os.path.join(local_directory, filename)
+                # local_path = os.path.join(local_directory, os.path.basename(urlparse(url).path))
+                Path(os.path.dirname(local_path)).mkdir(parents=True, exist_ok=True)
+                filename, headers = urlretrieve(url, local_path)
+                local_paths.append(filename)
+            else:
+                print(f"Unable to download file from {url}. Error message {req.text}")
         return local_paths
 
     def load_data(self, remote_path):
         content_type, encoding = mimetypes.guess_type(remote_path)
         if content_type == "application/json":
             return requests.get(remote_path).json()
         else:
```

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/CHANGELOG.md` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/LICENSE` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/LICENSE`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/README.md` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/README.md`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/data.js` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/data.js`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/document.json` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/document.json`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/favicon.ico` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/index.htm` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/index.htm`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/jsonTreeViewer.js` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/jsonTreeViewer.js`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/App.js` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/App.js`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/README.md` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/README.md`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/app.css` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/app.css`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/docs/index.htm` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/docs/index.htm`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/docs/main.css` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/docs/main.css`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/app/reset.css` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/app/reset.css`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/icons.svg` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/icons.svg`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.css` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.css`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.js` & `hbp_validation_framework-0.8.2/hbp_validation_framework/jsonTreeViewer/libs/jsonTree/jsonTree.js`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/sample.py` & `hbp_validation_framework-0.8.2/hbp_validation_framework/sample.py`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/templates/report_template.html` & `hbp_validation_framework-0.8.2/hbp_validation_framework/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/utils.py` & `hbp_validation_framework-0.8.2/hbp_validation_framework/utils.py`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework/versioning.py` & `hbp_validation_framework-0.8.2/hbp_validation_framework/versioning.py`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/hbp_validation_framework.egg-info/SOURCES.txt` & `hbp_validation_framework-0.8.2/hbp_validation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hbp_validation_framework-0.8.1/setup.py` & `hbp_validation_framework-0.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 json_files = package_files("hbp_validation_framework", "jsonTreeViewer")
 template_files = package_files("hbp_validation_framework", "templates")
 
 setup(
     name="hbp_validation_framework",
-    version="0.8.1",
+    version="0.8.2",
     packages=["hbp_validation_framework"],
     package_data={"": json_files + template_files},
     url="https://github.com/HumanBrainProject/hbp-validation-client",
     license="BSD",
     author="Andrew Davison and Shailesh Appukuttan",
     author_email="andrew.davison@unic.cnrs-gif.fr, shailesh.appukuttan@unic.cnrs-gif.fr",
     description="Python client for the EBRAINS Validation Framework web services",
```

