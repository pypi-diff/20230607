# Comparing `tmp/lsmmdma-0.1.7.tar.gz` & `tmp/lsmmdma-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsmmdma-0.1.7.tar", last modified: Tue Jun  6 14:38:36 2023, max compression
+gzip compressed data, was "lsmmdma-0.1.8.tar", last modified: Wed Jun  7 09:13:45 2023, max compression
```

## Comparing `lsmmdma-0.1.7.tar` & `lsmmdma-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/lsmmdma/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/lsmmdma/data/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/data/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/data/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/mmdma_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/lsmmdma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/lsmmdma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 14:38:36.000000 lsmmdma-0.1.7/lsmmdma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:38:36.043531 lsmmdma-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-06 14:38:23.000000 lsmmdma-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:13:45.330102 lsmmdma-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-07 09:13:45.330102 lsmmdma-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:13:45.330102 lsmmdma-0.1.8/lsmmdma/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:13:45.330102 lsmmdma-0.1.8/lsmmdma/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/data/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/data/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/mmdma_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/lsmmdma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:13:45.330102 lsmmdma-0.1.8/lsmmdma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-07 09:13:45.000000 lsmmdma-0.1.8/lsmmdma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-07 09:13:45.000000 lsmmdma-0.1.8/lsmmdma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:13:45.000000 lsmmdma-0.1.8/lsmmdma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 09:13:45.000000 lsmmdma-0.1.8/lsmmdma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 09:13:45.000000 lsmmdma-0.1.8/lsmmdma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:13:45.330102 lsmmdma-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-07 09:13:36.000000 lsmmdma-0.1.8/setup.py
```

### Comparing `lsmmdma-0.1.7/LICENSE` & `lsmmdma-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/PKG-INFO` & `lsmmdma-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsmmdma
-Version: 0.1.7
+Version: 0.1.8
 Summary: Scaling MMD-MA.
 Home-page: https://github.com/google-research/large_scale_mmdma
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: kernel,data integration
 Classifier: Intended Audience :: Science/Research
@@ -78,15 +78,18 @@
 
 In Google Colab, use the following command:
 ```bash
 $ !pip install lsmmdma
 ```
 
 The KeOps library might require to be installed separately in advance, according
-to the given [instructions](http://www.kernel-operations.io/keops/python/installation.html).
+to the given [instructions](http://www.kernel-operations.io/keops/python/installation.html). Typically, in Google Colab one would run this command before installing `lsmmmdma`:
+```bash
+$ !pip install pykeops
+```
 
 ## Command line instructions<a id="commandline"></a>
 
 The algorithm can be run with a command line using:
 
 ```bash
 python3 -m lsmmmda.main [flags]
```

### Comparing `lsmmdma-0.1.7/README.md` & `lsmmdma-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,18 @@
 
 In Google Colab, use the following command:
 ```bash
 $ !pip install lsmmdma
 ```
 
 The KeOps library might require to be installed separately in advance, according
-to the given [instructions](http://www.kernel-operations.io/keops/python/installation.html).
+to the given [instructions](http://www.kernel-operations.io/keops/python/installation.html). Typically, in Google Colab one would run this command before installing `lsmmmdma`:
+```bash
+$ !pip install pykeops
+```
 
 ## Command line instructions<a id="commandline"></a>
 
 The algorithm can be run with a command line using:
 
 ```bash
 python3 -m lsmmmda.main [flags]
```

### Comparing `lsmmdma-0.1.7/lsmmdma/__init__.py` & `lsmmdma-0.1.8/lsmmdma/__init__.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/data/__init__.py` & `lsmmdma-0.1.8/lsmmdma/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/data/checkpointer.py` & `lsmmdma-0.1.8/lsmmdma/data/checkpointer.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/data/data_pipeline.py` & `lsmmdma-0.1.8/lsmmdma/data/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/initializers.py` & `lsmmdma-0.1.8/lsmmdma/initializers.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/main.py` & `lsmmdma-0.1.8/lsmmdma/main.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/metrics.py` & `lsmmdma-0.1.8/lsmmdma/metrics.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/mmdma_functions.py` & `lsmmdma-0.1.8/lsmmdma/mmdma_functions.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/train.py` & `lsmmdma-0.1.8/lsmmdma/train.py`

 * *Files identical despite different names*

### Comparing `lsmmdma-0.1.7/lsmmdma/version.py` & `lsmmdma-0.1.8/lsmmdma/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current mmdma version."""
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

### Comparing `lsmmdma-0.1.7/lsmmdma.egg-info/PKG-INFO` & `lsmmdma-0.1.8/lsmmdma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsmmdma
-Version: 0.1.7
+Version: 0.1.8
 Summary: Scaling MMD-MA.
 Home-page: https://github.com/google-research/large_scale_mmdma
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: kernel,data integration
 Classifier: Intended Audience :: Science/Research
@@ -78,15 +78,18 @@
 
 In Google Colab, use the following command:
 ```bash
 $ !pip install lsmmdma
 ```
 
 The KeOps library might require to be installed separately in advance, according
-to the given [instructions](http://www.kernel-operations.io/keops/python/installation.html).
+to the given [instructions](http://www.kernel-operations.io/keops/python/installation.html). Typically, in Google Colab one would run this command before installing `lsmmmdma`:
+```bash
+$ !pip install pykeops
+```
 
 ## Command line instructions<a id="commandline"></a>
 
 The algorithm can be run with a command line using:
 
 ```bash
 python3 -m lsmmmda.main [flags]
```

### Comparing `lsmmdma-0.1.7/setup.py` & `lsmmdma-0.1.8/setup.py`

 * *Files identical despite different names*

