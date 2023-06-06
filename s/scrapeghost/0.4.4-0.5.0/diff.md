# Comparing `tmp/scrapeghost-0.4.4.tar.gz` & `tmp/scrapeghost-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeghost-0.4.4.tar", max compression
+gzip compressed data, was "scrapeghost-0.5.0.tar", max compression
```

## Comparing `scrapeghost-0.4.4.tar` & `scrapeghost-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18032 2023-03-20 02:41:03.735166 scrapeghost-0.4.4/LICENSE.md
--rw-r--r--   0        0        0     2397 2023-03-24 23:43:59.976785 scrapeghost-0.4.4/README.md
--rw-r--r--   0        0        0      779 2023-03-31 16:54:48.380006 scrapeghost-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      129 2023-03-23 05:45:31.983727 scrapeghost-0.4.4/src/scrapeghost/__init__.py
--rw-r--r--   0        0        0     7430 2023-03-26 17:59:21.157961 scrapeghost-0.4.4/src/scrapeghost/apicall.py
--rw-r--r--   0        0        0     1424 2023-03-23 05:45:31.984531 scrapeghost-0.4.4/src/scrapeghost/cli.py
--rw-r--r--   0        0        0      348 2023-03-22 20:30:45.431201 scrapeghost-0.4.4/src/scrapeghost/errors.py
--rw-r--r--   0        0        0     4503 2023-03-27 21:28:21.626622 scrapeghost-0.4.4/src/scrapeghost/postprocessors.py
--rw-r--r--   0        0        0     1355 2023-03-24 23:01:32.548716 scrapeghost-0.4.4/src/scrapeghost/preprocessors.py
--rw-r--r--   0        0        0        0 2023-03-22 07:13:24.569881 scrapeghost-0.4.4/src/scrapeghost/py.typed
--rw-r--r--   0        0        0      460 2023-03-23 06:09:37.973075 scrapeghost-0.4.4/src/scrapeghost/responses.py
--rw-r--r--   0        0        0     9051 2023-03-27 21:28:21.627186 scrapeghost-0.4.4/src/scrapeghost/scrapers.py
--rw-r--r--   0        0        0     1133 2023-03-23 05:45:31.985498 scrapeghost-0.4.4/src/scrapeghost/utils.py
--rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 scrapeghost-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    18032 2023-03-20 02:41:03.735166 scrapeghost-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     2397 2023-03-24 23:43:59.976785 scrapeghost-0.5.0/README.md
+-rw-r--r--   0        0        0      779 2023-06-06 22:39:24.524883 scrapeghost-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-06 08:14:17.157308 scrapeghost-0.5.0/src/scrapeghost/__init__.py
+-rw-r--r--   0        0        0     7430 2023-03-26 17:59:21.157961 scrapeghost-0.5.0/src/scrapeghost/apicall.py
+-rw-r--r--   0        0        0     1464 2023-06-06 08:14:17.157856 scrapeghost-0.5.0/src/scrapeghost/cli.py
+-rw-r--r--   0        0        0      348 2023-03-22 20:30:45.431201 scrapeghost-0.5.0/src/scrapeghost/errors.py
+-rw-r--r--   0        0        0     4603 2023-06-06 08:19:17.686537 scrapeghost-0.5.0/src/scrapeghost/postprocessors.py
+-rw-r--r--   0        0        0     1355 2023-03-24 23:01:32.548716 scrapeghost-0.5.0/src/scrapeghost/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-03-22 07:13:24.569881 scrapeghost-0.5.0/src/scrapeghost/py.typed
+-rw-r--r--   0        0        0      460 2023-03-23 06:09:37.973075 scrapeghost-0.5.0/src/scrapeghost/responses.py
+-rw-r--r--   0        0        0     9934 2023-06-06 22:37:38.898310 scrapeghost-0.5.0/src/scrapeghost/scrapers.py
+-rw-r--r--   0        0        0     1133 2023-03-23 05:45:31.985498 scrapeghost-0.5.0/src/scrapeghost/utils.py
+-rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 scrapeghost-0.5.0/PKG-INFO
```

### Comparing `scrapeghost-0.4.4/LICENSE.md` & `scrapeghost-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.4.4/README.md` & `scrapeghost-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.4.4/pyproject.toml` & `scrapeghost-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapeghost"
-version = "0.4.4"
+version = "0.5.0"
 description = "An experimental library for scraping websites using GPT."
 authors = ["James Turk <dev@jamesturk.net>"]
 license = "Hippocratic License HL3-EXTR-FFD-LAW-MIL-SV"
 readme = "README.md"
 
 [tool.poetry.scripts]
 scrapeghost = 'scrapeghost.cli:main'
