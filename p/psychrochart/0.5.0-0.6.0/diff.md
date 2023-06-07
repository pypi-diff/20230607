# Comparing `tmp/psychrochart-0.5.0.tar.gz` & `tmp/psychrochart-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.5.0.tar", max compression
+gzip compressed data, was "psychrochart-0.6.0.tar", max compression
```

## Comparing `psychrochart-0.5.0.tar` & `psychrochart-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6055 2023-06-05 11:57:37.165362 psychrochart-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-05 11:57:37.165362 psychrochart-0.5.0/LICENSE
--rw-r--r--   0        0        0     6746 2023-06-05 11:57:37.165362 psychrochart-0.5.0/README.md
--rw-r--r--   0        0        0      711 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/__main__.py
--rw-r--r--   0        0        0      254 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/agg.py
--rw-r--r--   0        0        0    11817 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart.py
--rw-r--r--   0        0        0     2157 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3064 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    14520 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chartdata.py
--rw-r--r--   0        0        0        0 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     4427 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/annots.py
--rw-r--r--   0        0        0     6671 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/config.py
--rw-r--r--   0        0        0     9239 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5852 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     1868 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1742 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/validators.py
--rw-r--r--   0        0        0     7361 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     6268 2023-06-05 11:57:37.269361 psychrochart-0.5.0/psychrochart/process_logic.py
--rw-r--r--   0        0        0     3898 2023-06-05 11:57:37.269361 psychrochart-0.5.0/psychrochart/util.py
--rw-r--r--   0        0        0     2222 2023-06-05 11:57:37.269361 psychrochart-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8035 1970-01-01 00:00:00.000000 psychrochart-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7288 2023-06-07 17:46:43.829993 psychrochart-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-07 17:46:43.829993 psychrochart-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7077 2023-06-07 17:46:43.829993 psychrochart-0.6.0/README.md
+-rw-r--r--   0        0        0      711 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/__main__.py
+-rw-r--r--   0        0        0    12177 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart.py
+-rw-r--r--   0        0        0     2157 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3080 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    17119 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chartdata.py
+-rw-r--r--   0        0        0        0 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     4427 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/base.py
+-rw-r--r--   0        0        0     6715 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/config.py
+-rw-r--r--   0        0        0     9238 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5852 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     1909 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1744 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/validators.py
+-rw-r--r--   0        0        0     7361 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     9076 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     3977 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/util.py
+-rw-r--r--   0        0        0     2195 2023-06-07 17:46:43.841993 psychrochart-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8366 1970-01-01 00:00:00.000000 psychrochart-0.6.0/PKG-INFO
```

### Comparing `psychrochart-0.5.0/CHANGELOG.md` & `psychrochart-0.6.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.6.0] - ✨ Chart config auto-refresh + bugfixes - 2023-06-07
+
+Before, chart customize was done by creating a new `Psychrochart` object based on some modified chart configuration,
+so creating custom plots, or even changing chart limits, was _challenging_ 😓
+
+**Now**, when `chart.config` changes, any call to `chart.save()`, `chart.make_svg()`, or `chart.plot()`
+will regenerate the chart data (limits, enabled curves, styling, etc.) before plotting, with only the visible curves inside limits,
+(no more 0-size artifacts in SVGs, and most errors because some var is out of range should be gone now 🤞)
+
+##### Changes
+
+- ♻️ Update example notebook with API changes, and using `chart.make_svg()` as the recommended method to generate SVGs
+- 💄 **Parse colors into RGBA values**, so "red", "#FF0000", "#FF0000FF" produce the same float repr [1., 0., 0., 1.]
+- 🏗️ Add **mutation control for configuration models**, and use it to check if there is any config change before creating a chart, triggering a chart-data regeneration if necessary
+- 🔧 Add new field `ChartFigure.dpi` to chart config, for easy customization of matplotlib Figure DPI
+- ⚡️ Optimize generation of psychrometric curves inside plot limits
+
 ## [0.5.0] - ♻️ Full re-work on internals to use pydantic models - 2023-06-05
 
 🧹 Internal evolution to update the code style to the latest versions and de facto standards, with better typing, input validation, and serialization.
 Hardly any new features, but some bug fixes.
 
 ### Changes
```

### Comparing `psychrochart-0.5.0/LICENSE` & `psychrochart-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/README.md` & `psychrochart-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,24 @@
 ## Usage
 
 ```python
 from psychrochart import PsychroChart
 
 # Load default style:
 chart_default = PsychroChart.create()
+# customize anything
+chart_default.limits.range_temp_c = (15.0, 35.0)
+chart_default.limits.range_humidity_g_kg = (5, 25)
+chart_default.config.saturation.linewidth = 1
+chart_default.config.constant_wet_temp.color = "darkblue"
+# plot
 axes = chart_default.plot()
 axes.get_figure()
+# or store on disk
+chart_default.save("my-custom-chart.svg")
 ```
 
 Called from the terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
 
 ```python
 from psychrochart import PsychroChart
 import matplotlib.pyplot as plt
@@ -72,15 +80,15 @@
 PsychroChart.create().plot(ax=plt.gca())
 plt.show()
 ```
 
 ### Chart customization
 
 The default styling for charts is defined in JSON files that you can change, or you can pass a path of a file in JSON, or a dict, when you create the psychrometric chart object.
-Included styles are: `default`, `ashrae`, `interior` and `minimal`.
+Included styles are: `default`, `ashrae`, `ashrae_ip` (adjusted for IP units), `interior`, and `minimal`.
 
 ```python
 from pathlib import Path
 from psychrochart import load_config, PsychroChart
 
 # Load preconfigured styles:
 chart_ashrae_style = PsychroChart.create('ashrae')
```

### Comparing `psychrochart-0.5.0/psychrochart/__init__.py` & `psychrochart-0.6.0/psychrochart/__init__.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/chart.py` & `psychrochart-0.6.0/psychrochart/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     apply_axis_styling,
     plot_annots_dbt_rh,
     plot_chart,
 )
 from psychrochart.process_logic import (
     append_zones_to_chart,
     generate_psychrochart,
+    update_psychrochart_data,
 )
 from psychrochart.util import mod_color
 
 
 def _select_fig_canvas(
     path_dest: Any, canvas_cls: Type[FigureCanvasBase] | None = None
 ) -> Type[FigureCanvasBase]:
