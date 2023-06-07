# Comparing `tmp/jquants_derivatives-0.1.0a0.tar.gz` & `tmp/jquants_derivatives-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_derivatives-0.1.0a0.tar", max compression
+gzip compressed data, was "jquants_derivatives-0.1.0a1.tar", max compression
```

## Comparing `jquants_derivatives-0.1.0a0.tar` & `jquants_derivatives-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2023-06-06 13:53:32.816616 jquants_derivatives-0.1.0a0/README.md
--rw-r--r--   0        0        0       97 2023-06-06 13:38:15.576989 jquants_derivatives-0.1.0a0/jquants_derivatives/__init__.py
--rw-r--r--   0        0        0     2296 2023-06-06 11:13:48.186610 jquants_derivatives-0.1.0a0/jquants_derivatives/client.py
--rw-r--r--   0        0        0     1290 2023-06-05 23:18:08.508412 jquants_derivatives-0.1.0a0/jquants_derivatives/database.py
--rw-r--r--   0        0        0     5242 2023-06-06 13:39:32.319480 jquants_derivatives-0.1.0a0/jquants_derivatives/derivatievs.py
--rw-r--r--   0        0        0     1230 2023-06-05 23:19:32.464553 jquants_derivatives-0.1.0a0/jquants_derivatives/models.py
--rw-r--r--   0        0        0      513 2023-06-06 13:45:52.861789 jquants_derivatives-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a0/setup.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-06 13:53:32.816616 jquants_derivatives-0.1.0a1/README.md
+-rw-r--r--   0        0        0      124 2023-06-06 14:36:12.452162 jquants_derivatives-0.1.0a1/jquants_derivatives/__init__.py
+-rw-r--r--   0        0        0     1870 2023-06-06 15:52:55.552479 jquants_derivatives-0.1.0a1/jquants_derivatives/client.py
+-rw-r--r--   0        0        0     1290 2023-06-05 23:18:08.508412 jquants_derivatives-0.1.0a1/jquants_derivatives/database.py
+-rw-r--r--   0        0        0     5337 2023-06-06 15:43:26.519073 jquants_derivatives-0.1.0a1/jquants_derivatives/derivatievs.py
+-rw-r--r--   0        0        0     1302 2023-06-06 15:08:31.605466 jquants_derivatives-0.1.0a1/jquants_derivatives/models.py
+-rw-r--r--   0        0        0      514 2023-06-06 14:46:30.172595 jquants_derivatives-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a1/setup.py
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a1/PKG-INFO
```

### Comparing `jquants_derivatives-0.1.0a0/jquants_derivatives/client.py` & `jquants_derivatives-0.1.0a1/jquants_derivatives/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from functools import wraps
-from typing import Type
+from typing import Any, Type, TypeAlias, Union
 
 import jquantsapi
 import numpy as np
 import pandas as pd
 
 from . import database
-from .models import IndexOption
+from .models import DataFrameColumnsBase, IndexOption
+
+ModelsType: TypeAlias = Union[Type[DataFrameColumnsBase], Type[IndexOption]]
 
 
 def cache(table_name: str):
     """関数が実行して返したDataFrameをsqlite3のデータベースに保管"""
 
     def decorator(func):
         @wraps(func)
@@ -24,59 +26,42 @@
                 return df
 
         return wrapper
 
     return decorator
 
 
-def cast_dataframe(data_class):
+def cast_dataframe(data_class: ModelsType):
     def decorator(func):
         @wraps(func)
         def wrapper(self, date_yyyymmdd: str):
-            print("called")
             df = func(self, date_yyyymmdd)
             return pd.DataFrame(
                 {
                     col: cast_series_dtype(df.loc[:, col], data_class.get_dtype(col))
                     for col in df.columns
                 }
             )
 
         return wrapper
 
     return decorator
 
 
-def cast_series_dtype(ser: pd.Series, dtype: type) -> pd.Series:
+def cast_series_dtype(ser: pd.Series, dtype: Type[Any]) -> pd.Series:
     """Seriesのデータ型を変換"""
     if np.issubdtype(dtype, np.number):
         return pd.to_numeric(ser, errors="coerce").astype(dtype)
     elif np.issubdtype(dtype, np.datetime64):
         return pd.to_datetime(ser)
     else:
         return ser.astype(dtype)
 
 
-def cast_dataframe_dtype(
-    df: pd.DataFrame, data_class: Type[IndexOption]
-) -> pd.DataFrame:
-    """DataFrameのデータ型をmodelsで定義したクラスの型に変換"""
-    return pd.DataFrame(
-        {
-            col: cast_series_dtype(df.loc[:, col], data_class.get_dtype(col))
-            for col in df.columns
-        }
-    )
-
-
 class Client(jquantsapi.Client):
     def __init__(self):
         super().__init__()
 
+    @cast_dataframe(IndexOption)
     @cache("OPTION_INDEX_OPTION")
     def get_option_index_option(self, *args, **kwargs) -> pd.DataFrame:
         return super().get_option_index_option(*args, **kwargs)
