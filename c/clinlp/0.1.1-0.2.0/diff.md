# Comparing `tmp/clinlp-0.1.1.tar.gz` & `tmp/clinlp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.1.1.tar", max compression
+gzip compressed data, was "clinlp-0.2.0.tar", max compression
```

## Comparing `clinlp-0.1.1.tar` & `clinlp-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-06 13:37:40.385218 clinlp-0.1.1/LICENSE
--rw-r--r--   0        0        0     8381 2023-05-23 14:07:16.856255 clinlp-0.1.1/README.md
--rw-r--r--   0        0        0       54 2023-05-23 13:53:46.196466 clinlp-0.1.1/clinlp/__init__.py
--rw-r--r--   0        0        0      250 2023-05-23 11:18:41.641635 clinlp-0.1.1/clinlp/component/__init__.py
--rw-r--r--   0        0        0    10757 2023-05-23 14:07:16.856623 clinlp-0.1.1/clinlp/component/qualifier.py
--rw-r--r--   0        0        0     2308 2023-05-23 11:18:41.641955 clinlp-0.1.1/clinlp/component/sentencizer.py
--rw-r--r--   0        0        0     7698 2023-05-23 13:20:57.844906 clinlp-0.1.1/clinlp/language.py
--rw-r--r--   0        0        0        0 2023-05-23 14:07:16.856699 clinlp-0.1.1/clinlp/resources/__init__.py
--rw-r--r--   0        0        0    24443 2023-05-23 13:32:24.283263 clinlp-0.1.1/clinlp/resources/psynlp_context_rules.json
--rw-r--r--   0        0        0      547 2023-05-23 14:09:46.872858 clinlp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9475 1970-01-01 00:00:00.000000 clinlp-0.1.1/setup.py
--rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 clinlp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 14:24:05.405783 clinlp-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8573 2023-06-07 14:24:05.405783 clinlp-0.2.0/README.md
+-rw-r--r--   0        0        0       54 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/__init__.py
+-rw-r--r--   0        0        0      285 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/__init__.py
+-rw-r--r--   0        0        0     1403 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/normalizer.py
+-rw-r--r--   0        0        0    10756 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/qualifier.py
+-rw-r--r--   0        0        0     2308 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/component/sentencizer.py
+-rw-r--r--   0        0        0     8447 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/language.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    24446 2023-06-07 14:24:05.405783 clinlp-0.2.0/clinlp/resources/psynlp_context_rules.json
+-rw-r--r--   0        0        0      547 2023-06-07 14:24:05.405783 clinlp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9131 1970-01-01 00:00:00.000000 clinlp-0.2.0/PKG-INFO
```

### Comparing `clinlp-0.1.1/LICENSE` & `clinlp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.1.1/README.md` & `clinlp-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,54 +24,36 @@
 ### Example
 ```python
 import clinlp
 import spacy
 
 nlp = spacy.blank("clinlp")
 
-# Sentences
-nlp.add_pipe('clinlp_sentencizer')
-
-# Entities
-ruler = nlp.add_pipe('entity_ruler')
-
-terms = {
-    'covid_19_symptomen': [
-        'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
-        'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
-        'koorts', 'verlies van reuk', 'verlies van smaak'
-    ]
-}
-
-for term_description, terms in terms.items():
-    ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
-import clinlp
-import spacy
-
-nlp = spacy.blank("clinlp")
+# Normalization
+nlp.add_pipe('clinlp_normalizer')
 
 # Sentences
 nlp.add_pipe('clinlp_sentencizer')
 
 # Entities
-ruler = nlp.add_pipe('entity_ruler')
+ruler = nlp.add_pipe('entity_ruler', config={'phrase_matcher_attr': "NORM"})
 
 terms = {
     'covid_19_symptomen': [
         'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
         'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
         'koorts', 'verlies van reuk', 'verlies van smaak'
     ]
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 
 # Qualifiers
-nlp.add_pipe('clinlp_context_matcher')
+nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
 
 text = (
     "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
     "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
     "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
@@ -107,51 +89,60 @@
 ### Introduction
 
 `clinlp` is built on top of spaCy, a widely used library for Natural Language Processing. Before getting started with `clinlp`, it may be useful to read [spaCy 101: Everything you need to know (~10 mins)](https://spacy.io/usage/spacy-101). Main things to know are that spaCy consists of a tokenizer (breaks a text up into small pieces, i.e. words), and various components that further process the text. 
 
 Currently, `clinlp` offers the following components, tailored to Dutch Clinical text, further discussed below: 
 
 1. [Tokenizer](#tokenizer)
-2. [Sentence splitter](#sentence-splitter)
-3. [Entity matcher (builtin Spacy)](#entity-matcher)
-4. [Context detection](#context-detection)
+2. [Normalizer](#normalizer)
+3. [Sentence splitter](#sentence-splitter)
+4. [Entity matcher (builtin Spacy)](#entity-matcher)
+5. [Context detection](#context-detection)
 
 ### Tokenizer
 
-The `clinlp` tokenizer is builin the blank model:
+The `clinlp` tokenizer is built into the blank model:
 
 ```python
 nlp = spacy.blank('clinlp')
 ```
 
 It employs some custom rule based logic, including:
 - Clinical text-specific logic for splitting punctuation, units, dosages (e.g. `20mg/dag` :arrow_right: `20` `mg` `/` `dag`)
 - Custom lists of abbreviations, units (e.g. `pt.`, `zn.`, `mmHg`)
 - Custom tokenizing rules (e.g. `xdd` :arrow_right: `x` `dd`)
 - Regarding [DEDUCE](https://github.com/vmenger/deduce) tags as a single token (e.g. `[DATUM-1]`). 
   - Deidentification is not builtin `clinlp` and should be done as a preprocessing step.
 
+### Normalizer
+
+The normalizer sets the `token.norm` attribute, which can be used by further components (entity recognition, qualification) for matching. It currently has two options (enabled by default):
+- Lowercasing
+- Removing diacritings, where possible. For instance, it will map `ë` `->` `e`, but keeps most other non-ascii characters intact (e.g. `µ`, `²`).
+
+Note that this component only has effect when explicitly configuring successor components to match on the `token.norm` attribute. 
+
 ### Sentence splitter
 
 The sentence splitter can be added as follows:
 
 ```python
 nlp.add_pipe('clinlp_sentencizer')
 ```
 
 It is designed to detect sentence boundaries in clinical text, whenever a character that demarks a sentence ending is matched (e.g. newline, period, question mark). It also correctly detects items in an enumerations (e.g. starting with `-` or `*`). 
 
 ### Entity matcher
 
-Currently, the spaCy builtin `PhraseMatcher` and `Matcher` can be used for finding (named) entities in text. The first one accepts literal phrases only, that are matched in the tokenized text, while the second only also accepts [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns). These are not tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained.
+Currently, the spaCy builtin `PhraseMatcher` and `Matcher` can be used for finding (named) entities in text. The first one accepts literal phrases only, that are matched in the tokenized text, while the second one also accepts [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns). These are not tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained.
 
 For instance, a matcher that helps recognize COVID19 symptoms:
 
 ```python