@@ -74,14 +75,15 @@
         cls,
         config: ChartConfig | dict[str, Any] | str | None = None,
         *,
         extra_zones: ChartZones | dict[str, Any] | str | None = None,
         use_unit_system_si: bool = True,
     ):
         chart_config = obj_loader(ChartConfig, config)
+        chart_config.commit_changes()
         chart_data = generate_psychrochart(
             chart_config, extra_zones, use_unit_system_si
         )
         chart = cls(config=chart_config, **chart_data.dict())
         return chart
 
     def __repr__(self) -> str:
@@ -89,17 +91,22 @@
         return (
             f"<PsychroChart [{self.config.dbt_min:g}"
             f"->{self.config.dbt_max:g} °C, "
             f"{self.config.w_min:g}"
             f"->{self.config.w_max:g} gr/kg_da]>"
         )
 
+    def _ensure_updated_data(self):
+        if self.config.has_changed:
+            update_psychrochart_data(self, self.config)
+
     @property
     def axes(self) -> Axes:
         """Return the Axes object plotting the chart if necessary."""
+        self._ensure_updated_data()
         if self._axes is None:
             self.plot()
         assert isinstance(self._axes, Axes)
         return self._axes
 
     def append_zones(
         self, zones: ChartZones | dict[str, Any] | str | None = None
@@ -282,19 +289,22 @@
             fancybox=fancybox,
             labelspacing=labelspacing,
             **params,
         )
 
     def plot(self, ax: Axes | None = None) -> Axes:
         """Plot the psychrochart and return the matplotlib Axes instance."""
+        self._ensure_updated_data()
         if ax is not None:
             self._fig = ax.get_figure()
         else:
             self._fig = figure.Figure(
-                figsize=self.config.figure.figsize, dpi=150, frameon=False
+                figsize=self.config.figure.figsize,
+                dpi=self.config.figure.dpi,
+                frameon=False,
             )
             ax = self._fig.add_subplot(position=self.config.figure.position)
         self._axes = ax
         apply_axis_styling(self.config, self._axes)
         return plot_chart(self, self._axes)
 
     def remove_annotations(self) -> None:
@@ -320,16 +330,16 @@
     ) -> None:
         """Write the chart to disk."""
         # ensure destination path if folder does not exist
         if (
             isinstance(path_dest, (str, Path))
             and not Path(path_dest).parent.exists()
         ):
-            Path(path_dest).parent.mkdir()
-        if self._axes is None:
+            Path(path_dest).parent.mkdir(parents=True)
+        if self._axes is None or self.config.has_changed:
             self.plot()
         assert self._fig is not None
         canvas_use = _select_fig_canvas(path_dest, canvas_cls)
         canvas_use(self._fig).print_figure(path_dest, **params)
         gc.collect()
 
     def make_svg(self, **params: Mapping[str, Any]) -> str:
```

### Comparing `psychrochart-0.5.0/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.6.0/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.6.0/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.6.0/psychrochart/chart_styles/default_chart_config.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285716%*

 * *Differences: {"'figure'": "{'dpi': 150}"}*

```diff
@@ -135,14 +135,15 @@
             0.875,
             1
         ],
         "linestyle": "-.",
         "linewidth": 1
     },
     "figure": {
+        "dpi": 150,
         "figsize": [
             16,
             9
         ],
         "fontsize": 10,
         "partial_axis": true,
         "position": [
```

### Comparing `psychrochart-0.5.0/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.6.0/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.6.0/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.6.0/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/chartdata.py` & `psychrochart-0.6.0/psychrochart/chartdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """A library to make psychrometric charts and overlay information in them."""
-from typing import Callable, Iterable
+import logging
+from typing import Sequence
 
 import numpy as np
 from psychrolib import (
+    GetHumRatioFromTWetBulb,
     GetHumRatioFromVapPres,
     GetMoistAirEnthalpy,
     GetMoistAirVolume,
-    GetRelHumFromTWetBulb,
+    GetRelHumFromHumRatio,
     GetSatVapPres,
     GetTDewPointFromVapPres,
     GetTDryBulbFromEnthalpyAndHumRatio,
     GetTDryBulbFromMoistAirVolumeAndHumRatio,
+    GetTWetBulbFromHumRatio,
     GetVapPresFromHumRatio,
     isIP,
 )
 from scipy.interpolate import interp1d
 
 from psychrochart.models.annots import ChartZone
 from psychrochart.models.curves import PsychroCurve, PsychroCurves
@@ -62,79 +65,81 @@
 
 
 def _make_vol_label(specific_vol: float) -> str:
     unit = "$ft³/lb_{da}$" if isIP() else "$m³/kg_{da}$"
     return f"{specific_vol:g} {unit}"
 
 
-def _gen_list_curves_range_temps(
-    func_curve: Callable,
-    curves_values: Iterable[float],
-    dbt_min: float,
-    dbt_max: float,
-    increment: float,
-    pressure: float,
-) -> tuple[np.array, list[np.array]]:
-    """Generate a curve from a range of temperatures."""
-    temps = np.arange(dbt_min, dbt_max + increment, increment)
-    curves = [func_curve(temps, value, pressure) for value in curves_values]
-    return temps, curves
-
-
 def _get_humid_ratio_in_saturation(
     dry_temps: np.ndarray, pressure: float
 ) -> np.array:
     sat_p = f_vec_sat_press(dry_temps)
     return _factor_out_w() * f_vec_hum_ratio_from_vap_press(sat_p, pressure)
 
 
