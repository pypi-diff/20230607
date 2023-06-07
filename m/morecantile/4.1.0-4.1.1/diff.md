# Comparing `tmp/morecantile-4.1.0.tar.gz` & `tmp/morecantile-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "morecantile-4.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-4.1.0.tar` & `morecantile-4.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      215 2023-06-06 16:11:11.947318 morecantile-4.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-06-06 16:11:11.947318 morecantile-4.1.0/.gitignore
--rw-r--r--   0        0        0      822 2023-06-06 16:11:11.947318 morecantile-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-06-06 16:11:11.947318 morecantile-4.1.0/LICENSE
--rw-r--r--   0        0        0     5305 2023-06-06 16:11:11.947318 morecantile-4.1.0/README.md
--rw-r--r--   0        0        0      436 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/commons.py
--rw-r--r--   0        0        0     7267 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/CanadianNAD83_LCC.json
--rw-r--r--   0        0        0     4679 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5176 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     8457 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/README.md
--rw-r--r--   0        0        0     7374 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     7365 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     7367 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6932 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/WGS1984Quad.json
--rw-r--r--   0        0        0     7843 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     7072 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/data/WorldCRS84Quad.json
--rw-r--r--   0        0        0     7001 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1748 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/defaults.py
--rw-r--r--   0        0        0      907 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/errors.py
--rw-r--r--   0        0        0    41068 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16657 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3364 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/utils.py
--rw-r--r--   0        0        0     2295 2023-06-06 16:11:11.951318 morecantile-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0      215 2023-06-07 13:57:21.361458 morecantile-4.1.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-06-07 13:57:21.361458 morecantile-4.1.1/.gitignore
+-rw-r--r--   0        0        0      822 2023-06-07 13:57:21.361458 morecantile-4.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-06-07 13:57:21.361458 morecantile-4.1.1/LICENSE
+-rw-r--r--   0        0        0     5305 2023-06-07 13:57:21.361458 morecantile-4.1.1/README.md
+-rw-r--r--   0        0        0      436 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/commons.py
+-rw-r--r--   0        0        0     7267 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0     5176 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1748 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/errors.py
+-rw-r--r--   0        0        0    41387 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/utils.py
+-rw-r--r--   0        0        0     2295 2023-06-07 13:57:21.365458 morecantile-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.1.1/PKG-INFO
```

### Comparing `morecantile-4.1.0/.gitignore` & `morecantile-4.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/.pre-commit-config.yaml` & `morecantile-4.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/LICENSE` & `morecantile-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/README.md` & `morecantile-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/commons.py` & `morecantile-4.1.1/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-4.1.1/morecantile/data/CanadianNAD83_LCC.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/EuropeanETRS89_LAEAQuad.json` & `morecantile-4.1.1/morecantile/data/EuropeanETRS89_LAEAQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-4.1.1/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/NZTM2000Quad.json` & `morecantile-4.1.1/morecantile/data/NZTM2000Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/UPSAntarcticWGS84Quad.json` & `morecantile-4.1.1/morecantile/data/UPSAntarcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/UPSArcticWGS84Quad.json` & `morecantile-4.1.1/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/UTM31WGS84Quad.json` & `morecantile-4.1.1/morecantile/data/UTM31WGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/WGS1984Quad.json` & `morecantile-4.1.1/morecantile/data/WGS1984Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/WebMercatorQuad.json` & `morecantile-4.1.1/morecantile/data/WebMercatorQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/WorldCRS84Quad.json` & `morecantile-4.1.1/morecantile/data/WorldCRS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/data/WorldMercatorWGS84Quad.json` & `morecantile-4.1.1/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/defaults.py` & `morecantile-4.1.1/morecantile/defaults.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/errors.py` & `morecantile-4.1.1/morecantile/errors.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/models.py` & `morecantile-4.1.1/morecantile/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from pydantic import (
     AnyHttpUrl,
     AnyUrl,
     BaseModel,
     Field,
     PrivateAttr,
     conlist,
-    root_validator,
     validator,
 )
 from pyproj import CRS, Transformer
 from pyproj.exceptions import CRSError, ProjError
 
 from morecantile.commons import BoundingBox, Coords, Tile
 from morecantile.errors import (
@@ -99,20 +98,31 @@
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/common-geodata/crs.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
     __root__: Union[str, Union[CRSUri, CRSWKT]] = Field(..., title="CRS")
+    _pyproj_crs: CRS = PrivateAttr()
 
-    @root_validator
-    def validate_crs(cls, values):
-        """Make sure the CRS can be used in Pyproj."""
-        assert CRS.from_user_input(values.get("__root__"))
-        return values
+    def __init__(self, **data):
+        """Custom Init to validate CRS string and create Pyproj CRS object."""
+        super().__init__(**data)
+
+        _pyproj_crs = CRS.from_user_input(data.get("__root__"))
+
+        self._pyproj_crs = _pyproj_crs
+
+    def to_epsg(self) -> Optional[int]:
+        """return EPSG number of the CRS."""
+        return self._pyproj_crs.to_epsg()
+
+    def to_wkt(self) -> str:
+        """return WKT version of the CRS."""
+        return self._pyproj_crs.to_wkt()
 
 
 def CRS_to_uri(crs: CRS) -> str:
     """Convert CRS to URI."""
     authority = "EPSG"
     code = None
     version = "0"
```

### Comparing `morecantile-4.1.0/morecantile/scripts/cli.py` & `morecantile-4.1.1/morecantile/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/morecantile/utils.py` & `morecantile-4.1.1/morecantile/utils.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/pyproject.toml` & `morecantile-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.0/PKG-INFO` & `morecantile-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 4.1.0
+Version: 4.1.1
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: morecantile Version: 4.1.0 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 4.1.1 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

