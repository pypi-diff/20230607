# Comparing `tmp/epub2txt-0.1.2a0.tar.gz` & `tmp/epub2txt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epub2txt-0.1.2a0.tar", max compression
+gzip compressed data, was "epub2txt-0.1.3.tar", max compression
```

## Comparing `epub2txt-0.1.2a0.tar` & `epub2txt-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2022-06-19 07:24:18.495484 epub2txt-0.1.2a0/epub2txt/__init__.py
--rw-r--r--   0        0        0     4740 2022-06-19 07:23:06.171912 epub2txt-0.1.2a0/epub2txt/__main__.py
--rw-r--r--   0        0        0      797 2021-02-07 16:14:03.598152 epub2txt-0.1.2a0/epub2txt/browse_filename.py
--rw-r--r--   0        0        0     3956 2021-02-08 02:36:44.014012 epub2txt-0.1.2a0/epub2txt/epub2txt.py
--rw-r--r--   0        0        0     1357 2021-02-07 17:17:09.586500 epub2txt-0.1.2a0/epub2txt/gen_filename.py
--rw-r--r--   0        0        0     1091 2021-02-07 07:51:04.577682 epub2txt-0.1.2a0/LICENSE
--rw-r--r--   0        0        0      579 2022-06-19 07:24:08.317917 epub2txt-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0     1587 2021-02-08 02:52:25.198192 epub2txt-0.1.2a0/README.md
--rw-r--r--   0        0        0     2449 2022-06-19 07:27:02.455151 epub2txt-0.1.2a0/setup.py
--rw-r--r--   0        0        0     2349 2022-06-19 07:27:02.455151 epub2txt-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-06-07 01:46:44.620780 epub2txt-0.1.3/epub2txt/__init__.py
+-rw-r--r--   0        0        0     4740 2022-06-19 07:23:06.171912 epub2txt-0.1.3/epub2txt/__main__.py
+-rw-r--r--   0        0        0      797 2021-02-07 16:14:03.598152 epub2txt-0.1.3/epub2txt/browse_filename.py
+-rw-r--r--   0        0        0     4088 2023-06-07 01:42:11.681117 epub2txt-0.1.3/epub2txt/epub2txt.py
+-rw-r--r--   0        0        0     1357 2021-02-07 17:17:09.586500 epub2txt-0.1.3/epub2txt/gen_filename.py
+-rw-r--r--   0        0        0     1091 2021-02-07 07:51:04.577682 epub2txt-0.1.3/LICENSE
+-rw-r--r--   0        0        0      614 2023-06-07 01:46:38.818096 epub2txt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1587 2021-02-08 02:52:25.198192 epub2txt-0.1.3/README.md
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 epub2txt-0.1.3/setup.py
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 epub2txt-0.1.3/PKG-INFO
```

### Comparing `epub2txt-0.1.2a0/epub2txt/__main__.py` & `epub2txt-0.1.3/epub2txt/__main__.py`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.2a0/epub2txt/browse_filename.py` & `epub2txt-0.1.3/epub2txt/browse_filename.py`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.2a0/epub2txt/epub2txt.py` & `epub2txt-0.1.3/epub2txt/epub2txt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """Convert epub to text."""
-# pylint:
-
-from typing import Any, Callable, List, Union
+# pylint: disable=invalid-name, too-many-branches, too-many-statements, broad-except, deprecated-class
 
 from pathlib import Path
+from typing import Any, Callable, List, Union
 
-# for with_func_attrs
-# from typing import Iterable
-from collections import Iterable  # < py38
+try:
+    from collections.abc import Iterable  # python 3.10+
+except ImportError:
+    from collections import Iterable  # python < 3.10
 
 # the rest
-from itertools import zip_longest
-import httpx
 import io
-from lxml import etree
-from ebooklib import epub
+from itertools import zip_longest
 
+import httpx
 import logzero
+from ebooklib import epub
 from logzero import logger
+from lxml import etree
 
 
 def with_func_attrs(**attrs: Any) -> Callable:
-    '''Deco with_func_attrs.'''
+    """Deco with_func_attrs."""
+
     def with_attrs(fct: Callable) -> Callable:
         for key, val in attrs.items():
             setattr(fct, key, val)
         return fct