```

### Comparing `scrapeghost-0.4.4/src/scrapeghost/apicall.py` & `scrapeghost-0.5.0/src/scrapeghost/apicall.py`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.4.4/src/scrapeghost/cli.py` & `scrapeghost-0.5.0/src/scrapeghost/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,13 +34,13 @@
         scraper.preprocessors.append(XPath(xpath))
     if css:
         scraper.preprocessors.append(CSS(css))
     result = scraper(url)
     typer.echo(json.dumps(result.data))
 
 
-def main() -> None:
+def main() -> None:  # pragma: no cover
     typer.run(scrape)
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `scrapeghost-0.4.4/src/scrapeghost/postprocessors.py` & `scrapeghost-0.5.0/src/scrapeghost/postprocessors.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 from pydantic import ValidationError
 
 from .utils import logger, _tostr
 from .errors import InvalidJSON, PostprocessingError
 from .responses import Response, ScrapeResponse
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from .apicall import OpenAiCall
     from .scrapers import SchemaScraper
 
 
 class JSONPostprocessor:
     def __init__(self, nudge: bool = True):
         self.nudge = nudge
@@ -26,15 +26,15 @@
 
         try:
             response.data = json.loads(response.data)
         except json.JSONDecodeError:
             if hasattr(scraper, "scrape") and self.nudge:
                 # call nudge and try again
                 response = self.nudge_json(scraper, response)  # type: ignore
-                if not isinstance(response.data, str):
+                if not isinstance(response.data, str):  # pragma: no cover
                     raise PostprocessingError(
                         f"Response data is not a string: {response.data}"
                     )
                 try:
                     response.data = json.loads(response.data)
                 except json.JSONDecodeError:
                     # if still invalid, raise error
@@ -65,15 +65,15 @@
         )
 
 
 class PydanticPostprocessor:
     def __init__(self, model: type):
         self.pydantic_model = model
 
