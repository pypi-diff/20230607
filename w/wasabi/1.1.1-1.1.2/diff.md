# Comparing `tmp/wasabi-1.1.1.tar.gz` & `tmp/wasabi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasabi-1.1.1.tar", last modified: Sat Jan 14 11:13:42 2023, max compression
+gzip compressed data, was "wasabi-1.1.2.tar", last modified: Wed Jun  7 07:30:14 2023, max compression
```

## Comparing `wasabi-1.1.1.tar` & `wasabi-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-14 11:13:42.739427 wasabi-1.1.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1079 2023-01-14 11:13:23.000000 wasabi-1.1.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-14 11:13:23.000000 wasabi-1.1.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    28362 2023-01-14 11:13:42.739427 wasabi-1.1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    28050 2023-01-14 11:13:23.000000 wasabi-1.1.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      656 2023-01-14 11:13:42.739427 wasabi-1.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      150 2023-01-14 11:13:23.000000 wasabi-1.1.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-14 11:13:42.735427 wasabi-1.1.1/wasabi/
--rw-r--r--   0 vsts      (1001) docker     (122)      311 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4229 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/markdown.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11775 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/printer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6773 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tables.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-14 11:13:42.739427 wasabi-1.1.1/wasabi/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-14 11:13:42.739427 wasabi-1.1.1/wasabi/tests/test-data/
--rw-r--r--   0 vsts      (1001) docker     (122)      835 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test-data/wasabi-test-notebook.ipynb
--rw-r--r--   0 vsts      (1001) docker     (122)     1122 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test_jupyter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test_markdown.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test_printer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17497 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test_tables.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1622 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test_traceback.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2453 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/tests/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4834 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/traceback_printer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7260 2023-01-14 11:13:23.000000 wasabi-1.1.1/wasabi/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-14 11:13:42.735427 wasabi-1.1.1/wasabi.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    28362 2023-01-14 11:13:42.000000 wasabi-1.1.1/wasabi.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      603 2023-01-14 11:13:42.000000 wasabi-1.1.1/wasabi.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-14 11:13:42.000000 wasabi-1.1.1/wasabi.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-01-14 11:13:42.000000 wasabi-1.1.1/wasabi.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-01-14 11:13:42.000000 wasabi-1.1.1/wasabi.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-14 11:13:42.000000 wasabi-1.1.1/wasabi.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 07:30:14.425761 wasabi-1.1.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1079 2023-06-07 07:30:03.000000 wasabi-1.1.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-07 07:30:03.000000 wasabi-1.1.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    28566 2023-06-07 07:30:14.425761 wasabi-1.1.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    28254 2023-06-07 07:30:03.000000 wasabi-1.1.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      656 2023-06-07 07:30:14.425761 wasabi-1.1.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      150 2023-06-07 07:30:03.000000 wasabi-1.1.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 07:30:14.421760 wasabi-1.1.2/wasabi/
+-rw-r--r--   0 vsts      (1001) docker     (122)      311 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4229 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/markdown.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12305 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/printer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6773 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tables.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 07:30:14.425761 wasabi-1.1.2/wasabi/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 07:30:14.425761 wasabi-1.1.2/wasabi/tests/test-data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      835 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test-data/wasabi-test-notebook.ipynb
+-rw-r--r--   0 vsts      (1001) docker     (122)     1122 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test_jupyter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test_markdown.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test_printer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17497 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1622 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test_traceback.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2453 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/tests/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4834 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/traceback_printer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7260 2023-06-07 07:30:03.000000 wasabi-1.1.2/wasabi/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-07 07:30:14.421760 wasabi-1.1.2/wasabi.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    28566 2023-06-07 07:30:14.000000 wasabi-1.1.2/wasabi.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      603 2023-06-07 07:30:14.000000 wasabi-1.1.2/wasabi.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-07 07:30:14.000000 wasabi-1.1.2/wasabi.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-06-07 07:30:14.000000 wasabi-1.1.2/wasabi.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-06-07 07:30:14.000000 wasabi-1.1.2/wasabi.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-07 07:30:14.000000 wasabi-1.1.2/wasabi.egg-info/zip-safe
```

### Comparing `wasabi-1.1.1/LICENSE` & `wasabi-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/PKG-INFO` & `wasabi-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasabi
-Version: 1.1.1
+Version: 1.1.2
 Summary: A lightweight console printing and formatting toolkit
 Home-page: https://github.com/explosion/wasabi
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 options, I've always ended up wanting something slightly different or slightly
 custom.
 
 This package is still a work in progress and aims to bundle those utilities in a
 standardised way so they can be shared across our other projects. It's super
 lightweight, has zero dependencies and works with Python 3.6+.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/1/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=1)
