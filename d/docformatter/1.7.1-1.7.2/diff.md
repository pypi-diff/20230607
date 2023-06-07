# Comparing `tmp/docformatter-1.7.1.tar.gz` & `tmp/docformatter-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.7.1.tar", max compression
+gzip compressed data, was "docformatter-1.7.2.tar", max compression
```

## Comparing `docformatter-1.7.1.tar` & `docformatter-1.7.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.1/LICENSE
--rw-r--r--   0        0        0     6864 2023-05-18 11:03:05.743440 docformatter-1.7.1/README.rst
--rw-r--r--   0        0        0     6191 2023-05-19 22:27:01.721656 docformatter-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1614 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     6251 2023-05-18 11:03:05.744440 docformatter-1.7.1/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-05-19 22:27:01.722656 docformatter-1.7.1/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    13256 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.7.1/src/docformatter/encode.py
--rw-r--r--   0        0        0    20564 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/format.py
--rw-r--r--   0        0        0     6998 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/strings.py
--rw-r--r--   0        0        0    23741 2023-05-19 22:01:42.795215 docformatter-1.7.1/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.1/src/docformatter/util.py
--rw-r--r--   0        0        0     8115 1970-01-01 00:00:00.000000 docformatter-1.7.1/setup.py
--rw-r--r--   0        0        0     8557 1970-01-01 00:00:00.000000 docformatter-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.2/LICENSE
+-rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.2/README.rst
+-rw-r--r--   0        0        0     6222 2023-06-07 03:06:35.281648 docformatter-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.2/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6501 2023-06-07 03:06:35.281648 docformatter-1.7.2/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.7.2/src/docformatter/encode.py
+-rw-r--r--   0        0        0    21022 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/format.py
+-rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.2/src/docformatter/strings.py
+-rw-r--r--   0        0        0    26471 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.2/src/docformatter/util.py
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 docformatter-1.7.2/PKG-INFO
```

### Comparing `docformatter-1.7.1/LICENSE` & `docformatter-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.1/README.rst` & `docformatter-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.1/pyproject.toml` & `docformatter-1.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.7.1"
+version = "1.7.2"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
@@ -91,14 +91,17 @@
     "too-many-return-statements",
     "useless-object-inheritance",
 ]
 
 [tool.docformatter]
 black = true
 non-strict = false