-    def __str__(self) -> str:
+    def __str__(self) -> str:  # pragma: no cover
         return f"PydanticPostprocessor({self.pydantic_model})"
 
     def __call__(self, response: Response, scraper: OpenAiCall) -> Response:
         if not isinstance(response.data, dict):
             raise PostprocessingError(
                 "PydanticPostprocessor expecting a dict, "
                 "ensure JSONPostprocessor or equivalent is used first."
@@ -94,19 +94,19 @@
 
     Default behavior is to check all top-level strings.
 
     If you desire more control, subclass this class and
     register it as a postprocessor.
     """
 
-    def __str__(self) -> str:
+    def __str__(self) -> str:  # pragma: no cover
         return "HallucinationChecker"
 
     def __call__(self, response: Response, scraper: OpenAiCall) -> Response:
-        if not isinstance(response, ScrapeResponse):
+        if not isinstance(response, ScrapeResponse):  # pragma: no cover
             raise PostprocessingError(
                 "HallucinationChecker expects ScrapeResponse, "
                 "Incompatible with auto_split_length"
             )
         html = _tostr(response.parsed_html)
 
         _check_data_in_html(html, response.data)
```

### Comparing `scrapeghost-0.4.4/src/scrapeghost/preprocessors.py` & `scrapeghost-0.5.0/src/scrapeghost/preprocessors.py`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.4.4/src/scrapeghost/scrapers.py` & `scrapeghost-0.5.0/src/scrapeghost/scrapers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 import json
+import typing
 import requests
 import lxml.html
 
+from typing import Any, Sequence
 from .errors import PreprocessorError
 from .responses import Response, ScrapeResponse
 from .apicall import OpenAiCall, Postprocessor
 from .utils import logger, _tokens, _tostr
 from .preprocessors import Preprocessor, CleanHTML
 from .postprocessors import (
     JSONPostprocessor,
@@ -34,15 +36,15 @@
         if isinstance(schema, (list, dict)):
             self.json_schema = json.dumps(schema)
         elif isinstance(schema, str):
             self.json_schema = schema
         elif hasattr(schema, "schema"):
             self.json_schema = _pydantic_to_simple_schema(schema)
             use_pydantic = True
-        else:
+        else:  # pragma: no cover
             raise ValueError(f"Invalid schema: {schema}")
 
         _default_postprocessors: list[Postprocessor]
         if auto_split_length:
             json_type = "list of JSON objects"
             _default_postprocessors = [
                 JSONPostprocessor(nudge=False),
@@ -57,15 +59,15 @@
             self.postprocessors = _default_postprocessors
         else:
             self.postprocessors = postprocessors
 
         self.system_messages = [
             f"For the given HTML, convert to a {json_type} matching this schema: "
             f"{self.json_schema}",
-            "Responses should be valid JSON, with no other text. "
+            "Limit responses to valid JSON, with no explanatory text. "
             "Never truncate the JSON with an ellipsis. "
             "Always use double quotes for strings and escape quotes with \\. "
             "Always omit trailing commas. ",
         ]
         if extra_instructions:
             self.system_messages.extend(extra_instructions)
 
@@ -141,15 +143,17 @@
                 _combine_responses(sr, [self._api_request(html)])
             )
 
     # allow the class to be called like a function
     __call__ = scrape
 
 
-def _combine_responses(sr: ScrapeResponse, responses: list[Response]) -> ScrapeResponse:
+def _combine_responses(
+    sr: ScrapeResponse, responses: Sequence[Response]
+) -> ScrapeResponse:
     """
     Combine (possibly paginated) API responses into a single ScrapeResponse.
     """
     sr.api_responses = [
         api_resp for resp in responses for api_resp in resp.api_responses
     ]
     sr.total_cost = sum([resp.total_cost for resp in responses])
@@ -221,43 +225,61 @@
 
     We don't use Pydantic's schema() method because the
     additional complexity of JSON Schema adds a lot of extra tokens
     and in testing did not work as well as the simplified versions.
     """
     schema = {}
     for field in pydantic_model.__fields__.values():  # type: ignore
+        # __fields__ is present on Pydantic models, so can process recursively
         if hasattr(field.outer_type_, "__fields__"):
             schema[field.name] = _pydantic_to_simple_schema(field.outer_type_)
         else:
             type_name = field.outer_type_.__name__
             if type_name == "list":
-                type_name += f"[{field.type_.__name__}]"
-            schema[field.name] = type_name
+                (inner,) = typing.get_args(field.outer_type_)
+                schema[field.name] = [inner.__name__]
+            elif type_name == "dict":
+                k, v = typing.get_args(field.outer_type_)
+                schema[field.name] = {k.__name__: v.__name__}
+            else:
+                schema[field.name] = type_name
     return schema
 
 
-# class PaginatedSchemaScraper(SchemaScraper):
-#     def __init__(self, schema: list | str | dict, **kwargs: Any):
-#         schema = {
-#             "results": schema,
-#             "next_link": "url",
-#         }
-#         super().__init__(schema, **kwargs)
-#       self.system_messages.append("If there is no next page, set next_link to null.")
-
-#     def scrape(self, url: str, **kwargs: Any):
-#         results = []
-#         seen_urls = set()
-#         while url:
-#             logger.debug("page", url=url)
-#             page = super().scrape(url, **kwargs)
-#             logger.debug(
-#                 "results",
-#                 next_link=page["next_link"],
-#                 added_results=len(page["results"]),
-#             )
-#             results.extend(page["results"])
-#             seen_urls.add(url)
-#             url = page["next_link"]
-#             if url in seen_urls:
-#                 break
-#         return results
+class PaginatedSchemaScraper(SchemaScraper):
+    def __init__(self, schema: list | str | dict, **kwargs: Any):
+        # modify schema to include next_page_link
+        schema = {
+            "results": schema,
+            "next_page": "url",
+        }
+        super().__init__(schema, **kwargs)
+        self.system_messages.append("If there is no next page, set next_page to null.")
+
+    def scrape(
+        self, url: str, extra_preprocessors: list | None = None
+    ) -> ScrapeResponse:
+        sr = ScrapeResponse()
+        responses = []
+        seen_urls = set([url])
+        while url:
+            logger.debug("page", url=url)
+            resp = super().scrape(url, extra_preprocessors=extra_preprocessors)
+            # modify response to remove next_page wrapper
+            if isinstance(resp.data, dict):
+                url = resp.data["next_page"]
+                resp.data = resp.data["results"]
+            else:  # pragma: no cover
+                raise ValueError("PaginatedSchemaScraper requires object response")
+            responses.append(resp)
+            logger.debug(
+                "page results",
+                next_page=url,
+                added_results=len(resp.data),
+            )
+            if url in seen_urls:
+                break
+            if url:
+                seen_urls.add(url)
+
+        sr.url = "; ".join(sorted(seen_urls))
+        return _combine_responses(sr, responses)
```

### Comparing `scrapeghost-0.4.4/src/scrapeghost/utils.py` & `scrapeghost-0.5.0/src/scrapeghost/utils.py`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.4.4/PKG-INFO` & `scrapeghost-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeghost
-Version: 0.4.4
+Version: 0.5.0
 Summary: An experimental library for scraping websites using GPT.
 License: Hippocratic License HL3-EXTR-FFD-LAW-MIL-SV
 Author: James Turk
 Author-email: dev@jamesturk.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