-ruler = nlp.add_pipe('entity_ruler')
+ruler = nlp.add_pipe('entity_ruler', config={'phrase_matcher_attr': "NORM"})
 
 terms = {
     'covid_19_symptomen': [
         'verkouden', 'neusverkouden', 'loopneus', 'niezen', 
         'keelpijn', 'hoesten', 'benauwd', 'kortademig', 'verhoging', 
         'koorts', 'verlies van reuk', 'verlies van smaak'
     ]
@@ -171,15 +162,15 @@
 ### Context detection
 
 After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) for this purpose. This algorithm is fairly accurate, and quite transparent and fast. Better solutions will hopefully be added to `clinlp` in the future. 
 
 A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
 
 ```python
-nlp.add_pipe('clinlp_context_matcher')
+nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
 ```
 
 A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows: 
 
 ```python
 from clinlp.component.qualifier import parse_rules
```

### Comparing `clinlp-0.1.1/clinlp/component/qualifier.py` & `clinlp-0.2.0/clinlp/component/qualifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,14 @@
         if default_rules is not None:
             self._load_default_rules(default_rules)
 
         if rules:
             self.add_rules(rules)
 
     def _load_default_rules(self, default_rules: str):
-
         with importlib.resources.path("clinlp.resources", default_rules) as path:
             self.add_rules(parse_rules(path))
 
     def add_rule(self, rule: ContextRule):
         """
         Add a rule.
         """