+def get_rh_max_min_in_limits(
+    dbt_min: float,
+    dbt_max: float,
+    w_humidity_ratio_min: float,
+    w_humidity_ratio_max: float,
+    pressure: float,
+) -> tuple[float, float]:
+    """Get max range for constant rel. humidity lines inside chart limits."""
+    rh_min = GetRelHumFromHumRatio(
+        dbt_max, w_humidity_ratio_min / _factor_out_w(), pressure
+    )
+    rh_max = GetRelHumFromHumRatio(
+        dbt_min, w_humidity_ratio_max / _factor_out_w(), pressure
+    )
+    return max(rh_min * 100.0, 0), min(rh_max * 100.0, 100)
+
+
 def gen_points_in_constant_relative_humidity(
-    dry_temps: Iterable[float],
-    rh_percentage: float | Iterable[float],
+    dry_temps: Sequence[float],
+    rh_percentage: float | Sequence[float],
     pressure: float,
 ) -> np.array:
     """Generate a curve (numpy array) of constant humidity ratio."""
     return _factor_out_w() * f_vec_hum_ratio_from_vap_press(
-        f_vec_sat_press(dry_temps) * np.array(rh_percentage) / 100.0, pressure
+        f_vec_sat_press(dry_temps)
+        * np.array(rh_percentage).clip(0, 100)
+        / 100.0,
+        pressure,
     )
 
 
 def make_constant_relative_humidity_lines(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
-    rh_perc_values: Iterable[float],
-    rh_label_values: Iterable[float],
+    rh_perc_values: list[int],
+    rh_label_values: list[int],
     style: CurveStyle,
     label_loc: float,
     family_label: str | None,
 ) -> PsychroCurves:
     """Generate curves of constant relative humidity for the chart."""
-    temps_ct_rh, curves_ct_rh = _gen_list_curves_range_temps(
-        gen_points_in_constant_relative_humidity,
-        rh_perc_values,
-        dbt_min,
-        dbt_max,
-        temp_step,
-        pressure,
-    )
+    rh_values = sorted(rh for rh in rh_perc_values if 0 <= rh <= 100)
+    temps_ct_rh = np.arange(dbt_min, dbt_max + temp_step, temp_step)
+    curves_ct_rh = [
+        gen_points_in_constant_relative_humidity(temps_ct_rh, rh, pressure)
+        for rh in rh_values
+    ]
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=temps_ct_rh,
                 y_data=curve_ct_rh,
                 style=style,
                 type_curve="constant_rh_data",
                 label_loc=label_loc,
-                label=(
-                    f"RH {rh:g} %" if round(rh, 1) in rh_label_values else None
-                ),
+                label=f"RH {rh:g} %" if rh in rh_label_values else None,
             )
-            for rh, curve_ct_rh in zip(rh_perc_values, curves_ct_rh)
+            for rh, curve_ct_rh in zip(rh_values, curves_ct_rh)
         ],
         family_label=family_label,
     )
 
 
 def make_constant_dry_bulb_v_line(
     w_humidity_ratio_min: float,
@@ -182,15 +187,15 @@
         family_label=family_label,
     )
 
 
 def make_constant_humidity_ratio_h_lines(
     dbt_max: float,
     pressure: float,
-    ws_hl: Iterable[float],
+    ws_hl: np.ndarray,
     style: CurveStyle,
     family_label: str | None,
 ) -> PsychroCurves:
     """Generate curves of constant absolute humidity (horizontal)."""
     arr_hum_ratios = np.array(ws_hl) / _factor_out_w()
     dew_points = f_vec_dew_point_from_vap_press(
         dbt_max, f_vec_vap_press_from_hum_ratio(arr_hum_ratios, pressure)
@@ -215,56 +220,77 @@
     temp_step: float,
     pressure: float,
     style: CurveStyle,
 ) -> PsychroCurves:
     """Generate line of saturation for the psychrochart."""
     temps_sat_line = np.arange(dbt_min, dbt_max + temp_step, temp_step)
     w_sat = gen_points_in_constant_relative_humidity(
-        temps_sat_line, 100.0, pressure
+        temps_sat_line, 100, pressure
     )
     sat_c = PsychroCurve(
         x_data=temps_sat_line,
         y_data=w_sat,
         style=style,
         type_curve="saturation",
     )
     return PsychroCurves(curves=[sat_c])
 
 
 def make_constant_enthalpy_lines(
     w_humidity_ratio_min: float,
     pressure: float,
-    enthalpy_values: Iterable[float],
-    h_label_values: Iterable[float],
+    enthalpy_values: np.ndarray,
+    h_label_values: list[float],
     style: CurveStyle,
     label_loc: float,
     family_label: str | None,
     saturation_curve: PsychroCurve,
-) -> PsychroCurves:
+    dbt_min_seen: float | None = None,
+) -> PsychroCurves | None:
     """Generate curves of constant enthalpy for the chart."""
-    enthalpy_objective = np.array(enthalpy_values)
-    temps_max_constant_h = f_vec_dry_temp_from_enthalpy(
-        enthalpy_objective * _factor_out_h(),
-        w_humidity_ratio_min / _factor_out_w(),
-    )
     h_in_sat = (
         f_vec_moist_air_enthalpy(
             saturation_curve.x_data, saturation_curve.y_data / _factor_out_w()
         )
         / _factor_out_h()
     )
     t_sat_interpolator = interp1d(
         h_in_sat,
         saturation_curve.x_data,
         fill_value="extrapolate",
         assume_sorted=True,
     )
+    h_min = (
+        GetMoistAirEnthalpy(
+            dbt_min_seen or saturation_curve.x_data[0],
+            w_humidity_ratio_min / _factor_out_w(),
+        )
+        / _factor_out_h()
+    )
+    h_max = h_in_sat[-1]
+    h_objective = np.array([h for h in enthalpy_values if h_min < h < h_max])
+    if not h_objective.shape[0]:
+        logging.warning(
+            "All %d enthalpy curves are outside limits"
+            "(%g->%g not inside [%g, %g])",
+            len(enthalpy_values),
+            enthalpy_values[0],
+            enthalpy_values[-1],
+            h_min,
+            h_max,
+        )
+        return None
+
+    temps_max_constant_h = f_vec_dry_temp_from_enthalpy(
+        h_objective * _factor_out_h(),
+        w_humidity_ratio_min / _factor_out_w(),
+    )
     t_sat_points = solve_curves_with_iteration(
         "ENTHALPHY",
-        enthalpy_objective,
+        h_objective,
         lambda *x: t_sat_interpolator(x[0]),
         lambda x: GetMoistAirEnthalpy(
             x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure)
         )
         / _factor_out_h(),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
