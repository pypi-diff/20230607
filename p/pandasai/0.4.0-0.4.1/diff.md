# Comparing `tmp/pandasai-0.4.0.tar.gz` & `tmp/pandasai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.4.0.tar", max compression
+gzip compressed data, was "pandasai-0.4.1.tar", max compression
```

## Comparing `pandasai-0.4.0.tar` & `pandasai-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1055 2023-06-06 00:41:09.700228 pandasai-0.4.0/LICENSE
--rw-r--r--   0        0        0     8904 2023-06-06 00:41:09.700228 pandasai-0.4.0/README.md
--rw-r--r--   0        0        0    17831 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/__init__.py
--rw-r--r--   0        0        0     1678 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/constants.py
--rw-r--r--   0        0        0     1494 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3774 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5347 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1466 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1487 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3103 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4325 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10698 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1838 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1481 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2869 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      734 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1786 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1333 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1603 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      505 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1414 2023-06-06 00:41:09.708228 pandasai-0.4.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1457 2023-06-06 00:41:09.708228 pandasai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9811 1970-01-01 00:00:00.000000 pandasai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-06 22:10:54.840191 pandasai-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8904 2023-06-06 22:10:54.840191 pandasai-0.4.1/README.md
+-rw-r--r--   0        0        0    18471 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1678 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1494 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3774 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5347 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1827 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1487 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3040 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4325 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10698 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1838 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1481 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2869 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1786 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1333 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1603 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      505 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1414 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1456 2023-06-06 22:10:54.848191 pandasai-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9804 1970-01-01 00:00:00.000000 pandasai-0.4.1/PKG-INFO
```

### Comparing `pandasai-0.4.0/LICENSE` & `pandasai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/README.md` & `pandasai-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/__init__.py` & `pandasai-0.4.1/pandasai/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
     ```
 """
 import ast
 import io
 import re
 import sys
+import uuid
 from contextlib import redirect_stdout
 from typing import Optional, Union
 
 import astor
 import matplotlib.pyplot as plt
 import pandas as pd
 
@@ -88,14 +89,15 @@
         _max_retries (int, optional): max no. of tries to generate code on failure. Default to 3
         _is_notebook (bool, optional): Whether to run code in notebook. Default to False
         _original_instructions (dict, optional): The dict of instruction to run. Default to None
         last_code_generated (str, optional): Pass last Code if generated. Default to None
         last_run_code (str, optional): Pass the last execution / run. Default to None
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
+        prompt_id (str, optional): Unique ID to differentiate calls. Default to None
 
 
     Returns (str): Response to a Question related to Data
 
     """
 
     _llm: LLM
@@ -109,14 +111,15 @@
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
     }
     _cache: Cache = Cache()
     _enable_cache: bool = True
+    _prompt_id: Optional[str] = None
     last_code_generated: Optional[str] = None
     last_run_code: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
@@ -145,14 +148,15 @@
             )
         self._llm = llm
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
         self._enable_cache = enable_cache
+        self._process_id = str(uuid.uuid4())
 
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
     def conversational_answer(self, question: str, answer: str) -> str:
         """
         Returns the answer in conversational form about the resultant data.
@@ -198,14 +202,17 @@
 
         Returns (str): Answer to the Input Questions about the DataFrame
 
         """
 
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
+        self._prompt_id = str(uuid.uuid4())
+        self.log(f"Prompt ID: {self._prompt_id}")
+
         try:
             if self._enable_cache and self._cache.get(prompt):
                 self.log("Using cached response")
                 code = self._cache.get(prompt)
             else:
                 rows_to_display = 0 if self._enforce_privacy else 5
 
@@ -417,15 +424,15 @@
 
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
 
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
-            code = add_save_chart(code)
+            code = add_save_chart(code, self._prompt_id)
 
         # Get the code to run removing unsafe imports and df overwrites
         code_to_run = self._clean_code(code)
         self.last_run_code = code_to_run
         self.log(
             f"""
 Code running:
@@ -509,7 +516,17 @@
         except Exception:  # pylint: disable=W0718
             return captured_output
 
     def log(self, message: str):
         """Log a message"""
         if self._verbose:
             print(message)
+
+    def process_id(self) -> str:
+        """Return the id of this PandasAI object."""
+        return self._process_id
+
+    def last_prompt_id(self) -> str:
+        """Return the id of the last prompt that was run."""
+        if self._prompt_id is None:
+            raise ValueError("Pandas AI has not been run yet.")
+        return self._prompt_id
```

