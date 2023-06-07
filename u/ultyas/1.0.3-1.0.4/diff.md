# Comparing `tmp/ultyas-1.0.3.tar.gz` & `tmp/ultyas-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultyas-1.0.3.tar", last modified: Tue Apr 18 15:48:07 2023, max compression
+gzip compressed data, was "ultyas-1.0.4.tar", last modified: Wed Jun  7 13:02:47 2023, max compression
```

## Comparing `ultyas-1.0.3.tar` & `ultyas-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-18 15:48:07.642502 ultyas-1.0.3/
--rw-r--r--   0 work      (1000) work      (1000)       26 2023-04-18 14:41:15.000000 ultyas-1.0.3/.gitignore
--rw-r--r--   0 work      (1000) work      (1000)    35149 2023-04-04 03:13:38.000000 ultyas-1.0.3/LICENSE
--rw-r--r--   0 work      (1000) work      (1000)     1735 2023-04-18 15:48:07.642502 ultyas-1.0.3/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      713 2023-04-18 14:41:15.000000 ultyas-1.0.3/README.md
--rw-r--r--   0 work      (1000) work      (1000)       38 2023-04-18 15:48:07.642502 ultyas-1.0.3/setup.cfg
--rwxr-xr-x   0 work      (1000) work      (1000)     1558 2023-04-18 15:46:36.000000 ultyas-1.0.3/setup.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-18 15:48:07.642502 ultyas-1.0.3/ultyas/
--rw-r--r--   0 work      (1000) work      (1000)     4574 2023-04-18 15:43:19.000000 ultyas-1.0.3/ultyas/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     4730 2023-04-18 15:42:26.000000 ultyas-1.0.3/ultyas/ultisnips.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-18 15:48:07.642502 ultyas-1.0.3/ultyas.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     1735 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      229 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)       66 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)        7 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/top_level.txt
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-06-07 13:02:47.006060 ultyas-1.0.4/
+-rw-r--r--   0 work      (1000) work      (1000)       26 2023-04-18 14:41:15.000000 ultyas-1.0.4/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)    35149 2023-04-04 03:13:38.000000 ultyas-1.0.4/LICENSE
+-rw-r--r--   0 work      (1000) work      (1000)     1428 2023-06-07 13:02:47.006060 ultyas-1.0.4/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      713 2023-04-18 14:41:15.000000 ultyas-1.0.4/README.md
+-rw-r--r--   0 work      (1000) work      (1000)       38 2023-06-07 13:02:47.006060 ultyas-1.0.4/setup.cfg
+-rwxr-xr-x   0 work      (1000) work      (1000)     1256 2023-06-07 13:01:04.000000 ultyas-1.0.4/setup.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-06-07 13:02:47.006060 ultyas-1.0.4/ultyas/
+-rw-r--r--   0 work      (1000) work      (1000)     4579 2023-06-07 12:45:28.000000 ultyas-1.0.4/ultyas/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)     6908 2023-06-07 12:45:28.000000 ultyas-1.0.4/ultyas/ultisnips.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-06-07 13:02:47.006060 ultyas-1.0.4/ultyas.egg-info/
+-rw-r--r--   0 work      (1000) work      (1000)     1428 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      229 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1000) work      (1000)        1 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1000) work      (1000)       66 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/entry_points.txt
+-rw-r--r--   0 work      (1000) work      (1000)        7 2023-06-07 13:02:46.000000 ultyas-1.0.4/ultyas.egg-info/top_level.txt
```

### Comparing `ultyas-1.0.3/LICENSE` & `ultyas-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ultyas-1.0.3/PKG-INFO` & `ultyas-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: ultyas
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool for converting code snippets from Ultisnips to YASnippet format
 Home-page: https://github.com/jamescherti/ultyas
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: Other
 Classifier: Topic :: Text Editors :: Emacs
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ultyas - Ultisnips to YASnippet Conversion Tool
 
 Ultyas is a command-line tool, written by [James Cherti](https://www.jamescherti.com), designed to simplify the process of converting code snippets from Ultisnips to YASnippet format.
```

### Comparing `ultyas-1.0.3/README.md` & `ultyas-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ultyas-1.0.3/setup.py` & `ultyas-1.0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ultyas",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     description=("A tool for converting code snippets from "
                  "Ultisnips to YASnippet format"),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/ultyas",
     author="James Cherti",
@@ -24,22 +24,15 @@
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Environment :: Console",
         "Operating System :: POSIX :: Linux",
         "Operating System :: POSIX :: Other",
         "Topic :: Text Editors :: Emacs",
-
-        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
     ],
     entry_points={
         "console_scripts": [
             "ultyas=ultyas.__init__:command_line_interface",
         ],
     },
 )
```

### Comparing `ultyas-1.0.3/ultyas/__init__.py` & `ultyas-1.0.4/ultyas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         default="nothing",
         choices=["auto", "fixed", "nothing"],
         required=False,
         help=("Add one of the following comments to the "
               "YASnippet snippets that will be generated: "
               "\"# expand-env: ((yas-indent-line 'fixed))\" or "
               "\"# expand-env: ((yas-indent-line 'auto))\". "
-              "For information on 'yas-indent-line', visit: "
+              "For more information on 'yas-indent-line', visit: "
               "https://joaotavora.github.io/yasnippet/snippet-reference.html"
               "#yas-indent-line"),
     )
 
     parser.add_argument(
         "-t",
         "--convert-tabs-to",
```

### Comparing `ultyas-1.0.3/ultyas.egg-info/PKG-INFO` & `ultyas-1.0.4/ultyas.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: ultyas
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool for converting code snippets from Ultisnips to YASnippet format
 Home-page: https://github.com/jamescherti/ultyas
 Author: James Cherti
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: Other
 Classifier: Topic :: Text Editors :: Emacs
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ultyas - Ultisnips to YASnippet Conversion Tool
 
 Ultyas is a command-line tool, written by [James Cherti](https://www.jamescherti.com), designed to simplify the process of converting code snippets from Ultisnips to YASnippet format.
```

