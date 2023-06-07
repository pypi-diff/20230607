# Comparing `tmp/sphinxcontrib-katex-0.9.4.tar.gz` & `tmp/sphinxcontrib-katex-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-katex-0.9.4.tar", last modified: Wed Jan  4 08:03:39 2023, max compression
+gzip compressed data, was "sphinxcontrib-katex-0.9.5.tar", last modified: Wed Jun  7 10:14:25 2023, max compression
```

## Comparing `sphinxcontrib-katex-0.9.4.tar` & `sphinxcontrib-katex-0.9.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 08:03:39.334425 sphinxcontrib-katex-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-01-04 08:03:39.334425 sphinxcontrib-katex-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 08:03:39.334425 sphinxcontrib-katex-0.9.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/macros.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-04 08:03:39.334425 sphinxcontrib-katex-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 08:03:39.334425 sphinxcontrib-katex-0.9.4/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib/auto-render.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib/katex-math.css
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib/katex-server.js
--rw-r--r--   0 runner    (1001) docker     (123)   276729 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib/katex.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-01-04 08:03:30.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib/katex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 08:03:39.334425 sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-01-04 08:03:39.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-04 08:03:39.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 08:03:39.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-04 08:03:39.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-04 08:03:39.000000 sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/macros.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/auto-render.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-math.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-server.js
+-rw-r--r--   0 runner    (1001) docker     (123)   276757 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-katex-0.9.4/CHANGELOG.rst` & `sphinxcontrib-katex-0.9.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.5 (2023-06-07)
+--------------------------
+
+* Changed: use KaTeX 0.16.7
+* Fixed: convert ``KaTeXServer.timeout_error()``
+  to class method
+
+
 Version 0.9.4 (2023-01-04)
 --------------------------
 
 * Changed: use KaTeX 0.16.4
 
 
 Version 0.9.3 (2022-11-25)
```

### Comparing `sphinxcontrib-katex-0.9.4/CONTRIBUTING.rst` & `sphinxcontrib-katex-0.9.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/LICENSE` & `sphinxcontrib-katex-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/PKG-INFO` & `sphinxcontrib-katex-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Sphinx extension for rendering math in HTML pages
 Home-page: https://github.com/hagenw/sphinxcontrib-katex
 Author: Hagen Wierstorf
 Author-email: hagenw@posteo.de
 License: MIT
 Keywords: sphinx,latex,katex,math,documentation
 Platform: any
@@ -105,15 +105,15 @@
 The behavior of ``sphinxcontrib.katex`` can be changed by configuration
 entries in ``conf.py`` of your documentation project. In the following
 all configuration entries are listed and their default values are shown.
 
 .. code-block:: python
 
     katex_css_path = \
-        'https://cdn.jsdelivr.net/npm/katex@0.16.4/dist/katex.min.css'
+        'https://cdn.jsdelivr.net/npm/katex@0.16.7/dist/katex.min.css'
     katex_js_path = 'katex.min.js'
     katex_autorender_path = 'auto-render.min.js'
     katex_inline = [r'\(', r'\)']
     katex_display = [r'\[', r'\]']
     katex_prerender = False
     katex_options = ''
 
@@ -201,14 +201,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.5 (2023-06-07)
+--------------------------
+
+* Changed: use KaTeX 0.16.7
+* Fixed: convert ``KaTeXServer.timeout_error()``
+  to class method
+
+
 Version 0.9.4 (2023-01-04)
 --------------------------
 
 * Changed: use KaTeX 0.16.4
 
 
 Version 0.9.3 (2022-11-25)
```

### Comparing `sphinxcontrib-katex-0.9.4/README.rst` & `sphinxcontrib-katex-0.9.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 The behavior of ``sphinxcontrib.katex`` can be changed by configuration
 entries in ``conf.py`` of your documentation project. In the following
 all configuration entries are listed and their default values are shown.
 
 .. code-block:: python
 
     katex_css_path = \
-        'https://cdn.jsdelivr.net/npm/katex@0.16.4/dist/katex.min.css'
+        'https://cdn.jsdelivr.net/npm/katex@0.16.7/dist/katex.min.css'
     katex_js_path = 'katex.min.js'
     katex_autorender_path = 'auto-render.min.js'
     katex_inline = [r'\(', r'\)']
     katex_display = [r'\[', r'\]']
     katex_prerender = False
     katex_options = ''
```

### Comparing `sphinxcontrib-katex-0.9.4/docs/conf.py` & `sphinxcontrib-katex-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/docs/definitions.py` & `sphinxcontrib-katex-0.9.5/docs/definitions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/docs/examples.rst` & `sphinxcontrib-katex-0.9.5/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/docs/index.rst` & `sphinxcontrib-katex-0.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/setup.cfg` & `sphinxcontrib-katex-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib/auto-render.min.js` & `sphinxcontrib-katex-0.9.5/sphinxcontrib/auto-render.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib/katex-math.css` & `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-math.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib/katex-server.js` & `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-server.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib/katex.min.js` & `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
                 o: function(e, t) {
                     return Object.prototype.hasOwnProperty.call(e, t)
                 }
             },
             t = {};
         e.d(t, {
             default: function() {
-                return Qn
+                return na
             }
         });
         var r = function e(t, r) {
             this.position = void 0;
             var n, a = "KaTeX parse error: " + t,
                 i = r && r.loc;
             if (i && i.start <= i.end) {
@@ -8114,18 +8114,22 @@
                 return n.setAttribute("mathvariant", "monospace"), n
             }
         });
         var Nn = function(e) {
                 return e.body.replace(/ /g, e.star ? "\u2423" : "\xa0")
             },
             qn = nt,
