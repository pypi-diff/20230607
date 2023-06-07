# Comparing `tmp/codezen-0.1.1.tar.gz` & `tmp/codezen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codezen-0.1.1.tar", max compression
+gzip compressed data, was "codezen-0.2.0.tar", max compression
```

## Comparing `codezen-0.1.1.tar` & `codezen-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.1.1/LICENSE
--rw-r--r--   0        0        0     1991 2023-05-23 15:08:53.787807 codezen-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.1.1/codezen/__init__.py
--rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.1.1/codezen/__main__.py
--rw-r--r--   0        0        0     4080 2023-05-23 13:21:39.848044 codezen-0.1.1/codezen/app.py
--rw-r--r--   0        0        0      498 2023-05-23 16:01:39.044776 codezen-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 codezen-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1918 2023-06-07 08:58:11.099573 codezen-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.2.0/codezen/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.2.0/codezen/__main__.py
+-rw-r--r--   0        0        0     4174 2023-06-07 09:00:19.963281 codezen-0.2.0/codezen/app.py
+-rw-r--r--   0        0        0      521 2023-06-07 09:01:27.807588 codezen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 codezen-0.2.0/PKG-INFO
```

### Comparing `codezen-0.1.1/LICENSE` & `codezen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codezen-0.1.1/README.md` & `codezen-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # CodeZen
 
 ## Description
 
-CodeZen is your indispensable partner in programming. It is a CLI utility that uses LLMs to help you debug and evolve your codebase based on your requests.
+CodeZen is a CLI utility that uses LLMs to help you debug and evolve your codebase based on your requests.
+
+Usage examples:
+```bash
+codezen "Why am I getting <some exception message>?"
+codezen "Write a README.md file for this project"
+```
 
 The differences from Github Copilot:
 * This is a CLI tool, meaning it can be used regardless of your chosen IDE.
-* This provides the LLM with the entire codebase, so it can do things that require a more wholistic view of your project.
+* This provides the LLM with the entire codebase, so it can do things that require a more holistic view of your project.
 
 Current limitations:
-* Only Work for small codebases- currently we send the entire codebase in each request. 😆
+* Only works for small codebases- currently it sends the entire codebase on each request. 😆
 * It can't change files autonomously, it only offers a solution.
-* It uses hard coded direcory names to know which files to ignore. Currently it only contains Python and Node.js common ignorable directories.
+* It uses gitignore file to know which files to ignore, so you must run this in a git repo and you can't currently ignore files that don't appear there.
 
 
 ## Installation
 ### Using PyPi
 You can install the application using `pip` or `pipx`:
 ```bash
 pip install --user codezen
@@ -32,41 +38,35 @@
 git clone https://github.com/mmaorc/codezen
 cd codezen
 poetry build
 ```
 
 
 ### Development
-For development purposes, clone the repository, navigate to the project directory, and install in a virtual environment:
+For development purposes, clone the repository, navigate to the project directory, and install it in a virtual environment:
 
 ```bash
 git clone https://github.com/mmaorc/codezen
 cd codezen
 poetry install
 poetry shell
 ```
 
 ## Usage
 
-Prior to running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
+Before running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
 
 Run CodeZen with the following command:
 
 ```bash
 codezen <issue_description>
 ```
 
 `<issue_description>`: Describe the issue you are facing with your code
 
-Example:
-
-```bash
-codezen "Im getting the following error: ValueError: invalid literal for int() with base 10: a"
-codezen "Write a readme.md file for this project"
-```
 
 ## Contributing
 
 If you would like to contribute to this project, please feel free to fork the repository, create a feature branch, and submit a pull request.
 
 ## License
```

### Comparing `codezen-0.1.1/codezen/app.py` & `codezen-0.2.0/codezen/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,67 @@
 import argparse
 import logging
+import subprocess
+from pathlib import Path
+
+from binaryornot.check import is_binary
 from langchain import LLMChain, PromptTemplate
+from langchain.callbacks import get_openai_callback
 from langchain.chat_models import ChatOpenAI
-
-import os
-from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.docstore.document import Document
+from langchain.text_splitter import RecursiveCharacterTextSplitter
 
