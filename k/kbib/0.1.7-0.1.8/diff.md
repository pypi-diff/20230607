# Comparing `tmp/kbib-0.1.7.tar.gz` & `tmp/kbib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbib-0.1.7.tar", last modified: Tue May 23 14:40:30 2023, max compression
+gzip compressed data, was "kbib-0.1.8.tar", last modified: Wed Jun  7 12:57:41 2023, max compression
```

## Comparing `kbib-0.1.7.tar` & `kbib-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:30.042519 kbib-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 14:40:09.000000 kbib-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 14:40:09.000000 kbib-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-23 14:40:30.042519 kbib-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-23 14:40:09.000000 kbib-0.1.7/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:30.042519 kbib-0.1.7/kbib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:09.000000 kbib-0.1.7/kbib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-23 14:40:09.000000 kbib-0.1.7/kbib/parseRefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-23 14:40:09.000000 kbib-0.1.7/kbib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:40:30.042519 kbib-0.1.7/kbib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 14:40:30.000000 kbib-0.1.7/kbib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:40:29.000000 kbib-0.1.7/kbib.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:40:30.042519 kbib-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-23 14:40:09.000000 kbib-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:41.454111 kbib-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 12:57:21.000000 kbib-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 12:57:21.000000 kbib-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 12:57:41.454111 kbib-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-07 12:57:21.000000 kbib-0.1.8/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:41.454111 kbib-0.1.8/kbib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:21.000000 kbib-0.1.8/kbib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-07 12:57:21.000000 kbib-0.1.8/kbib/parseRefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-06-07 12:57:21.000000 kbib-0.1.8/kbib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:57:41.454111 kbib-0.1.8/kbib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:57:41.000000 kbib-0.1.8/kbib.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:57:41.454111 kbib-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 12:57:21.000000 kbib-0.1.8/setup.py
```

### Comparing `kbib-0.1.7/LICENSE` & `kbib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kbib-0.1.7/PKG-INFO` & `kbib-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.7
+Version: 0.1.8
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,17 +58,18 @@
 
 | Argument    |  Description|
 | ----------- | ----------- 
 |    `-bib`    | DOI to get bibtex entry |
 |    `-ref`    | DOI to get bibtex entries for all the references | 
 |    `-pdf`    | PDF file name(s) to get bibtex info | 
 |    `-ren`    | PDF file name(s) to rename with bibtex info | 
-|    `-dup`    | Bib file name(s) to find duplicates. | 
+|    `-dup`    | Bib/Tex file name(s) to find duplicates. | 
 |    `-o`      | Output bib file | 
 
+#### Use cases
 * Get bibtex from a DOI
     ```bash
     kbib -bib https://doi.org/10xxxxxx
     ```
 * Get bibtex from a DOI and store in a file 'ref.bib'
     ```bash
     kbib -bib https://doi.org/10xxxxxx -o ref.bib
@@ -92,14 +93,22 @@
     kbib -ren *.pdf
     ```
 * Find duplicate bib entries in bibtex files.
     ```bash
     kbib -dup article_1.bib article_2.bib
     ```
 