@@ -280,49 +306,70 @@
                 label=(
                     _make_enthalpy_label(h)
                     if round(h, 3) in h_label_values
                     else None
                 ),
             )
             for t_sat, w_sat, t_max, h in zip(
-                t_sat_points, w_in_sat, temps_max_constant_h, enthalpy_values
+                t_sat_points, w_in_sat, temps_max_constant_h, h_objective
             )
         ],
         family_label=family_label,
     )
 
 
 def make_constant_specific_volume_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     vol_values: np.ndarray,
-    v_label_values: Iterable[float],
+    v_label_values: list[float],
     style: CurveStyle,
     label_loc: float,
     family_label: str | None,
     saturation_curve: PsychroCurve,
-) -> PsychroCurves:
+    dbt_min_seen: float | None = None,
+) -> PsychroCurves | None:
     """Generate curves of constant specific volume for the chart."""
-    temps_max_constant_v = f_vec_dry_temp_from_spec_vol(
-        np.array(vol_values), w_humidity_ratio_min / _factor_out_w(), pressure
-    )
     v_in_sat = f_vec_moist_air_volume(
         saturation_curve.x_data,
         saturation_curve.y_data / _factor_out_w(),
         pressure,
     )
+    v_min = GetMoistAirVolume(
+        dbt_min_seen or saturation_curve.x_data[0],
+        w_humidity_ratio_min / _factor_out_w(),
+        pressure,
+    )
+    v_max = v_in_sat[-1]
+    valid_objectives = [h for h in vol_values if v_min < h < v_max]
+    if not valid_objectives:
+        logging.warning(
+            "All %d constant-volume curves are outside limits "
+            "(%g->%g not inside [%g, %g])",
+            len(vol_values),
+            vol_values[0],
+            vol_values[-1],
+            v_min,
+            v_max,
+        )
+        return None
+
+    v_objective = np.array(valid_objectives)
+    temps_max_constant_v = f_vec_dry_temp_from_spec_vol(
+        np.array(v_objective), w_humidity_ratio_min / _factor_out_w(), pressure
+    )
     t_sat_interpolator = interp1d(
         v_in_sat,
         saturation_curve.x_data,
         fill_value="extrapolate",
         assume_sorted=True,
     )
     t_sat_points = solve_curves_with_iteration(
         "CONSTANT VOLUME",
-        vol_values,
+        v_objective,
         lambda *x: t_sat_interpolator(x[0]),
         lambda x: GetMoistAirVolume(
             x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure), pressure
         ),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
 
@@ -337,67 +384,96 @@
                 label=(
                     _make_vol_label(vol)
                     if round(vol, 3) in v_label_values
                     else None
                 ),
             )
             for t_sat, w_sat, t_max, vol in zip(
-                t_sat_points, w_in_sat, temps_max_constant_v, vol_values
+                t_sat_points, w_in_sat, temps_max_constant_v, v_objective
             )
         ],
         family_label=family_label,
     )
 
 
 def make_constant_wet_bulb_temperature_lines(
+    dry_bulb_temp_min: float,
     dry_bulb_temp_max: float,
+    w_humidity_ratio_min: float,
+    w_humidity_ratio_max: float,
     pressure: float,
     wbt_values: np.ndarray,
-    wbt_label_values: Iterable[float],
+    wbt_label_values: list[float],
     style: CurveStyle,
     label_loc: float,
     family_label: str | None,
-) -> PsychroCurves:
+) -> PsychroCurves | None:
     """Generate curves of constant wet bulb temperature for the chart."""