### Comparing `pandasai-0.4.0/pandasai/constants.py` & `pandasai-0.4.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/exceptions.py` & `pandasai-0.4.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/helpers/_optional.py` & `pandasai-0.4.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/helpers/anonymizer.py` & `pandasai-0.4.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/helpers/cache.py` & `pandasai-0.4.1/pandasai/helpers/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """Cache module for caching queries."""
-
+import glob
 import os
 import shelve
+from os.path import dirname
 
 
 class Cache:
     """Cache class for caching queries. It is used to cache queries to avoid save time and money.
 
     Args:
         filename (str): filename to store the cache.
     """
 
     def __init__(self, filename="cache"):
-        self.filename = filename
-        self.cache = shelve.open(filename)
+        # define cache directory and create directory if it does not exist
+        project_root = dirname(dirname(dirname(__file__)))
+        cache_dir = os.path.join(project_root, "cache")
+        if not os.path.exists(cache_dir):
+            os.makedirs(cache_dir)
+
+        self.filepath = os.path.join(cache_dir, filename)
+        self.cache = shelve.open(self.filepath)
 
     def set(self, key: str, value: str) -> None:
         """Set a key value pair in the cache.
 
         Args:
             key (str): key to store the value.
             value (str): value to store in the cache.
@@ -55,10 +62,10 @@
     def clear(self) -> None:
         """Clean the cache."""
 
         self.cache.clear()
 
     def destroy(self) -> None:
         """Destroy the cache."""
-
-        if os.path.exists(self.filename + ".db"):
-            os.remove(self.filename + ".db")
+        self.cache.close()
+        for cache_file in glob.glob(self.filepath + ".*"):
+            os.remove(cache_file)
```

### Comparing `pandasai-0.4.0/pandasai/helpers/from_excel.py` & `pandasai-0.4.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/helpers/notebook.py` & `pandasai-0.4.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/helpers/save_chart.py` & `pandasai-0.4.1/pandasai/helpers/save_chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Helper functions to save charts to a file, if plt.show() is called."""
 import ast
 import os
-from datetime import datetime
 from itertools import zip_longest
 from os.path import dirname
 from typing import Union
 
 import astor
 
 
@@ -45,51 +44,52 @@
         return all(
             compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
         )
 
     return node1 == node2
 
 
-def add_save_chart(code: str) -> str:
+def add_save_chart(code: str, folder_name: str) -> str:
     """
     Add line to code that save charts to a file, if plt.show() is called.
 
     Args:
         code (str): Code to add line to.
+        folder_name (str): Name of folder to save charts to.
 
     Returns:
         str: Code with line added.
 
     """
-    date = datetime.now().strftime("%Y-%m-%d")
-    timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
+
+    # define chart save directory
+    project_root = dirname(dirname(dirname(__file__)))
+    chart_save_dir = os.path.join(project_root, "exports", "charts", folder_name)
+
     tree = ast.parse(code)
 
     # count number of plt.show() calls
     show_count = sum(
         compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
         for node in ast.walk(tree)
     )
 
     # if there are no plt.show() calls, return the original code
     if show_count == 0:
         return code
 
-    # define chart save directory
-    project_root = dirname(dirname(dirname(__file__)))
-    chart_save_dir = os.path.join(project_root, "exports", "charts", date)
     if not os.path.exists(chart_save_dir):
         os.makedirs(chart_save_dir)
 
     # iterate through the AST and add plt.savefig() calls before plt.show() calls
     counter = ord("a")
     new_body = []
     for node in tree.body:
         if compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True):
-            filename = f"chart_{timestamp}"
+            filename = "chart"
             if show_count > 1:
                 filename += f"_{chr(counter)}"
                 counter += 1
 
             chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
             new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
         new_body.append(node)
```

### Comparing `pandasai-0.4.0/pandasai/llm/azure_openai.py` & `pandasai-0.4.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/llm/base.py` & `pandasai-0.4.1/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/llm/fake.py` & `pandasai-0.4.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/llm/google_palm.py` & `pandasai-0.4.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/llm/open_assistant.py` & `pandasai-0.4.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/llm/openai.py` & `pandasai-0.4.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/llm/starcoder.py` & `pandasai-0.4.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/prompts/base.py` & `pandasai-0.4.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.4.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.4.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/prompts/generate_python_code.py` & `pandasai-0.4.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.4.1/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.0/pyproject.toml` & `pandasai-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.4.0"
+version = "0.4.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
-pandas = "^2.0.1"
+pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
```

### Comparing `pandasai-0.4.0/PKG-INFO` & `pandasai-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pandas (==1.5.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
```

