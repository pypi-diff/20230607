# Comparing `tmp/ezyquant-0.7.0.tar.gz` & `tmp/ezyquant-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-0.7.0.tar", last modified: Fri Apr 21 06:29:51 2023, max compression
+gzip compressed data, was "ezyquant-0.7.1.tar", last modified: Wed Jun  7 04:07:36 2023, max compression
```

## Comparing `ezyquant-0.7.0.tar` & `ezyquant-0.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-21 06:29:35.000000 ezyquant-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-21 06:29:51.577684 ezyquant-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-21 06:29:35.000000 ezyquant-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.573684 ezyquant-0.7.0/ezyquant/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/ezyquant/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/ezyquant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 06:29:51.577684 ezyquant-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-21 06:29:35.000000 ezyquant-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 04:07:23.000000 ezyquant-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 04:07:36.461332 ezyquant-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-07 04:07:23.000000 ezyquant-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/ezyquant/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/ezyquant/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/backtesting/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-07 04:07:23.000000 ezyquant-0.7.1/ezyquant/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/ezyquant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 04:07:36.000000 ezyquant-0.7.1/ezyquant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 04:07:36.465332 ezyquant-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-07 04:07:23.000000 ezyquant-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:36.461332 ezyquant-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-06-07 04:07:23.000000 ezyquant-0.7.1/tests/test_utils.py
```

### Comparing `ezyquant-0.7.0/LICENSE.txt` & `ezyquant-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/PKG-INFO` & `ezyquant-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.0
+Version: 0.7.1
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
 Project-URL: Documentation, https://pydoc.ezyquant.com/
 Project-URL: Bug Reports, https://github.com/ezyquant/ezyquant/issues
 Project-URL: Source, https://github.com/ezyquant/ezyquant
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8.6
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Powerful backtest python library for Thai stocks
```

### Comparing `ezyquant-0.7.0/README.md` & `ezyquant-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/backtesting/_backtesting.py` & `ezyquant-0.7.1/ezyquant/backtesting/_backtesting.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from .context import Context
 from .position import SETPosition
 from .trade import SETTrade
 
 position_df_columns = ["timestamp"] + [i.name for i in fields(SETPosition)]
 trade_df_columns = [i.name for i in fields(SETTrade)]
 
+nan = float("nan")
+
 
 def _backtest(
     initial_cash: float,
     signal_df: pd.DataFrame,
     backtest_algorithm: Callable[[Context], float],
     close_price_df: pd.DataFrame,
     price_match_df: pd.DataFrame,
@@ -142,15 +144,15 @@
             ctx.close_price = acct.close_price_dict[k]
             if k in acct.position_dict:
                 pos = acct.position_dict[k]
                 ctx.volume = pos.volume
                 ctx.cost_price = pos.cost_price
             else:
                 ctx.volume = 0.0
-                ctx.cost_price = 0.0
+                ctx.cost_price = nan
 
             trade_volume = backtest_algorithm(ctx)
 
             if trade_volume > 0:
                 buy_volume_d[k] = trade_volume
             elif trade_volume < 0:
                 sell_volume_d[k] = trade_volume
```

### Comparing `ezyquant-0.7.0/ezyquant/backtesting/account.py` & `ezyquant-0.7.1/ezyquant/backtesting/account.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/backtesting/backtesting.py` & `ezyquant-0.7.1/ezyquant/backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/backtesting/context.py` & `ezyquant-0.7.1/ezyquant/backtesting/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/backtesting/position.py` & `ezyquant-0.7.1/ezyquant/backtesting/position.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/backtesting/trade.py` & `ezyquant-0.7.1/ezyquant/backtesting/trade.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/connect.py` & `ezyquant-0.7.1/ezyquant/connect.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/creator.py` & `ezyquant-0.7.1/ezyquant/creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         ...     symbol_list=["COM7", "MALEE"],
         ... )
         >>> ssc.get_data(
         ...     field="close",
         ...     timeframe="daily",
         ...     value_by="stock",
         ...     method="constant",
-        ...     period=0,
+        ...     period=1,
         ...     shift=0,
         ... )
                       COM7  MALEE
         2022-01-04  41.875   6.55
         2022-01-05  41.625   6.50
         2022-01-06  41.500   6.50
         2022-01-07  41.000   6.40
@@ -210,15 +210,15 @@
         2022-04-01  42.500   5.70
 
         >>> ssc.get_data(
         ...     field="cash",
         ...     timeframe="quarterly",
         ...     value_by="stock",
         ...     method="constant",
-        ...     period=0,
+        ...     period=1,
         ...     shift=0,
         ... )
                           COM7     MALEE
         2022-01-04         NaN       NaN
         2022-01-05         NaN       NaN
         2022-01-06         NaN       NaN
         2022-01-07         NaN       NaN
