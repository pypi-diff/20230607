# Comparing `tmp/fgo_api_types-2023.6.3.17.24.33.tar.gz` & `tmp/fgo_api_types-2023.6.7.4.43.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.6.3.17.24.33.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.6.7.4.43.22.tar", max compression
```

## Comparing `fgo_api_types-2023.6.3.17.24.33.tar` & `fgo_api_types-2023.6.7.4.43.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-06-03 17:24:12.099063 fgo_api_types-2023.6.3.17.24.33/LICENSE
--rw-r--r--   0        0        0      449 2023-06-03 17:24:12.099063 fgo_api_types-2023.6.3.17.24.33/README.md
--rw-r--r--   0        0        0        0 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157892 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    76303 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50619 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-06-03 17:24:33.691456 fgo_api_types-2023.6.3.17.24.33/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-06-03 17:24:34.019460 fgo_api_types-2023.6.3.17.24.33/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.3.17.24.33/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-07 04:43:01.173698 fgo_api_types-2023.6.7.4.43.22/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-07 04:43:01.173698 fgo_api_types-2023.6.7.4.43.22/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157892 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    76333 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50619 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-06-07 04:43:22.689691 fgo_api_types-2023.6.7.4.43.22/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-06-07 04:43:23.013691 fgo_api_types-2023.6.7.4.43.22/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.7.4.43.22/PKG-INFO
```

### Comparing `fgo_api_types-2023.6.3.17.24.33/LICENSE` & `fgo_api_types-2023.6.7.4.43.22/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/basic.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/common.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/enums.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/gameenums.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/nice.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,14 +643,15 @@
     num: int = -1
     name: str
     originalName: str
     ruby: str
     detail: Optional[str] = None
     unmodifiedDetail: Optional[str] = None
     type: NiceSkillType
+    svtId: int
     strengthStatus: int = -1
     priority: int = -1
     condQuestId: int = -1
     condQuestPhase: int = -1
     condLv: int = -1
     condLimitCount: int = -1
     icon: Optional[HttpUrl] = None
@@ -702,14 +703,15 @@
     rank: str
     type: str
     effectFlags: list[NiceTdEffectFlag]
     detail: Optional[str] = None
     unmodifiedDetail: Optional[str] = None
     npGain: NpGain
     npDistribution: list[int]
+    svtId: int
     strengthStatus: int
     priority: int
     condQuestId: int
     condQuestPhase: int
     releaseConditions: list[NiceSvtSkillRelease] = []
     individuality: list[NiceTrait]
     npSvts: list[NiceTdSvt]
```

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/raw.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/rayshift.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/fgo_api_types/search.py` & `fgo_api_types-2023.6.7.4.43.22/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.3.17.24.33/pyproject.toml` & `fgo_api_types-2023.6.7.4.43.22/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.06.03.17.24.33"
+version = "2023.06.07.04.43.22"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.6.3.17.24.33/PKG-INFO` & `fgo_api_types-2023.6.7.4.43.22/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.6.3.17.24.33
+Version: 2023.6.7.4.43.22
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