+[![tests](https://github.com/explosion/wasabi/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/wasabi/actions/workflows/tests.yml)
 [![PyPi](https://img.shields.io/pypi/v/wasabi.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/wasabi)
 [![conda](https://img.shields.io/conda/vn/conda-forge/wasabi.svg?style=flat-square&logo=conda-forge/logoColor=white)](https://anaconda.org/conda-forge/wasabi)
 [![GitHub](https://img.shields.io/github/release/ines/wasabi/all.svg?style=flat-square&logo=github)](https://github.com/ines/wasabi)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 <img width="609" src="https://user-images.githubusercontent.com/13643239/48663861-8c9ea000-ea96-11e8-8b04-d120c52276a8.png">
 
@@ -160,17 +160,17 @@
 msg = Printer()
 with msg.loading("Loading..."):
     # Do something here that takes longer
     time.sleep(10)
 msg.good("Successfully loaded something!")
 ```
 
-| Argument | Type | Description                        | Default           |
-| -------- | ---- | ---------------------------------- | ----------------- |
-| `text`   | str  | The text to display while loading. | `"Loading..."`    |
+| Argument | Type | Description                        | Default        |
+| -------- | ---- | ---------------------------------- | -------------- |
+| `text`   | str  | The text to display while loading. | `"Loading..."` |
 
 #### <kbd>method</kbd> `Printer.table`, `Printer.row`
 
 See [Tables](#tables).
 
 #### <kbd>property</kbd> `Printer.counts`
 
@@ -210,54 +210,54 @@
 ```
 Column 1   Column 2    Column 3
 --------   ---------   ----------
       a1      a2       a3
       b1      b2       b3
 ```
 
-| Argument    | Type                | Description                                                                                                                         | Default  |
-| ----------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | -------- |
-| `data`      | iterable / dict     | The data to render. Either a list of lists (one per row) or a dict for two-column tables.                                           |          |
-| `header`    | iterable            | Optional header columns.                                                                                                            | `None`   |
-| `footer`    | iterable            | Optional footer columns.                                                                                                            | `None`   |
-| `divider`   | bool                | Show a divider line between header/footer and body.                                                                                 | `False`  |
-| `widths`    | iterable / `"auto"` | Column widths in order. If `"auto"`, widths will be calculated automatically based on the largest value.                            | `"auto"` |
-| `max_col`   | int                 | Maximum column width.                                                                                                               | `30`     |
-| `spacing`   | int                 | Number of spaces between columns.                                                                                                   | `3`      |
-| `aligns`    | iterable / unicode  | Columns alignments in order. `"l"` (left, default), `"r"` (right) or `"c"` (center). If If a string, value is used for all columns. | `None`   |
-| `multiline` | bool                | If a cell value is a list of a tuple, render it on multiple lines, with one value per line.                                         | `False`  |
-| `env_prefix` | unicode                | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                         | `"WASABI"` |
-| `color_values` | dict                | Add or overwrite color values, name mapped to value.                                         | `None`   |
-| `fg_colors` | iterable                | Foreground colors, one per column. None can be specified for individual columns to retain the default background color. | `None`   |
-| `bg_colors` | iterable                | Background colors, one per column. None can be specified for individual columns to retain the default background color. | `None`   |
-| **RETURNS** | str                 | The formatted table.                                                                                                                |          |
+| Argument       | Type                | Description                                                                                                                         | Default    |
+| -------------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------- |
+| `data`         | iterable / dict     | The data to render. Either a list of lists (one per row) or a dict for two-column tables.                                           |            |
+| `header`       | iterable            | Optional header columns.                                                                                                            | `None`     |
+| `footer`       | iterable            | Optional footer columns.                                                                                                            | `None`     |
+| `divider`      | bool                | Show a divider line between header/footer and body.                                                                                 | `False`    |
+| `widths`       | iterable / `"auto"` | Column widths in order. If `"auto"`, widths will be calculated automatically based on the largest value.                            | `"auto"`   |
+| `max_col`      | int                 | Maximum column width.                                                                                                               | `30`       |
+| `spacing`      | int                 | Number of spaces between columns.                                                                                                   | `3`        |
+| `aligns`       | iterable / unicode  | Columns alignments in order. `"l"` (left, default), `"r"` (right) or `"c"` (center). If If a string, value is used for all columns. | `None`     |
+| `multiline`    | bool                | If a cell value is a list of a tuple, render it on multiple lines, with one value per line.                                         | `False`    |
+| `env_prefix`   | unicode             | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                                                         | `"WASABI"` |
+| `color_values` | dict                | Add or overwrite color values, name mapped to value.                                                                                | `None`     |
+| `fg_colors`    | iterable            | Foreground colors, one per column. None can be specified for individual columns to retain the default background color.             | `None`     |
+| `bg_colors`    | iterable            | Background colors, one per column. None can be specified for individual columns to retain the default background color.             | `None`     |
+| **RETURNS**    | str                 | The formatted table.                                                                                                                |            |
 
 #### <kbd>function</kbd> `row`
 
 ```python
 from wasabi import row
 
 data = ("a1", "a2", "a3")
 formatted = row(data)
 ```
 
 ```
 a1   a2   a3
 ```
 
-| Argument    | Type                      | Description                                                                                                                                                | Default  |
-| ----------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
-| `data`      | iterable                  | The individual columns to format.                                                                                                                          |          |
-| `widths`    | list / int / `"auto"` | Column widths, either one integer for all columns or an iterable of values. If "auto", widths will be calculated automatically based on the largest value. | `"auto"` |
-| `spacing`   | int                       | Number of spaces between columns.                                                                                                                          | `3`      |
-| `aligns`    | list                  | Columns alignments in order. `"l"` (left), `"r"` (right) or `"c"` (center).                                                                                | `None`   |
-| `env_prefix` | unicode                | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                         | `"WASABI"` |
-| `fg_colors`    | list                  | Foreground colors for the columns, in order. None can be specified for individual columns to retain the default foreground color. | `None`   |
-| `bg_colors`    | list                  | Background colors for the columns, in order. None can be specified for individual columns to retain the default background color. | `None`   |
-| **RETURNS** | str                       | The formatted row.                                                                                                                                         |          |
+| Argument     | Type                  | Description                                                                                                                                                | Default    |
+| ------------ | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
+| `data`       | iterable              | The individual columns to format.                                                                                                                          |            |
+| `widths`     | list / int / `"auto"` | Column widths, either one integer for all columns or an iterable of values. If "auto", widths will be calculated automatically based on the largest value. | `"auto"`   |
+| `spacing`    | int                   | Number of spaces between columns.                                                                                                                          | `3`        |
+| `aligns`     | list                  | Columns alignments in order. `"l"` (left), `"r"` (right) or `"c"` (center).                                                                                | `None`     |
+| `env_prefix` | unicode               | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                                                                                | `"WASABI"` |
+| `fg_colors`  | list                  | Foreground colors for the columns, in order. None can be specified for individual columns to retain the default foreground color.                          | `None`     |
+| `bg_colors`  | list                  | Background colors for the columns, in order. None can be specified for individual columns to retain the default background color.                          | `None`     |
+| **RETURNS**  | str                   | The formatted row.                                                                                                                                         |            |
 
 ### <kbd>class</kbd> `TracebackPrinter`
 
 Helper to output custom formatted tracebacks and error messages. Currently used
 in [Thinc](https://github.com/explosion/thinc).
 
 #### <kbd>method</kbd> `TracebackPrinter.__init__`
@@ -311,15 +311,16 @@
 | `*texts`    | str      | Optional texts to print (one per line).                                                    |         |
 | `highlight` | str      | Optional sequence to highlight in the traceback, e.g. the bad value that caused the error. | `False` |
 | `tb`        | iterable | The traceback, e.g. generated by `traceback.extract_stack()`.                              | `None`  |
 | **RETURNS** | str      | The formatted traceback. Can be printed or raised by custom exception.                     |         |
 
 ### <kbd>class</kbd> `MarkdownRenderer`
 
-Helper to create Markdown-formatted content. Will store the blocks added to the Markdown document in order.
+Helper to create Markdown-formatted content. Will store the blocks added to the
+Markdown document in order.
 
 ```python
 from wasabi import MarkdownRenderer
 
 md = MarkdownRenderer()
 md.add(md.title(1, "Hello world"))
 md.add("This is a paragraph")
```

### Comparing `wasabi-1.1.1/README.md` & `wasabi-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 options, I've always ended up wanting something slightly different or slightly
 custom.
 
 This package is still a work in progress and aims to bundle those utilities in a
 standardised way so they can be shared across our other projects. It's super
 lightweight, has zero dependencies and works with Python 3.6+.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/1/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=1)
+[![tests](https://github.com/explosion/wasabi/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/wasabi/actions/workflows/tests.yml)
 [![PyPi](https://img.shields.io/pypi/v/wasabi.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/wasabi)
 [![conda](https://img.shields.io/conda/vn/conda-forge/wasabi.svg?style=flat-square&logo=conda-forge/logoColor=white)](https://anaconda.org/conda-forge/wasabi)
 [![GitHub](https://img.shields.io/github/release/ines/wasabi/all.svg?style=flat-square&logo=github)](https://github.com/ines/wasabi)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 <img width="609" src="https://user-images.githubusercontent.com/13643239/48663861-8c9ea000-ea96-11e8-8b04-d120c52276a8.png">
 
@@ -148,17 +148,17 @@
 msg = Printer()
 with msg.loading("Loading..."):
     # Do something here that takes longer
     time.sleep(10)
 msg.good("Successfully loaded something!")
 ```
 
-| Argument | Type | Description                        | Default           |
-| -------- | ---- | ---------------------------------- | ----------------- |
-| `text`   | str  | The text to display while loading. | `"Loading..."`    |
+| Argument | Type | Description                        | Default        |
+| -------- | ---- | ---------------------------------- | -------------- |
+| `text`   | str  | The text to display while loading. | `"Loading..."` |
 
 #### <kbd>method</kbd> `Printer.table`, `Printer.row`
 
 See [Tables](#tables).
 
 #### <kbd>property</kbd> `Printer.counts`
 
@@ -198,54 +198,54 @@
 ```
 Column 1   Column 2    Column 3
 --------   ---------   ----------
       a1      a2       a3
       b1      b2       b3
 ```
 
-| Argument    | Type                | Description                                                                                                                         | Default  |
-| ----------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | -------- |
-| `data`      | iterable / dict     | The data to render. Either a list of lists (one per row) or a dict for two-column tables.                                           |          |
-| `header`    | iterable            | Optional header columns.                                                                                                            | `None`   |
-| `footer`    | iterable            | Optional footer columns.                                                                                                            | `None`   |
-| `divider`   | bool                | Show a divider line between header/footer and body.                                                                                 | `False`  |
-| `widths`    | iterable / `"auto"` | Column widths in order. If `"auto"`, widths will be calculated automatically based on the largest value.                            | `"auto"` |
-| `max_col`   | int                 | Maximum column width.                                                                                                               | `30`     |
-| `spacing`   | int                 | Number of spaces between columns.                                                                                                   | `3`      |
-| `aligns`    | iterable / unicode  | Columns alignments in order. `"l"` (left, default), `"r"` (right) or `"c"` (center). If If a string, value is used for all columns. | `None`   |
-| `multiline` | bool                | If a cell value is a list of a tuple, render it on multiple lines, with one value per line.                                         | `False`  |
-| `env_prefix` | unicode                | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                         | `"WASABI"` |
-| `color_values` | dict                | Add or overwrite color values, name mapped to value.                                         | `None`   |
-| `fg_colors` | iterable                | Foreground colors, one per column. None can be specified for individual columns to retain the default background color. | `None`   |
-| `bg_colors` | iterable                | Background colors, one per column. None can be specified for individual columns to retain the default background color. | `None`   |
-| **RETURNS** | str                 | The formatted table.                                                                                                                |          |
+| Argument       | Type                | Description                                                                                                                         | Default    |
+| -------------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------- |
+| `data`         | iterable / dict     | The data to render. Either a list of lists (one per row) or a dict for two-column tables.                                           |            |
+| `header`       | iterable            | Optional header columns.                                                                                                            | `None`     |
+| `footer`       | iterable            | Optional footer columns.                                                                                                            | `None`     |
+| `divider`      | bool                | Show a divider line between header/footer and body.                                                                                 | `False`    |
+| `widths`       | iterable / `"auto"` | Column widths in order. If `"auto"`, widths will be calculated automatically based on the largest value.                            | `"auto"`   |
+| `max_col`      | int                 | Maximum column width.                                                                                                               | `30`       |
+| `spacing`      | int                 | Number of spaces between columns.                                                                                                   | `3`        |
+| `aligns`       | iterable / unicode  | Columns alignments in order. `"l"` (left, default), `"r"` (right) or `"c"` (center). If If a string, value is used for all columns. | `None`     |
+| `multiline`    | bool                | If a cell value is a list of a tuple, render it on multiple lines, with one value per line.                                         | `False`    |
+| `env_prefix`   | unicode             | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                                                         | `"WASABI"` |
+| `color_values` | dict                | Add or overwrite color values, name mapped to value.                                                                                | `None`     |
+| `fg_colors`    | iterable            | Foreground colors, one per column. None can be specified for individual columns to retain the default background color.             | `None`     |
+| `bg_colors`    | iterable            | Background colors, one per column. None can be specified for individual columns to retain the default background color.             | `None`     |
+| **RETURNS**    | str                 | The formatted table.                                                                                                                |            |
 
 #### <kbd>function</kbd> `row`
 
 ```python
 from wasabi import row
 
 data = ("a1", "a2", "a3")
 formatted = row(data)
 ```
 
 ```
 a1   a2   a3
 ```
 
-| Argument    | Type                      | Description                                                                                                                                                | Default  |
-| ----------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
-| `data`      | iterable                  | The individual columns to format.                                                                                                                          |          |
-| `widths`    | list / int / `"auto"` | Column widths, either one integer for all columns or an iterable of values. If "auto", widths will be calculated automatically based on the largest value. | `"auto"` |
-| `spacing`   | int                       | Number of spaces between columns.                                                                                                                          | `3`      |
-| `aligns`    | list                  | Columns alignments in order. `"l"` (left), `"r"` (right) or `"c"` (center).                                                                                | `None`   |
-| `env_prefix` | unicode                | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                         | `"WASABI"` |
-| `fg_colors`    | list                  | Foreground colors for the columns, in order. None can be specified for individual columns to retain the default foreground color. | `None`   |
-| `bg_colors`    | list                  | Background colors for the columns, in order. None can be specified for individual columns to retain the default background color. | `None`   |
-| **RETURNS** | str                       | The formatted row.                                                                                                                                         |          |
+| Argument     | Type                  | Description                                                                                                                                                | Default    |
+| ------------ | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
+| `data`       | iterable              | The individual columns to format.                                                                                                                          |            |
+| `widths`     | list / int / `"auto"` | Column widths, either one integer for all columns or an iterable of values. If "auto", widths will be calculated automatically based on the largest value. | `"auto"`   |
+| `spacing`    | int                   | Number of spaces between columns.                                                                                                                          | `3`        |
+| `aligns`     | list                  | Columns alignments in order. `"l"` (left), `"r"` (right) or `"c"` (center).                                                                                | `None`     |
+| `env_prefix` | unicode               | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                                                                                | `"WASABI"` |
+| `fg_colors`  | list                  | Foreground colors for the columns, in order. None can be specified for individual columns to retain the default foreground color.                          | `None`     |
+| `bg_colors`  | list                  | Background colors for the columns, in order. None can be specified for individual columns to retain the default background color.                          | `None`     |
+| **RETURNS**  | str                   | The formatted row.                                                                                                                                         |            |
 
 ### <kbd>class</kbd> `TracebackPrinter`
 
 Helper to output custom formatted tracebacks and error messages. Currently used
 in [Thinc](https://github.com/explosion/thinc).
 
 #### <kbd>method</kbd> `TracebackPrinter.__init__`
@@ -299,15 +299,16 @@
 | `*texts`    | str      | Optional texts to print (one per line).                                                    |         |
 | `highlight` | str      | Optional sequence to highlight in the traceback, e.g. the bad value that caused the error. | `False` |
 | `tb`        | iterable | The traceback, e.g. generated by `traceback.extract_stack()`.                              | `None`  |
 | **RETURNS** | str      | The formatted traceback. Can be printed or raised by custom exception.                     |         |
 
 ### <kbd>class</kbd> `MarkdownRenderer`
 
-Helper to create Markdown-formatted content. Will store the blocks added to the Markdown document in order.
+Helper to create Markdown-formatted content. Will store the blocks added to the
+Markdown document in order.
 
 ```python
 from wasabi import MarkdownRenderer
 
 md = MarkdownRenderer()
 md.add(md.title(1, "Hello world"))
 md.add("This is a paragraph")
```

### Comparing `wasabi-1.1.1/setup.cfg` & `wasabi-1.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.1.1
+version = 1.1.2
 description = A lightweight console printing and formatting toolkit
 url = https://github.com/explosion/wasabi
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `wasabi-1.1.1/wasabi/markdown.py` & `wasabi-1.1.2/wasabi/markdown.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/printer.py` & `wasabi-1.1.2/wasabi/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import os
 import sys
 import time
 import traceback
 from collections import Counter
 from contextlib import contextmanager
 from multiprocessing import Process
-from typing import Any, Collection, Dict, Optional, Union, cast
+from typing import Any, Collection, Dict, NoReturn, Optional, Union, cast, overload
 
+from .compat import Literal
 from .tables import row, table
 from .util import COLORS, ICONS, MESSAGES, can_render
 from .util import color as _color
 from .util import locale_escape, supports_ansi, wrap
 
 
 class Printer(object):
@@ -88,22 +89,44 @@
         spaced (bool): Whether to add newlines around the output.
         exits (Optional[int]): Optional toggle to perform a system exit.
         """
         return self._get_msg(
             title, text, style=MESSAGES.GOOD, show=show, spaced=spaced, exits=exits
         )
 
+    @overload
     def fail(
         self,
         title: Any = "",
         text: Any = "",
         show: bool = True,
         spaced: bool = False,
-        exits: Optional[int] = None,
+        exits: Optional[Literal[0, False]] = None,
     ):
+        ...
+
+    @overload
+    def fail(
+        self,
+        title: Any = "",
+        text: Any = "",
+        show: bool = True,
+        spaced: bool = False,
+        exits: Literal[1, True] = True,
+    ) -> NoReturn:
+        ...
+
+    def fail(
+        self,
+        title: Any = "",
+        text: Any = "",
+        show: bool = True,
+        spaced: bool = False,
+        exits: Optional[Union[int, bool]] = None,
+    ) -> Union[str, None, NoReturn]:
         """Print an error message.
 
         title (Any): The main text to print.
         text (Any): Optional additional text to print.
         show (bool): Whether to print or not. Can be used to only output
             messages under certain condition, e.g. if --verbose flag is set.
         spaced (bool): Whether to add newlines around the output.
```

### Comparing `wasabi-1.1.1/wasabi/tables.py` & `wasabi-1.1.2/wasabi/tables.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test-data/wasabi-test-notebook.ipynb` & `wasabi-1.1.2/wasabi/tests/test-data/wasabi-test-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test_jupyter.py` & `wasabi-1.1.2/wasabi/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test_markdown.py` & `wasabi-1.1.2/wasabi/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test_printer.py` & `wasabi-1.1.2/wasabi/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test_tables.py` & `wasabi-1.1.2/wasabi/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test_traceback.py` & `wasabi-1.1.2/wasabi/tests/test_traceback.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/tests/test_util.py` & `wasabi-1.1.2/wasabi/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/traceback_printer.py` & `wasabi-1.1.2/wasabi/traceback_printer.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi/util.py` & `wasabi-1.1.2/wasabi/util.py`

 * *Files identical despite different names*

### Comparing `wasabi-1.1.1/wasabi.egg-info/PKG-INFO` & `wasabi-1.1.2/wasabi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasabi
-Version: 1.1.1
+Version: 1.1.2
 Summary: A lightweight console printing and formatting toolkit
 Home-page: https://github.com/explosion/wasabi
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -19,15 +19,15 @@
 options, I've always ended up wanting something slightly different or slightly
 custom.
 
 This package is still a work in progress and aims to bundle those utilities in a
 standardised way so they can be shared across our other projects. It's super
 lightweight, has zero dependencies and works with Python 3.6+.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/1/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=1)
+[![tests](https://github.com/explosion/wasabi/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/wasabi/actions/workflows/tests.yml)
 [![PyPi](https://img.shields.io/pypi/v/wasabi.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/wasabi)
 [![conda](https://img.shields.io/conda/vn/conda-forge/wasabi.svg?style=flat-square&logo=conda-forge/logoColor=white)](https://anaconda.org/conda-forge/wasabi)
 [![GitHub](https://img.shields.io/github/release/ines/wasabi/all.svg?style=flat-square&logo=github)](https://github.com/ines/wasabi)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 <img width="609" src="https://user-images.githubusercontent.com/13643239/48663861-8c9ea000-ea96-11e8-8b04-d120c52276a8.png">
 
@@ -160,17 +160,17 @@
 msg = Printer()
 with msg.loading("Loading..."):
     # Do something here that takes longer
     time.sleep(10)
 msg.good("Successfully loaded something!")
 ```
 
-| Argument | Type | Description                        | Default           |
-| -------- | ---- | ---------------------------------- | ----------------- |
-| `text`   | str  | The text to display while loading. | `"Loading..."`    |
+| Argument | Type | Description                        | Default        |
+| -------- | ---- | ---------------------------------- | -------------- |
+| `text`   | str  | The text to display while loading. | `"Loading..."` |
 
 #### <kbd>method</kbd> `Printer.table`, `Printer.row`
 
 See [Tables](#tables).
 
 #### <kbd>property</kbd> `Printer.counts`
 
@@ -210,54 +210,54 @@
 ```
 Column 1   Column 2    Column 3
 --------   ---------   ----------
       a1      a2       a3
       b1      b2       b3
 ```
 
-| Argument    | Type                | Description                                                                                                                         | Default  |
-| ----------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | -------- |
-| `data`      | iterable / dict     | The data to render. Either a list of lists (one per row) or a dict for two-column tables.                                           |          |
-| `header`    | iterable            | Optional header columns.                                                                                                            | `None`   |
-| `footer`    | iterable            | Optional footer columns.                                                                                                            | `None`   |
-| `divider`   | bool                | Show a divider line between header/footer and body.                                                                                 | `False`  |
-| `widths`    | iterable / `"auto"` | Column widths in order. If `"auto"`, widths will be calculated automatically based on the largest value.                            | `"auto"` |
-| `max_col`   | int                 | Maximum column width.                                                                                                               | `30`     |
-| `spacing`   | int                 | Number of spaces between columns.                                                                                                   | `3`      |
-| `aligns`    | iterable / unicode  | Columns alignments in order. `"l"` (left, default), `"r"` (right) or `"c"` (center). If If a string, value is used for all columns. | `None`   |
-| `multiline` | bool                | If a cell value is a list of a tuple, render it on multiple lines, with one value per line.                                         | `False`  |
-| `env_prefix` | unicode                | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                         | `"WASABI"` |
-| `color_values` | dict                | Add or overwrite color values, name mapped to value.                                         | `None`   |
-| `fg_colors` | iterable                | Foreground colors, one per column. None can be specified for individual columns to retain the default background color. | `None`   |
-| `bg_colors` | iterable                | Background colors, one per column. None can be specified for individual columns to retain the default background color. | `None`   |
-| **RETURNS** | str                 | The formatted table.                                                                                                                |          |
+| Argument       | Type                | Description                                                                                                                         | Default    |
+| -------------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------- |
+| `data`         | iterable / dict     | The data to render. Either a list of lists (one per row) or a dict for two-column tables.                                           |            |
+| `header`       | iterable            | Optional header columns.                                                                                                            | `None`     |
+| `footer`       | iterable            | Optional footer columns.                                                                                                            | `None`     |
+| `divider`      | bool                | Show a divider line between header/footer and body.                                                                                 | `False`    |
+| `widths`       | iterable / `"auto"` | Column widths in order. If `"auto"`, widths will be calculated automatically based on the largest value.                            | `"auto"`   |
+| `max_col`      | int                 | Maximum column width.                                                                                                               | `30`       |
+| `spacing`      | int                 | Number of spaces between columns.                                                                                                   | `3`        |
+| `aligns`       | iterable / unicode  | Columns alignments in order. `"l"` (left, default), `"r"` (right) or `"c"` (center). If If a string, value is used for all columns. | `None`     |
+| `multiline`    | bool                | If a cell value is a list of a tuple, render it on multiple lines, with one value per line.                                         | `False`    |
+| `env_prefix`   | unicode             | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                                                         | `"WASABI"` |
+| `color_values` | dict                | Add or overwrite color values, name mapped to value.                                                                                | `None`     |
+| `fg_colors`    | iterable            | Foreground colors, one per column. None can be specified for individual columns to retain the default background color.             | `None`     |
+| `bg_colors`    | iterable            | Background colors, one per column. None can be specified for individual columns to retain the default background color.             | `None`     |
+| **RETURNS**    | str                 | The formatted table.                                                                                                                |            |
 
 #### <kbd>function</kbd> `row`
 
 ```python
 from wasabi import row
 
 data = ("a1", "a2", "a3")
 formatted = row(data)
 ```
 
 ```
 a1   a2   a3
 ```
 
-| Argument    | Type                      | Description                                                                                                                                                | Default  |
-| ----------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
-| `data`      | iterable                  | The individual columns to format.                                                                                                                          |          |
-| `widths`    | list / int / `"auto"` | Column widths, either one integer for all columns or an iterable of values. If "auto", widths will be calculated automatically based on the largest value. | `"auto"` |
-| `spacing`   | int                       | Number of spaces between columns.                                                                                                                          | `3`      |
-| `aligns`    | list                  | Columns alignments in order. `"l"` (left), `"r"` (right) or `"c"` (center).                                                                                | `None`   |
-| `env_prefix` | unicode                | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                         | `"WASABI"` |
-| `fg_colors`    | list                  | Foreground colors for the columns, in order. None can be specified for individual columns to retain the default foreground color. | `None`   |
-| `bg_colors`    | list                  | Background colors for the columns, in order. None can be specified for individual columns to retain the default background color. | `None`   |
-| **RETURNS** | str                       | The formatted row.                                                                                                                                         |          |
+| Argument     | Type                  | Description                                                                                                                                                | Default    |
+| ------------ | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
+| `data`       | iterable              | The individual columns to format.                                                                                                                          |            |
+| `widths`     | list / int / `"auto"` | Column widths, either one integer for all columns or an iterable of values. If "auto", widths will be calculated automatically based on the largest value. | `"auto"`   |
+| `spacing`    | int                   | Number of spaces between columns.                                                                                                                          | `3`        |
+| `aligns`     | list                  | Columns alignments in order. `"l"` (left), `"r"` (right) or `"c"` (center).                                                                                | `None`     |
+| `env_prefix` | unicode               | Prefix for environment variables, e.g. WASABI_LOG_FRIENDLY.                                                                                                | `"WASABI"` |
+| `fg_colors`  | list                  | Foreground colors for the columns, in order. None can be specified for individual columns to retain the default foreground color.                          | `None`     |
+| `bg_colors`  | list                  | Background colors for the columns, in order. None can be specified for individual columns to retain the default background color.                          | `None`     |
+| **RETURNS**  | str                   | The formatted row.                                                                                                                                         |            |
 
 ### <kbd>class</kbd> `TracebackPrinter`
 
 Helper to output custom formatted tracebacks and error messages. Currently used
 in [Thinc](https://github.com/explosion/thinc).
 
 #### <kbd>method</kbd> `TracebackPrinter.__init__`
@@ -311,15 +311,16 @@
 | `*texts`    | str      | Optional texts to print (one per line).                                                    |         |
 | `highlight` | str      | Optional sequence to highlight in the traceback, e.g. the bad value that caused the error. | `False` |
 | `tb`        | iterable | The traceback, e.g. generated by `traceback.extract_stack()`.                              | `None`  |
 | **RETURNS** | str      | The formatted traceback. Can be printed or raised by custom exception.                     |         |
 
 ### <kbd>class</kbd> `MarkdownRenderer`
 
-Helper to create Markdown-formatted content. Will store the blocks added to the Markdown document in order.
+Helper to create Markdown-formatted content. Will store the blocks added to the
+Markdown document in order.
 
 ```python
 from wasabi import MarkdownRenderer
 
 md = MarkdownRenderer()
 md.add(md.title(1, "Hello world"))
 md.add("This is a paragraph")
```

### Comparing `wasabi-1.1.1/wasabi.egg-info/SOURCES.txt` & `wasabi-1.1.2/wasabi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

