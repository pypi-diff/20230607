# Comparing `tmp/datahtml-0.4.0rc0.tar.gz` & `tmp/datahtml-0.4.0rc1.tar.gz`

## Comparing `datahtml-0.4.0rc0.tar` & `datahtml-0.4.0rc1.tar`

### file list

```diff
@@ -1,52 +1,55 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/.pylintrc
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/_utils.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/base.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/crawler.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/defaults.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/errors.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/google.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/news.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/parsers.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/rss.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/sitemap.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/types.py
--rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/web.py
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/apis/__init__.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/datahtml/apis/youtube.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/Makefile
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api_reference.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/conf.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/make.bat
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/crawler.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/sitemap.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/types.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/docs/api/web.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/__init__.py
--rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/google_search.html
--rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/lanacion_article.html
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/robots.txt
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/root_carrefour_sitemap.xml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_apis_youtube.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_google.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_root.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/test_youtube.py
--rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_channel.html
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_channel_rss.xml
--rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_search.html
--rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_search_response.json
--rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video.html
--rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video.json
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video_multiple_ids.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/tests/youtube_video_response.json
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/README.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/pyproject.toml
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 datahtml-0.4.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/.pylintrc
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/_utils.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/base.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/crawler.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/defaults.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/errors.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/google.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/google_trends.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/news.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/parsers.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/rss.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/sitemap.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/types.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/web.py
+-rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/apis/__init__.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/apis/youtube.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api_reference.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/conf.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/make.bat
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/crawler.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/sitemap.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/types.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/web.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/google_search.html
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/google_trends_rss.xml
+-rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/lanacion_article.html
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/robots.txt
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/root_carrefour_sitemap.xml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_apis_youtube.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_google.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_google_trends.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_root.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_youtube.py
+-rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_channel.html
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_channel_rss.xml
+-rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_search.html
+-rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_search_response.json
+-rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video.html
+-rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video.json
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video_multiple_ids.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video_response.json
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/PKG-INFO
```

### Comparing `datahtml-0.4.0rc0/.pylintrc` & `datahtml-0.4.0rc1/.pylintrc`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/base.py` & `datahtml-0.4.0rc1/datahtml/base.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/crawler.py` & `datahtml-0.4.0rc1/datahtml/crawler.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/errors.py` & `datahtml-0.4.0rc1/datahtml/errors.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/google.py` & `datahtml-0.4.0rc1/datahtml/google.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/news.py` & `datahtml-0.4.0rc1/datahtml/news.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/parsers.py` & `datahtml-0.4.0rc1/datahtml/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,7 +204,17 @@
                 yield x
     elif isinstance(node, dict):
         if kv in node:
             yield node[kv]
         for j in node.values():
             for x in findkeys(j, kv):
                 yield x
+
+def meta_keywords(soup: BS) -> str:
+    data = extract_metadata(soup)
+    keywords = ""
+    for d in data:
+        if d.get("property"):
+            if d["property"] == "keywords":
+                keywords = d["content"]
+                break
+    return keywords
```

### Comparing `datahtml-0.4.0rc0/datahtml/rss.py` & `datahtml-0.4.0rc1/datahtml/rss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Dict, Any
 
 import feedparser
 from dateutil.parser import parse as dtparser
 
 from datahtml import errors, types
 from datahtml.base import CrawlerSpec
+
 # from datahtml.web import Web
 
 
 @dataclass
 class Entry:
     link: str
     title: Optional[str] = None
@@ -55,13 +56,18 @@
             entries.append(_entry)
         except KeyError:
             pass
 
     return entries
 
 
+def parse_as_dict(xmlcontent: str) -> List[Dict[str, Any]]:
+    feed = feedparser.parse(xmlcontent)
+    return feed["entries"]
+
+
 def find_rss_realated_links(links: List[types.Link]):
     rss_links = set()
     for link in links:
         if link.internal and "rss" in link.href or "feed" in link.href:
             rss_links.add(link.href)
     return rss_links
```

### Comparing `datahtml-0.4.0rc0/datahtml/sitemap.py` & `datahtml-0.4.0rc1/datahtml/sitemap.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/types.py` & `datahtml-0.4.0rc1/datahtml/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 
 
 @dataclass
 class Image:
     alt: str
     src: str
 
+@dataclass
+class MetaTag:
+    key: str
+    value: str
+
```

### Comparing `datahtml-0.4.0rc0/datahtml/web.py` & `datahtml-0.4.0rc1/datahtml/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Union
 
-from datahtml import errors, news, parsers, rss, sitemap, types
+from datahtml import defaults, errors, news, parsers, rss, sitemap, types
 from datahtml._utils import difference_from_now
 from datahtml.base import CrawlerSpec
 
 
 class WebDocument:
     """
     It's the main object for the library. It represents a HTML Document.
     This page could be a root link or a subpage.
     """
