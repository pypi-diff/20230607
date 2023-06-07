# Comparing `tmp/pytest-watcher-0.3.1.tar.gz` & `tmp/pytest_watcher-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-watcher-0.3.1.tar", max compression
+gzip compressed data, was "pytest_watcher-0.3.2.tar", max compression
```

## Comparing `pytest-watcher-0.3.1.tar` & `pytest_watcher-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-10-19 14:45:40.729543 pytest-watcher-0.3.1/LICENSE
--rw-r--r--   0        0        0     3330 2023-06-03 11:43:02.936615 pytest-watcher-0.3.1/README.md
--rw-r--r--   0        0        0     1563 2023-06-03 13:13:33.406945 pytest-watcher-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-03 12:47:15.872901 pytest-watcher-0.3.1/pytest_watcher/__init__.py
--rw-r--r--   0        0        0       81 2022-10-19 14:45:40.730627 pytest-watcher-0.3.1/pytest_watcher/__main__.py
--rw-r--r--   0        0        0     5043 2023-06-03 13:11:24.681213 pytest-watcher-0.3.1/pytest_watcher/watcher.py
--rw-r--r--   0        0        0     4312 2023-06-03 13:14:04.349757 pytest-watcher-0.3.1/setup.py
--rw-r--r--   0        0        0     4378 2023-06-03 13:14:04.349935 pytest-watcher-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3330 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/README.md
+-rw-r--r--   0        0        0     1563 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pytest_watcher/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pytest_watcher/__main__.py
+-rw-r--r--   0        0        0     5163 2023-06-07 19:08:57.493555 pytest_watcher-0.3.2/pytest_watcher/watcher.py
+-rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 pytest_watcher-0.3.2/PKG-INFO
```

### Comparing `pytest-watcher-0.3.1/LICENSE` & `pytest_watcher-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-watcher-0.3.1/README.md` & `pytest_watcher-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-watcher-0.3.1/pyproject.toml` & `pytest_watcher-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-watcher"
-version = "0.3.1"
+version = "0.3.2"
 description = "Automatically rerun your tests on file modifications"
 authors = ["Olzhas Arystanov <o.arystanov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/olzhasar/pytest-watcher"
 repository = "https://github.com/olzhasar/pytest-watcher"
 keywords = ["pytest", "watch", "watcher"]
```

### Comparing `pytest-watcher-0.3.1/pytest_watcher/watcher.py` & `pytest_watcher-0.3.2/pytest_watcher/watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import subprocess
 import sys
 import threading
 import time
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import List, Sequence
+from typing import List, Optional, Sequence
 
 from watchdog import events
 from watchdog.observers import Observer
 from watchdog.utils.patterns import match_any_paths
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 DEFAULT_DELAY = 0.2
+LOOP_DELAY = 0.1
 
 trigger_lock = threading.Lock()
 trigger = None
 
 
 logging.basicConfig(level=logging.INFO, format="[ptw] %(message)s")
 logger = logging.getLogger(__name__)
@@ -50,15 +51,19 @@
     EVENTS_WATCHED = {
         events.EVENT_TYPE_CREATED,
         events.EVENT_TYPE_DELETED,
         events.EVENT_TYPE_MODIFIED,
         events.EVENT_TYPE_MOVED,
     }
 
-    def __init__(self, patterns: List[str] = None, ignore_patterns: List[str] = None):
+    def __init__(
+        self,
+        patterns: Optional[List[str]] = None,
+        ignore_patterns: Optional[List[str]] = None,
+    ):
         self._patterns = patterns or ["*.py"]
         self._ignore_patterns = ignore_patterns or []
 
     @property
     def patterns(self) -> List[str]:
         return self._patterns
 
@@ -85,19 +90,18 @@
             logger.debug(f"IGNORED event: {event.event_type} src: {event.src_path}")
 
 
 def _invoke_runner(runner: str, args: Sequence[str]) -> None:
     subprocess.run([runner, *args])
 
 
-def _parse_patterns(arg: str):
-    return arg.split(",")
+def parse_arguments(args: Sequence[str]) -> ParsedArguments:
+    def _parse_patterns(arg: str):
+        return arg.split(",")
 
-
-def _parse_arguments(args: Sequence[str]) -> ParsedArguments:
     parser = argparse.ArgumentParser(
         prog="pytest_watcher",
         description="""
             Watch the <path> for file changes and trigger the test runner (pytest).\n
             Additional arguments are passed directly to the test runner.
         """,
     )
@@ -125,43 +129,44 @@
     )
     parser.add_argument(
         "--ignore-patterns",
         default=[],
         type=_parse_patterns,
         help="File patterns to ignore, specified as comma-separated Unix-style patterns (default: '')",
     )