-            In = new RegExp("[\u0300-\u036f]+$"),
-            Rn = function() {
+            In = "[ \r\n\t]",
+            Rn = "(\\\\[a-zA-Z@]+)" + In + "*",
+            Hn = "[\u0300-\u036f]",
+            On = new RegExp(Hn + "+$"),
+            En = "(" + In + "+)|\\\\(\n|[ \r\t]+\n?)[ \r\t]*|([!-\\[\\]-\u2027\u202a-\ud7ff\uf900-\uffff]" + Hn + "*|[\ud800-\udbff][\udc00-\udfff]" + Hn + "*|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5|" + Rn + "|\\\\[^\ud800-\udfff])",
+            Ln = function() {
                 function e(e, t) {
-                    this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = e, this.settings = t, this.tokenRegex = new RegExp("([ \r\n\t]+)|\\\\(\n|[ \r\t]+\n?)[ \r\t]*|([!-\\[\\]-\u2027\u202a-\ud7ff\uf900-\uffff][\u0300-\u036f]*|[\ud800-\udbff][\udc00-\udfff][\u0300-\u036f]*|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5|(\\\\[a-zA-Z@]+)[ \r\n\t]*|\\\\[^\ud800-\udfff])", "g"), this.catcodes = {
+                    this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = e, this.settings = t, this.tokenRegex = new RegExp(En, "g"), this.catcodes = {
                         "%": 14,
                         "~": 13
                     }
                 }
                 var t = e.prototype;
                 return t.setCatcode = function(e, t) {
                     this.catcodes[e] = t
@@ -8139,15 +8143,15 @@
                     if (14 === this.catcodes[a]) {
                         var i = e.indexOf("\n", this.tokenRegex.lastIndex);
                         return -1 === i ? (this.tokenRegex.lastIndex = e.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = i + 1, this.lex()
                     }
                     return new Gr(a, new Fr(this, t, this.tokenRegex.lastIndex))
                 }, e
             }(),
-            Hn = function() {
+            Dn = function() {
                 function e(e, t) {
                     void 0 === e && (e = {}), void 0 === t && (t = {}), this.current = void 0, this.builtins = void 0, this.undefStack = void 0, this.current = t, this.builtins = e, this.undefStack = []
                 }
                 var t = e.prototype;
                 return t.beginGroup = function() {
                     this.undefStack.push({})
                 }, t.endGroup = function() {
@@ -8167,15 +8171,15 @@
                     } else {
                         var a = this.undefStack[this.undefStack.length - 1];
                         a && !a.hasOwnProperty(e) && (a[e] = this.current[e])
                     }
                     null == t ? delete this.current[e] : this.current[e] = t
                 }, e
             }(),
-            On = Vr;
+            Vn = Vr;
         Pr("\\noexpand", (function(e) {
             var t = e.popToken();
             return e.isExpandable(t.text) && (t.noexpand = !0, t.treatAsRelax = !0), {
                 tokens: [t],
                 numArgs: 0
             }
         })), Pr("\\expandafter", (function(e) {
@@ -8211,15 +8215,15 @@
                 tokens: t[0],
                 numArgs: 0
             } : {
                 tokens: t[1],
                 numArgs: 0
             }
         }));
-        var En = {
+        var Pn = {
             0: 0,
             1: 1,
             2: 2,
             3: 3,
             4: 4,
             5: 5,
             6: 6,
@@ -8248,20 +8252,20 @@
                 if ("\\" === (r = e.popToken()).text[0]) a = r.text.charCodeAt(1);
                 else {
                     if ("EOF" === r.text) throw new n("\\char` missing argument");
                     a = r.text.charCodeAt(0)
                 }
             else t = 10;
             if (t) {
-                if (null == (a = En[r.text]) || a >= t) throw new n("Invalid base-" + t + " digit " + r.text);
-                for (var i; null != (i = En[e.future().text]) && i < t;) a *= t, a += i, e.popToken()
+                if (null == (a = Pn[r.text]) || a >= t) throw new n("Invalid base-" + t + " digit " + r.text);
+                for (var i; null != (i = Pn[e.future().text]) && i < t;) a *= t, a += i, e.popToken()
             }
             return "\\@char{" + a + "}"
         }));
-        var Ln = function(e, t, r) {
+        var Fn = function(e, t, r) {
             var a = e.consumeArg().tokens;
             if (1 !== a.length) throw new n("\\newcommand's first argument must be a macro name");
             var i = a[0].text,
                 o = e.isDefined(i);
             if (o && !t) throw new n("\\newcommand{" + i + "} attempting to redefine " + i + "; use \\renewcommand");
             if (!o && !r) throw new n("\\renewcommand{" + i + "} when command " + i + " does not yet exist; use \\newcommand");
             var s = 0;
@@ -8273,19 +8277,19 @@
             }
             return e.macros.set(i, {
                 tokens: a,
                 numArgs: s
             }), ""
         };
         Pr("\\newcommand", (function(e) {
-            return Ln(e, !1, !0)
+            return Fn(e, !1, !0)
         })), Pr("\\renewcommand", (function(e) {
-            return Ln(e, !0, !1)
+            return Fn(e, !0, !1)
         })), Pr("\\providecommand", (function(e) {
-            return Ln(e, !0, !0)
+            return Fn(e, !0, !0)
         })), Pr("\\message", (function(e) {
             var t = e.consumeArgs(1)[0];
             return console.log(t.reverse().map((function(e) {
                 return e.text
             })).join("")), ""
         })), Pr("\\errmessage", (function(e) {
             var t = e.consumeArgs(1)[0];
@@ -8293,15 +8297,15 @@
                 return e.text
             })).join("")), ""
         })), Pr("\\show", (function(e) {
             var t = e.popToken(),
                 r = t.text;
             return console.log(t, e.macros.get(r), qn[r], ae.math[r], ae.text[r]), ""
         })), Pr("\\bgroup", "{"), Pr("\\egroup", "}"), Pr("~", "\\nobreakspace"), Pr("\\lq", "`"), Pr("\\rq", "'"), Pr("\\aa", "\\r a"), Pr("\\AA", "\\r A"), Pr("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`\xa9}"), Pr("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), Pr("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`\xae}"), Pr("\u212c", "\\mathscr{B}"), Pr("\u2130", "\\mathscr{E}"), Pr("\u2131", "\\mathscr{F}"), Pr("\u210b", "\\mathscr{H}"), Pr("\u2110", "\\mathscr{I}"), Pr("\u2112", "\\mathscr{L}"), Pr("\u2133", "\\mathscr{M}"), Pr("\u211b", "\\mathscr{R}"), Pr("\u212d", "\\mathfrak{C}"), Pr("\u210c", "\\mathfrak{H}"), Pr("\u2128", "\\mathfrak{Z}"), Pr("\\Bbbk", "\\Bbb{k}"), Pr("\xb7", "\\cdotp"), Pr("\\llap", "\\mathllap{\\textrm{#1}}"), Pr("\\rlap", "\\mathrlap{\\textrm{#1}}"), Pr("\\clap", "\\mathclap{\\textrm{#1}}"), Pr("\\mathstrut", "\\vphantom{(}"), Pr("\\underbar", "\\underline{\\text{#1}}"), Pr("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), Pr("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`\u2260}}"), Pr("\\ne", "\\neq"), Pr("\u2260", "\\neq"), Pr("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`\u2209}}"), Pr("\u2209", "\\notin"), Pr("\u2258", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`\u2258}}"), Pr("\u2259", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`\u2258}}"), Pr("\u225a", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`\u225a}}"), Pr("\u225b", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`\u225b}}"), Pr("\u225d", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`\u225d}}"), Pr("\u225e", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`\u225e}}"), Pr("\u225f", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`\u225f}}"), Pr("\u27c2", "\\perp"), Pr("\u203c", "\\mathclose{!\\mkern-0.8mu!}"), Pr("\u220c", "\\notni"), Pr("\u231c", "\\ulcorner"), Pr("\u231d", "\\urcorner"), Pr("\u231e", "\\llcorner"), Pr("\u231f", "\\lrcorner"), Pr("\xa9", "\\copyright"), Pr("\xae", "\\textregistered"), Pr("\ufe0f", "\\textregistered"), Pr("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), Pr("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), Pr("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), Pr("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), Pr("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), Pr("\u22ee", "\\vdots"), Pr("\\varGamma", "\\mathit{\\Gamma}"), Pr("\\varDelta", "\\mathit{\\Delta}"), Pr("\\varTheta", "\\mathit{\\Theta}"), Pr("\\varLambda", "\\mathit{\\Lambda}"), Pr("\\varXi", "\\mathit{\\Xi}"), Pr("\\varPi", "\\mathit{\\Pi}"), Pr("\\varSigma", "\\mathit{\\Sigma}"), Pr("\\varUpsilon", "\\mathit{\\Upsilon}"), Pr("\\varPhi", "\\mathit{\\Phi}"), Pr("\\varPsi", "\\mathit{\\Psi}"), Pr("\\varOmega", "\\mathit{\\Omega}"), Pr("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), Pr("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), Pr("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), Pr("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), Pr("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), Pr("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
-        var Dn = {
+        var Gn = {
             ",": "\\dotsc",
             "\\not": "\\dotsb",
             "+": "\\dotsb",
             "=": "\\dotsb",
             "<": "\\dotsb",
             ">": "\\dotsb",
             "-": "\\dotsb",
@@ -8345,17 +8349,17 @@
             "\\iiiint": "\\dotsi",
             "\\idotsint": "\\dotsi",
             "\\DOTSX": "\\dotsx"
         };
         Pr("\\dots", (function(e) {
             var t = "\\dotso",
                 r = e.expandAfterFuture().text;
-            return r in Dn ? t = Dn[r] : ("\\not" === r.slice(0, 4) || r in ae.math && l.contains(["bin", "rel"], ae.math[r].group)) && (t = "\\dotsb"), t
+            return r in Gn ? t = Gn[r] : ("\\not" === r.slice(0, 4) || r in ae.math && l.contains(["bin", "rel"], ae.math[r].group)) && (t = "\\dotsb"), t
         }));
-        var Vn = {
+        var Un = {
             ")": !0,
             "]": !0,
             "\\rbrack": !0,
             "\\}": !0,
             "\\rbrace": !0,
             "\\rangle": !0,
             "\\rceil": !0,
@@ -8369,27 +8373,27 @@
             "\\Biggr": !0,
             $: !0,
             ";": !0,
             ".": !0,
             ",": !0
         };
         Pr("\\dotso", (function(e) {
-            return e.future().text in Vn ? "\\ldots\\," : "\\ldots"
+            return e.future().text in Un ? "\\ldots\\," : "\\ldots"
         })), Pr("\\dotsc", (function(e) {
             var t = e.future().text;
-            return t in Vn && "," !== t ? "\\ldots\\," : "\\ldots"
+            return t in Un && "," !== t ? "\\ldots\\," : "\\ldots"
         })), Pr("\\cdots", (function(e) {
-            return e.future().text in Vn ? "\\@cdots\\," : "\\@cdots"
+            return e.future().text in Un ? "\\@cdots\\," : "\\@cdots"
         })), Pr("\\dotsb", "\\cdots"), Pr("\\dotsm", "\\cdots"), Pr("\\dotsi", "\\!\\cdots"), Pr("\\dotsx", "\\ldots\\,"), Pr("\\DOTSI", "\\relax"), Pr("\\DOTSB", "\\relax"), Pr("\\DOTSX", "\\relax"), Pr("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), Pr("\\,", "\\tmspace+{3mu}{.1667em}"), Pr("\\thinspace", "\\,"), Pr("\\>", "\\mskip{4mu}"), Pr("\\:", "\\tmspace+{4mu}{.2222em}"), Pr("\\medspace", "\\:"), Pr("\\;", "\\tmspace+{5mu}{.2777em}"), Pr("\\thickspace", "\\;"), Pr("\\!", "\\tmspace-{3mu}{.1667em}"), Pr("\\negthinspace", "\\!"), Pr("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), Pr("\\negthickspace", "\\tmspace-{5mu}{.277em}"), Pr("\\enspace", "\\kern.5em "), Pr("\\enskip", "\\hskip.5em\\relax"), Pr("\\quad", "\\hskip1em\\relax"), Pr("\\qquad", "\\hskip2em\\relax"), Pr("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), Pr("\\tag@paren", "\\tag@literal{({#1})}"), Pr("\\tag@literal", (function(e) {
             if (e.macros.get("\\df@tag")) throw new n("Multiple \\tag");
             return "\\gdef\\df@tag{\\text{#1}}"
         })), Pr("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), Pr("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), Pr("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), Pr("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), Pr("\\newline", "\\\\\\relax"), Pr("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
-        var Pn = F(T["Main-Regular"]["T".charCodeAt(0)][1] - .7 * T["Main-Regular"]["A".charCodeAt(0)][1]);
-        Pr("\\LaTeX", "\\textrm{\\html@mathml{L\\kern-.36em\\raisebox{" + Pn + "}{\\scriptstyle A}\\kern-.15em\\TeX}{LaTeX}}"), Pr("\\KaTeX", "\\textrm{\\html@mathml{K\\kern-.17em\\raisebox{" + Pn + "}{\\scriptstyle A}\\kern-.15em\\TeX}{KaTeX}}"), Pr("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), Pr("\\@hspace", "\\hskip #1\\relax"), Pr("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), Pr("\\ordinarycolon", ":"), Pr("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), Pr("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), Pr("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), Pr("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), Pr("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), Pr("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), Pr("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), Pr("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), Pr("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), Pr("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), Pr("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), Pr("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), Pr("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), Pr("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), Pr("\u2237", "\\dblcolon"), Pr("\u2239", "\\eqcolon"), Pr("\u2254", "\\coloneqq"), Pr("\u2255", "\\eqqcolon"), Pr("\u2a74", "\\Coloneqq"), Pr("\\ratio", "\\vcentcolon"), Pr("\\coloncolon", "\\dblcolon"), Pr("\\colonequals", "\\coloneqq"), Pr("\\coloncolonequals", "\\Coloneqq"), Pr("\\equalscolon", "\\eqqcolon"), Pr("\\equalscoloncolon", "\\Eqqcolon"), Pr("\\colonminus", "\\coloneq"), Pr("\\coloncolonminus", "\\Coloneq"), Pr("\\minuscolon", "\\eqcolon"), Pr("\\minuscoloncolon", "\\Eqcolon"), Pr("\\coloncolonapprox", "\\Colonapprox"), Pr("\\coloncolonsim", "\\Colonsim"), Pr("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Pr("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Pr("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Pr("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Pr("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`\u220c}}"), Pr("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), Pr("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), Pr("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), Pr("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), Pr("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), Pr("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), Pr("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), Pr("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), Pr("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{\u2269}"), Pr("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{\u2268}"), Pr("\\ngeqq", "\\html@mathml{\\@ngeqq}{\u2271}"), Pr("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{\u2271}"), Pr("\\nleqq", "\\html@mathml{\\@nleqq}{\u2270}"), Pr("\\nleqslant", "\\html@mathml{\\@nleqslant}{\u2270}"), Pr("\\nshortmid", "\\html@mathml{\\@nshortmid}{\u2224}"), Pr("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{\u2226}"), Pr("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{\u2288}"), Pr("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{\u2289}"), Pr("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{\u228a}"), Pr("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{\u2acb}"), Pr("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{\u228b}"), Pr("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{\u2acc}"), Pr("\\imath", "\\html@mathml{\\@imath}{\u0131}"), Pr("\\jmath", "\\html@mathml{\\@jmath}{\u0237}"), Pr("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`\u27e6}}"), Pr("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`\u27e7}}"), Pr("\u27e6", "\\llbracket"), Pr("\u27e7", "\\rrbracket"), Pr("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`\u2983}}"), Pr("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`\u2984}}"), Pr("\u2983", "\\lBrace"), Pr("\u2984", "\\rBrace"), Pr("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`\u29b5}}"), Pr("\u29b5", "\\minuso"), Pr("\\darr", "\\downarrow"), Pr("\\dArr", "\\Downarrow"), Pr("\\Darr", "\\Downarrow"), Pr("\\lang", "\\langle"), Pr("\\rang", "\\rangle"), Pr("\\uarr", "\\uparrow"), Pr("\\uArr", "\\Uparrow"), Pr("\\Uarr", "\\Uparrow"), Pr("\\N", "\\mathbb{N}"), Pr("\\R", "\\mathbb{R}"), Pr("\\Z", "\\mathbb{Z}"), Pr("\\alef", "\\aleph"), Pr("\\alefsym", "\\aleph"), Pr("\\Alpha", "\\mathrm{A}"), Pr("\\Beta", "\\mathrm{B}"), Pr("\\bull", "\\bullet"), Pr("\\Chi", "\\mathrm{X}"), Pr("\\clubs", "\\clubsuit"), Pr("\\cnums", "\\mathbb{C}"), Pr("\\Complex", "\\mathbb{C}"), Pr("\\Dagger", "\\ddagger"), Pr("\\diamonds", "\\diamondsuit"), Pr("\\empty", "\\emptyset"), Pr("\\Epsilon", "\\mathrm{E}"), Pr("\\Eta", "\\mathrm{H}"), Pr("\\exist", "\\exists"), Pr("\\harr", "\\leftrightarrow"), Pr("\\hArr", "\\Leftrightarrow"), Pr("\\Harr", "\\Leftrightarrow"), Pr("\\hearts", "\\heartsuit"), Pr("\\image", "\\Im"), Pr("\\infin", "\\infty"), Pr("\\Iota", "\\mathrm{I}"), Pr("\\isin", "\\in"), Pr("\\Kappa", "\\mathrm{K}"), Pr("\\larr", "\\leftarrow"), Pr("\\lArr", "\\Leftarrow"), Pr("\\Larr", "\\Leftarrow"), Pr("\\lrarr", "\\leftrightarrow"), Pr("\\lrArr", "\\Leftrightarrow"), Pr("\\Lrarr", "\\Leftrightarrow"), Pr("\\Mu", "\\mathrm{M}"), Pr("\\natnums", "\\mathbb{N}"), Pr("\\Nu", "\\mathrm{N}"), Pr("\\Omicron", "\\mathrm{O}"), Pr("\\plusmn", "\\pm"), Pr("\\rarr", "\\rightarrow"), Pr("\\rArr", "\\Rightarrow"), Pr("\\Rarr", "\\Rightarrow"), Pr("\\real", "\\Re"), Pr("\\reals", "\\mathbb{R}"), Pr("\\Reals", "\\mathbb{R}"), Pr("\\Rho", "\\mathrm{P}"), Pr("\\sdot", "\\cdot"), Pr("\\sect", "\\S"), Pr("\\spades", "\\spadesuit"), Pr("\\sub", "\\subset"), Pr("\\sube", "\\subseteq"), Pr("\\supe", "\\supseteq"), Pr("\\Tau", "\\mathrm{T}"), Pr("\\thetasym", "\\vartheta"), Pr("\\weierp", "\\wp"), Pr("\\Zeta", "\\mathrm{Z}"), Pr("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), Pr("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), Pr("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), Pr("\\bra", "\\mathinner{\\langle{#1}|}"), Pr("\\ket", "\\mathinner{|{#1}\\rangle}"), Pr("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), Pr("\\Bra", "\\left\\langle#1\\right|"), Pr("\\Ket", "\\left|#1\\right\\rangle");
-        var Fn = function(e) {
+        var Yn = F(T["Main-Regular"]["T".charCodeAt(0)][1] - .7 * T["Main-Regular"]["A".charCodeAt(0)][1]);
+        Pr("\\LaTeX", "\\textrm{\\html@mathml{L\\kern-.36em\\raisebox{" + Yn + "}{\\scriptstyle A}\\kern-.15em\\TeX}{LaTeX}}"), Pr("\\KaTeX", "\\textrm{\\html@mathml{K\\kern-.17em\\raisebox{" + Yn + "}{\\scriptstyle A}\\kern-.15em\\TeX}{KaTeX}}"), Pr("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), Pr("\\@hspace", "\\hskip #1\\relax"), Pr("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), Pr("\\ordinarycolon", ":"), Pr("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), Pr("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), Pr("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), Pr("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), Pr("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), Pr("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), Pr("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), Pr("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), Pr("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), Pr("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), Pr("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), Pr("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), Pr("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), Pr("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), Pr("\u2237", "\\dblcolon"), Pr("\u2239", "\\eqcolon"), Pr("\u2254", "\\coloneqq"), Pr("\u2255", "\\eqqcolon"), Pr("\u2a74", "\\Coloneqq"), Pr("\\ratio", "\\vcentcolon"), Pr("\\coloncolon", "\\dblcolon"), Pr("\\colonequals", "\\coloneqq"), Pr("\\coloncolonequals", "\\Coloneqq"), Pr("\\equalscolon", "\\eqqcolon"), Pr("\\equalscoloncolon", "\\Eqqcolon"), Pr("\\colonminus", "\\coloneq"), Pr("\\coloncolonminus", "\\Coloneq"), Pr("\\minuscolon", "\\eqcolon"), Pr("\\minuscoloncolon", "\\Eqcolon"), Pr("\\coloncolonapprox", "\\Colonapprox"), Pr("\\coloncolonsim", "\\Colonsim"), Pr("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Pr("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Pr("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Pr("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Pr("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`\u220c}}"), Pr("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), Pr("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), Pr("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), Pr("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), Pr("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), Pr("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), Pr("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), Pr("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), Pr("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{\u2269}"), Pr("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{\u2268}"), Pr("\\ngeqq", "\\html@mathml{\\@ngeqq}{\u2271}"), Pr("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{\u2271}"), Pr("\\nleqq", "\\html@mathml{\\@nleqq}{\u2270}"), Pr("\\nleqslant", "\\html@mathml{\\@nleqslant}{\u2270}"), Pr("\\nshortmid", "\\html@mathml{\\@nshortmid}{\u2224}"), Pr("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{\u2226}"), Pr("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{\u2288}"), Pr("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{\u2289}"), Pr("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{\u228a}"), Pr("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{\u2acb}"), Pr("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{\u228b}"), Pr("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{\u2acc}"), Pr("\\imath", "\\html@mathml{\\@imath}{\u0131}"), Pr("\\jmath", "\\html@mathml{\\@jmath}{\u0237}"), Pr("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`\u27e6}}"), Pr("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`\u27e7}}"), Pr("\u27e6", "\\llbracket"), Pr("\u27e7", "\\rrbracket"), Pr("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`\u2983}}"), Pr("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`\u2984}}"), Pr("\u2983", "\\lBrace"), Pr("\u2984", "\\rBrace"), Pr("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`\u29b5}}"), Pr("\u29b5", "\\minuso"), Pr("\\darr", "\\downarrow"), Pr("\\dArr", "\\Downarrow"), Pr("\\Darr", "\\Downarrow"), Pr("\\lang", "\\langle"), Pr("\\rang", "\\rangle"), Pr("\\uarr", "\\uparrow"), Pr("\\uArr", "\\Uparrow"), Pr("\\Uarr", "\\Uparrow"), Pr("\\N", "\\mathbb{N}"), Pr("\\R", "\\mathbb{R}"), Pr("\\Z", "\\mathbb{Z}"), Pr("\\alef", "\\aleph"), Pr("\\alefsym", "\\aleph"), Pr("\\Alpha", "\\mathrm{A}"), Pr("\\Beta", "\\mathrm{B}"), Pr("\\bull", "\\bullet"), Pr("\\Chi", "\\mathrm{X}"), Pr("\\clubs", "\\clubsuit"), Pr("\\cnums", "\\mathbb{C}"), Pr("\\Complex", "\\mathbb{C}"), Pr("\\Dagger", "\\ddagger"), Pr("\\diamonds", "\\diamondsuit"), Pr("\\empty", "\\emptyset"), Pr("\\Epsilon", "\\mathrm{E}"), Pr("\\Eta", "\\mathrm{H}"), Pr("\\exist", "\\exists"), Pr("\\harr", "\\leftrightarrow"), Pr("\\hArr", "\\Leftrightarrow"), Pr("\\Harr", "\\Leftrightarrow"), Pr("\\hearts", "\\heartsuit"), Pr("\\image", "\\Im"), Pr("\\infin", "\\infty"), Pr("\\Iota", "\\mathrm{I}"), Pr("\\isin", "\\in"), Pr("\\Kappa", "\\mathrm{K}"), Pr("\\larr", "\\leftarrow"), Pr("\\lArr", "\\Leftarrow"), Pr("\\Larr", "\\Leftarrow"), Pr("\\lrarr", "\\leftrightarrow"), Pr("\\lrArr", "\\Leftrightarrow"), Pr("\\Lrarr", "\\Leftrightarrow"), Pr("\\Mu", "\\mathrm{M}"), Pr("\\natnums", "\\mathbb{N}"), Pr("\\Nu", "\\mathrm{N}"), Pr("\\Omicron", "\\mathrm{O}"), Pr("\\plusmn", "\\pm"), Pr("\\rarr", "\\rightarrow"), Pr("\\rArr", "\\Rightarrow"), Pr("\\Rarr", "\\Rightarrow"), Pr("\\real", "\\Re"), Pr("\\reals", "\\mathbb{R}"), Pr("\\Reals", "\\mathbb{R}"), Pr("\\Rho", "\\mathrm{P}"), Pr("\\sdot", "\\cdot"), Pr("\\sect", "\\S"), Pr("\\spades", "\\spadesuit"), Pr("\\sub", "\\subset"), Pr("\\sube", "\\subseteq"), Pr("\\supe", "\\supseteq"), Pr("\\Tau", "\\mathrm{T}"), Pr("\\thetasym", "\\vartheta"), Pr("\\weierp", "\\wp"), Pr("\\Zeta", "\\mathrm{Z}"), Pr("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), Pr("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), Pr("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), Pr("\\bra", "\\mathinner{\\langle{#1}|}"), Pr("\\ket", "\\mathinner{|{#1}\\rangle}"), Pr("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), Pr("\\Bra", "\\left\\langle#1\\right|"), Pr("\\Ket", "\\left|#1\\right\\rangle");
+        var Xn = function(e) {
             return function(t) {
                 var r = t.consumeArg().tokens,
                     n = t.consumeArg().tokens,
                     a = t.consumeArg().tokens,
                     i = t.consumeArg().tokens,
                     o = t.macros.get("|"),
                     s = t.macros.get("\\|");
@@ -8410,28 +8414,28 @@
                     c = t.expandTokens([].concat(i, h, r));
                 return t.macros.endGroup(), {
                     tokens: c.reverse(),
                     numArgs: 0
                 }
             }
         };
-        Pr("\\bra@ket", Fn(!1)), Pr("\\bra@set", Fn(!0)), Pr("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), Pr("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), Pr("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), Pr("\\angln", "{\\angl n}"), Pr("\\blue", "\\textcolor{##6495ed}{#1}"), Pr("\\orange", "\\textcolor{##ffa500}{#1}"), Pr("\\pink", "\\textcolor{##ff00af}{#1}"), Pr("\\red", "\\textcolor{##df0030}{#1}"), Pr("\\green", "\\textcolor{##28ae7b}{#1}"), Pr("\\gray", "\\textcolor{gray}{#1}"), Pr("\\purple", "\\textcolor{##9d38bd}{#1}"), Pr("\\blueA", "\\textcolor{##ccfaff}{#1}"), Pr("\\blueB", "\\textcolor{##80f6ff}{#1}"), Pr("\\blueC", "\\textcolor{##63d9ea}{#1}"), Pr("\\blueD", "\\textcolor{##11accd}{#1}"), Pr("\\blueE", "\\textcolor{##0c7f99}{#1}"), Pr("\\tealA", "\\textcolor{##94fff5}{#1}"), Pr("\\tealB", "\\textcolor{##26edd5}{#1}"), Pr("\\tealC", "\\textcolor{##01d1c1}{#1}"), Pr("\\tealD", "\\textcolor{##01a995}{#1}"), Pr("\\tealE", "\\textcolor{##208170}{#1}"), Pr("\\greenA", "\\textcolor{##b6ffb0}{#1}"), Pr("\\greenB", "\\textcolor{##8af281}{#1}"), Pr("\\greenC", "\\textcolor{##74cf70}{#1}"), Pr("\\greenD", "\\textcolor{##1fab54}{#1}"), Pr("\\greenE", "\\textcolor{##0d923f}{#1}"), Pr("\\goldA", "\\textcolor{##ffd0a9}{#1}"), Pr("\\goldB", "\\textcolor{##ffbb71}{#1}"), Pr("\\goldC", "\\textcolor{##ff9c39}{#1}"), Pr("\\goldD", "\\textcolor{##e07d10}{#1}"), Pr("\\goldE", "\\textcolor{##a75a05}{#1}"), Pr("\\redA", "\\textcolor{##fca9a9}{#1}"), Pr("\\redB", "\\textcolor{##ff8482}{#1}"), Pr("\\redC", "\\textcolor{##f9685d}{#1}"), Pr("\\redD", "\\textcolor{##e84d39}{#1}"), Pr("\\redE", "\\textcolor{##bc2612}{#1}"), Pr("\\maroonA", "\\textcolor{##ffbde0}{#1}"), Pr("\\maroonB", "\\textcolor{##ff92c6}{#1}"), Pr("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), Pr("\\maroonD", "\\textcolor{##ca337c}{#1}"), Pr("\\maroonE", "\\textcolor{##9e034e}{#1}"), Pr("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), Pr("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), Pr("\\purpleC", "\\textcolor{##aa87ff}{#1}"), Pr("\\purpleD", "\\textcolor{##7854ab}{#1}"), Pr("\\purpleE", "\\textcolor{##543b78}{#1}"), Pr("\\mintA", "\\textcolor{##f5f9e8}{#1}"), Pr("\\mintB", "\\textcolor{##edf2df}{#1}"), Pr("\\mintC", "\\textcolor{##e0e5cc}{#1}"), Pr("\\grayA", "\\textcolor{##f6f7f7}{#1}"), Pr("\\grayB", "\\textcolor{##f0f1f2}{#1}"), Pr("\\grayC", "\\textcolor{##e3e5e6}{#1}"), Pr("\\grayD", "\\textcolor{##d6d8da}{#1}"), Pr("\\grayE", "\\textcolor{##babec2}{#1}"), Pr("\\grayF", "\\textcolor{##888d93}{#1}"), Pr("\\grayG", "\\textcolor{##626569}{#1}"), Pr("\\grayH", "\\textcolor{##3b3e40}{#1}"), Pr("\\grayI", "\\textcolor{##21242c}{#1}"), Pr("\\kaBlue", "\\textcolor{##314453}{#1}"), Pr("\\kaGreen", "\\textcolor{##71B307}{#1}");
-        var Gn = {
+        Pr("\\bra@ket", Xn(!1)), Pr("\\bra@set", Xn(!0)), Pr("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), Pr("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), Pr("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), Pr("\\angln", "{\\angl n}"), Pr("\\blue", "\\textcolor{##6495ed}{#1}"), Pr("\\orange", "\\textcolor{##ffa500}{#1}"), Pr("\\pink", "\\textcolor{##ff00af}{#1}"), Pr("\\red", "\\textcolor{##df0030}{#1}"), Pr("\\green", "\\textcolor{##28ae7b}{#1}"), Pr("\\gray", "\\textcolor{gray}{#1}"), Pr("\\purple", "\\textcolor{##9d38bd}{#1}"), Pr("\\blueA", "\\textcolor{##ccfaff}{#1}"), Pr("\\blueB", "\\textcolor{##80f6ff}{#1}"), Pr("\\blueC", "\\textcolor{##63d9ea}{#1}"), Pr("\\blueD", "\\textcolor{##11accd}{#1}"), Pr("\\blueE", "\\textcolor{##0c7f99}{#1}"), Pr("\\tealA", "\\textcolor{##94fff5}{#1}"), Pr("\\tealB", "\\textcolor{##26edd5}{#1}"), Pr("\\tealC", "\\textcolor{##01d1c1}{#1}"), Pr("\\tealD", "\\textcolor{##01a995}{#1}"), Pr("\\tealE", "\\textcolor{##208170}{#1}"), Pr("\\greenA", "\\textcolor{##b6ffb0}{#1}"), Pr("\\greenB", "\\textcolor{##8af281}{#1}"), Pr("\\greenC", "\\textcolor{##74cf70}{#1}"), Pr("\\greenD", "\\textcolor{##1fab54}{#1}"), Pr("\\greenE", "\\textcolor{##0d923f}{#1}"), Pr("\\goldA", "\\textcolor{##ffd0a9}{#1}"), Pr("\\goldB", "\\textcolor{##ffbb71}{#1}"), Pr("\\goldC", "\\textcolor{##ff9c39}{#1}"), Pr("\\goldD", "\\textcolor{##e07d10}{#1}"), Pr("\\goldE", "\\textcolor{##a75a05}{#1}"), Pr("\\redA", "\\textcolor{##fca9a9}{#1}"), Pr("\\redB", "\\textcolor{##ff8482}{#1}"), Pr("\\redC", "\\textcolor{##f9685d}{#1}"), Pr("\\redD", "\\textcolor{##e84d39}{#1}"), Pr("\\redE", "\\textcolor{##bc2612}{#1}"), Pr("\\maroonA", "\\textcolor{##ffbde0}{#1}"), Pr("\\maroonB", "\\textcolor{##ff92c6}{#1}"), Pr("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), Pr("\\maroonD", "\\textcolor{##ca337c}{#1}"), Pr("\\maroonE", "\\textcolor{##9e034e}{#1}"), Pr("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), Pr("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), Pr("\\purpleC", "\\textcolor{##aa87ff}{#1}"), Pr("\\purpleD", "\\textcolor{##7854ab}{#1}"), Pr("\\purpleE", "\\textcolor{##543b78}{#1}"), Pr("\\mintA", "\\textcolor{##f5f9e8}{#1}"), Pr("\\mintB", "\\textcolor{##edf2df}{#1}"), Pr("\\mintC", "\\textcolor{##e0e5cc}{#1}"), Pr("\\grayA", "\\textcolor{##f6f7f7}{#1}"), Pr("\\grayB", "\\textcolor{##f0f1f2}{#1}"), Pr("\\grayC", "\\textcolor{##e3e5e6}{#1}"), Pr("\\grayD", "\\textcolor{##d6d8da}{#1}"), Pr("\\grayE", "\\textcolor{##babec2}{#1}"), Pr("\\grayF", "\\textcolor{##888d93}{#1}"), Pr("\\grayG", "\\textcolor{##626569}{#1}"), Pr("\\grayH", "\\textcolor{##3b3e40}{#1}"), Pr("\\grayI", "\\textcolor{##21242c}{#1}"), Pr("\\kaBlue", "\\textcolor{##314453}{#1}"), Pr("\\kaGreen", "\\textcolor{##71B307}{#1}");
+        var Wn = {
                 "^": !0,
                 _: !0,
                 "\\limits": !0,
                 "\\nolimits": !0
             },
-            Un = function() {
+            _n = function() {
                 function e(e, t, r) {
-                    this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = t, this.expansionCount = 0, this.feed(e), this.macros = new Hn(On, t.macros), this.mode = r, this.stack = []
+                    this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = t, this.expansionCount = 0, this.feed(e), this.macros = new Dn(Vn, t.macros), this.mode = r, this.stack = []
                 }
                 var t = e.prototype;
                 return t.feed = function(e) {
-                    this.lexer = new Rn(e, this.settings)
+                    this.lexer = new Ln(e, this.settings)
                 }, t.switchMode = function(e) {
                     this.mode = e
                 }, t.beginGroup = function() {
                     this.macros.beginGroup()
                 }, t.endGroup = function() {
                     this.macros.endGroup()
                 }, t.endGroups = function() {
@@ -8499,15 +8503,15 @@
                     return o
                 }, t.expandOnce = function(e) {
                     var t = this.popToken(),
                         r = t.text,
                         a = t.noexpand ? null : this._getExpansion(r);
                     if (null == a || e && a.unexpandable) {
                         if (e && null == a && "\\" === r[0] && !this.isDefined(r)) throw new n("Undefined control sequence: " + r);
-                        return this.pushToken(t), t
+                        return this.pushToken(t), !1
                     }
                     if (this.expansionCount++, this.expansionCount > this.settings.maxExpand) throw new n("Too many expansions: infinite loop or need to increase maxExpand setting");
                     var i = a.tokens,
                         o = this.consumeArgs(a.numArgs, a.delimiters);
                     if (a.numArgs)
                         for (var s = (i = i.slice()).length - 1; s >= 0; --s) {
                             var l = i[s];
@@ -8517,33 +8521,33 @@
                                 else {
                                     if (!/^[1-9]$/.test(l.text)) throw new n("Not a valid argument number", l);
                                     var h;
                                     (h = i).splice.apply(h, [s, 2].concat(o[+l.text - 1]))
                                 }
                             }
                         }
-                    return this.pushTokens(i), i
+                    return this.pushTokens(i), i.length
                 }, t.expandAfterFuture = function() {
                     return this.expandOnce(), this.future()
                 }, t.expandNextToken = function() {
-                    for (;;) {
-                        var e = this.expandOnce();
-                        if (e instanceof Gr) return e.treatAsRelax && (e.text = "\\relax"), this.stack.pop()
-                    }
-                    throw new Error
+                    for (;;)
+                        if (!1 === this.expandOnce()) {
+                            var e = this.stack.pop();
+                            return e.treatAsRelax && (e.text = "\\relax"), e
+                        } throw new Error
                 }, t.expandMacro = function(e) {
                     return this.macros.has(e) ? this.expandTokens([new Gr(e)]) : void 0
                 }, t.expandTokens = function(e) {
                     var t = [],
                         r = this.stack.length;
-                    for (this.pushTokens(e); this.stack.length > r;) {
-                        var n = this.expandOnce(!0);
-                        n instanceof Gr && (n.treatAsRelax && (n.noexpand = !1, n.treatAsRelax = !1), t.push(this.stack.pop()))
-                    }
-                    return t
+                    for (this.pushTokens(e); this.stack.length > r;)
+                        if (!1 === this.expandOnce(!0)) {
+                            var n = this.stack.pop();
+                            n.treatAsRelax && (n.noexpand = !1, n.treatAsRelax = !1), t.push(n)
+                        } return t
                 }, t.expandMacroAsText = function(e) {
                     var t = this.expandMacro(e);
                     return t ? t.map((function(e) {
                         return e.text
                     })).join("") : t
                 }, t._getExpansion = function(e) {
                     var t = this.macros.get(e);
@@ -8553,31 +8557,31 @@
                         if (null != r && 13 !== r) return
                     }
                     var n = "function" == typeof t ? t(this) : t;
                     if ("string" == typeof n) {
                         var a = 0;
                         if (-1 !== n.indexOf("#"))
                             for (var i = n.replace(/##/g, ""); - 1 !== i.indexOf("#" + (a + 1));) ++a;
-                        for (var o = new Rn(n, this.settings), s = [], l = o.lex();
+                        for (var o = new Ln(n, this.settings), s = [], l = o.lex();
                             "EOF" !== l.text;) s.push(l), l = o.lex();
                         return s.reverse(), {
                             tokens: s,
                             numArgs: a
                         }
                     }
                     return n
                 }, t.isDefined = function(e) {
-                    return this.macros.has(e) || qn.hasOwnProperty(e) || ae.math.hasOwnProperty(e) || ae.text.hasOwnProperty(e) || Gn.hasOwnProperty(e)
+                    return this.macros.has(e) || qn.hasOwnProperty(e) || ae.math.hasOwnProperty(e) || ae.text.hasOwnProperty(e) || Wn.hasOwnProperty(e)
                 }, t.isExpandable = function(e) {
                     var t = this.macros.get(e);
                     return null != t ? "string" == typeof t || "function" == typeof t || !t.unexpandable : qn.hasOwnProperty(e) && !qn[e].primitive
                 }, e
             }(),
-            Yn = /^[\u208a\u208b\u208c\u208d\u208e\u2080\u2081\u2082\u2083\u2084\u2085\u2086\u2087\u2088\u2089\u2090\u2091\u2095\u1d62\u2c7c\u2096\u2097\u2098\u2099\u2092\u209a\u1d63\u209b\u209c\u1d64\u1d65\u2093\u1d66\u1d67\u1d68\u1d69\u1d6a]/,
-            Xn = Object.freeze({
+            jn = /^[\u208a\u208b\u208c\u208d\u208e\u2080\u2081\u2082\u2083\u2084\u2085\u2086\u2087\u2088\u2089\u2090\u2091\u2095\u1d62\u2c7c\u2096\u2097\u2098\u2099\u2092\u209a\u1d63\u209b\u209c\u1d64\u1d65\u2093\u1d66\u1d67\u1d68\u1d69\u1d6a]/,
+            $n = Object.freeze({
                 "\u208a": "+",
                 "\u208b": "-",
                 "\u208c": "=",
                 "\u208d": "(",
                 "\u208e": ")",
                 "\u2080": "0",
                 "\u2081": "1",
@@ -8673,15 +8677,15 @@
                 "\u1d5d": "\u03b2",
                 "\u1d5e": "\u03b3",
                 "\u1d5f": "\u03b4",
                 "\u1d60": "\u03d5",
                 "\u1d61": "\u03c7",
                 "\u1dbf": "\u03b8"
             }),
-            Wn = {
+            Zn = {
                 "\u0301": {
                     text: "\\'",
                     math: "\\acute"
                 },
                 "\u0300": {
                     text: "\\`",
                     math: "\\grave"
@@ -8721,15 +8725,15 @@
                 "\u030b": {
                     text: "\\H"
                 },
                 "\u0327": {
                     text: "\\c"
                 }
             },
-            _n = {
+            Kn = {
                 "\xe1": "a\u0301",
                 "\xe0": "a\u0300",
                 "\xe4": "a\u0308",
                 "\u01df": "a\u0308\u0304",
                 "\xe3": "a\u0303",
                 "\u0101": "a\u0304",
                 "\u0103": "a\u0306",
@@ -9067,17 +9071,17 @@
                 "\u1fea": "\u03a5\u0300",
                 "\u03ab": "\u03a5\u0308",
                 "\u1fe9": "\u03a5\u0304",
                 "\u1fe8": "\u03a5\u0306",
                 "\u038f": "\u03a9\u0301",
                 "\u1ffa": "\u03a9\u0300"
             },
-            jn = function() {
+            Jn = function() {
                 function e(e, t) {
-                    this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new Un(e, t, this.mode), this.settings = t, this.leftrightDepth = 0
+                    this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new _n(e, t, this.mode), this.settings = t, this.leftrightDepth = 0
                 }
                 var t = e.prototype;
                 return t.expect = function(e, t) {
                     if (void 0 === t && (t = !0), this.fetch().text !== e) throw new n("Expected '" + e + "', got '" + this.fetch().text + "'", this.fetch());
                     t && this.consume()
                 }, t.consume = function() {
                     this.nextToken = null
@@ -9186,22 +9190,22 @@
                                 "'" === this.fetch().text;) h.push(l), this.consume();
                             "^" === this.fetch().text && h.push(this.handleSupSubscript("superscript")), r = {
                                 type: "ordgroup",
                                 mode: this.mode,
                                 body: h
                             }
                         } else {
-                            if (!Xn[o.text]) break;
-                            var c = Xn[o.text],
-                                m = Yn.test(o.text);
+                            if (!$n[o.text]) break;
+                            var c = $n[o.text],
+                                m = jn.test(o.text);
                             for (this.consume();;) {
                                 var u = this.fetch().text;
-                                if (!Xn[u]) break;
-                                if (Yn.test(u) !== m) break;
-                                this.consume(), c += Xn[u]
+                                if (!$n[u]) break;
+                                if (jn.test(u) !== m) break;
+                                this.consume(), c += $n[u]
                             }
                             var p = new e(c, this.settings).parse();
                             m ? a = {
                                 type: "ordgroup",
                                 mode: "math",
                                 body: p
                             } : r = {
@@ -9377,15 +9381,15 @@
                         this.expect(o), this.gullet.endGroup(), r = {
                             type: "ordgroup",
                             mode: this.mode,
                             loc: Fr.range(a, l),
                             body: s,
                             semisimple: "\\begingroup" === i || void 0
                         }
-                    } else if (null == (r = this.parseFunction(t, e) || this.parseSymbol()) && "\\" === i[0] && !Gn.hasOwnProperty(i)) {
+                    } else if (null == (r = this.parseFunction(t, e) || this.parseSymbol()) && "\\" === i[0] && !Wn.hasOwnProperty(i)) {
                         if (this.settings.throwOnError) throw new n("Undefined control sequence: " + i, a);
                         r = this.formatUnsupportedCmd(i), this.consume()
                     }
                     return r
                 }, t.formLigatures = function(e) {
                     for (var t = e.length - 1, r = 0; r < t; ++r) {
                         var n = e[r],
@@ -9418,16 +9422,16 @@
                         return {
                             type: "verb",
                             mode: "text",
                             body: r = r.slice(1, -1),
                             star: a
                         }
                     }
-                    _n.hasOwnProperty(t[0]) && !ae[this.mode][t[0]] && (this.settings.strict && "math" === this.mode && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + t[0] + '" used in math mode', e), t = _n[t[0]] + t.slice(1));
-                    var i, o = In.exec(t);
+                    Kn.hasOwnProperty(t[0]) && !ae[this.mode][t[0]] && (this.settings.strict && "math" === this.mode && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + t[0] + '" used in math mode', e), t = Kn[t[0]] + t.slice(1));
+                    var i, o = On.exec(t);
                     if (o && ("i" === (t = t.substring(0, o.index)) ? t = "\u0131" : "j" === t && (t = "\u0237")), ae[this.mode][t]) {
                         this.settings.strict && "math" === this.mode && Ee.indexOf(t) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + t[0] + '" used in math mode', e);
                         var s, l = ae[this.mode][t].group,
                             h = Fr.range(e);
                         if (te.hasOwnProperty(l)) {
                             var c = l;
                             s = {
@@ -9452,98 +9456,99 @@
                             loc: Fr.range(e),
                             text: t
                         }
                     }
                     if (this.consume(), o)
                         for (var m = 0; m < o[0].length; m++) {
                             var u = o[0][m];
-                            if (!Wn[u]) throw new n("Unknown accent ' " + u + "'", e);
-                            var p = Wn[u][this.mode] || Wn[u].text;
+                            if (!Zn[u]) throw new n("Unknown accent ' " + u + "'", e);
+                            var p = Zn[u][this.mode] || Zn[u].text;
                             if (!p) throw new n("Accent " + u + " unsupported in " + this.mode + " mode", e);
                             i = {
                                 type: "accent",
                                 mode: this.mode,
                                 loc: Fr.range(e),
                                 label: p,
                                 isStretchy: !1,
                                 isShifty: !0,
                                 base: i
                             }
                         }
                     return i
                 }, e
             }();
-        jn.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"];
-        var $n = function(e, t) {
+        Jn.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"];
+        var Qn = function(e, t) {
                 if (!("string" == typeof e || e instanceof String)) throw new TypeError("KaTeX can only parse string typed expression");
-                var r = new jn(e, t);
+                var r = new Jn(e, t);
                 delete r.gullet.macros.current["\\df@tag"];
                 var a = r.parse();
                 if (delete r.gullet.macros.current["\\current@color"], delete r.gullet.macros.current["\\color"], r.gullet.macros.get("\\df@tag")) {
                     if (!t.displayMode) throw new n("\\tag works only in display equations");
                     a = [{
                         type: "tag",
                         mode: "text",
                         body: a,
                         tag: r.subparse([new Gr("\\df@tag")])
                     }]
                 }
                 return a
             },
-            Zn = function(e, t, r) {
+            ea = function(e, t, r) {
                 t.textContent = "";
-                var n = Jn(e, r).toNode();
+                var n = ra(e, r).toNode();
                 t.appendChild(n)
             };
-        "undefined" != typeof document && "CSS1Compat" !== document.compatMode && ("undefined" != typeof console && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), Zn = function() {
+        "undefined" != typeof document && "CSS1Compat" !== document.compatMode && ("undefined" != typeof console && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), ea = function() {
             throw new n("KaTeX doesn't work in quirks mode.")
         });
-        var Kn = function(e, t, r) {
+        var ta = function(e, t, r) {
                 if (r.throwOnError || !(e instanceof n)) throw e;
                 var a = Ke.makeSpan(["katex-error"], [new Z(t)]);
                 return a.setAttribute("title", e.toString()), a.setAttribute("style", "color:" + r.errorColor), a
             },
-            Jn = function(e, t) {
+            ra = function(e, t) {
                 var r = new m(t);
                 try {
-                    var n = $n(e, r);
+                    var n = Qn(e, r);
                     return Lt(n, e, r)
                 } catch (t) {
-                    return Kn(t, e, r)
+                    return ta(t, e, r)
                 }
             },
-            Qn = {
-                version: "0.16.4",
-                render: Zn,
+            na = {
+                version: "0.16.7",
+                render: ea,
                 renderToString: function(e, t) {
-                    return Jn(e, t).toMarkup()
+                    return ra(e, t).toMarkup()
                 },
                 ParseError: n,
                 SETTINGS_SCHEMA: h,
                 __parse: function(e, t) {
                     var r = new m(t);
-                    return $n(e, r)
+                    return Qn(e, r)
                 },
-                __renderToDomTree: Jn,
+                __renderToDomTree: ra,
                 __renderToHTMLTree: function(e, t) {
                     var r = new m(t);
                     try {
                         return function(e, t, r) {
                             var n = St(e, Ot(r)),
                                 a = Ke.makeSpan(["katex"], [n]);
                             return Et(a, r)
-                        }($n(e, r), 0, r)
+                        }(Qn(e, r), 0, r)
                     } catch (t) {
-                        return Kn(t, e, r)
+                        return ta(t, e, r)
                     }
                 },
                 __setFontMetrics: function(e, t) {
                     T[e] = t
                 },
                 __defineSymbol: ie,
+                __defineFunction: ot,
                 __defineMacro: Pr,
                 __domTree: {
                     Span: W,
                     Anchor: _,
                     SymbolNode: Z,
                     SvgNode: K,
                     PathNode: J,
```

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib/katex.py` & `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from subprocess import PIPE, Popen, TimeoutExpired
 
 from sphinx.locale import _
 from sphinx.errors import ExtensionError
 from sphinx.util.osutil import copyfile
 
 
-__version__ = '0.9.4'
-katex_version = '0.16.4'
+__version__ = '0.9.5'
+katex_version = '0.16.7'
 filename_css = 'katex-math.css'
 filename_autorenderer = 'katex_autorenderer.js'
 SRC_DIR = Path(__file__).parent
 SCRIPT_PATH = str(SRC_DIR / "katex-server.js")
 
 ONE_MILLISECOND = 0.001
 
@@ -358,16 +358,16 @@
 
     # global instance
     KATEX_SERVER = None
 
     # wait for the server to stop in seconds
     STOP_TIMEOUT = 0.1
 
-    @staticmethod
-    def timeout_error(self, timeout):
+    @classmethod
+    def timeout_error(cls, timeout):
         message = STARTUP_TIMEOUT_EXPIRED.format(timeout)
         return KaTeXError(message)
 
     @staticmethod
     def build_command(socket=None, port=None):
         cmd = [NODEJS_BINARY, SCRIPT_PATH]
```

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/PKG-INFO` & `sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Sphinx extension for rendering math in HTML pages
 Home-page: https://github.com/hagenw/sphinxcontrib-katex
 Author: Hagen Wierstorf
 Author-email: hagenw@posteo.de
 License: MIT
 Keywords: sphinx,latex,katex,math,documentation
 Platform: any
@@ -105,15 +105,15 @@
 The behavior of ``sphinxcontrib.katex`` can be changed by configuration
 entries in ``conf.py`` of your documentation project. In the following
 all configuration entries are listed and their default values are shown.
 
 .. code-block:: python
 
     katex_css_path = \
-        'https://cdn.jsdelivr.net/npm/katex@0.16.4/dist/katex.min.css'
+        'https://cdn.jsdelivr.net/npm/katex@0.16.7/dist/katex.min.css'
     katex_js_path = 'katex.min.js'
     katex_autorender_path = 'auto-render.min.js'
     katex_inline = [r'\(', r'\)']
     katex_display = [r'\[', r'\]']
     katex_prerender = False
     katex_options = ''
 
@@ -201,14 +201,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.5 (2023-06-07)
+--------------------------
+
+* Changed: use KaTeX 0.16.7
+* Fixed: convert ``KaTeXServer.timeout_error()``
+  to class method
+
+
 Version 0.9.4 (2023-01-04)
 --------------------------
 
 * Changed: use KaTeX 0.16.4
 
 
 Version 0.9.3 (2022-11-25)
```

### Comparing `sphinxcontrib-katex-0.9.4/sphinxcontrib_katex.egg-info/SOURCES.txt` & `sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

