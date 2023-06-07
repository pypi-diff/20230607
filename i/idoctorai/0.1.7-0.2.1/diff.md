# Comparing `tmp/idoctorai-0.1.7.tar.gz` & `tmp/idoctorai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.1.7.tar", max compression
+gzip compressed data, was "idoctorai-0.2.1.tar", max compression
```

## Comparing `idoctorai-0.1.7.tar` & `idoctorai-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.1.7/LICENSE
--rw-r--r--   0        0        0    16574 2023-06-05 11:32:52.312900 idoctorai-0.1.7/pandasai/__init__.py
--rw-r--r--   0        0        0     1200 2023-06-05 10:38:51.205810 idoctorai-0.1.7/pandasai/constants.py
--rw-r--r--   0        0        0     1001 2023-06-05 10:38:51.206807 idoctorai-0.1.7/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.1.7/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.1.7/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0      593 2023-06-05 10:38:51.207805 idoctorai-0.1.7/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.1.7/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     2723 2023-06-05 10:38:51.207805 idoctorai-0.1.7/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.1.7/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.1.7/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11269 2023-06-05 11:26:38.666244 idoctorai-0.1.7/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.1.7/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.1.7/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.1.7/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.1.7/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.1.7/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.1.7/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.1.7/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.1.7/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.1.7/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.1.7/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.1.7/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1455 2023-06-05 10:38:51.207805 idoctorai-0.1.7/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1093 2023-06-05 12:53:10.833279 idoctorai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       33 2023-06-05 10:50:23.961401 idoctorai-0.1.7/README.md
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 idoctorai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.2.1/LICENSE
+-rw-r--r--   0        0        0    19001 2023-06-07 12:41:32.619799 idoctorai-0.2.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.2.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.2.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.2.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.2.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.2.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.2.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.2.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.2.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.2.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.2.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.2.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11096 2023-06-07 12:25:21.036958 idoctorai-0.2.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.2.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.2.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.2.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2973 2023-05-31 07:10:59.367662 idoctorai-0.2.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.2.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.2.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.2.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.2.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.2.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.2.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.2.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1511 2023-06-07 12:41:32.620825 idoctorai-0.2.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1396 2023-06-07 12:41:32.621795 idoctorai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-06-07 12:41:32.591875 idoctorai-0.2.1/README.md
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 idoctorai-0.2.1/PKG-INFO
```

### Comparing `idoctorai-0.1.7/LICENSE` & `idoctorai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/__init__.py` & `idoctorai-0.2.1/pandasai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-""" PandasAI is a wrapper around a LLM to make dataframes conversational
+"""
+PandasAI is a wrapper around a LLM to make dataframes conversational
 
 This module includes the implementation of basis  PandasAI class with methods to run the LLMs
 models on Pandas dataframes. Following LLMs are implemented so far.
 
 Example:
 
     This module is the Entry point of the `pandasai` package. Following is an example of how to
@@ -22,131 +23,147 @@
         "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
     })
 
     # Instantiate a LLM
     from pandasai.llm.openai import OpenAI
     llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-    pandas_ai = PandasAI(llm, conversational=False)
