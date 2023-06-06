# Comparing `tmp/pipen_annotate-0.7.3.tar.gz` & `tmp/pipen_annotate-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_annotate-0.7.3.tar", max compression
+gzip compressed data, was "pipen_annotate-0.8.0.tar", max compression
```

## Comparing `pipen_annotate-0.7.3.tar` & `pipen_annotate-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/LICENSE
--rw-r--r--   0        0        0     1592 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/README.md
--rw-r--r--   0        0        0      108 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pipen_annotate/__init__.py
--rw-r--r--   0        0        0     7341 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pipen_annotate/annotate.py
--rw-r--r--   0        0        0    11354 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pipen_annotate/sections.py
--rw-r--r--   0        0        0      958 2023-06-02 23:08:05.758171 pipen_annotate-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.7.3/setup.py
--rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1592 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/README.md
+-rw-r--r--   0        0        0      108 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/pipen_annotate/__init__.py
+-rw-r--r--   0        0        0     7736 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/pipen_annotate/annotate.py
+-rw-r--r--   0        0        0    14710 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/pipen_annotate/sections.py
+-rw-r--r--   0        0        0     1525 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/pipen_annotate/utils.py
+-rw-r--r--   0        0        0      958 2023-06-06 23:37:48.460994 pipen_annotate-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.8.0/setup.py
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.8.0/PKG-INFO
```

### Comparing `pipen_annotate-0.7.3/LICENSE` & `pipen_annotate-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.3/README.md` & `pipen_annotate-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.7.3/pipen_annotate/annotate.py` & `pipen_annotate-0.8.0/pipen_annotate/annotate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
-import re
 import textwrap
+from abc import ABC
 from typing import Any, Callable, Type, MutableMapping
 
 from diot import OrderedDiot
+from liquid import Liquid
 from pipen import Proc, ProcGroup
-from pipen.utils import mark as proc_mark, get_marked as proc_get_marked
+from pipen.utils import mark, get_marked
 
+from .utils import indent as indent_text, FORMAT_INDENT, is_section
 from .sections import (
     Section,
     SectionSummary,
     SectionInput,
     SectionOutput,
     SectionEnvs,
     SectionItems,
@@ -33,69 +35,25 @@
     "References": SectionText,
     "Examples": SectionText,
     "Todo": SectionText,
     "Text": SectionText,
     "Items": SectionItems,
 }
 
-META_CONTAINER = "__meta__"
-
-
-def _mark(cls: type, **kwargs) -> type:
-    """Mark a class, not only a Proc
-
-    Args:
-        cls: The class to be marked
-        kwargs: The marks
-
-    Returns:
-        The marked class
-    """
-    if issubclass(cls, Proc):
-        return proc_mark(**kwargs)(cls)
-
-    if not getattr(cls, META_CONTAINER, None):
-        setattr(cls, META_CONTAINER, {})
-
-    meta = getattr(cls, META_CONTAINER)
-    meta.update(kwargs)
-    return cls
-
-
-def _get_marked(cls: type, mark_name: str, default: Any = None) -> Any:
-    """Get the marked value from a class, not only a Proc
-
-    Args:
-        cls: The class to get marked value from
-        mark_name: The mark name
-        default: The default value if not found
-
-    Returns:
-        The marked value
-    """
-    if issubclass(cls, Proc):
-        return proc_get_marked(cls, mark_name, default)
-
-    if not getattr(cls, META_CONTAINER, None):
-        setattr(cls, META_CONTAINER, {})
-
-    meta = getattr(cls, META_CONTAINER)
-    return meta.get(mark_name, default)
-
 
 def _annotate_uninherited(cls: type) -> OrderedDiot:
     """Annotate a Proc class with docstring, without inheriting from base.
 
     Args:
         cls: The class to be annotated.
 
     Returns:
         The annotated dict.
     """
-    annotated = OrderedDiot()
+    annotated = OrderedDiot(diot_nest=False)
     docstring = cls.__doc__
 
     if docstring:
         if docstring[0] in (" ", "\t"):
             docstring = textwrap.dedent(docstring)
         else:
             parts = docstring.split("\n", 1)
@@ -116,15 +74,15 @@
                     if section_name == "Args" and issubclass(cls, ProcGroup):
                         section = SectionProcGroupArgs(cls, section_name)
                     else:
                         section = SECTION_TYPES[section_name](
                             cls,
                             section_name,
                         )