-# I should try to use .gitignore file here
-ignored_directories = [
-    ".git",
-    "node_modules",
-    "public",
-    ".mypy_cache",
-    "venv",
-    ".venv",
-    "__pycache__",
-    "dist",
-    "docs",
-    ".mypy_cache",
-]
-ignored_filenames = ["package-lock.json", ".DS_Store", "poetry.lock"]
-
-prompt = """You are an AI debugger who is trying to debug a program for a user based on their file system. The user has provided you with the following files and their contents, finally folllowed by the error message or issue they are facing.
+prompt = """You are an AI coder who is trying to help the user develop and debug an application based on their file system. The user has provided you with the following files and their contents, finally folllowed by the error message or issue they are facing.
 
 The file list is given between the triple backticks (```), Each file is separated by three dashes (---). There are no files in the project besides the ones listed here.
 ```
 {file_context}
 ```
 
 The issue is given between the triple hashes (###):
 ###
 {issue_description}
 ###
 
-If you need further information please ask. If you don't know the answer, say that you don't know.
+If you are not sure what the answer is, say that explicitly.
 """
 prompt_template = PromptTemplate(
     input_variables=["file_context", "issue_description"], template=prompt
 )
 
 
-def load_files(root_dir):
+def get_project_files_paths(root_dir: str) -> list[Path]:
+    result = subprocess.run(
+        ["git", "ls-files"], cwd=root_dir, capture_output=True, text=True
+    ).stdout
+    file_paths_strings = result.splitlines()
+    file_paths = [Path(root_dir) / Path(fp) for fp in file_paths_strings]
+    return file_paths
+
+
+def load_files_to_langchain_documents(root_dir: Path, project_files_paths: list[Path]):
     text_splitter = RecursiveCharacterTextSplitter()
 
     docs = []
-    for dirpath, dirnames, filenames in os.walk(root_dir):
-        relpath = os.path.relpath(dirpath, root_dir)
-        if not any(d in relpath for d in ignored_directories):
-            for file in filenames:
-                if file not in ignored_filenames:
-                    abs_file_path = os.path.join(dirpath, file)
-                    try:
-                        with open(abs_file_path, encoding="utf-8") as f:
-                            text = f.read()
-                        natural_document = Document(
-                            page_content=text,
-                            metadata={"source": os.path.join(relpath, file)},
-                        )
-                        split_document = text_splitter.split_documents(
-                            [natural_document]
-                        )
-                        docs.extend(split_document)
-                    except Exception as e:
-                        print(
-                            f"Exception loading the document {abs_file_path}:\n"
-                            + str(e)
-                        )
+    for file_path in project_files_paths:
+        try:
+            if is_binary(str(file_path)):
+                logging.info(f"Skipping binary file {file_path}")
+                continue
+            with open(file_path, encoding="utf-8") as f:
+                text = f.read()
+            relative_path = file_path.relative_to(root_dir)  # Maybe we don't need this?
+            natural_document = Document(
+                page_content=text,
+                metadata={"source": relative_path},
+            )
+            split_document = text_splitter.split_documents([natural_document])
+            docs.extend(split_document)
+        except Exception as e:
+            raise Exception(f"Exception loading the document {file_path}:\n") from e
 
     return docs
 
 
 def build_context_string(docs):
     all_context = []
     for doc in docs:
@@ -108,24 +99,32 @@
         help="The issue description",
     )
     args = parser.parse_args()
 
     # Set logging level
     logging.basicConfig(level=logging.WARNING)
     if args.verbose:
-        logging.basicConfig(level=logging.DEBUG)
+        logging.basicConfig(level=logging.INFO)
 
     model = ChatOpenAI(model_name=args.model_name)
     llm = LLMChain(llm=model, prompt=prompt_template)
 
-    docs = load_files(args.root_dir)
+    project_files_paths = get_project_files_paths(args.root_dir)
+    docs = load_files_to_langchain_documents(args.root_dir, project_files_paths)
     context_string = build_context_string(docs)
 
     logging.info(
         f"Loaded {len(docs)} documents, total of {sum([len(doc.page_content) for doc in docs])} characters"
     )
 
-    result = llm.run(
-        file_context=context_string, issue_description=args.issue_description
-    )
+    with get_openai_callback() as cb:
+        result = llm.run(
+            file_context=context_string, issue_description=args.issue_description
+        )
 
+    print()
+    print("Answer:")
     print(result)
+
+    print()
+    print("OpenAI stats:")
+    print(cb)
```

### Comparing `codezen-0.1.1/PKG-INFO` & `codezen-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: codezen
-Version: 0.1.1
+Version: 0.2.0
 Summary: Your indispensable partner in programming
 Home-page: https://github.com/mmaorc/codezen
 Author: Maor Cohen
 Author-email: me@maorcohen.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: langchain (>=0.0.177,<0.0.178)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Description-Content-Type: text/markdown
 
 # CodeZen
 
 ## Description
 
-CodeZen is your indispensable partner in programming. It is a CLI utility that uses LLMs to help you debug and evolve your codebase based on your requests.
+CodeZen is a CLI utility that uses LLMs to help you debug and evolve your codebase based on your requests.
+
+Usage examples:
+```bash
+codezen "Why am I getting <some exception message>?"
+codezen "Write a README.md file for this project"
+```
 
 The differences from Github Copilot:
 * This is a CLI tool, meaning it can be used regardless of your chosen IDE.
-* This provides the LLM with the entire codebase, so it can do things that require a more wholistic view of your project.
+* This provides the LLM with the entire codebase, so it can do things that require a more holistic view of your project.
 
 Current limitations:
-* Only Work for small codebases- currently we send the entire codebase in each request. 😆
+* Only works for small codebases- currently it sends the entire codebase on each request. 😆
 * It can't change files autonomously, it only offers a solution.
-* It uses hard coded direcory names to know which files to ignore. Currently it only contains Python and Node.js common ignorable directories.
+* It uses gitignore file to know which files to ignore, so you must run this in a git repo and you can't currently ignore files that don't appear there.
 
 
 ## Installation
 ### Using PyPi
 You can install the application using `pip` or `pipx`:
 ```bash
 pip install --user codezen
@@ -46,41 +53,35 @@
 git clone https://github.com/mmaorc/codezen
 cd codezen
 poetry build
 ```
 
 
 ### Development
-For development purposes, clone the repository, navigate to the project directory, and install in a virtual environment:
+For development purposes, clone the repository, navigate to the project directory, and install it in a virtual environment:
 
 ```bash
 git clone https://github.com/mmaorc/codezen
 cd codezen
 poetry install
 poetry shell
 ```
 
 ## Usage
 
-Prior to running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
+Before running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
 
 Run CodeZen with the following command:
 
 ```bash
 codezen <issue_description>
 ```
 
 `<issue_description>`: Describe the issue you are facing with your code
 
-Example:
-
-```bash
-codezen "Im getting the following error: ValueError: invalid literal for int() with base 10: a"
-codezen "Write a readme.md file for this project"
-```
 
 ## Contributing
 
 If you would like to contribute to this project, please feel free to fork the repository, create a feature branch, and submit a pull request.
 
 ## License
```