+* If a .tex file is provided, it will find the duplicates that are cited in the tex file
+    ```bash
+    kbib -dup article.tex article_1.bib article_2.bib
+    ```
+
+
+
+
 #### ⚓Limitation:
 - `kbib` parses DOI information from [Crossref API](https://github.com/CrossRef/rest-api-doc). So if the article is not indexed in Crossref database this tool will fail to get the necessary information. Also the API may temporarily block requests from an IP if a large number of queries are made within a short period of time.
 - Special/Latex characters in the title may gets messed up during the API call. One needs to be careful using title field for the bibtex created by `kbib`.
 - For bibtex keys and renaming files, `kbib` uses format as `<Short Journal Name>_<Volume>_<Year>_<Last name of first author>`, which is presently hardcoded in the tool. Therefore, one can not use any desired format through the command line.
 
 
 #### ⏳ Work-in-Progress:
```

### Comparing `kbib-0.1.7/Readme.md` & `kbib-0.1.8/Readme.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,17 +35,18 @@
 
 | Argument    |  Description|
 | ----------- | ----------- 
 |    `-bib`    | DOI to get bibtex entry |
 |    `-ref`    | DOI to get bibtex entries for all the references | 
 |    `-pdf`    | PDF file name(s) to get bibtex info | 
 |    `-ren`    | PDF file name(s) to rename with bibtex info | 
-|    `-dup`    | Bib file name(s) to find duplicates. | 
+|    `-dup`    | Bib/Tex file name(s) to find duplicates. | 
 |    `-o`      | Output bib file | 
 
+#### Use cases
 * Get bibtex from a DOI
     ```bash
     kbib -bib https://doi.org/10xxxxxx
     ```
 * Get bibtex from a DOI and store in a file 'ref.bib'
     ```bash
     kbib -bib https://doi.org/10xxxxxx -o ref.bib
@@ -69,14 +70,22 @@
     kbib -ren *.pdf
     ```
 * Find duplicate bib entries in bibtex files.
     ```bash
     kbib -dup article_1.bib article_2.bib
     ```
 
+* If a .tex file is provided, it will find the duplicates that are cited in the tex file
+    ```bash
+    kbib -dup article.tex article_1.bib article_2.bib
+    ```
+
+
+
+
 #### ⚓Limitation:
 - `kbib` parses DOI information from [Crossref API](https://github.com/CrossRef/rest-api-doc). So if the article is not indexed in Crossref database this tool will fail to get the necessary information. Also the API may temporarily block requests from an IP if a large number of queries are made within a short period of time.
 - Special/Latex characters in the title may gets messed up during the API call. One needs to be careful using title field for the bibtex created by `kbib`.
 - For bibtex keys and renaming files, `kbib` uses format as `<Short Journal Name>_<Volume>_<Year>_<Last name of first author>`, which is presently hardcoded in the tool. Therefore, one can not use any desired format through the command line.
 
 
 #### ⏳ Work-in-Progress:
```

### Comparing `kbib-0.1.7/kbib/parseRefs.py` & `kbib-0.1.8/kbib/parseRefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     )
 
     #adding options for numerical jobs
     parser.add_argument('-bib', type=str, help="DOI to get bibtex entry", metavar="DOI")
     parser.add_argument('-ref', type=str, help="DOI to get bibtex entries for all the references", metavar="DOI")
     parser.add_argument('-pdf', type=str, help="PDF file name(s) to get bibtex info", metavar="PDF", nargs='*')
     parser.add_argument('-ren', type=str, help="PDF file name(s) to rename with bibtex info", metavar="PDF", nargs='*')
-    parser.add_argument('-dup', type=str, help="Bib file name(s) to find duplicates.", metavar="BIB", nargs='*')
+    parser.add_argument('-dup', type=str, help="Bib/Tex file name(s) to find duplicates.", metavar="BIB", nargs='*')
     parser.add_argument('-o',   type=str, help="Output bib file", metavar="FILE")
 
     return parser
```

### Comparing `kbib-0.1.7/kbib/utils.py` & `kbib-0.1.8/kbib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     TimeRemainingColumn,
     BarColumn,
     MofNCompleteColumn
 )
 from argparse import ArgumentParser, RawTextHelpFormatter
 from datetime import timedelta
 from rich import print as rprint
-from collections import Counter
+from collections import Counter, defaultdict
 try:
     import pdf2doi
     PDF_AVAILABLE = True
     pdf2doi.config.set('verbose',False)
 except ImportError:
     PDF_AVAILABLE = False
 
@@ -272,36 +272,93 @@
             ch = input(f"Rename {file} -> {newName}? [y/n] ")
             if ch=='y':
                 os.rename(file,newName)
 
 
 
 
-def listDuplicates(bibFiles):
+def getCitaionsFromTex(texFile):
+    with open(texFile) as f:
+        txt = f.read()
+    rx = re.compile(r'''(?<!\\)%.+|(\\(?:no)?citep?\{((?!\*)[^{}]+)\})''')
+
+
+    authors = [m.group(2) for m in rx.finditer(txt) if m.group(2)]
+
+    allBibs = []
+
+    for i in authors:
+        j = i.split(',')
+        j = [k.strip() for k in j]
+        allBibs.extend(j)
+
+
+    allBibs = list(set(allBibs))
+    return allBibs
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+def listDuplicates(files):
+    
+    bibFiles, texFiles = [], []
+
+
+    for f in files:
+        if f.endswith('.tex'):
+            texFiles.append(f)
+        elif f.endswith('.bib'):
+            bibFiles.append(f)
+        else:
+            raise Exception('Only .tex or .bib files are allowed.')
+
+    if len(texFiles)>1:
+        raise Exception("Only one .tex file is allowed.")
+
+
+    checkTex = False
+    if len(texFiles)>1:
+        raise Exception("Only one .tex file is allowed.")
+    elif len(texFiles)==1:
+        cites = getCitaionsFromTex(texFiles[0])
+        checkTex = True
+
+
+
     bib_db = bibtexparser.loads('\n'.join(open(f).read() for f in bibFiles))
     entries = bib_db.entries
 
