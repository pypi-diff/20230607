# Comparing `tmp/jupyternb-setup-1.3.4rc3.tar.gz` & `tmp/jupyternb-setup-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyternb-setup-1.3.4rc3.tar", last modified: Thu Jun  1 18:23:49 2023, max compression
+gzip compressed data, was "jupyternb-setup-1.3.5.tar", last modified: Wed Jun  7 01:47:51 2023, max compression
```

## Comparing `jupyternb-setup-1.3.4rc3.tar` & `jupyternb-setup-1.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.4rc3/.gitignore
--rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.4rc3/LICENSE
--rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.4rc3/README.md
--rw-r--r--   0        0        0       51 2023-06-01 18:22:07.945162 jupyternb-setup-1.3.4rc3/jupyternb/__init__.py
--rw-r--r--   0        0        0    15366 2023-06-01 18:23:17.264441 jupyternb-setup-1.3.4rc3/jupyternb/jupyter_startup.py
--rw-r--r--   0        0        0      977 2023-06-01 18:23:33.328333 jupyternb-setup-1.3.4rc3/pyproject.toml
--rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.4rc3/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.5/.gitignore
+-rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.5/LICENSE
+-rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.5/README.md
+-rw-r--r--   0        0        0       48 2023-06-07 01:39:34.185379 jupyternb-setup-1.3.5/jupyternb/__init__.py
+-rw-r--r--   0        0        0    15458 2023-06-07 01:39:26.326953 jupyternb-setup-1.3.5/jupyternb/jupyter_startup.py
+-rw-r--r--   0        0        0      977 2023-06-01 18:23:33.328333 jupyternb-setup-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.5/PKG-INFO
```

### Comparing `jupyternb-setup-1.3.4rc3/.gitignore` & `jupyternb-setup-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc3/LICENSE` & `jupyternb-setup-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc3/README.md` & `jupyternb-setup-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc3/jupyternb/jupyter_startup.py` & `jupyternb-setup-1.3.5/jupyternb/jupyter_startup.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,17 +286,19 @@
             variable = variable.replace("export", "")
 
             # Remove leading/trailing whitespaces from the variable and value
             variable = variable.strip()
             value = value.strip()
 
             if variable in [self.FABRIC_BASTION_KEY_LOCATION, self.FABRIC_SLICE_PRIVATE_KEY_FILE]:
-                os.chmod(value, 0o600)
+                if os.path.exists(value):
+                    os.chmod(value, 0o600)
             elif variable in [self.FABRIC_SLICE_PUBLIC_KEY_FILE]:
-                os.chmod(value, 0o644)
+                if os.path.exists(value):
+                    os.chmod(value, 0o644)
 
     def initialize(self):
         """
         Initialize Jupyter Notebook Container
         """
         if not os.path.exists(self.token_location):
             # New jupyternb container has been created
```

### Comparing `jupyternb-setup-1.3.4rc3/pyproject.toml` & `jupyternb-setup-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc3/PKG-INFO` & `jupyternb-setup-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyternb-setup
-Version: 1.3.4rc3
+Version: 1.3.5
 Summary: Fabric Jupyter Notebook Container Setup
 Keywords: Fabric Jupyter Notebook Container Setup,Jupyter Hub,Jupyter Notebook
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