+non-cap = [
+	"docformatter",
+]
 
 [tool.pydocstyle]
 convention = "pep257"
 
 [tool.pytest.ini_options]
 markers = [
     "unit: mark the test as a unit test.",
```

### Comparing `docformatter-1.7.1/src/docformatter/__init__.py` & `docformatter-1.7.2/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.1/src/docformatter/__main__.py` & `docformatter-1.7.2/src/docformatter/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 
 
 def _help():
     """Print docformatter's help."""
     print(
         """\
 usage: docformatter [-h] [-i | -c] [-d] [-r] [-e [EXCLUDE ...]]
-                    [-n [NON-CAP ...]] [--black] [--wrap-summaries length]
+                    [-n [NON-CAP ...]] [-s [style]] [--rest-section-adorns REGEX]
+                    [--black] [--wrap-summaries length]
                     [--wrap-descriptions length] [--force-wrap]
                     [--tab-width width] [--blank] [--pre-summary-newline]
                     [--pre-summary-space] [--make-summary-multi-line]
                     [--close-quotes-on-newline] [--range line line]
                     [--docstring-length length length] [--non-strict]
                     [--config CONFIG] [--version] files [files ...]
 
@@ -65,14 +66,17 @@
   -n [NON-CAP ...], --non-cap [NON-CAP ...]
                         list of words not to capitalize when they appear as the
                         first word in the summary
 
   -s style, --style style
                         the docstring style to use when formatting parameter
                         lists.  One of epytext, sphinx. (default: sphinx)
+  --rest-section-adorns REGEX
+                        regular expression for identifying reST section adornments
+                        (default: [!\"#$%&'()*+,-./\\:;<=>?@[]^_`{|}~]{4,})
   --black               make formatting compatible with standard black options
                         (default: False)
   --wrap-summaries length
                         wrap long summary lines at this length; set to 0 to
                         disable wrapping (default: 79, 88 with --black option)
   --wrap-descriptions length
                         wrap descriptions at this length; set to 0 to disable
@@ -109,15 +113,15 @@
 
 def _main(argv, standard_out, standard_error, standard_in):
     """Run internal main entry point."""
     configurator = _configuration.Configurater(argv)
 
     if "--help" in configurator.args_lst:
         _help()
-        sys.exit()
+        return 0
     else:
         configurator.do_parse_arguments()
 
     formator = _format.Formatter(
         configurator.args,
         stderror=standard_error,
         stdin=standard_in,
```

### Comparing `docformatter-1.7.1/src/docformatter/__pkginfo__.py` & `docformatter-1.7.2/src/docformatter/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.7.1"
+__version__ = "1.7.2"
```

### Comparing `docformatter-1.7.1/src/docformatter/configuration.py` & `docformatter-1.7.2/src/docformatter/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,16 @@
         )
         self.parser.add_argument(
             "-n",
             "--non-cap",
             action="store",
             nargs="*",
             default=self.flargs_dct.get("non-cap", None),
-            help="list of words not to capitalize "
-            "when they appear as the "
-            "first word in the summary",
+            help="list of words not to capitalize when they appear as the first word "
+            "in the summary",
         )
         self.parser.add_argument(
             "--black",
             action="store_true",
             default=self.flargs_dct.get("black", "false").lower() == "true",
             help="make formatting compatible with standard black options "
             "(default: False)",
@@ -168,14 +167,23 @@
             "-s",
             "--style",
             default=self.flargs_dct.get("style", "sphinx"),
             help="name of the docstring style to use when formatting "
             "parameter lists (default: sphinx)",
         )
         self.parser.add_argument(
+            "--rest-section-adorns",
+            type=str,
+            dest="rest_section_adorns",
+            default=self.flargs_dct.get(
+                "rest_section_adorns", r"[!\"#$%&'()*+,-./:;<=>?@[\]^_`{|}~]{4,}"
+            ),
+            help="regex for identifying reST section header adornments",
+        )
+        self.parser.add_argument(
             "--wrap-summaries",
             default=int(self.flargs_dct.get("wrap-summaries", _default_wrap_summaries)),
             type=int,
             metavar="length",
             help="wrap long summary lines at this length; "
             "set to 0 to disable wrapping (default: 79, 88 with --black "
             "option)",
@@ -225,15 +233,15 @@
         self.parser.add_argument(
             "--pre-summary-space",
             action="store_true",
             default=self.flargs_dct.get(
                 "pre-summary-space", _default_pre_summary_space
             ).lower()
             == "true",
-            help="add a space after the opening triple quotes " "(default: False)",
+            help="add a space after the opening triple quotes (default: False)",
         )
         self.parser.add_argument(
             "--make-summary-multi-line",
             action="store_true",
             default=self.flargs_dct.get("make-summary-multi-line", "false").lower()
             == "true",
             help="add a newline before and after the summary of a one-line "
```

### Comparing `docformatter-1.7.1/src/docformatter/encode.py` & `docformatter-1.7.2/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.1/src/docformatter/format.py` & `docformatter-1.7.2/src/docformatter/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import contextlib
 import io
 import re
 import tokenize
 from typing import TextIO, Tuple
 
 # Third Party Imports
-import untokenize
+import untokenize  # type: ignore
 
 # docformatter Package Imports
 import docformatter.encode as _encode
 import docformatter.strings as _strings
 import docformatter.syntax as _syntax
 import docformatter.util as _util
 
@@ -173,15 +173,15 @@
         "U'''",
     )
     QUOTE_TYPES = STR_QUOTE_TYPES + RAW_QUOTE_TYPES + UCODE_QUOTE_TYPES
 
     parser = None
     """Parser object."""
 
-    args: argparse.Namespace = None
+    args: argparse.Namespace = argparse.Namespace()
 
     def __init__(
         self,
         args: argparse.Namespace,
         stderror: TextIO,
         stdin: TextIO,
         stdout: TextIO,
@@ -455,25 +455,33 @@
         _links = _syntax.do_find_links(contents)
         with contextlib.suppress(IndexError):
             if _links[0][0] == 0 and _links[0][1] == len(contents):
                 return docstring
 
         summary, description = _strings.split_summary_and_description(contents)
 
-        # Leave docstrings with underlined summaries alone.
+        # Leave docstrings with only field lists alone.
+        if _syntax.is_some_sort_of_field_list(summary, self.args.style):
+            return docstring
+
+        # Leave docstrings with underlined descriptions alone.
+        # TODO: Deprecate the remove_section_header method now that section headers
+        #  are being handled.
         if _syntax.remove_section_header(description).strip() != description.strip():
             return docstring
 
         if not self.args.force_wrap and (
             _syntax.is_some_sort_of_list(
                 summary,
                 self.args.non_strict,
+                self.args.rest_section_adorns,
                 self.args.style,
             )
             or _syntax.do_find_directives(summary)
+            or _syntax.do_find_links(summary)
         ):
             # Something is probably not right with the splitting.
             return docstring
 
         # Compensate for textwrap counting each tab in indentation as 1
         # character.
         tab_compensation = indentation.count("\t") * (self.args.tab_width - 1)
@@ -584,14 +592,15 @@
         ).lstrip()
         description = _syntax.wrap_description(
             description,
             indentation=indentation,
             wrap_length=self.args.wrap_descriptions,
             force_wrap=self.args.force_wrap,
             strict=self.args.non_strict,
+            rest_sections=self.args.rest_section_adorns,
             style=self.args.style,
         )
         post_description = "\n" if self.args.post_description_blank else ""
         return f'''\
 {open_quote}{pre_summary}{summary}
 
 {description}{post_description}
```

### Comparing `docformatter-1.7.1/src/docformatter/strings.py` & `docformatter-1.7.2/src/docformatter/strings.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.1/src/docformatter/syntax.py` & `docformatter-1.7.2/src/docformatter/syntax.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 # Standard Library Imports
 import contextlib
 import re
 import textwrap
 from typing import Iterable, List, Tuple, Union
 
+DEFAULT_INDENT = 4
+
 BULLET_REGEX = r"\s*[*\-+] [\S ]+"
 """Regular expression to use for finding bullet lists."""
 
 ENUM_REGEX = r"\s*\d\."
 """Regular expression to use for finding enumerated lists."""
 
 EPYTEXT_REGEX = r"@[a-zA-Z0-9_\-\s]+:"
@@ -47,18 +49,18 @@
 
 NUMPY_REGEX = r"^\s[a-zA-Z0-9_\- ]+ ?: [\S ]+"
 """Regular expression to use for finding Numpy-style field lists."""
 
 OPTION_REGEX = r"^-{1,2}[\S ]+ {2}\S+"
 """Regular expression to use for finding option lists."""
 
-REST_REGEX = r"(\.{2}|``) ?[\w-]+(:{1,2}|``)?"
+REST_REGEX = r"((\.{2}|`{2}) ?[\w.~-]+(:{2}|`{2})?[\w ]*?|`[\w.~]+`)"
 """Regular expression to use for finding reST directives."""
 
-SPHINX_REGEX = r":[a-zA-Z0-9_\- ]*:"
+SPHINX_REGEX = r":[a-zA-Z0-9_\-() ]*:"
 """Regular expression to use for finding Sphinx-style field lists."""
 
 URL_PATTERNS = (
     "afp|"
     "apt|"
     "bitcoin|"
     "chrome|"
@@ -362,28 +364,39 @@
     wrap_length : int
         The column to wrap each line at.
     style : str
         The docstring style to use for dealing with parameter lists.
 
     Returns
     -------
-    lines : list
+    _lines : list
         A list containing each line of the description with any links put
         back together.
     """
     _lines: List[str] = []
     _text_idx = 0
 
     # Check if the description contains any URLs.
     _url_idx = do_find_links(text)
 
     # Check if the description contains any field lists.
-    _parameter_idx, _wrap_parameters = do_find_field_lists(text, style)
+    _field_idx, _wrap_fields = do_find_field_lists(text, style)
 
-    if not _url_idx and not (_parameter_idx and _wrap_parameters):
+    # Field list wrapping takes precedence over URL wrapping.
+    for _fieldl, _fieldu in _field_idx:
+        for _key, _value in enumerate(_url_idx):
+            if (
+                _value[0] == _fieldl
+                or _value[0] == _fieldu
+                or _value[1] == _fieldl
+                or _value[1] == _fieldu
+            ):
+                _url_idx.pop(_key)
+
+    if not _url_idx and not (_field_idx and _wrap_fields):
         return description_to_list(
             text,
             indentation,
             wrap_length,
         )
 
     if _url_idx:
@@ -391,54 +404,54 @@
             text,
             _url_idx,
             0,
             indentation,
             wrap_length,
         )
 
-    if _parameter_idx:
-        _lines, _text_idx = do_wrap_parameter_lists(
+    if _field_idx:
+        _lines, _text_idx = do_wrap_field_lists(
             text,
-            _parameter_idx,
+            _field_idx,
             _lines,
             _text_idx,
             indentation,
             wrap_length,
         )
     else:
-        # Finally, add everything after the last field list directive.
+        # Finally, add everything after the last URL or field list directive.
         with contextlib.suppress(IndexError):
             _text = (
                 text[_text_idx + 1 :] if text[_text_idx] == "\n" else text[_text_idx:]
             ).splitlines()
             for _idx, _line in enumerate(_text):
                 if _line not in ["", "\n", f"{indentation}"]:
                     _text[_idx] = f"{indentation}{_line.strip()}"
 
             _lines += _text
 
     return _lines
 
 
-def do_wrap_parameter_lists(  # noqa: PLR0913
+def do_wrap_field_lists(  # noqa: PLR0913
     text: str,
-    parameter_idx: List[Tuple[int, int]],
+    field_idx: List[Tuple[int, int]],
     lines: List[str],
     text_idx: int,
     indentation: str,
     wrap_length: int,
 ) -> Tuple[List[str], int]:
-    """Wrap parameter lists in the long description.
+    """Wrap field lists in the long description.
 
     Parameters
     ----------
     text : str
         The long description text.
-    parameter_idx : list
-        The list of parameter list indices found in the description text.
+    field_idx : list
+        The list of field list indices found in the description text.
     lines : list
         The list of formatted lines in the description that come before the
         first parameter list item.
     text_idx : int
         The index in the description of the end of the last parameter list
         item.
     indentation : str
@@ -450,47 +463,40 @@
     -------
     lines, text_idx : tuple
          A list of the long description lines and the index in the long
         description where the last parameter list item ended.
     """
     lines.extend(
         description_to_list(
-            text[text_idx : parameter_idx[0][0]],
+            text[text_idx : field_idx[0][0]],
             indentation,
             wrap_length,
         )
     )
 
-    for _idx, _parameter in enumerate(parameter_idx):
-        try:
-            _parameter_description = text[
-                _parameter[1] : parameter_idx[_idx + 1][0]
-            ].strip()
-        except IndexError:
-            _parameter_description = text[_parameter[1] :].strip()
-
-        if len(_parameter_description) <= (wrap_length - len(indentation)):
-            lines.append(
-                f"{indentation}{text[_parameter[0]: _parameter[1]]} "
-                f"{_parameter_description}"
-            )
+    for _idx, __ in enumerate(field_idx):
+        _field_name = text[field_idx[_idx][0] : field_idx[_idx][1]]
+        _field_body = _do_join_field_body(
+            text,
+            field_idx,
+            _idx,
+        ).strip()
+
+        if len(f"{_field_name} {_field_body}") <= (wrap_length - len(indentation)):
+            if _field_body.startswith("`") or not _field_body:
+                _field = f"{_field_name}{_field_body}"
+            else:
+                _field = f"{_field_name} {_field_body}"
+            lines.append(f"{indentation}{_field}")
         else:
             lines.extend(
-                textwrap.wrap(
-                    textwrap.dedent(
-                        f"{text[_parameter[0]:_parameter[1]]} "
-                        f"{_parameter_description.replace(2*indentation, '')}"
-                    ),
-                    width=wrap_length,
-                    initial_indent=indentation,
-                    subsequent_indent=2 * indentation,
-                )
+                _do_wrap_field(_field_name, _field_body, indentation, wrap_length)
             )
 
-        text_idx = _parameter[1]
+        text_idx = field_idx[_idx][1]
 
     return lines, text_idx
 
 
 def do_wrap_urls(
     text: str,
     url_idx: Iterable,
@@ -533,20 +539,27 @@
             _lines.extend(
                 description_to_list(
                     text[text_idx : _url[0]],
                     indentation,
                     wrap_length,
                 )
             )
+
             with contextlib.suppress(IndexError):
-                if not text[_url[0] - len(indentation) - 2] == "\n" and not _lines[-1]:
+                if text[_url[0] - len(indentation) - 2] != "\n" and not _lines[-1]:
                     _lines.pop(-1)
 
-            # Add the URL.
-            _lines.append(f"{do_clean_url(text[_url[0] : _url[1]], indentation)}")
+            # Add the URL making sure that the leading quote is kept with a quoted URL.
+            _text = f"{text[_url[0]: _url[1]]}"
+            with contextlib.suppress(IndexError):
+                if _lines[0][-1] == '"':
+                    _lines[0] = _lines[0][:-2]
+                    _text = f'"{text[_url[0] : _url[1]]}'
+
+            _lines.append(f"{do_clean_url(_text, indentation)}")
 
             text_idx = _url[1]
 
     return _lines, text_idx
 
 
 def is_some_sort_of_field_list(
@@ -590,14 +603,15 @@
     return False
 
 
 # pylint: disable=line-too-long
 def is_some_sort_of_list(
     text: str,
     strict: bool,
+    rest_sections: str,
     style: str,
 ) -> bool:
     """Determine if docstring is a reST list.
 
     Notes
     -----
     There are five types of lists in reST/docutils that need to be handled.
@@ -633,14 +647,19 @@
             # "- parameter" <-- Bullet list
             # "+ parameter" <-- Bullet list
             re.match(BULLET_REGEX, line)
             or
             # "1. item" <-- Enumerated list
             re.match(ENUM_REGEX, line)
             or
+            # "====\ndescription\n====" <-- reST section
+            # "----\ndescription\n----" <-- reST section
+            # "description\n----" <-- reST section
+            re.match(rest_sections, line)
+            or
             # "-a  description" <-- Option list
             # "--long  description" <-- Option list
             re.match(OPTION_REGEX, line)
             or
             # "@param x:" <-- Epytext style
             # "@type x:" <-- Epytext style
             re.match(EPYTEXT_REGEX, line)
@@ -752,14 +771,15 @@
 
 def wrap_description(  # noqa: PLR0913
     text,
     indentation,
     wrap_length,
     force_wrap,
     strict,
+    rest_sections,
     style: str = "sphinx",
 ):
     """Return line-wrapped description text.
 
     We only wrap simple descriptions. We leave doctests, multi-paragraph text, and
     bulleted lists alone.
 
@@ -772,14 +792,16 @@
     wrap_length : int
         The line length at which to wrap long lines.
     force_wrap : bool
         Whether to force docformatter to wrap long lines when normally they
         would remain untouched.
     strict : bool
         Whether to strictly follow reST syntax to identify lists.
+    rest_sections : str
+        A regular expression used to find reST section header adornments.
     style : str
         The name of the docstring style to use when dealing with parameter
         lists (default is sphinx).
 
     Returns
     -------
     description : str
@@ -795,15 +817,83 @@
 
     # Ignore possibly complicated cases.
     if wrap_length <= 0 or (
         not force_wrap
         and (
             is_some_sort_of_code(text)
             or do_find_directives(text)
-            or is_some_sort_of_list(text, strict, style)
+            or is_some_sort_of_list(text, strict, rest_sections, style)
         )
     ):
         return text
 
     lines = do_split_description(text, indentation, wrap_length, style)
 
     return indentation + "\n".join(lines).strip()
+
+
+def _do_join_field_body(text, field_idx, idx):
+    """Join the filed body lines into a single line that can be wrapped.
+
+    Parameters
+    ----------
+    text : str
+        The docstring long description text that contains field lists.
+    field_idx : list
+        The list of tuples containing the found field list start and end position.
+
+    Returns
+    -------
+    _field_body : str
+        The field body collapsed into a single line.
+    """
+    try:
+        _field_body = text[field_idx[idx][1] : field_idx[idx + 1][0]].strip()
+    except IndexError:
+        _field_body = text[field_idx[idx][1] :].strip()
+
+    _field_body = " ".join(
+        [_line.strip() for _line in _field_body.splitlines()]
+    ).strip()
+
+    if _field_body:
+        _field_body = f" {_field_body}"
+
+    return _field_body
+
+
+def _do_wrap_field(field_name, field_body, indentation, wrap_length):
+    """Wrap complete field at wrap_length characters.
+
+    Parameters
+    ----------
+    field_name : str
+        The name text of the field.
+    field_body : str
+        The body text of the field.
+    indentation : str
+        The string to use for indentation of the first line in the field.
+    wrap_length : int
+        The number of characters at which to wrap the field.
+
+    Returns
+    -------
+    _wrapped_field : str
+        The field wrapped at wrap_length characters.
+    """
+    if len(indentation) > DEFAULT_INDENT:
+        _subsequent = indentation + int(0.5 * len(indentation)) * " "
+    else:
+        _subsequent = 2 * indentation
+
+    _wrapped_field = textwrap.wrap(
+        textwrap.dedent(f"{field_name} {field_body.strip()}"),
+        width=wrap_length,
+        initial_indent=indentation,
+        subsequent_indent=_subsequent,
+    )
+
+    for _idx, _field in enumerate(_wrapped_field):
+        _indent = indentation if _idx == 0 else _subsequent
+        _wrapped_field[_idx] = f"{_indent}{re.sub(' +', ' ', _field.strip())}"
+
+    return _wrapped_field
```

### Comparing `docformatter-1.7.1/src/docformatter/util.py` & `docformatter-1.7.2/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.1/setup.py` & `docformatter-1.7.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,254 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: docformatter
+Version: 1.7.2
+Summary: Formats docstrings to follow PEP 257
+Home-page: https://github.com/PyCQA/docformatter
+License: Expat
+Keywords: PEP 257,pep257,style,formatter,docstrings
+Author: Steven Myint
+Maintainer: Doyle Rowland
+Maintainer-email: doyle.rowland@reliaqual.com
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Provides-Extra: tomli
+Requires-Dist: charset_normalizer (>=3.0.0,<4.0.0)
+Requires-Dist: tomli (>=2.0.0,<3.0.0) ; (python_version < "3.11") and (extra == "tomli")
+Requires-Dist: untokenize (>=0.1.1,<0.2.0)
+Project-URL: Documentation, https://github.com/PyCQA/docformatter
+Project-URL: Repository, https://github.com/PyCQA/docformatter
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+============
+docformatter
+============
 
-packages = \
-['docformatter']
+.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master
+    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml
+.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter
+    :target: https://coveralls.io/github/PyCQA/docformatter
+.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter
+    :target: https://github.com/PyCQA/docformatter/graphs/contributors
+.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter
+.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1
+    :target: https://pycqa.github.io/isort/
+.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg
+    :target: https://github.com/PyCQA/docformatter
+.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg
+    :target: https://www.sphinx-doc.org/en/master/usage/index.html
+.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg
+    :target: https://numpydoc.readthedocs.io/en/latest/format.html
+.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg
+    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['charset_normalizer>=3.0.0,<4.0.0', 'untokenize>=0.1.1,<0.2.0']
-
-extras_require = \
-{'tomli:python_version < "3.11"': ['tomli>=2.0.0,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['docformatter = docformatter.__main__:main']}
-
-setup_kwargs = {
-    'name': 'docformatter',
-    'version': '1.7.1',
-    'description': 'Formats docstrings to follow PEP 257',
-    'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\n``docformatter`` formats docstrings compatible with ``black`` when passed the\n``--black`` option.\n\n``docformatter`` formats field lists that use Epytext or Sphinx styles.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter and you\'re using\nPython < 3.11::\n\n    $ pip install --upgrade docformatter[tomli]\n\nWith Python >=3.11, ``tomllib`` from the standard library is used.\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
-    'author': 'Steven Myint',
-    'author_email': 'None',
-    'maintainer': 'Doyle Rowland',
-    'maintainer_email': 'doyle.rowland@reliaqual.com',
-    'url': 'https://github.com/PyCQA/docformatter',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter
+.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter
+.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter
+.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter
+.. |DD| image:: https://img.shields.io/pypi/dd/docformatter
+.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases
 
++----------------+----------------------------------------------------------+
+| **Code**       + |BLACK| |ISORT|                                          +
++----------------+----------------------------------------------------------+
+| **Docstrings** + |SELF| |NUMPSTYLE|                                       +
++----------------+----------------------------------------------------------+
+| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +
++----------------+----------------------------------------------------------+
+| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +
++----------------+----------------------------------------------------------+
+
+Formats docstrings to follow `PEP 257`_.
+
+.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/
+
+Features
+========
+
+``docformatter`` automatically formats docstrings to follow a subset of the PEP
+257 conventions. Below are the relevant items quoted from PEP 257.
+
+- For consistency, always use triple double quotes around docstrings.
+- Triple quotes are used even though the string fits on one line.
+- Multi-line docstrings consist of a summary line just like a one-line
+  docstring, followed by a blank line, followed by a more elaborate
+  description.
+- Unless the entire docstring fits on a line, place the closing quotes
+  on a line by themselves.
+
+``docformatter`` also handles some of the PEP 8 conventions.
+
+- Don't write string literals that rely on significant trailing
+  whitespace. Such trailing whitespace is visually indistinguishable
+  and some editors (or more recently, reindent.py) will trim them.
+
+``docformatter`` formats docstrings compatible with ``black`` when passed the
+``--black`` option.
+
+``docformatter`` formats field lists that use Epytext or Sphinx styles.
+
+See the the full documentation at `read-the-docs`_, especially the
+`requirements`_ section for a more detailed discussion of PEP 257 and other
+requirements.
+
+.. _read-the-docs: https://docformatter.readthedocs.io
+.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html
+
+Installation
+============
+
+From pip::
+
+    $ pip install --upgrade docformatter
+
+Or, if you want to use pyproject.toml to configure docformatter and you're using
+Python < 3.11::
+
+    $ pip install --upgrade docformatter[tomli]
+
+With Python >=3.11, ``tomllib`` from the standard library is used.
+
+Or, if you want to use a release candidate (or any other tag)::
+
+    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>
+
+Where <RC_TAG> is the release candidate tag you'd like to install.  Release
+candidate tags will have the format v1.6.0-rc1  Release candidates will also be
+made available as a Github Release.
+
+Example
+=======
+
+After running::
+
+    $ docformatter --in-place example.py
+
+this code
+
+.. code-block:: python
+
+    """   Here are some examples.
+
+        This module docstring should be dedented."""
+
+
+    def launch_rocket():
+        """Launch
+    the
+    rocket. Go colonize space."""
+
+
+    def factorial(x):
+        '''
+
+        Return x factorial.
+
+        This uses math.factorial.
+
+        '''
+        import math
+        return math.factorial(x)
+
+
+    def print_factorial(x):
+        """Print x factorial"""
+        print(factorial(x))
+
+
+    def main():
+        """Main
+        function"""
+        print_factorial(5)
+        if factorial(10):
+            launch_rocket()
+
+
+gets formatted into this
+
+.. code-block:: python
+
+    """Here are some examples.
+
+    This module docstring should be dedented.
+    """
+
+
+    def launch_rocket():
+        """Launch the rocket.
+
+        Go colonize space.
+        """
+
+
+    def factorial(x):
+        """Return x factorial.
+
+        This uses math.factorial.
+        """
+        import math
+        return math.factorial(x)
+
+
+    def print_factorial(x):
+        """Print x factorial."""
+        print(factorial(x))
+
+
+    def main():
+        """Main function."""
+        print_factorial(5)
+        if factorial(10):
+            launch_rocket()
+
+Marketing
+=========
+Do you use *docformatter*?  What style docstrings do you use?  Add some badges to your project's **README** and let everyone know.
+
+|SELF|
+
+.. code-block::
+
+    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg
+        :target: https://github.com/PyCQA/docformatter
+
+|SPHINXSTYLE|
+
+.. code-block::
+
+    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg
+        :target: https://www.sphinx-doc.org/en/master/usage/index.html
+
+|NUMPSTYLE|
+
+.. code-block::
+
+    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg
+        :target: https://numpydoc.readthedocs.io/en/latest/format.html
+
+|GOOGSTYLE|
+
+.. code-block::
+
+    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg
+        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings
+
+Issues
+======
+
+Bugs and patches can be reported on the `GitHub page`_.
+
+.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues
 
-setup(**setup_kwargs)
```

