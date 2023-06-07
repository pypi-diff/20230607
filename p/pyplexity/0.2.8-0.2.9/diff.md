# Comparing `tmp/pyplexity-0.2.8.tar.gz` & `tmp/pyplexity-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplexity-0.2.8.tar", max compression
+gzip compressed data, was "pyplexity-0.2.9.tar", max compression
```

## Comparing `pyplexity-0.2.8.tar` & `pyplexity-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     4043 2022-02-28 13:33:40.467881 pyplexity-0.2.8/README.md
--rw-r--r--   0        0        0      169 2022-03-01 18:15:30.010506 pyplexity-0.2.8/pyplexity/__init__.py
--rw-r--r--   0        0        0     2957 2022-03-01 18:15:46.802364 pyplexity-0.2.8/pyplexity/__main__.py
--rw-r--r--   0        0        0     5382 2021-10-07 10:32:00.574000 pyplexity-0.2.8/pyplexity/dataset_processor/CustomWARCWriter.py
--rw-r--r--   0        0        0     4889 2021-12-30 23:29:18.502104 pyplexity-0.2.8/pyplexity/dataset_processor/__pycache__/CustomWARCWriter.cpython-38.pyc
--rw-r--r--   0        0        0     3648 2021-12-30 23:29:18.466104 pyplexity-0.2.8/pyplexity/dataset_processor/__pycache__/dataset_processor.cpython-38.pyc
--rw-r--r--   0        0        0     4153 2021-12-30 23:29:16.000000 pyplexity-0.2.8/pyplexity/dataset_processor/dataset_processor.py
--rw-r--r--   0        0        0     1240 2022-01-03 12:08:36.431397 pyplexity-0.2.8/pyplexity/distributed_files_server.py
--rw-r--r--   0        0        0     5071 2022-03-01 18:18:38.832930 pyplexity-0.2.8/pyplexity/perpl_model.py
--rw-r--r--   0        0        0     2023 2021-12-30 23:30:20.000000 pyplexity-0.2.8/pyplexity/tag_remover.py
--rw-r--r--   0        0        0      836 2022-03-14 15:31:40.692026 pyplexity-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5257 2022-03-14 15:31:42.578781 pyplexity-0.2.8/setup.py
--rw-r--r--   0        0        0     5130 2022-03-14 15:31:42.579392 pyplexity-0.2.8/PKG-INFO
+-rwxr-xr-x   0        0        0    35147 2022-03-01 17:16:17.000000 pyplexity-0.2.9/LICENSE
+-rwxr-xr-x   0        0        0     8425 2022-03-14 16:42:30.000000 pyplexity-0.2.9/README.md
+-rwxr-xr-x   0        0        0      859 2022-03-14 16:42:30.000000 pyplexity-0.2.9/pyplexity/__init__.py
+-rwxr-xr-x   0        0        0     3745 2022-03-14 16:42:30.000000 pyplexity-0.2.9/pyplexity/__main__.py
+-rwxr-xr-x   0        0        0     6072 2022-03-01 17:16:17.000000 pyplexity-0.2.9/pyplexity/dataset_processor/CustomWARCWriter.py
+-rwxr-xr-x   0        0        0     4846 2022-03-14 16:42:30.000000 pyplexity-0.2.9/pyplexity/dataset_processor/dataset_processor.py
+-rwxr-xr-x   0        0        0     1930 2022-03-01 17:16:17.000000 pyplexity-0.2.9/pyplexity/distributed_files_server.py
+-rwxr-xr-x   0        0        0     5761 2022-03-14 15:46:20.000000 pyplexity-0.2.9/pyplexity/perpl_model.py
+-rwxr-xr-x   0        0        0     1821 2023-02-06 21:09:09.032959 pyplexity-0.2.9/pyplexity/tag_remover.py
+-rwxr-xr-x   0        0        0      836 2023-02-07 12:37:57.442787 pyplexity-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9719 1970-01-01 00:00:00.000000 pyplexity-0.2.9/setup.py
+-rw-r--r--   0        0        0     9563 1970-01-01 00:00:00.000000 pyplexity-0.2.9/PKG-INFO
```

### Comparing `pyplexity-0.2.8/pyplexity/dataset_processor/CustomWARCWriter.py` & `pyplexity-0.2.9/pyplexity/dataset_processor/CustomWARCWriter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# PyPlexity
+# Copyright (C) 2022 Manuel Prada Corral
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import zlib
 
 from socket import gethostname
 
 from warcio.recordbuilder import RecordBuilder
 
 from warcio.statusandheaders import StatusAndHeadersParser
