# Comparing `tmp/markdownparser-0.4.3.tar.gz` & `tmp/markdownparser-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.4.3.tar", max compression
+gzip compressed data, was "markdownparser-0.5.0.tar", max compression
```

## Comparing `markdownparser-0.4.3.tar` & `markdownparser-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.4.3/LICENSE
--rw-r--r--   0        0        0       98 2023-04-28 15:33:12.004410 markdownparser-0.4.3/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5798 2023-04-28 16:45:24.751198 markdownparser-0.4.3/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    23433 2023-05-24 15:46:59.936330 markdownparser-0.4.3/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     6631 2023-05-24 15:43:29.079077 markdownparser-0.4.3/MarkdownParser/core.py
--rw-r--r--   0        0        0     3329 2023-04-28 12:24:15.406020 markdownparser-0.4.3/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21511 2023-05-24 14:55:53.230047 markdownparser-0.4.3/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-05-24 15:48:25.887452 markdownparser-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     4747 2023-05-24 15:46:28.898138 markdownparser-0.4.3/README.md
--rw-r--r--   0        0        0     5510 1970-01-01 00:00:00.000000 markdownparser-0.4.3/setup.py
--rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 markdownparser-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.0/LICENSE
+-rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.0/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5798 2023-04-28 16:45:24.751198 markdownparser-0.5.0/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    23756 2023-06-07 17:04:24.782153 markdownparser-0.5.0/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     6831 2023-06-07 17:08:57.851143 markdownparser-0.5.0/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3329 2023-04-28 12:24:15.406020 markdownparser-0.5.0/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21511 2023-05-24 14:55:53.230047 markdownparser-0.5.0/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-06-07 17:09:12.973979 markdownparser-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4799 2023-06-06 07:17:04.103864 markdownparser-0.5.0/README.md
+-rw-r--r--   0        0        0     5572 1970-01-01 00:00:00.000000 markdownparser-0.5.0/PKG-INFO
```

### Comparing `markdownparser-0.4.3/LICENSE` & `markdownparser-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.4.3/MarkdownParser/base_class.py` & `markdownparser-0.5.0/MarkdownParser/base_class.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.4.3/MarkdownParser/block_parser.py` & `markdownparser-0.5.0/MarkdownParser/block_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,16 +511,16 @@
         super().__init__(parser)
         # 匹配嵌套 + 忽略末尾多余 )
 
         # Typora               r'\[([^\[\]]*?)\]\((.*?)\)'
         # Markdown All in One  ...
         self.RE = re.compile(r"""(
             \[(.*?)\]\((.*?)\)|
-            <((?:[a-zA-z@:\.\/])+?)>|
-            https?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?
+            <(https?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?)>|
+            \bhttps?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?\b
         )""", re.VERBOSE)
 
     def subFunc(self, match: re.Match):
         word = match.group(2)
         url = match.group(3)
 
         if url is None:
@@ -741,14 +741,19 @@
 class TextBlock(Block):
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
 
+        # fix bug: 修复一些 <abc> 这种虽然不匹配网址, 但是会被 html 解析为标签的情况
+        # 见 test14.md
+        RE = re.compile(r'<([A-Za-z][^ ]*)>')
+        self.input['word'] = re.sub(RE,r'&lt\1&gt', self.input['word'])
+
         return self.input['word']
 
 
 def buildBlockParser():
     # block parser 用于逐行处理文本, 并将结果解析为一颗未优化的树
     block_parser = BlockParser()
     block_parser.register(EmptyBlockHandler(block_parser), 100)
```

### Comparing `markdownparser-0.4.3/MarkdownParser/core.py` & `markdownparser-0.5.0/MarkdownParser/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -137,45 +137,53 @@
             for cblock in block.child_blocks:
                 sub_navigator_html += self._get_header_navigator(cblock)
             navigator_html = f'<ul><li><a href=\"#{tag}\">{word}</a>{sub_navigator_html}</li></ul>'
 
         return navigator_html
 
 
-def parse(text: str) -> str:
-
+def parse(text: str, ) -> str:
+    '''
+    解析 markdown 文本转 html
+    '''
     assert type(text) == str, "输入应为字符串"
 
     # 空输入
     if not text.strip():
         return ''
 
     md = Markdown()
     return md.parse(text)
 
 
-def parseFile(file_name: str) -> str:
-
+def parse_file(file_name: str) -> str:
+    '''
+    解析 md 文件转 html
+    '''
     with open(file_name, 'r', encoding='utf-8') as f:
         text = f.read()
 
     return parse(text)
 
 
-def parse_withtag(text: str) -> str:
-
+def parse_toc(text: str) -> str:
+    '''
+    解析 markdown 文本, 带目录树
+    '''
     assert type(text) == str, "输入应为字符串"
 
     # 空输入
     if not text.strip():
         return ''
 
     md = Markdown()
     return md.parse_with_tag(text)
 
 
-def parseFile_withtag(file_name: str) -> str:
-
+def parse_file_toc(file_name: str) -> str:
+    '''
+    解析 md 文件, 带目录树
+    '''
     with open(file_name, 'r', encoding='utf-8') as f:
         text = f.read()
 
-    return parse_withtag(text)
+    return parse_toc(text)
```

### Comparing `markdownparser-0.4.3/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.0/MarkdownParser/preprocess_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.4.3/MarkdownParser/tree_parser.py` & `markdownparser-0.5.0/MarkdownParser/tree_parser.py`

 * *Files identical despite different names*

### Comparing `markdownparser-0.4.3/README.md` & `markdownparser-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,25 @@
 
 #<div class='markdown-body'><h1>Hello World!</h1></div>
 ```
 
 接口函数
 
 ```python
-# 解析markdown text
+# 解析 markdown 文本转 html
 def parse(text: str) -> str:
 
-# 解析markdown 文件
-def parseFile(file_name: str) -> str:
+# 解析 md 文件转 html
+def parse_file(file_name: str) -> str:
 
-# 见下方补充说明
-def parse_withtag(text: str) -> str:
+# 解析 markdown 文本, 带目录树
+def parse_toc(text: str) -> str:
 
-def parseFile_withtag(file_name: str) -> str:
+# 解析 md 文件, 带目录树
+def parse_file_toc(file_name: str) -> str:
 ```
 
 第二个参数为可选项, `has_tag` 表示是否将
 
 ## 测试
 
 ```bash
