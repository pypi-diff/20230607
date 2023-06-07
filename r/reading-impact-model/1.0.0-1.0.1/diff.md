# Comparing `tmp/reading_impact_model-1.0.0.tar.gz` & `tmp/reading_impact_model-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reading_impact_model-1.0.0.tar", max compression
+gzip compressed data, was "reading_impact_model-1.0.1.tar", max compression
```

## Comparing `reading_impact_model-1.0.0.tar` & `reading_impact_model-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     6941 2023-03-25 09:51:54.164506 reading_impact_model-1.0.0/README.md
--rw-r--r--   0        0        0     1185 2023-03-25 09:53:22.093629 reading_impact_model-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-25 09:53:22.093999 reading_impact_model-1.0.0/reading_impact_model/__init__.py
--rw-r--r--   0        0        0    21445 2023-03-25 09:23:34.833907 reading_impact_model-1.0.0/reading_impact_model/impact_model.py
--rw-r--r--   0        0        0        0 2023-03-21 06:20:35.500337 reading_impact_model-1.0.0/reading_impact_model/matchers/__init__.py
--rw-r--r--   0        0        0      203 2023-03-21 06:50:01.001599 reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5284 2023-03-22 13:46:51.249891 reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc
--rw-r--r--   0        0        0    14361 2023-03-25 09:36:41.648917 reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc
--rw-r--r--   0        0        0     1866 2023-03-24 12:38:36.508590 reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc
--rw-r--r--   0        0        0     4736 2023-03-22 13:16:07.552479 reading_impact_model-1.0.0/reading_impact_model/matchers/alpino_matcher.py
--rw-r--r--   0        0        0    11246 2023-03-21 06:24:13.469150 reading_impact_model-1.0.0/reading_impact_model/matchers/alpinor_matcher_old.py
--rw-r--r--   0        0        0    21410 2023-03-25 09:36:36.406988 reading_impact_model-1.0.0/reading_impact_model/matchers/matcher.py
--rw-r--r--   0        0        0      775 2023-03-21 06:27:57.741456 reading_impact_model-1.0.0/reading_impact_model/matchers/nltk_matcher.py
--rw-r--r--   0        0        0     1474 2023-03-24 12:38:28.094550 reading_impact_model-1.0.0/reading_impact_model/matchers/spacy_matcher.py
--rw-r--r--   0        0        0     1240 2023-03-22 13:17:03.674991 reading_impact_model-1.0.0/reading_impact_model/matchers/stanza_matcher.py
--rw-r--r--   0        0        0     1186 2023-03-22 13:17:03.671968 reading_impact_model-1.0.0/reading_impact_model/matchers/trankit_matcher.py
--rw-r--r--   0        0        0        0 2023-03-20 14:46:41.117875 reading_impact_model-1.0.0/reading_impact_model/model/__init__.py
--rw-r--r--   0        0        0     5589 2023-03-20 14:34:36.075954 reading_impact_model-1.0.0/reading_impact_model/model/phrase.py
--rw-r--r--   0        0        0        0 2023-03-20 14:46:41.124577 reading_impact_model-1.0.0/reading_impact_model/models/__init__.py
--rw-r--r--   0        0        0      201 2023-03-20 14:55:07.896122 reading_impact_model-1.0.0/reading_impact_model/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0   619876 2023-03-20 14:55:07.939597 reading_impact_model-1.0.0/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc
--rw-r--r--   0        0        0   160274 2023-03-20 14:55:07.905894 reading_impact_model-1.0.0/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc
--rw-r--r--   0        0        0   356666 2020-06-19 22:04:56.168319 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.1.pcl
--rw-r--r--   0        0        0   209835 2021-04-20 14:51:48.208246 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.2.pcl
--rw-r--r--   0        0        0   230737 2021-07-02 13:07:05.214976 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.3.pcl
--rw-r--r--   0        0        0   230678 2021-07-05 10:41:51.476919 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.4.pcl
--rw-r--r--   0        0        0   230690 2021-07-06 11:33:29.799021 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.5.pcl
--rw-r--r--   0        0        0   692078 2021-10-25 11:59:27.603446 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.6.json
--rw-r--r--   0        0        0   579958 2021-10-25 11:59:27.554350 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.6.pcl
--rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.251013 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.7.json
--rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.228629 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.7.pcl
--rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.264532 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en.json
--rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.234743 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en.pcl
--rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.657433 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-nl-1.0.json
--rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.645116 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-nl.json
--rw-r--r--   0        0        0   176064 2020-05-19 14:38:46.549523 reading_impact_model-1.0.0/reading_impact_model/models/impact_model-nl.pcl
--rw-r--r--   0        0        0   692090 2021-10-25 11:59:46.390314 reading_impact_model-1.0.0/reading_impact_model/models/impact_model_en.py
--rw-r--r--   0        0        0   244764 2023-03-20 14:34:33.867788 reading_impact_model-1.0.0/reading_impact_model/models/impact_model_nl.py
--rw-r--r--   0        0        0      903 2023-03-21 06:24:13.480622 reading_impact_model-1.0.0/reading_impact_model/reading_impact.py
--rw-r--r--   0        0        0     7854 1970-01-01 00:00:00.000000 reading_impact_model-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6941 2023-03-25 09:51:54.164506 reading_impact_model-1.0.1/README.md
+-rw-r--r--   0        0        0     1185 2023-06-07 13:55:29.913779 reading_impact_model-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-07 13:55:29.913977 reading_impact_model-1.0.1/reading_impact_model/__init__.py
+-rw-r--r--   0        0        0    21445 2023-03-25 09:23:34.833907 reading_impact_model-1.0.1/reading_impact_model/impact_model.py
+-rw-r--r--   0        0        0        0 2023-03-21 06:20:35.500337 reading_impact_model-1.0.1/reading_impact_model/matchers/__init__.py
+-rw-r--r--   0        0        0      203 2023-03-21 06:50:01.001599 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5284 2023-03-22 13:46:51.249891 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0    14361 2023-03-25 09:36:41.648917 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     1866 2023-03-24 12:38:36.508590 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     4736 2023-03-22 13:16:07.552479 reading_impact_model-1.0.1/reading_impact_model/matchers/alpino_matcher.py
+-rw-r--r--   0        0        0    11246 2023-03-21 06:24:13.469150 reading_impact_model-1.0.1/reading_impact_model/matchers/alpinor_matcher_old.py
+-rw-r--r--   0        0        0    21568 2023-06-07 13:48:46.145196 reading_impact_model-1.0.1/reading_impact_model/matchers/matcher.py
+-rw-r--r--   0        0        0      775 2023-03-21 06:27:57.741456 reading_impact_model-1.0.1/reading_impact_model/matchers/nltk_matcher.py
+-rw-r--r--   0        0        0     1532 2023-06-07 13:49:21.112807 reading_impact_model-1.0.1/reading_impact_model/matchers/spacy_matcher.py
+-rw-r--r--   0        0        0     1240 2023-03-22 13:17:03.674991 reading_impact_model-1.0.1/reading_impact_model/matchers/stanza_matcher.py
+-rw-r--r--   0        0        0     1186 2023-03-22 13:17:03.671968 reading_impact_model-1.0.1/reading_impact_model/matchers/trankit_matcher.py
+-rw-r--r--   0        0        0        0 2023-03-20 14:46:41.117875 reading_impact_model-1.0.1/reading_impact_model/model/__init__.py
+-rw-r--r--   0        0        0     5589 2023-03-20 14:34:36.075954 reading_impact_model-1.0.1/reading_impact_model/model/phrase.py
+-rw-r--r--   0        0        0        0 2023-03-20 14:46:41.124577 reading_impact_model-1.0.1/reading_impact_model/models/__init__.py
+-rw-r--r--   0        0        0      201 2023-03-20 14:55:07.896122 reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0   619876 2023-03-20 14:55:07.939597 reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc
+-rw-r--r--   0        0        0   160274 2023-03-20 14:55:07.905894 reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc
+-rw-r--r--   0        0        0   356666 2020-06-19 22:04:56.168319 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.1.pcl
+-rw-r--r--   0        0        0   209835 2021-04-20 14:51:48.208246 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.2.pcl
+-rw-r--r--   0        0        0   230737 2021-07-02 13:07:05.214976 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.3.pcl
+-rw-r--r--   0        0        0   230678 2021-07-05 10:41:51.476919 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.4.pcl
+-rw-r--r--   0        0        0   230690 2021-07-06 11:33:29.799021 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.5.pcl
+-rw-r--r--   0        0        0   692078 2021-10-25 11:59:27.603446 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.json
+-rw-r--r--   0        0        0   579958 2021-10-25 11:59:27.554350 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.pcl
+-rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.251013 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.json
+-rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.228629 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.pcl
+-rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.264532 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.json
+-rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.234743 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.pcl
+-rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.657433 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl-1.0.json
+-rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.645116 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.json
+-rw-r--r--   0        0        0   176064 2020-05-19 14:38:46.549523 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.pcl
+-rw-r--r--   0        0        0   692090 2021-10-25 11:59:46.390314 reading_impact_model-1.0.1/reading_impact_model/models/impact_model_en.py
+-rw-r--r--   0        0        0   244764 2023-03-20 14:34:33.867788 reading_impact_model-1.0.1/reading_impact_model/models/impact_model_nl.py
+-rw-r--r--   0        0        0      903 2023-03-21 06:24:13.480622 reading_impact_model-1.0.1/reading_impact_model/reading_impact.py
+-rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 reading_impact_model-1.0.1/PKG-INFO
```

### Comparing `reading_impact_model-1.0.0/README.md` & `reading_impact_model-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/pyproject.toml` & `reading_impact_model-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reading-impact-model"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Marijn Koolen <marijn.koolen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/marijnkoolen/reading-impact-model"
 repository = "https://github.com/marijnkoolen/reading-impact-model"
 classifiers = [
@@ -26,15 +26,15 @@
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `reading_impact_model-1.0.0/reading_impact_model/impact_model.py` & `reading_impact_model-1.0.1/reading_impact_model/impact_model.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc` & `reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc` & `reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc` & `reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/alpino_matcher.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/alpino_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/alpinor_matcher_old.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/alpinor_matcher_old.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/matcher.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,25 +133,25 @@
         vocab_terms = self.impact_model.get_matching_vocab_term(token.lemma)
         if isinstance(vocab_terms, str):
             self.sentence_vocab_terms[vocab_terms].add(token)
         elif isinstance(vocab_terms, set):
             for vocab_term in vocab_terms:
                 self.sentence_vocab_terms[vocab_term].add(token)
 
-    def _set_dict_sentence(self, sentence_index: int, sentence: Dict[str, any], doc_id: str) -> None:
+    def _set_dict_sentence(self, sentence: Dict[str, any], sentence_index: int, doc_id: str) -> None:
         self.sentence_string = sentence['text']
-        self.sentence_id = (sentence_index, doc_id)
+        self.sentence_id = (sentence_index, doc_id) if sentence_index and doc_id else None
         for ti, token in enumerate(sentence['tokens']):
             token = Token(word=token.word, index=ti, lemma=token.lemma, pos=token.pos if 'pos' in token else None)
             self._add_sentence_token(token)
             self.add_candidate_rules(token.word, token.lemma)
 
-    def _set_string_sentence(self, sentence_index: int, sentence: str, doc_id: str) -> None:
+    def _set_string_sentence(self, sentence: str, sentence_index: int, doc_id: str) -> None:
         self.sentence_string = sentence
-        self.sentence_id = (sentence_index, doc_id)
+        self.sentence_id = (sentence_index, doc_id) if sentence_index and doc_id else None
         words = re.split(r'\W+', sentence)
         for wi, word in enumerate(words):
             token = Token(word, wi, lemma=word)
             self._add_sentence_token(token)
             self.add_candidate_rules(word, word)
         # print('sentence_string:', self.sentence_string)
         # print('sentence_tokens:', self.sentence_tokens)
@@ -159,28 +159,28 @@
     def _reset_sentence(self):
         self.sentence_string = ''
         self.sentence_tokens = []
         self.sentence_vocab_terms = defaultdict(set)
         self.candidate_rules = defaultdict(int)
         self.sent_id = None
 
-    def _set_sentence(self, sentence_index: int, sentence: str, doc_id: str) -> None:
+    def _set_sentence(self, sentence: str, sentence_index: int = None, doc_id: str = None) -> None:
         self._reset_sentence()
         self.doc_id = doc_id
         if isinstance(sentence, dict) and 'text' in sentence and 'tokens' in sentence:
-            self._set_dict_sentence(sentence_index, sentence, doc_id)
+            self._set_dict_sentence(sentence, sentence_index=sentence_index, doc_id=doc_id)
         elif isinstance(sentence, str):
-            self._set_string_sentence(sentence_index, sentence, doc_id)
+            self._set_string_sentence(sentence, sentence_index=sentence_index, doc_id=doc_id)
         else:
             raise TypeError(
                 "sentence must be either a string, an Sentence object from Alpino, Spacy or Stanza.")
 
     def _iter_text_sentences(self, text: str, doc_id: str = None):
         for si, sent in enumerate(sent_tokenize(text)):
-            self._set_sentence(si, sent, doc_id)
+            self._set_sentence(sent, sentence_index=si, doc_id=doc_id)
             yield si
 
     def analyse_text(self, text: str, doc_id: str = None,
                      include_neutral: bool = False) -> List[Dict[str, any]]:
         all_matches = []
         for _ in self._iter_text_sentences(text, doc_id):
             sentence_matches = self._match_rules()
```

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/nltk_matcher.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/nltk_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/spacy_matcher.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/spacy_matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,20 @@
         super().__init__(lang=lang, impact_model=impact_model, **kwargs)
         self.parser = parser
         self.lang = lang
 
     def _iter_text_sentences(self, text: str, doc_id: str = None):
         doc = self.parser(text)
         for si, sent in enumerate(doc.sents):
-            self._set_sentence(si, sent, doc_id)
+            self._set_sentence(sent, si, doc_id)
             yield si
 
-    def _set_sentence(self, sentence_index: int, sentence: Union[str, SpacySentence], doc_id: str) -> None:
+    def _set_sentence(self, sentence: Union[str, SpacySentence],
+                      sentence_index: int = None,
+                      doc_id: str = None) -> None:
         self._reset_sentence()
         if isinstance(sentence, str):
             sentence = self.parser(sentence)
         self.sentence_string = sentence.text
         self.sentence_index = sentence_index
         self.doc_id = doc_id
         for si, spacy_token in enumerate(sentence):
```

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/stanza_matcher.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/stanza_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/matchers/trankit_matcher.py` & `reading_impact_model-1.0.1/reading_impact_model/matchers/trankit_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/model/phrase.py` & `reading_impact_model-1.0.1/reading_impact_model/model/phrase.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc` & `reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc` & `reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.1.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.1.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.2.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.2.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.3.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.3.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.4.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.4.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.5.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.5.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.6.json` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.6.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.7.json` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en-0.7.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en.json` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-en.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-nl-1.0.json` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl-1.0.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-nl.json` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model-nl.pcl` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model_en.py` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model_en.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/models/impact_model_nl.py` & `reading_impact_model-1.0.1/reading_impact_model/models/impact_model_nl.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/reading_impact_model/reading_impact.py` & `reading_impact_model-1.0.1/reading_impact_model/reading_impact.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.0/PKG-INFO` & `reading_impact_model-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: reading-impact-model
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Home-page: https://github.com/marijnkoolen/reading-impact-model
 License: MIT
 Author: Marijn Koolen
 Author-email: marijn.koolen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/marijnkoolen/reading-impact-model
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: reading-impact-model Version: 1.0.0 Summary: Home-
+Metadata-Version: 2.1 Name: reading-impact-model Version: 1.0.1 Summary: Home-
 page: https://github.com/marijnkoolen/reading-impact-model License: MIT Author:
 Marijn Koolen Author-email: marijn.koolen@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Topic :: Scientific/Engineering Requires-Dist: nltk
-(>=3.8.1,<4.0.0) Requires-Dist: pytest (>=7.2.2,<8.0.0) Requires-Dist:
-xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository, https://github.com/
-marijnkoolen/reading-impact-model Description-Content-Type: text/markdown #
-reading-impact-model Reading Impact Model for analyzing reading impact in
-online book reviews. - [Explanation of the impact types](./docs/impact.md) -
-[Examples of impact types](./docs/examples.md) - [Installation and Usage]
-(#installation-and-usage) - [Citing](#citing) - [Contributors](#contributors)
-## The Impact of Fiction How does your favorite book make you feel? If youâre
-an avid reader, this question might be hard to answer. Books can make us feel
-extatically happy or deeply sad. Books can inspire us, motivate us, or make us
-feel like we are a part of something that matters. As long as stories have
-existed, they have made people laugh, and they have made people cry. In this
-research project, we are trying to measure the emotional impact of books and
-stories, by analyzing the kind of emotional responses that readers express in
-online reviews. The Impact_of_Fiction is a project of the Huygens_Institute and
-the KNAW_Humanities_Cluster, coordinated by Peter Boot (Huygens) and Marijn
-Koolen (KNAW Humanities Cluster). ## Computational Analysis of Reading Impact
-There are millions upon millions of reviews on the internet today. Because of
-the staggering number of online reviews available, computational analysis is
-the ideal tool for analyzing them. But emotional impact is not easy to detect
-computationally. Thatâs why weâve created a list of words relating to
-features from literature (aspect-terms) and a list of words relating to
-literatureâs emotional impact (impact-terms) and a set of rules formulated to
-measure impact in relation to specific aspects. Hereâs an example:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: pytest
+(>=7.2.2,<8.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL:
+Repository, https://github.com/marijnkoolen/reading-impact-model Description-
+Content-Type: text/markdown # reading-impact-model Reading Impact Model for
+analyzing reading impact in online book reviews. - [Explanation of the impact
+types](./docs/impact.md) - [Examples of impact types](./docs/examples.md) -
+[Installation and Usage](#installation-and-usage) - [Citing](#citing) -
+[Contributors](#contributors) ## The Impact of Fiction How does your favorite
+book make you feel? If youâre an avid reader, this question might be hard to
+answer. Books can make us feel extatically happy or deeply sad. Books can
+inspire us, motivate us, or make us feel like we are a part of something that
+matters. As long as stories have existed, they have made people laugh, and they
+have made people cry. In this research project, we are trying to measure the
+emotional impact of books and stories, by analyzing the kind of emotional
+responses that readers express in online reviews. The Impact_of_Fiction is a
+project of the Huygens_Institute and the KNAW_Humanities_Cluster, coordinated
+by Peter Boot (Huygens) and Marijn Koolen (KNAW Humanities Cluster). ##
+Computational Analysis of Reading Impact There are millions upon millions of
+reviews on the internet today. Because of the staggering number of online
+reviews available, computational analysis is the ideal tool for analyzing them.
+But emotional impact is not easy to detect computationally. Thatâs why
+weâve created a list of words relating to features from literature (aspect-
+terms) and a list of words relating to literatureâs emotional impact (impact-
+terms) and a set of rules formulated to measure impact in relation to specific
+aspects. Hereâs an example:
 lovely        + character     = narrative engagement
 [impact-term] + [aspect-term] = type of impact
 By looking at examples from a large set of online reviews, we formulated more
 than 1300 rules of this kind, measuring different types of impact. For an
 explanation of our categories of impact, go to the âExplanation of impactâ
 page. Hereâs another example: In 2020, researchers at the Huygens Institute
 completed a similar research project on Dutch_online_reviews. They found, among
```