```

### Comparing `ezyquant-0.7.0/ezyquant/fields.py` & `ezyquant-0.7.1/ezyquant/fields.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/indicators.py` & `ezyquant-0.7.1/ezyquant/indicators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+import operator
 from typing import Callable, Tuple
 
+import numpy as np
 import pandas as pd
-from ta.momentum import ROCIndicator, RSIIndicator, StochasticOscillator
+import zigzag
+from ta.momentum import ROCIndicator, RSIIndicator, StochasticOscillator, rsi
 from ta.trend import MACD, ADXIndicator, CCIIndicator, IchimokuIndicator, PSARIndicator
 from ta.utils import _ema, _sma
 from ta.volatility import (
     AverageTrueRange,
     BollingerBands,
     DonchianChannel,
     KeltnerChannel,
 )
 
 from .errors import InputError
 
+nan = float("nan")
+
 
 class TA:
     """Trend Indicators."""
 
     @staticmethod
     def sma(close: pd.DataFrame, window: int, fillna: bool = False) -> pd.DataFrame:
         """Simple Moving Average (SMA)
@@ -344,14 +349,60 @@
         )
 
         rsi = _apply_t(ind, RSIIndicator.rsi)
 
         return rsi
 
     @staticmethod
+    def rsi_divergence(
+        high: pd.DataFrame,
+        low: pd.DataFrame,
+        close: pd.DataFrame,
+        rsi_period: int = 14,
+        pivot_up_thresh: float = 0.05,
+        pivot_down_thresh: float = -0.05,
+    ) -> pd.DataFrame:
+        """Relative Strength Index (RSI) Divergence.
+
+        Parameters
+        ----------
+        high: pd.DataFrame
+            dataset 'High' dataframe.
+        low: pd.DataFrame
+            dataset 'Low' dataframe.
+        close: pd.DataFrame
+            dataset 'Close' dataframe.
+        rsi_period: int = 14
+            n period for RSI.
+        pivot_up_thresh: float = 0.05
+            threshold for pivot up.
+        pivot_down_thresh: float = -0.05
+            threshold for pivot down.
+
+        Returns
+        -------
+        pd.DataFrame
+            Relative Strength Index (RSI) Divergence
+        """
+        out = close.apply(
+            lambda x: rsi_divergence(
+                close=x,
+                rsi_period=rsi_period,
+                pivot_up_thresh=pivot_up_thresh,
+                pivot_down_thresh=pivot_down_thresh,
+            )
+        )
+
+        # Return only signal
+        out = np.sign(out)
+        assert isinstance(out, pd.DataFrame)
+        out = out.fillna(0)
+        return out
+
+    @staticmethod
     def sto(
         high: pd.DataFrame,
         low: pd.DataFrame,
         close: pd.DataFrame,
         window: int = 14,
         smooth_window: int = 3,
         fillna: bool = False,
@@ -663,7 +714,114 @@
 
 def _apply_t(series: pd.Series, func: Callable) -> pd.DataFrame:
     df = series.apply(func).T
     if df.empty:
         raise InputError(f"{func.__name__} returned an empty dataframe")
     assert isinstance(df, pd.DataFrame)
     return df
+
+
+"""
+Pivot
+"""
+
+
+def pivot_points_high(high: pd.Series, left_bars: int, right_bars: int) -> pd.Series:
+    """Pivot Points High.
+
+    High is the highest high in a window between left_bars and
+    right_bars. If multiple bars have the same high, the most right bar
+    is used.
+    """
+    max_ = high.rolling(window=left_bars + 1).max()
+    max_right = high.rolling(window=right_bars).max().shift(-right_bars)
+
+    return high.where((max_ == high) & (max_ > max_right))
+
+
+def pivot_points_low(low: pd.Series, left_bars: int, right_bars: int) -> pd.Series:
+    """Pivot Points Low.
+
+    Low is the lowest low in a window between left_bars and right_bars.
+    If multiple bars have the same low, the most right bar is used.
+    """
+    min_ = low.rolling(window=left_bars + 1).min()
+    min_right = low.rolling(window=right_bars).min().shift(-right_bars)
+
+    return low.where((min_ == low) & (min_ < min_right))
+
+
+"""
+RSI Divergence
+"""
+
+
+def rsi_divergence(
+    close: pd.Series,
+    rsi_period: int = 14,
+    pivot_up_thresh: float = 0.05,
+    pivot_down_thresh: float = -0.05,
+) -> pd.Series:
+    """Return Positive RSI of the bullish divergence points and Negative RSI of
+    the bearish divergence points.
+
+    Parameters
+    ----------
+    high : pd.Series
+        Series of 'high' prices.
+    low : pd.Series
+        Series of 'low' prices.
+    close : pd.Series
+        Series of 'close' prices.
+    rsi_period : int, optional
+        RSI period, by default 14
+    pivot_up_thresh : int
+        Pivot up threshold, by default 0.05
+    pivot_down_thresh : int
+        Pivot down threshold, by default -0.05
+    """
+    # Calculate RSI
+    rsi_ = rsi(close, window=rsi_period)
+
+    # Calculate pivot points using zigzag
+    zz_ = zigzag.peak_valley_pivots(  # type: ignore
+        close,
+        up_thresh=pivot_up_thresh,
+        down_thresh=pivot_down_thresh,
+    )
+    close_pl = close[zz_ < 0]
+    close_ph = close[zz_ > 0]
+
+    # Calculate Divergence
+    bullish = _divergence(close_pl, rsi_, bullish=True)
+    bearish = _divergence(close_ph, rsi_, bullish=False)
+
+    return bullish.fillna(-bearish)
+
+
+def _divergence(
+    price_pivot: pd.Series, indicator: pd.Series, bullish: bool = True
+) -> pd.Series:
+    """Divergence.
+
+    Parameters
+    ----------
+    price_pivot : pd.Series
+        Price pivot points. low for bullish divergence and high for bearish divergence.
+    indicator : pd.Series
+        indicator series.
+    bullish : bool, optional
+        bullish or bearish divergence, by default True
+
+    Returns
+    -------
+    pd.Series
+        Divergence series. Not NaN when divergence occurs.
+    """
+    indicator_pivot = indicator[price_pivot.index]
+
+    op = operator.lt if bullish else operator.gt
+
+    return indicator.where(
+        op(price_pivot, price_pivot.shift(1))
+        & op(indicator_pivot.shift(1), indicator_pivot)
+    )
```

### Comparing `ezyquant-0.7.0/ezyquant/reader.py` & `ezyquant-0.7.1/ezyquant/reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/report.py` & `ezyquant-0.7.1/ezyquant/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,15 +669,15 @@
             (self.pct_avg_profit * self.win_trades)
             + (self.pct_avg_loss * self.loss_trades)
         ) / self.all_trades
 
     @property
     @return_nan_on_failure
     def avg_bar_held(self) -> float:
-        """sum of bars in trades / number of trades."""
+        """Sum of bars in trades / number of trades."""
         df = self.summary_trade_df
         return df["hold_days"].mean()
 
     @property
     @return_nan_on_failure
     def win_trades(self) -> int:
         """Number of win trades."""
```

### Comparing `ezyquant-0.7.0/ezyquant/utils.py` & `ezyquant-0.7.1/ezyquant/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant/validators.py` & `ezyquant-0.7.1/ezyquant/validators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/ezyquant.egg-info/PKG-INFO` & `ezyquant-0.7.1/ezyquant.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.7.0
+Version: 0.7.1
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
 Project-URL: Documentation, https://pydoc.ezyquant.com/
 Project-URL: Bug Reports, https://github.com/ezyquant/ezyquant/issues
 Project-URL: Source, https://github.com/ezyquant/ezyquant
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8.6
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Powerful backtest python library for Thai stocks
```

### Comparing `ezyquant-0.7.0/ezyquant.egg-info/SOURCES.txt` & `ezyquant-0.7.1/ezyquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/setup.py` & `ezyquant-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     description="Powerful backtest python library for Thai stocks",
     long_description="Powerful backtest python library for Thai stocks",
     author="Fintech (Thailand) Company Limited",
     author_email="admin@fintech.co.th",
     url="https://www.ezyquant.com/",
     maintainer="Fintech (Thailand) Company Limited",
     maintainer_email="admin@fintech.co.th",
-    python_requires=">=3.8.6",
+    python_requires=">=3.8",
     install_requires=[
         "pandas>=1.3",
         "sqlalchemy>=2.0",
         "psycopg2-binary>=2.9",
         "ta>=0.10",
         "XlsxWriter>=3.0",
         "typing_extensions>=4.4",
         "quantstats>=0.0",
+        "zigzag>=0.3.2",
     ],
     license="The MIT License (MIT)",
     classifiers=[
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ezyquant-0.7.0/tests/test_creator.py` & `ezyquant-0.7.1/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/tests/test_reader.py` & `ezyquant-0.7.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/tests/test_test_utils.py` & `ezyquant-0.7.1/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.7.0/tests/test_utils.py` & `ezyquant-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

