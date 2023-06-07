# Comparing `tmp/cvxreg-0.0.6.tar.gz` & `tmp/cvxreg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.0.6.tar", last modified: Mon Jun  5 17:27:08 2023, max compression
+gzip compressed data, was "cvxreg-0.0.7.tar", last modified: Wed Jun  7 21:29:24 2023, max compression
```

## Comparing `cvxreg-0.0.6.tar` & `cvxreg-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-05 17:26:58.000000 cvxreg-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-05 17:27:08.175946 cvxreg-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 17:26:58.000000 cvxreg-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/models/_penalized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/_param_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/extmath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-05 17:26:58.000000 cvxreg-0.0.6/cvxreg/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:27:08.175946 cvxreg-0.0.6/cvxreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:27:08.000000 cvxreg-0.0.6/cvxreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:27:08.175946 cvxreg-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-05 17:26:58.000000 cvxreg-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.190260 cvxreg-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 21:29:13.000000 cvxreg-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-07 21:29:24.190260 cvxreg-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-07 21:29:13.000000 cvxreg-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.182260 cvxreg-0.0.7/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.186260 cvxreg-0.0.7/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.190260 cvxreg-0.0.7/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/_param_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/_pyomo_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/extmath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.186260 cvxreg-0.0.7/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:29:23.000000 cvxreg-0.0.7/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:29:24.190260 cvxreg-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-07 21:29:13.000000 cvxreg-0.0.7/setup.py
```

### Comparing `cvxreg-0.0.6/LICENSE` & `cvxreg-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Convex Regression
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Convex Regression
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `cvxreg-0.0.6/PKG-INFO` & `cvxreg-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Package for Convex Regression
-Home-page: https://github.com/ConvexRegression/ConvexRegression
+Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://img.shields.io/pypi/v/cvxreg.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
+[![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
+[![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
+[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
 **cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
 
-The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/ConvexRegression). Please feel free to download and test it. We welcome any bug reports and feedback.
+The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/cvxreg). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI 
 
     pip install cvxreg
```

