# Comparing `tmp/openepd-0.6.0.tar.gz` & `tmp/openepd-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.6.0.tar", max compression
+gzip compressed data, was "openepd-0.7.0.tar", max compression
```

## Comparing `openepd-0.6.0.tar` & `openepd-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-02 12:58:17.392304 openepd-0.6.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-06-02 12:58:17.392304 openepd-0.6.0/README.md
--rw-r--r--   0        0        0     3051 2023-06-02 12:58:17.392304 openepd-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     2613 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     3365 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    12201 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     8887 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3811 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2855 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3342 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-06-02 12:58:17.392304 openepd-0.6.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 09:51:04.050774 openepd-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2841 2023-06-07 09:51:04.050774 openepd-0.7.0/README.md
+-rw-r--r--   0        0        0     3051 2023-06-07 09:51:04.050774 openepd-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     2613 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     3365 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    12201 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0    11266 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3811 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2855 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.7.0/PKG-INFO
```

### Comparing `openepd-0.6.0/LICENSE` & `openepd-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/README.md` & `openepd-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/pyproject.toml` & `openepd-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.6.0"
+version = "0.7.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.6.0"
+version = "0.7.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.6.0/src/openepd/__init__.py` & `openepd-0.7.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/__version__.py` & `openepd-0.7.0/src/openepd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.6.0"
+VERSION = "0.7.0"
```

### Comparing `openepd-0.6.0/src/openepd/model/__init__.py` & `openepd-0.7.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/base.py` & `openepd-0.7.0/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/common.py` & `openepd-0.7.0/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/epd.py` & `openepd-0.7.0/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/lcia.py` & `openepd-0.7.0/src/openepd/model/lcia.py`

 * *Files 26% similar despite different names*

```diff
@@ -157,13 +157,45 @@
         "First use bio-based materials used as an energy source. Hydropower, solar and wind power used "
         "in the technosphere are also included in this indicator"
     )
     RPRm: ScopeSet | None = pyd.Field(
         description="Renewable primary resources with energy content used as material. "
         "First use biobased materials used as materials (e.g. wood, hemp, etc.)."
     )
+    rpre: ScopeSet | None = pyd.Field(description="Renewable primary energy resources as energy")
+    nrpre: ScopeSet | None = pyd.Field(description="Non-renewable primary resources as energy (fuel)")
+    nrprm: ScopeSet | None = pyd.Field(description="Non-renewable primary resources as material")
+    fw: ScopeSet | None = pyd.Field(description="Use of net fresh water")
+    sm: ScopeSet | None = pyd.Field(description="Use of secondary materials")
+    rsf: ScopeSet | None = pyd.Field(description="Use of renewable secondary materials")
+    nrsf: ScopeSet | None = pyd.Field(description="Use of non-renewable secondary fuels")
+    re: ScopeSet | None = pyd.Field(description="Renewable energy resources")
+    pere: ScopeSet | None = pyd.Field(
+        description="Use of renewable primary energy excluding renewable primary energy resources used as raw materials"
+    )
+    perm: ScopeSet | None = pyd.Field(description="Use of renewable primary energy resources used as raw materials")
+    pert: ScopeSet | None = pyd.Field(description="Total use of renewable primary energy resources")
+    penre: ScopeSet | None = pyd.Field(
+        description="Use of non-renewable primary energy excluding "
+        "non-renewable primary energy resources used as raw materials"
+    )
+    penrm: ScopeSet | None = pyd.Field(
+        description="Use of non-renewable primary energy resources used as raw materials"
+    )
+    penrt: ScopeSet | None = pyd.Field(description="Total use of non-renewable primary energy resources")
 
 
 class OutputFlowSet(BaseOpenEpdSchema):
     """A set of output flows, such as waste, emissions, etc."""
 
+    twd: ScopeSet | None = pyd.Field(description="Total waste disposed")
     hwd: ScopeSet | None = pyd.Field(description="Hazardous waste disposed")
+    nhwd: ScopeSet | None = pyd.Field(description="Non-hazardous waste disposed")
+    rwd: ScopeSet | None = pyd.Field(description="Radioactive waste disposed")
+    hlrw: ScopeSet | None = pyd.Field(description="High level radioactive waste disposed")
+    illrw: ScopeSet | None = pyd.Field(description="Intermediate level radioactive waste disposed")
+    cru: ScopeSet | None = pyd.Field(description="Components for re-use")
+    mr: ScopeSet | None = pyd.Field(description="Recycled materials")
+    mfr: ScopeSet | None = pyd.Field(description="Materials for recycling")
+    mer: ScopeSet | None = pyd.Field(description="Materials for energy recovery")
+    ee: ScopeSet | None = pyd.Field(description="Exported energy")
+    eh: ScopeSet | None = pyd.Field(description="Exported heat")
```

### Comparing `openepd-0.6.0/src/openepd/model/org.py` & `openepd-0.7.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/pcr.py` & `openepd-0.7.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/specs/__init__.py` & `openepd-0.7.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/specs/concrete.py` & `openepd-0.7.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/src/openepd/model/standard.py` & `openepd-0.7.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-0.6.0/PKG-INFO` & `openepd-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.6.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.7.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

