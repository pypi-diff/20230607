# Comparing `tmp/datahtml-0.4.0rc1.tar.gz` & `tmp/datahtml-0.4.0rc2.tar.gz`

## Comparing `datahtml-0.4.0rc1.tar` & `datahtml-0.4.0rc2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/.pylintrc
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/readthedocs.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/_utils.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/base.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/crawler.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/defaults.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/errors.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/google.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/google_trends.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/news.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/parsers.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/rss.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/sitemap.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/types.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/web.py
--rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/apis/__init__.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/datahtml/apis/youtube.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/Makefile
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api_reference.rst
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/conf.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/make.bat
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/crawler.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/sitemap.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/types.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/docs/api/web.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/__init__.py
--rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/google_search.html
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/google_trends_rss.xml
--rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/lanacion_article.html
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/robots.txt
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/root_carrefour_sitemap.xml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_apis_youtube.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_google.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_google_trends.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_root.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/test_youtube.py
--rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_channel.html
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_channel_rss.xml
--rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_search.html
--rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_search_response.json
--rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video.html
--rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video.json
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video_multiple_ids.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/tests/youtube_video_response.json
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/README.md
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 datahtml-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/.pylintrc
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/readthedocs.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/_utils.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/base.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/crawler.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/defaults.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/errors.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/google.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/google_trends.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/news.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/parsers.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/rss.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/sitemap.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/types.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/web.py
+-rw-r--r--   0        0        0    10774 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/apis/__init__.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/datahtml/apis/youtube.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/Makefile
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api_reference.rst
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/conf.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/make.bat
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/crawler.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/sitemap.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/types.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/docs/api/web.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0   264417 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/google_search.html
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/google_trends_rss.xml
+-rw-r--r--   0        0        0   284678 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/lanacion_article.html
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/robots.txt
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/root_carrefour_sitemap.xml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_apis_youtube.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_google.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_google_trends.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_root.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/test_youtube.py
+-rw-r--r--   0        0        0   333386 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_channel.html
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_channel_rss.xml
+-rw-r--r--   0        0        0   568777 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_search.html
+-rw-r--r--   0        0        0    29235 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_search_response.json
+-rw-r--r--   0        0        0   597066 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video.html
+-rw-r--r--   0        0        0   295956 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video.json
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video_multiple_ids.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/tests/youtube_video_response.json
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/LICENSE
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/README.md
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 datahtml-0.4.0rc2/PKG-INFO
```

### Comparing `datahtml-0.4.0rc1/.pylintrc` & `datahtml-0.4.0rc2/.pylintrc`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/base.py` & `datahtml-0.4.0rc2/datahtml/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def is_json(self):
         if "application/json" in self.headers["content-type"]:
             return True
         return False
 
     @property
     def is_xml(self):
-        if "text/xml" in self.headers["content-type"]:
+        if "xml" in self.headers["content-type"]:
             return True
         return False
 
     @property
     def is_txt(self):
         if "text/plain" in self.headers["content-type"]:
             return True
```

### Comparing `datahtml-0.4.0rc1/datahtml/crawler.py` & `datahtml-0.4.0rc2/datahtml/crawler.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/defaults.py` & `datahtml-0.4.0rc2/datahtml/defaults.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,13 +12,15 @@
     "tiktok.com",
     "youtube.com",
     "spotify.com",
     "wikipedia.org",
     "meetup.com",
     "linkedin.com",
     "books.google.com",
-    "bit.ly"
+    "bit.ly",
+    "apps.apple.com",
+    "play.google.com",
 ]
 
 WORDS_REGEX = re.compile(r'\b[A-Za-z]+\b')
-OG_KEYS = ["og:url", "og:image", "og:description", "og:type", "og:locale"]
+OG_KEYS = ["og:url", "og:image", "og:description", "og:type", "og:locale", "og:title"]
```

### Comparing `datahtml-0.4.0rc1/datahtml/errors.py` & `datahtml-0.4.0rc2/datahtml/errors.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/google.py` & `datahtml-0.4.0rc2/datahtml/google.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/google_trends.py` & `datahtml-0.4.0rc2/datahtml/google_trends.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/news.py` & `datahtml-0.4.0rc2/datahtml/news.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/parsers.py` & `datahtml-0.4.0rc2/datahtml/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         internal = True
 
     return types.Link(
         title=text.strip(), href=href.strip(), internal=internal, is_file=is_a_file
     )
 
 
-def _is_social(base_url, socials):
+def is_social(base_url, socials):
     # print(_u)
     for s in socials:
         if s in base_url:
             return True
     return False
 
 
@@ -110,16 +110,22 @@
     fullurl = f"{_u.scheme}://{_u.netloc}/{_path}"
     url_short = f"{_u.netloc}/{_path}"
     if trailing:
         fullurl = fullurl.strip("/")
         url_short = url_short.strip("/")
     return fullurl, url_short
 
+def get_domain_base(url: str) -> str:
+    url_regex = re.findall(URL_REGEX, url)
+    if not url_regex:
+        raise errors.URLParsingError(url)
+    domain = url_regex[0][1]
+    return str(domain)
 