+    pandas_ai = PandasAI(llm)
     pandas_ai(df, prompt='Which are the 5 happiest countries?')
 
     ```
 """
 import ast
 import io
 import re
+import sys
+import uuid
 from contextlib import redirect_stdout
-from typing import Optional
+from typing import Optional, Union
 
 import astor
 import matplotlib.pyplot as plt
 import pandas as pd
 
-from .constants import WHITELISTED_BUILTINS, WHITELISTED_LIBRARIES
-from .exceptions import LLMNotFoundError
+from .constants import (
+    ENVIRONMENT_DEFAULTS,
+    WHITELISTED_BUILTINS,
+    WHITELISTED_LIBRARIES,
+    WHITELISTED_OPTIONAL_LIBRARIES,
+)
+from .exceptions import BadImportError, LLMNotFoundError
+from .helpers._optional import import_optional_dependency
 from .helpers.anonymizer import anonymize_dataframe_head
+from .helpers.cache import Cache
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
 from .llm.base import LLM
 from .prompts.correct_error_prompt import CorrectErrorPrompt
+from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
-from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
+
 
 # pylint: disable=too-many-instance-attributes disable=too-many-arguments
 class PandasAI:
-    """PandasAI is a wrapper around a LLM to make dataframes conversational.
+    """
+    PandasAI is a wrapper around a LLM to make dataframes conversational.
 
 
-    This is a an entry point of `pandasai` object. This class consists of methods to interface the
-    LLMs with Pandas     dataframes. A pandas dataframe metadata i.e df.head() and prompt is
+    This is an entry point of `pandasai` object. This class consists of methods to interface the
+    LLMs with Pandas     dataframes. A pandas dataframe metadata i.e. df.head() and prompt is
     passed on to chosen LLMs API end point to     generate a Python code to answer the questions
     asked. The resultant python code is run on actual data and answer is converted into a
     conversational form.
 
     Note:
         Do not include the `self` parameter in the ``Args`` section.
     Args:
         _llm (obj): LLMs option to be used for API access
-        _verbose (bool, optional): To show the intermediate outputs e.g python code
+        _verbose (bool, optional): To show the intermediate outputs e.g. python code
         generated and execution step on the prompt. Default to False
         _is_conversational_answer (bool, optional): Whether to return answer in conversational
         form. Default to False
         _enforce_privacy (bool, optional): Do not display the data on prompt in case of
         Sensitive data. Default to False
         _max_retries (int, optional): max no. of tries to generate code on failure. Default to 3
         _is_notebook (bool, optional): Whether to run code in notebook. Default to False
         _original_instructions (dict, optional): The dict of instruction to run. Default to None
         last_code_generated (str, optional): Pass last Code if generated. Default to None
         last_run_code (str, optional): Pass the last execution / run. Default to None
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
+        prompt_id (str, optional): Unique ID to differentiate calls. Default to None
 
 
-    Returns:
-        response (str): Returns the Response to a Question related to Data
+    Returns (str): Response to a Question related to Data
 
     """
 
     _llm: LLM
     _verbose: bool = False
-    _is_conversational_answer: bool = True
+    _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
-    _max_retries: int = 1
+    _max_retries: int = 3
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
     }
+    _cache: Cache = Cache()
+    _enable_cache: bool = True
+    _prompt_id: Optional[str] = None
     last_code_generated: Optional[str] = None
     last_run_code: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
-
-
     def __init__(
         self,
         llm=None,
-        conversational=True,
+        conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
+        enable_cache=True,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
-            conversational (bool): Whether to return answer in conversational form. Default to True
-            verbose (bool): To show the intermediate outputs e.g python code generated and
+            conversational (bool): Whether to return answer in conversational form. Default to False
+            verbose (bool): To show the intermediate outputs e.g. python code generated and
              execution step on the prompt.  Default to False
             enforce_privacy (bool): Execute the codes with Privacy Mode ON.  Default to False
+            save_charts (bool): Save the charts generated in the notebook. Default to False
         """
         if llm is None:
             raise LLMNotFoundError(
                 "An LLM should be provided to instantiate a PandasAI instance"
             )
         self._llm = llm
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
+        self._enable_cache = enable_cache
+        self._process_id = str(uuid.uuid4())
 
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
     def conversational_answer(self, question: str, answer: str) -> str:
-
-        """Returns the answer in conversational form about the resultant data.
+        """
+        Returns the answer in conversational form about the resultant data.
 
         Args:
             question (str): A question in Conversational form
             answer (str): A summary / resultant Data
 
         Returns (str): Response
 
@@ -164,92 +181,102 @@
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
-    ) -> str:
+    ) -> Union[str, pd.DataFrame]:
         """
         Run the PandasAI to make Dataframes Conversational.
 
         Args:
             data_frame (pd.Dataframe): A pandas Dataframe
             prompt (str): A prompt to query about the Dataframe
             is_conversational_answer (bool): Whether to return answer in conversational form.
             Default to False
             show_code (bool): To show the intermediate python code generated on the prompt.
             Default to False
             anonymize_df (bool): Running the code with Sensitive Data. Default to True
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
-        Returns: Answer to the Input Questions about the DataFrame
+        Returns (str): Answer to the Input Questions about the DataFrame
 
         """
 
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
-        try:
-            rows_to_display = 0 if self._enforce_privacy else 5
+        self._prompt_id = str(uuid.uuid4())
+        self.log(f"Prompt ID: {self._prompt_id}")
 
-            multiple: bool = isinstance(data_frame, list)
+        try:
+            if self._enable_cache and self._cache.get(prompt):
+                self.log("Using cached response")
+                code = self._cache.get(prompt)
+            else:
+                rows_to_display = 0 if self._enforce_privacy else 5
 
-            if multiple:
+                multiple: bool = isinstance(data_frame, list)
 
-                heads = [anonymize_dataframe_head(dataframe)
+                if multiple:
+                    heads = [
+                        anonymize_dataframe_head(dataframe)
                         if anonymize_df
                         else dataframe.head(rows_to_display)
-                        for dataframe in data_frame]
-
-                code = self._llm.generate_code(
-                    MultipleDataframesPrompt(dataframes=heads),
-                    prompt,
-                )
+                        for dataframe in data_frame
+                    ]
 
-                self._original_instructions = {
-                    "question": prompt,
-                    "df_head": heads,
-                    "rows_to_display": rows_to_display,
-                }
+                    code = self._llm.generate_code(
+                        MultipleDataframesPrompt(dataframes=heads),
+                        prompt,
+                    )
 
-            else:
+                    self._original_instructions = {
+                        "question": prompt,
+                        "df_head": heads,
+                        "rows_to_display": rows_to_display,
+                    }
+
+                else:
+                    df_head = data_frame.head(rows_to_display)
+                    if anonymize_df:
+                        df_head = anonymize_dataframe_head(df_head)
+
+                    code = self._llm.generate_code(
+                        GeneratePythonCodePrompt(
+                            prompt=prompt,
+                            df_head=df_head,
+                            num_rows=data_frame.shape[0],
+                            num_columns=data_frame.shape[1],
+                            rows_to_display=rows_to_display,
+                        ),
+                        prompt,
+                    )
 
-                df_head = data_frame.head(rows_to_display)
-                if anonymize_df:
-                    df_head = anonymize_dataframe_head(df_head)
-
-                code = self._llm.generate_code(
-                    GeneratePythonCodePrompt(
-                        prompt=prompt,
-                        df_head=df_head,
-                        num_rows=data_frame.shape[0],
-                        num_columns=data_frame.shape[1],
-                        rows_to_display=rows_to_display,
-                    ),
-                    prompt,
+                    self._original_instructions = {
+                        "question": prompt,
+                        "df_head": df_head,
+                        "num_rows": data_frame.shape[0],
+                        "num_columns": data_frame.shape[1],
+                        "rows_to_display": rows_to_display,
+                    }
+
+                self.last_code_generated = code
+                self.log(
+                    f"""
+                        Code generated:
+                        ```
+                        {code}
+                        ```
+                    """
                 )
 
-                self._original_instructions = {
-                    "question": prompt,
-                    "df_head": df_head,
-                    "num_rows": data_frame.shape[0],
-                    "num_columns": data_frame.shape[1],
-                    "rows_to_display": rows_to_display,
-                }
-
-            self.last_code_generated = code
-            self.log(
-                f"""
-                    Code generated:
-                    ```
-                    {code}
-                    ```
-                """
-            )
+                self._cache.set(prompt, code)
+
             if show_code and self._in_notebook:
                 self.notebook.create_new_cell(code)
 
             answer = self.run_code(
                 code,
                 data_frame,
                 use_error_correction_framework=use_error_correction_framework,
@@ -267,154 +294,171 @@
             self.last_error = str(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
 
+    def clear_cache(self):
+        """
+        Clears the cache of the PandasAI instance.
+        """
+        self._cache.clear()
+
     def __call__(
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
-    ) -> str:
+    ) -> Union[str, pd.DataFrame]:
         """
-        __call__ method of PandasAI class. It call `run` method
+        __call__ method of PandasAI class. It calls the `run` method.
+
         Args:
             data_frame:
             prompt:
             is_conversational_answer:
             show_code:
             anonymize_df:
             use_error_correction_framework:
 
-        Returns:
+        Returns (str): Answer to the Input Questions about the DataFrame.
 
         """
 
         return self.run(
             data_frame,
             prompt,
             is_conversational_answer,
             show_code,
             anonymize_df,
             use_error_correction_framework,
         )
 
-    def is_unsafe_import(self, node: ast.stmt) -> bool:
-
-        """Remove non-whitelisted imports from the code to prevent malicious code execution
+    def _is_unsafe_import(self, node: ast.stmt) -> bool:
+        """
+        Remove non-whitelisted imports from the code to prevent malicious code execution
 
         Args:
             node (object): ast.stmt
 
         Returns (bool): A flag if unsafe_imports found.
 
         """
 
-        return isinstance(node, (ast.Import, ast.ImportFrom)) and any(
-            alias.name not in WHITELISTED_LIBRARIES for alias in node.names
-        )
+        if isinstance(node, (ast.Import, ast.ImportFrom)):
+            for alias in node.names:
+                if (
+                    alias.name in WHITELISTED_BUILTINS
+                    or alias.name in ENVIRONMENT_DEFAULTS
+                ):
+                    return True
+                if alias.name in WHITELISTED_OPTIONAL_LIBRARIES:
+                    import_optional_dependency(alias.name)
+                    continue
+                if alias.name.split(".")[0] not in WHITELISTED_LIBRARIES:
+                    raise BadImportError(alias.name)
 
-    def is_df_overwrite(self, node: ast.stmt) -> str:
+        return False
 
+    def _is_df_overwrite(self, node: ast.stmt) -> bool:
         """
         Remove df declarations from the code to prevent malicious code execution. A helper method.
+
         Args:
             node (object): ast.stmt
 
-        Returns (str):
+        Returns (bool):
 
         """
 
         return (
             isinstance(node, ast.Assign)
             and isinstance(node.targets[0], ast.Name)
             and re.match(r"df\d{0,2}$", node.targets[0].id)
         )
 
-    def clean_code(self, code: str) -> str:
-
+    def _clean_code(self, code: str) -> str:
         """
         A method to clean the code to prevent malicious code execution
+
         Args:
             code(str): A python code
 
         Returns (str): Returns a Clean Code String
 
         """
 
         tree = ast.parse(code)
 
         new_body = [
             node
             for node in tree.body
-            if not (self.is_unsafe_import(node) or self.is_df_overwrite(node))
+            if not (self._is_unsafe_import(node) or self._is_df_overwrite(node))
         ]
 
         new_tree = ast.Module(body=new_body)
         return astor.to_source(new_tree).strip()
 
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
         """
         A method to execute the python code generated by LLMs to answer the question about the
         input dataframe. Run the code in the current context and return the result.
+
         Args:
             code (str): A python code to execute
             data_frame (pd.DataFrame): A full Pandas DataFrame
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
             Default to True
 
-        Returns:
+        Returns (str): String representation of the result of the code execution.
 
         """
 
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
 
         multiple: bool = isinstance(data_frame, list)
 
         # Add save chart code
         if self._save_charts:
-            code = add_save_chart(code)
+            code = add_save_chart(code, self._prompt_id)
 
         # Get the code to run removing unsafe imports and df overwrites
-        print(code)
-        code_to_run = self.clean_code(code)
+        code_to_run = self._clean_code(code)
         self.last_run_code = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
         )
 
         environment: dict = {
-            "pd": pd,
-            "plt": plt,
+            **{
+                alias: sys.modules[library]
+                for library, alias in ENVIRONMENT_DEFAULTS.items()
+            },
             "__builtins__": {
-                **{
-                    builtin: __builtins__[builtin]
-                    for builtin in WHITELISTED_BUILTINS
-                },
+                **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
             },
         }
 
         if multiple:
-            environment.update({
-                f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start = 1)
-            })
+            environment.update(
+                {f"df{i}": dataframe for i, dataframe in enumerate(data_frame, start=1)}
+            )
 
         else:
             environment["df"] = data_frame
 
         # Redirect standard output to a StringIO buffer
         with redirect_stdout(io.StringIO()) as output:
             count = 0
@@ -427,30 +471,34 @@
                 except Exception as e:  # pylint: disable=W0718 disable=C0103
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
 
                     if multiple:
-                        error_correcting_instruction = CorrectMultipleDataframesErrorPrompt(
-                            code=code,
-                            error_returned=e,
-                            question=self._original_instructions["question"],
-                            df_head=self._original_instructions["df_head"],
+                        error_correcting_instruction = (
+                            CorrectMultipleDataframesErrorPrompt(
+                                code=code,
+                                error_returned=e,
+                                question=self._original_instructions["question"],
+                                df_head=self._original_instructions["df_head"],
+                            )
                         )
 
                     else:
                         error_correcting_instruction = CorrectErrorPrompt(
                             code=code,
                             error_returned=e,
                             question=self._original_instructions["question"],
                             df_head=self._original_instructions["df_head"],
                             num_rows=self._original_instructions["num_rows"],
                             num_columns=self._original_instructions["num_columns"],
-                            rows_to_display=self._original_instructions["rows_to_display"],
+                            rows_to_display=self._original_instructions[
+                                "rows_to_display"
+                            ],
                         )
 
                     code_to_run = self._llm.generate_code(
                         error_correcting_instruction, ""
                     )
 
         captured_output = output.getvalue()
@@ -468,7 +516,17 @@
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

### Comparing `idoctorai-0.1.7/pandasai/helpers/anonymizer.py` & `idoctorai-0.2.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/helpers/from_excel.py` & `idoctorai-0.2.1/pandasai/helpers/from_excel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
-""" Helper Module to Handle Data
+"""
+Helper Module to Handle Data
 This module collects the helper function on handling various Data Sources.
 
