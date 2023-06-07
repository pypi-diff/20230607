# Comparing `tmp/screener-0.3.1.tar.gz` & `tmp/screener-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screener-0.3.1.tar", max compression
+gzip compressed data, was "screener-0.3.2.tar", max compression
```

## Comparing `screener-0.3.1.tar` & `screener-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1919 2023-06-07 19:00:57.528329 screener-0.3.1/README.md
--rw-r--r--   0        0        0     2509 2023-06-07 19:21:33.590229 screener-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.3.1/screener/__init__.py
--rw-r--r--   0        0        0     2614 2023-06-07 19:21:33.590229 screener-0.3.1/screener/__main__.py
--rw-r--r--   0        0        0      554 2023-06-07 19:00:57.535328 screener-0.3.1/screener/diagnostic.py
--rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.3.1/screener/parser/__init__.py
--rw-r--r--   0        0        0      935 2023-06-07 19:00:57.535328 screener-0.3.1/screener/parser/epub.py
--rw-r--r--   0        0        0     1332 2023-06-07 19:00:57.535328 screener-0.3.1/screener/parser/kindle.py
--rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.3.1/screener/reader/__init__.py
--rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.3.1/screener/reader/abstract.py
--rw-r--r--   0        0        0      796 2023-06-07 19:00:57.535328 screener-0.3.1/screener/reader/epub.py
--rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.3.1/screener/reader/kindle.py
--rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.3.1/screener/utils.py
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 screener-0.3.1/setup.py
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 screener-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1919 2023-06-07 19:00:57.528329 screener-0.3.2/README.md
+-rw-r--r--   0        0        0     2514 2023-06-07 19:35:11.668394 screener-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.3.2/screener/__init__.py
+-rw-r--r--   0        0        0     2614 2023-06-07 19:35:11.668394 screener-0.3.2/screener/__main__.py
+-rw-r--r--   0        0        0      554 2023-06-07 19:00:57.535328 screener-0.3.2/screener/diagnostic.py
+-rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.3.2/screener/parser/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-07 19:00:57.535328 screener-0.3.2/screener/parser/epub.py
+-rw-r--r--   0        0        0     1332 2023-06-07 19:00:57.535328 screener-0.3.2/screener/parser/kindle.py
+-rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.3.2/screener/reader/__init__.py
+-rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.3.2/screener/reader/abstract.py
+-rw-r--r--   0        0        0      796 2023-06-07 19:00:57.535328 screener-0.3.2/screener/reader/epub.py
+-rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.3.2/screener/reader/kindle.py
+-rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.3.2/screener/utils.py
+-rw-r--r--   0        0        0     2848 1970-01-01 00:00:00.000000 screener-0.3.2/setup.py
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 screener-0.3.2/PKG-INFO
```

### Comparing `screener-0.3.1/README.md` & `screener-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/pyproject.toml` & `screener-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Screener"
-version = "0.3.1"
+version = "0.3.2"
 description = "Check e-book files for security and privacy issues."
 authors = ["Tom Kuson <mail@tjkuson.me>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "screener", from = "." },
 ]
@@ -84,12 +84,12 @@
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["ebooklib", "ebooklib.epub", "mobi", "kindle"]
 ignore_missing_imports = true
 
 [tool.poetry.scripts]
-screener = "screener:__main__"
+screener = "screener.__main__:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `screener-0.3.1/screener/__main__.py` & `screener-0.3.2/screener/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         usage="%(prog)s [OPTION] [FILE]...",
         description="Check e-book files for security and privacy issues.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
-        version=f"{parser.prog} version 0.3.1",
+        version=f"{parser.prog} version 0.3.2",
     )
     parser.add_argument("files", nargs="*")
     return parser
 
 
 def check_file(
     file: Path,
```

### Comparing `screener-0.3.1/screener/diagnostic.py` & `screener-0.3.2/screener/diagnostic.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/screener/parser/epub.py` & `screener-0.3.2/screener/parser/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/screener/parser/kindle.py` & `screener-0.3.2/screener/parser/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/screener/reader/abstract.py` & `screener-0.3.2/screener/reader/abstract.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/screener/reader/epub.py` & `screener-0.3.2/screener/reader/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/screener/reader/kindle.py` & `screener-0.3.2/screener/reader/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/screener/utils.py` & `screener-0.3.2/screener/utils.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.1/setup.py` & `screener-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['EbookLib>=0.18,<0.19', 'beautifulsoup4>=4.12.2,<5.0.0', 'mobi>=0.3.3,<0.4.0']
 
 entry_points = \
-{'console_scripts': ['screener = screener:__main__']}
+{'console_scripts': ['screener = screener.__main__:main']}
 
 setup_kwargs = {
     'name': 'screener',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Check e-book files for security and privacy issues.',
     'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n_Screener is currently in early development. Please consider contributing if you have the time and know-how!_\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreen is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
     'author': 'Tom Kuson',
     'author_email': 'mail@tjkuson.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tjkuson/screener/',
```

### Comparing `screener-0.3.1/PKG-INFO` & `screener-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screener
-Version: 0.3.1
+Version: 0.3.2
 Summary: Check e-book files for security and privacy issues.
 Home-page: https://github.com/tjkuson/screener/
 License: LGPL-3.0-only
 Keywords: ebook,security,privacy,epub,mobi,kindle
 Author: Tom Kuson
 Author-email: mail@tjkuson.me
 Requires-Python: >=3.10,<4.0
```