### Comparing `cvxreg-0.0.6/README.md` & `cvxreg-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-[![PyPI version](https://img.shields.io/pypi/v/cvxreg.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
-
-**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
-
-The core aims of this package are:
-* make convex regression models "easy to call" from python,
-* interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
-* focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
-
-## Installation
-
-The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/ConvexRegression). Please feel free to download and test it. We welcome any bug reports and feedback.
-
-#### PyPI 
-
-    pip install cvxreg
-
+[![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
+[![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
+[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
+
+**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+
+The core aims of this package are:
+* make convex regression models "easy to call" from python,
+* interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
+* focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
+
+## Installation
+
+The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/cvxreg). Please feel free to download and test it. We welcome any bug reports and feedback.
+
+#### PyPI 
+
+    pip install cvxreg
+
```

### Comparing `cvxreg-0.0.6/cvxreg/base.py` & `cvxreg-0.0.7/cvxreg/base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import numpy as np
-import inspect
-
-from .utils.check import check_x_y
-from .utils.check import check_array
-from .utils.check import _check_y
-from .utils._param_check import validate_parameter_constraints
-
-class BaseEstimator:
-    """Base class for all estimators in cvxreg."""
-
-    @classmethod
-    def _get_param_names(cls):
-        """Get parameter names for the estimator"""
-        init_signature = inspect.signature(cls.__init__)
-        # Consider the constructor parameters excluding 'self'
-        parameters = [
-            p for p in init_signature.parameters.values()
-            if p.name != "self" and p.kind != p.VAR_KEYWORD
-        ]
-        for p in parameters:
-            if p.kind == p.VAR_POSITIONAL:
-                raise RuntimeError(
-                    "cvxreg estimators should always "
-                    "specify their parameters in the signature"
-                    " of their __init__ (no varargs)."
-                    " %s with constructor %s doesn't "
-                    " follow this convention." % (cls, init_signature))
-        # Extract and sort argument names excluding 'self'
-        return sorted([p.name for p in parameters])
-    
-    def get_params(self, deep=True):
-        """Get parameters for this estimator.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            If True, will return the parameters for this estimator and
-            contained subobjects that are estimators.
-
-        Returns
-        -------
-        params : dict
-            Parameter names mapped to their values.
-        """
-        out = dict()
-        for key in self._get_param_names():
-            value = getattr(self, key, None)
-            if deep and hasattr(value, "get_params"):
-                deep_items = value.get_params().items()
-                out.update((key + "__" + k, val) for k, val in deep_items)
-            out[key] = value
-        return out
-
-    def _validate_data(self, 
-                       x="novalidattion", 
-                       y="novalidation"):
-        """Validate input data.
-        parameters
-        ----------
-        x : input object to be checked
-        if novalidation, x will not be validated.
-        y : input object to be checked shape of y should be (n, )
-        """
-        no_val_x = isinstance(x, str) and x == "novalidation"
-        no_val_y = y is None or isinstance(y, str) and y == "novalidation"
-
-        if no_val_x and no_val_y:
-            raise ValueError("Please input x or y.")
-        elif not no_val_x and no_val_y:
-            x = check_array(x)
-            out = x
-        elif no_val_x and not no_val_y:
-            y = _check_y(y)
-            out = y
-        else:
-            x, y = check_x_y(x, y)
-            out = x, y
-        return out
-    
-    def _validate_params(self):
-        """Validate types and values of constructor parameters
-
-        The expected type and values must be defined in the `_parameter_constraints`
-        class attribute, which is a dictionary `param_name: list of constraints`. See
-        the docstring of `validate_parameter_constraints` for a description of the
-        accepted constraints.
-        """
-        validate_parameter_constraints(
-            self._parameter_constraints,
-            self.get_params(deep=False),
-            caller_name=self.__class__.__name__,
+import numpy as np
+import inspect
+
+from .utils.check import check_x_y
+from .utils.check import check_array
+from .utils.check import _check_y
+from .utils._param_check import validate_parameter_constraints
+
+class BaseEstimator:
+    """Base class for all estimators in cvxreg."""
+
+    @classmethod
+    def _get_param_names(cls):
+        """Get parameter names for the estimator"""
+        init_signature = inspect.signature(cls.__init__)
+        # Consider the constructor parameters excluding 'self'
+        parameters = [
+            p for p in init_signature.parameters.values()
+            if p.name != "self" and p.kind != p.VAR_KEYWORD
+        ]
+        for p in parameters:
+            if p.kind == p.VAR_POSITIONAL:
+                raise RuntimeError(
+                    "cvxreg estimators should always "
+                    "specify their parameters in the signature"
+                    " of their __init__ (no varargs)."
+                    " %s with constructor %s doesn't "
+                    " follow this convention." % (cls, init_signature))
+        # Extract and sort argument names excluding 'self'
+        return sorted([p.name for p in parameters])
+    
+    def get_params(self, deep=True):
+        """Get parameters for this estimator.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            If True, will return the parameters for this estimator and
+            contained subobjects that are estimators.
+
+        Returns
+        -------
+        params : dict
+            Parameter names mapped to their values.
+        """
+        out = dict()
+        for key in self._get_param_names():
+            value = getattr(self, key, None)
+            if deep and hasattr(value, "get_params"):
+                deep_items = value.get_params().items()
+                out.update((key + "__" + k, val) for k, val in deep_items)
+            out[key] = value
+        return out
+
+    def _validate_data(self, 
+                       x="novalidattion", 
+                       y="novalidation"):
+        """Validate input data.
+        parameters
+        ----------
+        x : input object to be checked
+        if novalidation, x will not be validated.
+        y : input object to be checked shape of y should be (n, )
+        """
+        no_val_x = isinstance(x, str) and x == "novalidation"
+        no_val_y = y is None or isinstance(y, str) and y == "novalidation"
+
+        if no_val_x and no_val_y:
+            raise ValueError("Please input x or y.")
+        elif not no_val_x and no_val_y:
+            x = check_array(x)
+            out = x
+        elif no_val_x and not no_val_y:
+            y = _check_y(y)
+            out = y
+        else:
+            x, y = check_x_y(x, y)
+            out = x, y
+        return out
+    
+    def _validate_params(self):
+        """Validate types and values of constructor parameters
+
+        The expected type and values must be defined in the `_parameter_constraints`
+        class attribute, which is a dictionary `param_name: list of constraints`. See
+        the docstring of `validate_parameter_constraints` for a description of the
+        accepted constraints.
+        """
+        validate_parameter_constraints(
+            self._parameter_constraints,
+            self.get_params(deep=False),
+            caller_name=self.__class__.__name__,
         )
```

### Comparing `cvxreg-0.0.6/cvxreg/models/_base.py` & `cvxreg-0.0.7/cvxreg/models/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,131 @@
-# import dependencies
-from abc import ABCMeta, abstractmethod
-import numpy as np
-import pandas as pd
-from pystoned import CNLS
-
-from ..base import BaseEstimator
-from ..constant import Convex, Concave, OPT_DEFAULT, OPT_LOCAL
-from ..utils import tools
-from ..utils.extmath import yhat
-from ..utils._param_check import StrOptions
-
-class CRModel(BaseEstimator, metaclass=ABCMeta):
-    """
-    Base class for CR models
-    """
-    @abstractmethod
-    def fit(self):
-        """Fit model."""
-
-    def _decision_function(self, x):
-        tools.assert_optimized(self.optimization_status)
-        
-        x = self._validate_data(x)
-        y_hat = yhat(self.intercept_, self.coef_, x, fun=self.shape)
-        return y_hat
-    
-    def predict(self, x):
-        """
-        Predict the output variable
-
-        Args:
-            x (float): input variables.
-
-        Returns:
-            float: predicted output variable
-        """
-        return self._decision_function(x)
-    
-
-class CR(CRModel, CNLS.CNLS):
-    """
-    Convex Regression (CR) model
-    """
-    _parameter_constraints: dict = {
-        "shape": [StrOptions({Convex, Concave})],
-        'fit_intercept': ['boolean'],
-        'positive': ['boolean']
-    }
-    
-    def __init__(self, shape=Convex, positive=False, fit_intercept=True):
-        """CNLS model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            fun (String, optional): FUN_CVX (convex funtion) or FUN_CCV (concave funtion). Defaults to FUN_CVX.
-            positive (bool, optional): True if the coefficients are positive. Defaults to False.
-            fit_intercept (bool, optional): True if the model should include an intercept. Defaults to True.
-        """
-        
-        self.shape = shape
-        self.fit_intercept = fit_intercept
-        self.positive = positive
-
-
-    def fit(self, x, y, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        self._validate_params()
-        x, y = self._validate_data(x, y)
-
-        # interface with CNLS
-        if self.shape == Convex:
-            self.fun_var = CNLS.FUN_COST
-        elif self.shape == Concave:
-            self.fun_var = CNLS.FUN_PROD
-        if self.fit_intercept:
-            self.intercept = CNLS.RTS_VRS
-        else:
-            self.intercept = CNLS.RTS_CRS
-        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=self.fun_var, rts=self.intercept)
-        if self.positive:
-            self.__model__.beta.setlb(0.0)
-        else:
-            self.__model__.beta.setlb(None)
-
-        # optimize the model with solver
-        self.problem_status, self.optimization_status = tools.optimize_model(
-            self.__model__, email, solver)
-        
-        tools.assert_optimized(self.optimization_status)
-
-        alpha = list(self.__model__.alpha[:].value)
-
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-    
-        if self.fit_intercept:
-            self.intercept_ = np.array(alpha)
-            self.coef_ = beta.to_numpy()
-        else:
-            self.intercept_ = 0.0
-            self.coef_ = beta.to_numpy()
-
-        return self
+# import dependencies
+from abc import ABCMeta, abstractmethod
+import numpy as np
+import pandas as pd
+from pystoned import CNLS
+
+from ..base import BaseEstimator
+from ..constant import convex, concave
+from ..utils.extmath import yhat
+from ..utils._pyomo_opt import optimize_model, check_optimization_status
+from ..utils._param_check import StrOptions
+
+class CRModel(BaseEstimator, metaclass=ABCMeta):
+    """
+    Base class for CR models
+    """
+    @abstractmethod
+    def fit(self):
+        """Fit model."""
+
+    def _decision_function(self, x):
+        
+        x = self._validate_data(x)
+        y_hat = yhat(self.intercept_, self.coef_, x, fun=self.shape)
+        return y_hat
+    
+    def predict(self, x):
+        """
+        Predict the output variable
+
+        Args:
+            x (float): input variables.
+
+        Returns:
+            float: predicted output variable
+        """
+        return self._decision_function(x)
+    
+
+class CR(CRModel, CNLS.CNLS):
+    """
+    Convex Regression (CR) model.
+
+    parameters
+    ----------
+    shape : string, optional (default=Convex)
+        The shape of the estimated function. It can be either Convex or Concave.
+    positive : boolean, optional (default=False)
+        Whether the estimated function is monotonic increasing or not.
+    fit_intercept : boolean, optional (default=True)
+        Whether to calculate the intercept for this model. If set to False, no intercept will be used in calculations.
+    email : string, optional (default=None)
+        The email address for remote optimization. It will optimize locally if None is given.
+    solver : string, optional (default='mosek')
+        The solver chosen for optimization. It will optimize with mosek solver if None is given.
+    """
+
+
+    _parameter_constraints: dict = {
+        "shape": [StrOptions({convex, concave})],
+        'fit_intercept': ['boolean'],
+        'positive': ['boolean'],
+        'email': [None, str],
+        'solver': [str]
+    }
+    
+    def __init__(
+        self, 
+        shape=convex, 
+        positive=False, 
+        fit_intercept=True, 
+        email=None, 
+        solver='mosek'
+    ):
+        self.shape = shape
+        self.fit_intercept = fit_intercept
+        self.positive = positive
+        self.email = email
+        self.solver = solver
+
+    def fit(self, x, y):
+        """fit the model with solver
+
+        parameters
+        ----------
+        x : ndarray of shape (n_samples, n_features) data.
+        y : ndarray of shape (n_samples,) target values.
+
+        Returns
+        -------
+        self : returns an instance of self
+                Fitted model.
+        """
+        self._validate_params()
+        x, y = self._validate_data(x, y)
+
+        # interface with CNLS
+        if self.shape == convex:
+            fun_var = CNLS.FUN_COST
+        elif self.shape == concave:
+            fun_var = CNLS.FUN_PROD
+        if self.fit_intercept:
+            intercept = CNLS.RTS_VRS
+        else:
+            intercept = CNLS.RTS_CRS
+        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=intercept)
+        if self.positive:
+            self.__model__.beta.setlb(0.0)
+        else:
+            self.__model__.beta.setlb(None)
+
+        # optimize the model with solver
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, self.email, self.solver)
+        check_optimization_status(self.optimization_status)
+        
+        alpha = list(self.__model__.alpha[:].value)
+
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+    
+        if self.fit_intercept:
+            self.intercept_ = np.array(alpha)
+            self.coef_ = beta.to_numpy()
+        else:
+            self.intercept_ = 0.0
+            self.coef_ = beta.to_numpy()
+
+        return self
```

### Comparing `cvxreg-0.0.6/cvxreg/models/_penalized.py` & `cvxreg-0.0.7/cvxreg/models/_penalized.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,115 @@
-from numbers import Real
-
-import numpy as np
-import pandas as pd
-from pystoned import CNLS
-from pyomo.environ import Objective, minimize
-
-from ._base import CRModel
-from ..constant import Convex, Concave, OPT_DEFAULT, OPT_LOCAL
-from ..utils import tools
-from ..utils._param_check import Interval, StrOptions
-
-
-class PCR(CRModel, CNLS.CNLS):
-    """
-    Penalized Convex Regression (PCR) model
-    """
-
-    _parameter_constraints: dict = {
-        "c": [Interval(Real, 0, None)],
-        "shape": [StrOptions({Convex, Concave})],
-        'fit_intercept': ['boolean'],
-        'positive': ['boolean']
-    }
-
-    def __init__(self, c=1.0, shape=Convex, positive=False, fit_intercept=True):
-        """PCR model
-
-        Args:
-            y (float): output variable. 
-            x (float): input variables.
-            fun (String, optional): FUN_CVX (convex funtion) or FUN_CCV (concave funtion). Defaults to FUN_CVX.
-            positive (bool, optional): True if the coefficients are positive. Defaults to False.
-            fit_intercept (bool, optional): True if the model should include an intercept. Defaults to True.
-        """
-        
-        self.c = c
-        self.shape = shape
-        self.fit_intercept = fit_intercept
-        self.positive = positive
-
-    def fit(self, x, y, email=OPT_LOCAL, solver=OPT_DEFAULT):
-        """Optimize the function by requested method
-
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
-        """
-        self._validate_params()
-        x, y = self._validate_data(x, y)
-
-        if self.shape == Convex:
-            fun_var = CNLS.FUN_COST
-        elif self.shape == Concave:
-            fun_var = CNLS.FUN_PROD
-        if self.fit_intercept:
-            intercept = CNLS.RTS_VRS
-        else:
-            intercept = CNLS.RTS_CRS
-        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=intercept)
-
-        # new objective function
-        self.__model__.objective.deactivate()
-        self.__model__.new_objective = Objective(rule=self.__new_objective_rule(),
-                                                     sense=minimize,
-                                                     doc='objective function')
-
-        if self.positive:
-            self.__model__.beta.setlb(0.0)
-        else:
-            self.__model__.beta.setlb(None)
-
-        # TODO(error/warning handling): Check problem status after optimization
-        self.problem_status, self.optimization_status = tools.optimize_model(
-            self.__model__, email, solver)
-        
-        tools.assert_optimized(self.optimization_status)
-
-        alpha = list(self.__model__.alpha[:].value)
-
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
-    
-        if self.fit_intercept:
-            self.intercept_ = alpha
-            self.coef_ = beta.to_numpy()
-        else:
-            self.intercept_ = 0.0
-            self.coef_ = beta.to_numpy()
-        return self
-    
-    def __new_objective_rule(self):
-        """return new objective function"""
-        def objective_rule(model):
-            return sum(model.epsilon[i] ** 2 for i in model.I) \
-                + self.c * sum(model.beta[i, j] ** 2 for i in model.I for j in model.J)
+from numbers import Real
+
+import numpy as np
+import pandas as pd
+from pystoned import CNLS
+from pyomo.environ import Objective, minimize
+
+from ._base import CRModel
+from ..constant import convex, concave, OPT_DEFAULT, OPT_LOCAL
+from ..utils._pyomo_opt import check_optimization_status, optimize_model
+from ..utils._param_check import Interval, StrOptions
+
+
+class PCR(CRModel, CNLS.CNLS):
+    """
+    Penalized Convex Regression (PCR) model.
+
+    parameters
+    ----------
+    c : float, optional (default=1.0)
+        The penalty parameter.
+    shape : string, optional (default=Convex)
+        The shape of the estimated function. It can be either Convex or Concave.
+    positive : boolean, optional (default=False)
+        Whether the estimated function is monotonic increasing or not.
+    fit_intercept : boolean, optional (default=True)
+        Whether to calculate the intercept for this model. If set to False, no intercept will be used in calculations.
+    email : string, optional (default=None)
+        The email address for remote optimization. It will optimize locally if None is given.
+    solver : string, optional (default='mosek')
+        The solver chosen for optimization. It will optimize with mosek solver if None is given.
+    """
+
+    _parameter_constraints: dict = {
+        "c": [Interval(Real, 0, None)],
+        "shape": [StrOptions({convex, concave})],
+        'fit_intercept': ['boolean'],
+        'positive': ['boolean'],
+        'email': [None, str],
+        'solver': [str]
+    }
+
+    def __init__(
+        self, 
+        c=1.0, 
+        shape=convex, 
+        positive=False, 
+        fit_intercept=True,
+        email=None, 
+        solver='mosek'
+    ):
+        self.c = c
+        self.shape = shape
+        self.fit_intercept = fit_intercept
+        self.positive = positive
+        self.email = email
+        self.solver = solver
+
+    def fit(self, x, y):
+        """Optimize the function by requested method
+
+        Args:
+            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
+            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        """
+        self._validate_params()
+        x, y = self._validate_data(x, y)
+
+        if self.shape == convex:
+            fun_var = CNLS.FUN_COST
+        elif self.shape == concave:
+            fun_var = CNLS.FUN_PROD
+        if self.fit_intercept:
+            intercept = CNLS.RTS_VRS
+        else:
+            intercept = CNLS.RTS_CRS
+        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=intercept)
+
+        # new objective function
+        self.__model__.objective.deactivate()
+        self.__model__.new_objective = Objective(rule=self.__new_objective_rule(),
+                                                     sense=minimize,
+                                                     doc='objective function')
+
+        if self.positive:
+            self.__model__.beta.setlb(0.0)
+        else:
+            self.__model__.beta.setlb(None)
+
+                # optimize the model with solver
+        self.problem_status, self.optimization_status = optimize_model(
+            self.__model__, self.email, self.solver)
+        check_optimization_status(self.optimization_status)
+
+        alpha = list(self.__model__.alpha[:].value)
+
+        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
+                                                          list(self.__model__.beta[:, :].value))])
+        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
+        beta = beta.pivot(index='Name', columns='Key', values='Value')
+    
+        if self.fit_intercept:
+            self.intercept_ = alpha
+            self.coef_ = beta.to_numpy()
+        else:
+            self.intercept_ = 0.0
+            self.coef_ = beta.to_numpy()
+        return self
+    
+    def __new_objective_rule(self):
+        """return new objective function"""
+        def objective_rule(model):
+            return sum(model.epsilon[i] ** 2 for i in model.I) \
+                + self.c * sum(model.beta[i, j] ** 2 for i in model.I for j in model.J)
         return objective_rule
