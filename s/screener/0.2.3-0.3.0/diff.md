# Comparing `tmp/screener-0.2.3.tar.gz` & `tmp/screener-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screener-0.2.3.tar", max compression
+gzip compressed data, was "screener-0.3.0.tar", max compression
```

## Comparing `screener-0.2.3.tar` & `screener-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1866 2023-05-23 18:42:05.097804 screener-0.2.3/README.md
--rw-r--r--   0        0        0     2451 2023-05-23 18:56:40.870037 screener-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.2.3/screener/__init__.py
--rw-r--r--   0        0        0     1839 2023-05-23 18:56:40.885037 screener-0.2.3/screener/__main__.py
--rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.2.3/screener/parser/__init__.py
--rw-r--r--   0        0        0      727 2023-05-21 20:35:22.715235 screener-0.2.3/screener/parser/epub.py
--rw-r--r--   0        0        0      809 2023-05-22 09:42:14.086332 screener-0.2.3/screener/parser/kindle.py
--rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.2.3/screener/reader/__init__.py
--rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.2.3/screener/reader/abstract.py
--rw-r--r--   0        0        0      877 2023-05-22 10:19:24.692693 screener-0.2.3/screener/reader/epub.py
--rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.2.3/screener/reader/kindle.py
--rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.2.3/screener/utils.py
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 screener-0.2.3/setup.py
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 screener-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1919 2023-06-07 19:00:57.528329 screener-0.3.0/README.md
+-rw-r--r--   0        0        0     2452 2023-06-07 19:00:57.535328 screener-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.3.0/screener/__init__.py
+-rw-r--r--   0        0        0     2598 2023-06-07 19:00:57.535328 screener-0.3.0/screener/__main__.py
+-rw-r--r--   0        0        0      554 2023-06-07 19:00:57.535328 screener-0.3.0/screener/diagnostic.py
+-rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.3.0/screener/parser/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-07 19:00:57.535328 screener-0.3.0/screener/parser/epub.py
+-rw-r--r--   0        0        0     1332 2023-06-07 19:00:57.535328 screener-0.3.0/screener/parser/kindle.py
+-rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.3.0/screener/reader/__init__.py
+-rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.3.0/screener/reader/abstract.py
+-rw-r--r--   0        0        0      796 2023-06-07 19:00:57.535328 screener-0.3.0/screener/reader/epub.py
+-rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.3.0/screener/reader/kindle.py
+-rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.3.0/screener/utils.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 screener-0.3.0/setup.py
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 screener-0.3.0/PKG-INFO
```

### Comparing `screener-0.2.3/README.md` & `screener-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ```bash
 pip install screener
 ```
 
 #### Development installation
 
-To install Screener for development, clone the repository and run:
+To install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:
 
 ```bash
 poetry install
 ```
 
 ## Contributing
```

### Comparing `screener-0.2.3/pyproject.toml` & `screener-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "Screener"
-version = "0.2.3"
+version = "0.3.0"
 description = "Check e-book files for security and privacy issues."
 authors = ["Tom Kuson <mail@tjkuson.me>"]