-def parse_url(url: str) -> types.URL:
+def parse_url(url: str, socials_url=SOCIALS_COM) -> types.URL:
     """Parse a url string to URL.
     URL_REGEX return a tuple with 3 values:
     (protocol, netloc, path)
     """
     url_regex = re.findall(URL_REGEX, url)
 
     if not url_regex:
@@ -136,25 +142,25 @@
     www = False
     _www = domain.split("www.")
     if len(_www) > 1:
         www = True
         domain_base = _www[1]
         netloc = netloc.split("www.")[1]
 
-    is_social = _is_social(domain_base, SOCIALS_COM)
+    _is_social = is_social(domain_base, socials_url)
     is_secure = protocol == "https"
     tld = domain.split(".")[-1]
 
     return types.URL(
         fullurl=fullurl,
         url_short=url_short,
         domain_base=domain_base,
         netloc=_u.netloc,
         path=path,
-        is_social=is_social,
+        is_social=_is_social,
         secure=is_secure,
         www=www,
         tld=tld,
     )
 
 
 def extract_links(soup: BS, fullurl: str) -> List[types.Link]:
```

### Comparing `datahtml-0.4.0rc1/datahtml/rss.py` & `datahtml-0.4.0rc2/datahtml/rss.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/sitemap.py` & `datahtml-0.4.0rc2/datahtml/sitemap.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/types.py` & `datahtml-0.4.0rc2/datahtml/types.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/web.py` & `datahtml-0.4.0rc2/datahtml/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,23 @@
            Use :func:`datahtml.web.download`
 
         """
         rsp = crawler.get(url)
         obj = cls(url=url, html_txt=rsp.text, is_root=is_root)
         return obj
 
+    def social_urls(self) -> List[types.URL]:
+        _socials = []
+        for l in self.links():
+            if not l.internal:
+                _url = parsers.parse_url(l.href)
+                if _url.is_social:
+                    _socials.append(_url)
+        return _socials
+
     def links(self) -> List[types.Link]:
         links = parsers.extract_links(self.soup, fullurl=self.url.fullurl.strip("/"))
         return links
 
     def images(self) -> List[types.Image]:
         return parsers.extract_images(self.soup)
 
@@ -81,15 +90,15 @@
         return metas
 
     def get_locale(self) -> Union[str, None]:
         locale = None
         l = self.soup.html.get("lang")
         og_l = self.meta_og(keys=["og:locale"])
         if og_l:
-            locale =  og_l["locale"]
+            locale = og_l["locale"]
         elif l:
             locale = l
         return locale
 
     def __repr__(self):
         return f"<WebDocument '{self.url.fullurl}'>"
```

### Comparing `datahtml-0.4.0rc1/datahtml/youtube.py` & `datahtml-0.4.0rc2/datahtml/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/datahtml/apis/youtube.py` & `datahtml-0.4.0rc2/datahtml/apis/youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/docs/Makefile` & `datahtml-0.4.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/docs/conf.py` & `datahtml-0.4.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/docs/index.rst` & `datahtml-0.4.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/docs/make.bat` & `datahtml-0.4.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/google_search.html` & `datahtml-0.4.0rc2/tests/google_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/google_trends_rss.xml` & `datahtml-0.4.0rc2/tests/google_trends_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/lanacion_article.html` & `datahtml-0.4.0rc2/tests/lanacion_article.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/root_carrefour_sitemap.xml` & `datahtml-0.4.0rc2/tests/root_carrefour_sitemap.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/test_apis_youtube.py` & `datahtml-0.4.0rc2/tests/test_apis_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/test_youtube.py` & `datahtml-0.4.0rc2/tests/test_youtube.py`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_channel.html` & `datahtml-0.4.0rc2/tests/youtube_channel.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_channel_rss.xml` & `datahtml-0.4.0rc2/tests/youtube_channel_rss.xml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_search.html` & `datahtml-0.4.0rc2/tests/youtube_search.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_search_response.json` & `datahtml-0.4.0rc2/tests/youtube_search_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_video.html` & `datahtml-0.4.0rc2/tests/youtube_video.html`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_video.json` & `datahtml-0.4.0rc2/tests/youtube_video.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_video_multiple_ids.json` & `datahtml-0.4.0rc2/tests/youtube_video_multiple_ids.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/tests/youtube_video_response.json` & `datahtml-0.4.0rc2/tests/youtube_video_response.json`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/.gitignore` & `datahtml-0.4.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/LICENSE` & `datahtml-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/README.md` & `datahtml-0.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/pyproject.toml` & `datahtml-0.4.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datahtml-0.4.0rc1/PKG-INFO` & `datahtml-0.4.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahtml
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: A lib to work with html and web data
 Project-URL: Documentation, https://github.com/algorinfo/datahtml#readme
 Project-URL: Issues, https://github.com/algorinfo/datahtml/issues
 Project-URL: Source, https://github.com/algorinfo/datahtml
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

