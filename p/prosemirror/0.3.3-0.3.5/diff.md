# Comparing `tmp/prosemirror-0.3.3.tar.gz` & `tmp/prosemirror-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosemirror-0.3.3.tar", max compression
+gzip compressed data, was "prosemirror-0.3.5.tar", max compression
```

## Comparing `prosemirror-0.3.3.tar` & `prosemirror-0.3.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1528 2020-07-22 18:58:24.221533 prosemirror-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     3630 2023-03-27 22:18:48.531456 prosemirror-0.3.3/README.md
--rw-r--r--   0        0        0      330 2020-07-22 18:58:24.222880 prosemirror-0.3.3/prosemirror/__init__.py
--rw-r--r--   0        0        0      492 2020-12-14 16:31:43.199118 prosemirror-0.3.3/prosemirror/model/__init__.py
--rw-r--r--   0        0        0       42 2020-07-22 18:58:24.223271 prosemirror-0.3.3/prosemirror/model/comparedeep.py
--rw-r--r--   0        0        0    12692 2023-03-27 22:18:48.542687 prosemirror-0.3.3/prosemirror/model/content.py
--rw-r--r--   0        0        0     2731 2020-07-22 18:58:24.223708 prosemirror-0.3.3/prosemirror/model/diff.py
--rw-r--r--   0        0        0     8051 2023-03-27 22:18:48.544169 prosemirror-0.3.3/prosemirror/model/fragment.py
--rw-r--r--   0        0        0     2344 2022-07-11 00:51:15.545329 prosemirror-0.3.3/prosemirror/model/mark.py
--rw-r--r--   0        0        0    10899 2022-07-11 00:51:15.547534 prosemirror-0.3.3/prosemirror/model/node.py
--rw-r--r--   0        0        0     8169 2021-10-26 17:54:48.043358 prosemirror-0.3.3/prosemirror/model/replace.py
--rw-r--r--   0        0        0     6581 2021-10-26 17:54:48.051172 prosemirror-0.3.3/prosemirror/model/resolvedpos.py
--rw-r--r--   0        0        0    10512 2023-03-27 22:18:48.545830 prosemirror-0.3.3/prosemirror/model/schema.py
--rw-r--r--   0        0        0     6677 2023-03-27 22:43:29.288111 prosemirror-0.3.3/prosemirror/model/to_dom.py
--rw-r--r--   0        0        0       36 2020-07-22 18:58:24.225163 prosemirror-0.3.3/prosemirror/schema/basic/__init__.py
--rw-r--r--   0        0        0     2940 2021-10-26 17:54:48.074794 prosemirror-0.3.3/prosemirror/schema/basic/schema_basic.py
--rw-r--r--   0        0        0       35 2020-07-22 18:58:24.225514 prosemirror-0.3.3/prosemirror/schema/list/__init__.py
--rw-r--r--   0        0        0      959 2023-03-27 22:18:48.546486 prosemirror-0.3.3/prosemirror/schema/list/schema_list.py
--rw-r--r--   0        0        0     1013 2021-10-26 17:54:48.076049 prosemirror-0.3.3/prosemirror/test_builder/__init__.py
--rw-r--r--   0        0        0     3779 2021-10-26 17:54:48.084539 prosemirror-0.3.3/prosemirror/test_builder/build.py
--rw-r--r--   0        0        0      778 2020-07-22 18:58:24.226382 prosemirror-0.3.3/prosemirror/transform/__init__.py
--rw-r--r--   0        0        0     7832 2023-03-27 22:18:48.548629 prosemirror-0.3.3/prosemirror/transform/map.py
--rw-r--r--   0        0        0      149 2021-10-26 17:54:48.101136 prosemirror-0.3.3/prosemirror/transform/mark.py
--rw-r--r--   0        0        0     4804 2021-10-26 17:54:48.108925 prosemirror-0.3.3/prosemirror/transform/mark_step.py
--rw-r--r--   0        0        0    16415 2022-07-11 00:51:15.554148 prosemirror-0.3.3/prosemirror/transform/replace.py
--rw-r--r--   0        0        0     7537 2021-10-26 17:54:48.126732 prosemirror-0.3.3/prosemirror/transform/replace_step.py
--rw-r--r--   0        0        0     1790 2021-10-26 17:54:48.135968 prosemirror-0.3.3/prosemirror/transform/step.py
--rw-r--r--   0        0        0     8191 2023-03-27 22:18:48.555619 prosemirror-0.3.3/prosemirror/transform/structure.py
--rw-r--r--   0        0        0    16886 2023-03-27 22:18:48.557999 prosemirror-0.3.3/prosemirror/transform/transform.py
--rw-r--r--   0        0        0       69 2023-03-27 22:18:48.559628 prosemirror-0.3.3/prosemirror/utils.py
--rw-r--r--   0        0        0      897 2023-03-27 22:43:37.427706 prosemirror-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4386 1970-01-01 00:00:00.000000 prosemirror-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1528 2023-06-07 14:22:51.037197 prosemirror-0.3.5/LICENSE.md
+-rw-r--r--   0        0        0     3631 2023-06-07 14:22:51.037197 prosemirror-0.3.5/README.md
+-rw-r--r--   0        0        0      330 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/__init__.py
+-rw-r--r--   0        0        0      492 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/comparedeep.py
+-rw-r--r--   0        0        0    12692 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/content.py
+-rw-r--r--   0        0        0     2731 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/diff.py
+-rw-r--r--   0        0        0     8051 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/fragment.py
+-rw-r--r--   0        0        0     2344 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/mark.py
+-rw-r--r--   0        0        0    10899 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/node.py
+-rw-r--r--   0        0        0     8170 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/replace.py
+-rw-r--r--   0        0        0     6581 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/resolvedpos.py
+-rw-r--r--   0        0        0    10514 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/schema.py
+-rw-r--r--   0        0        0     6676 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/model/to_dom.py
+-rw-r--r--   0        0        0       36 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/schema/basic/__init__.py
+-rw-r--r--   0        0        0     2939 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/schema/basic/schema_basic.py
+-rw-r--r--   0        0        0       35 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/schema/list/__init__.py
+-rw-r--r--   0        0        0      959 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/schema/list/schema_list.py
+-rw-r--r--   0        0        0     1013 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/test_builder/__init__.py
+-rw-r--r--   0        0        0     3779 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/test_builder/build.py
+-rw-r--r--   0        0        0      778 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/__init__.py
+-rw-r--r--   0        0        0     1798 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/attr_step.py
+-rw-r--r--   0        0        0     7832 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/map.py
+-rw-r--r--   0        0        0      149 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/mark.py
+-rw-r--r--   0        0        0     8217 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/mark_step.py
+-rw-r--r--   0        0        0    16891 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/replace.py
+-rw-r--r--   0        0        0     7537 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/replace_step.py
+-rw-r--r--   0        0        0     1790 2023-06-07 14:22:51.037197 prosemirror-0.3.5/prosemirror/transform/step.py
+-rw-r--r--   0        0        0     8191 2023-06-07 14:22:51.041197 prosemirror-0.3.5/prosemirror/transform/structure.py
+-rw-r--r--   0        0        0    17528 2023-06-07 14:22:51.041197 prosemirror-0.3.5/prosemirror/transform/transform.py
+-rw-r--r--   0        0        0       69 2023-06-07 14:22:51.041197 prosemirror-0.3.5/prosemirror/utils.py
+-rw-r--r--   0        0        0      971 2023-06-07 14:22:51.041197 prosemirror-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 prosemirror-0.3.5/PKG-INFO
```

### Comparing `prosemirror-0.3.3/LICENSE.md` & `prosemirror-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/README.md` & `prosemirror-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![License](https://img.shields.io/pypi/l/prosemirror.svg?style=flat)](https://github.com/fellowapp/prosemirror-py/blob/master/LICENSE.md)
 [![Fellow Careers](https://img.shields.io/badge/fellow.app-hiring-576cf7.svg?style=flat)](https://fellow.app/careers/)
 
 This package provides Python implementations of the following
 [ProseMirror](https://prosemirror.net/) packages:
 
 - [`prosemirror-model`](https://github.com/ProseMirror/prosemirror-model) version 1.18.1
-- [`prosemirror-transform`](https://github.com/ProseMirror/prosemirror-transform) version 1.6.0
+- [`prosemirror-transform`](https://github.com/ProseMirror/prosemirror-transform) version 1.7.1
 - [`prosemirror-test-builder`](https://github.com/ProseMirror/prosemirror-test-builder)
 - [`prosemirror-schema-basic`](https://github.com/ProseMirror/prosemirror-schema-basic) version 1.1.2
 - [`prosemirror-schema-list`](https://github.com/ProseMirror/prosemirror-schema-list)
 
 The original implementation has been followed as closely as possible during
 translation to simplify keeping this package up-to-date with any upstream
 changes.
@@ -83,8 +83,8 @@
             'text': 'Heo'
         }, {
             'type': 'text',
             'text': ', world!'
         }]
     }]
 }
-```
+```
```

### Comparing `prosemirror-0.3.3/prosemirror/model/content.py` & `prosemirror-0.3.5/prosemirror/model/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from functools import reduce, cmp_to_key
+from functools import cmp_to_key, reduce
 from typing import ClassVar
 
 from .fragment import Fragment
 
 
 class ContentMatch:
     empty: ClassVar["ContentMatch"]
@@ -71,15 +71,15 @@
             if finished and (not to_end or finished.valid_end):
                 return Fragment.from_([tp.create_and_fill() for tp in types])
             for i in range(0, len(match.next), 2):
                 type = match.next[i]
                 next = match.next[i + 1]
                 if not (type.is_text or type.has_required_attrs()) and next not in seen:
                     seen.append(next)
-                    found = search(next, types + [type])
+                    found = search(next, [*types, type])
                     if found:
                         return found
 
         return search(self, [])
 
     def find_wrapping(self, target):
         for i in range(0, len(self.wrap_cache), 2):
@@ -319,15 +319,15 @@
             return [edge(loop)]
         elif expr["type"] == "plus":
             loop = node()
             connect(compile(expr["expr"], from_), loop)
             connect(compile(expr["expr"], loop), loop)
             return [edge(loop)]
         elif expr["type"] == "opt":
-            return [edge(from_)] + compile(expr["expr"], from_)
+            return [edge(from_), *compile(expr["expr"], from_)]
         elif expr["type"] == "range":
             cur = from_
             for i in range(expr["min"]):
                 next = node()
                 connect(compile(expr["expr"], cur), next)
                 cur = next
             if expr["max"] == -1:
```

### Comparing `prosemirror-0.3.3/prosemirror/model/diff.py` & `prosemirror-0.3.5/prosemirror/model/diff.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/model/fragment.py` & `prosemirror-0.3.5/prosemirror/model/fragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import ClassVar, Iterable, TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar, Iterable
 
 from prosemirror.utils import text_length
 
 from .diff import find_diff_end, find_diff_start
 
 if TYPE_CHECKING:
     from .node import Node
@@ -129,18 +129,18 @@
             return self
         copy = self.content.copy()
         size = self.size + node.node_size - current.node_size
         copy[index] = node
         return Fragment(copy, size)
 
     def add_to_start(self, node):
-        return Fragment([node] + self.content, self.size + node.node_size)
+        return Fragment([node, *self.content], self.size + node.node_size)
 
     def add_to_end(self, node):
-        return Fragment(self.content + [node], self.size + node.node_size)
+        return Fragment([*self.content, node], self.size + node.node_size)
 
     def eq(self, other):
         if len(self.content) != len(other.content):
             return False
         return all(a.eq(b) for (a, b) in zip(self.content, other.content))
 
     @property
```

### Comparing `prosemirror-0.3.3/prosemirror/model/mark.py` & `prosemirror-0.3.5/prosemirror/model/mark.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/model/node.py` & `prosemirror-0.3.5/prosemirror/model/node.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/model/replace.py` & `prosemirror-0.3.5/prosemirror/model/replace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import ClassVar
+
 from .fragment import Fragment
 
 
 class ReplaceError(ValueError):
     pass
```

### Comparing `prosemirror-0.3.3/prosemirror/model/resolvedpos.py` & `prosemirror-0.3.5/prosemirror/model/resolvedpos.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/model/schema.py` & `prosemirror-0.3.5/prosemirror/model/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import OrderedDict
+
 from typing_extensions import Literal
 
 from .content import ContentMatch
 from .fragment import Fragment
 from .mark import Mark
 from .node import Node, TextNode
 
@@ -23,15 +24,15 @@
         if value:
             given = value.get(name)
         if given is None:
             attr = attrs.get(name)
             if attr.has_default:
                 given = attr.default
             else:
-                raise ValueError("No value supplied for attribute" + name)
+                raise ValueError("No value supplied for attribute " + name)
         built[name] = given
     return built
 
 
 def init_attrs(attrs):
     result = {}
     if attrs:
```

### Comparing `prosemirror-0.3.3/prosemirror/model/to_dom.py` & `prosemirror-0.3.5/prosemirror/model/to_dom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import html
-from typing import cast, Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 
 from . import Fragment, Mark, Node, Schema
 
-
 HTMLNode = Union["Element", str]
 
 
 class DocumentFragment:
     def __init__(self, children: List[HTMLNode]):
         self.children = children
```

### Comparing `prosemirror-0.3.3/prosemirror/schema/basic/schema_basic.py` & `prosemirror-0.3.5/prosemirror/schema/basic/schema_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from prosemirror.model import Schema
 
-
 p_dom = ["p", 0]
 blockquote_dom = ["blockquote", 0]
 hr_dom = ["hr"]
 pre_dom = ["pre", ["code", 0]]
 br_dom = ["br"]
```

### Comparing `prosemirror-0.3.3/prosemirror/schema/list/schema_list.py` & `prosemirror-0.3.5/prosemirror/schema/list/schema_list.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/test_builder/__init__.py` & `prosemirror-0.3.5/prosemirror/test_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/test_builder/build.py` & `prosemirror-0.3.5/prosemirror/test_builder/build.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/transform/__init__.py` & `prosemirror-0.3.5/prosemirror/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/transform/map.py` & `prosemirror-0.3.5/prosemirror/transform/map.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/transform/replace.py` & `prosemirror-0.3.5/prosemirror/transform/replace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from prosemirror.model import Fragment, ResolvedPos, Slice
 from typing import List, Optional
 
+from prosemirror.model import Fragment, ResolvedPos, Slice
+
 from .replace_step import ReplaceAroundStep, ReplaceStep, Step
 
 
 def replace_step(doc, from_, to=None, slice=None):
     if to is None:
         to = from_
     if slice is None:
@@ -112,16 +113,30 @@
                 placed_size,
             )
         if slice.size or from__.pos != self.to_.pos:
             return ReplaceStep(from__.pos, to_.pos, slice)
         return None
 
     def find_fittable(self) -> Optional[_Fittable]:
+        start_depth = self.unplaced.open_start
+        cur = self.unplaced.content
+        open_end = self.unplaced.open_end
+        for d in range(start_depth):
+            node = cur.first_child
+            if cur.child_count > 1:
+                open_end = 0
+            if node.type.spec.get("isolating") and open_end <= d:
+                start_depth = d
+                break
+            cur = node.content
+
         for pass_ in [1, 2]:
-            for slice_depth in range(self.unplaced.open_start, -1, -1):
+            for slice_depth in range(
+                start_depth if pass_ == 1 else self.unplaced.open_start, -1, -1
+            ):
                 if slice_depth:
                     parent = content_at(
                         self.unplaced.content, slice_depth - 1
                     ).first_child
                     fragment = parent.content
                 else:
                     parent = None
```

### Comparing `prosemirror-0.3.3/prosemirror/transform/replace_step.py` & `prosemirror-0.3.5/prosemirror/transform/replace_step.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/transform/step.py` & `prosemirror-0.3.5/prosemirror/transform/step.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/transform/structure.py` & `prosemirror-0.3.5/prosemirror/transform/structure.py`

 * *Files identical despite different names*

### Comparing `prosemirror-0.3.3/prosemirror/transform/transform.py` & `prosemirror-0.3.5/prosemirror/transform/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union
 
-from prosemirror.model import Fragment, MarkType, Node, NodeType, Slice
+from prosemirror.model import Fragment, Mark, MarkType, Node, NodeType, Slice
 
 from . import replace, structure
+from .attr_step import AttrStep
 from .map import Mapping
-from .mark_step import AddMarkStep, RemoveMarkStep
+from .mark_step import AddMarkStep, AddNodeMarkStep, RemoveMarkStep, RemoveNodeMarkStep
 from .replace import close_fragment, covered_depths, fits_trivially, replace_step
 from .replace_step import ReplaceAroundStep, ReplaceStep
 from .structure import can_change_type, insert_point
 
 
 def defines_content(type: Union[NodeType, MarkType]):
     return type.spec.get("defining") or type.spec.get("definingForContent")
@@ -452,14 +453,30 @@
                 pos + node.node_size - 1,
                 Slice(Fragment.from_(new_node), 0, 0),
                 1,
                 True,
             )
         )
 
+    def set_node_attribute(self, pos, attr, value):
+        return self.step(AttrStep(pos, attr, value))
+
+    def add_node_mark(self, pos, mark):
+        return self.step(AddNodeMarkStep(pos, mark))
+
+    def remove_node_mark(self, pos, mark):
+        if not isinstance(mark, Mark):
+            node = self.doc.node_at(pos)
+            if not node:
+                raise ValueError("No node at position " + pos)
+            mark = mark.is_in_set(node.marks)
+            if not mark:
+                return self
+        return self.step(RemoveNodeMarkStep(pos, mark))
+
     def split(self, pos, depth=None, types_after=None):
         if depth is None:
             depth = 1
         pos_ = self.doc.resolve(pos)
         before = Fragment.empty
         after = Fragment.empty
         d = pos_.depth
```

### Comparing `prosemirror-0.3.3/pyproject.toml` & `prosemirror-0.3.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 [tool.poetry]
 name = "prosemirror"
-version = "0.3.3"
+version = "0.3.5"
 description = "Python implementation of core ProseMirror modules for collaborative editing"
 readme = "README.md"
 authors = ["Shen Li <shen@fellow.co>"]
 license = "BSD-3-Clause"
 packages = [{ include = "prosemirror" }]
 homepage = "https://github.com/fellowinsights/prosemirror-py"
 repository = "https://github.com/fellowinsights/prosemirror-py"
 keywords = ["prosemirror", "collaborative", "editing"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+codecov = "^2.1.13"
+coverage = "^7.0.5"
 flake8 = "^6.0.0"
-black = "^22.12.0"
-mypy = "^0.991"
-pytest = "^7.2.1"
-pydash = "^5.1.2"
+isort = "^5.11.4"
+mypy = "^1.3.0"
 pandoc = "^2.3"
+pydash = "^7.0.3"
+pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-isort = "^5.11.4"
-codecov = "^2.1.12"
-coverage = "^7.0.5"
-ruff = "^0.0.230"
+ruff = "^0.0.271"
 
 [tool.black]
-max-line-length=88
+max-line-length = 88
+
+[tool.ruff]
+select = [
+    "E",
+    "F",
+    "W",
+    "I",
+    "RUF",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prosemirror-0.3.3/PKG-INFO` & `prosemirror-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosemirror
-Version: 0.3.3
+Version: 0.3.5
 Summary: Python implementation of core ProseMirror modules for collaborative editing
 Home-page: https://github.com/fellowinsights/prosemirror-py
 License: BSD-3-Clause
 Keywords: prosemirror,collaborative,editing
 Author: Shen Li
 Author-email: shen@fellow.co
 Requires-Python: >=3.8.1,<4
@@ -26,15 +26,15 @@
 [![License](https://img.shields.io/pypi/l/prosemirror.svg?style=flat)](https://github.com/fellowapp/prosemirror-py/blob/master/LICENSE.md)
 [![Fellow Careers](https://img.shields.io/badge/fellow.app-hiring-576cf7.svg?style=flat)](https://fellow.app/careers/)
 
 This package provides Python implementations of the following
 [ProseMirror](https://prosemirror.net/) packages:
 
 - [`prosemirror-model`](https://github.com/ProseMirror/prosemirror-model) version 1.18.1
-- [`prosemirror-transform`](https://github.com/ProseMirror/prosemirror-transform) version 1.6.0
+- [`prosemirror-transform`](https://github.com/ProseMirror/prosemirror-transform) version 1.7.1
 - [`prosemirror-test-builder`](https://github.com/ProseMirror/prosemirror-test-builder)
 - [`prosemirror-schema-basic`](https://github.com/ProseMirror/prosemirror-schema-basic) version 1.1.2
 - [`prosemirror-schema-list`](https://github.com/ProseMirror/prosemirror-schema-list)
 
 The original implementation has been followed as closely as possible during
 translation to simplify keeping this package up-to-date with any upstream
 changes.
@@ -103,7 +103,8 @@
         }, {
             'type': 'text',
             'text': ', world!'
         }]
     }]
 }
 ```
+
```

