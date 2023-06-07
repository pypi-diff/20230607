# Comparing `tmp/machinable-4.3.0.tar.gz` & `tmp/machinable-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machinable-4.3.0.tar", max compression
+gzip compressed data, was "machinable-4.3.1.tar", max compression
```

## Comparing `machinable-4.3.0.tar` & `machinable-4.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      795 2023-06-01 07:18:36.030406 machinable-4.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2023-06-01 07:18:36.030406 machinable-4.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1135 2023-06-01 07:18:36.030406 machinable-4.3.0/README.md
--rw-r--r--   0        0        0     2159 2023-06-01 07:18:36.034407 machinable-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     1385 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/__init__.py
--rw-r--r--   0        0        0     3137 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/cli.py
--rw-r--r--   0        0        0    37644 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/collection.py
--rw-r--r--   0        0        0    11403 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/component.py
--rw-r--r--   0        0        0     2933 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/config.py
--rw-r--r--   0        0        0    22346 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/element.py
--rw-r--r--   0        0        0      615 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/errors.py
--rw-r--r--   0        0        0     6525 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/execution.py
--rw-r--r--   0        0        0     1596 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/group.py
--rw-r--r--   0        0        0     7549 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/index.py
--rw-r--r--   0        0        0    13534 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/interface.py
--rw-r--r--   0        0        0     2480 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/mixin.py
--rw-r--r--   0        0        0    10855 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/project.py
--rw-r--r--   0        0        0       10 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/py.typed
--rw-r--r--   0        0        0      630 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/schedule.py
--rw-r--r--   0        0        0     1433 2023-06-01 07:18:36.034407 machinable-4.3.0/src/machinable/schema.py
--rw-r--r--   0        0        0     1002 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/settings.py
--rw-r--r--   0        0        0     1041 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/storage.py
--rw-r--r--   0        0        0      359 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/types.py
--rw-r--r--   0        0        0    16473 2023-06-01 07:18:36.038407 machinable-4.3.0/src/machinable/utils.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 machinable-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0      896 2023-06-07 18:23:36.935176 machinable-4.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2023-06-07 18:23:36.935176 machinable-4.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1135 2023-06-07 18:23:36.935176 machinable-4.3.1/README.md
+-rw-r--r--   0        0        0     2137 2023-06-07 18:23:36.939177 machinable-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1385 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/__init__.py
+-rw-r--r--   0        0        0     3137 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/cli.py
+-rw-r--r--   0        0        0    37644 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/collection.py
+-rw-r--r--   0        0        0    11517 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/component.py
+-rw-r--r--   0        0        0     2933 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/config.py
+-rw-r--r--   0        0        0    22346 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/element.py
+-rw-r--r--   0        0        0      615 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/errors.py
+-rw-r--r--   0        0        0     6562 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/execution.py
+-rw-r--r--   0        0        0     1596 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/group.py
+-rw-r--r--   0        0        0     7787 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/index.py
+-rw-r--r--   0        0        0    13534 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/interface.py
+-rw-r--r--   0        0        0     2480 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/mixin.py
+-rw-r--r--   0        0        0    10929 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/project.py
+-rw-r--r--   0        0        0       10 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/py.typed
+-rw-r--r--   0        0        0      630 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/schedule.py
+-rw-r--r--   0        0        0     1296 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/schema.py
+-rw-r--r--   0        0        0     1002 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/settings.py
+-rw-r--r--   0        0        0     1041 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/storage.py
+-rw-r--r--   0        0        0      359 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/types.py
+-rw-r--r--   0        0        0    16362 2023-06-07 18:23:36.939177 machinable-4.3.1/src/machinable/utils.py
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 machinable-4.3.1/PKG-INFO
```

### Comparing `machinable-4.3.0/CHANGELOG.md` & `machinable-4.3.1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 <!-- Please add changes under the Unreleased section that reads 'No current changes' otherwise -->
 
 # Unreleased
 
 No current changes
 