-                elif re.sub(r"(?!^) ", "", line[:-1]).isidentifier():
+                elif is_section(line[:-1]):
                     annotated[section_name] = section.parse()
                     section_name = line[:-1]
                     section = SectionText(cls, section_name)
                 else:
                     section.consume(line)
             else:
                 section.consume(line)
@@ -137,24 +95,28 @@
         if "Input" not in annotated:
             annotated.Input = SectionInput(cls, "Input").parse()
         if "Output" not in annotated:
             annotated.Output = SectionOutput(cls, "Output").parse()
         if "Envs" not in annotated:
             annotated.Envs = SectionEnvs(cls, "Envs").parse()
 
+    if issubclass(cls, ProcGroup):
+        if "Args" not in annotated:
+            annotated.Args = SectionProcGroupArgs(cls, "Args").parse()
+
     return annotated
 
 
 def _update_annotation(
     base: OrderedDiot | None,
     other: OrderedDiot,
 ) -> OrderedDiot:
     """Update the annotation with another annotation."""
     if base is None:
-        base = OrderedDiot()
+        base = OrderedDiot(diot_nest=False)
     else:
         base = base.copy()
 
     for key, value in other.items():
         section_class = SECTION_TYPES.get(key)
         if key not in base or section_class is None:
             base[key] = value
@@ -169,40 +131,36 @@
 
     Args:
         cls: The class to be annotated.
 
     Returns:
         The annotated dict.
     """
-    annotated = _get_marked(cls, "annotate_annotated")
-    inherit = _get_marked(cls, "annotate_inherit", True)
+    annotated = get_marked(cls, "annotate_annotated")
+    inherit = get_marked(cls, "annotate_inherit", True)
+    is_proc_or_pg = issubclass(cls, Proc) or issubclass(cls, ProcGroup)
 
-    if not annotated:
+    if not annotated or not is_proc_or_pg:
         annotated = _annotate_uninherited(cls)
-        if issubclass(cls, Proc):
-            base = [
-                mro
-                for mro in cls.__mro__
-                if issubclass(mro, Proc)
-                and mro is not Proc
-                and mro is not cls
+        base = [
+            mro
+            for mro in cls.__mro__
+            if (
+                mro is not cls
                 and mro is not object
-            ]
-        else:
-            base = [
-                mro
-                for mro in cls.__mro__
-                if mro is not cls
-                and mro is not object
-            ]
+                and mro is not Proc
+                and mro is not ProcGroup
+                and mro is not ABC
+            )
+        ]
 
         base = base[0] if base else None
         annotated_base = annotate(base) if inherit and base else None
         annotated = _update_annotation(annotated_base, annotated)
-        _mark(cls, annotate_annotated=annotated)
+        mark(annotate_annotated=annotated)(cls)
 
     return annotated
 
 
 def _register_section(
     section: str,
     section_class: Type[Section] | str | None = None,
@@ -242,16 +200,66 @@
 
     Args:
         section: The section name.
     """
     SECTION_TYPES.pop(section, None)
 
 
-def _no_doc_inherit(proc: type) -> type:
-    """A decorator to disable docstring inheritance for a class"""
-    _mark(proc, annotate_inherit=False)
-    return proc
+def _format_doc(
+    cls: type | None = None,
+    /,
+    *,
+    base: type | None = None,
+    indent: int | str = 1,
+) -> type | Callable[[type], type]:
+    """Inherit docstring from base class.
+
+    Args:
+        cls: The class to be inherited.
+        base: The base class to inherit from.
+            if None, inherit from the first base class that is not object,
+            Proc, or ProcGroup.
+
+    Returns:
+        When cls is None, return a decorator.
+        When cls is not None, return the class with docstring inherited.
+    """
+    if cls is None:
+        return lambda c: _format_doc(c, base=base)
+
+    if base is None:
+        base = [
+            mro
+            for mro in cls.__mro__
+            if mro is not cls
+            and mro is not object
+            and mro is not Proc
+            and mro is not ProcGroup
+        ]
+
+        base = base[0] if base else None
+
+    if base is None:
+        return cls
+
+    if isinstance(indent, int):
+        indent = FORMAT_INDENT * indent
+
+    docstr = cls.__doc__
+    if docstr is None or not docstr.strip():
+        if not base.__doc__ or not base.__doc__.strip():
+            return cls
+
+        # If the class has no docstring, inherit from base class
+        cls.__doc__ = indent_text(base.__doc__, indent)
+        return cls
+
+    base_annotated = annotate(base)
+    docstr = Liquid(docstr, from_file=False).render(base=base_annotated)
+    cls.__doc__ = indent_text(docstr, indent)
+
+    return cls
 
 
 annotate.register_section = _register_section
 annotate.unregister_section = _unregister_section