```

### Comparing `pyplexity-0.2.8/pyplexity/perpl_model.py` & `pyplexity-0.2.9/pyplexity/perpl_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# PyPlexity
+# Copyright (C) 2022 Manuel Prada Corral
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import math
 import re
 import signal
 from typing import Union
 
 import nltk
 import pandas
```

### Comparing `pyplexity-0.2.8/pyplexity/tag_remover.py` & `pyplexity-0.2.9/pyplexity/tag_remover.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
+# PyPlexity
+# Copyright (C) 2022 Manuel Prada Corral
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import lxml
 from lxml import etree
 from lxml.html import HtmlElement, html5parser
 
 from pyplexity.dataset_processor.dataset_processor import ContentProcessor
 
 
 class HTMLTagRemover(ContentProcessor):
 
     def process(self, content: bytes) -> str:
         return self._remove_html_tags_lxml(content)
 
     def __init__(self):
         self.build_text_list = etree.XPath("//text()")
-        # logging.getLogger("bs4").setLevel(logging.CRITICAL)
-        # logging.getLogger("bs4.dammit").setLevel(logging.CRITICAL)
-        # warnings.simplefilter("ignore")  # disable htmlsoup warnings
 
     def _remove_html_tags_lxml(self, content):
-        content = content.decode(errors="ignore").encode("ascii", errors="ignore")
+        if isinstance(content, (bytes, bytearray)):
+            content = decode(errors="ignore")
+        content = content.encode("ascii", errors="ignore")
         try:
             html: HtmlElement = lxml.html.document_fromstring(content)
         except etree.ParserError:
             return ""
         except:  # if lxml (faster parser) doesnt work, try with html5lib (slower but more stable)
             print("html5lib")
             html = html5parser.fromstring(content)
         texts = self.build_text_list(html)  # recorrido eficiente de textos con eliminacion posterior: 6.05s
         res = " ".join([s.strip() for s in texts if s.getparent().tag not in ["script", "style"]])
         return res
-        # recorrido eficiente con eliminacion eficiente: 6.21s
-        # for bad in html.xpath("//style|//script"):
-        #    bad.getparent().remove(bad)
-        # return etree.tostring(html, method="text", encoding="utf8")
-
-    # def _remove_html_tags_bs4(self, content):
-    #     try:
-    #         soup = BeautifulSoup(content, "lxml")  # parse HTML
-    #     except:  # if lxml (faster parser) doesnt work, try with html5lib (slower but more stable)
-    #         print("html5lib")
-    #         soup = BeautifulSoup(content, "html5lib")
-    #     for script in soup(["script", "style"]):  # tag removal from parsed HTML tree
-    #         script.decompose()
-    #     return soup.get_text(separator=" ", strip=True)  # extract text from rest of HTML tags
```

### Comparing `pyplexity-0.2.8/pyproject.toml` & `pyplexity-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyplexity"
-version = "0.2.8"
+version = "0.2.9"
 description = "Perplexity filter for documents and bulk HTML and WARC boilerplate removal."
 authors = ["Manuel de Prada Corral <manuel.deprada.corral@usc.es>", "Marcos Fernández Pichel <marcosfernandez.pichel@usc.es>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/citiususc/pyplexity"
```