-
 """
 from __future__ import annotations
 
 import pandas as pd
 
 
 def from_excel(file, sheet: str | int | None = 0) -> pd.DataFrame:
-
     """
     Return a pandas DataFrame from an Excel file.
     Wrapper for pandas.read_excel().
+
     Args:
         file (str):  A file path to be read
         sheet (str | int): Name of the sheet or Sheet No. Default is 0
 
     Returns (pd.DataFrame): A Pandas Dataframe
 
     """
```

### Comparing `idoctorai-0.1.7/pandasai/helpers/notebook.py` & `idoctorai-0.2.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/helpers/save_chart.py` & `idoctorai-0.2.1/pandasai/helpers/save_chart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 """Helper functions to save charts to a file, if plt.show() is called."""
 import ast
 import os
-from datetime import datetime
 from itertools import zip_longest
 from os.path import dirname
 from typing import Union
 
 import astor
 
 
 def compare_ast(
     node1: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
     node2: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
     ignore_args=False,
 ) -> bool:
-    """Compare two AST nodes for equality.
-    Source: https://stackoverflow.com/a/66733795/11080806"""
+    """
+    Compare two AST nodes for equality.
+    Source: https://stackoverflow.com/a/66733795/11080806
+
+    Args:
+        node1 (ast.AST): First AST node to compare.
+        node2 (ast.AST): Second AST node to compare.
+        ignore_args (bool, optional): Whether to ignore the arguments of the nodes.
+            Defaults to False.
+
+    Returns:
+        bool: True if the nodes are equal, False otherwise.
+
+    """
     if type(node1) is not type(node2):
         return False
 
     if isinstance(node1, ast.AST):
         for k, node in vars(node1).items():
             if k in {"lineno", "end_lineno", "col_offset", "end_col_offset", "ctx"}:
                 continue