+    parser.add_argument("--version", action="version", version=VERSION)
 
     namespace, runner_args = parser.parse_known_args(args)
 
     return ParsedArguments(
         path=namespace.path,
         now=namespace.now,
         delay=namespace.delay,
         runner=namespace.runner,
         patterns=namespace.patterns,
         ignore_patterns=namespace.ignore_patterns,
         runner_args=runner_args,
     )
 
 
-def _run_main_loop(*, runner: str, runner_args: Sequence[str], delay: float) -> None:
+def main_loop(*, runner: str, runner_args: Sequence[str], delay: float) -> None:
     global trigger
 
     now = datetime.now()
     if trigger and now - trigger > timedelta(seconds=delay):
         _invoke_runner(runner, runner_args)
 
         with trigger_lock:
             trigger = None
 
-    time.sleep(delay)
+    time.sleep(LOOP_DELAY)
 
 
 def run():
-    args = _parse_arguments(sys.argv[1:])
+    args = parse_arguments(sys.argv[1:])
 
     event_handler = EventHandler(
         patterns=args.patterns, ignore_patterns=args.ignore_patterns
     )
 
     observer = Observer()
 
@@ -173,13 +178,11 @@
     sys.stdout.write(f"Waiting for file changes in {args.path.absolute()}\n")
 
     if args.now:
         emit_trigger()
 
     try:
         while True:
-            _run_main_loop(
-                runner=args.runner, runner_args=args.runner_args, delay=args.delay
-            )
+            main_loop(runner=args.runner, runner_args=args.runner_args, delay=args.delay)
     finally:
         observer.stop()
         observer.join()
```

### Comparing `pytest-watcher-0.3.1/setup.py` & `pytest_watcher-0.3.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,152 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-watcher
+Version: 0.3.2
+Summary: Automatically rerun your tests on file modifications
+Home-page: https://github.com/olzhasar/pytest-watcher
+License: MIT
+Keywords: pytest,watch,watcher
+Author: Olzhas Arystanov
+Author-email: o.arystanov@gmail.com
+Requires-Python: >=3.7.0,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Dist: watchdog (>=2.0.0)
+Project-URL: Repository, https://github.com/olzhasar/pytest-watcher
+Description-Content-Type: text/markdown
 
-packages = \
-['pytest_watcher']
+# A simple watcher for pytest
 