```

### Comparing `clinlp-0.1.1/clinlp/component/sentencizer.py` & `clinlp-0.2.0/clinlp/component/sentencizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.1.1/clinlp/language.py` & `clinlp-0.2.0/clinlp/language.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import importlib.metadata
+import warnings
 from typing import Callable, Optional
 
 import spacy.lang.char_classes
 import spacy.lang.nl.tokenizer_exceptions
 import spacy.lang.punctuation
 import spacy.lang.tokenizer_exceptions
 from spacy.language import BaseDefaults, Language
@@ -378,7 +380,24 @@
     writing_system = {"direction": "ltr", "has_case": True, "has_letters": True}
 
 
 @spacy.registry.languages("clinlp")
 class Clinlp(Language):
     lang = "clinlp"
     Defaults = ClinlpDefaults
+
+    def __init__(self, *args, **kwargs):
+        meta = dict(kwargs.pop("meta", {}))
+        clinlp_version = importlib.metadata.version(__package__ or __name__)
+
+        if "clinlp_version" in meta:
+            if meta["clinlp_version"] != clinlp_version:
+                warnings.warn(
+                    f"This spaCy model was built with clinlp version {meta['clinlp_version']}, "
+                    f"but you currently have version {clinlp_version} installed, "
+                    f"potentially leading to unexpected results.",
+                    UserWarning,
+                )
+        else:
+            meta["clinlp_version"] = clinlp_version
+
+        super().__init__(*args, meta=meta, **kwargs)
```

### Comparing `clinlp-0.1.1/clinlp/resources/psynlp_context_rules.json` & `clinlp-0.2.0/clinlp/resources/psynlp_context_rules.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'description'": "'A set of context rules based on the psynlp package, a rule-based approach "*

 * *                  "somewhat tailored to information extraction from clinical text.'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "description": "A set of qualifiers based on the psynlp package, a rule-based approach somewhat tailored to information extraction from clinical text.",
