# Comparing `tmp/tracarbon-0.6.4.tar.gz` & `tmp/tracarbon-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracarbon-0.6.4.tar", max compression
+gzip compressed data, was "tracarbon-0.6.5.tar", max compression
```

## Comparing `tracarbon-0.6.4.tar` & `tracarbon-0.6.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0    10264 2023-04-04 10:18:38.641134 tracarbon-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0     9707 2023-04-04 10:18:38.641134 tracarbon-0.6.4/README.md
--rw-r--r--   0        0        0     2643 2023-04-04 10:18:38.645135 tracarbon-0.6.4/pyproject.toml
--rwxr-xr-x   0        0        0      246 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/__init__.py
--rw-r--r--   0        0        0       70 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/__main__.py
--rw-r--r--   0        0        0     2225 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/builder.py
--rw-r--r--   0        0        0     4517 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/cli/__init__.py
--rwxr-xr-x   0        0        0     2320 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/conf.py
--rw-r--r--   0        0        0       51 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/emissions/__init__.py
--rw-r--r--   0        0        0     6361 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/emissions/carbon_emissions.py
--rw-r--r--   0        0        0      734 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exceptions.py
--rwxr-xr-x   0        0        0      237 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exporters/__init__.py
--rwxr-xr-x   0        0        0     2207 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exporters/datadog_exporter.py
--rwxr-xr-x   0        0        0     3617 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exporters/exporter.py
--rw-r--r--   0        0        0     2126 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exporters/json_exporter.py
--rw-r--r--   0        0        0     2524 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exporters/prometheus_exporter.py
--rwxr-xr-x   0        0        0      886 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/exporters/stdout.py
--rw-r--r--   0        0        0    10599 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/general_metrics.py
--rwxr-xr-x   0        0        0      210 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/__init__.py
--rw-r--r--   0        0        0     1303 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/cloud_providers.py
--rw-r--r--   0        0        0     4876 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/containers.py
--rw-r--r--   0        0        0        0 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/data/__init__.py
--rw-r--r--   0        0        0   160141 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/data/aws-instances.csv
--rw-r--r--   0        0        0     4720 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/energy.py
--rw-r--r--   0        0        0     1362 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/gpu.py
--rwxr-xr-x   0        0        0     1653 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/hardware.py
--rw-r--r--   0        0        0     6166 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/rapl.py
--rw-r--r--   0        0        0     7242 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/hardwares/sensors.py
--rwxr-xr-x   0        0        0       85 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/locations/__init__.py
--rw-r--r--   0        0        0     6229 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/locations/country.py
--rw-r--r--   0        0        0        0 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/locations/data/__init__.py
--rw-r--r--   0        0        0     1614 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json
--rw-r--r--   0        0        0     1179 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/locations/data/grid-emissions-factors-aws.csv
--rwxr-xr-x   0        0        0     1576 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/locations/location.py
--rw-r--r--   0        0        0        0 2023-04-04 10:18:38.649135 tracarbon-0.6.4/tracarbon/py.typed
--rw-r--r--   0        0        0    11297 1970-01-01 00:00:00.000000 tracarbon-0.6.4/PKG-INFO
+-rwxr-xr-x   0        0        0    10264 2023-06-07 14:21:37.910555 tracarbon-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     9707 2023-06-07 14:21:37.910555 tracarbon-0.6.5/README.md
+-rw-r--r--   0        0        0     2665 2023-06-07 14:21:37.914555 tracarbon-0.6.5/pyproject.toml
+-rwxr-xr-x   0        0        0      246 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/__main__.py
+-rw-r--r--   0        0        0     2225 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/builder.py
+-rw-r--r--   0        0        0     4517 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/cli/__init__.py
+-rwxr-xr-x   0        0        0     2320 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/conf.py
+-rw-r--r--   0        0        0       51 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/emissions/__init__.py
+-rw-r--r--   0        0        0     6361 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/emissions/carbon_emissions.py
+-rw-r--r--   0        0        0      734 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exceptions.py
+-rwxr-xr-x   0        0        0      237 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/__init__.py
+-rwxr-xr-x   0        0        0     2207 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/datadog_exporter.py
+-rwxr-xr-x   0        0        0     3617 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/exporter.py
+-rw-r--r--   0        0        0     2126 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/json_exporter.py
+-rw-r--r--   0        0        0     2524 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/prometheus_exporter.py
+-rwxr-xr-x   0        0        0      886 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/exporters/stdout.py
+-rw-r--r--   0        0        0    10599 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/general_metrics.py
+-rwxr-xr-x   0        0        0      210 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/__init__.py
+-rw-r--r--   0        0        0     1303 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/cloud_providers.py
+-rw-r--r--   0        0        0     4876 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/containers.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/data/__init__.py
+-rw-r--r--   0        0        0   160141 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/data/aws-instances.csv
+-rw-r--r--   0        0        0     4720 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/energy.py
+-rw-r--r--   0        0        0     1362 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/gpu.py
+-rwxr-xr-x   0        0        0     1653 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/hardware.py
+-rw-r--r--   0        0        0     6166 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/rapl.py
+-rw-r--r--   0        0        0     7242 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/hardwares/sensors.py
+-rwxr-xr-x   0        0        0       85 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/__init__.py
+-rw-r--r--   0        0        0     6103 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/country.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/data/__init__.py
+-rw-r--r--   0        0        0     1614 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json
+-rw-r--r--   0        0        0     1179 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/data/grid-emissions-factors-aws.csv
+-rwxr-xr-x   0        0        0     1576 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/locations/location.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:21:37.914555 tracarbon-0.6.5/tracarbon/py.typed
+-rw-r--r--   0        0        0    11290 1970-01-01 00:00:00.000000 tracarbon-0.6.5/PKG-INFO
```

### Comparing `tracarbon-0.6.4/LICENSE.txt` & `tracarbon-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/README.md` & `tracarbon-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/pyproject.toml` & `tracarbon-0.6.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 [tool.poetry]
 name = "tracarbon"
 authors = ["Florian Valeye <fvaleye@github.com>"]
