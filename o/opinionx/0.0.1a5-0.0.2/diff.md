# Comparing `tmp/opinionx-0.0.1a5.tar.gz` & `tmp/opinionx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\UIBE??\?????\????\opinionx\dist\tmpo7xmo535\opinionx-0.0.1a5.tar", last modified: Sat Jan 29 22:55:31 2022, max compression
+gzip compressed data, was "opinionx-0.0.2.tar", last modified: Wed Jun  7 01:22:54 2023, max compression
```

## Comparing `opinionx-0.0.1a5.tar` & `opinionx-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 opinionx-0.0.1a5/LICENSE
--rw-rw-rw-   0        0        0      278 2022-01-16 05:22:04.000000 opinionx-0.0.1a5/MANIFEST.in
--rw-rw-rw-   0        0        0     2790 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/PKG-INFO
--rw-rw-rw-   0        0        0     1678 2022-01-17 14:30:56.000000 opinionx-0.0.1a5/README.md
--rw-rw-rw-   0        0        0       81 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/setup.cfg
--rw-rw-rw-   0        0        0     8623 2022-01-29 22:55:10.000000 opinionx-0.0.1a5/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx/
--rw-rw-rw-   0        0        0      349 2022-01-17 14:48:19.000000 opinionx-0.0.1a5/src/opinionx/content.py
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx/data/
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx/data/stopwords/
--rw-rw-rw-   0        0        0     9131 2020-03-04 12:49:10.000000 opinionx-0.0.1a5/src/opinionx/data/stopwords/baidu_stopwords.txt
--rw-rw-rw-   0        0        0     4717 2020-03-04 12:49:10.000000 opinionx-0.0.1a5/src/opinionx/data/stopwords/cn_stopwords.txt
--rw-rw-rw-   0        0        0     5273 2020-03-04 12:49:10.000000 opinionx-0.0.1a5/src/opinionx/data/stopwords/hit_stopwords.txt
--rw-rw-rw-   0        0        0     7597 2020-03-04 12:49:10.000000 opinionx-0.0.1a5/src/opinionx/data/stopwords/scu_stopwords.txt
--rw-rw-rw-   0        0        0     5195 2022-01-29 22:55:10.000000 opinionx-0.0.1a5/src/opinionx/text.py
--rw-rw-rw-   0        0        0    11214 2022-01-17 14:41:55.000000 opinionx-0.0.1a5/src/opinionx/tfidf.py
--rw-rw-rw-   0        0        0     2029 2022-01-17 14:59:17.000000 opinionx-0.0.1a5/src/opinionx/tfidf_shell.py
--rw-rw-rw-   0        0        0       71 2022-01-26 03:49:02.000000 opinionx-0.0.1a5/src/opinionx/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx/__pycache__/
--rw-rw-rw-   0        0        0      588 2022-01-17 14:48:20.000000 opinionx-0.0.1a5/src/opinionx/__pycache__/content.cpython-36.pyc
--rw-rw-rw-   0        0        0     2937 2022-01-17 12:57:14.000000 opinionx-0.0.1a5/src/opinionx/__pycache__/text.cpython-36.pyc
--rw-rw-rw-   0        0        0     9354 2022-01-17 14:55:43.000000 opinionx-0.0.1a5/src/opinionx/__pycache__/tfidf.cpython-36.pyc
--rw-rw-rw-   0        0        0     1178 2022-01-17 14:59:17.000000 opinionx-0.0.1a5/src/opinionx/__pycache__/tfidf_shell.cpython-36.pyc
--rw-rw-rw-   0        0        0      162 2022-01-16 08:06:11.000000 opinionx-0.0.1a5/src/opinionx/__pycache__/__init__.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx.egg-info/
--rw-rw-rw-   0        0        0        1 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2790 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      113 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      772 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2022-01-29 22:55:31.000000 opinionx-0.0.1a5/src/opinionx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.216787 opinionx-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 opinionx-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      278 2022-01-16 05:22:04.000000 opinionx-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2765 2023-06-07 01:22:54.216787 opinionx-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1678 2022-01-17 14:30:56.000000 opinionx-0.0.2/README.md
+-rw-rw-rw-   0        0        0       81 2023-06-07 01:22:54.224788 opinionx-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     8621 2023-06-07 01:20:12.000000 opinionx-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.090791 opinionx-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.097790 opinionx-0.0.2/src/opinionx/
+-rw-rw-rw-   0        0        0       71 2022-01-26 03:49:02.000000 opinionx-0.0.2/src/opinionx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.181788 opinionx-0.0.2/src/opinionx/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-01-16 08:06:11.000000 opinionx-0.0.2/src/opinionx/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      588 2022-01-17 14:48:20.000000 opinionx-0.0.2/src/opinionx/__pycache__/content.cpython-36.pyc
+-rw-rw-rw-   0        0        0     2937 2022-01-17 12:57:14.000000 opinionx-0.0.2/src/opinionx/__pycache__/text.cpython-36.pyc
+-rw-rw-rw-   0        0        0     9354 2022-01-17 14:55:43.000000 opinionx-0.0.2/src/opinionx/__pycache__/tfidf.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1178 2022-01-17 14:59:17.000000 opinionx-0.0.2/src/opinionx/__pycache__/tfidf_shell.cpython-36.pyc
+-rw-rw-rw-   0        0        0      349 2022-01-17 14:48:19.000000 opinionx-0.0.2/src/opinionx/content.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.090791 opinionx-0.0.2/src/opinionx/data/
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.215788 opinionx-0.0.2/src/opinionx/data/stopwords/
+-rw-rw-rw-   0        0        0     9131 2020-03-04 12:49:10.000000 opinionx-0.0.2/src/opinionx/data/stopwords/baidu_stopwords.txt
+-rw-rw-rw-   0        0        0     4717 2020-03-04 12:49:10.000000 opinionx-0.0.2/src/opinionx/data/stopwords/cn_stopwords.txt
+-rw-rw-rw-   0        0        0     5273 2020-03-04 12:49:10.000000 opinionx-0.0.2/src/opinionx/data/stopwords/hit_stopwords.txt
+-rw-rw-rw-   0        0        0     7597 2020-03-04 12:49:10.000000 opinionx-0.0.2/src/opinionx/data/stopwords/scu_stopwords.txt
+-rw-rw-rw-   0        0        0     4232 2022-02-04 05:37:38.000000 opinionx-0.0.2/src/opinionx/lda.py
+-rw-rw-rw-   0        0        0     5195 2022-01-29 22:55:10.000000 opinionx-0.0.2/src/opinionx/text.py
+-rw-rw-rw-   0        0        0    11665 2023-06-07 01:20:12.000000 opinionx-0.0.2/src/opinionx/tfidf.py
+-rw-rw-rw-   0        0        0     2029 2022-01-17 14:59:17.000000 opinionx-0.0.2/src/opinionx/tfidf_shell.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:22:54.145789 opinionx-0.0.2/src/opinionx.egg-info/
+-rw-rw-rw-   0        0        0     2765 2023-06-07 01:22:54.000000 opinionx-0.0.2/src/opinionx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2023-06-07 01:22:54.000000 opinionx-0.0.2/src/opinionx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 01:22:54.000000 opinionx-0.0.2/src/opinionx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-06-07 01:22:54.000000 opinionx-0.0.2/src/opinionx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 01:22:54.000000 opinionx-0.0.2/src/opinionx.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opinionx-0.0.1a5/LICENSE` & `opinionx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/PKG-INFO` & `opinionx-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: opinionx
-Version: 0.0.1a5
+Version: 0.0.2
 Summary: Opinion Analysis Toolkit
 Home-page: https://github.com/dhchenx/opinionx
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/opinionx/issues
 Project-URL: Source, https://github.com/dhchenx/opinionx
 Keywords: public opinion analysis,text analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -76,9 +75,7 @@
 
 - [Stanza](https://stanfordnlp.github.io/stanza/index.html)
 - [jieba](https://github.com/fxsjy/jieba)
 
 ### License
 The `opinionx` project is provided by [Donghua Chen](https://github.com/dhchenx). 
 
-
-
```

### Comparing `opinionx-0.0.1a5/README.md` & `opinionx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/setup.py` & `opinionx-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1a5',  # Required
+    version='0.0.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Opinion Analysis Toolkit',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `opinionx-0.0.1a5/src/opinionx/data/stopwords/baidu_stopwords.txt` & `opinionx-0.0.2/src/opinionx/data/stopwords/baidu_stopwords.txt`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/data/stopwords/cn_stopwords.txt` & `opinionx-0.0.2/src/opinionx/data/stopwords/cn_stopwords.txt`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/data/stopwords/hit_stopwords.txt` & `opinionx-0.0.2/src/opinionx/data/stopwords/hit_stopwords.txt`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/data/stopwords/scu_stopwords.txt` & `opinionx-0.0.2/src/opinionx/data/stopwords/scu_stopwords.txt`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/text.py` & `opinionx-0.0.2/src/opinionx/text.py`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/tfidf.py` & `opinionx-0.0.2/src/opinionx/tfidf.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,24 +87,37 @@
     list_word=[]
     for word, flag in words:
         # temp = "%s_%s " % (word, flag)
         # result1 = result1 + temp
         list_word.append([word,flag])
     return list_word
 
+def get_meaningful_words(doc):
+    list_words = peg.cut(doc)
+    list_w = []
+    for w, f in list_words:
+        # print(w,f)
+        if f in ['n',  'nr1','nr2','nrj','nrf','nsf',  'nt', 'nz', 'nl','ng','v','vn', 'vd','nd', 'nh', 'nl', 'i','x','a','ad']:
+            if w not in list_words and len(w) != 1:
+                list_w.append(w)
+    return list_w
+
+
 def process_text_into_tokens(text):
     text=text.strip()
     lines=text.split("\n")
     tokens=[]
     for line in lines:
         line=line.strip()
         sentences=line.split("。")
         for sentence in sentences:
             sentence=sentence.strip()
             # words=jieba.cut(sentence,cut_all=False)
+            list_w=get_meaningful_words(sentence)
+            '''
             words=seg_cut(sentence)
             new_words=[]
             for item in words:
                 w=item[0]
                 pos=item[1]
                 w=w.strip()
                 w = w.lower()
@@ -114,16 +127,16 @@
                     continue
                 if len(w)==4 and w.isnumeric() and not w.startswith("20") and not w.startswith("19"):
                     continue
                 if pos not in ['n']: # 词性过滤
                     continue
                 if not w in list_stopwords:
                     new_words.append(w)
-
-            for w in new_words:
+            '''
+            for w in list_w:
                 tokens.append(w)
     return tokens
 
 
 
 class KeyWordsBasesOnTermFreq():
```

### Comparing `opinionx-0.0.1a5/src/opinionx/tfidf_shell.py` & `opinionx-0.0.2/src/opinionx/tfidf_shell.py`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/__pycache__/content.cpython-36.pyc` & `opinionx-0.0.2/src/opinionx/__pycache__/content.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/__pycache__/text.cpython-36.pyc` & `opinionx-0.0.2/src/opinionx/__pycache__/text.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/__pycache__/tfidf.cpython-36.pyc` & `opinionx-0.0.2/src/opinionx/__pycache__/tfidf.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx/__pycache__/tfidf_shell.cpython-36.pyc` & `opinionx-0.0.2/src/opinionx/__pycache__/tfidf_shell.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `opinionx-0.0.1a5/src/opinionx.egg-info/PKG-INFO` & `opinionx-0.0.2/src/opinionx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: opinionx
-Version: 0.0.1a5
+Version: 0.0.2
 Summary: Opinion Analysis Toolkit
 Home-page: https://github.com/dhchenx/opinionx
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/opinionx/issues
 Project-URL: Source, https://github.com/dhchenx/opinionx
 Keywords: public opinion analysis,text analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -76,9 +75,7 @@
 
 - [Stanza](https://stanfordnlp.github.io/stanza/index.html)
 - [jieba](https://github.com/fxsjy/jieba)
 
 ### License
 The `opinionx` project is provided by [Donghua Chen](https://github.com/dhchenx). 
 
-
-
```

### Comparing `opinionx-0.0.1a5/src/opinionx.egg-info/SOURCES.txt` & `opinionx-0.0.2/src/opinionx.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 src/opinionx/__init__.py
 src/opinionx/content.py
+src/opinionx/lda.py
 src/opinionx/text.py
 src/opinionx/tfidf.py
 src/opinionx/tfidf_shell.py
 src/opinionx.egg-info/PKG-INFO
 src/opinionx.egg-info/SOURCES.txt
 src/opinionx.egg-info/dependency_links.txt
 src/opinionx.egg-info/requires.txt
```