+    "description": "A set of context rules based on the psynlp package, a rule-based approach somewhat tailored to information extraction from clinical text.",
     "name": "default_qualifiers",
     "qualifiers": [
         {
             "levels": [
                 "PATIENT",
                 "OTHER"
             ],
```

### Comparing `clinlp-0.1.1/pyproject.toml` & `clinlp-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinlp"
-version = "0.1.1"
+version = "0.2.0"
 description = "Performant and production-ready NLP pipelines for clinical text written in Dutch"
 authors = ["UMCU DIT Analytics <analytics@umcutrecht.nl>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 spacy = "^3.4.4"
```

### Comparing `clinlp-0.1.1/PKG-INFO` & `clinlp-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.1.1
+Version: 0.2.0
 Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
 Author: UMCU DIT Analytics
 Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -39,54 +39,36 @@
 ### Example
 ```python
 import clinlp
 import spacy
 
 nlp = spacy.blank("clinlp")
 
-# Sentences
-nlp.add_pipe('clinlp_sentencizer')
-
-# Entities
-ruler = nlp.add_pipe('entity_ruler')
-
-terms = {
-    'covid_19_symptomen': [
-        'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
-        'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
-        'koorts', 'verlies van reuk', 'verlies van smaak'
-    ]
-}
-
-for term_description, terms in terms.items():
-    ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
-import clinlp
-import spacy
-
-nlp = spacy.blank("clinlp")
+# Normalization
+nlp.add_pipe('clinlp_normalizer')
 
 # Sentences
 nlp.add_pipe('clinlp_sentencizer')
 
 # Entities
-ruler = nlp.add_pipe('entity_ruler')
+ruler = nlp.add_pipe('entity_ruler', config={'phrase_matcher_attr': "NORM"})
 
 terms = {
     'covid_19_symptomen': [
         'verkoudheid', 'neusverkoudheid', 'loopneus', 'niezen', 'vermoeidheid',
         'keelpijn', 'hoesten', 'benauwdheid', 'kortademigheid', 'verhoging', 
         'koorts', 'verlies van reuk', 'verlies van smaak'
     ]
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 
 # Qualifiers
-nlp.add_pipe('clinlp_context_matcher')
+nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
 
 text = (
     "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
     "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
     "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
@@ -122,51 +104,60 @@
 ### Introduction
 
 `clinlp` is built on top of spaCy, a widely used library for Natural Language Processing. Before getting started with `clinlp`, it may be useful to read [spaCy 101: Everything you need to know (~10 mins)](https://spacy.io/usage/spacy-101). Main things to know are that spaCy consists of a tokenizer (breaks a text up into small pieces, i.e. words), and various components that further process the text. 
 
 Currently, `clinlp` offers the following components, tailored to Dutch Clinical text, further discussed below: 
 
 1. [Tokenizer](#tokenizer)
-2. [Sentence splitter](#sentence-splitter)
-3. [Entity matcher (builtin Spacy)](#entity-matcher)
-4. [Context detection](#context-detection)
+2. [Normalizer](#normalizer)
+3. [Sentence splitter](#sentence-splitter)
+4. [Entity matcher (builtin Spacy)](#entity-matcher)
+5. [Context detection](#context-detection)
 
 ### Tokenizer
 
-The `clinlp` tokenizer is builin the blank model:
+The `clinlp` tokenizer is built into the blank model:
 
 ```python
 nlp = spacy.blank('clinlp')
 ```
 
 It employs some custom rule based logic, including:
 - Clinical text-specific logic for splitting punctuation, units, dosages (e.g. `20mg/dag` :arrow_right: `20` `mg` `/` `dag`)
 - Custom lists of abbreviations, units (e.g. `pt.`, `zn.`, `mmHg`)
 - Custom tokenizing rules (e.g. `xdd` :arrow_right: `x` `dd`)
 - Regarding [DEDUCE](https://github.com/vmenger/deduce) tags as a single token (e.g. `[DATUM-1]`). 
   - Deidentification is not builtin `clinlp` and should be done as a preprocessing step.
 
+### Normalizer
+
+The normalizer sets the `token.norm` attribute, which can be used by further components (entity recognition, qualification) for matching. It currently has two options (enabled by default):
+- Lowercasing
+- Removing diacritings, where possible. For instance, it will map `ë` `->` `e`, but keeps most other non-ascii characters intact (e.g. `µ`, `²`).
+
+Note that this component only has effect when explicitly configuring successor components to match on the `token.norm` attribute. 
+
 ### Sentence splitter
 
 The sentence splitter can be added as follows:
 
 ```python
 nlp.add_pipe('clinlp_sentencizer')
 ```
 
 It is designed to detect sentence boundaries in clinical text, whenever a character that demarks a sentence ending is matched (e.g. newline, period, question mark). It also correctly detects items in an enumerations (e.g. starting with `-` or `*`). 
 
 ### Entity matcher
 
-Currently, the spaCy builtin `PhraseMatcher` and `Matcher` can be used for finding (named) entities in text. The first one accepts literal phrases only, that are matched in the tokenized text, while the second only also accepts [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns). These are not tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained.
+Currently, the spaCy builtin `PhraseMatcher` and `Matcher` can be used for finding (named) entities in text. The first one accepts literal phrases only, that are matched in the tokenized text, while the second one also accepts [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns). These are not tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained.
 
 For instance, a matcher that helps recognize COVID19 symptoms:
 
 ```python
-ruler = nlp.add_pipe('entity_ruler')
+ruler = nlp.add_pipe('entity_ruler', config={'phrase_matcher_attr': "NORM"})
 
 terms = {
     'covid_19_symptomen': [
         'verkouden', 'neusverkouden', 'loopneus', 'niezen', 
         'keelpijn', 'hoesten', 'benauwd', 'kortademig', 'verhoging', 
         'koorts', 'verlies van reuk', 'verlies van smaak'
     ]
@@ -186,15 +177,15 @@
 ### Context detection
 
 After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) for this purpose. This algorithm is fairly accurate, and quite transparent and fast. Better solutions will hopefully be added to `clinlp` in the future. 
 
 A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
 
 ```python
-nlp.add_pipe('clinlp_context_matcher')
+nlp.add_pipe('clinlp_context_matcher', config={'phrase_matcher_attr': 'NORM'})
 ```
 
 A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows: 
 
 ```python
 from clinlp.component.qualifier import parse_rules
```