+# v4.3.1
+
+- Drops commandlib dependency
+- Fix Component.execution resolution for resource retrieval
+
 # v4.3.0
 
 - Generalized storage (#437)
 - Support for in-session element instances
 - Allow unstructured untyped dict-config
 - Simplified event structure
```

### Comparing `machinable-4.3.0/LICENSE.txt` & `machinable-4.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/README.md` & `machinable-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/pyproject.toml` & `machinable-4.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "machinable"
-version = "4.3.0"
+version = "4.3.1"
 description = "A modular configuration system for research projects"
 license = "MIT"
 authors = [
     "Frithjof Gressmann <hello@machinable.org>"
 ]
 maintainers = [
     "Frithjof Gressmann <hello@machinable.org>"
@@ -25,15 +25,14 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 flatten-dict = "^0.4"
 jsonlines = "^3.1"
 pydantic = "^1.10.8"
 arrow = "^1.2"
 importlib-metadata = {version = "^6.6", python = "<3.8"}
-commandlib = "^0.3.5"
 omegaconf = "^2.3.0"
 dill = "^0.3.6"
 typing-extensions = {version = "^4.5.0", python = "<3.11"}
 
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.5"
```

### Comparing `machinable-4.3.0/src/machinable/__init__.py` & `machinable-4.3.1/src/machinable/__init__.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/cli.py` & `machinable-4.3.1/src/machinable/cli.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/collection.py` & `machinable-4.3.1/src/machinable/collection.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/component.py` & `machinable-4.3.1/src/machinable/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,22 @@
 
         return self
 
     @classmethod
     def collect(cls, components) -> "ComponentCollection":
         return ComponentCollection(components)
 
-    def resources(self) -> Optional[Dict]:
-        if self.execution is None:
+    def resources(
+        self, execution: Optional["Execution"] = None
+    ) -> Optional[Dict]:
+        if execution is None:
+            execution = self.execution
+        if execution is None:
             return None
-        return self.load_file(f"resources-{self.execution.id}.json", None)
+        return self.load_file(f"resources/{execution.id}.json", None)
 
     def dispatch(self) -> Self:
         """Dispatch the component lifecycle"""
         writes_meta_data = (
             self.on_write_meta_data() is not False and self.is_mounted()
         )
         try:
```

### Comparing `machinable-4.3.0/src/machinable/config.py` & `machinable-4.3.1/src/machinable/config.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/element.py` & `machinable-4.3.1/src/machinable/element.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/errors.py` & `machinable-4.3.1/src/machinable/errors.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/execution.py` & `machinable-4.3.1/src/machinable/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
         self.commit()
 
         try:
             # compute resources
             for executable in self.pending_executables:
                 executable.save_file(
-                    f"resources-{self.id}.json",
+                    f"resources/{self.id}.json",
                     self.compute_resources(executable),
                 )
             self.__call__()
             self.on_after_dispatch()
         except BaseException as _ex:  # pylint: disable=broad-except
             raise ExecutionFailed("Execution failed") from _ex
 
@@ -197,13 +197,14 @@
     def on_after_dispatch(self) -> None:
         """Event triggered after the dispatch of an execution"""
 
     def __iter__(self):
         yield from self.executables
 
     def __exit__(self, *args, **kwargs):
-        self.dispatch()
-
-        super().__exit__()
+        try:
+            self.dispatch()
+        finally:
+            super().__exit__()
 
     def __repr__(self) -> str:
         return "Execution"
```

### Comparing `machinable-4.3.0/src/machinable/group.py` & `machinable-4.3.1/src/machinable/group.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/index.py` & `machinable-4.3.1/src/machinable/index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, List, Optional, Union
 
 import json
 import os
+from datetime import datetime
 
 try:
     from pysqlite3 import dbapi2 as sqlite3
 except ModuleNotFoundError:
     import sqlite3
 
 from machinable import schema
@@ -53,14 +54,15 @@
         cur.execute(
             """CREATE TABLE 'relations' (
                 id integer PRIMARY KEY NOT NULL,
                 relation text NOT NULL,
                 uuid text NOT NULL REFERENCES 'index' (uuid),
                 related_uuid text NOT NULL REFERENCES 'index' (uuid),
                 'priority' integer NOT NULL DEFAULT 0,
+                'timestamp' real,
                 UNIQUE (uuid, related_uuid, relation)
             )"""
         )
         cur.execute("PRAGMA user_version = 1;")
         db.commit()
         version += 1
     if version == 1:
@@ -154,40 +156,39 @@
 
     def create_relation(
         self,
         relation: str,
         uuid: str,
         related_uuid: Union[str, List[str]],
         priority: int = 0,
+        timestamp: Optional[float] = None,
     ) -> None:
         if isinstance(related_uuid, (list, tuple)):
             for r in related_uuid:
-                self.create_relation(relation, uuid, r, priority)
+                self.create_relation(relation, uuid, r, priority, timestamp)
             return
 
         cur = self.db.cursor()
         if cur.execute(
             """SELECT id FROM 'relations' WHERE uuid=? AND related_uuid=? AND relation=?""",
             (uuid, related_uuid, relation),
         ).fetchone():
             # already exists
             return
+        if timestamp is None:
+            timestamp = datetime.now().timestamp()
         cur.execute(
             """INSERT INTO 'relations' (
                 relation,
                 uuid,
                 related_uuid,
-                priority
-            ) VALUES (?,?,?,?)""",
-            (
-                relation,
-                uuid,
-                related_uuid,
                 priority,
-            ),
+                timestamp
+            ) VALUES (?,?,?,?,?)""",
+            (relation, uuid, related_uuid, priority, timestamp),
         )
         self.db.commit()
 
     def find(self, uuid: str) -> Optional[schema.Interface]:
         cur = self.db.cursor()
         row = cur.execute(
             """SELECT * FROM 'index' WHERE uuid=?""", (uuid,)
@@ -223,21 +224,21 @@
     ) -> Union[None, List[schema.Interface]]:
         cur = self.db.cursor()
         if not inverse:
             rows = cur.execute(
                 """SELECT * FROM 'index' WHERE uuid IN
                     (
                     SELECT related_uuid FROM relations WHERE uuid=? AND relation=?
-                    )
+                    )  ORDER BY 'timestamp' ASC
                 """,
                 (uuid, relation),
             ).fetchall()
         else:
             rows = cur.execute(
                 """SELECT * FROM 'index' WHERE uuid IN
                     (
-                    SELECT uuid FROM relations WHERE related_uuid=? AND relation=?
-                    )
+                    SELECT uuid FROM relations WHERE related_uuid=? AND relation=? ORDER BY 'timestamp' DESC
+                    )  ORDER BY 'timestamp' ASC
                 """,
                 (uuid, relation),
             ).fetchall()
         return [interface_row_factory(cur, row) for row in rows or []]
```

### Comparing `machinable-4.3.0/src/machinable/interface.py` & `machinable-4.3.1/src/machinable/interface.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/mixin.py` & `machinable-4.3.1/src/machinable/mixin.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/project.py` & `machinable-4.3.1/src/machinable/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import types
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import getpass
 import importlib
 import os
 import platform
 import socket
+import subprocess
 import sys
 from dataclasses import dataclass
 
 import machinable
-from commandlib import Command
 from machinable import schema
 from machinable.config import Field, validator
 from machinable.element import Element, get_lineage, instantiate, normversion
 from machinable.errors import ConfigurationError
 from machinable.interface import Interface
 from machinable.types import VersionType
 from machinable.utils import (
@@ -41,19 +40,22 @@
 
     # we use symlink rather than copy for performance and consistency
     fetch_link(source, target)
 
     return True
 
 
-def fetch_git(source, target):
-    git = Command("git")
+def fetch_git(source: str, target: str) -> bool:
     name, directory = os.path.split(target)
-    clone = git("clone").in_dir(directory)
-    clone(source, name).run()
+    command = ["git", "clone", source, name]
+    process = subprocess.Popen(command, cwd=directory)
+    process.communicate()
+
+    if process.returncode != 0:
+        return False
 
     return True
 
 
 def fetch_vendor(source, target):
     if source is None:
         return False
```

### Comparing `machinable-4.3.0/src/machinable/schedule.py` & `machinable-4.3.1/src/machinable/schedule.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/schema.py` & `machinable-4.3.1/src/machinable/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 
 from datetime import datetime
 from uuid import uuid4
 
 from machinable.utils import generate_nickname, generate_seed
 from pydantic import BaseModel, Field, PrivateAttr
 
-if TYPE_CHECKING:
-    from machinable.execution import Execution as ExecutionElement
-    from machinable.storage.storage import Storage
-
 
 class Element(BaseModel):
     uuid: str = Field(default_factory=lambda: uuid4().hex)
     kind: str = "Element"
     module: Optional[str] = None
     version: List[Union[str, Dict]] = []
     config: Optional[Dict] = None
```

### Comparing `machinable-4.3.0/src/machinable/settings.py` & `machinable-4.3.1/src/machinable/settings.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/storage.py` & `machinable-4.3.1/src/machinable/storage.py`

 * *Files identical despite different names*

### Comparing `machinable-4.3.0/src/machinable/utils.py` & `machinable-4.3.1/src/machinable/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 import importlib
 import inspect
 import json
 import os
 import random
 import re
 import string
+import subprocess
 import sys
 from keyword import iskeyword
 from pathlib import Path
 from uuid import UUID
 
 import arrow
-import commandlib
 import dill as pickle
 import jsonlines
 import omegaconf
 from flatten_dict import unflatten as _unflatten_dict
 
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
@@ -465,69 +465,66 @@
             flat[k] = unflatten_dict(nested, splitter, inverse, recursive, copy)
         return flat
 
     return d
 
 
 def get_diff(repository: str) -> Optional[str]:
-    git = commandlib.Command("git").in_dir(os.path.abspath(repository))
-
+    command = ["git", "diff", "--staged"]
     try:
-        return git("diff", "--staged").output()
-    except commandlib.exceptions.CommandError:
+        process = subprocess.run(
+            command,
+            cwd=os.path.abspath(repository),
+            capture_output=True,
+            text=True,
+            check=True,
+        )
+        return process.stdout
+    except subprocess.CalledProcessError:
         return None
 
 
-# This following method is modified 3rd party source code from
-# https://github.com/IDSIA/sacred/blob/7897c664b1b93fa2e2b6f3af244dfee590b1342a/sacred/dependencies.py#L401.
-# The copyright and license agreement can be found in the ThirdPartyNotices.txt file at the root of this repository.
-
-
 def get_commit(repository: str) -> dict:
     try:
-        import git
 
-        try:
-            repo = git.Repo(repository, search_parent_directories=False)
-            try:
-                branch = str(repo.active_branch)
-            except TypeError:
-                branch = None
-
-            try:
-                path = repo.remote().url
-            except ValueError:
-                path = "git:/" + repo.working_dir
-            is_dirty = repo.is_dirty()
-            commit = repo.head.commit.hexsha
-            return {
-                "path": path,
-                "commit": commit,
-                "is_dirty": is_dirty,
-                "branch": branch,
-            }
-        except (git.exc.GitError, ValueError):
-            pass
-    except ImportError:
-        pass
+        def run_git_command(command):
+            return (
+                subprocess.check_output(
+                    ["git", "-C", repository] + command,
+                    stderr=subprocess.DEVNULL,
+                )
+                .decode()
+                .strip()
+            )
 
-    # todo: fallback
+        branch = run_git_command(["rev-parse", "--abbrev-ref", "HEAD"])
+        path = run_git_command(["config", "--get", "remote.origin.url"])
+        is_dirty = run_git_command(["status", "--porcelain"]) != ""
+        commit = run_git_command(["rev-parse", "HEAD"])
+
+        return {
+            "path": path,
+            "commit": commit,
+            "is_dirty": is_dirty,
+            "branch": branch,
+        }
+    except subprocess.CalledProcessError:
+        pass
 
     return {"path": None, "commit": None, "is_dirty": None, "branch": None}
 
 
 def get_root_commit(repository: str) -> Optional[str]:
+    command = ["git", "rev-list", "--parents", "HEAD"]
     try:
-        return (
-            commandlib.Command("git", "rev-list", "--parents", "HEAD")
-            .in_dir(repository)
-            .output()[-1]
-            .replace("\n", "")
+        process = subprocess.run(
+            command, cwd=repository, capture_output=True, text=True, check=True
         )
-    except commandlib.exceptions.CommandError:
+        return process.stdout.split("\n")[-2]
+    except subprocess.CalledProcessError:
         return None
 
 
 class Jsonable:
     def as_json(self, stringify=True, default=serialize, **dumps_kwargs):
         serialized = self.serialize()
         if stringify:
```

### Comparing `machinable-4.3.0/PKG-INFO` & `machinable-4.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinable
-Version: 4.3.0
+Version: 4.3.1
 Summary: A modular configuration system for research projects
 Home-page: https://machinable.org
 License: MIT
 Keywords: machine-learning,research
 Author: Frithjof Gressmann
 Author-email: hello@machinable.org
 Maintainer: Frithjof Gressmann
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Requires-Dist: arrow (>=1.2,<2.0)
-Requires-Dist: commandlib (>=0.3.5,<0.4.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: flatten-dict (>=0.4,<0.5)
 Requires-Dist: importlib-metadata (>=6.6,<7.0) ; python_version < "3.8"
 Requires-Dist: jsonlines (>=3.1,<4.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
```