+
     return with_attrs
 
 
 def flatten_iter(items):
     """Yield items from any nested iterable; see Reference."""
     for x in items:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
@@ -58,15 +60,15 @@
     """
     if debug:
         logzero.loglevel(10)
     else:
         logzero.loglevel(20)
 
     # process possible url
-    if filepath.__str__().startswith("http"):
+    if str(filepath).startswith("http"):
         try:
             resp = httpx.get(filepath, timeout=30)
             resp.raise_for_status()
         except Exception as exc:
             logger.error("httpx.get(%s) exc: %s", filepath, exc)
             raise
         cont = io.BytesIO(resp.content)
```

### Comparing `epub2txt-0.1.2a0/epub2txt/gen_filename.py` & `epub2txt-0.1.3/epub2txt/gen_filename.py`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.2a0/LICENSE` & `epub2txt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.2a0/README.md` & `epub2txt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `epub2txt-0.1.2a0/setup.py` & `epub2txt-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['absl-py>=0.11.0,<0.12.0',
  'ebooklib>=0.17.1,<0.18.0',
- 'httpx>=0.16.1,<0.17.0',
+ 'httpx',
  'logzero>=1.6.3,<2.0.0',
  'tqdm>=4.56.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['epub2txt = epub2txt.__main__:main']}
 
 setup_kwargs = {
     'name': 'epub2txt',
-    'version': '0.1.2a0',
+    'version': '0.1.3',
     'description': 'Convert epub to txt with additonal utils',
     'long_description': '# epub2txt [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05c422da73a14c23b87b0657af9c8df7)](https://www.codacy.com/gh/ffreemt/epub2txt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ffreemt/epub2txt&amp;utm_campaign=Badge_Grade)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/epub2txt.svg)](https://badge.fury.io/py/epub2txt)\n\nConvert epub to txt with additonal utils\n\n<!--- Refer to dualtext-epub\\der_fanger_de_en.py\n\t\t__main__.py refer to tmx2epub.__main__\n--->\n\n## Installation\n\n```bash\npip install epub2txt\n# pip install epub2txt -U  # to upgrade\n```\n\n## Usage\n\n### From command line\n\n```bash\n# convert test.epub to test.txt\nepub2txt -f test.epub\n\n# browse for epub file, txt file will be in the same directory as the epub file\nepub2txt\n\n# show epub book info: title and toc\nepub2txt -i\n\n# show more epub book info: title, toc, metadata, spine (list of stuff packed into the epub)\nepub2txt -m\n\n# show epub2txt version\nepub2txt -V\n\n```\n\n### `python` code\n\n```python\nfrom epub2txt import epub2txt\n# from a url to epub\nurl = "https://github.com/ffreemt/tmx2epub/raw/master/tests/1.tmx.epub"\nres = epub2txt(url)\n\n# from a local epub file\nfilepath = r"tests\\test.epub"\nres = epub2txt(filepath)\n\n```\n\n## TODO\n*   Extract a single chapter\n*   Batch conversion of several epub files\n\n',
     'author': 'freemt',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/ffreemt/epub2txt',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `epub2txt-0.1.2a0/PKG-INFO` & `epub2txt-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: epub2txt
-Version: 0.1.2a0
+Version: 0.1.3
 Summary: Convert epub to txt with additonal utils
 Home-page: https://github.com/ffreemt/epub2txt
 License: MIT
 Author: freemt
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: absl-py (>=0.11.0,<0.12.0)
 Requires-Dist: ebooklib (>=0.17.1,<0.18.0)
-Requires-Dist: httpx (>=0.16.1,<0.17.0)
+Requires-Dist: httpx
 Requires-Dist: logzero (>=1.6.3,<2.0.0)
 Requires-Dist: tqdm (>=4.56.0,<5.0.0)
 Project-URL: Repository, https://github.com/ffreemt/epub2txt
 Description-Content-Type: text/markdown
 
 # epub2txt [![Codacy Badge](https://app.codacy.com/project/badge/Grade/05c422da73a14c23b87b0657af9c8df7)](https://www.codacy.com/gh/ffreemt/epub2txt/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ffreemt/epub2txt&amp;utm_campaign=Badge_Grade)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/epub2txt.svg)](https://badge.fury.io/py/epub2txt)
```