-version = "0.6.4"
+version = "0.6.5"
 description = "Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions."
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["energy", "sustainability", "energy-consumption", "electricity-consumption", "energy-efficiency", "carbon-footprint", "carbon-emissions"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only"
 ]
 include = ["tracarbon/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-loguru = "^0.6.0"
+loguru = ">=0.6,<0.8"
 aiohttp = "^3.8.1"
 aiocache = "^0.12.0"
 aiofiles = "^23.1.0"
 psutil = "^5.9.4"
 ujson = "^5.7.0"
 msgpack = "^1.0.4"
 pydantic = "^1.10.7"
-typer = "^0.7.0"
+typer = ">=0.7,<0.10"
 ec2-metadata = "^2.11.0"
 python-dotenv = ">=0.21,<1.1"
 datadog = {version = ">=0.44,<0.46", optional = true}
-prometheus-client = {version = "^0.16", optional = true}
+prometheus-client = {version = ">=0.16,<0.18", optional = true}
 kubernetes = {version = "^26.1.0", optional = true}
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.0"
+mypy = "^1.3"
 black = "^23.3.0"
 isort = "^5.11.5"
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-mock = "^3.7.0"
 pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
-pytest-xdist = "^3.1.0"
+pytest-cov = "^4.1.0"
+pytest-xdist = "^3.3.1"
 pytest-clarity = "^1.0.1"
-sphinx = "^6.1.3"
+sphinx = "^7.0.1"
 pydata-sphinx-theme = "^0.13.3"
 toml = "^0.10.2"
 types-ujson = "^5.7.0"
 datadog = ">=0.44,<0.46"
-prometheus-client = "^0.16"
-types-requests = "^2.28.11"
+prometheus-client = ">=0.16,<0.18"
+types-requests = "^2.31.0"
 bandit = "^1.7.4"
 radon = "^6.0.1"
 types-aiofiles = "^23.1.0"
 kubernetes = "^26.1.0"
 
 [tool.poetry.extras]
 datadog = ["datadog"]
```

### Comparing `tracarbon-0.6.4/tracarbon/builder.py` & `tracarbon-0.6.5/tracarbon/builder.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/cli/__init__.py` & `tracarbon-0.6.5/tracarbon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/conf.py` & `tracarbon-0.6.5/tracarbon/conf.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/emissions/carbon_emissions.py` & `tracarbon-0.6.5/tracarbon/emissions/carbon_emissions.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/exceptions.py` & `tracarbon-0.6.5/tracarbon/exceptions.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/exporters/datadog_exporter.py` & `tracarbon-0.6.5/tracarbon/exporters/datadog_exporter.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/exporters/exporter.py` & `tracarbon-0.6.5/tracarbon/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/exporters/json_exporter.py` & `tracarbon-0.6.5/tracarbon/exporters/json_exporter.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/exporters/prometheus_exporter.py` & `tracarbon-0.6.5/tracarbon/exporters/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/exporters/stdout.py` & `tracarbon-0.6.5/tracarbon/exporters/stdout.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/general_metrics.py` & `tracarbon-0.6.5/tracarbon/general_metrics.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/cloud_providers.py` & `tracarbon-0.6.5/tracarbon/hardwares/cloud_providers.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/containers.py` & `tracarbon-0.6.5/tracarbon/hardwares/containers.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/data/aws-instances.csv` & `tracarbon-0.6.5/tracarbon/hardwares/data/aws-instances.csv`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/energy.py` & `tracarbon-0.6.5/tracarbon/hardwares/energy.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/gpu.py` & `tracarbon-0.6.5/tracarbon/hardwares/gpu.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/hardware.py` & `tracarbon-0.6.5/tracarbon/hardwares/hardware.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/rapl.py` & `tracarbon-0.6.5/tracarbon/hardwares/rapl.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/hardwares/sensors.py` & `tracarbon-0.6.5/tracarbon/hardwares/sensors.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/locations/country.py` & `tracarbon-0.6.5/tracarbon/locations/country.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,20 +156,18 @@
                         )
                 if not co2g_kwh:
                     raise CloudProviderRegionIsMissing(
                         f"The region [{region_name}] is not in the AWS grid emissions factors file."
                     )
 
     @cached()  # type: ignore
-    async def get_latest_co2g_kwh(self, today_date: str, hour: str) -> float:
+    async def get_latest_co2g_kwh(self) -> float:
         """
         Get the latest co2g_kwh for AWS.
 
-        :param today_date: the date for the request
-        :param hour: the hour for the request
         :return: the latest co2g_kwh
         """
         return self.co2g_kwh
 
     async def get_co2g_kwh(self) -> float:
         """
         Get the Co2g per kwh.
```

### Comparing `tracarbon-0.6.4/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json` & `tracarbon-0.6.5/tracarbon/locations/data/co2-emission-intensity-9.exhibit.json`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/locations/data/grid-emissions-factors-aws.csv` & `tracarbon-0.6.5/tracarbon/locations/data/grid-emissions-factors-aws.csv`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/tracarbon/locations/location.py` & `tracarbon-0.6.5/tracarbon/locations/location.py`

 * *Files identical despite different names*

### Comparing `tracarbon-0.6.4/PKG-INFO` & `tracarbon-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracarbon
-Version: 0.6.4
+Version: 0.6.5
 Summary: Tracarbon is a Python library that tracks your device's energy consumption and calculates your carbon emissions.
 License: Apache-2.0
 Keywords: energy,sustainability,energy-consumption,electricity-consumption,energy-efficiency,carbon-footprint,carbon-emissions
 Author: Florian Valeye
 Author-email: fvaleye@github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -20,21 +20,21 @@
 Provides-Extra: prometheus
 Requires-Dist: aiocache (>=0.12.0,<0.13.0)
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: datadog (>=0.44,<0.46) ; extra == "datadog"
 Requires-Dist: ec2-metadata (>=2.11.0,<3.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0) ; extra == "kubernetes"
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
-Requires-Dist: prometheus-client (>=0.16,<0.17) ; extra == "prometheus"
+Requires-Dist: prometheus-client (>=0.16,<0.18) ; extra == "prometheus"
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21,<1.1)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.7,<0.10)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 ![Tracarbon Logo](https://raw.githubusercontent.com/fvaleye/tracarbon/main/logo.png "Tracarbon logo")
 
 ![example workflow](https://github.com/fvaleye/tracarbon/actions/workflows/build.yml/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/tracarbon.svg?style=flat-square)](https://pypi.org/project/tracarbon/)
```

