# Comparing `tmp/ezyquant-0.7.1.tar.gz` & `tmp/ezyquant-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-0.7.1.tar", last modified: Wed Jun  7 04:07:36 2023, max compression
+gzip compressed data, was "ezyquant-0.7.2.tar", last modified: Wed Jun  7 12:05:23 2023, max compression
```

## Comparing `ezyquant-0.7.1.tar` & `ezyquant-0.7.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 04:07:23.000000 ezyquant-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 04:07:36.461332 ezyquant-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-07 04:07:23.000000 ezyquant-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/ezyquant/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/ezyquant/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/ezyquant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 04:07:36.465332 ezyquant-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-07 04:07:23.000000 ezyquant-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 12:04:19.000000 ezyquant-0.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 12:05:23.944775 ezyquant-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-07 12:04:19.000000 ezyquant-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/ezyquant/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/ezyquant/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/backtesting/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23370 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-07 12:04:19.000000 ezyquant-0.7.2/ezyquant/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/ezyquant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 12:05:23.000000 ezyquant-0.7.2/ezyquant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 12:05:23.948775 ezyquant-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-07 12:04:19.000000 ezyquant-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:23.944775 ezyquant-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-07 12:04:19.000000 ezyquant-0.7.2/tests/test_utils.py
```

### Comparing `ezyquant-0.7.1/LICENSE.txt` & `ezyquant-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/PKG-INFO` & `ezyquant-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.1
+Version: 0.7.2
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.7.1/README.md` & `ezyquant-0.7.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-# Ezyquant
-
-Powerful backtest python library for Thai stocks
+<div align="center">
+  <img src="docs\source\_static\logo-text-right.svg">
+</div>
+
+-----------------
+
+# Ezyquant: Powerful backtest python library for Thai stocks
+
+[![PyPI](https://img.shields.io/pypi/v/ezyquant?label=PyPI)](https://pydoc.ezyquant.com/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ezyquant?label=PyPI%20Downloads)](https://pepy.tech/project/ezyquant)
+[![License](https://img.shields.io/pypi/l/ezyquant.svg)](https://github.com/ezyquant/ezyquant/blob/main/LICENSE.txt)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## Features
 
 - Backtest
 - Signal Creator
 - Data Reader
 
 ## Installation
 
-```
+```bash
 pip install ezyquant
 ```
 
 or
 
-```
+```bash
 pip install git+https://github.com/ezyquant/ezyquant
 ```
 
 ## Quick Example
 
-```
+```python
 import pandas as pd
 
 import ezyquant as ez
 from ezyquant import SETDataReader, backtest
 from ezyquant.backtest import Context
 
 ez.connect_sqlite("ezyquant.db")
@@ -56,15 +66,15 @@
     initial_cash=initial_cash,
     pct_commission=0.25,
 )
 ```
 
 Backtest report:
 
-```
+```python
                                port_value port_value_with_dividend
 pct_net_profit                   0.024916                 0.024916
 cagr                             0.025055                 0.025055
 pct_maximum_drawdown            -0.223604                -0.223604
 cagr_divided_maxdd               0.112052                 0.112052
 pct_win_per_trade                     1.0                      1.0
 std                               0.32582                  0.32582
```

### Comparing `ezyquant-0.7.1/ezyquant/backtesting/_backtesting.py` & `ezyquant-0.7.2/ezyquant/backtesting/_backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/backtesting/account.py` & `ezyquant-0.7.2/ezyquant/backtesting/account.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/backtesting/backtesting.py` & `ezyquant-0.7.2/ezyquant/backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/backtesting/context.py` & `ezyquant-0.7.2/ezyquant/backtesting/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/backtesting/position.py` & `ezyquant-0.7.2/ezyquant/backtesting/position.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/backtesting/trade.py` & `ezyquant-0.7.2/ezyquant/backtesting/trade.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/connect.py` & `ezyquant-0.7.2/ezyquant/connect.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/creator.py` & `ezyquant-0.7.2/ezyquant/creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/fields.py` & `ezyquant-0.7.2/ezyquant/fields.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/indicators.py` & `ezyquant-0.7.2/ezyquant/indicators.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,29 +350,23 @@
 
         rsi = _apply_t(ind, RSIIndicator.rsi)
 
         return rsi
 
     @staticmethod
     def rsi_divergence(
-        high: pd.DataFrame,
-        low: pd.DataFrame,
         close: pd.DataFrame,
         rsi_period: int = 14,
         pivot_up_thresh: float = 0.05,
         pivot_down_thresh: float = -0.05,
     ) -> pd.DataFrame:
         """Relative Strength Index (RSI) Divergence.
 
         Parameters
         ----------
-        high: pd.DataFrame
-            dataset 'High' dataframe.
-        low: pd.DataFrame
-            dataset 'Low' dataframe.
         close: pd.DataFrame
             dataset 'Close' dataframe.
         rsi_period: int = 14
             n period for RSI.
         pivot_up_thresh: float = 0.05
             threshold for pivot up.
         pivot_down_thresh: float = -0.05
@@ -780,15 +774,15 @@
         Pivot down threshold, by default -0.05
     """
     # Calculate RSI
     rsi_ = rsi(close, window=rsi_period)
 
     # Calculate pivot points using zigzag
     zz_ = zigzag.peak_valley_pivots(  # type: ignore
-        close,
+        close.to_numpy(),
         up_thresh=pivot_up_thresh,
         down_thresh=pivot_down_thresh,
     )
     close_pl = close[zz_ < 0]
     close_ph = close[zz_ > 0]
 
     # Calculate Divergence
```

### Comparing `ezyquant-0.7.1/ezyquant/reader.py` & `ezyquant-0.7.2/ezyquant/reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/report.py` & `ezyquant-0.7.2/ezyquant/report.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/utils.py` & `ezyquant-0.7.2/ezyquant/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant/validators.py` & `ezyquant-0.7.2/ezyquant/validators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/ezyquant.egg-info/PKG-INFO` & `ezyquant-0.7.2/ezyquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.1
+Version: 0.7.2
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.7.1/ezyquant.egg-info/SOURCES.txt` & `ezyquant-0.7.2/ezyquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/setup.py` & `ezyquant-0.7.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import re
 
 from setuptools import find_packages, setup
 
-NAME = "ezyquant"
-
 VERSIONFILE = "ezyquant/_version.py"
 verstrline = open(VERSIONFILE, "rt").read()
 VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     verstr = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 setup(
-    name=NAME,
+    name="ezyquant",
     packages=find_packages(include=["ezyquant", "ezyquant.*"]),
     version=verstr,
     description="Powerful backtest python library for Thai stocks",
     long_description="Powerful backtest python library for Thai stocks",
     author="Fintech (Thailand) Company Limited",
     author_email="admin@fintech.co.th",
     url="https://www.ezyquant.com/",
     maintainer="Fintech (Thailand) Company Limited",
     maintainer_email="admin@fintech.co.th",
     python_requires=">=3.8",
     install_requires=[
-        "pandas>=1.3",
+        "pandas>=1.5",
         "sqlalchemy>=2.0",
         "psycopg2-binary>=2.9",
         "ta>=0.10",
         "XlsxWriter>=3.0",
         "typing_extensions>=4.4",
         "quantstats>=0.0",
-        "zigzag>=0.3.2",
+        "zigzag==0.2.2",
     ],
     license="The MIT License (MIT)",
     classifiers=[
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ezyquant-0.7.1/tests/test_creator.py` & `ezyquant-0.7.2/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/tests/test_indicators.py` & `ezyquant-0.7.2/tests/test_indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,19 +143,17 @@
         self._check(result)
 
     @pytest.mark.parametrize("n_row", [1, 20])
     @pytest.mark.parametrize("n_col", [1, 20])
     def test_rsi_divergence(self, n_row: int, n_col: int):
         # Mock
         df1 = make_random_df(n_row=n_row, n_col=n_col)
-        df2 = make_random_df(n_row=n_row, n_col=n_col)
-        df3 = make_random_df(n_row=n_row, n_col=n_col)
 
         # Test
-        result = SETSignalCreator.ta.rsi_divergence(df1, df2, df3)
+        result = SETSignalCreator.ta.rsi_divergence(df1)
 
         # Check
         self._check(result)
 
     @pytest.mark.parametrize("n_row", [1, 20])
     @pytest.mark.parametrize("n_col", [1, 20])
     def test_sto(self, n_row: int, n_col: int):
```

### Comparing `ezyquant-0.7.1/tests/test_reader.py` & `ezyquant-0.7.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/tests/test_test_utils.py` & `ezyquant-0.7.2/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.1/tests/test_utils.py` & `ezyquant-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