-    # decide duplicates based on year, volume and pages. Can we make it in more sophisticated way
-    test_en = [(en.get('year',''), en.get('volume',''),en.get('pages','')) for en in entries]
-
-    duplicates = []
-    for item, count in Counter(test_en).items():
-        if count>1:
-            dupTmp = []
-            for en in entries:
-                it = (en.get('year',''), en.get('volume',''),en.get('pages',''))
-                if it==item:
-                    dupTmp.append(en.get('ID'))
-            if len(dupTmp)>1:
-                duplicates.append(dupTmp)
-
-    if len(duplicates):
-        print("The following bib entries may be duplicate. Please check:")
-        for i, item in enumerate(duplicates, start=1):
-            print(f"{i}. {' '.join(item)}")
+    dat = defaultdict(list)
+    # duplication will be decided based only on these keys
+    keysToMatch = ['year','volume','pages']  
+
+
+    for en in entries:
+        it = tuple(en.get(i,'') for i in keysToMatch)
+        idd = en.get('ID')
+        if checkTex:
+            if idd in cites:  # only references that are cited
+                dat[it].append(en.get('ID'))
+        else:
+            dat[it].append(en.get('ID'))
+
+
+    for k,v in dat.items():
+        if len(v)>1:
+            print(v)
 
 
 # progress = Progress()
 
 # progress.start()
 # task = progress.add_task("Getting references-------------",total=124)
```

### Comparing `kbib-0.1.7/kbib.egg-info/PKG-INFO` & `kbib-0.1.8/kbib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.7
+Version: 0.1.8
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,17 +58,18 @@
 
 | Argument    |  Description|
 | ----------- | ----------- 
 |    `-bib`    | DOI to get bibtex entry |
 |    `-ref`    | DOI to get bibtex entries for all the references | 
 |    `-pdf`    | PDF file name(s) to get bibtex info | 
 |    `-ren`    | PDF file name(s) to rename with bibtex info | 
-|    `-dup`    | Bib file name(s) to find duplicates. | 
+|    `-dup`    | Bib/Tex file name(s) to find duplicates. | 
 |    `-o`      | Output bib file | 
 
+#### Use cases
 * Get bibtex from a DOI
     ```bash
     kbib -bib https://doi.org/10xxxxxx
     ```
 * Get bibtex from a DOI and store in a file 'ref.bib'
     ```bash
     kbib -bib https://doi.org/10xxxxxx -o ref.bib
@@ -92,14 +93,22 @@
     kbib -ren *.pdf
     ```
 * Find duplicate bib entries in bibtex files.
     ```bash
     kbib -dup article_1.bib article_2.bib
     ```
 
+* If a .tex file is provided, it will find the duplicates that are cited in the tex file
+    ```bash
+    kbib -dup article.tex article_1.bib article_2.bib
+    ```
+
+
+
+
 #### ⚓Limitation:
 - `kbib` parses DOI information from [Crossref API](https://github.com/CrossRef/rest-api-doc). So if the article is not indexed in Crossref database this tool will fail to get the necessary information. Also the API may temporarily block requests from an IP if a large number of queries are made within a short period of time.
 - Special/Latex characters in the title may gets messed up during the API call. One needs to be careful using title field for the bibtex created by `kbib`.
 - For bibtex keys and renaming files, `kbib` uses format as `<Short Journal Name>_<Volume>_<Year>_<Last name of first author>`, which is presently hardcoded in the tool. Therefore, one can not use any desired format through the command line.
 
 
 #### ⏳ Work-in-Progress:
```

### Comparing `kbib-0.1.7/setup.py` & `kbib-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('Readme.md') as f:
     txt = f.read()
 
 setup(name='kbib',
-    version='0.1.7',
+    version='0.1.8',
     description='A command line tool to get bibtex information from DOIs and PDFs',
     long_description=txt,
     long_description_content_type='text/markdown',
     author='Koushik Naskar',
     author_email='koushik.naskar9@gmail.com',
     license="MIT",
     classifiers=[
```