+
     def __init__(self, url: str, *, html_txt: str, is_root=False):
         """
         :param url: url where the document belongs.
         :type url: str
         :param html_txt: html text of the document.
         :type html_txt: str
         :param is_root: if is the root site or a subpage.
@@ -49,23 +50,50 @@
 
     def images(self) -> List[types.Image]:
         return parsers.extract_images(self.soup)
 
     def ld_json(self) -> Dict[str, Any]:
         return parsers.extract_ld_json(self.soup)
 
-    def meta_og(
-        self, keys=["og:url", "og:image", "og:description", "og:type"]
-    ) -> Dict[str, str]:
+    def meta_og(self, keys=defaults.OG_KEYS) -> Dict[str, str]:
         return parsers.extract_meta_og(self.soup, meta=keys)
 
     def article(self) -> news.ArticleData:
         ad = news.ArticleData.from_html(url=self.url.fullurl, html=self._html)
         return ad
 
+    def keywords(self) -> Union[str, None]:
+        k = None
+        for m in self.soup.find_all("meta"):
+            p = m.get("property")
+            if p and p == "keywords":
+                k = m.get("content")
+        return k
+
+    def metas(self) -> List[types.MetaTag]:
+        metas = []
+        for m in self.soup.find_all("meta"):
+            if m.get("content") and m.get("property"):
+                _mt = types.MetaTag(key=m.get("property"), value=m.get("content"))
+                metas.append(_mt)
+            elif m.get("content") and m.get("name"):
+                _mt = types.MetaTag(key=m.get("name"), value=m.get("content"))
+                metas.append(_mt)
+        return metas
+
+    def get_locale(self) -> Union[str, None]:
+        locale = None
+        l = self.soup.html.get("lang")
+        og_l = self.meta_og(keys=["og:locale"])
+        if og_l:
+            locale =  og_l["locale"]
+        elif l:
+            locale = l
+        return locale
+
     def __repr__(self):
         return f"<WebDocument '{self.url.fullurl}'>"
 
     def __str__(self):
         return f"<WebDocument '{self.url.fullurl}'>"
```

### Comparing `datahtml-0.4.0rc0/datahtml/youtube.py` & `datahtml-0.4.0rc1/datahtml/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/datahtml/apis/youtube.py` & `datahtml-0.4.0rc1/datahtml/apis/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/docs/Makefile` & `datahtml-0.4.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/docs/conf.py` & `datahtml-0.4.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/docs/index.rst` & `datahtml-0.4.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/docs/make.bat` & `datahtml-0.4.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/google_search.html` & `datahtml-0.4.0rc1/tests/google_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/lanacion_article.html` & `datahtml-0.4.0rc1/tests/lanacion_article.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/root_carrefour_sitemap.xml` & `datahtml-0.4.0rc1/tests/root_carrefour_sitemap.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/test_apis_youtube.py` & `datahtml-0.4.0rc1/tests/test_apis_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/test_youtube.py` & `datahtml-0.4.0rc1/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_channel.html` & `datahtml-0.4.0rc1/tests/youtube_channel.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_channel_rss.xml` & `datahtml-0.4.0rc1/tests/youtube_channel_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_search.html` & `datahtml-0.4.0rc1/tests/youtube_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_search_response.json` & `datahtml-0.4.0rc1/tests/youtube_search_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_video.html` & `datahtml-0.4.0rc1/tests/youtube_video.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_video.json` & `datahtml-0.4.0rc1/tests/youtube_video.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_video_multiple_ids.json` & `datahtml-0.4.0rc1/tests/youtube_video_multiple_ids.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/tests/youtube_video_response.json` & `datahtml-0.4.0rc1/tests/youtube_video_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/.gitignore` & `datahtml-0.4.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/LICENSE` & `datahtml-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/README.md` & `datahtml-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc0/pyproject.toml` & `datahtml-0.4.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	"lxml~=4.6.3",
 	"ujson~=4.2.0",
 	"extruct~=0.13.0",
 	"feedparser~=6.0.8",
 	# "reppy~=0.4.14",
 	"newspaper3k~=0.2.8",
 	"httpx~=0.23.0",
-        "pydantic~=1.10.7"
+    "pydantic~=1.10.7"
         
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/algorinfo/datahtml#readme"
 Issues = "https://github.com/algorinfo/datahtml/issues"
```

### Comparing `datahtml-0.4.0rc0/PKG-INFO` & `datahtml-0.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: datahtml
-Version: 0.4.0rc0
+Version: 0.4.0rc1
 Summary: A lib to work with html and web data
 Project-URL: Documentation, https://github.com/algorinfo/datahtml#readme
 Project-URL: Issues, https://github.com/algorinfo/datahtml/issues
 Project-URL: Source, https://github.com/algorinfo/datahtml
 Author-email: Xavier Petit <nuxion@gmail.com>
-License-Expression: MPL-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