```

### Comparing `cvxreg-0.0.6/cvxreg/utils/_param_check.py` & `cvxreg-0.0.7/cvxreg/utils/_param_check.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,189 +1,206 @@
-from abc import ABC
-from abc import abstractmethod
-from numbers import Real,Integral
-
-import numpy as np
-
-class InvalidParameterError(ValueError):
-    """Exception class to raise if a parameter value is invalid."""
-
-def validate_parameter_constraints(parameter_constraints, params, caller_name):
-    """Validate types and values of constructor parameters.
-
-    Parameters
-    ----------
-    parameter_constraints : dict
-        A dictionary `param_name: list of constraints`, where `param_name` is a
-        string and the list of constraints is a list of `Constraint` objects.
-        See the docstring of `Constraint` for a description of the accepted
-        constraints.
-        Constraints can be:
-        -an Interval, in which case the parameter value must be in the range of numbers
-        -a StrOptions, in which case the parameter value must be one of the strings
-        -the string 'boolean', in which case the parameter value must be a boolean
-        -the string 'array-like', in which case the parameter value must be an array-like object
-    params : dict
-        A dictionary `param_name: param_value`, where `param_name` is a string
-        and `param_value` is the value passed to the constructor.
-    caller_name : str
-        The name of the calling function, used to format error messages.
-    """
-    for para_names, para_values in params.items():
-        if para_names not in parameter_constraints:
-            raise InvalidParameterError(
-                "Invalid parameter %s for estimator %s. "
-                "Check the list of available parameters "
-                "with `estimator.get_params().keys()`." %
-                (para_names, caller_name))
-        constraints = parameter_constraints[para_names]
-        constraints = [make_constraint(constraint) for constraint in constraints]
-        for constraint in constraints:
-            if constraint.check(para_values):
-                break
-            else:
-                raise InvalidParameterError(
-                    f"The parameter {para_names} must be {constraint}."
-                    f" Got {para_values} instead."
-                    )
-            
-def make_constraint(constraint):
-    """Make a constraint object from a user-provided value."""
-
-    if isinstance(constraint, type):
-        return _Instancesof(constraint)
-    if isinstance(constraint, (Interval, StrOptions)):
-        return constraint
-    if isinstance(constraint, str) and constraint == 'boolean':
-        return _booleans()
-    raise ValueError("Invalid constraint: %s" % constraint)
-
-
-class _Constraint(ABC):
-    """Base class for parameter constraints."""
-    
-    def __init__(self):
-        self.hidden = False
-
-    @abstractmethod
-    def check(self, value):
-        """Check that the parameter value satisfies the constraint.
-
-        Parameters
-        ----------
-        value : object
-            The parameter value to check.
-        """
-
-    @abstractmethod
-    def __repr__(self):
-        """Return a string representation of the constraint."""
-
-class RealNotInt(Real):
-    """Class representing a real number that is not an integer."""
-
-RealNotInt.register(float)
-    
-
-class _Instancesof(_Constraint):
-    """Constraint representing a list of allowed types."""
-
-    def __init__(self, types):
-        super().__init__()
-        self.types = types
-
-    def check(self, value):
-        return isinstance(value, self.types)
-    
-    def __repr__(self):
-        return "Instances of %s" % (self.types,)
-
-class Interval(_Constraint):
-    """Constraint representing a closed interval of numbers.
-
-    parameters
-    ----------
-    type : {numeric, int, float}
-        The type of the parameter values.
-    lower : numeric or None
-        The lower bound of the interval. If None, there is no lower bound.
-    upper : numeric or None
-        The upper bound of the interval. If None, there is no upper bound.
-    """
-
-    def __init__(self, type, lower, upper):
-        super().__init__()
-        self.type = type
-        self.lower = lower
-        self.upper = upper
-
-        self._check_params()
-    
-    def _check_params(self):
-        if self.type not in (Integral, Real, RealNotInt):
-            raise ValueError(
-                "type must be Integral, Real or RealNotInt"
-                "Got %s instead." % self.type)
-        if self.lower is not None and not isinstance(self.lower, Real):
-            raise ValueError("lower bound must be a real number")
-        if self.upper is not None and not isinstance(self.upper, Real):
-            raise ValueError("upper bound must be a real number")
-        if self.lower is not None and self.upper is not None and self.lower >= self.upper:
-            raise ValueError(
-                "lower bound must be less than or equal to upper bound."
-                " Got %s and %s instead." % (self.lower, self.upper)
-                )
-
-    def __contains__(self, value):
-        if np.isnan(value):
-            return False
-        if self.lower is not None and value < self.lower:
-            return False
-        if self.upper is not None and value > self.upper:
-            return False
-        return True
-    
-    def check(self, value):
-        if not isinstance(value, self.type):
-            return False
-        return value in self
-    
-    def __repr__(self):
-        return "Interval(%s, %s)" % (self.lower, self.upper)
-    
-
-class Options(_Constraint):
-    """Constraint representing a list of allowed options."""
-
-    def __init__(self, type, options):
-        super().__init__()
-        self.options = options
-        self.type = type
-
-    def check(self, value):
-        return isinstance(value, self.type) and value in self.options
-    
-    def __repr__(self):
-        return "Options: %s" % (self.options,)
-
-class StrOptions(Options):
-    """Constraint representing a list of allowed strings."""
-
-    def __init__(self, options):
-        super().__init__(str, options=options)
-    
-
-class _booleans(_Constraint):
-    """Base class for boolean constraints."""
-
-    def __init__(self):
-        super().__init__()
-        self._constraint = [
-            _Instancesof(bool),
-            _Instancesof(np.bool_)
-        ]
-
-    def check(self, value):
-        return any(constraint.check(value) for constraint in self._constraint)
-    
-    def __repr__(self):
+from abc import ABC
+from abc import abstractmethod
+from numbers import Real,Integral
+
+import numpy as np
+
+class InvalidParameterError(ValueError):
+    """Exception class to raise if a parameter value is invalid."""
+
+def validate_parameter_constraints(parameter_constraints, params, caller_name):
+    """Validate types and values of constructor parameters.
+
+    Parameters
+    ----------
+    parameter_constraints : dict
+        A dictionary `param_name: list of constraints`, where `param_name` is a
+        string and the list of constraints is a list of `Constraint` objects.
+        See the docstring of `Constraint` for a description of the accepted
+        constraints.
+        Constraints can be:
+        -an Interval, in which case the parameter value must be in the range of numbers
+        -a StrOptions, in which case the parameter value must be one of the strings
+        -the string 'boolean', in which case the parameter value must be a boolean
+        -the string 'array-like', in which case the parameter value must be an array-like object
+    params : dict
+        A dictionary `param_name: param_value`, where `param_name` is a string
+        and `param_value` is the value passed to the constructor.
+    caller_name : str
+        The name of the calling function, used to format error messages.
+    """
+    for para_names, para_values in params.items():
+        if para_names not in parameter_constraints:
+            raise InvalidParameterError(
+                "Invalid parameter %s for estimator %s. "
+                "Check the list of available parameters "
+                "with `estimator.get_params().keys()`." %
+                (para_names, caller_name))
+        
+        constraints = parameter_constraints[para_names]
+
+        if constraints == "novalidation":
+            continue
+
+        constraints = [make_constraint(constraint) for constraint in constraints]
+
+        for constraint in constraints:
+            if constraint.check(para_values):
+                break
+        else:
+            raise InvalidParameterError(
+                f"The parameter {para_names} must be {constraint}."
+                f" Got {para_values} instead."
+                )
+            
+def make_constraint(constraint):
+    """Make a constraint object from a user-provided value."""
+
+    if isinstance(constraint, type):
+        return _Instancesof(constraint)
+    if constraint is None:
+        return _NoneConstraint()
+    if isinstance(constraint, (Interval, StrOptions)):
+        return constraint
+    if isinstance(constraint, str) and constraint == 'boolean':
+        return _booleans()
+    raise ValueError("Invalid constraint: %s" % constraint)
+
+
+class _Constraint(ABC):
+    """Base class for parameter constraints."""
+    
+    def __init__(self):
+        self.hidden = False
+
+    @abstractmethod
+    def check(self, value):
+        """Check that the parameter value satisfies the constraint.
+
+        Parameters
+        ----------
+        value : object
+            The parameter value to check.
+        """
+
+    @abstractmethod
+    def __repr__(self):
+        """Return a string representation of the constraint."""
+
+class RealNotInt(Real):
+    """Class representing a real number that is not an integer."""
+
+RealNotInt.register(float)
+    
+
+class _Instancesof(_Constraint):
+    """Constraint representing a list of allowed types."""
+
+    def __init__(self, types):
+        super().__init__()
+        self.types = types
+
+    def check(self, value):
+        return isinstance(value, self.types)
+    
+    def __repr__(self):
+        return "Instances of %s" % (self.types,)
+
+class _NoneConstraint(_Constraint):
+    """Constraint representing the None singleton."""
+
+    def check(self, value):
+        return value is None
+    
+    def __repr__(self):
+        return "None"
+    
+class Interval(_Constraint):
+    """Constraint representing a closed interval of numbers.
+
+    parameters
+    ----------
+    type : {numeric, int, float}
+        The type of the parameter values.
+    lower : numeric or None
+        The lower bound of the interval. If None, there is no lower bound.
+    upper : numeric or None
+        The upper bound of the interval. If None, there is no upper bound.
+    """
+
+    def __init__(self, type, lower, upper):
+        super().__init__()
+        self.type = type
+        self.lower = lower
+        self.upper = upper
+
+        self._check_params()
+    
+    def _check_params(self):
+        if self.type not in (Integral, Real, RealNotInt):
+            raise ValueError(
+                "type must be Integral, Real or RealNotInt"
+                "Got %s instead." % self.type)
+        if self.lower is not None and not isinstance(self.lower, Real):
+            raise ValueError("lower bound must be a real number")
+        if self.upper is not None and not isinstance(self.upper, Real):
+            raise ValueError("upper bound must be a real number")
+        if self.lower is not None and self.upper is not None and self.lower >= self.upper:
+            raise ValueError(
+                "lower bound must be less than or equal to upper bound."
+                " Got %s and %s instead." % (self.lower, self.upper)
+                )
+
+    def __contains__(self, value):
+        if np.isnan(value):
+            return False
+        if self.lower is not None and value < self.lower:
+            return False
+        if self.upper is not None and value > self.upper:
+            return False
+        return True
+    
+    def check(self, value):
+        if not isinstance(value, self.type):
+            return False
+        return value in self
+    
+    def __repr__(self):
+        return "Interval(%s, %s)" % (self.lower, self.upper)
+    
+
+class Options(_Constraint):
+    """Constraint representing a list of allowed options."""
+
+    def __init__(self, type, options):
+        super().__init__()
+        self.options = options
+        self.type = type
+
+    def check(self, value):
+        return isinstance(value, self.type) and value in self.options
+    
+    def __repr__(self):
+        return "Options: %s" % (self.options,)
+
+class StrOptions(Options):
+    """Constraint representing a list of allowed strings."""
+
+    def __init__(self, options):
+        super().__init__(str, options=options)
+    
+
+class _booleans(_Constraint):
+    """Base class for boolean constraints."""
+
+    def __init__(self):
+        super().__init__()
+        self._constraint = [
+            _Instancesof(bool),
+            _Instancesof(np.bool_)
+        ]
+
+    def check(self, value):
+        return any(constraint.check(value) for constraint in self._constraint)
+    
+    def __repr__(self):
         return ("Boolean")