-license = "GPL-3.0-only"
+license = "LGPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "screener", from = "." },
 ]
 repository = "https://github.com/tjkuson/screener/"
 keywords = ["ebook", "security", "privacy", "epub", "mobi", "kindle"]
 classifiers = [
@@ -23,15 +23,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 mypy = "^1.2.0"
 types-beautifulsoup4 = "^4.12.0.5"
-ruff = "^0.0.269"
+ruff = "^0.0.271"
 ssort = "^0.11.6"
 
 [tool.black]
 line-length = 88
 target-version = ["py310"]
 
 [tool.ruff]
```

### Comparing `screener-0.2.3/screener/__main__.py` & `screener-0.3.0/screener/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Screener entry-point script."""
 
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 
+from screener.diagnostic import (
+    ExternalImageDiagnostic,
+    JavaScriptDiagnostic,
+    ParseErrorDiagnostic,
+)
 from screener.parser import parse_epub, parse_kindle
 from screener.reader import EpubFileReader, KindleFileReader
 
 
 def init_argparse() -> ArgumentParser:
     """Create argument parser for system args."""
     parser = ArgumentParser(
@@ -15,43 +20,56 @@
         usage="%(prog)s [OPTION] [FILE]...",
         description="Check e-book files for security and privacy issues.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
-        version=f"{parser.prog} version 0.2.3",
+        version=f"{parser.prog} version 0.3.0",
     )
     parser.add_argument("files", nargs="*")
     return parser
 
 
+def check_file(
+    file: Path,
+) -> JavaScriptDiagnostic | ExternalImageDiagnostic | ParseErrorDiagnostic | None:
+    """Check file."""
+    try:
+        extension = file.suffix
+        match extension:
+            case ".epub":
+                with EpubFileReader(file) as epub:
+                    return parse_epub(epub.file_path)
+            case ".azw3", ".mobi":
+                with KindleFileReader(file) as azw3:
+                    return parse_kindle(azw3.file_path)
+        return ParseErrorDiagnostic(file.name, f"unknown file extension: {extension}")
+    except (FileNotFoundError, IsADirectoryError) as exc:
+        print(f"{sys.argv[0]}: {file}: {exc.strerror}", file=sys.stderr)
+        return ParseErrorDiagnostic(file.name, exc.strerror)
+
+
 def main() -> None:
     """Read system args and check e-book files."""
     parser = init_argparse()
     args = parser.parse_args()
     if not args.files:
-        print("no file input")
+        print("No files specified. Run with -h for help.", file=sys.stderr)
     for file in args.files:
         if file == "-":
-            print("stdin not supported")
+            print("stdin not supported", file=sys.stderr)
             continue
-        try:
-            extension = Path(file).suffix
-            is_safe = True
-            match extension:
-                case ".epub":
-                    with EpubFileReader(file) as epub:
-                        is_safe = parse_epub(epub.file_path)
-                case ".azw3", ".mobi":
-                    with KindleFileReader(file) as azw3:
-                        is_safe = parse_kindle(azw3.file_path)
-            if is_safe:
-                print(f"No JavaScript/external images detected in {file}")
-            else:
-                print(f"JavaScript/external images detected in {file}!")
-        except (FileNotFoundError, IsADirectoryError) as exc:
-            print(f"{sys.argv[0]}: {file}: {exc.strerror}", file=sys.stderr)
+        diagnostic = check_file(Path(file))
+        match diagnostic:
+            case JavaScriptDiagnostic(file_path):
+                print(f"{file_path}: contains JavaScript", file=sys.stderr)
+            case ExternalImageDiagnostic(file_path):
+                print(f"{file_path}: contains external images", file=sys.stderr)
+            case ParseErrorDiagnostic(file_path, msg):
+                print(f"{file_path}: could not be parsed ({msg})", file=sys.stderr)
+            case None:
+                print(f"{file}: safe", file=sys.stderr)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `screener-0.2.3/screener/parser/epub.py` & `screener-0.3.0/screener/parser/epub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Parse epub file to check that it is safe."""
 
 from pathlib import Path
 
 from ebooklib import ITEM_DOCUMENT
 
+from screener.diagnostic import ExternalImageDiagnostic, JavaScriptDiagnostic
 from screener.reader import EpubFileReader
 from screener.utils import (
     html_contains_images_with_external_sources,
     html_contains_javascript,
 )
 
 
-def parse_epub(path_to_epub: Path) -> bool:
+def parse_epub(
+    path_to_epub: Path,
+) -> JavaScriptDiagnostic | ExternalImageDiagnostic | None:
     """Parse epub to check that it is safe."""
     with EpubFileReader(path_to_epub) as epub:
         for item in epub.book.get_items_of_type(ITEM_DOCUMENT):
             content = item.get_content()
             if html_contains_javascript(content):
-                return False
+                return JavaScriptDiagnostic(path_to_epub.name)
             if html_contains_images_with_external_sources(content):
-                return False
-        return True
+                return ExternalImageDiagnostic(path_to_epub.name)
+        return None
```

### Comparing `screener-0.2.3/screener/reader/abstract.py` & `screener-0.3.0/screener/reader/abstract.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.3/screener/reader/epub.py` & `screener-0.3.0/screener/reader/epub.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,12 @@
 
     def __init__(self: EpubFileReader, file_path: Path) -> None:
         """Initialize the class."""
         super().__init__(file_path)
 
     def __enter__(self: EpubFileReader) -> EpubFileReader:
         """Runtime context."""
-        print("Reading epub file")
         with warnings.catch_warnings():
             # Have to do this because of bug in ebooklib
             warnings.simplefilter("ignore")
             self.book = epub.read_epub(self.file_path, options={"ignore_ncx": False})
-        print("Finished reading epub file")
         return self
```

### Comparing `screener-0.2.3/screener/reader/kindle.py` & `screener-0.3.0/screener/reader/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.3/screener/utils.py` & `screener-0.3.0/screener/utils.py`

 * *Files identical despite different names*

### Comparing `screener-0.2.3/setup.py` & `screener-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['EbookLib>=0.18,<0.19', 'beautifulsoup4>=4.12.2,<5.0.0', 'mobi>=0.3.3,<0.4.0']
 
 setup_kwargs = {
     'name': 'screener',
-    'version': '0.2.3',
+    'version': '0.3.0',
     'description': 'Check e-book files for security and privacy issues.',
-    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n_Screener is currently in early development. Please consider contributing if you have the time and know-how!_\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreen is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
+    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n_Screener is currently in early development. Please consider contributing if you have the time and know-how!_\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreen is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
     'author': 'Tom Kuson',
     'author_email': 'mail@tjkuson.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tjkuson/screener/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `screener-0.2.3/PKG-INFO` & `screener-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: screener
-Version: 0.2.3
+Version: 0.3.0
 Summary: Check e-book files for security and privacy issues.
 Home-page: https://github.com/tjkuson/screener/
-License: GPL-3.0-only
+License: LGPL-3.0-only
 Keywords: ebook,security,privacy,epub,mobi,kindle
 Author: Tom Kuson
 Author-email: mail@tjkuson.me
 Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: EbookLib (>=0.18,<0.19)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
@@ -52,15 +52,15 @@
 
 ```bash
 pip install screener
 ```
 
 #### Development installation
 
-To install Screener for development, clone the repository and run:
+To install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:
 
 ```bash
 poetry install
 ```
 
 ## Contributing
```