-package_data = \
-{'': ['*']}
+[![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
+[![GitHub](https://img.shields.io/github/license/olzhasar/pytest-watcher)](https://github.com/olzhasar/pytest-watcher/blob/master/LICENSE)
 
-install_requires = \
-['watchdog>=2.0.0']
-
-entry_points = \
-{'console_scripts': ['ptw = pytest_watcher:run',
-                     'pytest-watcher = pytest_watcher:run']}
-
-setup_kwargs = {
-    'name': 'pytest-watcher',
-    'version': '0.3.1',
-    'description': 'Automatically rerun your tests on file modifications',
-    'long_description': '# A simple watcher for pytest\n\n[![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)\n[![GitHub](https://img.shields.io/github/license/olzhasar/pytest-watcher)](https://github.com/olzhasar/pytest-watcher/blob/master/LICENSE)\n\n## Overview\n\n**pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.\n\nWorks on Unix (Linux, MacOS, BSD) and Windows.\n\n## Table of Contents\n\n- [Motivation](#motivation)\n- [File Events](#file-events)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Using a different test runner](#using-a-different-test-runner)\n- [Watching different patterns](#watching-different-patterns)\n- [Delay](#delay)\n- [Compatibility](#compatibility)\n- [License](#license)\n\n## Motivation\n\n### Why not general tools (e.g. `watchmedo`, `entr`)?\n\n- Easy to use and remember\n- Works for most python projects out of the box\n- Minimum dependencies (`watchdog` is the only one)\n- Handles post-processing properly (see [delay](#delay))\n\n### What about pytest-watch?\n\n[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.\n\n## File events\n\nBy default `pytest-watcher` looks for the following events:\n\n- New `*.py` file created\n- Existing `*.py` file modified\n- Existing `*.py` file deleted\n- A `*.py` file moved either from or to the watched path\n\nYou can specify alternative file patterns to watch. See [Watching different patterns](#watching-different-patterns)\n\n## Installation\n\n```sh\npip install pytest-watcher\n```\n\n## Usage\n\nSpecify the path that you want to monitor:\n\n```sh\nptw .\n```\n\nor\n\n```sh\nptw /home/repos/project\n```\n\nAny arguments after `<path>` will be passed to the test runner (which is `pytest` by default). For example:\n\n```sh\nptw . -x --lf --nf\n```\n\nwill call `pytest` with the following arguments:\n\n```sh\npytest -x --lf --nf\n```\n\n## Using a different test runner\n\nYou can specify an alternative test runner using the `--runner` flag:\n\n```sh\nptw . --runner tox\n```\n\n## Watching different patterns\n\nYou can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\\*.py".\n\nExample:\n\n```sh\nptw . --patterns \'*.py,pyproject.toml\'\n```\n\nYou can also **ignore** certain patterns using the `--ignore-patterns` flag:\n\n```sh\nptw . --ignore-patterns \'settings.py,db.py\'\n```\n\n## Delay\n\n`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.\n\nYou can control the actual delay value with the `--delay` flag:\n\n`ptw . --delay 0.2`\n\nTo disable the delay altogether, you can provide zero as a value:\n\n`ptw . --delay 0`\n\n## Compatibility\n\nThe code is tested for Python versions 3.7+\n\n## License\n\nThis project is licensed under the [MIT License](LICENSE).\n',
-    'author': 'Olzhas Arystanov',
-    'author_email': 'o.arystanov@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/olzhasar/pytest-watcher',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.0,<4.0.0',
-}
+## Overview
 
+**pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.
+
+Works on Unix (Linux, MacOS, BSD) and Windows.
+
+## Table of Contents
+
+- [Motivation](#motivation)
+- [File Events](#file-events)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Using a different test runner](#using-a-different-test-runner)
+- [Watching different patterns](#watching-different-patterns)
+- [Delay](#delay)
+- [Compatibility](#compatibility)
+- [License](#license)
+
+## Motivation
+
+### Why not general tools (e.g. `watchmedo`, `entr`)?
+
+- Easy to use and remember
+- Works for most python projects out of the box
+- Minimum dependencies (`watchdog` is the only one)
+- Handles post-processing properly (see [delay](#delay))
+
+### What about pytest-watch?
+
+[pytest-watch](https://github.com/joeyespo/pytest-watch) has been around for a long time and used to address exactly this problem. Unfortunately, pytest-watch is no longer maintained and does not work for many users. To provide a substitute, I developed this tool.
+
+## File events
+
+By default `pytest-watcher` looks for the following events:
+
+- New `*.py` file created
+- Existing `*.py` file modified
+- Existing `*.py` file deleted
+- A `*.py` file moved either from or to the watched path
+
+You can specify alternative file patterns to watch. See [Watching different patterns](#watching-different-patterns)
+
+## Installation
+
+```sh
+pip install pytest-watcher
+```
+
+## Usage
+
+Specify the path that you want to monitor:
+
+```sh
+ptw .
+```
+
+or
+
+```sh
+ptw /home/repos/project
+```
+
+Any arguments after `<path>` will be passed to the test runner (which is `pytest` by default). For example:
+
+```sh
+ptw . -x --lf --nf
+```
+
+will call `pytest` with the following arguments:
+
+```sh
+pytest -x --lf --nf
+```
+
+## Using a different test runner
+
+You can specify an alternative test runner using the `--runner` flag:
+
+```sh
+ptw . --runner tox
+```
+
+## Watching different patterns
+
+You can use the `--patterns` flag to specify file patterns that you want to monitor. It accepts a list of Unix-style patterns separated by a comma. The default value is "\*.py".
+
+Example:
+
+```sh
+ptw . --patterns '*.py,pyproject.toml'
+```
+
+You can also **ignore** certain patterns using the `--ignore-patterns` flag:
+
+```sh
+ptw . --ignore-patterns 'settings.py,db.py'
+```
+
+## Delay
+
+`pytest-watcher` uses a short delay (0.2 seconds by default) before triggering the actual test run. The main motivation for this is post-processors that can run after you save the file (e.g., `black` plugin in your IDE). This ensures that tests will be run with the latest version of your code.
+
+You can control the actual delay value with the `--delay` flag:
+
+`ptw . --delay 0.2`
+
+To disable the delay altogether, you can provide zero as a value:
+
+`ptw . --delay 0`
+
+## Compatibility
+
+The code is tested for Python versions 3.7+
+
+## License
+
+This project is licensed under the [MIT License](LICENSE).
 
-setup(**setup_kwargs)
```