-annotate.no_inherit = _no_doc_inherit
+annotate.format_doc = _format_doc
```

### Comparing `pipen_annotate-0.7.3/pipen_annotate/sections.py` & `pipen_annotate-0.8.0/pipen_annotate/sections.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from typing import List, Mapping, MutableMapping
+from typing import Any, List, Mapping, MutableMapping
 
 import re
-import textwrap
 import warnings
 
 from diot import Diot, OrderedDiot
 from pipen.defaults import ProcInputType
 
-__all__ = (
-    "SectionSummary",
-    "SectionInput",
-    "SectionOutput",
-    "SectionEnvs",
-    "SectionItems",
-    "SectionText",
+from .utils import (
+    FORMAT_INDENT,
+    dedent,
+    end_of_sentence,
+    cleanup_empty_lines,
 )
 
 ITEM_LINE_REGEX = re.compile(
     r"^(?P<name>[^\s]+)\s*(?:\((?P<attrs>.+?)\))?:(?P<help>.+)?$"
 )
 ITEM_ATTR_REGEX = re.compile(r"^(?P<name>[\w-]+)(?:\s*[:=]\s*(?P<value>.+))?$")
 
@@ -28,81 +25,189 @@
     """Raised when the annotation is malformatted"""
 
 
 class UnknownAnnotationItemWarning(Warning):
     """Raised when the annotation item is unknown"""
 
 
-def _dedent(lines: List[str]) -> List[str]:
-    """Dedent a list of lines.
-    """
-    return textwrap.dedent("\n".join(lines)).splitlines()
+class Mixin:
 
+    def _set_meta(self, key: str, value: Any) -> None:
+        self.__diot__[f"_{key}"] = value
 
-def _end_of_sentence(line: str) -> bool:
-    """Check if a line ends with a sentence.
-    """
-    return (
-        line.endswith(".")
-        or line.endswith("?")
-        or line.endswith("!")
-        or line.endswith(":")
-    )
+    def _get_meta(self, key: str) -> Any:
+        return self.__diot__.get(f"_{key}")
+
+    def __iadd__(self, other: str) -> str:
+        return f"{self}{other}"
+
+
+class ItemAttrs(Mixin, OrderedDiot):
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("diot_nest", False)
+        super().__init__(*args, **kwargs)
+        self._set_meta("origin", [])
+
+    def __str__(self) -> str:
+        out = []
+        for key in self._get_meta("origin"):
+            value = self[key]
+            if value is True:
+                out.append(key)
+            else:
+                out.append(f"{key}={value}")
+        return ";".join(out)
+
+
+class ItemTerm(Mixin, Diot):
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("diot_nest", False)
+        super().__init__(*args, **kwargs)
+        self._set_meta("raw_help", [])
+        self._set_meta("prefix", None)
+
+    def __str__(self) -> str:
+        out = self._get_meta("prefix") or ""
+        out += self.name
+        if self.attrs._get_meta("origin"):
+            out += f" ({self.attrs})"
+        out += ":"
+
+        raw_help = self._get_meta("raw_help")
+        if raw_help:
+            out += " " + raw_help[0]
+
+        for line in raw_help[1:]:
+            out += f"\n{FORMAT_INDENT}{line}"
+
+        if self.terms:
+            out += f"\n{self.terms}"
+
+        return out
+
+
+class ItemTerms(Mixin, OrderedDiot):
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("diot_nest", False)
+        super().__init__(*args, **kwargs)
+        self._set_meta("name", None)
+        self._set_meta("level", 0)
+
+    def __str__(self) -> str:
+        name = self._get_meta("name")
+        out = []
+        level = self._get_meta("level")
+        if name:
+            out.append(f"{FORMAT_INDENT * level}{name}:")
+
+        for term in self.values():
+            out.extend(
+                (f"{FORMAT_INDENT * (level + 1)}{line}")
+                for line in str(term).splitlines()
+            )
+        return "\n".join(out)
+
+
+class SummaryParsed(Mixin, Diot):
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("diot_nest", False)
+        super().__init__(*args, **kwargs)
+
+    def __str__(self) -> str:
+        return f"{self.short}\n\n{self.long}"
+
+
+class TextLines(list):
+
+    def __str__(self) -> str:  # pragma: no cover
+        return "\n".join(self)
+
+    # For jinja2/Liquid to work
+    def splitlines(self):
+        return cleanup_empty_lines(self)
+
+
+class TextParsed(Mixin, Diot):
+
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault("diot_nest", False)
+        super().__init__(*args, **kwargs)
+
+    def __str__(self) -> str:
+        name = self._get_meta("name")
+        out = f"{name}:\n" if name else ""
+        out += "\n".join(f"{FORMAT_INDENT}{line}" for line in self.lines)
+        return out
 
 
 def _parse_terms(
     lines: List[str],
     prefix: str | None = None,
-) -> Diot:
+    level: int = 0,
+    name: str | None = None,
+) -> ItemTerms:
     """Parse a list of lines as terms.
     """