@@ -33,48 +44,57 @@
         return all(
             compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
         )
 
     return node1 == node2
 
 
-def add_save_chart(code: str) -> str:
-    """Add line to code that save charts to a file, if plt.show() is called."""
-    date = datetime.now().strftime("%Y-%m-%d")
-    timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
+def add_save_chart(code: str, folder_name: str) -> str:
+    """
+    Add line to code that save charts to a file, if plt.show() is called.
+
+    Args:
+        code (str): Code to add line to.
+        folder_name (str): Name of folder to save charts to.
+
+    Returns:
+        str: Code with line added.
+
+    """
 
     # define chart save directory
     project_root = dirname(dirname(dirname(__file__)))
-    chart_save_dir = os.path.join(project_root, f"exports\\charts\\{date}")
-    if not os.path.exists(chart_save_dir):
-        os.makedirs(chart_save_dir)
+    chart_save_dir = os.path.join(project_root, "exports", "charts", folder_name)
 
     tree = ast.parse(code)
 
     # count number of plt.show() calls
     show_count = sum(
         compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
         for node in ast.walk(tree)
     )
 
     # if there are no plt.show() calls, return the original code
     if show_count == 0:
         return code
 
+    if not os.path.exists(chart_save_dir):
+        os.makedirs(chart_save_dir)
+
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
-            new_body.append(
-                ast.parse(f"plt.savefig(r'{chart_save_dir}\\{filename}.png')")
-            )
+
+            chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
+            new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
         new_body.append(node)
 
     new_body.append(ast.parse(f"print(r'Charts saved to: {chart_save_dir}')"))
 
     new_tree = ast.Module(body=new_body)
     return astor.to_source(new_tree).strip()