```

### Comparing `cvxreg-0.0.6/cvxreg/utils/check.py` & `cvxreg-0.0.7/cvxreg/utils/check.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import numpy as np
-
-def _num_samples(x):
-    """Return number of samples in array-like x."""
-    message = "Expected sequence or array-like, got %s" % type(x)
-    if hasattr(x, "fit") and callable(x.fit):
-        raise TypeError(message)
-    if not hasattr(x, "__len__") and not hasattr(x, "shape"):
-        if hasattr(x, "__array__"):
-            x = np.asarray(x)
-        else:
-            raise TypeError(message)
-    if hasattr(x, "shape"):
-        if len(x.shape) == 0:
-            raise TypeError(
-                "Singleton array %r cannot be considered a valid"
-                " collection." % x)
-        return x.shape[0]
-    else:
-        return len(x)
-    
-def check_array(array, ensure_2d=True):
-    """Input check on array and list.
-    parameters
-    ----------
-    array : input object to be checked
-    """
-    if isinstance(array, np.matrix):
-        raise ValueError("Please input a numpy array instead of a numpy matrix.")
-    
-    
-    array = np.array(array)
-
-    if ensure_2d:
-        if array.ndim == 0:
-            raise ValueError("Please input a 2D array.")
-        elif array.ndim == 1:
-            raise ValueError("Expected 2D array, got 1D array instead:\narray={}.\n"
-                            "Reshape your data either using array.reshape(-1, 1) if "
-                            "your data has a single feature or array.reshape(1, -1) ")
-    return array
-    
-def _check_y(y):
-    """Input check for y."""
-    if isinstance(y, np.matrix):
-        raise ValueError("Please input a numpy array instead of a numpy matrix.")
-    y = check_array(y, ensure_2d=False)
-
-    shape = y.shape
-    if len(shape) == 1:
-        return y
-    if len(shape) == 2 and shape[1] == 1:
-        return y.ravel()
-    raise ValueError("y should be a 1d array, got an array of shape {} instead.".format(shape))
-
-def check_consistent_length(*arrays):
-    """Check that all arrays have consistent first dimensions.
-    Checks whether all objects in arrays have the same shape or length.
-
-    Parameters
-    ----------
-    *arrays : list or tuple of input objects.
-        Objects that will be checked for consistent length.
-    """
-    lengths = [_num_samples(x) for x in arrays if x is not None]
-    uniques = np.unique(lengths)
-    if len(uniques) > 1:
-        raise ValueError("Found input variables with inconsistent numbers of samples: %r" % [int(l) for l in lengths])
-    
-def check_x_y(x, y):
-    """Input check for x and y.
-    Check x and y for consistent length, enforece x to be 2d and y 1d.
-
-    Parameters
-    ----------
-    x : {ndarray, list}
-        Input data.
-    y : {ndarray, list}
-        Output data.
-    """
-    if y is None:
-        raise ValueError("y must be specified.")
-    x = check_array(x)
-    y = _check_y(y)
-
-    check_consistent_length(x, y)
-
-    return x, y
+import numpy as np
+
+def _num_samples(x):
+    """Return number of samples in array-like x."""
+    message = "Expected sequence or array-like, got %s" % type(x)
+    if hasattr(x, "fit") and callable(x.fit):
+        raise TypeError(message)
+    if not hasattr(x, "__len__") and not hasattr(x, "shape"):
+        if hasattr(x, "__array__"):
+            x = np.asarray(x)
+        else:
+            raise TypeError(message)
+    if hasattr(x, "shape"):
+        if len(x.shape) == 0:
+            raise TypeError(
+                "Singleton array %r cannot be considered a valid"
+                " collection." % x)
+        return x.shape[0]
+    else:
+        return len(x)
+    
+def check_array(array, ensure_2d=True):
+    """Input check on array and list.
+    parameters
+    ----------
+    array : input object to be checked
+    """
+    if isinstance(array, np.matrix):
+        raise ValueError("Please input a numpy array instead of a numpy matrix.")
+    
+    
+    array = np.array(array)
+
+    if ensure_2d:
+        if array.ndim == 0:
+            raise ValueError("Please input a 2D array.")
+        elif array.ndim == 1:
+            raise ValueError("Expected 2D array, got 1D array instead:\narray={}.\n"
+                            "Reshape your data either using array.reshape(-1, 1) if "
+                            "your data has a single feature or array.reshape(1, -1) ")
+    return array
+    
+def _check_y(y):
+    """Input check for y."""
+    if isinstance(y, np.matrix):
+        raise ValueError("Please input a numpy array instead of a numpy matrix.")
+    y = check_array(y, ensure_2d=False)
+
+    shape = y.shape
+    if len(shape) == 1:
+        return y
+    if len(shape) == 2 and shape[1] == 1:
+        return y.ravel()
+    raise ValueError("y should be a 1d array, got an array of shape {} instead.".format(shape))
+
+def check_consistent_length(*arrays):
+    """Check that all arrays have consistent first dimensions.
+    Checks whether all objects in arrays have the same shape or length.
+
+    Parameters
+    ----------
+    *arrays : list or tuple of input objects.
+        Objects that will be checked for consistent length.
+    """
+    lengths = [_num_samples(x) for x in arrays if x is not None]
+    uniques = np.unique(lengths)
+    if len(uniques) > 1:
+        raise ValueError("Found input variables with inconsistent numbers of samples: %r" % [int(l) for l in lengths])
+    
+def check_x_y(x, y):
+    """Input check for x and y.
+    Check x and y for consistent length, enforece x to be 2d and y 1d.
+
+    Parameters
+    ----------
+    x : {ndarray, list}
+        Input data.
+    y : {ndarray, list}
+        Output data.
+    """
+    if y is None:
+        raise ValueError("y must be specified.")
+    x = check_array(x)
+    y = _check_y(y)
+
+    check_consistent_length(x, y)
+
+    return x, y
```

### Comparing `cvxreg-0.0.6/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.0.7/cvxreg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Package for Convex Regression
-Home-page: https://github.com/ConvexRegression/ConvexRegression
+Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![PyPI version](https://img.shields.io/pypi/v/cvxreg.svg?maxAge=3600)](https://pypi.org/project/cvxreg/)[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
+[![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
+[![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
+[![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
 **cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
 * interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
 
-The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/ConvexRegression). Please feel free to download and test it. We welcome any bug reports and feedback.
+The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/cvxreg). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI 
 
     pip install cvxreg
```

### Comparing `cvxreg-0.0.6/setup.py` & `cvxreg-0.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    README = readme_file.read()
-
-setup_args = dict(
-    name='cvxreg',
-    version='0.0.6',
-    description='A Python Package for Convex Regression',
-    long_description_content_type="text/markdown",
-    long_description=README,
-    license='MIT',
-    packages=find_packages(),
-    author='Zhiqiang Liao',
-    author_email='zhiqiang.liao@aalto.fi',
-    keywords=['ML', 'Prediction', 'Regression'],
-    url='https://github.com/ConvexRegression/ConvexRegression',
-    download_url='https://pypi.org/project/cvxreg/',
-    include_package_data=True,
-    zip_safe=False,
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Science/Research',
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-)
-
-install_requires = [
-    'numpy>=1.19.2',
-    'pandas>=1.1.3',
-    'pystoned>=0.6.0',
-    'scipy>=1.5.2'
-]
-
-if __name__ == '__main__':
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    README = readme_file.read()
+
+setup_args = dict(
+    name='cvxreg',
+    version='0.0.7',
+    description='A Python Package for Convex Regression',
+    long_description_content_type="text/markdown",
+    long_description=README,
+    license='MIT',
+    packages=find_packages(),
+    author='Zhiqiang Liao',
+    author_email='zhiqiang.liao@aalto.fi',
+    keywords=['ML', 'Prediction', 'Regression'],
+    url='https://github.com/ConvexRegression/cvxreg',
+    download_url='https://pypi.org/project/cvxreg/',
+    include_package_data=True,
+    zip_safe=False,
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Science/Research',
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+)
+
+install_requires = [
+    'numpy>=1.19.2',
+    'pandas>=1.1.3',
+    'pystoned>=0.6.0',
+    'pyomo>=5.7.3'
+]
+
+if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

