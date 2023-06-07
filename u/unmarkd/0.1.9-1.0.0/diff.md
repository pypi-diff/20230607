# Comparing `tmp/unmarkd-0.1.9.tar.gz` & `tmp/unmarkd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unmarkd-0.1.9.tar", max compression
+gzip compressed data, was "unmarkd-1.0.0.tar", max compression
```

## Comparing `unmarkd-0.1.9.tar` & `unmarkd-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    35149 2021-02-21 03:47:27.745822 unmarkd-0.1.9/LICENSE.md
--rw-r--r--   0        0        0     8401 2022-03-22 03:44:17.183356 unmarkd-0.1.9/README.md
--rw-r--r--   0        0        0     1352 2022-06-18 16:47:15.775344 unmarkd-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      325 2022-06-18 16:47:11.651806 unmarkd-0.1.9/unmarkd/__init__.py
--rw-r--r--   0        0        0     9520 2022-06-18 16:46:36.508213 unmarkd-0.1.9/unmarkd/unmarkers.py
--rw-r--r--   0        0        0     9453 2022-06-18 16:48:01.795796 unmarkd-0.1.9/setup.py
--rw-r--r--   0        0        0     9905 2022-06-18 16:48:01.796311 unmarkd-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 03:58:44.466970 unmarkd-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     8773 2023-06-07 04:49:42.568345 unmarkd-1.0.0/README.md
+-rw-r--r--   0        0        0     2870 2023-06-07 05:11:19.601322 unmarkd-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      319 2023-06-07 05:09:39.165015 unmarkd-1.0.0/unmarkd/__init__.py
+-rw-r--r--   0        0        0    10478 2023-06-07 05:05:56.801088 unmarkd-1.0.0/unmarkd/unmarkers.py
+-rw-r--r--   0        0        0     9941 1970-01-01 00:00:00.000000 unmarkd-1.0.0/PKG-INFO
```

### Comparing `unmarkd-0.1.9/LICENSE.md` & `unmarkd-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unmarkd-0.1.9/README.md` & `unmarkd-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-**NOTE: This project is *maintained.*** While it may seem inactive, it is because there is nothing to add. If you want an enhancement or want to file a bug report, please go to the [issues](https://github.com/ThatXliner/unmarkd/issues).
+**NOTE: This project is _maintained._** While it may seem inactive, it is because there is nothing to add. If you want an enhancement or want to file a bug report, please go to the [issues](https://github.com/ThatXliner/unmarkd/issues).
 
 # 🔄 Unmarkd
-[![codecov](https://codecov.io/gh/ThatXliner/unmarkd/branch/master/graph/badge.svg?token=PWVIERHTG3)](https://codecov.io/gh/ThatXliner/unmarkd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml/badge.svg)](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/unmarkd)](https://pypi.org/project/unmarkd/)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)[![codecov](https://codecov.io/gh/ThatXliner/unmarkd/branch/master/graph/badge.svg?token=PWVIERHTG3)](https://codecov.io/gh/ThatXliner/unmarkd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml/badge.svg)](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/unmarkd)](https://pypi.org/project/unmarkd/)
 
 > A markdown reverser.
 
 ---
+
 Unmarkd is a [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)-powered [Markdown](https://en.wikipedia.org/wiki/Markdown) reverser written in Python and for Python.
 
 ## Why
 
 This is created as a [StackSearch](http://github.com/ThatXliner/stacksearch) (one of my other projects) dependency. In order to create a better API, I needed a way to reverse HTML. So I created this.
 
-There are [similar projects](https://github.com/xijo/reverse_markdown) (written in Ruby) ~~but I have not found any written in Python (or for Python)~~ later I found a popular library, [html2text](https://github.com/Alir3z4/html2text). But Unmarkd still is *still* better. See [comparison](#comparison).
+There are [similar projects](https://github.com/xijo/reverse_markdown) (written in Ruby) ~~but I have not found any written in Python (or for Python)~~ later I found a popular library, [html2text](https://github.com/Alir3z4/html2text).
 
 ## Installation
 
 You know the drill
 
 ```bash
 pip install unmarkd
@@ -24,15 +29,14 @@
 
 ## Comparison
 
 **TL;DR: Html2Text is fast. If you don't need much configuration, you could use Html2Text for the little speed increase.**
 
 <details>
 
-
 <summary>Click to expand</summary>
 
 ### Speed
 
 **TL;DR: Unmarkd < Html2Text**
 
 Html2Text is basically faster:
@@ -49,26 +53,25 @@
 
 I hope that's a good explanation of the speed difference.
 
 ### Correctness
 
 **TL;DR: Unmarkd == Html2Text**
 
-I actually found *two* html-to-markdown libraries. One of them was [Tomd](https://github.com/gaojiuli/tomd) which had an *incorrect implementation*:
+I actually found _two_ html-to-markdown libraries. One of them was [Tomd](https://github.com/gaojiuli/tomd) which had an _incorrect implementation_:
 
 ![Actual results](./assets/tomd_cant_handle.png)
 
 It seems to be abandoned, anyway.
 
 Now with Html2Text and Unmarkd:
 
 ![Epic showdown](./assets/correct.png)
 
-
-In other words, they *work*
+In other words, they _work_
 
 ### Configurability
 
 **TL;DR: Unmarkd > Html2Text**
 
 This is Unmarkd's strong point.
 
@@ -122,17 +125,18 @@
 <p>Or inline code like <code>var foo = &#39;bar&#39;;</code>.</p>
 <p>Or an image of bears</p>
 <p><img src="http://placebear.com/200/200" alt="bears"></p>
 <p>The end ...</p>
 """
 print(unmarkd.unmark(html_doc))
 ```
+
 and the output:
 
-```markdown
+````markdown
     # Sample Markdown
 
 
     This is some basic, sample markdown.
 
     ## Second Heading
 
@@ -164,51 +168,52 @@
     Or inline code like `var foo = 'bar';`.
 
     Or an image of bears
 
     ![bears](http://placebear.com/200/200)
 
     The end ...
-```
+````
+
 ### Extending
 
 #### Brief Overview
 
 Most functionality should be covered by the `BasicUnmarker` class defined in `unmarkd.unmarkers`.
 
 If you need to reverse markdown from StackExchange (as in the case for my other project), you may use the `StackOverflowUnmarker` (or it's alias, `StackExchangeUnmarker`), which is also defined in `unmarkd.unmarkers`.
 
 #### Customizing
 
 If the above two classes do not suit your needs, you can subclass the `unmarkd.unmarkers.BaseUnmarker` abstract class.
 
-Currently, you can *optionally* override the following methods:
-
- - `detect_language` (parameters: **1**)
-    - **Parameters**:
-        - html: `bs4.BeautifulSoup`
-    - When a fenced code block is approached, this function is called with a parameter of type `bs4.BeautifulSoup` passed to it; this is the element the code block was detected from (i.e. `pre`).
-    - This function is responsible for detecting the programming language (or returning `''` if none was detected) of the code block.
-    - Note: This method is different from `unmarkd.unmarkers.BasicUnmarker`. It is simpler and does less checking/filtering
+Currently, you can _optionally_ override the following methods:
 
+- `detect_language` (parameters: **1**)
+  - **Parameters**:
+    - html: `bs4.BeautifulSoup`
+  - When a fenced code block is approached, this function is called with a parameter of type `bs4.BeautifulSoup` passed to it; this is the element the code block was detected from (i.e. `pre`).
+  - This function is responsible for detecting the programming language (or returning `''` if none was detected) of the code block.
+  - Note: This method is different from `unmarkd.unmarkers.BasicUnmarker`. It is simpler and does less checking/filtering
 
 But Unmarkd is more flexible than that.
 
 ##### Customizable constants
 
 There are currently 3 constants you may override:
- - Formats:
-    NOTE: Use the [**Format String Syntax**](https://docs.python.org/3/library/string.html#formatstrings)
-     - `UNORDERED_FORMAT`
-        - The string format of unordered (bulleted) lists.
-     - `ORDERED_FORMAT`
-        -  The string format of ordered (numbered) lists.
- - Miscellaneous:
-     - `ESCAPABLES`
-        - A container (preferably a `set`) of length-1 `str` that should be escaped
+
+- Formats:
+  NOTE: Use the [**Format String Syntax**](https://docs.python.org/3/library/string.html#formatstrings)
+  - `UNORDERED_FORMAT`
+    - The string format of unordered (bulleted) lists.
+  - `ORDERED_FORMAT`
+    - The string format of ordered (numbered) lists.
+- Miscellaneous:
+  - `ESCAPABLES`
+    - A container (preferably a `set`) of length-1 `str` that should be escaped
 
 ##### Customize converting HTML tags
 
 For an HTML tag `some_tag`, you can customize how it's converted to markdown by overriding a method like so:
 
 ```python
 from unmarkd.unmarkers import BaseUnmarker
@@ -221,21 +226,21 @@
 
 If you really need to, you may also modify `DEFAULT_TAG_ALIASES`. Be warned: if you do so, **you will also need to implement the aliases** (currently `em` and `strong`).
 
 ##### Utility functions when overriding
 
 You may use (when extending) the following functions:
 
- - `__parse`, 2 parameters:
-    - `html`: *bs4.BeautifulSoup*
-        - The html to unmark. This is used internally by the `unmark` method and is slightly faster.
-    - `escape`: *bool*
-        - Whether to escape the characters inside the string or not. Defaults to `False`.
- - `escape`: 1 parameter:
-    - `string`: *str*
-        - The string to escape and make markdown-safe
- - `wrap`: 2 parameters:
-    - `element`: *bs4.BeautifulSoup*
-        - The element to wrap.
-    - `around_with`: *str*
-        - The character to wrap the element around with. **WILL NOT BE ESCPAED**
- - And, of course, `tag_*` and `detect_language`.
+- `__parse`, 2 parameters:
+  - `html`: _bs4.BeautifulSoup_
+    - The html to unmark. This is used internally by the `unmark` method and is slightly faster.
+  - `escape`: _bool_
+    - Whether to escape the characters inside the string or not. Defaults to `False`.
+- `escape`: 1 parameter:
+  - `string`: _str_
+    - The string to escape and make markdown-safe
+- `wrap`: 2 parameters:
+  - `element`: _bs4.BeautifulSoup_
+    - The element to wrap.
+  - `around_with`: _str_
+    - The character to wrap the element around with. **WILL NOT BE ESCPAED**
+- And, of course, `tag_*` and `detect_language`.
```

### Comparing `unmarkd-0.1.9/unmarkd/unmarkers.py` & `unmarkd-1.0.0/unmarkd/unmarkers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,76 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""Generate markdown from messy HTML"""
-
+"""Generate markdown from messy HTML."""
 import abc
+import contextlib
 import html as lib_html
-import re
 import textwrap
-from typing import Callable, Dict, Set, Union
+from typing import Callable, Dict, Optional, Set, Union
 
 import bs4
 
 
 class BaseUnmarker(abc.ABC):
+    """To customize the behavior of your reverser, inherit from this abstract class."""
+
     ESCAPABLES: Set[str] = {
         "*",
         "`",
         "\\",
         "~",
         "_",
         "-",
         "[",
         "]",
         ">",
         "#",
-        # "(",
-        # ")",
     }
     TAG_ALIASES: Dict[str, str] = {}
     DEFAULT_TAG_ALIASES: Dict[str, str] = {"em": "i", "strong": "b", "s": "del"}
     UNORDERED_FORMAT: str = "\n- {next_item}"
     ORDERED_FORMAT: str = "\n {number_index}. {next_item}"
 
-    # def parse_css(self, css: str) -> Dict[str, str]:
-    #     return {k: v for style in css.split(";") for k, v in style.split(":", 1)}
+    # def parse_css(self: "BaseUnmarker", css: str) -> Dict[str, str]:
 
     def _render_list(
-        self,
+        self: "BaseUnmarker",
         element: bs4.BeautifulSoup,
         item_format: str,
         counter_initial_value: int = 1,
     ) -> str:
         """Render a list of items according to a format.
 
         Made to reduce code duplication.
         """
         output = ""
         for counter, item in enumerate(
-            element(True, recursive=False), counter_initial_value
+            element(True, recursive=False),
+            counter_initial_value,
         ):
             output += (
                 item_format.strip().format(
-                    next_item=self.tag_li(item).rstrip(), number_index=counter
+                    next_item=self.tag_li(item).rstrip(),
+                    number_index=counter,
                 )
                 + "\n"
             )
         return output
 
-    def escape(self, string: str) -> str:
-        """Escape a string to be markdown-safe"""
+    def escape(self: "BaseUnmarker", string: str) -> str:
+        """Escape a string to be markdown-safe."""
         return "".join(map(self.__escape_character, string))
 
-    def __escape_character(self, char: str) -> str:
-        """Escape a single character"""
+    def __escape_character(self: "BaseUnmarker", char: str) -> str:
+        """Escape a single character."""
         assert len(char) == 1
         if char in self.ESCAPABLES:
             return "\\" + char
         return lib_html.escape(char)
 
-    def wrap(self, element: bs4.BeautifulSoup, around_with: str) -> str:
-        """Wrap an element in a markdown-safe manner
+    def wrap(self: "BaseUnmarker", element: bs4.BeautifulSoup, around_with: str) -> str:
+        """Wrap an element in a markdown-safe manner.
 
         Parameters
         ----------
         element : bs4.BeautifulSoup
             The element to wrap.
         around_with : str
             What to wrap `element` around with.
@@ -85,149 +83,168 @@
         -------
         str
             The wrapped version of the element.
 
         """
         return around_with + self.__parse(element, escape=True) + around_with
 
-    def resolve_handler_func(self, name: str) -> Callable[[bs4.BeautifulSoup], str]:
+    def resolve_handler_func(
+        self: "BaseUnmarker",
+        name: str,
+    ) -> Callable[[bs4.BeautifulSoup], str]:
         return getattr(self, "tag_" + name)
 
-    def __parse(self, html: bs4.BeautifulSoup, escape: bool = False) -> str:
+    def __parse(
+        self: "BaseUnmarker",
+        html: bs4.BeautifulSoup,
+        escape: bool = False,
+    ) -> str:
         """Parse an HTML element into valid markdown."""
         output = ""
         if html is None:
             return ""
         for child in html.children:
             if type(child) in (str, bs4.NavigableString):
                 if child == "\n":
                     output += "\n\n"
                 else:
                     output += self.escape(child) if escape else child
             elif type(child) is bs4.element.Doctype:
                 continue
             else:
-                name: str = child.name
+                name: Optional[str] = child.name
                 # To reduce code duplication
                 name = (
                     self.DEFAULT_TAG_ALIASES.get(name)
                     or self.TAG_ALIASES.get(name)
                     or name
                 )
+                if name is None:
+                    assert isinstance(child, bs4.Comment)
+                    output += self.handle_comment(child)
+                    continue
 
                 try:
                     output += self.resolve_handler_func(name)(child)
                 except AttributeError:
                     if name.startswith("h"):  # XXX: Maybe H1, up to H6, is enough?
                         output += "#" * int(name[1:]) + " " + self.__parse(child) + "\n"
                         continue
                     output += self.handle_default(child)
         return output
 
-    def handle_default(self, child: bs4.BeautifulSoup) -> str:
-        """Whenever a tag isn't handled by one of these methods, this is called"""
+    def handle_comment(self: "BaseUnmarker", child: bs4.Comment) -> str:
+        """Self explanatory."""
+        # Should not cause any escaping problems since
+        # BeautifulSoup escapes the string contents
+        # See also https://www.crummy.com/software/BeautifulSoup/bs4/doc/#output-formatters
+        return f"<!--{child}-->"
+
+    def handle_default(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
+        """Whenever a tag isn't handled by one of these methods, this is called."""
         return str(child)
 
-    def tag_div(self, child: bs4.BeautifulSoup) -> str:
+    def tag_div(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.__parse(child)
 
-    def tag_p(self, child: bs4.BeautifulSoup) -> str:
+    def tag_p(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.__parse(child, escape=True)
 
-    def tag_del(self, child: bs4.BeautifulSoup) -> str:
+    def tag_del(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.wrap(child, around_with="~~")
 
-    def tag_pre(self, child: bs4.BeautifulSoup) -> str:
+    def tag_pre(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return f"\n```{self.detect_language(child)}\n{child.code.get_text()}```\n"
 
-    def tag_code(self, child: bs4.BeautifulSoup) -> str:
+    def tag_code(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return f"`{self.__parse(child)}`"
 
-    def tag_hr(self, _: bs4.BeautifulSoup) -> str:
+    def tag_hr(self: "BaseUnmarker", _: bs4.BeautifulSoup) -> str:
         return "\n---\n"
 
-    def tag_td(self, child: bs4.BeautifulSoup) -> str:
+    def tag_td(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.__parse(child, escape=True)
 
-    def tag_b(self, child: bs4.BeautifulSoup) -> str:
+    def tag_b(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.wrap(child, around_with="**")
 
-    def tag_i(self, child: bs4.BeautifulSoup) -> str:
+    def tag_i(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.wrap(child, around_with="*")
 
-    def tag_a(self, child: bs4.BeautifulSoup) -> str:
+    def tag_a(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return (
             f"[{self.__parse(child)}]({child['href']}"
             + (" " + repr(self.escape(child["title"])) if child.get("title") else "")
             + ")"
         )
 
-    def tag_img(self, child: bs4.BeautifulSoup) -> str:
+    def tag_img(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         try:
             tag = child.contents[0]
         except IndexError:
             tag = child
         try:
             tag_text = child.contents[-1]
         except IndexError:
             next_sib = tag.next_sibling
             tag_text = (
                 next_sib.extract().strip() if next_sib else tag.get_text().strip()
             )
         return f"![{tag.get('alt') or tag_text}]({tag['src']})"
 
-    def tag_ul(self, child: bs4.BeautifulSoup) -> str:
+    def tag_ul(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self._render_list(child, self.UNORDERED_FORMAT)
 
-    def tag_ol(self, child: bs4.BeautifulSoup) -> str:
+    def tag_ol(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self._render_list(
             child,
             self.ORDERED_FORMAT,
             counter_initial_value=int(child.get("start", 1)),
         )
 
-    def tag_li(self, child: bs4.BeautifulSoup) -> str:
+    def tag_li(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         output = ""
         for elstr in child.children:
             if str(elstr) == elstr:
                 output += str(elstr).rstrip(" ")
+            elif elstr.name in ("ol", "ul"):
+                output += textwrap.indent(
+                    self.resolve_handler_func(elstr.name)(elstr),
+                    "    ",
+                )
             else:
-                if elstr.name in ("ol", "ul"):
-                    output += textwrap.indent(
-                        self.resolve_handler_func(elstr.name)(elstr), "    "
-                    )
-                else:
-                    output += self.resolve_handler_func(elstr.name)(elstr)
+                output += self.resolve_handler_func(elstr.name)(elstr)
         return output
 
-    def tag_br(self, _: bs4.BeautifulSoup) -> str:
+    def tag_br(self: "BaseUnmarker", _: bs4.BeautifulSoup) -> str:
         return "\n\n"
 
-    def tag_blockquote(self, child: bs4.BeautifulSoup) -> str:
+    def tag_blockquote(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return ">" + self.__parse(child).strip() + "\n"
 
-    def tag_q(self, child: bs4.BeautifulSoup) -> str:
+    def tag_q(self: "BaseUnmarker", child: bs4.BeautifulSoup) -> str:
         return self.wrap(child, around_with='"')
 
-    def unmark(self, html: Union[str, bs4.BeautifulSoup]) -> str:
-        """The main reverser method. Use this to convert HTML into markdown"""
+    def unmark(self: "BaseUnmarker", html: Union[str, bs4.BeautifulSoup]) -> str:
+        """Convert HTML into markdown."""
         if type(html) != bs4.BeautifulSoup:
             assert isinstance(html, str)
             html = bs4.BeautifulSoup(html, "html.parser")
         assert isinstance(html, bs4.BeautifulSoup)
         if html.html is not None:  # Testing if not using "html.parser"
             html.html.unwrap()  # Maintaining lxml and html5lib compatibility
             if html.head is not None:  # html5lib compatibility... for the future
                 html.head.decompose()
             if html.body is not None:  # lxml compatibility
                 html.body.unwrap()
         return self.__parse(html).strip().replace("\u0000", "\uFFFD")
 
     def detect_language(
-        self, html: bs4.BeautifulSoup
+        self: "BaseUnmarker",
+        html: bs4.BeautifulSoup,
     ) -> str:  # XXX: Replace with info string
         """From a block of HTML, detect the language from the class attribute.
 
         Warning
         -------
         The default is very dumb and will return the first class.
 
@@ -243,53 +260,52 @@
 
         """
         classes = html.get("class") or html.code.get("class")
         return classes[0] or ""
 
 
 class StackOverflowUnmarker(BaseUnmarker):
-    """A specialized unmarker for HTML found on StackOverflow"""
+    """A specialized unmarker for HTML found on StackOverflow."""
 
-    def detect_language(self, html: bs4.BeautifulSoup) -> str:
+    def detect_language(self: "BaseUnmarker", html: bs4.BeautifulSoup) -> str:
         classes = html.get("class") or html.code.get("class")
         if classes is None:
             return ""
         classes = classes[:]  # Copy it
         for item in (
             "default",
             "s-code-block",
             "hljs",
             "snippet-code-js",
             "prettyprint-override",
         ):
-            try:
+            with contextlib.suppress(ValueError):
                 classes.remove(item)
-            except ValueError:
-                pass
+
         if len(classes) == 0:
             return ""
         output = classes[0]
         if output.startswith("lang-"):
-            output = output[5:]
+            return output[5:]
         if output.startswith("snippet-code-"):
-            output = output[13:]
+            return output[13:]
         return output
 
 
 StackExchangeUnmarker = StackOverflowUnmarker
 
 
 class BasicUnmarker(BaseUnmarker):
-    """The basic, generic unmarker"""
+    """The basic, generic unmarker."""
 
-    def detect_language(self, html: bs4.BeautifulSoup) -> str:
+    def detect_language(self: "BaseUnmarker", html: bs4.BeautifulSoup) -> str:
         classes = html.get("class") or html.code.get("class")
         if classes is None:
             return ""
         classes = classes[:]  # Copy it
         assert len(classes) == 1
         lang = classes[0]
         if lang.startswith("lang-"):
-            lang = lang[5:]
-        elif lang.startswith("language-"):
-            lang = lang[9:]
+            return lang[5:]
+        if lang.startswith("language-"):
+            return lang[9:]
         return lang
```

### Comparing `unmarkd-0.1.9/setup.py` & `unmarkd-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,274 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: unmarkd
+Version: 1.0.0
+Summary: A markdown reverser
+Home-page: https://github.com/ThatXliner/unmarkd
+License: GPL-3.0-or-later
+Author: Bryan Hu
+Author-email: bryan.hu.2020@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Typing :: Typed
+Requires-Dist: beautifulsoup4 (>=4.12.2)
+Project-URL: Documentation, https://unmarkd.readthedocs.io/en/latest/index.html
+Description-Content-Type: text/markdown
 
-packages = \
-['unmarkd']
+**NOTE: This project is _maintained._** While it may seem inactive, it is because there is nothing to add. If you want an enhancement or want to file a bug report, please go to the [issues](https://github.com/ThatXliner/unmarkd/issues).
 
-package_data = \
-{'': ['*']}
+# 🔄 Unmarkd
 
-install_requires = \
-['beautifulsoup4>=4.9.0,<5.0.0']
-
-extras_require = \
-{'all': ['cchardet>=2.1.7,<3.0.0'], 'speedups': ['cchardet>=2.1.7,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'unmarkd',
-    'version': '0.1.9',
-    'description': 'A markdown reverser.',
-    'long_description': '**NOTE: This project is *maintained.*** While it may seem inactive, it is because there is nothing to add. If you want an enhancement or want to file a bug report, please go to the [issues](https://github.com/ThatXliner/unmarkd/issues).\n\n# 🔄 Unmarkd\n[![codecov](https://codecov.io/gh/ThatXliner/unmarkd/branch/master/graph/badge.svg?token=PWVIERHTG3)](https://codecov.io/gh/ThatXliner/unmarkd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml/badge.svg)](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/unmarkd)](https://pypi.org/project/unmarkd/)\n\n> A markdown reverser.\n\n---\nUnmarkd is a [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)-powered [Markdown](https://en.wikipedia.org/wiki/Markdown) reverser written in Python and for Python.\n\n## Why\n\nThis is created as a [StackSearch](http://github.com/ThatXliner/stacksearch) (one of my other projects) dependency. In order to create a better API, I needed a way to reverse HTML. So I created this.\n\nThere are [similar projects](https://github.com/xijo/reverse_markdown) (written in Ruby) ~~but I have not found any written in Python (or for Python)~~ later I found a popular library, [html2text](https://github.com/Alir3z4/html2text). But Unmarkd still is *still* better. See [comparison](#comparison).\n\n## Installation\n\nYou know the drill\n\n```bash\npip install unmarkd\n```\n\n## Comparison\n\n**TL;DR: Html2Text is fast. If you don\'t need much configuration, you could use Html2Text for the little speed increase.**\n\n<details>\n\n\n<summary>Click to expand</summary>\n\n### Speed\n\n**TL;DR: Unmarkd < Html2Text**\n\nHtml2Text is basically faster:\n\n![Benchmark](./assets/benchmark.png)\n\n(The `DOC` variable used can be found [here](./assets/benchmark.html))\n\nUnmarkd sacrifices speed for [power](#configurability).\n\nHtml2Text directly uses Python\'s [`html.parser`](https://docs.python.org/3/library/html.parser.html) module (in the standard library). On the other hand, Unmarkd uses the powerful HTML parsing library, `beautifulsoup4`. BeautifulSoup can be configured to use different HTML parsers. In Unmarkd, we configure it to use Python\'s `html.parser`, too.\n\nBut another layer of code means more code is ran.\n\nI hope that\'s a good explanation of the speed difference.\n\n### Correctness\n\n**TL;DR: Unmarkd == Html2Text**\n\nI actually found *two* html-to-markdown libraries. One of them was [Tomd](https://github.com/gaojiuli/tomd) which had an *incorrect implementation*:\n\n![Actual results](./assets/tomd_cant_handle.png)\n\nIt seems to be abandoned, anyway.\n\nNow with Html2Text and Unmarkd:\n\n![Epic showdown](./assets/correct.png)\n\n\nIn other words, they *work*\n\n### Configurability\n\n**TL;DR: Unmarkd > Html2Text**\n\nThis is Unmarkd\'s strong point.\n\nIn Html2Text, you only have a limited [set of options](https://github.com/Alir3z4/html2text/blob/master/docs/usage.md#available-options).\n\nIn Unmarkd, you can subclass the `BaseUnmarker` and implement conversions for new tags (e.g. `<q>`), etc. In my opinion, it\'s much easier to extend and configure Unmarkd.\n\nUnmarkd was originally written as a StackSearch dependancy.\n\nHtml2Text has no options for configuring parsing of code blocks. Unmarkd does\n\n</details>\n\n## Documentation\n\nHere\'s an example of basic usage\n\n```python\nimport unmarkd\nprint(unmarkd.unmark("<b>I <i>love</i> markdown!</b>"))\n# Output: **I *love* markdown!**\n```\n\nor something more complex (shamelessly taken from [here](https://markdowntohtml.com)):\n\n```python\nimport unmarkd\nhtml_doc = R"""<h1 id="sample-markdown">Sample Markdown</h1>\n<p>This is some basic, sample markdown.</p>\n<h2 id="second-heading">Second Heading</h2>\n<ul>\n<li>Unordered lists, and:<ol>\n<li>One</li>\n<li>Two</li>\n<li>Three</li>\n</ol>\n</li>\n<li>More</li>\n</ul>\n<blockquote>\n<p>Blockquote</p>\n</blockquote>\n<p>And <strong>bold</strong>, <em>italics</em>, and even <em>italics and later <strong>bold</strong></em>. Even <del>strikethrough</del>. <a href="https://markdowntohtml.com">A link</a> to somewhere.</p>\n<p>And code highlighting:</p>\n<pre><code class="lang-js"><span class="hljs-keyword">var</span> foo = <span class="hljs-string">\'bar\'</span>;\n\n<span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">baz</span><span class="hljs-params">(s)</span> </span>{\n   <span class="hljs-keyword">return</span> foo + <span class="hljs-string">\':\'</span> + s;\n}\n</code></pre>\n<p>Or inline code like <code>var foo = &#39;bar&#39;;</code>.</p>\n<p>Or an image of bears</p>\n<p><img src="http://placebear.com/200/200" alt="bears"></p>\n<p>The end ...</p>\n"""\nprint(unmarkd.unmark(html_doc))\n```\nand the output:\n\n```markdown\n    # Sample Markdown\n\n\n    This is some basic, sample markdown.\n\n    ## Second Heading\n\n\n\n    - Unordered lists, and:\n     1. One\n     2. Two\n     3. Three\n    - More\n\n    >Blockquote\n\n\n    And **bold**, *italics*, and even *italics and later **bold***. Even ~~strikethrough~~. [A link](https://markdowntohtml.com) to somewhere.\n\n    And code highlighting:\n\n\n    ```js\n    var foo = \'bar\';\n\n    function baz(s) {\n       return foo + \':\' + s;\n    }\n    ```\n\n\n    Or inline code like `var foo = \'bar\';`.\n\n    Or an image of bears\n\n    ![bears](http://placebear.com/200/200)\n\n    The end ...\n```\n### Extending\n\n#### Brief Overview\n\nMost functionality should be covered by the `BasicUnmarker` class defined in `unmarkd.unmarkers`.\n\nIf you need to reverse markdown from StackExchange (as in the case for my other project), you may use the `StackOverflowUnmarker` (or it\'s alias, `StackExchangeUnmarker`), which is also defined in `unmarkd.unmarkers`.\n\n#### Customizing\n\nIf the above two classes do not suit your needs, you can subclass the `unmarkd.unmarkers.BaseUnmarker` abstract class.\n\nCurrently, you can *optionally* override the following methods:\n\n - `detect_language` (parameters: **1**)\n    - **Parameters**:\n        - html: `bs4.BeautifulSoup`\n    - When a fenced code block is approached, this function is called with a parameter of type `bs4.BeautifulSoup` passed to it; this is the element the code block was detected from (i.e. `pre`).\n    - This function is responsible for detecting the programming language (or returning `\'\'` if none was detected) of the code block.\n    - Note: This method is different from `unmarkd.unmarkers.BasicUnmarker`. It is simpler and does less checking/filtering\n\n\nBut Unmarkd is more flexible than that.\n\n##### Customizable constants\n\nThere are currently 3 constants you may override:\n - Formats:\n    NOTE: Use the [**Format String Syntax**](https://docs.python.org/3/library/string.html#formatstrings)\n     - `UNORDERED_FORMAT`\n        - The string format of unordered (bulleted) lists.\n     - `ORDERED_FORMAT`\n        -  The string format of ordered (numbered) lists.\n - Miscellaneous:\n     - `ESCAPABLES`\n        - A container (preferably a `set`) of length-1 `str` that should be escaped\n\n##### Customize converting HTML tags\n\nFor an HTML tag `some_tag`, you can customize how it\'s converted to markdown by overriding a method like so:\n\n```python\nfrom unmarkd.unmarkers import BaseUnmarker\nclass MyCustomUnmarker(BaseUnmarker):\n    def tag_some_tag(self, child) -> str:\n        ...  # parse code here\n```\n\nTo reduce code duplication, if your tag also has aliases (e.g. `strong` is an alias for `b` in HTML) then you may modify the `TAG_ALIASES`.\n\nIf you really need to, you may also modify `DEFAULT_TAG_ALIASES`. Be warned: if you do so, **you will also need to implement the aliases** (currently `em` and `strong`).\n\n##### Utility functions when overriding\n\nYou may use (when extending) the following functions:\n\n - `__parse`, 2 parameters:\n    - `html`: *bs4.BeautifulSoup*\n        - The html to unmark. This is used internally by the `unmark` method and is slightly faster.\n    - `escape`: *bool*\n        - Whether to escape the characters inside the string or not. Defaults to `False`.\n - `escape`: 1 parameter:\n    - `string`: *str*\n        - The string to escape and make markdown-safe\n - `wrap`: 2 parameters:\n    - `element`: *bs4.BeautifulSoup*\n        - The element to wrap.\n    - `around_with`: *str*\n        - The character to wrap the element around with. **WILL NOT BE ESCPAED**\n - And, of course, `tag_*` and `detect_language`.\n',
-    'author': 'Bryan Hu',
-    'author_email': 'bryan.hu.2020@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ThatXliner/unmarkd/tree/master',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)[![codecov](https://codecov.io/gh/ThatXliner/unmarkd/branch/master/graph/badge.svg?token=PWVIERHTG3)](https://codecov.io/gh/ThatXliner/unmarkd) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml/badge.svg)](https://github.com/ThatXliner/unmarkd/actions/workflows/ci.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/unmarkd)](https://pypi.org/project/unmarkd/)
+
+> A markdown reverser.
+
+---
+
+Unmarkd is a [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)-powered [Markdown](https://en.wikipedia.org/wiki/Markdown) reverser written in Python and for Python.
+
+## Why
+
+This is created as a [StackSearch](http://github.com/ThatXliner/stacksearch) (one of my other projects) dependency. In order to create a better API, I needed a way to reverse HTML. So I created this.
+
+There are [similar projects](https://github.com/xijo/reverse_markdown) (written in Ruby) ~~but I have not found any written in Python (or for Python)~~ later I found a popular library, [html2text](https://github.com/Alir3z4/html2text).
+
+## Installation
+
+You know the drill
+
+```bash
+pip install unmarkd
+```
+
+## Comparison
+
+**TL;DR: Html2Text is fast. If you don't need much configuration, you could use Html2Text for the little speed increase.**
+
+<details>
+
+<summary>Click to expand</summary>
+
+### Speed
+
+**TL;DR: Unmarkd < Html2Text**
+
+Html2Text is basically faster:
+
+![Benchmark](./assets/benchmark.png)
+
+(The `DOC` variable used can be found [here](./assets/benchmark.html))
+
+Unmarkd sacrifices speed for [power](#configurability).
+
+Html2Text directly uses Python's [`html.parser`](https://docs.python.org/3/library/html.parser.html) module (in the standard library). On the other hand, Unmarkd uses the powerful HTML parsing library, `beautifulsoup4`. BeautifulSoup can be configured to use different HTML parsers. In Unmarkd, we configure it to use Python's `html.parser`, too.
+
+But another layer of code means more code is ran.
+
+I hope that's a good explanation of the speed difference.
+
+### Correctness
+
+**TL;DR: Unmarkd == Html2Text**
+
+I actually found _two_ html-to-markdown libraries. One of them was [Tomd](https://github.com/gaojiuli/tomd) which had an _incorrect implementation_:
+
+![Actual results](./assets/tomd_cant_handle.png)
+
+It seems to be abandoned, anyway.
+
+Now with Html2Text and Unmarkd:
+
+![Epic showdown](./assets/correct.png)
+
+In other words, they _work_
+
+### Configurability
+
+**TL;DR: Unmarkd > Html2Text**
+
+This is Unmarkd's strong point.
+
+In Html2Text, you only have a limited [set of options](https://github.com/Alir3z4/html2text/blob/master/docs/usage.md#available-options).
+
+In Unmarkd, you can subclass the `BaseUnmarker` and implement conversions for new tags (e.g. `<q>`), etc. In my opinion, it's much easier to extend and configure Unmarkd.
+
+Unmarkd was originally written as a StackSearch dependancy.
+
+Html2Text has no options for configuring parsing of code blocks. Unmarkd does
+
+</details>
+
+## Documentation
+
+Here's an example of basic usage
+
+```python
+import unmarkd
+print(unmarkd.unmark("<b>I <i>love</i> markdown!</b>"))
+# Output: **I *love* markdown!**
+```
+
+or something more complex (shamelessly taken from [here](https://markdowntohtml.com)):
+
+```python
+import unmarkd
+html_doc = R"""<h1 id="sample-markdown">Sample Markdown</h1>
+<p>This is some basic, sample markdown.</p>
+<h2 id="second-heading">Second Heading</h2>
+<ul>
+<li>Unordered lists, and:<ol>
+<li>One</li>
+<li>Two</li>
+<li>Three</li>
+</ol>
+</li>
+<li>More</li>
+</ul>
+<blockquote>
+<p>Blockquote</p>
+</blockquote>
+<p>And <strong>bold</strong>, <em>italics</em>, and even <em>italics and later <strong>bold</strong></em>. Even <del>strikethrough</del>. <a href="https://markdowntohtml.com">A link</a> to somewhere.</p>
+<p>And code highlighting:</p>
+<pre><code class="lang-js"><span class="hljs-keyword">var</span> foo = <span class="hljs-string">'bar'</span>;
+
+<span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">baz</span><span class="hljs-params">(s)</span> </span>{
+   <span class="hljs-keyword">return</span> foo + <span class="hljs-string">':'</span> + s;
 }
+</code></pre>
+<p>Or inline code like <code>var foo = &#39;bar&#39;;</code>.</p>
+<p>Or an image of bears</p>
+<p><img src="http://placebear.com/200/200" alt="bears"></p>
+<p>The end ...</p>
+"""
+print(unmarkd.unmark(html_doc))
+```
+
+and the output:
+
+````markdown
+    # Sample Markdown
+
+
+    This is some basic, sample markdown.
+
+    ## Second Heading
+
+
+
+    - Unordered lists, and:
+     1. One
+     2. Two
+     3. Three
+    - More
+
+    >Blockquote
+
+
+    And **bold**, *italics*, and even *italics and later **bold***. Even ~~strikethrough~~. [A link](https://markdowntohtml.com) to somewhere.
+
+    And code highlighting:
+
+
+    ```js
+    var foo = 'bar';
+
+    function baz(s) {
+       return foo + ':' + s;
+    }
+    ```
+
+
+    Or inline code like `var foo = 'bar';`.
+
+    Or an image of bears
+
+    ![bears](http://placebear.com/200/200)
+
+    The end ...
+````
+
+### Extending
+
+#### Brief Overview
+
+Most functionality should be covered by the `BasicUnmarker` class defined in `unmarkd.unmarkers`.
+
+If you need to reverse markdown from StackExchange (as in the case for my other project), you may use the `StackOverflowUnmarker` (or it's alias, `StackExchangeUnmarker`), which is also defined in `unmarkd.unmarkers`.
+
+#### Customizing
+
+If the above two classes do not suit your needs, you can subclass the `unmarkd.unmarkers.BaseUnmarker` abstract class.
+
+Currently, you can _optionally_ override the following methods:
+
+- `detect_language` (parameters: **1**)
+  - **Parameters**:
+    - html: `bs4.BeautifulSoup`
+  - When a fenced code block is approached, this function is called with a parameter of type `bs4.BeautifulSoup` passed to it; this is the element the code block was detected from (i.e. `pre`).
+  - This function is responsible for detecting the programming language (or returning `''` if none was detected) of the code block.
+  - Note: This method is different from `unmarkd.unmarkers.BasicUnmarker`. It is simpler and does less checking/filtering
+
+But Unmarkd is more flexible than that.
+
+##### Customizable constants
+
+There are currently 3 constants you may override:
+
+- Formats:
+  NOTE: Use the [**Format String Syntax**](https://docs.python.org/3/library/string.html#formatstrings)
+  - `UNORDERED_FORMAT`
+    - The string format of unordered (bulleted) lists.
+  - `ORDERED_FORMAT`
+    - The string format of ordered (numbered) lists.
+- Miscellaneous:
+  - `ESCAPABLES`
+    - A container (preferably a `set`) of length-1 `str` that should be escaped
+
+##### Customize converting HTML tags
+
+For an HTML tag `some_tag`, you can customize how it's converted to markdown by overriding a method like so:
+
+```python
+from unmarkd.unmarkers import BaseUnmarker
+class MyCustomUnmarker(BaseUnmarker):
+    def tag_some_tag(self, child) -> str:
+        ...  # parse code here
+```
+
+To reduce code duplication, if your tag also has aliases (e.g. `strong` is an alias for `b` in HTML) then you may modify the `TAG_ALIASES`.
+
+If you really need to, you may also modify `DEFAULT_TAG_ALIASES`. Be warned: if you do so, **you will also need to implement the aliases** (currently `em` and `strong`).
+
+##### Utility functions when overriding
+
+You may use (when extending) the following functions:
 
+- `__parse`, 2 parameters:
+  - `html`: _bs4.BeautifulSoup_
+    - The html to unmark. This is used internally by the `unmark` method and is slightly faster.
+  - `escape`: _bool_
+    - Whether to escape the characters inside the string or not. Defaults to `False`.
+- `escape`: 1 parameter:
+  - `string`: _str_
+    - The string to escape and make markdown-safe
+- `wrap`: 2 parameters:
+  - `element`: _bs4.BeautifulSoup_
+    - The element to wrap.
+  - `around_with`: _str_
+    - The character to wrap the element around with. **WILL NOT BE ESCPAED**
+- And, of course, `tag_*` and `detect_language`.
 
-setup(**setup_kwargs)
```