@@ -103,15 +104,15 @@
 
   .markdown-body  ul>li:has(input)>ul {
     list-style-type: none;
     padding-left: 8px;
   }
   ```
 
-- 您可以使用 `parse_withtag` 将 HashHeadBlock 提取出来组成目录树, 得到一个 `<div class="header-navigator">...</div>` 并添加到返回的 HTML 元素中, 您可能还需要一些 js 相关的代码实现跳转, 具体可以参考 [template.html](./template.html)
+- 您可以使用 `parse_toc` 将 HashHeadBlock 提取出来组成目录树, 得到一个 `<div class="header-navigator">...</div>` 并添加到返回的 HTML 元素中, 您可能还需要一些 js 相关的代码实现跳转, 具体可以参考 [template.html](./template.html)
 
   ```js
   let links = document.querySelectorAll('div a[href^="#"]');
     links.forEach(link => {
       link.addEventListener('click', function(event) {
         event.preventDefault();
         let target = document.querySelector(this.getAttribute('href'));
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # MarkdownParser [![codecov](https://codecov.io/gh/luzhixing12345/
 MarkdownParser/branch/main/graph/badge.svg?)](https://codecov.io/gh/
 luzhixing12345/MarkdownParser) MarkdownParser æ¯ä¸ä¸ª Markdown
 è¯­æ³è§£æå¨,ç¨äºå®ç°mdå°htmlæ ç­¾çè½¬æ¢ ## å®è£ ```bash pip
 install markdownparser ``` ## å¿«éä½¿ç¨ ```python import MarkdownParser html
 = MarkdownParser.parse('# Hello World!') print(html) #
 ****** Hello World! ******
-``` æ¥å£å½æ° ```python # è§£æmarkdown text def parse(text: str) -> str: #
-è§£æmarkdown æä»¶ def parseFile(file_name: str) -> str: #
-è§ä¸æ¹è¡¥åè¯´æ def parse_withtag(text: str) -> str: def
-parseFile_withtag(file_name: str) -> str: ``` ç¬¬äºä¸ªåæ°ä¸ºå¯éé¡¹,
-`has_tag` è¡¨ç¤ºæ¯å¦å° ## æµè¯ ```bash python generate.py  # python
-generate.py ./testfiles/test1.md # python generate.py README.md ```
-è¿è¡ä¼çæindex.html,
+``` æ¥å£å½æ° ```python # è§£æ markdown ææ¬è½¬ html def parse(text:
+str) -> str: # è§£æ md æä»¶è½¬ html def parse_file(file_name: str) -> str:
+# è§£æ markdown ææ¬, å¸¦ç®å½æ  def parse_toc(text: str) -> str: #
+è§£æ md æä»¶, å¸¦ç®å½æ  def parse_file_toc(file_name: str) -> str: ```
+ç¬¬äºä¸ªåæ°ä¸ºå¯éé¡¹, `has_tag` è¡¨ç¤ºæ¯å¦å° ## æµè¯ ```bash python
+generate.py  # python generate.py ./testfiles/test1.md # python generate.py
+README.md ``` è¿è¡ä¼çæindex.html,
 ä½¿ç¨æµè§å¨æå¼çæçindex.htmlå³å¯ä¸æ¨çMarkdownç¼è¾å¨çé¢ææ¸²æç»æå¯¹æ¯
 ![20230218202400](https://raw.githubusercontent.com/learner-lu/picbed/master/
 20230218202400.png) ä»£ç è¦çç ```bash pip install coverage coverage run -
 m unittest coverage html ``` ## å®ç°æè·¯ [Markdownè§£æå¨çä»£ç å®ç°]
 (https://www.bilibili.com/video/BV1LA411X7X3) æ¨å¯éè¿åæ¶ [core.py](./
 MarkdownParser/core.py) æ³¨éæ¥è·åæ çç»æ ```python def parse(self,
 text: str) -> str: # å»é¤ç©ºè¡/æ³¨é/htmlæ ç­¾ lines =
@@ -28,15 +28,15 @@
 çæçç»æå¦ä¸ `
 markdownåå®¹
 ` - ä»£ç æ®µä¼æ ¹æ®è¯­è¨å å¥ä¸ä¸ªç±»åä¾¿äºåæé«äº®,ä¾å¦
 `class="language-cpp"`, æªå®ä¹è¯­è¨åä¸º `language-UNKNOWN` -
 é»è®¤å¯¼åºçHTMLä¸­å±çº§ä»»å¡åè¡¨ä¼ææ¾ç¤ºé®é¢,è¿æ¯å ä¸ºä½¿ç¨äºul+li+checkboxçæ¹å¼,æ¨éè¦æ·»å ä»¥ä¸cssæ ·å¼ä¿®æ­£
 ```css .markdown-body > ul>li:has(input) { padding-left: 0; margin-bottom: 0; }
 .markdown-body ul>li:has(input)>ul { list-style-type: none; padding-left: 8px;
-} ``` - æ¨å¯ä»¥ä½¿ç¨ `parse_withtag` å° HashHeadBlock
+} ``` - æ¨å¯ä»¥ä½¿ç¨ `parse_toc` å° HashHeadBlock
 æååºæ¥ç»æç®å½æ , å¾å°ä¸ä¸ª `
 ...
 ` å¹¶æ·»å å°è¿åç HTML åç´ ä¸­, æ¨å¯è½è¿éè¦ä¸äº js
 ç¸å³çä»£ç å®ç°è·³è½¬, å·ä½å¯ä»¥åè [template.html](./
 template.html) ```js let links = document.querySelectorAll('div a[href^="#"]');
 links.forEach(link => { link.addEventListener('click', function(event)
 { event.preventDefault(); let target = document.querySelector(this.getAttribute
```

### Comparing `markdownparser-0.4.3/setup.py` & `markdownparser-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,345 +1,349 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 276d 6172 6b64 6f77 6e70 6172   \.['markdownpar
-00000050: 7365 7227 5d0a 0a70 6163 6b61 6765 5f64  ser']..package_d
-00000060: 6174 6120 3d20 5c0a 7b27 273a 205b 272a  ata = \.{'': ['*
-00000070: 275d 7d0a 0a73 6574 7570 5f6b 7761 7267  ']}..setup_kwarg
-00000080: 7320 3d20 7b0a 2020 2020 276e 616d 6527  s = {.    'name'
-00000090: 3a20 276d 6172 6b64 6f77 6e70 6172 7365  : 'markdownparse
-000000a0: 7227 2c0a 2020 2020 2776 6572 7369 6f6e  r',.    'version
-000000b0: 273a 2027 302e 342e 3327 2c0a 2020 2020  ': '0.4.3',.    
-000000c0: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
-000000d0: 272c 0a20 2020 2027 6c6f 6e67 5f64 6573  ',.    'long_des
-000000e0: 6372 6970 7469 6f6e 273a 2027 2320 4d61  cription': '# Ma
-000000f0: 726b 646f 776e 5061 7273 6572 5c6e 5c6e  rkdownParser\n\n
-00000100: 5b21 5b63 6f64 6563 6f76 5d28 6874 7470  [![codecov](http
-00000110: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-00000120: 682f 6c75 7a68 6978 696e 6731 3233 3435  h/luzhixing12345
-00000130: 2f4d 6172 6b64 6f77 6e50 6172 7365 722f  /MarkdownParser/
-00000140: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
-00000150: 682f 6261 6467 652e 7376 673f 295d 2868  h/badge.svg?)](h
-00000160: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-00000170: 6f2f 6768 2f6c 757a 6869 7869 6e67 3132  o/gh/luzhixing12
-00000180: 3334 352f 4d61 726b 646f 776e 5061 7273  345/MarkdownPars
-00000190: 6572 295c 6e5c 6e4d 6172 6b64 6f77 6e50  er)\n\nMarkdownP
-000001a0: 6172 7365 7220 e698 afe4 b880 e4b8 aa20  arser ......... 
-000001b0: 4d61 726b 646f 776e 20e8 afad e6b3 95e8  Markdown .......
-000001c0: a7a3 e69e 90e5 99a8 2ce7 94a8 e4ba 8ee5  ........,.......
-000001d0: ae9e e78e b06d 64e5 88b0 6874 6d6c e6a0  .....md...html..
-000001e0: 87e7 adbe e79a 84e8 bdac e68d a25c 6e5c  .............\n\
-000001f0: 6e23 2320 e5ae 89e8 a385 5c6e 5c6e 6060  n## ......\n\n``
-00000200: 6062 6173 685c 6e70 6970 2069 6e73 7461  `bash\npip insta
-00000210: 6c6c 206d 6172 6b64 6f77 6e70 6172 7365  ll markdownparse
-00000220: 725c 6e60 6060 5c6e 5c6e 2323 20e5 bfab  r\n```\n\n## ...
-00000230: e980 9fe4 bdbf e794 a85c 6e5c 6e60 6060  .........\n\n```
-00000240: 7079 7468 6f6e 5c6e 696d 706f 7274 204d  python\nimport M
-00000250: 6172 6b64 6f77 6e50 6172 7365 725c 6e5c  arkdownParser\n\
-00000260: 6e68 746d 6c20 3d20 4d61 726b 646f 776e  nhtml = Markdown
-00000270: 5061 7273 6572 2e70 6172 7365 285c 2723  Parser.parse(\'#
-00000280: 2048 656c 6c6f 2057 6f72 6c64 215c 2729   Hello World!\')
-00000290: 5c6e 7072 696e 7428 6874 6d6c 295c 6e5c  \nprint(html)\n\
-000002a0: 6e23 3c64 6976 2063 6c61 7373 3d5c 276d  n#<div class=\'m
-000002b0: 6172 6b64 6f77 6e2d 626f 6479 5c27 3e3c  arkdown-body\'><
-000002c0: 6831 3e48 656c 6c6f 2057 6f72 6c64 213c  h1>Hello World!<
-000002d0: 2f68 313e 3c2f 6469 763e 5c6e 6060 605c  /h1></div>\n```\
-000002e0: 6e5c 6ee6 8ea5 e58f a3e5 87bd e695 b05c  n\n............\
-000002f0: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 2320  n\n```python\n# 
-00000300: e8a7 a3e6 9e90 6d61 726b 646f 776e 2074  ......markdown t
-00000310: 6578 745c 6e64 6566 2070 6172 7365 2874  ext\ndef parse(t
-00000320: 6578 743a 2073 7472 2920 2d3e 2073 7472  ext: str) -> str
-00000330: 3a5c 6e5c 6e23 20e8 a7a3 e69e 906d 6172  :\n\n# ......mar
-00000340: 6b64 6f77 6e20 e696 87e4 bbb6 5c6e 6465  kdown ......\nde
-00000350: 6620 7061 7273 6546 696c 6528 6669 6c65  f parseFile(file
-00000360: 5f6e 616d 653a 2073 7472 2920 2d3e 2073  _name: str) -> s
-00000370: 7472 3a5c 6e5c 6e23 20e8 a781 e4b8 8be6  tr:\n\n# .......
-00000380: 96b9 e8a1 a5e5 8585 e8af b4e6 988e 5c6e  ..............\n
-00000390: 6465 6620 7061 7273 655f 7769 7468 7461  def parse_withta
-000003a0: 6728 7465 7874 3a20 7374 7229 202d 3e20  g(text: str) -> 
-000003b0: 7374 723a 5c6e 5c6e 6465 6620 7061 7273  str:\n\ndef pars
-000003c0: 6546 696c 655f 7769 7468 7461 6728 6669  eFile_withtag(fi
-000003d0: 6c65 5f6e 616d 653a 2073 7472 2920 2d3e  le_name: str) ->
-000003e0: 2073 7472 3a5c 6e60 6060 5c6e 5c6e e7ac   str:\n```\n\n..
-000003f0: ace4 ba8c e4b8 aae5 8f82 e695 b0e4 b8ba  ................
-00000400: e58f afe9 8089 e9a1 b92c 2060 6861 735f  ........., `has_
-00000410: 7461 6760 20e8 a1a8 e7a4 bae6 98af e590  tag` ...........
-00000420: a6e5 b086 5c6e 5c6e 2323 20e6 b58b e8af  ....\n\n## .....
-00000430: 955c 6e5c 6e60 6060 6261 7368 5c6e 7079  .\n\n```bash\npy
-00000440: 7468 6f6e 2067 656e 6572 6174 652e 7079  thon generate.py
-00000450: 203c 4649 4c45 5f4e 414d 453e 5c6e 5c6e   <FILE_NAME>\n\n
-00000460: 2320 7079 7468 6f6e 2067 656e 6572 6174  # python generat
-00000470: 652e 7079 202e 2f74 6573 7466 696c 6573  e.py ./testfiles
-00000480: 2f74 6573 7431 2e6d 645c 6e23 2070 7974  /test1.md\n# pyt
-00000490: 686f 6e20 6765 6e65 7261 7465 2e70 7920  hon generate.py 
-000004a0: 5245 4144 4d45 2e6d 645c 6e60 6060 5c6e  README.md\n```\n
-000004b0: 5c6e e8bf 90e8 a18c e4bc 9ae7 949f e688  \n..............
-000004c0: 9069 6e64 6578 2e68 746d 6c2c 20e4 bdbf  .index.html, ...
-000004d0: e794 a8e6 b58f e8a7 88e5 99a8 e689 93e5  ................
-000004e0: bc80 e794 9fe6 8890 e79a 8469 6e64 6578  ...........index
-000004f0: 2e68 746d 6ce5 8db3 e58f afe4 b88e e682  .html...........
-00000500: a8e7 9a84 4d61 726b 646f 776e e7bc 96e8  ....Markdown....
-00000510: be91 e599 a8e7 9a84 e9a2 84e6 9c9f e6b8  ................
-00000520: b2e6 9f93 e7bb 93e6 9e9c e5af b9e6 af94  ................
-00000530: 5c6e 5c6e 215b 3230 3233 3032 3138 3230  \n\n![2023021820
-00000540: 3234 3030 5d28 6874 7470 733a 2f2f 7261  2400](https://ra
-00000550: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000560: 656e 742e 636f 6d2f 6c65 6172 6e65 722d  ent.com/learner-
-00000570: 6c75 2f70 6963 6265 642f 6d61 7374 6572  lu/picbed/master
-00000580: 2f32 3032 3330 3231 3832 3032 3430 302e  /20230218202400.
-00000590: 706e 6729 5c6e 5c6e e4bb a3e7 a081 e8a6  png)\n\n........
-000005a0: 86e7 9b96 e78e 875c 6e5c 6e60 6060 6261  .......\n\n```ba
-000005b0: 7368 5c6e 7069 7020 696e 7374 616c 6c20  sh\npip install 
-000005c0: 636f 7665 7261 6765 5c6e 5c6e 636f 7665  coverage\n\ncove
-000005d0: 7261 6765 2072 756e 202d 6d20 756e 6974  rage run -m unit
-000005e0: 7465 7374 5c6e 636f 7665 7261 6765 2068  test\ncoverage h
-000005f0: 746d 6c5c 6e60 6060 5c6e 5c6e 2323 20e5  tml\n```\n\n## .
-00000600: ae9e e78e b0e6 809d e8b7 af5c 6e5c 6e5b  ...........\n\n[
-00000610: 4d61 726b 646f 776e e8a7 a3e6 9e90 e599  Markdown........
-00000620: a8e7 9a84 e4bb a3e7 a081 e5ae 9ee7 8eb0  ................
-00000630: 5d28 6874 7470 733a 2f2f 7777 772e 6269  ](https://www.bi
-00000640: 6c69 6269 6c69 2e63 6f6d 2f76 6964 656f  libili.com/video
-00000650: 2f42 5631 4c41 3431 3158 3758 3329 5c6e  /BV1LA411X7X3)\n
-00000660: 5c6e e682 a8e5 8faf e980 9ae8 bf87 e58f  \n..............
-00000670: 96e6 b688 205b 636f 7265 2e70 795d 282e  .... [core.py](.
-00000680: 2f4d 6172 6b64 6f77 6e50 6172 7365 722f  /MarkdownParser/
-00000690: 636f 7265 2e70 7929 20e6 b3a8 e987 8ae6  core.py) .......
-000006a0: 9da5 e88e b7e5 8f96 e6a0 91e7 9a84 e7bb  ................
-000006b0: 93e6 9e84 5c6e 5c6e 6060 6070 7974 686f  ....\n\n```pytho
-000006c0: 6e5c 6e64 6566 2070 6172 7365 2873 656c  n\ndef parse(sel
-000006d0: 662c 2074 6578 743a 2073 7472 2920 2d3e  f, text: str) ->
-000006e0: 2073 7472 3a5c 6e5c 6e20 2020 2023 20e5   str:\n\n    # .
-000006f0: 8ebb e999 a4e7 a9ba e8a1 8c2f e6b3 a8e9  .........../....
-00000700: 878a 2f68 746d 6ce6 a087 e7ad be5c 6e20  ../html......\n 
-00000710: 2020 206c 696e 6573 203d 2073 656c 662e     lines = self.
-00000720: 7072 6570 726f 6365 7373 5f70 6172 7365  preprocess_parse
-00000730: 7228 7465 7874 295c 6e20 2020 2023 2070  r(text)\n    # p
-00000740: 7269 6e74 286c 696e 6573 295c 6e20 2020  rint(lines)\n   
-00000750: 2023 20e9 8090 e8a1 8ce8 a7a3 e69e 902c   # ............,
-00000760: e5be 97e5 88b0 e4b8 80e9 a297 e69c aae4  ................
-00000770: bc98 e58c 96e7 9a84 e6a0 915c 6e20 2020  ...........\n   
-00000780: 2072 6f6f 7420 3d20 7365 6c66 2e62 6c6f   root = self.blo
-00000790: 636b 5f70 6172 7365 7228 6c69 6e65 7329  ck_parser(lines)
-000007a0: 5c6e 2020 2020 2320 726f 6f74 2e69 6e66  \n    # root.inf
-000007b0: 6f28 295c 6e20 2020 2023 20e4 bc98 e58c  o()\n    # .....
-000007c0: 962c e5be 97e5 88b0 e6ad a3e7 a1ae e79a  .,..............
-000007d0: 846d 6172 6b64 6f77 6ee8 a7a3 e69e 90e6  .markdown.......
-000007e0: a091 5c6e 2020 2020 7472 6565 203d 2073  ..\n    tree = s
-000007f0: 656c 662e 7472 6565 5f70 6172 7365 7228  elf.tree_parser(
-00000800: 726f 6f74 295c 6e20 2020 2023 2074 7265  root)\n    # tre
-00000810: 652e 696e 666f 2829 5c6e 2020 2020 2320  e.info()\n    # 
-00000820: e8be 93e5 87ba e588 b0e5 b18f e5b9 9520  ............... 
-00000830: 2f20 e5af bce5 87ba 6874 6d6c e696 87e4  / ......html....
-00000840: bbb6 5c6e 2020 2020 7265 7475 726e 2074  ..\n    return t
-00000850: 7265 652e 746f 4854 4d4c 2829 5c6e 6060  ree.toHTML()\n``
-00000860: 605c 6e5c 6e23 2320 e4b8 8de6 94af e68c  `\n\n## ........
-00000870: 815c 6e5c 6e2d 20e5 9b9b e4b8 aae7 a9ba  .\n\n- .........
-00000880: e6a0 bce5 8f98 e4b8 bae4 bba3 e7a0 81e6  ................
-00000890: aeb5 5c6e 2d20 5b5e 315d e79a 84e5 bc95  ..\n- [^1]......
-000008a0: e794 a8e6 96b9 e5bc 8f5c 6e2d 2053 6574  .........\n- Set
-000008b0: 6578 7420 e5bd a2e5 bc8f e79a 84e6 a087  ext ............
-000008c0: e9a2 985c 6e2d 20e4 b88a e6a0 8720 2f20  ...\n- ...... / 
-000008d0: e4b8 8be6 a087 202f 20e4 b88b e588 92e7  ...... / .......
-000008e0: babf 5c6e 5c6e 2323 20e8 a1a5 e585 85e8  ..\n\n## .......
-000008f0: afb4 e698 8e5c 6e5c 6e2d 20e7 949f e688  .....\n\n- .....
-00000900: 90e7 9a84 e7bb 93e6 9e9c e5a6 82e4 b88b  ................
-00000910: 2060 3c64 6976 2063 6c61 7373 3d5c 276d   `<div class=\'m
-00000920: 6172 6b64 6f77 6e2d 626f 6479 5c27 3e6d  arkdown-body\'>m
-00000930: 6172 6b64 6f77 6ee5 8685 e5ae b93c 2f64  arkdown......</d
-00000940: 6976 3e60 5c6e 2d20 e4bb a3e7 a081 e6ae  iv>`\n- ........
-00000950: b5e4 bc9a e6a0 b9e6 8dae e8af ade8 a880  ................
-00000960: e58a a0e5 85a5 e4b8 80e4 b8aa e7b1 bbe5  ................
-00000970: 908d e4be bfe4 ba8e e590 8ee6 9c9f e9ab  ................
-00000980: 98e4 baae 2ce4 be8b e5a6 8220 6063 6c61  ....,...... `cla
-00000990: 7373 3d22 6c61 6e67 7561 6765 2d63 7070  ss="language-cpp
-000009a0: 2260 2c20 e69c aae5 ae9a e4b9 89e8 afad  "`, ............
-000009b0: e8a8 80e5 8899 e4b8 ba20 606c 616e 6775  ......... `langu
-000009c0: 6167 652d 554e 4b4e 4f57 4e60 5c6e 2d20  age-UNKNOWN`\n- 
-000009d0: e9bb 98e8 aea4 e5af bce5 87ba e79a 8448  ...............H
-000009e0: 544d 4ce4 b8ad e5b1 82e7 baa7 e4bb bbe5  TML.............
-000009f0: 8aa1 e588 97e8 a1a8 e4bc 9ae6 9c89 e698  ................
-00000a00: bee7 a4ba e997 aee9 a298 2ce8 bf99 e698  ..........,.....
-00000a10: afe5 9ba0 e4b8 bae4 bdbf e794 a8e4 ba86  ................
-00000a20: 756c 2b6c 692b 6368 6563 6b62 6f78 e79a  ul+li+checkbox..
-00000a30: 84e6 96b9 e5bc 8f2c e682 a8e9 9c80 e8a6  .......,........
-00000a40: 81e6 b7bb e58a a0e4 bba5 e4b8 8b63 7373  .............css
-00000a50: e6a0 b7e5 bc8f e4bf aee6 ada3 5c6e 5c6e  ............\n\n
-00000a60: 2020 6060 6063 7373 5c6e 2020 2e6d 6172    ```css\n  .mar
-00000a70: 6b64 6f77 6e2d 626f 6479 203e 2075 6c3e  kdown-body > ul>
-00000a80: 6c69 3a68 6173 2869 6e70 7574 2920 7b5c  li:has(input) {\
-00000a90: 6e20 2020 2070 6164 6469 6e67 2d6c 6566  n    padding-lef
-00000aa0: 743a 2030 3b5c 6e20 2020 206d 6172 6769  t: 0;\n    margi
-00000ab0: 6e2d 626f 7474 6f6d 3a20 303b 5c6e 2020  n-bottom: 0;\n  
-00000ac0: 7d5c 6e5c 6e20 202e 6d61 726b 646f 776e  }\n\n  .markdown
-00000ad0: 2d62 6f64 7920 2075 6c3e 6c69 3a68 6173  -body  ul>li:has
-00000ae0: 2869 6e70 7574 293e 756c 207b 5c6e 2020  (input)>ul {\n  
-00000af0: 2020 6c69 7374 2d73 7479 6c65 2d74 7970    list-style-typ
-00000b00: 653a 206e 6f6e 653b 5c6e 2020 2020 7061  e: none;\n    pa
-00000b10: 6464 696e 672d 6c65 6674 3a20 3870 783b  dding-left: 8px;
-00000b20: 5c6e 2020 7d5c 6e20 2060 6060 5c6e 5c6e  \n  }\n  ```\n\n
-00000b30: 2d20 e682 a8e5 8faf e4bb a5e4 bdbf e794  - ..............
-00000b40: a820 6070 6172 7365 5f77 6974 6874 6167  . `parse_withtag
-00000b50: 6020 e5b0 8620 4861 7368 4865 6164 426c  ` ... HashHeadBl
-00000b60: 6f63 6b20 e68f 90e5 8f96 e587 bae6 9da5  ock ............
-00000b70: e7bb 84e6 8890 e79b aee5 bd95 e6a0 912c  ...............,
-00000b80: 20e5 be97 e588 b0e4 b880 e4b8 aa20 603c   ............ `<
-00000b90: 6469 7620 636c 6173 733d 2268 6561 6465  div class="heade
-00000ba0: 722d 6e61 7669 6761 746f 7222 3e2e 2e2e  r-navigator">...
-00000bb0: 3c2f 6469 763e 6020 e5b9 b6e6 b7bb e58a  </div>` ........
-00000bc0: a0e5 88b0 e8bf 94e5 9b9e e79a 8420 4854  ............. HT
-00000bd0: 4d4c 20e5 8583 e7b4 a0e4 b8ad 2c20 e682  ML ........., ..
-00000be0: a8e5 8faf e883 bde8 bf98 e99c 80e8 a681  ................
-00000bf0: e4b8 80e4 ba9b 206a 7320 e79b b8e5 85b3  ...... js ......
-00000c00: e79a 84e4 bba3 e7a0 81e5 ae9e e78e b0e8  ................
-00000c10: b7b3 e8bd ac2c 20e5 85b7 e4bd 93e5 8faf  ....., .........
-00000c20: e4bb a5e5 8f82 e880 8320 5b74 656d 706c  ......... [templ
-00000c30: 6174 652e 6874 6d6c 5d28 2e2f 7465 6d70  ate.html](./temp
-00000c40: 6c61 7465 2e68 746d 6c29 5c6e 5c6e 2020  late.html)\n\n  
-00000c50: 6060 606a 735c 6e20 206c 6574 206c 696e  ```js\n  let lin
-00000c60: 6b73 203d 2064 6f63 756d 656e 742e 7175  ks = document.qu
-00000c70: 6572 7953 656c 6563 746f 7241 6c6c 285c  erySelectorAll(\
-00000c80: 2764 6976 2061 5b68 7265 665e 3d22 2322  'div a[href^="#"
-00000c90: 5d5c 2729 3b5c 6e20 2020 206c 696e 6b73  ]\');\n    links
-00000ca0: 2e66 6f72 4561 6368 286c 696e 6b20 3d3e  .forEach(link =>
-00000cb0: 207b 5c6e 2020 2020 2020 6c69 6e6b 2e61   {\n      link.a
-00000cc0: 6464 4576 656e 744c 6973 7465 6e65 7228  ddEventListener(
-00000cd0: 5c27 636c 6963 6b5c 272c 2066 756e 6374  \'click\', funct
-00000ce0: 696f 6e28 6576 656e 7429 207b 5c6e 2020  ion(event) {\n  
-00000cf0: 2020 2020 2020 6576 656e 742e 7072 6576        event.prev
-00000d00: 656e 7444 6566 6175 6c74 2829 3b5c 6e20  entDefault();\n 
-00000d10: 2020 2020 2020 206c 6574 2074 6172 6765         let targe
-00000d20: 7420 3d20 646f 6375 6d65 6e74 2e71 7565  t = document.que
-00000d30: 7279 5365 6c65 6374 6f72 2874 6869 732e  rySelector(this.
-00000d40: 6765 7441 7474 7269 6275 7465 285c 2768  getAttribute(\'h
-00000d50: 7265 665c 2729 293b 5c6e 2020 2020 2020  ref\'));\n      
-00000d60: 2020 7461 7267 6574 2e73 6372 6f6c 6c49    target.scrollI
-00000d70: 6e74 6f56 6965 7728 7b20 6265 6861 7669  ntoView({ behavi
-00000d80: 6f72 3a20 5c27 736d 6f6f 7468 5c27 207d  or: \'smooth\' }
-00000d90: 293b 5c6e 2020 2020 2020 7d29 3b5c 6e20  );\n      });\n 
-00000da0: 2020 207d 293b 5c6e 2020 6060 605c 6e5c     });\n  ```\n\
-00000db0: 6e20 20e4 bba5 e58f 8ae4 b880 e4ba 9be6  n  .............
-00000dc0: a0b7 e5bc 8fe7 be8e e58c 965c 6e5c 6e20  ...........\n\n 
-00000dd0: 2060 6060 6373 735c 6e20 202e 6865 6164   ```css\n  .head
-00000de0: 6572 2d6e 6176 6967 6174 6f72 207b 5c6e  er-navigator {\n
-00000df0: 2020 2020 706f 7369 7469 6f6e 3a20 6669      position: fi
-00000e00: 7865 643b 5c6e 2020 7d5c 6e20 2060 6060  xed;\n  }\n  ```
-00000e10: 5c6e 5c6e 2d20 e5a6 82e6 9e9c e682 a8e6  \n\n- ..........
-00000e20: 83b3 e6b7 bbe5 8aa0 e5af b95b 4d65 726d  ...........[Merm
-00000e30: 6169 645d 2868 7474 7073 3a2f 2f6d 6572  aid](https://mer
-00000e40: 6d61 6964 2e6a 732e 6f72 672f 29e7 9a84  maid.js.org/)...
-00000e50: e694 afe6 8c81 2c20 e682 a8e5 8faf e58f  ......, ........
-00000e60: 82e8 8083 5b6d 6572 6d61 6964 2070 6c75  ....[mermaid plu
-00000e70: 6769 6e5d 2868 7474 7073 3a2f 2f6d 6572  gin](https://mer
-00000e80: 6d61 6964 2e6a 732e 6f72 672f 696e 7472  maid.js.org/intr
-00000e90: 6f2f 6e30 3062 2d67 6574 7469 6e67 5374  o/n00b-gettingSt
-00000ea0: 6172 7465 642e 6874 6d6c 235f 322d 7573  arted.html#_2-us
-00000eb0: 696e 672d 6d65 726d 6169 642d 706c 7567  ing-mermaid-plug
-00000ec0: 696e 7329 e59c a8e6 82a8 e79a 8468 746d  ins).........htm
-00000ed0: 6ce9 a1b5 e99d a220 603c 626f 6479 3e60  l...... `<body>`
-00000ee0: 20e6 9cab e5b0 bee6 b7bb e58a a0e5 a682   ...............
-00000ef0: e4b8 8b20 603c 7363 7269 7074 3e60 5c6e  ... `<script>`\n
-00000f00: 5c6e 2020 6060 6068 746d 6c5c 6e20 203c  \n  ```html\n  <
-00000f10: 7363 7269 7074 2074 7970 653d 226d 6f64  script type="mod
-00000f20: 756c 6522 3e5c 6e20 2020 2063 6f6e 7374  ule">\n    const
-00000f30: 2063 6f64 6542 6c6f 636b 7320 3d20 646f   codeBlocks = do
-00000f40: 6375 6d65 6e74 2e71 7565 7279 5365 6c65  cument.querySele
-00000f50: 6374 6f72 416c 6c28 5c27 2e6c 616e 6775  ctorAll(\'.langu
-00000f60: 6167 652d 6d65 726d 6169 645c 2729 3b5c  age-mermaid\');\
-00000f70: 6e20 2020 2063 6f64 6542 6c6f 636b 732e  n    codeBlocks.
-00000f80: 666f 7245 6163 6828 636f 6465 426c 6f63  forEach(codeBloc
-00000f90: 6b20 3d3e 207b 5c6e 2020 2020 2020 2020  k => {\n        
-00000fa0: 636f 6465 426c 6f63 6b2e 636c 6173 734c  codeBlock.classL
-00000fb0: 6973 742e 7265 6d6f 7665 285c 276c 616e  ist.remove(\'lan
-00000fc0: 6775 6167 652d 6d65 726d 6169 645c 2729  guage-mermaid\')
-00000fd0: 3b5c 6e20 2020 2020 2020 2063 6f64 6542  ;\n        codeB
-00000fe0: 6c6f 636b 2e63 6c61 7373 4c69 7374 2e61  lock.classList.a
-00000ff0: 6464 285c 276d 6572 6d61 6964 5c27 293b  dd(\'mermaid\');
-00001000: 5c6e 2020 2020 7d29 3b5c 6e20 2020 2069  \n    });\n    i
-00001010: 6d70 6f72 7420 6d65 726d 6169 6420 6672  mport mermaid fr
-00001020: 6f6d 205c 2768 7474 7073 3a2f 2f63 646e  om \'https://cdn
-00001030: 2e6a 7364 656c 6976 722e 6e65 742f 6e70  .jsdelivr.net/np
-00001040: 6d2f 6d65 726d 6169 6440 3130 2f64 6973  m/mermaid@10/dis
-00001050: 742f 6d65 726d 6169 642e 6573 6d2e 6d69  t/mermaid.esm.mi
-00001060: 6e2e 6d6a 735c 273b 5c6e 2020 2020 6d65  n.mjs\';\n    me
-00001070: 726d 6169 642e 696e 6974 6961 6c69 7a65  rmaid.initialize
-00001080: 287b 2073 7461 7274 4f6e 4c6f 6164 3a20  ({ startOnLoad: 
-00001090: 7472 7565 207d 293b 5c6e 2020 3c2f 7363  true });\n  </sc
-000010a0: 7269 7074 3e5c 6e20 2060 6060 5c6e 5c6e  ript>\n  ```\n\n
-000010b0: 2020 3e20 2a2a e8af b7e6 b3a8 e684 8f2a    > **.........*
-000010c0: 2a2c 20e7 94b1 e4ba 8ee6 9cac 4d61 726b  *, .........Mark
-000010d0: 646f 776e e8a7 a3e6 9e90 e599 a8e7 9a84  down............
-000010e0: 436f 6465 426c 6f63 6be8 a7a3 e69e 90e5  CodeBlock.......
-000010f0: be97 e588 b0e7 9a84 e7b1 bbe5 908d e4b8  ................
-00001100: ba20 606c 616e 6775 6167 652d 6d65 726d  . `language-merm
-00001110: 6169 6460 2c20 e880 8c6d 6572 6d61 6964  aid`, ...mermaid
-00001120: e68f 92e4 bbb6 e694 afe6 8c81 e79a 84e7  ................
-00001130: b1bb e590 8de6 a0bc e5bc 8fe4 b8ba 606d  ..............`m
-00001140: 6572 6d61 6964 602c 20e6 8980 e4bb a5e4  ermaid`, .......
-00001150: bba3 e7a0 81e4 b8ad e689 8be5 8aa8 e4bf  ................
-00001160: aee6 94b9 e4ba 8620 606c 616e 6775 6167  ....... `languag
-00001170: 652d 6d65 726d 6169 6460 20e7 9a84 e7b1  e-mermaid` .....
-00001180: bbe5 908d 5c6e 5c6e 2d20 e5a6 82e6 9e9c  ....\n\n- ......
-00001190: e682 a8e6 83b3 e6b7 bbe5 8aa0 e5af b94c  ...............L
-000011a0: 6174 6578 e695 b0e5 ada6 e585 ace5 bc8f  atex............
-000011b0: e79a 84e6 94af e68c 812c 20e5 8faf e4bb  ........., .....
-000011c0: a5e5 9ca8 6874 6d6c e9a1 b5e9 9da2 2060  ....html...... `
-000011d0: 3c62 6f64 793e 6020 e69c abe5 b0be e6b7  <body>` ........
-000011e0: bbe5 8aa0 e5a6 82e4 b88b 2060 3c73 6372  .......... `<scr
-000011f0: 6970 743e 605c 6e5c 6e20 2060 6060 6874  ipt>`\n\n  ```ht
-00001200: 6d6c 5c6e 2020 3c73 6372 6970 743e 5c6e  ml\n  <script>\n
-00001210: 2020 2020 2020 4d61 7468 4a61 7820 3d20        MathJax = 
-00001220: 7b5c 6e20 2020 2020 2020 2074 6578 3a20  {\n        tex: 
-00001230: 7b5c 6e20 2020 2020 2020 2020 2069 6e6c  {\n          inl
-00001240: 696e 654d 6174 683a 205b 5b5c 2724 5c27  ineMath: [[\'$\'
-00001250: 2c20 5c27 245c 275d 2c20 5b5c 275c 5c5c  , \'$\'], [\'\\\
-00001260: 5c28 5c27 2c20 5c27 5c5c 5c5c 295c 275d  \(\', \'\\\\)\']
-00001270: 5d5c 6e20 2020 2020 2020 207d 5c6e 2020  ]\n        }\n  
-00001280: 2020 2020 7d3b 5c6e 2020 2020 2020 3c2f      };\n      </
-00001290: 7363 7269 7074 3e5c 6e20 203c 7363 7269  script>\n  <scri
-000012a0: 7074 2069 643d 224d 6174 684a 6178 2d73  pt id="MathJax-s
-000012b0: 6372 6970 7422 2061 7379 6e63 5c6e 2020  cript" async\n  
-000012c0: 7372 633d 2268 7474 7073 3a2f 2f63 646e  src="https://cdn
-000012d0: 2e6a 7364 656c 6976 722e 6e65 742f 6e70  .jsdelivr.net/np
-000012e0: 6d2f 6d61 7468 6a61 7840 332f 6573 352f  m/mathjax@3/es5/
-000012f0: 7465 782d 6368 746d 6c2e 6a73 223e 5c6e  tex-chtml.js">\n
-00001300: 2020 3c2f 7363 7269 7074 3e5c 6e20 2060    </script>\n  `
-00001310: 6060 5c6e 5c6e 2020 e6b3 a8e6 848f 2ce8  ``\n\n  ......,.
-00001320: bf99 e987 8ce4 bb85 e694 afe6 8c81 e5be  ................
-00001330: 88e5 b091 e4b8 80e9 83a8 e588 86e6 95b0  ................
-00001340: e5ad a6e5 85ac e5bc 8f5c 6e5c 6e5c 6e23  .........\n\n\n#
-00001350: 2320 e79b b8e5 85b3 e58f 82e8 8083 5c6e  # ............\n
-00001360: 5c6e 2d20 5b47 6974 6875 6220 4d61 726b  \n- [Github Mark
-00001370: 646f 776e 2043 5353 5d28 6874 7470 733a  down CSS](https:
-00001380: 2f2f 6364 6e2e 6a73 6465 6c69 7672 2e6e  //cdn.jsdelivr.n
-00001390: 6574 2f6e 706d 2f67 6974 6875 622d 6d61  et/npm/github-ma
-000013a0: 726b 646f 776e 2d63 7373 4034 2e30 2e30  rkdown-css@4.0.0
-000013b0: 2f67 6974 6875 622d 6d61 726b 646f 776e  /github-markdown
-000013c0: 2e63 7373 295c 6e2d 205b 4d65 726d 6169  .css)\n- [Mermai
-000013d0: 6420 4150 495d 2868 7474 7073 3a2f 2f6d  d API](https://m
-000013e0: 6572 6d61 6964 2e6a 732e 6f72 672f 696e  ermaid.js.org/in
-000013f0: 7472 6f2f 236d 6572 6d61 6964 2d61 7069  tro/#mermaid-api
-00001400: 295c 6e2d 205b 4d61 7468 4a61 785d 2868  )\n- [MathJax](h
-00001410: 7474 7073 3a2f 2f64 6f63 732e 6d61 7468  ttps://docs.math
-00001420: 6a61 782e 6f72 672f 656e 2f6c 6174 6573  jax.org/en/lates
-00001430: 742f 7765 622f 7374 6172 742e 6874 6d6c  t/web/start.html
-00001440: 2927 2c0a 2020 2020 2761 7574 686f 7227  )',.    'author'
-00001450: 3a20 276c 757a 6869 7869 6e67 3132 3334  : 'luzhixing1234
-00001460: 3527 2c0a 2020 2020 2761 7574 686f 725f  5',.    'author_
-00001470: 656d 6169 6c27 3a20 276c 757a 6869 7869  email': 'luzhixi
-00001480: 6e67 3132 3334 3540 3136 332e 636f 6d27  ng12345@163.com'
-00001490: 2c0a 2020 2020 276d 6169 6e74 6169 6e65  ,.    'maintaine
-000014a0: 7227 3a20 274e 6f6e 6527 2c0a 2020 2020  r': 'None',.    
-000014b0: 276d 6169 6e74 6169 6e65 725f 656d 6169  'maintainer_emai
-000014c0: 6c27 3a20 274e 6f6e 6527 2c0a 2020 2020  l': 'None',.    
-000014d0: 2775 726c 273a 2027 6874 7470 733a 2f2f  'url': 'https://
-000014e0: 6769 7468 7562 2e63 6f6d 2f6c 757a 6869  github.com/luzhi
-000014f0: 7869 6e67 3132 3334 352f 4d61 726b 646f  xing12345/Markdo
-00001500: 776e 5061 7273 6572 272c 0a20 2020 2027  wnParser',.    '
-00001510: 7061 636b 6167 6573 273a 2070 6163 6b61  packages': packa
-00001520: 6765 732c 0a20 2020 2027 7061 636b 6167  ges,.    'packag
-00001530: 655f 6461 7461 273a 2070 6163 6b61 6765  e_data': package
-00001540: 5f64 6174 612c 0a20 2020 2027 7079 7468  _data,.    'pyth
-00001550: 6f6e 5f72 6571 7569 7265 7327 3a20 273e  on_requires': '>
-00001560: 3d33 2e37 2c3c 342e 3027 2c0a 7d0a 0a0a  =3.7,<4.0',.}...
-00001570: 7365 7475 7028 2a2a 7365 7475 705f 6b77  setup(**setup_kw
-00001580: 6172 6773 290a                           args).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 726b  : 2.1.Name: mark
+00000020: 646f 776e 7061 7273 6572 0a56 6572 7369  downparser.Versi
+00000030: 6f6e 3a20 302e 352e 300a 5375 6d6d 6172  on: 0.5.0.Summar
+00000040: 793a 200a 486f 6d65 2d70 6167 653a 2068  y: .Home-page: h
+00000050: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000060: 6d2f 6c75 7a68 6978 696e 6731 3233 3435  m/luzhixing12345
+00000070: 2f4d 6172 6b64 6f77 6e50 6172 7365 720a  /MarkdownParser.
+00000080: 4c69 6365 6e73 653a 204d 4954 0a41 7574  License: MIT.Aut
+00000090: 686f 723a 206c 757a 6869 7869 6e67 3132  hor: luzhixing12
+000000a0: 3334 350a 4175 7468 6f72 2d65 6d61 696c  345.Author-email
+000000b0: 3a20 6c75 7a68 6978 696e 6731 3233 3435  : luzhixing12345
+000000c0: 4031 3633 2e63 6f6d 0a52 6571 7569 7265  @163.com.Require
+000000d0: 732d 5079 7468 6f6e 3a20 3e3d 332e 372c  s-Python: >=3.7,
+000000e0: 3c34 2e30 0a43 6c61 7373 6966 6965 723a  <4.0.Classifier:
+000000f0: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000100: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000110: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+00000120: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000130: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000140: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+00000150: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000160: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000170: 6f6e 203a 3a20 332e 370a 436c 6173 7369  on :: 3.7.Classi
+00000180: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001a0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+000001b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000001c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001d0: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+000001e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000200: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000210: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000220: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000230: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000240: 2e31 310a 5072 6f6a 6563 742d 5552 4c3a  .11.Project-URL:
+00000250: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
+00000260: 6874 7470 733a 2f2f 6c75 7a68 6978 696e  https://luzhixin
+00000270: 6731 3233 3435 2e67 6974 6875 622e 696f  g12345.github.io
+00000280: 2f4d 6172 6b64 6f77 6e50 6172 7365 722f  /MarkdownParser/
+00000290: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
+000002a0: 706f 7369 746f 7279 2c20 6874 7470 733a  pository, https:
+000002b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 757a  //github.com/luz
+000002c0: 6869 7869 6e67 3132 3334 352f 4d61 726b  hixing12345/Mark
+000002d0: 646f 776e 5061 7273 6572 0a44 6573 6372  downParser.Descr
+000002e0: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+000002f0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+00000300: 776e 0a0a 2320 4d61 726b 646f 776e 5061  wn..# MarkdownPa
+00000310: 7273 6572 0a0a 5b21 5b63 6f64 6563 6f76  rser..[![codecov
+00000320: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+00000330: 762e 696f 2f67 682f 6c75 7a68 6978 696e  v.io/gh/luzhixin
+00000340: 6731 3233 3435 2f4d 6172 6b64 6f77 6e50  g12345/MarkdownP
+00000350: 6172 7365 722f 6272 616e 6368 2f6d 6169  arser/branch/mai
+00000360: 6e2f 6772 6170 682f 6261 6467 652e 7376  n/graph/badge.sv
+00000370: 673f 295d 2868 7474 7073 3a2f 2f63 6f64  g?)](https://cod
+00000380: 6563 6f76 2e69 6f2f 6768 2f6c 757a 6869  ecov.io/gh/luzhi
+00000390: 7869 6e67 3132 3334 352f 4d61 726b 646f  xing12345/Markdo
+000003a0: 776e 5061 7273 6572 290a 0a4d 6172 6b64  wnParser)..Markd
+000003b0: 6f77 6e50 6172 7365 7220 e698 afe4 b880  ownParser ......
+000003c0: e4b8 aa20 4d61 726b 646f 776e 20e8 afad  ... Markdown ...
+000003d0: e6b3 95e8 a7a3 e69e 90e5 99a8 2ce7 94a8  ............,...
+000003e0: e4ba 8ee5 ae9e e78e b06d 64e5 88b0 6874  .........md...ht
+000003f0: 6d6c e6a0 87e7 adbe e79a 84e8 bdac e68d  ml..............
+00000400: a20a 0a23 2320 e5ae 89e8 a385 0a0a 6060  ...## ........``
+00000410: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+00000420: 6c20 6d61 726b 646f 776e 7061 7273 6572  l markdownparser
+00000430: 0a60 6060 0a0a 2323 20e5 bfab e980 9fe4  .```..## .......
+00000440: bdbf e794 a80a 0a60 6060 7079 7468 6f6e  .......```python
+00000450: 0a69 6d70 6f72 7420 4d61 726b 646f 776e  .import Markdown
+00000460: 5061 7273 6572 0a0a 6874 6d6c 203d 204d  Parser..html = M
+00000470: 6172 6b64 6f77 6e50 6172 7365 722e 7061  arkdownParser.pa
+00000480: 7273 6528 2723 2048 656c 6c6f 2057 6f72  rse('# Hello Wor
+00000490: 6c64 2127 290a 7072 696e 7428 6874 6d6c  ld!').print(html
+000004a0: 290a 0a23 3c64 6976 2063 6c61 7373 3d27  )..#<div class='
+000004b0: 6d61 726b 646f 776e 2d62 6f64 7927 3e3c  markdown-body'><
+000004c0: 6831 3e48 656c 6c6f 2057 6f72 6c64 213c  h1>Hello World!<
+000004d0: 2f68 313e 3c2f 6469 763e 0a60 6060 0a0a  /h1></div>.```..
+000004e0: e68e a5e5 8fa3 e587 bde6 95b0 0a0a 6060  ..............``
+000004f0: 6070 7974 686f 6e0a 2320 e8a7 a3e6 9e90  `python.# ......
+00000500: 206d 6172 6b64 6f77 6e20 e696 87e6 9cac   markdown ......
+00000510: e8bd ac20 6874 6d6c 0a64 6566 2070 6172  ... html.def par
+00000520: 7365 2874 6578 743a 2073 7472 2920 2d3e  se(text: str) ->
+00000530: 2073 7472 3a0a 0a23 20e8 a7a3 e69e 9020   str:..# ...... 
+00000540: 6d64 20e6 9687 e4bb b6e8 bdac 2068 746d  md ......... htm
+00000550: 6c0a 6465 6620 7061 7273 655f 6669 6c65  l.def parse_file
+00000560: 2866 696c 655f 6e61 6d65 3a20 7374 7229  (file_name: str)
+00000570: 202d 3e20 7374 723a 0a0a 2320 e8a7 a3e6   -> str:..# ....
+00000580: 9e90 206d 6172 6b64 6f77 6e20 e696 87e6  .. markdown ....
+00000590: 9cac 2c20 e5b8 a6e7 9bae e5bd 95e6 a091  .., ............
+000005a0: 0a64 6566 2070 6172 7365 5f74 6f63 2874  .def parse_toc(t
+000005b0: 6578 743a 2073 7472 2920 2d3e 2073 7472  ext: str) -> str
+000005c0: 3a0a 0a23 20e8 a7a3 e69e 9020 6d64 20e6  :..# ...... md .
+000005d0: 9687 e4bb b62c 20e5 b8a6 e79b aee5 bd95  ....., .........
+000005e0: e6a0 910a 6465 6620 7061 7273 655f 6669  ....def parse_fi
+000005f0: 6c65 5f74 6f63 2866 696c 655f 6e61 6d65  le_toc(file_name
+00000600: 3a20 7374 7229 202d 3e20 7374 723a 0a60  : str) -> str:.`
+00000610: 6060 0a0a e7ac ace4 ba8c e4b8 aae5 8f82  ``..............
+00000620: e695 b0e4 b8ba e58f afe9 8089 e9a1 b92c  ...............,
+00000630: 2060 6861 735f 7461 6760 20e8 a1a8 e7a4   `has_tag` .....
+00000640: bae6 98af e590 a6e5 b086 0a0a 2323 20e6  ............## .
+00000650: b58b e8af 950a 0a60 6060 6261 7368 0a70  .......```bash.p
+00000660: 7974 686f 6e20 6765 6e65 7261 7465 2e70  ython generate.p
+00000670: 7920 3c46 494c 455f 4e41 4d45 3e0a 0a23  y <FILE_NAME>..#
+00000680: 2070 7974 686f 6e20 6765 6e65 7261 7465   python generate
+00000690: 2e70 7920 2e2f 7465 7374 6669 6c65 732f  .py ./testfiles/
+000006a0: 7465 7374 312e 6d64 0a23 2070 7974 686f  test1.md.# pytho
+000006b0: 6e20 6765 6e65 7261 7465 2e70 7920 5245  n generate.py RE
+000006c0: 4144 4d45 2e6d 640a 6060 600a 0ae8 bf90  ADME.md.```.....
+000006d0: e8a1 8ce4 bc9a e794 9fe6 8890 696e 6465  ............inde
+000006e0: 782e 6874 6d6c 2c20 e4bd bfe7 94a8 e6b5  x.html, ........
+000006f0: 8fe8 a788 e599 a8e6 8993 e5bc 80e7 949f  ................
+00000700: e688 90e7 9a84 696e 6465 782e 6874 6d6c  ......index.html
+00000710: e58d b3e5 8faf e4b8 8ee6 82a8 e79a 844d  ...............M
+00000720: 6172 6b64 6f77 6ee7 bc96 e8be 91e5 99a8  arkdown.........
+00000730: e79a 84e9 a284 e69c 9fe6 b8b2 e69f 93e7  ................
+00000740: bb93 e69e 9ce5 afb9 e6af 940a 0a21 5b32  .............![2
+00000750: 3032 3330 3231 3832 3032 3430 305d 2868  0230218202400](h
+00000760: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000770: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000780: 2f6c 6561 726e 6572 2d6c 752f 7069 6362  /learner-lu/picb
+00000790: 6564 2f6d 6173 7465 722f 3230 3233 3032  ed/master/202302
+000007a0: 3138 3230 3234 3030 2e70 6e67 290a 0ae4  18202400.png)...
+000007b0: bba3 e7a0 81e8 a686 e79b 96e7 8e87 0a0a  ................
+000007c0: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
+000007d0: 616c 6c20 636f 7665 7261 6765 0a0a 636f  all coverage..co
+000007e0: 7665 7261 6765 2072 756e 202d 6d20 756e  verage run -m un
+000007f0: 6974 7465 7374 0a63 6f76 6572 6167 6520  ittest.coverage 
+00000800: 6874 6d6c 0a60 6060 0a0a 2323 20e5 ae9e  html.```..## ...
+00000810: e78e b0e6 809d e8b7 af0a 0a5b 4d61 726b  ...........[Mark
+00000820: 646f 776e e8a7 a3e6 9e90 e599 a8e7 9a84  down............
+00000830: e4bb a3e7 a081 e5ae 9ee7 8eb0 5d28 6874  ............](ht
+00000840: 7470 733a 2f2f 7777 772e 6269 6c69 6269  tps://www.bilibi
+00000850: 6c69 2e63 6f6d 2f76 6964 656f 2f42 5631  li.com/video/BV1
+00000860: 4c41 3431 3158 3758 3329 0a0a e682 a8e5  LA411X7X3)......
+00000870: 8faf e980 9ae8 bf87 e58f 96e6 b688 205b  .............. [
+00000880: 636f 7265 2e70 795d 282e 2f4d 6172 6b64  core.py](./Markd
+00000890: 6f77 6e50 6172 7365 722f 636f 7265 2e70  ownParser/core.p
+000008a0: 7929 20e6 b3a8 e987 8ae6 9da5 e88e b7e5  y) .............
+000008b0: 8f96 e6a0 91e7 9a84 e7bb 93e6 9e84 0a0a  ................
+000008c0: 6060 6070 7974 686f 6e0a 6465 6620 7061  ```python.def pa
+000008d0: 7273 6528 7365 6c66 2c20 7465 7874 3a20  rse(self, text: 
+000008e0: 7374 7229 202d 3e20 7374 723a 0a0a 2020  str) -> str:..  
+000008f0: 2020 2320 e58e bbe9 99a4 e7a9 bae8 a18c    # ............
+00000900: 2fe6 b3a8 e987 8a2f 6874 6d6c e6a0 87e7  /....../html....
+00000910: adbe 0a20 2020 206c 696e 6573 203d 2073  ...    lines = s
+00000920: 656c 662e 7072 6570 726f 6365 7373 5f70  elf.preprocess_p
+00000930: 6172 7365 7228 7465 7874 290a 2020 2020  arser(text).    
+00000940: 2320 7072 696e 7428 6c69 6e65 7329 0a20  # print(lines). 
+00000950: 2020 2023 20e9 8090 e8a1 8ce8 a7a3 e69e     # ...........
+00000960: 902c e5be 97e5 88b0 e4b8 80e9 a297 e69c  .,..............
+00000970: aae4 bc98 e58c 96e7 9a84 e6a0 910a 2020  ..............  
+00000980: 2020 726f 6f74 203d 2073 656c 662e 626c    root = self.bl
+00000990: 6f63 6b5f 7061 7273 6572 286c 696e 6573  ock_parser(lines
+000009a0: 290a 2020 2020 2320 726f 6f74 2e69 6e66  ).    # root.inf
+000009b0: 6f28 290a 2020 2020 2320 e4bc 98e5 8c96  o().    # ......
+000009c0: 2ce5 be97 e588 b0e6 ada3 e7a1 aee7 9a84  ,...............
+000009d0: 6d61 726b 646f 776e e8a7 a3e6 9e90 e6a0  markdown........
+000009e0: 910a 2020 2020 7472 6565 203d 2073 656c  ..    tree = sel
+000009f0: 662e 7472 6565 5f70 6172 7365 7228 726f  f.tree_parser(ro
+00000a00: 6f74 290a 2020 2020 2320 7472 6565 2e69  ot).    # tree.i
+00000a10: 6e66 6f28 290a 2020 2020 2320 e8be 93e5  nfo().    # ....
+00000a20: 87ba e588 b0e5 b18f e5b9 9520 2f20 e5af  ........... / ..
+00000a30: bce5 87ba 6874 6d6c e696 87e4 bbb6 0a20  ....html....... 
+00000a40: 2020 2072 6574 7572 6e20 7472 6565 2e74     return tree.t
+00000a50: 6f48 544d 4c28 290a 6060 600a 0a23 2320  oHTML().```..## 
+00000a60: e4b8 8de6 94af e68c 810a 0a2d 20e5 9b9b  ...........- ...
+00000a70: e4b8 aae7 a9ba e6a0 bce5 8f98 e4b8 bae4  ................
+00000a80: bba3 e7a0 81e6 aeb5 0a2d 205b 5e31 5de7  .........- [^1].
+00000a90: 9a84 e5bc 95e7 94a8 e696 b9e5 bc8f 0a2d  ...............-
+00000aa0: 2053 6574 6578 7420 e5bd a2e5 bc8f e79a   Setext ........
+00000ab0: 84e6 a087 e9a2 980a 2d20 e4b8 8ae6 a087  ........- ......
+00000ac0: 202f 20e4 b88b e6a0 8720 2f20 e4b8 8be5   / ...... / ....
+00000ad0: 8892 e7ba bf0a 0a23 2320 e8a1 a5e5 8585  .......## ......
+00000ae0: e8af b4e6 988e 0a0a 2d20 e794 9fe6 8890  ........- ......
+00000af0: e79a 84e7 bb93 e69e 9ce5 a682 e4b8 8b20  ............... 
+00000b00: 603c 6469 7620 636c 6173 733d 276d 6172  `<div class='mar
+00000b10: 6b64 6f77 6e2d 626f 6479 273e 6d61 726b  kdown-body'>mark
+00000b20: 646f 776e e586 85e5 aeb9 3c2f 6469 763e  down......</div>
+00000b30: 600a 2d20 e4bb a3e7 a081 e6ae b5e4 bc9a  `.- ............
+00000b40: e6a0 b9e6 8dae e8af ade8 a880 e58a a0e5  ................
+00000b50: 85a5 e4b8 80e4 b8aa e7b1 bbe5 908d e4be  ................
+00000b60: bfe4 ba8e e590 8ee6 9c9f e9ab 98e4 baae  ................
+00000b70: 2ce4 be8b e5a6 8220 6063 6c61 7373 3d22  ,...... `class="
+00000b80: 6c61 6e67 7561 6765 2d63 7070 2260 2c20  language-cpp"`, 
+00000b90: e69c aae5 ae9a e4b9 89e8 afad e8a8 80e5  ................
+00000ba0: 8899 e4b8 ba20 606c 616e 6775 6167 652d  ..... `language-
+00000bb0: 554e 4b4e 4f57 4e60 0a2d 20e9 bb98 e8ae  UNKNOWN`.- .....
+00000bc0: a4e5 afbc e587 bae7 9a84 4854 4d4c e4b8  ..........HTML..
+00000bd0: ade5 b182 e7ba a7e4 bbbb e58a a1e5 8897  ................
+00000be0: e8a1 a8e4 bc9a e69c 89e6 98be e7a4 bae9  ................
+00000bf0: 97ae e9a2 982c e8bf 99e6 98af e59b a0e4  .....,..........
+00000c00: b8ba e4bd bfe7 94a8 e4ba 8675 6c2b 6c69  ...........ul+li
+00000c10: 2b63 6865 636b 626f 78e7 9a84 e696 b9e5  +checkbox.......
+00000c20: bc8f 2ce6 82a8 e99c 80e8 a681 e6b7 bbe5  ..,.............
+00000c30: 8aa0 e4bb a5e4 b88b 6373 73e6 a0b7 e5bc  ........css.....
+00000c40: 8fe4 bfae e6ad a30a 0a20 2060 6060 6373  .........  ```cs
+00000c50: 730a 2020 2e6d 6172 6b64 6f77 6e2d 626f  s.  .markdown-bo
+00000c60: 6479 203e 2075 6c3e 6c69 3a68 6173 2869  dy > ul>li:has(i
+00000c70: 6e70 7574 2920 7b0a 2020 2020 7061 6464  nput) {.    padd
+00000c80: 696e 672d 6c65 6674 3a20 303b 0a20 2020  ing-left: 0;.   
+00000c90: 206d 6172 6769 6e2d 626f 7474 6f6d 3a20   margin-bottom: 
+00000ca0: 303b 0a20 207d 0a0a 2020 2e6d 6172 6b64  0;.  }..  .markd
+00000cb0: 6f77 6e2d 626f 6479 2020 756c 3e6c 693a  own-body  ul>li:
+00000cc0: 6861 7328 696e 7075 7429 3e75 6c20 7b0a  has(input)>ul {.
+00000cd0: 2020 2020 6c69 7374 2d73 7479 6c65 2d74      list-style-t
+00000ce0: 7970 653a 206e 6f6e 653b 0a20 2020 2070  ype: none;.    p
+00000cf0: 6164 6469 6e67 2d6c 6566 743a 2038 7078  adding-left: 8px
+00000d00: 3b0a 2020 7d0a 2020 6060 600a 0a2d 20e6  ;.  }.  ```..- .
+00000d10: 82a8 e58f afe4 bba5 e4bd bfe7 94a8 2060  .............. `
+00000d20: 7061 7273 655f 746f 6360 20e5 b086 2048  parse_toc` ... H
+00000d30: 6173 6848 6561 6442 6c6f 636b 20e6 8f90  ashHeadBlock ...
+00000d40: e58f 96e5 87ba e69d a5e7 bb84 e688 90e7  ................
+00000d50: 9bae e5bd 95e6 a091 2c20 e5be 97e5 88b0  ........, ......
+00000d60: e4b8 80e4 b8aa 2060 3c64 6976 2063 6c61  ...... `<div cla
+00000d70: 7373 3d22 6865 6164 6572 2d6e 6176 6967  ss="header-navig
+00000d80: 6174 6f72 223e 2e2e 2e3c 2f64 6976 3e60  ator">...</div>`
+00000d90: 20e5 b9b6 e6b7 bbe5 8aa0 e588 b0e8 bf94   ...............
+00000da0: e59b 9ee7 9a84 2048 544d 4c20 e585 83e7  ...... HTML ....
+00000db0: b4a0 e4b8 ad2c 20e6 82a8 e58f afe8 83bd  ....., .........
+00000dc0: e8bf 98e9 9c80 e8a6 81e4 b880 e4ba 9b20  ............... 
+00000dd0: 6a73 20e7 9bb8 e585 b3e7 9a84 e4bb a3e7  js .............
+00000de0: a081 e5ae 9ee7 8eb0 e8b7 b3e8 bdac 2c20  .............., 
+00000df0: e585 b7e4 bd93 e58f afe4 bba5 e58f 82e8  ................
+00000e00: 8083 205b 7465 6d70 6c61 7465 2e68 746d  .. [template.htm
+00000e10: 6c5d 282e 2f74 656d 706c 6174 652e 6874  l](./template.ht
+00000e20: 6d6c 290a 0a20 2060 6060 6a73 0a20 206c  ml)..  ```js.  l
+00000e30: 6574 206c 696e 6b73 203d 2064 6f63 756d  et links = docum
+00000e40: 656e 742e 7175 6572 7953 656c 6563 746f  ent.querySelecto
+00000e50: 7241 6c6c 2827 6469 7620 615b 6872 6566  rAll('div a[href
+00000e60: 5e3d 2223 225d 2729 3b0a 2020 2020 6c69  ^="#"]');.    li
+00000e70: 6e6b 732e 666f 7245 6163 6828 6c69 6e6b  nks.forEach(link
+00000e80: 203d 3e20 7b0a 2020 2020 2020 6c69 6e6b   => {.      link
+00000e90: 2e61 6464 4576 656e 744c 6973 7465 6e65  .addEventListene
+00000ea0: 7228 2763 6c69 636b 272c 2066 756e 6374  r('click', funct
+00000eb0: 696f 6e28 6576 656e 7429 207b 0a20 2020  ion(event) {.   
+00000ec0: 2020 2020 2065 7665 6e74 2e70 7265 7665       event.preve
+00000ed0: 6e74 4465 6661 756c 7428 293b 0a20 2020  ntDefault();.   
+00000ee0: 2020 2020 206c 6574 2074 6172 6765 7420       let target 
+00000ef0: 3d20 646f 6375 6d65 6e74 2e71 7565 7279  = document.query
+00000f00: 5365 6c65 6374 6f72 2874 6869 732e 6765  Selector(this.ge
+00000f10: 7441 7474 7269 6275 7465 2827 6872 6566  tAttribute('href
+00000f20: 2729 293b 0a20 2020 2020 2020 2074 6172  '));.        tar
+00000f30: 6765 742e 7363 726f 6c6c 496e 746f 5669  get.scrollIntoVi
+00000f40: 6577 287b 2062 6568 6176 696f 723a 2027  ew({ behavior: '
+00000f50: 736d 6f6f 7468 2720 7d29 3b0a 2020 2020  smooth' });.    
+00000f60: 2020 7d29 3b0a 2020 2020 7d29 3b0a 2020    });.    });.  
+00000f70: 6060 600a 0a20 20e4 bba5 e58f 8ae4 b880  ```..  .........
+00000f80: e4ba 9be6 a0b7 e5bc 8fe7 be8e e58c 960a  ................
+00000f90: 0a20 2060 6060 6373 730a 2020 2e68 6561  .  ```css.  .hea
+00000fa0: 6465 722d 6e61 7669 6761 746f 7220 7b0a  der-navigator {.
+00000fb0: 2020 2020 706f 7369 7469 6f6e 3a20 6669      position: fi
+00000fc0: 7865 643b 0a20 207d 0a20 2060 6060 0a0a  xed;.  }.  ```..
+00000fd0: 2d20 e5a6 82e6 9e9c e682 a8e6 83b3 e6b7  - ..............
+00000fe0: bbe5 8aa0 e5af b95b 4d65 726d 6169 645d  .......[Mermaid]
+00000ff0: 2868 7474 7073 3a2f 2f6d 6572 6d61 6964  (https://mermaid
+00001000: 2e6a 732e 6f72 672f 29e7 9a84 e694 afe6  .js.org/).......
+00001010: 8c81 2c20 e682 a8e5 8faf e58f 82e8 8083  .., ............
+00001020: 5b6d 6572 6d61 6964 2070 6c75 6769 6e5d  [mermaid plugin]
+00001030: 2868 7474 7073 3a2f 2f6d 6572 6d61 6964  (https://mermaid
+00001040: 2e6a 732e 6f72 672f 696e 7472 6f2f 6e30  .js.org/intro/n0
+00001050: 3062 2d67 6574 7469 6e67 5374 6172 7465  0b-gettingStarte
+00001060: 642e 6874 6d6c 235f 322d 7573 696e 672d  d.html#_2-using-
+00001070: 6d65 726d 6169 642d 706c 7567 696e 7329  mermaid-plugins)
+00001080: e59c a8e6 82a8 e79a 8468 746d 6ce9 a1b5  .........html...
+00001090: e99d a220 603c 626f 6479 3e60 20e6 9cab  ... `<body>` ...
+000010a0: e5b0 bee6 b7bb e58a a0e5 a682 e4b8 8b20  ............... 
+000010b0: 603c 7363 7269 7074 3e60 0a0a 2020 6060  `<script>`..  ``
+000010c0: 6068 746d 6c0a 2020 3c73 6372 6970 7420  `html.  <script 
+000010d0: 7479 7065 3d22 6d6f 6475 6c65 223e 0a20  type="module">. 
+000010e0: 2020 2063 6f6e 7374 2063 6f64 6542 6c6f     const codeBlo
+000010f0: 636b 7320 3d20 646f 6375 6d65 6e74 2e71  cks = document.q
+00001100: 7565 7279 5365 6c65 6374 6f72 416c 6c28  uerySelectorAll(
+00001110: 272e 6c61 6e67 7561 6765 2d6d 6572 6d61  '.language-merma
+00001120: 6964 2729 3b0a 2020 2020 636f 6465 426c  id');.    codeBl
+00001130: 6f63 6b73 2e66 6f72 4561 6368 2863 6f64  ocks.forEach(cod
+00001140: 6542 6c6f 636b 203d 3e20 7b0a 2020 2020  eBlock => {.    
+00001150: 2020 2020 636f 6465 426c 6f63 6b2e 636c      codeBlock.cl
+00001160: 6173 734c 6973 742e 7265 6d6f 7665 2827  assList.remove('
+00001170: 6c61 6e67 7561 6765 2d6d 6572 6d61 6964  language-mermaid
+00001180: 2729 3b0a 2020 2020 2020 2020 636f 6465  ');.        code
+00001190: 426c 6f63 6b2e 636c 6173 734c 6973 742e  Block.classList.
+000011a0: 6164 6428 276d 6572 6d61 6964 2729 3b0a  add('mermaid');.
+000011b0: 2020 2020 7d29 3b0a 2020 2020 696d 706f      });.    impo
+000011c0: 7274 206d 6572 6d61 6964 2066 726f 6d20  rt mermaid from 
+000011d0: 2768 7474 7073 3a2f 2f63 646e 2e6a 7364  'https://cdn.jsd
+000011e0: 656c 6976 722e 6e65 742f 6e70 6d2f 6d65  elivr.net/npm/me
+000011f0: 726d 6169 6440 3130 2f64 6973 742f 6d65  rmaid@10/dist/me
+00001200: 726d 6169 642e 6573 6d2e 6d69 6e2e 6d6a  rmaid.esm.min.mj
+00001210: 7327 3b0a 2020 2020 6d65 726d 6169 642e  s';.    mermaid.
+00001220: 696e 6974 6961 6c69 7a65 287b 2073 7461  initialize({ sta
+00001230: 7274 4f6e 4c6f 6164 3a20 7472 7565 207d  rtOnLoad: true }
+00001240: 293b 0a20 203c 2f73 6372 6970 743e 0a20  );.  </script>. 
+00001250: 2060 6060 0a0a 2020 3e20 2a2a e8af b7e6   ```..  > **....
+00001260: b3a8 e684 8f2a 2a2c 20e7 94b1 e4ba 8ee6  .....**, .......
+00001270: 9cac 4d61 726b 646f 776e e8a7 a3e6 9e90  ..Markdown......
+00001280: e599 a8e7 9a84 436f 6465 426c 6f63 6be8  ......CodeBlock.
+00001290: a7a3 e69e 90e5 be97 e588 b0e7 9a84 e7b1  ................
+000012a0: bbe5 908d e4b8 ba20 606c 616e 6775 6167  ....... `languag
+000012b0: 652d 6d65 726d 6169 6460 2c20 e880 8c6d  e-mermaid`, ...m
+000012c0: 6572 6d61 6964 e68f 92e4 bbb6 e694 afe6  ermaid..........
+000012d0: 8c81 e79a 84e7 b1bb e590 8de6 a0bc e5bc  ................
+000012e0: 8fe4 b8ba 606d 6572 6d61 6964 602c 20e6  ....`mermaid`, .
+000012f0: 8980 e4bb a5e4 bba3 e7a0 81e4 b8ad e689  ................
+00001300: 8be5 8aa8 e4bf aee6 94b9 e4ba 8620 606c  ............. `l
+00001310: 616e 6775 6167 652d 6d65 726d 6169 6460  anguage-mermaid`
+00001320: 20e7 9a84 e7b1 bbe5 908d 0a0a 2d20 e5a6   ...........- ..
+00001330: 82e6 9e9c e682 a8e6 83b3 e6b7 bbe5 8aa0  ................
+00001340: e5af b94c 6174 6578 e695 b0e5 ada6 e585  ...Latex........
+00001350: ace5 bc8f e79a 84e6 94af e68c 812c 20e5  ............., .
+00001360: 8faf e4bb a5e5 9ca8 6874 6d6c e9a1 b5e9  ........html....
+00001370: 9da2 2060 3c62 6f64 793e 6020 e69c abe5  .. `<body>` ....
+00001380: b0be e6b7 bbe5 8aa0 e5a6 82e4 b88b 2060  .............. `
+00001390: 3c73 6372 6970 743e 600a 0a20 2060 6060  <script>`..  ```
+000013a0: 6874 6d6c 0a20 203c 7363 7269 7074 3e0a  html.  <script>.
+000013b0: 2020 2020 2020 4d61 7468 4a61 7820 3d20        MathJax = 
+000013c0: 7b0a 2020 2020 2020 2020 7465 783a 207b  {.        tex: {
+000013d0: 0a20 2020 2020 2020 2020 2069 6e6c 696e  .          inlin
+000013e0: 654d 6174 683a 205b 5b27 2427 2c20 2724  eMath: [['$', '$
+000013f0: 275d 2c20 5b27 5c5c 2827 2c20 275c 5c29  '], ['\\(', '\\)
+00001400: 275d 5d0a 2020 2020 2020 2020 7d0a 2020  ']].        }.  
+00001410: 2020 2020 7d3b 0a20 2020 2020 203c 2f73      };.      </s
+00001420: 6372 6970 743e 0a20 203c 7363 7269 7074  cript>.  <script
+00001430: 2069 643d 224d 6174 684a 6178 2d73 6372   id="MathJax-scr
+00001440: 6970 7422 2061 7379 6e63 0a20 2073 7263  ipt" async.  src
+00001450: 3d22 6874 7470 733a 2f2f 6364 6e2e 6a73  ="https://cdn.js
+00001460: 6465 6c69 7672 2e6e 6574 2f6e 706d 2f6d  delivr.net/npm/m
+00001470: 6174 686a 6178 4033 2f65 7335 2f74 6578  athjax@3/es5/tex
+00001480: 2d63 6874 6d6c 2e6a 7322 3e0a 2020 3c2f  -chtml.js">.  </
+00001490: 7363 7269 7074 3e0a 2020 6060 600a 0a20  script>.  ```.. 
+000014a0: 20e6 b3a8 e684 8f2c e8bf 99e9 878c e4bb   ......,........
+000014b0: 85e6 94af e68c 81e5 be88 e5b0 91e4 b880  ................
+000014c0: e983 a8e5 8886 e695 b0e5 ada6 e585 ace5  ................
+000014d0: bc8f 0a0a 0a23 2320 e79b b8e5 85b3 e58f  .....## ........
+000014e0: 82e8 8083 0a0a 2d20 5b47 6974 6875 6220  ......- [Github 
+000014f0: 4d61 726b 646f 776e 2043 5353 5d28 6874  Markdown CSS](ht
+00001500: 7470 733a 2f2f 6364 6e2e 6a73 6465 6c69  tps://cdn.jsdeli
+00001510: 7672 2e6e 6574 2f6e 706d 2f67 6974 6875  vr.net/npm/githu
+00001520: 622d 6d61 726b 646f 776e 2d63 7373 4034  b-markdown-css@4
+00001530: 2e30 2e30 2f67 6974 6875 622d 6d61 726b  .0.0/github-mark
+00001540: 646f 776e 2e63 7373 290a 2d20 5b4d 6572  down.css).- [Mer
+00001550: 6d61 6964 2041 5049 5d28 6874 7470 733a  maid API](https:
+00001560: 2f2f 6d65 726d 6169 642e 6a73 2e6f 7267  //mermaid.js.org
+00001570: 2f69 6e74 726f 2f23 6d65 726d 6169 642d  /intro/#mermaid-
+00001580: 6170 6929 0a2d 205b 4d61 7468 4a61 785d  api).- [MathJax]
+00001590: 2868 7474 7073 3a2f 2f64 6f63 732e 6d61  (https://docs.ma
+000015a0: 7468 6a61 782e 6f72 672f 656e 2f6c 6174  thjax.org/en/lat
+000015b0: 6573 742f 7765 622f 7374 6172 742e 6874  est/web/start.ht
+000015c0: 6d6c 290a                                ml).
```