```

### Comparing `idoctorai-0.1.7/pandasai/llm/azure_openai.py` & `idoctorai-0.2.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/llm/base.py` & `idoctorai-0.2.1/pandasai/llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
+from ..helpers._optional import import_optional_dependency
 from ..prompts.base import Prompt
 
 
 class LLM:
     """Base class to implement a new LLM."""
 
     last_prompt: Optional[str] = None
@@ -148,15 +149,14 @@
     max_tokens: int = 512
     top_p: float = 1
     frequency_penalty: float = 0
     presence_penalty: float = 0.6
     stop: Optional[str] = None
 
     def _set_params(self, **kwargs):
-
         """
         Set Parameters
         Args:
             **kwargs: ["model", "engine", "deployment_id", "temperature","max_tokens",
             "top_p", "frequency_penalty", "presence_penalty", "stop", ]
 
         Returns: None
@@ -176,15 +176,14 @@
         ]
         for key, value in kwargs.items():
             if key in valid_params:
                 setattr(self, key, value)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
-
         """
         Get the default parameters for calling OpenAI API
 
         Returns (Dict): A dict of OpenAi API parameters
 
         """
 
@@ -234,16 +233,14 @@
                 }
             ],
         }
 
         if self.stop is not None:
             params["stop"] = [self.stop]
 
-        print(value)
-
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
 
 
 class HuggingFaceLLM(LLM):
     """Base class to implement a new Hugging Face LLM.
