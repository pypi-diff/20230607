# Comparing `tmp/markdownparser-0.5.0.tar.gz` & `tmp/markdownparser-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.0.tar", max compression
+gzip compressed data, was "markdownparser-0.5.1.tar", max compression
```

## Comparing `markdownparser-0.5.0.tar` & `markdownparser-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.0/LICENSE
--rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.0/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5798 2023-04-28 16:45:24.751198 markdownparser-0.5.0/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    23756 2023-06-07 17:04:24.782153 markdownparser-0.5.0/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     6831 2023-06-07 17:08:57.851143 markdownparser-0.5.0/MarkdownParser/core.py
--rw-r--r--   0        0        0     3329 2023-04-28 12:24:15.406020 markdownparser-0.5.0/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21511 2023-05-24 14:55:53.230047 markdownparser-0.5.0/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-06-07 17:09:12.973979 markdownparser-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4799 2023-06-06 07:17:04.103864 markdownparser-0.5.0/README.md
--rw-r--r--   0        0        0     5572 1970-01-01 00:00:00.000000 markdownparser-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.1/LICENSE
+-rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.1/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5798 2023-04-28 16:45:24.751198 markdownparser-0.5.1/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    23723 2023-06-07 17:45:16.263585 markdownparser-0.5.1/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     6831 2023-06-07 17:43:22.492464 markdownparser-0.5.1/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3329 2023-04-28 12:24:15.406020 markdownparser-0.5.1/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21511 2023-05-24 14:55:53.230047 markdownparser-0.5.1/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-06-07 17:47:12.001165 markdownparser-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4743 2023-06-07 17:14:23.962993 markdownparser-0.5.1/README.md
+-rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 markdownparser-0.5.1/PKG-INFO
```

### Comparing `markdownparser-0.5.0/LICENSE` & `markdownparser-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.0/MarkdownParser/base_class.py` & `markdownparser-0.5.1/MarkdownParser/base_class.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.0/MarkdownParser/block_parser.py` & `markdownparser-0.5.1/MarkdownParser/block_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -743,16 +743,15 @@
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
 
         # fix bug: 修复一些 <abc> 这种虽然不匹配网址, 但是会被 html 解析为标签的情况
         # 见 test14.md
-        RE = re.compile(r'<([A-Za-z][^ ]*)>')
-        self.input['word'] = re.sub(RE,r'&lt\1&gt', self.input['word'])
+        self.input['word'] = self.input['word'].replace('<','&lt').replace('>','&gt')
 
         return self.input['word']
 
 
 def buildBlockParser():
     # block parser 用于逐行处理文本, 并将结果解析为一颗未优化的树
     block_parser = BlockParser()
```

### Comparing `markdownparser-0.5.0/MarkdownParser/core.py` & `markdownparser-0.5.1/MarkdownParser/core.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.0/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.1/MarkdownParser/preprocess_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.0/MarkdownParser/tree_parser.py` & `markdownparser-0.5.1/MarkdownParser/tree_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.0/README.md` & `markdownparser-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 # 解析 markdown 文本, 带目录树
 def parse_toc(text: str) -> str:
 
 # 解析 md 文件, 带目录树
 def parse_file_toc(file_name: str) -> str:
 ```
 
-第二个参数为可选项, `has_tag` 表示是否将
-
 ## 测试
 
 ```bash
 python generate.py <FILE_NAME>
 
 # python generate.py ./testfiles/test1.md
 # python generate.py README.md
```

#### html2text {}

```diff
@@ -5,17 +5,16 @@
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
 ``` æ¥å£å½æ° ```python # è§£æ markdown ææ¬è½¬ html def parse(text:
 str) -> str: # è§£æ md æä»¶è½¬ html def parse_file(file_name: str) -> str:
 # è§£æ markdown ææ¬, å¸¦ç®å½æ  def parse_toc(text: str) -> str: #
 è§£æ md æä»¶, å¸¦ç®å½æ  def parse_file_toc(file_name: str) -> str: ```
-ç¬¬äºä¸ªåæ°ä¸ºå¯éé¡¹, `has_tag` è¡¨ç¤ºæ¯å¦å° ## æµè¯ ```bash python
-generate.py  # python generate.py ./testfiles/test1.md # python generate.py
-README.md ``` è¿è¡ä¼çæindex.html,
+## æµè¯ ```bash python generate.py  # python generate.py ./testfiles/test1.md
+# python generate.py README.md ``` è¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
 20230218202400.png) ä»£ç è¦çç ```bash pip install coverage coverage run -
 m unittest coverage html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°]
 (https://www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
 MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ ```python def parse(self,
 text: str) -> str: # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines =
```

### Comparing `markdownparser-0.5.0/PKG-INFO` & `markdownparser-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,14 @@
 # 解析 markdown 文本, 带目录树
 def parse_toc(text: str) -> str:
 
 # 解析 md 文件, 带目录树
 def parse_file_toc(file_name: str) -> str:
 ```
 
-第二个参数为可选项, `has_tag` 表示是否将
-
 ## 测试
 
 ```bash
 python generate.py <FILE_NAME>
 
 # python generate.py ./testfiles/test1.md
 # python generate.py README.md
```

