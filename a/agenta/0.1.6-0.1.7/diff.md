# Comparing `tmp/agenta-0.1.6.tar.gz` & `tmp/agenta-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.6.tar", max compression
+gzip compressed data, was "agenta-0.1.7.tar", max compression
```

## Comparing `agenta-0.1.6.tar` & `agenta-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.6/README.md
--rw-r--r--   0        0        0       48 2023-06-07 08:35:40.016460 agenta-0.1.6/agenta/__init__.py
--rw-r--r--   0        0        0     3198 2023-06-07 08:35:40.016930 agenta-0.1.6/agenta/agenta.py
--rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.6/agenta/cli/helper.py
--rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.6/agenta/cli/main.py
--rw-r--r--   0        0        0     8450 2023-06-05 14:29:35.924942 agenta-0.1.6/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.6/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.6/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.6/agenta/client/api_models.py
--rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.6/agenta/client/client.py
--rw-r--r--   0        0        0      641 2023-06-05 14:29:35.925644 agenta-0.1.6/agenta/config.py
--rw-r--r--   0        0        0      131 2023-06-05 14:29:35.926009 agenta-0.1.6/agenta/config.toml
--rw-r--r--   0        0        0      374 2023-06-07 08:59:05.567568 agenta-0.1.6/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.6/agenta/docker/docker-assets/README.md
--rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.6/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2702 2023-06-07 09:02:57.670742 agenta-0.1.6/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0       43 2023-06-07 08:37:18.934913 agenta-0.1.6/agenta/templates/simple_prompt/.env.example
--rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.6/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.6/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.6/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.6/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      570 2023-06-07 09:11:07.717998 agenta-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 agenta-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.7/README.md
+-rw-r--r--   0        0        0       48 2023-06-07 08:35:40.016460 agenta-0.1.7/agenta/__init__.py
+-rw-r--r--   0        0        0     3198 2023-06-07 08:35:40.016930 agenta-0.1.7/agenta/agenta.py
+-rw-r--r--   0        0        0     2378 2023-06-05 14:29:35.924380 agenta-0.1.7/agenta/cli/helper.py
+-rw-r--r--   0        0        0     2108 2023-06-05 14:29:35.924670 agenta-0.1.7/agenta/cli/main.py
+-rw-r--r--   0        0        0     8450 2023-06-05 14:29:35.924942 agenta-0.1.7/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.7/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.7/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.7/agenta/client/api_models.py
+-rw-r--r--   0        0        0     4355 2023-06-05 14:29:35.925335 agenta-0.1.7/agenta/client/client.py
+-rw-r--r--   0        0        0      641 2023-06-05 14:29:35.925644 agenta-0.1.7/agenta/config.py
+-rw-r--r--   0        0        0      131 2023-06-05 14:29:35.926009 agenta-0.1.7/agenta/config.toml
+-rw-r--r--   0        0        0      372 2023-06-07 09:28:19.623624 agenta-0.1.7/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.7/agenta/docker/docker-assets/README.md
+-rwxr-xr-x   0        0        0       43 2023-06-07 09:27:57.848261 agenta-0.1.7/agenta/docker/docker-assets/entrypoint.sh
+-rw-r--r--   0        0        0      239 2023-06-07 09:45:05.306275 agenta-0.1.7/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2804 2023-06-07 09:47:39.138898 agenta-0.1.7/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0       43 2023-06-07 08:37:18.934913 agenta-0.1.7/agenta/templates/simple_prompt/.env.example
+-rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.7/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.7/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.7/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.7/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      570 2023-06-07 11:00:17.459057 agenta-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 agenta-0.1.7/PKG-INFO
```

### Comparing `agenta-0.1.6/agenta/agenta.py` & `agenta-0.1.7/agenta/agenta.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/agenta/cli/helper.py` & `agenta-0.1.7/agenta/cli/helper.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/agenta/cli/main.py` & `agenta-0.1.7/agenta/cli/main.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/agenta/cli/variant_commands.py` & `agenta-0.1.7/agenta/cli/variant_commands.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/agenta/client/client.py` & `agenta-0.1.7/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/agenta/config.py` & `agenta-0.1.7/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/agenta/docker/docker_utils.py` & `agenta-0.1.7/agenta/docker/docker_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     with TemporaryDirectory() as temp_dir:
         # Create a Dockerfile for the app
         # TODO: Later do this in the temp dir
         dockerfile_path = create_dockerfile(folder)
         shutil.copy(Path(__file__).parent.parent / "agenta.py", folder)
         shutil.copy(Path(__file__).parent /
                     "docker-assets" / "main.py", folder)
+        shutil.copy(Path(__file__).parent /
+                    "docker-assets" / "entrypoint.sh", folder)
 
         # Copy the app files to a temporary directory
         shutil.copytree(folder, temp_dir, dirs_exist_ok=True)
 
         # Build the Docker image
         registry = settings.registry
         tag = f"{registry}/{app_name.lower()}_{variant_name.lower()}:latest"
@@ -60,15 +62,15 @@
             image, build_log = client.images.build(
                 path=temp_dir,
                 tag=tag,
                 rm=True  # Remove intermediate containers after a successful build
             )
 
         except docker.errors.BuildError as ex:
-            logger.error("Error building Docker image:\n" + ex)
+            logger.error("Error building Docker image:\n")
             # Print the build log
             for line in ex.build_log:
                 logger.error(line)
             raise ex
         # Upload the Docker image to the Agenta registry
         print("Uploading Docker image...")
         client.images.push(repository=f"{registry}", tag="latest")
```

### Comparing `agenta-0.1.6/agenta/templates/simple_prompt/app.py` & `agenta-0.1.7/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.6/pyproject.toml` & `agenta-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agenta"
-version = "0.1.6"
+version = "0.1.7"
 description = "Code for the SDK and CLI for the Agenta Lab platform"
 authors = ["Mahmoud Mabrouk <mahmoudmabrouk.mail@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.1"
```

### Comparing `agenta-0.1.6/PKG-INFO` & `agenta-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.6
+Version: 0.1.7
 Summary: Code for the SDK and CLI for the Agenta Lab platform
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

