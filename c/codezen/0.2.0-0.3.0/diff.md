# Comparing `tmp/codezen-0.2.0.tar.gz` & `tmp/codezen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codezen-0.2.0.tar", max compression
+gzip compressed data, was "codezen-0.3.0.tar", max compression
```

## Comparing `codezen-0.2.0.tar` & `codezen-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.2.0/LICENSE
--rw-r--r--   0        0        0     1918 2023-06-07 08:58:11.099573 codezen-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.2.0/codezen/__init__.py
--rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.2.0/codezen/__main__.py
--rw-r--r--   0        0        0     4174 2023-06-07 09:00:19.963281 codezen-0.2.0/codezen/app.py
--rw-r--r--   0        0        0      521 2023-06-07 09:01:27.807588 codezen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 codezen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1918 2023-06-07 08:58:11.099573 codezen-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.3.0/codezen/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.3.0/codezen/__main__.py
+-rw-r--r--   0        0        0     4633 2023-06-07 13:39:21.600172 codezen-0.3.0/codezen/app.py
+-rw-r--r--   0        0        0      582 2023-06-07 13:38:29.938525 codezen-0.3.0/codezen/ignore_files.py
+-rw-r--r--   0        0        0      542 2023-06-07 13:41:03.444856 codezen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 codezen-0.3.0/PKG-INFO
```

### Comparing `codezen-0.2.0/LICENSE` & `codezen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codezen-0.2.0/README.md` & `codezen-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `codezen-0.2.0/codezen/app.py` & `codezen-0.3.0/codezen/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from binaryornot.check import is_binary
 from langchain import LLMChain, PromptTemplate
 from langchain.callbacks import get_openai_callback
 from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
+from codezen.ignore_files import filter_files, load_ignore_file
+
+
 prompt = """You are an AI coder who is trying to help the user develop and debug an application based on their file system. The user has provided you with the following files and their contents, finally folllowed by the error message or issue they are facing.
 
 The file list is given between the triple backticks (```), Each file is separated by three dashes (---). There are no files in the project besides the ones listed here.
 ```
 {file_context}
 ```
 
@@ -91,28 +94,42 @@
         "-d",
         "--root-dir",
         dest="root_dir",
         default=".//",
         help="The root directory of the project",
     )
     parser.add_argument(
+        "-i",
+        "--ignore-file",
+        dest="ignore_file",
+        default="./.czignore",
+        help="The path to the .czignore file",
+    )
+    parser.add_argument(
         "issue_description",
         help="The issue description",
     )
     args = parser.parse_args()
 
     # Set logging level
     logging.basicConfig(level=logging.WARNING)
     if args.verbose:
         logging.basicConfig(level=logging.INFO)
 
     model = ChatOpenAI(model_name=args.model_name)
     llm = LLMChain(llm=model, prompt=prompt_template)
 
     project_files_paths = get_project_files_paths(args.root_dir)
+    czignore_patterns = load_ignore_file(args.ignore_file)
+    project_files_paths = (
+        filter_files(project_files_paths, czignore_patterns)
+        if czignore_patterns
+        else project_files_paths
+    )
+
     docs = load_files_to_langchain_documents(args.root_dir, project_files_paths)
     context_string = build_context_string(docs)
 
     logging.info(
         f"Loaded {len(docs)} documents, total of {sum([len(doc.page_content) for doc in docs])} characters"
     )
```

### Comparing `codezen-0.2.0/pyproject.toml` & `codezen-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "codezen"
-version = "0.2.0"
+version = "0.3.0"
 description = "Your indispensable partner in programming"
 authors = ["Maor Cohen <me@maorcohen.net>"]
 homepage = "https://github.com/mmaorc/codezen"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 langchain = "^0.0.177"
 openai = "^0.27.7"
 binaryornot = "^0.4.4"
+pathspec = "^0.11.1"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `codezen-0.2.0/PKG-INFO` & `codezen-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: codezen
-Version: 0.2.0
+Version: 0.3.0
 Summary: Your indispensable partner in programming
 Home-page: https://github.com/mmaorc/codezen
 Author: Maor Cohen
 Author-email: me@maorcohen.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: langchain (>=0.0.177,<0.0.178)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
+Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Description-Content-Type: text/markdown
 
 # CodeZen
 
 ## Description
 
 CodeZen is a CLI utility that uses LLMs to help you debug and evolve your codebase based on your requests.
```

