# Comparing `tmp/braintrust-0.0.2.tar.gz` & `tmp/braintrust-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.2.tar", last modified: Wed May 24 03:34:59 2023, max compression
+gzip compressed data, was "braintrust-0.0.3.tar", last modified: Wed Jun  7 15:57:32 2023, max compression
```

## Comparing `braintrust-0.0.2.tar` & `braintrust-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.807954 braintrust-0.0.2/
--rw-r--r--   0 ankur      (501) staff       (20)      494 2023-05-24 03:34:59.807785 braintrust-0.0.2/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.2/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-05-24 03:34:59.808003 braintrust-0.0.2/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1592 2023-05-24 03:21:54.000000 braintrust-0.0.2/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.804862 braintrust-0.0.2/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.806839 braintrust-0.0.2/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    10847 2023-05-21 16:20:09.000000 braintrust-0.0.2/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.2/src/braintrust/cache.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.2/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-05-24 03:34:51.000000 braintrust-0.0.2/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-05-24 03:34:59.807577 braintrust-0.0.2/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      494 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      347 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      196 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-05-24 03:34:59.000000 braintrust-0.0.2/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.813499 braintrust-0.0.3/
+-rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-07 15:57:32.813379 braintrust-0.0.3/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.3/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-07 15:57:32.813537 braintrust-0.0.3/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1582 2023-06-06 15:10:19.000000 braintrust-0.0.3/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.811734 braintrust-0.0.3/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.812438 braintrust-0.0.3/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    12709 2023-06-06 15:10:19.000000 braintrust-0.0.3/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.3/src/braintrust/cache.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.3/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-07 15:56:14.000000 braintrust-0.0.3/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-07 15:57:32.813205 braintrust-0.0.3/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      347 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      251 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-07 15:57:32.000000 braintrust-0.0.3/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.2/setup.py` & `braintrust-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         "flake8-isort",
         "IPython",
         "isort==5.10.1",
         "pre-commit",
         "pytest",
         "twine",
     ],