-    terms = OrderedDiot()
-    lines = _dedent(lines)
+    terms = ItemTerms()
+    terms._set_meta("name", name)
+    terms._set_meta("level", level)
+    lines = dedent(lines)
     sublines = []
     item = None
     just_matched = False
     help_continuing = False
     for line in lines:
         if prefix:
             matched = ITEM_LINE_REGEX.match(line[len(prefix):])
         else:
             matched = ITEM_LINE_REGEX.match(line)
 
         lstripped_line = line.lstrip()
         if matched:
             if item:
                 # See if we have sub-terms
-                item.terms = _parse_terms(sublines, prefix="- ")
+                item.terms = _parse_terms(sublines, "- ", level + 1)
                 sublines.clear()
 
             # Create a new item
             name = matched.group("name")
             attrs = matched.group("attrs")
             help = matched.group("help")
-            terms[name] = Diot(attrs={}, terms={}, help="")
+            terms[name] = ItemTerm(
+                name=name,
+                attrs=ItemAttrs(),
+                terms=ItemTerms(),
+                help="",
+            )
+            terms[name]._set_meta("prefix", prefix)
 
             if attrs:
                 for attr in attrs.split(";"):
                     attr = attr.strip()
                     attr_matched = ITEM_ATTR_REGEX.match(attr)
                     if not attr_matched:
                         raise MalFormattedAnnotationError(
                             f"\nInvalid item attribute: {attr}"
                             "\nExpecting: <name>[:=]<value>"
                             f"\nFull attributes: {attrs}"
                         )
                     attr_name = attr_matched.group("name")
                     attr_value = attr_matched.group("value")
-
+                    terms[name].attrs._get_meta("origin").append(attr_name)
                     terms[name].attrs[attr_name] = (
                         True if attr_value is None else attr_value
                     )
 
             if help is not None:
                 terms[name].help = help.strip()
+                terms[name]._get_meta("raw_help").append(terms[name].help)
                 if terms[name].help == "|":
                     help_continuing = True
 
             item = terms[name]
             just_matched = True
         elif item is None:
             raise MalFormattedAnnotationError(
@@ -112,33 +217,34 @@
         elif just_matched and not lstripped_line.startswith("- "):
             if help_continuing and item.help == "|":
                 sep = item.help = ""
             else:
                 sep = (
                     "\n"
                     if help_continuing
-                    or _end_of_sentence(item.help)
+                    or end_of_sentence(item.help)
                     or lstripped_line.startswith(">>>")
                     or (
                         item.help
                         and item.help.splitlines()[-1].startswith(">>>")
                     )
                     else " "
                 )
+            item._get_meta("raw_help").append(lstripped_line)
             item.help = f"{item.help}{sep}{lstripped_line}"
         elif lstripped_line.startswith("- "):
             sublines.append(line)
             just_matched = False
             help_continuing = False
         else:
             sublines.append(line)
 
     if item:
         # See if we have sub-terms
-        item.terms = _parse_terms(sublines, prefix="- ")
+        item.terms = _parse_terms(sublines, prefix="- ", level=level + 1)
 
     return terms
 
 
 def _parse_one_output(out: str) -> List[str] | None:
     """Parse one output item, such as `out:file:<outfile>`"""
     parts = out.split(":")
@@ -156,15 +262,20 @@
 ) -> None:
     """Update the attrs of parsed terms with the class envs."""
     envs = envs or {}
     for key, value in envs.items():
         whole_key = f"{prev_key}.{key}" if prev_key else key
 
         if key not in parsed:
-            parsed[key] = Diot(attrs={}, terms={}, help="")
+            parsed[key] = ItemTerm(
+                name=key,
+                attrs=ItemAttrs(),
+                terms=ItemTerms(),
+                help="",
+            )
 
         if (
             parsed[key].attrs.get("ns", False)
             or parsed[key].attrs.get("namespace", False)
             or parsed[key].attrs.get("action", "") in ("ns", "namespace")
             or (isinstance(value, dict) and parsed[key].terms)
         ):
@@ -202,15 +313,15 @@
         self._cls = cls
         self._lines: List[str] = []
 
     def consume(self, line: str) -> None:
         self._lines.append(line)
 
     @abstractmethod
-    def parse(self) -> str | Diot | List[str]:  # pragma: no cover
+    def parse(self) -> Diot:  # pragma: no cover
         pass
 
     @classmethod
     def update_parsed(
         cls,
         base: str | List[str] | MutableMapping,
         other: str | List[str] | MutableMapping,
@@ -222,33 +333,33 @@
             return base + other
 
         base = base.copy()
         base.update(other)
         return base
 
 
-class SectionSummary(Section):
+class SectionSummary(Mixin, Section):
 
-    def parse(self) -> str | Diot | List[str]:
+    def parse(self) -> Diot:
         """Parse the summary section."""
         lines = self._lines
         if lines:
             if lines[0] and lines[0][0] in (" ", "\t"):
-                lines = _dedent(self._lines)
+                lines = dedent(self._lines)
             else:
-                lines = [lines[0]] + _dedent(lines[1:])
+                lines = [lines[0]] + dedent(lines[1:])
 
         short = long = ""
         for i, line in enumerate(lines):
             if not line:
                 long = "\n".join(lines[i + 1:])
                 break
             short += line + " "
 
-        return Diot(short=short.rstrip(), long=long)
+        return SummaryParsed(short=short.rstrip(), long=long)
 
     @classmethod
     def update_parsed(
         cls,
         base: str | List[str] | MutableMapping,
         other: str | List[str] | MutableMapping,
     ) -> str | List[str] | MutableMapping:
@@ -257,19 +368,19 @@
         if other.short:
             base.short = other.short
         if other.long:
             base.long = other.long
         return base
 
 
-class SectionItems(Section):
+class SectionItems(Mixin, Section):
 
-    def parse(self) -> str | Diot | List[str]:
+    def parse(self) -> Diot:
         try:
-            return _parse_terms(self._lines)
+            return _parse_terms(self._lines, name=self.name)
         except MalFormattedAnnotationError as e:
             raise MalFormattedAnnotationError(
                 f"[{self._cls.__name__}/{self.name}] {e}"
             ) from None
 
     @classmethod
     def update_parsed(
@@ -279,15 +390,15 @@
     ) -> str | List[str] | MutableMapping:
         """Update the parsed result with the other result."""
         return _update_terms(base, other)
 
 
 class SectionInput(SectionItems):
 
-    def parse(self) -> str | Diot | List[str]:
+    def parse(self) -> Diot:
         parsed = super().parse()
         input_keys = self._cls.input
 
         if isinstance(input_keys, str):
             input_keys = [
                 input_key.strip() for input_key in input_keys.split(",")
             ]
@@ -296,17 +407,18 @@
         for input_key_type in input_keys or []:
             if ":" not in input_key_type:
                 input_key_type = f"{input_key_type}:{ProcInputType.VAR}"
 
             input_key, input_type = input_key_type.split(":", 1)
             input_key_names.add(input_key)
             if input_key not in parsed:
-                parsed[input_key] = Diot(
-                    attrs={"itype": input_type},
-                    terms={},
+                parsed[input_key] = ItemTerm(
+                    name=input_key,
+                    attrs=ItemAttrs(itype=input_type),
+                    terms=ItemTerms(),
                     help="",
                 )
             else:
                 parsed[input_key].attrs["itype"] = input_type
 
             parsed[input_key].attrs["nargs"] = "+"
             if input_type in (ProcInputType.FILES, ProcInputType.DIRS):
@@ -322,35 +434,38 @@
             )
 
         return parsed
 
 
 class SectionOutput(SectionItems):
 
-    def parse(self) -> str | Diot | List[str]:
+    def parse(self) -> Diot:
         output = self._cls.output
         if not output:
-            return Diot()
+            out = ItemTerms()
+            out._set_meta("name", self.name)
+            return out
 
         parsed = super().parse()
 
         if not isinstance(output, (list, tuple)):
             output = [out.strip() for out in output.split(",")]
 
         out_names = set()
         for out in output:
             parts = _parse_one_output(out)
             if not parts:
                 continue
 
             out_names.add(parts[0])
             if parts[0] not in parsed:
-                parsed[parts[0]] = Diot(
-                    attrs={"otype": parts[1], "default": parts[2]},
-                    terms={},
+                parsed[parts[0]] = ItemTerm(
+                    name=parts[0],
+                    attrs=ItemAttrs(otype=parts[1], default=parts[2]),
+                    terms=ItemTerms(),
                     help="",
                 )
             else:
                 parsed[parts[0]].attrs["otype"] = parts[1]
                 parsed[parts[0]].attrs["default"] = parts[2]
 
         if set(parsed) - out_names:
@@ -361,25 +476,29 @@
             )
 
         return parsed
 
 
 class SectionEnvs(SectionItems):
 
-    def parse(self) -> str | Diot | List[str]:
+    def parse(self) -> Diot:
         parsed = super().parse()
         _update_attrs_with_cls(parsed, self._cls.envs)
         return parsed
 
 
 class SectionProcGroupArgs(SectionItems):
 
-    def parse(self) -> str | Diot | List[str]:
+    def parse(self) -> Diot:
         parsed = super().parse()
         _update_attrs_with_cls(parsed, self._cls.DEFAULTS)
         return parsed
 
 
 class SectionText(Section):
 
-    def parse(self) -> str | Diot | List[str]:
-        return "\n".join(_dedent(self._lines))
+    def parse(self) -> Diot:
+        lines = dedent(self._lines)
+        lines = cleanup_empty_lines(lines)
+        out = TextParsed(lines=TextLines(lines))
+        out._set_meta("name", self.name)
+        return out
```

### Comparing `pipen_annotate-0.7.3/pyproject.toml` & `pipen_annotate-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-annotate"
-version = "0.7.3"
+version = "0.8.0"
 description = "Use docstring to annotate pipen processes"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `pipen_annotate-0.7.3/setup.py` & `pipen_annotate-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pipen>=0.9,<0.10']
 
 setup_kwargs = {
     'name': 'pipen-annotate',
-    'version': '0.7.3',
+    'version': '0.8.0',
     'description': 'Use docstring to annotate pipen processes',
     'long_description': '# pipen-annotate\n\nUse docstring to annotate [pipen](https://github.com/pwwang/pipen) processes\n\n## Installation\n\n```shell\npip install -U pipen-annotate\n```\n\n## Usage\n\n```python\nfrom pprint import pprint\nfrom pipen import Proc\nfrom pipen_annotate import annotate\n\n\nclass Process(Proc):\n    """Short description\n\n    Long description\n\n    Input:\n        infile: An input file\n        invar: An input variable\n\n    Output:\n        outfile: The output file\n\n    Envs:\n        ncores: Number of cores\n    """\n    input = "infile:file, invar"\n    output = "outfile:file:output.txt"\n    args = {\'ncores\': 1}\n\nannotated = annotate(Process)\n# prints:\n{\'Envs\': {\'ncores\': {\'attrs\': OrderedDiot([(\'default\', 1)]),\n                     \'help\': \'Number of cores\',\n                     \'terms\': OrderedDiot([])}},\n \'Input\': {\'infile\': {\'attrs\': {\'action\': \'extend\',\n                                \'itype\': \'file\',\n                                \'nargs\': \'+\'},\n                      \'help\': \'An input file\',\n                      \'terms\': OrderedDiot([])},\n           \'invar\': {\'attrs\': {\'action\': \'extend\',\n                               \'itype\': \'var\',\n                               \'nargs\': \'+\'},\n                     \'help\': \'An input variable\',\n                     \'terms\': OrderedDiot([])}},\n \'Output\': {\'outfile\': {\'attrs\': {\'default\': \'output.txt\',\n                                  \'otype\': \'file\'},\n                        \'help\': \'The output file\',\n                        \'terms\': OrderedDiot([])}},\n \'Summary\': {\'long\': \'Long description\\n\',\n             \'short\': \'Short description\'}}\n```\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_annotate-0.7.3/PKG-INFO` & `pipen_annotate-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-annotate
-Version: 0.7.3
+Version: 0.8.0
 Summary: Use docstring to annotate pipen processes
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