@@ -276,15 +273,14 @@
         response = requests.post(
             self._api_url, headers=headers, json=payload, timeout=60
         )
 
         return response.json()[0]["generated_text"]
 
     def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
-
         """
         A call method of HuggingFaceLLM class.
         Args:
             instruction (object): A prompt object
             value (str):
             suffix (str):
 
@@ -307,15 +303,15 @@
         output = response.replace(prompt + value + suffix, "")
         return output
 
 
 class BaseGoogle(LLM):
     """Base class to implement a new Google LLM
 
-     LLM base class is extended to be used with Google Palm API.
+    LLM base class is extended to be used with Google Palm API.
     """
 
     genai: Any
     temperature: Optional[float] = 0
     top_p: Optional[float] = None
     top_k: Optional[float] = None
     max_output_tokens: Optional[int] = None
@@ -328,24 +324,19 @@
 
         Returns:
 
         """
 
         if not api_key:
             raise APIKeyNotFoundError("Google Palm API key is required")
-        try:
-            # pylint: disable=import-outside-toplevel
-            import google.generativeai as genai
 
-            genai.configure(api_key=api_key)
-        except ImportError as ex:
-            raise ImportError(
-                "Could not import google-generativeai python package. "
-                "Please install it with `pip install google-generativeai`."
-            ) from ex
+        err_msg = "Install google-generativeai >= 0.1 for Google Palm API"
+        genai = import_optional_dependency("google.generativeai", extra=err_msg)
+
+        genai.configure(api_key=api_key)
         self.genai = genai
 
     def _valid_params(self):
         return ["temperature", "top_p", "top_k", "max_output_tokens"]
 
     def _set_params(self, **kwargs):
         """
```

### Comparing `idoctorai-0.1.7/pandasai/llm/fake.py` & `idoctorai-0.2.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/llm/google_palm.py` & `idoctorai-0.2.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/llm/open_assistant.py` & `idoctorai-0.2.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/llm/openai.py` & `idoctorai-0.2.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/llm/starcoder.py` & `idoctorai-0.2.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/prompts/base.py` & `idoctorai-0.2.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.2.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.2.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/prompts/generate_python_code.py` & `idoctorai-0.2.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/prompts/generate_response.py` & `idoctorai-0.2.1/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.1.7/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.2.1/pandasai/prompts/multiple_dataframes.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, dataframes: list[pd.DataFrame]): # pylint: disable=super-init-not-called
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
+            data_text = dataframe.head().to_string()
+
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the result of `print(df{i}.head())`:
-{dataframe}"""
+{data_text}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
         )
```

### Comparing `idoctorai-0.1.7/pyproject.toml` & `idoctorai-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.1.7"
+version = "0.2.1"
 description = "this is idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
+
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
 
 
@@ -27,14 +28,21 @@
 pytest-mock = "^3.10.0"
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 
 [tool.poetry.extras]
 google = ["google-generativeai"]
 
+[tool.poetry.group.whitelist.dependencies]
+statsmodels = {version = "^0.14.0", optional = true}
+scikit-learn = {version = "^1.2.2", optional = true}
+seaborn = {version = "^0.12.2", optional = true}
+plotly = {version = "^5.14.1", optional = true}
+ggplot = {version = "^0.11.5", optional = true}
+
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.0"
 mkdocstrings-python = "0.7.1"
 markdown-include = "^0.6.0"
 
 [tool.poetry.scripts]
 pai = "pai.__main__:main"
```

### Comparing `idoctorai-0.1.7/PKG-INFO` & `idoctorai-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.1.7
+Version: 0.2.1
 Summary: this is idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,14 +12,14 @@
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
 
 ## idoctorai
 
 this is idoctorai
```

