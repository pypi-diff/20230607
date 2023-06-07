# Comparing `tmp/psychoanalyze-0.1.2.tar.gz` & `tmp/psychoanalyze-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.1.2.tar", max compression
+gzip compressed data, was "psychoanalyze-0.2.1.tar", max compression
```

## Comparing `psychoanalyze-0.1.2.tar` & `psychoanalyze-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.1.2/LICENSE
--rw-r--r--   0        0        0     1369 2022-11-29 09:37:00.290126 psychoanalyze-0.1.2/psychoanalyze/__init__.py
--rw-r--r--   0        0        0       54 2022-10-04 02:36:06.520931 psychoanalyze-0.1.2/psychoanalyze/amp.py
--rw-r--r--   0        0        0     5526 2022-11-25 16:59:23.201602 psychoanalyze-0.1.2/psychoanalyze/blocks.py
--rw-r--r--   0        0        0     2756 2022-11-25 02:30:28.911080 psychoanalyze-0.1.2/psychoanalyze/data.py
--rw-r--r--   0        0        0      350 2022-11-25 05:41:38.251412 psychoanalyze-0.1.2/psychoanalyze/detection.py
--rw-r--r--   0        0        0     8933 2022-11-25 02:30:28.911080 psychoanalyze-0.1.2/psychoanalyze/layout.py
--rw-r--r--   0        0        0     5308 2022-11-25 02:30:28.911080 psychoanalyze-0.1.2/psychoanalyze/plot.py
--rw-r--r--   0        0        0     5131 2022-11-29 09:35:51.918787 psychoanalyze-0.1.2/psychoanalyze/points.py
--rw-r--r--   0        0        0     1759 2022-11-25 05:30:51.949990 psychoanalyze-0.1.2/psychoanalyze/schemas.py
--rw-r--r--   0        0        0     1998 2022-11-25 07:19:57.749508 psychoanalyze-0.1.2/psychoanalyze/sessions.py
--rw-r--r--   0        0        0        0 2022-11-25 02:30:28.921080 psychoanalyze-0.1.2/psychoanalyze/simulate.py
--rw-r--r--   0        0        0       95 2022-11-25 02:30:28.931080 psychoanalyze-0.1.2/psychoanalyze/stimulus.py
--rw-r--r--   0        0        0      565 2022-10-15 02:21:08.107033 psychoanalyze-0.1.2/psychoanalyze/strength_duration.py
--rw-r--r--   0        0        0      175 2022-11-25 02:30:28.931080 psychoanalyze-0.1.2/psychoanalyze/subjects.py
--rw-r--r--   0        0        0     2512 2022-11-25 02:30:28.941080 psychoanalyze-0.1.2/psychoanalyze/trials.py
--rw-r--r--   0        0        0     1708 2022-10-04 02:36:06.520931 psychoanalyze-0.1.2/psychoanalyze/weber.py
--rw-r--r--   0        0        0     1281 2022-11-29 10:51:50.999266 psychoanalyze-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 psychoanalyze-0.1.2/setup.py
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 psychoanalyze-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 06:11:56.821547 psychoanalyze-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1148 2023-06-07 06:11:56.821547 psychoanalyze-0.2.1/README.md
+-rw-r--r--   0        0        0     1250 2023-06-07 06:13:18.150573 psychoanalyze-0.2.1/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0     6723 2023-06-07 06:11:56.909548 psychoanalyze-0.2.1/psychoanalyze/blocks.py
+-rw-r--r--   0        0        0     2133 2023-06-07 06:11:56.909548 psychoanalyze-0.2.1/psychoanalyze/data.py
+-rw-r--r--   0        0        0      148 2023-06-07 06:11:56.909548 psychoanalyze-0.2.1/psychoanalyze/gescheider.py
+-rw-r--r--   0        0        0     8869 2023-06-07 06:11:56.909548 psychoanalyze-0.2.1/psychoanalyze/layout.py
+-rw-r--r--   0        0        0     5594 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     5036 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/points.py
+-rw-r--r--   0        0        0     1784 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/schemas.py
+-rw-r--r--   0        0        0     2419 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/sessions.py
+-rw-r--r--   0        0        0     2380 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/simulate.py
+-rw-r--r--   0        0        0       95 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/stimulus.py
+-rw-r--r--   0        0        0      565 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/strength_duration.py
+-rw-r--r--   0        0        0      745 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/subjects.py
+-rw-r--r--   0        0        0        0 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/transformations.py
+-rw-r--r--   0        0        0     4069 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/trials.py
+-rw-r--r--   0        0        0     1692 2023-06-07 06:11:56.913549 psychoanalyze-0.2.1/psychoanalyze/weber.py
+-rw-r--r--   0        0        0     1991 2023-06-07 06:13:18.150573 psychoanalyze-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 psychoanalyze-0.2.1/PKG-INFO
```

### Comparing `psychoanalyze-0.1.2/LICENSE` & `psychoanalyze-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.1.2/psychoanalyze/__init__.py` & `psychoanalyze-0.2.1/psychoanalyze/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,36 +5,32 @@
     sessions,
     blocks,
     points,
     plot,
     data,
     trials,
     weber,