-
-    def get_option_index_option_processed(self, date_yyyymmdd: str) -> pd.DataFrame:
-        df = self.get_option_index_option(date_yyyymmdd)
-        casted_df = cast_dataframe_dtype(df, IndexOption)
-        return casted_df
```

### Comparing `jquants_derivatives-0.1.0a0/jquants_derivatives/database.py` & `jquants_derivatives-0.1.0a1/jquants_derivatives/database.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a0/jquants_derivatives/derivatievs.py` & `jquants_derivatives-0.1.0a1/jquants_derivatives/derivatievs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from typing import Optional
 
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 
 
 @dataclass
@@ -15,26 +16,28 @@
         self.date = self.df.loc[:, "Date"].iloc[0]
         self._groupby_contract_month: pd.core.groupby.generic.DataFrameGroupBy = (
             self.df.groupby("ContractMonth")
         )
         self.contract_month: list = sorted(self._groupby_contract_month.groups.keys())[
             : self.contracts
         ][: self.contracts]
-        self.contracts_dfs: dict[pd.DataFrame] = self.get_processed_data()
-        self.underlying_price: dict[float] = self.get_common_value("UnderlyingPrice")
-        self.base_volatility: dict[float] = self.get_common_value("BaseVolatility")
-        self.interest_rate: dict[float] = self.get_common_value("InterestRate")
-        self.last_tradingDay: dict[pd.Timestamp] = self.get_common_value(
+        self.contracts_dfs: dict[str, pd.DataFrame] = self.get_processed_data()
+        self.underlying_price: dict[str, float] = self.get_common_value(
+            "UnderlyingPrice"
+        )
+        self.base_volatility: dict[str, float] = self.get_common_value("BaseVolatility")
+        self.interest_rate: dict[str, float] = self.get_common_value("InterestRate")
+        self.last_tradingDay: dict[str, pd.Timestamp] = self.get_common_value(
             "LastTradingDay"
         )
-        self.special_quotationDay: dict[pd.Timestamp] = self.get_common_value(
+        self.special_quotationDay: dict[str, pd.Timestamp] = self.get_common_value(
             "SpecialQuotationDay"
         )
 
-    def get_processed_data(self) -> dict[pd.DataFrame]:
+    def get_processed_data(self) -> dict[str, pd.DataFrame]:
         contracts_dfs = {
             contract: self.filter_data(self._groupby_contract_month.get_group(contract))
             for contract in self.contract_month
         }
         for key in contracts_dfs:
             contracts_dfs[key] = self.percentage_to_decimal(contracts_dfs[key])
         return contracts_dfs
@@ -86,15 +89,15 @@
             contract: self.contracts_dfs[contract].loc[:, value].iloc[0]
             for contract in self.contracts_dfs
         }
 
 
 def plot_volatility(
     option: Option,
-    option_other: Option = None,
+    option_other: Optional[Option] = None,
     colors: list = px.colors.qualitative.Dark2,
 ) -> go.Figure:
     date = f"{option.date: %Y/%m/%d}"
     underlying_price = {k: round(v, 2) for k, v in option.underlying_price.items()}
     base_volatility = {k: round(v, 4) for k, v in option.base_volatility.items()}
     layout = go.Layout(
         title={
```

### Comparing `jquants_derivatives-0.1.0a0/jquants_derivatives/models.py` & `jquants_derivatives-0.1.0a1/jquants_derivatives/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABC
 from dataclasses import dataclass
+from typing import Any, Type
 
 import numpy as np
 
 
 @dataclass
-class Base(ABC):
+class DataFrameColumnsBase(ABC):
     @classmethod
-    def get_dtype(cls, field: str) -> str:
+    def get_dtype(cls, field: str) -> Type[Any]:
         return cls.__annotations__[field]
 
 
 @dataclass
-class IndexOption(Base):
+class IndexOption(DataFrameColumnsBase):
     Date: np.dtype("datetime64[ns]")
     Code: str
     WholeDayOpen: float
     WholeDayHigh: float
     WholeDayLow: float
     WholeDayClose: float
     NightSessionOpen: float
@@ -41,10 +42,10 @@
     TheoreticalPrice: float
     BaseVolatility: float
     UnderlyingPrice: float
     ImpliedVolatility: float
     InterestRate: float
 
     @classmethod
-    def get_dtype(cls, field: str) -> type:
+    def get_dtype(cls, field: str) -> Type[Any]:
         key = field.replace("(", "").replace(")", "")
         return cls.__annotations__[key]
```

### Comparing `jquants_derivatives-0.1.0a0/pyproject.toml` & `jquants_derivatives-0.1.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-derivatives"
-version = "0.1.0-alpha"
+version = "0.1.0-alpha1"
 description = ""
 authors = ["driller"]
 readme = "README.md"
 packages = [{include = "jquants_derivatives"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `jquants_derivatives-0.1.0a0/setup.py` & `jquants_derivatives-0.1.0a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['jquants-api-client>=1.2.0,<2.0.0', 'plotly>=5.14.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'jquants-derivatives',
-    'version': '0.1.0a0',
+    'version': '0.1.0a1',
     'description': '',
     'long_description': '# jquants-derivatives\n',
     'author': 'driller',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