+    "doc": ["pydoc-markdown[novella]"],
 }
 
 extras_require["all"] = sorted({package for packages in extras_require.values() for package in packages})
 
 setuptools.setup(
     name="braintrust",
     version=version_contents["VERSION"],
@@ -40,15 +41,14 @@
     long_description_content_type="text/markdown",
     url="https://www.braintrustdata.com",
     # project_urls={
     #    "Bug Tracker": "https://github.com/TODO/issues",
     # },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7.0",
     entry_points={"console_scripts": ["braintrust = braintrust.cli.__main__:main"]},
     install_requires=install_requires,
```

### Comparing `braintrust-0.0.2/src/braintrust/__init__.py` & `braintrust-0.0.3/src/braintrust/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+"""
+A Python library for logging data to BrainTrust.
+
+### Quickstart
+
+Install the library with pip.
+
+```bash
+pip install braintrust
+```
+
+Then, run a simple experiment with the following code:
+
+```python
+import braintrust
+
+experiment = braintrust.init(project="PyTest")
+experiment.log(
+    inputs={"test": 1},
+    output="foo",
+    expected="bar",
+    scores={
+        "n": 0.5,
+    },
+    metadata={
+        "id": 1,
+    },
+)
+print(experiment.summarize())
+```
+
+### API Reference
+"""
 import atexit
 import datetime
 import json
 import logging
 import os
 import queue
 import threading
@@ -11,36 +44,30 @@
 from functools import cache as _cache
 from getpass import getpass
 from typing import Any
 
 import git
 import openai
 import requests
-import urllib3
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .cache import API_INFO_PATH, CACHE_PATH
 from .oai import run_cached_request
 
 
-# XXX Refactor this to use some kind of documentable dataclass
 class BrainTrustState:
     def __init__(self):
         self.current_project = None
         self.current_experiment = None
 
 
 _state = BrainTrustState()
 
 
-def urljoin(*parts):
-    return "/".join([x.lstrip("/") for x in parts])
-
-
 API_URL = None
 ORG_ID = None
 LOG_URL = None
 
 
 class HTTPConnection:
     def __init__(self, base_url=API_URL):
@@ -54,18 +81,18 @@
         self.session.mount("https://", adapter)
 
     def set_token(self, token):
         token = token.rstrip("\n")
         self.session.headers.update({"Authorization": f"Bearer {token}"})
 
     def get(self, path, *args, **kwargs):
-        return self.session.get(urljoin(self.base_url, path), *args, **kwargs)
+        return self.session.get(_urljoin(self.base_url, path), *args, **kwargs)
 
     def post(self, path, *args, **kwargs):
-        return self.session.post(urljoin(self.base_url, path), *args, **kwargs)
+        return self.session.post(_urljoin(self.base_url, path), *args, **kwargs)
 
 
 @_cache
 def api_conn():
     return HTTPConnection(LOG_URL)  # TODO: Fix to use global install
 
 
@@ -304,22 +331,69 @@
         self.logger.log(args)
         return args["id"]
 
     def summarize(self):
         # TODO: Show results so far here as well
         org_name = _user_info()["organizations"][0]["name"]
 
-        project_url = f"{API_URL}/app/{urllib.parse.quote(org_name)}/{urllib.parse.quote(self.project.name)}"
+        project_url = f"{API_URL}/app/{urllib.parse.quote(org_name)}/p/{urllib.parse.quote(self.project.name)}"
         experiment_url = f"{project_url}/{urllib.parse.quote(self.name)}"
 
         print(f"See results for all experiments in {self.project.name} at {project_url}")
         print(f"See results for {self.name} at {experiment_url}")
 
 
+def init(project, experiment=None, description=None, api_url=None):
+    """
+    Initialize a new experiment in a specified project. If the project does not exist, it will be created.
+
+    :param project: The name of the project to create the experiment in.
+    :param experiment: The name of the experiment to create. If not specified, a name will be generated automatically.
+    :param description: An optional description of the experiment.
+    :param api_url: The URL of the BrainTrust API to use. If not specified, the default will be used.
+    :returns: The experiment object.
+    """
+    kwargs = {}
+    if api_url:
+        kwargs["api_url"] = api_url
+    login(**kwargs)
+
+    _state.current_project = Project(project)
+    _state.current_experiment = Experiment(_state.current_project, name=experiment, description=description)
+    return _state.current_experiment
+
+
+def log(inputs, output, expected, scores, metadata=None):
+    """
+    Log a single event to the current experiment. The event will be batched and uploaded behind the scenes.
+
+    :param inputs: The inputs to the model (an arbitrary, JSON serializable object).
+    :param output: The output of the model (an arbitrary, JSON serializable object).
+    :param expected: The expected output of the model (an arbitrary, JSON serializable object).
+    :param scores: A dictionary of scores to log.
+    :param metadata: (Optional) Additional metadata about the event (that you can later use to slice/dice your results).
+    :returns: The `id` of the logged event.
+    """
+
+    if not _state.current_experiment:
+        raise Exception("Not initialized. Please call init() or login() first")
+
+    return _state.current_experiment.log(
+        inputs=inputs, output=output, expected=expected, scores=scores, metadata=metadata
+    )
+
+
 def login(api_url=os.environ.get("BRAINTRUST_API_URL", "https://www.braintrustdata.com")):
+    """
+    Login to BrainTrust. This will prompt you for your API token, which you can find at
+    https://www.braintrustdata.com/app/token. This method is called automatically by `init()`.
+
+    :param api_url: The URL of the BrainTrust API. Defaults to https://www.braintrustdata.com.
+    """
+
     global API_URL, ORG_ID, LOG_URL
 
     API_URL = api_url
 
     os.makedirs(CACHE_PATH, exist_ok=True)
 
     api_info = None
@@ -339,15 +413,15 @@
         ping_resp = conn.get("ping")
         ping_ok = ping_resp.ok
 
     if not ping_ok:
         print(f"Please copy your API token from {API_URL}/app/token")
         temp_token = getpass("Token: ")
 
-        resp = requests.post(urljoin(API_URL, "/api/id-token"), json={"token": temp_token})
+        resp = requests.post(_urljoin(API_URL, "/api/id-token"), json={"token": temp_token})
         assert resp.ok, f"Failed to acquire token: {resp.text}"
         info = resp.json()
         token, ORG_ID, LOG_URL = info["token"], info["org_info"][0]["id"], info["org_info"][0]["api_url"]
 
         with open(API_INFO_PATH, "w") as f:
             json.dump({"token": token, "org_id": ORG_ID, "log_url": LOG_URL}, f)
 
@@ -355,27 +429,12 @@
         conn.set_token(token)
 
     assert conn, "Conn should be set at this point (a bug)"
     resp = conn.get("ping")
     assert resp.ok, "Invalid token: " + resp.text
 
 
-def init(project, api_url=None, experiment=None, description=None):
-    kwargs = {}
-    if api_url:
-        kwargs["api_url"] = api_url
-    login(**kwargs)
-
-    _state.current_project = Project(project)
-    _state.current_experiment = Experiment(_state.current_project, name=experiment, description=description)
-    return _state.current_experiment
-
-
-def log(inputs, output, expected=None, scores=None, metadata=None):
-    # XXX Fix with proper exception
-    assert _state.current_experiment, "not initialized"
-    return _state.current_experiment.log(
-        inputs=inputs, output=output, expected=expected, scores=scores, metadata=metadata
-    )
+def _urljoin(*parts):
+    return "/".join([x.lstrip("/") for x in parts])
 
 
-__all__ = ["init", "log"]
+__all__ = ["init", "log", "login"]
```

### Comparing `braintrust-0.0.2/src/braintrust/oai.py` & `braintrust-0.0.3/src/braintrust/oai.py`

 * *Files identical despite different names*