-    detection,
-    amp,
     strength_duration,
     subjects,
     stimulus,
     simulate,
 )
 
 pd.options.plotting.backend = "plotly"
 
-__version__ = "0.1.0"
+__version__ = "0.2.1"
 
 __all__ = [
     "schemas",
     "plot",
     "data",
     "trial",
     "blocks",
     "sessions",
     "weber",
-    "detection",
-    "amp",
     "points",
     "trials",
     "blocks",
     "strength_duration",
     "subjects",
     "stimulus",
     "simulate",
@@ -51,13 +47,12 @@
     return 1
 
 
 def psi(threshold=0, slope=1, lambda_=0, gamma=0, x_range=(-3, 3)) -> pd.Series:
     """Basic sigmoid psychometric function psi (Ψ) = expit/logistic"""
     x = np.linspace(x_range[0], x_range[1])
     y = gamma + (1 - lambda_ - gamma) * 1 / (1 + np.exp((-slope) * (x - threshold)))
-    # y = gamma + (1 - lambda_ - gamma) * expit(x)
-    return pd.Series(y, index=x)  # type: ignore
+    return pd.Series(y, index=x)
 
 
 def fit(data):
     return {"Fit": [1, 1, 0, 0]}
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/blocks.py` & `psychoanalyze-0.2.1/psychoanalyze/blocks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pandas as pd
 import numpy as np
-from scipy.stats import logistic  # type: ignore
-from scipy.special import logit, expit  # type: ignore
+from scipy.stats import logistic
+from scipy.special import logit, expit
 import psychoanalyze as pa
-import plotly.express as px  # type: ignore
+import plotly.express as px
 import os
 import pathlib
+from sklearn.linear_model import LogisticRegression
 
 
 dims = ["Amp2", "Width2", "Freq2", "Dur2", "Active Channels", "Return Channels"]
 index_levels = dims
 
 
 def add_posterior(data, posterior):
@@ -55,17 +56,17 @@
     if dim == "Amp":
         levels = levels + ["Width1"]
         df = points.groupby(levels).apply(pa.points.to_block)
         return df[df["n Levels"] > 1].drop(columns="Dimension")
     return points.groupby(levels).apply(pa.points.to_block)
 
 
-def from_trials(trials: pd.DataFrame) -> pd.Series:
+def from_trials(trials: pd.Series) -> pd.Series:
     points = pa.points.from_trials(trials)
-    return from_points(points)
+    return from_points(points.reset_index())
 
 
 def dimensions(points, dims=None):
     if dims is None:
         return pa.points.dimension(points)
     return points.groupby(
         [dim for dim in list(points.index.names) if dim not in dims]
@@ -184,7 +185,54 @@
 
 def monkey_counts(data):
     summary = (
         data.index.get_level_values("Monkey").value_counts().rename("Total Blocks")
     )
     summary.index.name = "Monkey"
     return summary
+
+
+def model_predictions(intensity_choices, k, x_0=0.0):
+    return pd.Series(
+        [1 / (1 + np.exp(-k * (x - x_0))) for x in intensity_choices],
+        index=intensity_choices,
+        name="Hit Rate",
+    )
+
+
+def make_predictions(fit, intensity_choices) -> pd.Series:
+    return pd.Series(
+        fit.predict_proba(pd.DataFrame({"Intensity": intensity_choices}))[:, 1],
+        name="Hit Rate",
+        index=pd.Index(intensity_choices, name="Intensity"),
+    )
+
+
+def get_fit(trials):
+    return LogisticRegression().fit(trials[["Intensity"]], trials["Result"])
+
+
+def fit_params(fit):
+    return pd.Series(
+        {
+            "slope": fit.coef_[0][0],
+            "intercept": fit.intercept_[0],
+        }
+    )
+
+
+def generate_trials(
+    n_trials: int,
+    model_params: dict[str, float],
+    n_levels: int,
+    fixed_range: dict[str, float],
+    fixed_n: int,
+) -> pd.Series:
+    return pd.concat(
+        {
+            fixed_intensity: pa.trials.moc_sample(n_trials, model_params, n_levels)
+            for fixed_intensity in np.linspace(
+                fixed_range["min"], fixed_range["max"], fixed_n
+            )
+        },
+        names=["Fixed Intensity"],
+    )
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/data.py` & `psychoanalyze-0.2.1/psychoanalyze/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,37 @@
 from pathlib import Path
-from typing import List
 import pandas as pd
-import numpy as np
-from scipy.stats import logistic as scipy_logistic  # type: ignore
+from numpy.random import default_rng
+from numpy import linspace
+from scipy.stats import logistic as scipy_logistic
 import psychoanalyze as pa
 from itertools import accumulate
 
 
-def subjects(n_subjects):
-    return list("ABCDEFG"[:n_subjects])
-
-
-def construct_index(subjects: List[str], days: List[int], x: List[float]):
-    levels = [days, x]
-    names = ["Day", "x"]
-    if subjects:
-        levels = [subjects] + levels  # type: ignore
-        names = ["Subject"] + names
-    return pd.MultiIndex.from_product(levels, names=names)
-
-
 def generate_outcomes(n_trials_per_stim_level, index, threshold, scale):
-    return np.random.binomial(
+    random_number_generator = default_rng()
+    return random_number_generator.binomial(
         n_trials_per_stim_level,
         scipy_logistic.cdf(index.get_level_values("x"), threshold, scale),
         len(index),
     )
 
 
-def psych(hits, n_trials_per_stim_level, index, y):
-    df = pd.DataFrame(
-        {
-            "Hits": hits,
-            y: hits / n_trials_per_stim_level,
-            "n": [n_trials_per_stim_level] * len(index),
-        },
-        index=index,
-    )
-    df["Hit Rate"] = pa.blocks.hit_rate
-    return df
-
-
 def logistic(threshold=0, scale=1, gamma=0, lambda_=0):
-    x = np.linspace(scipy_logistic.ppf(0.01), scipy_logistic.ppf(0.99), 100)
+    x = linspace(scipy_logistic.ppf(0.01), scipy_logistic.ppf(0.99), 100)
     index = pd.Index(x, name="x")
     return pd.Series(
         gamma + (1 - gamma - lambda_) * scipy_logistic.cdf(x, threshold, scale),
         index=index,
         name="Hit Rate",
     )
 
 
 def mu(fit):
-    df = fit.loc["mu", ["5%", "50%", "95%"]]  # type: ignore
+    df = fit.loc["mu", ["5%", "50%", "95%"]]
     return df.T
 
 
 def transform_errors(df):
     df["err+"] = df["95%"] - df["50%"]
     df["err-"] = df["50%"] - df["5%"]
     return df.drop(columns=["95%", "5%"])
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/layout.py` & `psychoanalyze-0.2.1/psychoanalyze/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import dash_bootstrap_components as dbc  # type: ignore
-from dash import html, dcc  # type: ignore
+import dash_bootstrap_components as dbc
+from dash import html, dcc
 import psychoanalyze as pa
-import dash_daq as daq  # type: ignore
-import plotly.express as px  # type: ignore
+import dash_daq as daq
+import plotly.express as px
 import pandas as pd
 
 defaults = {
     "session": {"sessions": 1, "trials": 100, "subjects": 1},
     "param": {"thresh": 0, "scale": 1, "gamma": 0, "lambda": 0},
     "x_min": {"x_min": -3},
     "x_max": {"x_max": 3},
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/plot.py` & `psychoanalyze-0.2.1/psychoanalyze/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import plotly.express as px  # type: ignore
+import plotly.express as px
 import pandas as pd
 import psychoanalyze as pa
 from plotly import graph_objects as go
+from psychoanalyze.schemas import PsiAnimation
+from pandera.typing import DataFrame
 
 axis_settings = {
     "ticks": "outside",
-    # "rangemode": "tozero",
     "showgrid": False,
     "showline": True,
     "zeroline": False,
     "title": {"font": {"size": 12, "family": "Arial"}},
 }
 
 template = go.layout.Template(
@@ -86,26 +87,25 @@
         y="Hits",
         animation_group="x",
         animation_frame="n",
         range_y=(0, max(df["Hits"])),
     )
 
 
-def hit_rate_animation(cumulative_draws: pd.DataFrame):
-    df = cumulative_draws.reset_index()
-    return px.scatter(
+def psi_animation(df: DataFrame[PsiAnimation]):
+    return px.line(
         df,
-        x="x",
+        x="Intensity",
         y="Hit Rate",
-        error_y="err+",
-        error_y_minus="err-",
-        color=df.get("Subject") or df.get("Type"),
-        symbol=df.get("Day"),
-        animation_group="x",
-        animation_frame="n",
+        # error_y="err+",
+        # error_y_minus="err-",
+        # color=df.get("Subject") or df.get("Type"),
+        # symbol=df.get("Day"),
+        animation_group="Intensity",
+        animation_frame="Trial",
         template=template,
     )
 
 
 def posterior_animation(cumulative_draws: pd.DataFrame):
     df = cumulative_draws
     df = pa.data.transform_errors(df).reset_index()
@@ -166,15 +166,14 @@
 def get_labels_given_dim(labels, dim, plot_type):
     return {"x": labels[dim]["x"], "y": labels[dim]["y"][plot_type]}
 
 
 def strength_duration(
     data=None, dim=None, plot_type=None, x_data=[], y_data=[], points=None
 ):
-
     labels_given_dim = get_labels_given_dim(labels=labels, dim=dim, plot_type=plot_type)
     x = labels_given_dim["x"]
     y = labels_given_dim["y"]
     if data is not None:
         sd_df = pa.data.filter(data, dim=dim)
     else:
         sd_df = pd.DataFrame({x: x_data, y: y_data})
@@ -203,7 +202,16 @@
         blocks.reset_index(), x=param, color=blocks.get("Monkey")
     ).update_layout(xaxis_title=param)
 
 
 def psychometric(fit, x_range=(-3, 3)):
     s = pa.psi(fit["Threshold"], fit["width"], fit["lambda"], fit["gamma"], x_range)
     return px.line(s, template=pa.plot.template)
+
+
+def combine_figs(fig1: go.Figure, fig2: go.Figure) -> go.Figure:
+    return go.Figure(
+        data=fig1.data + fig2.data,
+        layout_xaxis_title_text="Stimulus Magnitude",
+        layout_yaxis_title_text="Hit Rate",
+        layout_template=pa.plot.template,
+    )
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/schemas.py` & `psychoanalyze-0.2.1/psychoanalyze/schemas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 import pandera as pr
+from pandera.typing import Series
+
 
 session_dims = ["Monkey", "Date"]
 block_stim_dims = ["Amp2", "Width2", "Freq2", "Dur2"]
 block_channel_dims = ["Active Channels", "Return Channels"]
 block_dims = block_stim_dims + block_channel_dims
 point_dims = ["Amp1", "Width1", "Freq1", "Dur1"]
 
 block_index_levels = session_dims + block_dims
 points_index_levels = block_index_levels + point_dims
 
 
 points = pr.DataFrameSchema(
     {
-        "n": pr.Column(int, coerce=True),
-        "x": pr.Column(float, coerce=True),
-        "Hits": pr.Column(float, coerce=True),
-    },
-    index=pr.MultiIndex(
-        [
-            pr.Index(str, name="Monkey"),
-            pr.Index("datetime64", name="Date", coerce=True),
-        ]
-        + [pr.Index(float, name=dim) for dim in block_stim_dims]
-        + [pr.Index(int, name=dim) for dim in block_channel_dims]
-        + [pr.Index(float, name=dim) for dim in point_dims]
-    ),
-    coerce=True,
+        "n": pr.Column(int),
+        "Intensity": pr.Column(float),
+        "Hits": pr.Column(int),
+    }
 )
 
 blocks = pr.DataFrameSchema(
     columns={"Threshold": pr.Column(dtype=float), "width": pr.Column(dtype=float)},
     index=pr.MultiIndex(
         [
             pr.Index(str, name="Monkey"),
@@ -50,7 +42,26 @@
         ]
         + [pr.Index(float, name=dim) for dim in block_stim_dims]
         + [pr.Index(int, name=dim) for dim in block_channel_dims]
         + [pr.Index(float, name=dim) for dim in point_dims]
     ),
     coerce=True,
 )
+
+psi_animation = pr.DataFrameSchema(
+    {
+        "Trial": pr.Column(int),
+        "Intensity": pr.Column(float),
+        "Hit Rate": pr.Column(float),
+    }
+)
+
+
+class PsiAnimation(pr.DataFrameModel):
+    trial_id: Series[int]
+    intensity: Series[float]
+    hit_rate: Series[float]
+
+
+class PsiAnimationFrame(pr.DataFrameModel):
+    intensity: Series[float]
+    hit_rate: Series[float]
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/sessions.py` & `psychoanalyze-0.2.1/psychoanalyze/sessions.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,7 +62,26 @@
 def n_trials(sessions, trials):
     return trials.groupby(["Monkey", "Date"])[["Result"]].count()
 
 
 def load_cached(data_dir, monkey=None):
     sessions = pd.read_csv(data_dir / "sessions.csv", index_col=["Monkey", "Date"])
     return sessions[sessions.index.get_level_values("Monkey") == monkey]
+
+
+def generate_trials(
+    n_trials: int,
+    model_params: dict[str, float],
+    n_levels: int,
+    fixed_range: dict[str, float],
+    fixed_n: int,
+    n_days: int,
+) -> pd.Series:
+    return pd.concat(
+        {
+            day: pa.blocks.generate_trials(
+                n_trials, model_params, n_levels, fixed_range, fixed_n
+            )
+            for day in range(n_days)
+        },
+        names=["Day"],
+    )
```

### Comparing `psychoanalyze-0.1.2/psychoanalyze/strength_duration.py` & `psychoanalyze-0.2.1/psychoanalyze/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.1.2/psychoanalyze/weber.py` & `psychoanalyze-0.2.1/psychoanalyze/weber.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import plotly.express as px  # type: ignore
+import plotly.express as px
 import psychoanalyze as pa
 import pandas as pd
 
 
 def plot(
     data,
     trendline="ols",
```

### Comparing `psychoanalyze-0.1.2/pyproject.toml` & `psychoanalyze-0.2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,95 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.1.2"
+version = "0.2.1"
 description = "A Pythonic analysis package for psychophysics data"
-authors = ["Ty Schlichenmeyer <ty.schlich@gmail.com>"]
+authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
+readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.11.0"
-mkdocs = "^1.3.0"
+python = "3.11.3"
 pandas = "^1.4.2"
-black = "^22.3.0"
+black = "^23.3.0"
 datatest = "^0.11.1"
-pytest = "^7.2.0"
+pytest = "^7.2.2"
 scipy = "^1.8.0"
 numpy = "^1.23.4"
 mkdocstrings = "^0.18.1"
-mkdocs-gen-files = "^0.3.4"
-matplotlib = "^3.5.1"
-plotly = "^5.11.0"
-dash = {extras = ["testing"], version = "^2.7.0"}
-dash-bootstrap-components = "^1.1.0"
-pytest-sugar = "^0.9.4"
+plotly = "^5.14.1"
+dash-bootstrap-components = "^1.4.1"
+pytest-sugar = "^0.9.6"
 pytest-mock = "^3.7.0"
 statsmodels = "^0.13.2"
-mypy = "^0.990"
-hypothesis = "^6.50.0"
-flake8 = "^4.0.1"
+mypy = "^1.2.0"
+hypothesis = "^6.70.0"
 bandit = "^1.7.4"
-importlib-resources = "^5.8.0"
 safety = "^2.0.0"
 mkdocs-material = "^8.3.9"
 tabulate = "^0.8.10"
-gunicorn = "^20.1.0"
-pandera = "^0.11.0"
-kaleido = "0.2.1"
+pandera = {extras = ["mypy"], version = "^0.14.5"}
 pre-commit = "^2.20.0"
 dash-daq = "^0.5.0"
-pandas-stubs = "^1.5.1.221024"
+pandas-stubs = "^1.5.3.230321"
 cmdstanpy = "^1.0.8"
+dbt-core = "^1.5.1"
+dash = "^2.10.2"
+dbt-duckdb = "^1.5.1"
+ydata-profiling = "^4.1.2"
+nbformat = "^5.8.0"
+gunicorn = "^20.1.0"
+shandy-sqlfmt = {extras = ["jinjafmt"], version = "^0.18.0"}
+scikit-learn = "^1.2.2"
+ipywidgets = "^8.0.6"
+conda-lock = "^2.0.0"
+bambi = "^0.11.0"
+python-semantic-release = "7.28.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
+ipykernel = "^6.22.0"
+
+
+[tool.poetry.group.ci.dependencies]
+ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.semantic_release]
+version_variable = [
+    "psychoanalyze/__init__.py:__version__",
+    "pyproject.toml:version"
+]
+branch = "main"
+build_command = "poetry build"
+major_on_zero = true
+
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning",
     "ignore::FutureWarning"
 ]
 
 [tool.bandit]
 targets = ["psychoanalyze/"]
-skips = ["B311"]
+skips = ["B311"]
+
+[tool.mypy]
+exclude = [
+    'tests',
+]
+
+[[tool.mypy.overrides]]
+module = [
+    'dash',
+    'plotly',
+    'dash_bootstrap_components',
+    'plotly.express',
+    'scipy.stats',
+    'scipy.special',
+    'sklearn.linear_model',
+    'dash_daq',
+    'datatest'
+]
+ignore_missing_imports = true
```

### Comparing `psychoanalyze-0.1.2/PKG-INFO` & `psychoanalyze-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,75 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.1.2
+Version: 0.2.1
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
-Author-email: ty.schlich@gmail.com
-Requires-Python: ==3.11.0
+Author-email: t.schlic@wustl.edu
+Requires-Python: ==3.11.3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bambi (>=0.11.0,<0.12.0)
 Requires-Dist: bandit (>=1.7.4,<2.0.0)
-Requires-Dist: black (>=22.3.0,<23.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: cmdstanpy (>=1.0.8,<2.0.0)
-Requires-Dist: dash-bootstrap-components (>=1.1.0,<2.0.0)
+Requires-Dist: conda-lock (>=2.0.0,<3.0.0)
+Requires-Dist: dash (>=2.10.2,<3.0.0)
+Requires-Dist: dash-bootstrap-components (>=1.4.1,<2.0.0)
 Requires-Dist: dash-daq (>=0.5.0,<0.6.0)
-Requires-Dist: dash[testing] (>=2.7.0,<3.0.0)
 Requires-Dist: datatest (>=0.11.1,<0.12.0)
-Requires-Dist: flake8 (>=4.0.1,<5.0.0)
+Requires-Dist: dbt-core (>=1.5.1,<2.0.0)
+Requires-Dist: dbt-duckdb (>=1.5.1,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: hypothesis (>=6.50.0,<7.0.0)
-Requires-Dist: importlib-resources (>=5.8.0,<6.0.0)
-Requires-Dist: kaleido (==0.2.1)
-Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
-Requires-Dist: mkdocs (>=1.3.0,<2.0.0)
-Requires-Dist: mkdocs-gen-files (>=0.3.4,<0.4.0)
+Requires-Dist: hypothesis (>=6.70.0,<7.0.0)
+Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
 Requires-Dist: mkdocs-material (>=8.3.9,<9.0.0)
 Requires-Dist: mkdocstrings (>=0.18.1,<0.19.0)
-Requires-Dist: mypy (>=0.990,<0.991)
+Requires-Dist: mypy (>=1.2.0,<2.0.0)
+Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: pandas-stubs (>=1.5.1.221024,<2.0.0.0)
-Requires-Dist: pandera (>=0.11.0,<0.12.0)
-Requires-Dist: plotly (>=5.11.0,<6.0.0)
+Requires-Dist: pandas-stubs (>=1.5.3.230321,<2.0.0.0)
+Requires-Dist: pandera[mypy] (>=0.14.5,<0.15.0)
+Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pre-commit (>=2.20.0,<3.0.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0)
+Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pytest-mock (>=3.7.0,<4.0.0)
-Requires-Dist: pytest-sugar (>=0.9.4,<0.10.0)
+Requires-Dist: pytest-sugar (>=0.9.6,<0.10.0)
+Requires-Dist: python-semantic-release (==7.28.1)
 Requires-Dist: safety (>=2.0.0,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Requires-Dist: shandy-sqlfmt[jinjafmt] (>=0.18.0,<0.19.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: tabulate (>=0.8.10,<0.9.0)
+Requires-Dist: ydata-profiling (>=4.1.2,<5.0.0)
+Description-Content-Type: text/markdown
+
+# PsychoAnalyze
+
+Psychophysics analysis in Python.
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
+![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![Documentation Status](https://readthedocs.org/projects/psychoanalyze/badge/?version=latest)](https://psychoanalyze.readthedocs.io/en/latest/?badge=latest)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
+[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
+
+
+## Installation
+pip:
+```console
+pip install psychoanalyze
+```
+poetry:
+```console
+poetry add psychoanalyze
+```
+
+## Dashboard
+See what `psychoanalyze` can do by [viewing our dashboard](https://app.psychoanalyze.io/).
+
+## Documentation
+View the full documentation [here](https://docs.psychoanalyze.io).
+
```