-    w_max_constant_wbt = f_vec_hum_ratio_from_vap_press(
-        f_vec_sat_press(np.array(wbt_values)), pressure
+    wt_min = GetTWetBulbFromHumRatio(
+        dry_bulb_temp_min, w_humidity_ratio_min / _factor_out_w(), pressure
     )
-
-    def _hum_ratio_for_constant_wet_temp_at_dry_temp(db_t, wb_t, p_atm):
-        return _factor_out_w() * GetHumRatioFromVapPres(
-            GetSatVapPres(db_t) * GetRelHumFromTWetBulb(db_t, wb_t, p_atm),
-            p_atm,
+    if -0.75 < wt_min < 0.0:  # slope change zone
+        wt_min = 0
+    wt_bottom_right = GetTWetBulbFromHumRatio(dry_bulb_temp_max, 0, pressure)
+    wt_top_right = GetTWetBulbFromHumRatio(
+        dry_bulb_temp_max,
+        min(
+            w_humidity_ratio_max / _factor_out_w(),
+            GetHumRatioFromVapPres(GetSatVapPres(dry_bulb_temp_max), pressure),
+        ),
+        pressure,
+    )
+    wbt_objective = np.array(
+        [wt for wt in wbt_values if wt_min < wt < wt_top_right]
+    )
+    if wbt_objective.shape[0] == 0:
+        logging.warning(
+            "All %d wetbulb-temp curves are outside limits "
+            "(%g->%g not inside [%g, %g])",
+            len(wbt_values),
+            wbt_values[0],
+            wbt_values[-1],
+            wt_min,
+            dry_bulb_temp_max,
         )
+        return None
 
+    w_max_constant_wbt = f_vec_hum_ratio_from_vap_press(
+        f_vec_sat_press(wbt_objective), pressure
+    )
     curves = []
-    for wbt, w_max in zip(wbt_values, w_max_constant_wbt):
-        pair_t = [wbt, dry_bulb_temp_max]
-        pair_w = [
-            _factor_out_w() * w_max,
-            _hum_ratio_for_constant_wet_temp_at_dry_temp(
-                pair_t[1], wbt, pressure
-            ),
-        ]
-        while pair_w[1] <= 0.01:
-            pair_t[1] -= 0.5 * (pair_t[1] - wbt)
-            pair_w[1] = _hum_ratio_for_constant_wet_temp_at_dry_temp(
-                pair_t[1], wbt, pressure
+    for wbt, w_max in zip(wbt_objective, w_max_constant_wbt):
+        dbt_objective = dry_bulb_temp_max
+        w_left = _factor_out_w() * w_max
+        if wbt >= wt_bottom_right:
+            # on vertical y-axis
+            w_right = _factor_out_w() * GetHumRatioFromTWetBulb(
+                dbt_objective, wbt, pressure
             )
-
-            if pair_w[1] > 0.01:
-                # extend curve to the bottom axis
-                slope = (pair_t[1] - pair_t[0]) / (pair_w[1] - pair_w[0])
-                new_dbt = wbt - slope * pair_w[0]
-                pair_t[1] = new_dbt
-                pair_w[1] = 0.0
-                break
+        else:
+            # on horizontal x-axis
+            dbt_objective = dry_bulb_temp_max
+            w_right = _factor_out_w() * GetHumRatioFromTWetBulb(
+                dbt_objective, wbt, pressure
+            )
+            while w_right <= 0.01:
+                dbt_objective -= 0.5 * (dbt_objective - wbt)
+                w_right = _factor_out_w() * GetHumRatioFromTWetBulb(
+                    dbt_objective, wbt, pressure
+                )
+                if w_right > 0.01:
+                    # extend curve to the bottom axis
+                    slope = (dbt_objective - wbt) / (w_right - w_left)
+                    dbt_objective = wbt - slope * w_left
+                    w_right = 0.0
+                    break
 
         c = PsychroCurve(
-            x_data=np.array(pair_t),
-            y_data=np.array(pair_w),
+            x_data=np.array([wbt, dbt_objective]),
+            y_data=np.array([w_left, w_right]),
             style=style,
             type_curve="constant_wbt_data",
             label_loc=label_loc,
             label=(_make_temp_label(wbt) if wbt in wbt_label_values else None),
         )
         curves.append(c)
 
@@ -412,14 +488,15 @@
     rh_max: float,
     pressure: float,
     style: ZoneStyle,
     label: str | None = None,
 ) -> PsychroCurve:
     """Generate points for zone between constant dry bulb temps and RH."""
     temps = np.arange(t_min, t_max + increment, increment)
+    assert rh_min >= 0.0 and rh_max <= 100.0
     curve_rh_up = gen_points_in_constant_relative_humidity(
         temps, rh_max, pressure
     )
     curve_rh_down = gen_points_in_constant_relative_humidity(
         temps, rh_min, pressure
     )
     abs_humid: list[float] = (
@@ -455,13 +532,13 @@
             pressure,
             zone_conf.style,
             label=zone_conf.label,
         )
     else:
         # zone_type: 'xy-points'
         return PsychroCurve(
-            x_data=zone_conf.points_x,
-            y_data=zone_conf.points_y,
+            x_data=np.array(zone_conf.points_x),
+            y_data=np.array(zone_conf.points_y),
             style=zone_conf.style,
             type_curve="custom path",
             label=zone_conf.label,
         )
```

### Comparing `psychrochart-0.5.0/psychrochart/models/annots.py` & `psychrochart-0.6.0/psychrochart/models/annots.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/models/config.py` & `psychrochart-0.6.0/psychrochart/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-from pydantic import BaseModel, Extra, Field
+from pydantic import Extra, Field
 
-from psychrochart.models.styles import CurveStyle, LabelStyle, TickStyle
+from psychrochart.models.styles import (
+    BaseConfig,
+    CurveStyle,
+    LabelStyle,
+    TickStyle,
+)
 
 _DEFAULT_RANGE_VOL_M3_KG = (0.78, 0.98)
 _DEFAULT_RANGE_ENTALPHY = (5, 155)
 _DEFAULT_RANGE_WET_TEMP = (-10, 40)
 _DEFAULT_POSITION = [0.025, 0.075, 0.925, 0.875]
 
 _DEFAULT_RH_CURVES = [10, 20, 30, 40, 45, 50, 55, 60, 70, 80, 90]
@@ -28,18 +33,19 @@
     color=[0.855, 0.145, 0.114], linewidth=0.75, linestyle=":"
 )
 _DEFAULT_STYLE_HUMID = CurveStyle(
     color=[0.0, 0.125, 0.376], linewidth=0.75, linestyle=":"
 )
 
 
-class ChartFigure(BaseModel):
+class ChartFigure(BaseConfig):
     """Psychrochart settings for matplotlib Figure."""
 
     figsize: tuple[float, float] = Field(default=(16, 9))
+    dpi: int = Field(default=150)
     fontsize: int = Field(default=10)
     title: str | None = Field(default="Psychrometric Chart")
     x_label: str | None = Field(default="Dry-bulb temperature, $°C$")
     y_label: str | None = Field(default="Humidity ratio $w, g_w / kg_{da}$")
 
     x_axis: CurveStyle = Field(default=_DEFAULT_X_AXIS)
     x_axis_labels: LabelStyle = Field(default=_DEFAULT_X_AXIS_LABELS)
@@ -50,33 +56,31 @@
 
     partial_axis: bool = Field(default=True)
     position: list[float] = Field(
         default_factory=lambda: list(_DEFAULT_POSITION)
     )
 
 
-class ChartLimits(BaseModel):
+class ChartLimits(BaseConfig):
     """Psychrochart temperature + humidity + pressure limits."""
 
     range_temp_c: tuple[float, float] = Field(default=(0, 50))
     range_humidity_g_kg: tuple[float, float] = Field(default=(0, 40))
     altitude_m: int = Field(default=0)
     pressure_kpa: float | None = Field(default=None)
     step_temp: float = Field(default=1)
 
 
-class ChartParams(BaseModel):
+class ChartParams(BaseConfig):
     """Psychrochart plotting parameters."""
 
     with_constant_rh: bool = Field(default=True)
     constant_rh_label: str | None = Field(default="Constant relative humidity")
     constant_rh_curves: list[int] = Field(default=_DEFAULT_RH_CURVES)
-    constant_rh_labels: list[float] = Field(
-        default=_DEFAULT_CONSTANT_RH_LABELS
-    )
+    constant_rh_labels: list[int] = Field(default=_DEFAULT_CONSTANT_RH_LABELS)
     constant_rh_labels_loc: float = Field(default=0.85)
 
     with_constant_v: bool = Field(default=True)
     constant_v_label: str | None = Field(default="Constant specific volume")
     constant_v_step: float = Field(default=0.02)
     range_vol_m3_kg: tuple[float, float] = Field(
         default=_DEFAULT_RANGE_VOL_M3_KG
@@ -114,15 +118,15 @@
     constant_humid_step: float = Field(default=1)
     constant_humid_label_step: float = Field(default=2)
     constant_humid_label_include_limits: bool = Field(default=True)
 
     with_zones: bool = Field(default=True)
 
 
-class ChartConfig(BaseModel):
+class ChartConfig(BaseConfig):
     """
     Psychrochart configuration model.
 
     Includes:
     * matplotlib figure settings and styling
     * chart limits
     * plotting parameters
```

### Comparing `psychrochart-0.5.0/psychrochart/models/curves.py` & `psychrochart-0.6.0/psychrochart/models/curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,16 +116,16 @@
         if (
             self.x_data is None
             or self.y_data is None
             or not _between_limits(
                 self.x_data, self.y_data, xmin, xmax, ymin, ymax
             )
         ):
-            logging.debug(
-                "%s (label:%s) Not between limits ([%.2g, %.2g, %.2g, %.2g]) "
+            logging.info(
+                "%s (label:%s) not between limits ([%.2g, %.2g, %.2g, %.2g]) "
                 "-> x:%s, y:%s",
                 self.type_curve,
                 self.label or "unnamed",
                 xmin,
                 xmax,
                 ymin,
                 ymax,
```

### Comparing `psychrochart-0.5.0/psychrochart/models/parsers.py` & `psychrochart-0.6.0/psychrochart/models/parsers.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/models/styles.py` & `psychrochart-0.6.0/psychrochart/models/styles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from pydantic import BaseModel, Extra, Field, root_validator, validator
+from pydantic import Extra, Field, root_validator, validator
 
+from psychrochart.models.base import BaseConfig
 from psychrochart.models.validators import parse_color, reduce_field_abrs
 
 
-class CurveStyle(BaseModel):
+class CurveStyle(BaseConfig):
     """Container for matplotlib styling of psychro curve."""
 
     color: list[float] = Field(default=[0.2, 0.2, 0.2])
     linewidth: float = Field(default=1)
     linestyle: str = Field(default="-")
 
     class Config:
@@ -18,43 +19,43 @@
         return parse_color(v)
 
     @root_validator(pre=True)
     def _remove_aliases(cls, values):
         return reduce_field_abrs(values)
 
 
-class LabelStyle(BaseModel):
+class LabelStyle(BaseConfig):
     """Container for matplotlib styling of labels."""
 
     color: list[float] = Field(default=[0.2, 0.2, 0.2])
     fontsize: int | float = Field(default=9)
 
     class Config:
         extra = Extra.allow
 
     @validator("color", pre=True, always=True)
     def _color_arr(cls, v, values):
         return parse_color(v)
 
 
-class TickStyle(BaseModel):
+class TickStyle(BaseConfig):
     """Container for matplotlib tick axes styling."""
 
     direction: str = Field(default="out")
     color: list[float] = Field(default=[0.2, 0.2, 0.2])
 
     class Config:
         extra = Extra.allow
 
     @validator("color", pre=True, always=True)
     def _color_arr(cls, v, values):
         return parse_color(v)
 
 
-class ZoneStyle(BaseModel):
+class ZoneStyle(BaseConfig):
     """Container for matplotlib patch styling of zones in psychrochart."""
 
     edgecolor: list[float]
     facecolor: list[float]
     linewidth: float = Field(default=2)
     linestyle: str = Field(default="--")
```

### Comparing `psychrochart-0.5.0/psychrochart/models/validators.py` & `psychrochart-0.6.0/psychrochart/models/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from matplotlib.colors import to_rgb
+from matplotlib.colors import to_rgba
 import numpy as np
 
 
 def parse_color(raw_color) -> list[float]:
     """Pydantic validator for 'color' fields, stored as float values."""
     if isinstance(raw_color, str):
-        return list(to_rgb(raw_color))
+        return list(to_rgba(raw_color))
     return list(raw_color)
 
 
 def reduce_field_abrs(values):
     """Pydantic validator for abbreviation of matplotlib style fields."""
     if "c" in values:
         values["color"] = parse_color(values.pop("c"))
```

### Comparing `psychrochart-0.5.0/psychrochart/plot_logic.py` & `psychrochart-0.6.0/psychrochart/plot_logic.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.5.0/psychrochart/process_logic.py` & `psychrochart-0.6.0/psychrochart/process_logic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 import logging
 from typing import Any
 
 import numpy as np
 import psychrolib as psy
-from psychrolib import GetStandardAtmPressure, IP, SetUnitSystem, SI
+from psychrolib import (
+    GetStandardAtmPressure,
+    GetUnitSystem,
+    IP,
+    SetUnitSystem,
+    SI,
+)
+from scipy.interpolate import interp1d
 
 from psychrochart.chartdata import (
+    get_rh_max_min_in_limits,
     make_constant_dry_bulb_v_lines,
     make_constant_enthalpy_lines,
     make_constant_humidity_ratio_h_lines,
     make_constant_relative_humidity_lines,
     make_constant_specific_volume_lines,
     make_constant_wet_bulb_temperature_lines,
     make_saturation_line,
     make_zone_curve,
 )
 from psychrochart.models.annots import ChartZones, DEFAULT_ZONES
-from psychrochart.models.config import ChartConfig
+from psychrochart.models.config import ChartConfig, ChartLimits
 from psychrochart.models.curves import PsychroChartModel, PsychroCurves
 from psychrochart.models.parsers import obj_loader
 
 spec_vol_vec = np.vectorize(psy.GetMoistAirVolume)
 
 
 def set_unit_system(use_unit_system_si: bool = True) -> None:
     """Set unit system for psychrolib."""
-    if use_unit_system_si:
+    if use_unit_system_si and GetUnitSystem() != SI:
         SetUnitSystem(SI)
         logging.info("[SI units mode] ENABLED")
-    else:
+    elif not use_unit_system_si and GetUnitSystem() != IP:
         SetUnitSystem(IP)
         logging.info("[IP units mode] ENABLED")
 
 
+def get_pressure_pa(limits: ChartLimits, unit_system_si: bool = True) -> float:
+    """Set unit system and process ChartLimits for base pressure for chart."""
+    set_unit_system(unit_system_si)
+    if limits.pressure_kpa is not None:
+        return limits.pressure_kpa * 1000.0  # to Pa
+    else:
+        return GetStandardAtmPressure(limits.altitude_m)
+
+
 def append_zones_to_chart(
     config: ChartConfig,
     chart: PsychroChartModel,
     zones: ChartZones | dict[str, Any] | str | None = None,
 ) -> None:
     """Append zones as patches to the psychrometric chart data-container."""
     chart.zones.append(
@@ -49,53 +66,44 @@
                     ChartZones, zones, default_obj=DEFAULT_ZONES
                 ).zones
             ]
         )
     )
 
 
-def generate_psychrochart(
-    config: ChartConfig,
-    extra_zones: ChartZones | dict[str, Any] | str | None = None,
-    use_unit_system_si: bool = True,
-) -> PsychroChartModel:
-    """Create the PsychroChart object."""
-    # Set unit system for psychrolib and get standard pressure
-    altitude_m = -1
-    set_unit_system(use_unit_system_si)
-    if config.limits.pressure_kpa is not None:
-        pressure = config.limits.pressure_kpa * 1000.0  # to Pa
-    else:
-        altitude_m = config.limits.altitude_m
-        pressure = GetStandardAtmPressure(altitude_m)
-
-    # base chart with saturation line:
-    chart = PsychroChartModel(
-        unit_system_si=use_unit_system_si,
-        altitude_m=altitude_m,
-        pressure=pressure,
-        saturation=make_saturation_line(
-            config.dbt_min,
-            config.dbt_max,
-            config.limits.step_temp,
-            pressure,
-            style=config.saturation,
-        ),
-    )
+def _generate_chart_curves(
+    config: ChartConfig, chart: PsychroChartModel, pressure: float
+):
+    # check chart limits are not fully above the saturation curve!
+    assert (chart.saturation.curves[0].y_data > config.w_min).any()
+    # check if sat curve cuts x-axis with T > config.dbt_min
+    dbt_min_seen: float | None = None
+    if chart.saturation.curves[0].y_data[0] < config.w_min:
+        temp_sat_interpolator = interp1d(
+            chart.saturation.curves[0].y_data,
+            chart.saturation.curves[0].x_data,
+            assume_sorted=True,
+        )
+        dbt_min_seen = temp_sat_interpolator(config.w_min)
 
     # Dry bulb constant lines (vertical):
     if config.chart_params.with_constant_dry_temp:
         step = config.chart_params.constant_temp_step
+        temps_vl = np.arange(config.dbt_min, config.dbt_max, step)
+        if dbt_min_seen:
+            temps_vl = temps_vl[temps_vl > dbt_min_seen]
         chart.constant_dry_temp_data = make_constant_dry_bulb_v_lines(
             config.w_min,
             pressure,
-            temps_vl=np.arange(config.dbt_min, config.dbt_max, step),
+            temps_vl=temps_vl,
             style=config.constant_dry_temp,
             family_label=config.chart_params.constant_temp_label,
         )
+    else:
+        chart.constant_dry_temp_data = None
 
     # Absolute humidity constant lines (horizontal):
     if config.chart_params.with_constant_humidity:
         step = config.chart_params.constant_humid_step
         chart.constant_humidity_data = make_constant_humidity_ratio_h_lines(
             config.dbt_max,
             pressure,
@@ -103,70 +111,149 @@
                 config.w_min + step,
                 config.w_max + step / 10,
                 step,
             ),
             style=config.constant_humidity,
             family_label=config.chart_params.constant_humid_label,
         )
+    else:
+        chart.constant_humidity_data = None
 
     # Constant relative humidity curves:
     if config.chart_params.with_constant_rh:
+        rh_min, rh_max = get_rh_max_min_in_limits(
+            dbt_min_seen or config.dbt_min,
+            config.dbt_max,
+            config.w_min,
+            config.w_max,
+            pressure,
+        )
+        rh_values = sorted(
+            rh
+            for rh in config.chart_params.constant_rh_curves
+            if rh_min < rh < rh_max
+        )
+        start = (
+            config.limits.step_temp * (dbt_min_seen // config.limits.step_temp)
+            if dbt_min_seen
+            else config.dbt_min
+        )
         chart.constant_rh_data = make_constant_relative_humidity_lines(
-            config.dbt_min,
+            start,
             config.dbt_max,
             config.limits.step_temp,
             pressure,
-            rh_perc_values=config.chart_params.constant_rh_curves,
+            rh_perc_values=rh_values,
             rh_label_values=config.chart_params.constant_rh_labels,
             style=config.constant_rh,
             label_loc=config.chart_params.constant_rh_labels_loc,
             family_label=config.chart_params.constant_rh_label,
         )
+    else:
+        chart.constant_rh_data = None
 
     # Constant enthalpy lines:
     if config.chart_params.with_constant_h:
         step = config.chart_params.constant_h_step
         start, end = config.chart_params.range_h
         chart.constant_h_data = make_constant_enthalpy_lines(
             config.w_min,
             pressure,
             enthalpy_values=np.arange(start, end, step),
             h_label_values=config.chart_params.constant_h_labels,
             style=config.constant_h,
             label_loc=config.chart_params.constant_h_labels_loc,
             family_label=config.chart_params.constant_h_label,
             saturation_curve=chart.saturation.curves[0],
+            dbt_min_seen=dbt_min_seen,
         )
+    else:
+        chart.constant_h_data = None
 
     # Constant specific volume lines:
     if config.chart_params.with_constant_v:
         step = config.chart_params.constant_v_step
         start, end = config.chart_params.range_vol_m3_kg
         chart.constant_v_data = make_constant_specific_volume_lines(
             config.w_min,
             pressure,
             vol_values=np.arange(start, end, step),
             v_label_values=config.chart_params.constant_v_labels,
             style=config.constant_v,
             label_loc=config.chart_params.constant_v_labels_loc,
             family_label=config.chart_params.constant_v_label,
             saturation_curve=chart.saturation.curves[0],
+            dbt_min_seen=dbt_min_seen,
         )
+    else:
+        chart.constant_v_data = None
 
     # Constant wet bulb temperature lines:
     if config.chart_params.with_constant_wet_temp:
         step = config.chart_params.constant_wet_temp_step
         start, end = config.chart_params.range_wet_temp
         chart.constant_wbt_data = make_constant_wet_bulb_temperature_lines(
+            dbt_min_seen or config.dbt_min,
             config.dbt_max,
+            config.w_min,
+            config.w_max,
             pressure,
             wbt_values=np.arange(start, end, step),
             wbt_label_values=config.chart_params.constant_wet_temp_labels,
             style=config.constant_wet_temp,
             label_loc=config.chart_params.constant_wet_temp_labels_loc,
             family_label=config.chart_params.constant_wet_temp_label,
         )
+    else:
+        chart.constant_wbt_data = None
+
+
+def generate_psychrochart(
+    config: ChartConfig,
+    extra_zones: ChartZones | dict[str, Any] | str | None = None,
+    use_unit_system_si: bool = True,
+) -> PsychroChartModel:
+    """Create the PsychroChart object."""
+    # Set unit system for psychrolib and get standard pressure
+    pressure = get_pressure_pa(config.limits, use_unit_system_si)
+
+    # base chart with saturation line:
+    chart = PsychroChartModel(
+        unit_system_si=use_unit_system_si,
+        altitude_m=config.limits.altitude_m,
+        pressure=pressure,
+        saturation=make_saturation_line(
+            config.dbt_min,
+            config.dbt_max,
+            config.limits.step_temp,
+            pressure,
+            style=config.saturation,
+        ),
+    )
+    _generate_chart_curves(config, chart, pressure)
 
     if config.chart_params.with_zones:
         append_zones_to_chart(config, chart, extra_zones)
 
     return chart
+
+
+def update_psychrochart_data(
+    current_chart: PsychroChartModel, config: ChartConfig
+) -> None:
+    """Update the PsychroChart data with config changes."""
+    if config.limits.has_changed:
+        current_chart.altitude_m = config.limits.altitude_m
+        current_chart.pressure = get_pressure_pa(
+            config.limits, current_chart.unit_system_si
+        )
+
+    # regen all curves
+    current_chart.saturation = make_saturation_line(
+        config.dbt_min,
+        config.dbt_max,
+        config.limits.step_temp,
+        current_chart.pressure,
+        style=config.saturation,
+    )
+    _generate_chart_curves(config, current_chart, current_chart.pressure)
+    config.commit_changes()
```

### Comparing `psychrochart-0.5.0/psychrochart/util.py` & `psychrochart-0.6.0/psychrochart/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 NUM_ITERS_MAX = 100
 TESTING_MODE = os.getenv("PYTEST_CURRENT_TEST") is not None
 
 
 def _iter_solver(
     initial_value: np.ndarray,
     objective_value: np.ndarray,
-    func_eval: Callable,
+    func_eval: Callable[[np.ndarray | float], float],
     initial_increment: float = 4.0,
     num_iters_max: int = NUM_ITERS_MAX,
     precision: float = 0.01,
 ) -> tuple[float, int]:
     """Solve by iteration."""
     decreasing = True
     increment = initial_increment
@@ -27,21 +27,21 @@
         error = objective_value - iteration_value
         if abs(error) < precision:
             break
         if error < 0:
             if not decreasing:
                 increment /= 2
                 decreasing = True
-            increment = max(precision / 10, increment)
+            increment = max(precision / 20, increment)
             value_calc -= increment
         else:
             if decreasing:
                 increment /= 2
                 decreasing = False
-            increment = max(precision / 10, increment)
+            increment = max(precision / 20, increment)
             value_calc += increment
         num_iter += 1
 
         if num_iter == num_iters_max:  # pragma: no cover
             raise AssertionError(
                 f"No convergence error after {num_iter} iterations! "
                 f"Last value: {value_calc}, ∆: {increment}. "
@@ -49,16 +49,16 @@
             )
     return value_calc, num_iter
 
 
 def solve_curves_with_iteration(
     family_name,
     objective_values: np.ndarray,
-    func_init: Callable,
-    func_eval: Callable,
+    func_init: Callable[[np.ndarray], float],
+    func_eval: Callable[[np.ndarray | float], float],
 ) -> np.ndarray:
     """Run the iteration solver for a list of objective values
     for the three types of curves solved with this method."""
     # family:= checking precision | initial_increment | precision
     families = {
         "ENTHALPHY": (0.01, 0.5, 0.01),
         "CONSTANT VOLUME": (0.0005, 1, 0.00025),
```

### Comparing `psychrochart-0.5.0/pyproject.toml` & `psychrochart-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [tool.black]
-exclude = "^.*/charts/.*$"
 line_length = 79
 target_version = ["py311"]
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 combine_as_imports = true
@@ -39,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.5.0"
+version = "0.6.0"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `psychrochart-0.5.0/PKG-INFO` & `psychrochart-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.5.0
+Version: 0.6.0
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.12
@@ -85,16 +85,24 @@
 ## Usage
 
 ```python
 from psychrochart import PsychroChart
 
 # Load default style:
 chart_default = PsychroChart.create()
+# customize anything
+chart_default.limits.range_temp_c = (15.0, 35.0)
+chart_default.limits.range_humidity_g_kg = (5, 25)
+chart_default.config.saturation.linewidth = 1
+chart_default.config.constant_wet_temp.color = "darkblue"
+# plot
 axes = chart_default.plot()
 axes.get_figure()
+# or store on disk
+chart_default.save("my-custom-chart.svg")
 ```
 
 Called from the terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
 
 ```python
 from psychrochart import PsychroChart
 import matplotlib.pyplot as plt
@@ -102,15 +110,15 @@
 PsychroChart.create().plot(ax=plt.gca())
 plt.show()
 ```
 
 ### Chart customization
 
 The default styling for charts is defined in JSON files that you can change, or you can pass a path of a file in JSON, or a dict, when you create the psychrometric chart object.
-Included styles are: `default`, `ashrae`, `interior` and `minimal`.
+Included styles are: `default`, `ashrae`, `ashrae_ip` (adjusted for IP units), `interior`, and `minimal`.
 
 ```python
 from pathlib import Path
 from psychrochart import load_config, PsychroChart
 
 # Load preconfigured styles:
 chart_ashrae_style = PsychroChart.create('ashrae')
```

