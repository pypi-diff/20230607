# Comparing `tmp/event2vec-0.0.32.tar.gz` & `tmp/event2vec-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event2vec-0.0.32.tar", max compression
+gzip compressed data, was "event2vec-0.0.33.tar", max compression
```

## Comparing `event2vec-0.0.32.tar` & `event2vec-0.0.33.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.32/LICENSE
--rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.32/README.md
--rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.32/bin/config.cfg
--rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.32/bin/submit_i2b2.py
--rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.32/bin/submit_omop.py
--rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.32/event2vec/__init__.py
--rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.32/event2vec/concept_proximity.py
--rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.32/event2vec/config.py
--rw-r--r--   0        0        0     3999 2023-04-21 19:54:05.145765 event2vec-0.0.32/event2vec/cooccurrence_matrix_pandas.py
--rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.32/event2vec/cooccurrence_matrix_spark.py
--rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.32/event2vec/datasets.py
--rw-r--r--   0        0        0    20149 2023-05-26 19:09:13.964381 event2vec-0.0.32/event2vec/event_transformer.py
--rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.32/event2vec/nomenclatures.py
--rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.32/event2vec/svd_ppmi.py
--rw-r--r--   0        0        0     2040 2023-05-25 20:07:29.250350 event2vec-0.0.32/event2vec/utils.py
--rw-r--r--   0        0        0     4603 2023-05-26 19:14:04.514315 event2vec-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 event2vec-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0    15731 2023-03-14 22:29:01.448203 event2vec-0.0.33/LICENSE
+-rw-r--r--   0        0        0      762 2023-03-14 22:29:01.448203 event2vec-0.0.33/README.md
+-rw-r--r--   0        0        0      242 2023-03-14 22:29:01.448203 event2vec-0.0.33/bin/config.cfg
+-rw-r--r--   0        0        0     5993 2023-04-21 19:43:26.765843 event2vec-0.0.33/bin/submit_i2b2.py
+-rw-r--r--   0        0        0     5384 2023-04-21 19:43:24.325844 event2vec-0.0.33/bin/submit_omop.py
+-rw-r--r--   0        0        0       17 2023-03-14 22:29:01.778203 event2vec-0.0.33/event2vec/__init__.py
+-rw-r--r--   0        0        0     1148 2023-03-14 22:29:01.778203 event2vec-0.0.33/event2vec/concept_proximity.py
+-rw-r--r--   0        0        0     1411 2023-05-25 16:23:01.245183 event2vec-0.0.33/event2vec/config.py
+-rw-r--r--   0        0        0     5203 2023-05-31 16:16:31.163153 event2vec-0.0.33/event2vec/cooccurrence_matrix_pandas.py
+-rw-r--r--   0        0        0     7099 2023-04-22 02:17:00.822933 event2vec-0.0.33/event2vec/cooccurrence_matrix_spark.py
+-rw-r--r--   0        0        0     1818 2023-05-25 19:08:52.021601 event2vec-0.0.33/event2vec/datasets.py
+-rw-r--r--   0        0        0    20190 2023-06-07 15:53:22.497176 event2vec-0.0.33/event2vec/event_transformer.py
+-rw-r--r--   0        0        0     6425 2023-03-14 22:29:01.778203 event2vec-0.0.33/event2vec/nomenclatures.py
+-rw-r--r--   0        0        0     6867 2023-05-25 20:21:37.250039 event2vec-0.0.33/event2vec/svd_ppmi.py
+-rw-r--r--   0        0        0     2040 2023-05-25 20:07:29.250350 event2vec-0.0.33/event2vec/utils.py
+-rw-r--r--   0        0        0     4603 2023-06-07 16:14:27.367068 event2vec-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 event2vec-0.0.33/PKG-INFO
```

### Comparing `event2vec-0.0.32/LICENSE` & `event2vec-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/README.md` & `event2vec-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/bin/submit_i2b2.py` & `event2vec-0.0.33/bin/submit_i2b2.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/bin/submit_omop.py` & `event2vec-0.0.33/bin/submit_omop.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/concept_proximity.py` & `event2vec-0.0.33/event2vec/concept_proximity.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/config.py` & `event2vec-0.0.33/event2vec/config.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/cooccurrence_matrix_pandas.py` & `event2vec-0.0.33/event2vec/cooccurrence_matrix_pandas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import json
 import os
-from datetime import datetime
-from itertools import chain
 from pathlib import Path
 from typing import Dict, Tuple
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 from scipy.sparse import csr_matrix, save_npz
 from sklearn.feature_extraction.text import CountVectorizer
 
+from event2vec.config import COLNAME_PERSON
 from event2vec.utils import (
     WINDOW_BACKWARD_LABEL,
     WINDOW_CENTER_LABEL,
     _get_window,
 )
 
 
 def build_cooccurrence_matrix_pd(
     events: pd.DataFrame,
     output_dir: str = None,
     radius_in_days: int = 30,
     window_orientation: str = "center",
     colname_concept: str = "event_source_concept_id",
+    max_patients_by_block: int = 10000,
 ) -> Tuple[np.array, np.array, Dict]:
     """
     Pandas method for building the cooccurrence matrix in-memory.
 
     Parameters
     ----------
     events : DataFrame
@@ -56,55 +56,89 @@
         center = True
     elif window_orientation == WINDOW_BACKWARD_LABEL:
         center = False
     else:
         raise ValueError(
             f"Choose window_orientation in {[WINDOW_CENTER_LABEL, WINDOW_BACKWARD_LABEL]}"
         )
-    events_sorted = events.sort_values(["person_id", "start"])
-    events_in_window = events_sorted.groupby("person_id")[
-        [colname_concept, "start"]
-    ].rolling(
-        on="start", window=str(window) + "D", center=center, closed="both"
-    )
-    sep_tok = "<SEP>"
-    windowed_events = [
-        sep_tok.join(w.tolist()) for w in events_in_window[colname_concept]
-    ]
-    # TODO: we can do better than joining the word and then making the
-    # countvectorizer split them. Eg. build a dummy analyzer that does nothing
-    transformer = CountVectorizer(analyzer=lambda x: x.split(sep_tok))
-    logger.info("Fit, transform events with count vectorizer model")
-    sparse_counts = transformer.fit_transform(windowed_events)
-    logger.info(f"Vocabulary of length {len(transformer.vocabulary_)}")
-    encoder = transformer.vocabulary_
-    vocabulary_size = len(encoder.keys())
-    # TODO: is it less efficient than a join ?
-    context_encoded = (
-        events_sorted[colname_concept].apply(lambda x: encoder[x]).values
-    )
-    n_words = sparse_counts.sum(axis=0)
-    n_contexts = np.unique(context_encoded, return_counts=True)[1]
-    # use ultra fast sparse matrix product
-    rows = np.arange(len(context_encoded))
-    cols = context_encoded
-    values = np.ones(len(context_encoded))
-    context_matrix = csr_matrix(
-        (values, (rows, cols)),
-        shape=(len(context_encoded), vocabulary_size),
-    ).transpose()
-    sparse_cooccurrence = context_matrix.dot(sparse_counts)
-    # Have to withdraw the diagonal to avoid double counting
-    cooccurrence_matrix = sparse_cooccurrence - csr_matrix(np.diag(n_contexts))
+    vocabulary_ = events[colname_concept].unique()
+    unique_patients = events.person_id.unique()
+    n_blocks = len(unique_patients) // max_patients_by_block
+    if n_blocks == 0:
+        n_blocks = 1
+    # iterate over patient blocks
+    full_coocurrence_matrix = csr_matrix((len(vocabulary_), len(vocabulary_)))
+    for block_id in range(n_blocks):
+        if block_id != n_blocks - 1:
+            block_patients = unique_patients[
+                block_id
+                * max_patients_by_block : (block_id + 1)
+                * max_patients_by_block
+            ]
+        else:
+            block_patients = unique_patients[
+                block_id * max_patients_by_block :
+            ]
+        block_events = events.merge(
+            pd.DataFrame({COLNAME_PERSON: block_patients}),
+            how="inner",
+            on=COLNAME_PERSON,
+        )
+        events_sorted = block_events.sort_values(["person_id", "start"])
+        events_in_window = events_sorted.groupby("person_id")[
+            [colname_concept, "start"]
+        ].rolling(
+            on="start", window=str(window) + "D", center=center, closed="both"
+        )
+        sep_tok = "<SEP>"
+        windowed_events = [
+            sep_tok.join(w.tolist()) for w in events_in_window[colname_concept]
+        ]
+        # TODO: we can do better than joining the word and then making the
+        # countvectorizer split them. Eg. build a dummy analyzer that does nothing
+        transformer = CountVectorizer(
+            analyzer=lambda x: x.split(sep_tok),
+            vocabulary=vocabulary_,
+            lowercase=False,
+        )
+        sparse_counts = transformer.fit_transform(windowed_events)
+        encoder = transformer.vocabulary_
+        vocabulary_size = len(encoder.keys())
+        context_encoded = (
+            events_sorted[colname_concept].apply(lambda x: encoder[x]).values
+        )
+        # use fast sparse matrix product to sum each occurrence by context
+        rows = np.arange(len(context_encoded))
+        cols = context_encoded
+        values = np.ones(len(context_encoded))
+        context_matrix = csr_matrix(
+            (values, (rows, cols)),
+            shape=(len(context_encoded), vocabulary_size),
+        ).transpose()
+        sparse_cooccurrence = context_matrix.dot(sparse_counts)
+        # Have to withdraw the diagonal to avoid double counting
+        contexts_ix, n_contexts = np.unique(
+            context_encoded, return_counts=True
+        )
+        diagonal_context = csr_matrix(
+            (n_contexts, (contexts_ix, contexts_ix)),
+            shape=(vocabulary_size, vocabulary_size),
+        )
+
+        block_cooccurrence_matrix = sparse_cooccurrence - diagonal_context
+        full_coocurrence_matrix = (
+            full_coocurrence_matrix + block_cooccurrence_matrix
+        )
+
     if output_dir is not None:
         logger.info(
             f"Saving coocurrence_matrix, event_count and vocabulary at {output_dir}"
         )
         Path(output_dir).mkdir(parents=True, exist_ok=True)
         path2matrix = str(Path(output_dir) / "cooccurrence_matrix.npz")
         logger.info(f"Saving cooccurrence matrix as parquet at: {path2matrix}")
-        save_npz(path2matrix, cooccurrence_matrix)
+        save_npz(path2matrix, full_coocurrence_matrix)
 
         with open(os.path.join(output_dir, "vocabulary.json"), "w") as file:
             json.dump(encoder, file)
         np.save(os.path.join(output_dir, "event_count.npy"), n_contexts)
-    return cooccurrence_matrix, n_contexts, encoder
+    return full_coocurrence_matrix, n_contexts, encoder
```

### Comparing `event2vec-0.0.32/event2vec/cooccurrence_matrix_spark.py` & `event2vec-0.0.33/event2vec/cooccurrence_matrix_spark.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/datasets.py` & `event2vec-0.0.33/event2vec/datasets.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/event_transformer.py` & `event2vec-0.0.33/event2vec/event_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         output_dir: str = None,
         colname_code: str = COLNAME_SOURCE_CODE,
         colname_demographics: List[str] = None,
         window_radius_in_days=30,
         window_orientation: str = "center",
         matrix_type: str = "numpy",
         backend="pandas",
-        d: int = 300,
+        d: int = 150,
         smoothing_factor: float = 0.75,
         k: int = 1,
         n_min_events: int = 10,
         decay_half_life_in_days: np.array = np.array([0]),
     ) -> None:
         self.event = event
         self.output_dir = output_dir
@@ -198,20 +198,21 @@
         # order the columns to correspond to the vocabulary.
         self.embedding_ = embedding[self.vocabulary_]
         return self
 
     def transform(self, X: pd.DataFrame) -> np.array:
         # passing the person ids is necessary to aligne make_counts aggregated
         # rows with the person ids in y.
+        X_ = X.reset_index(drop=True)
         X_event = self.event.merge(
-            X[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
+            X_[[COLNAME_PERSON]], on=COLNAME_PERSON, how="inner"
         )
         X_counts = make_counts(
             event=X_event,
-            person_id=X[[COLNAME_PERSON]],
+            person_id=X_[[COLNAME_PERSON]],
             decay_half_life_in_days=self.decay_half_life_in_days,
             vocabulary=self.vocabulary_,
             sparse=True,
         )
         embedding_array_ = sp.csr_matrix(
             self.embedding_[self.vocabulary_].values
         )
@@ -227,15 +228,15 @@
         embedding_dimension = embedding_array_.shape[0]
         for decay_ in self.decay_half_life_in_days:
             for i in range(embedding_dimension):
                 X_embedded_columns.append(f"dim_{i}__decay_{decay_}")
         X_embedded_df = pd.DataFrame(X_embedded, columns=X_embedded_columns)
         if self.static_features_ is not None:
             X_embedded_df = pd.concat(
-                [X[self.static_features_], X_embedded_df], axis=1
+                [X_[self.static_features_], X_embedded_df], axis=1
             )
         return X_embedded_df
 
 
 class Event2vecPretrained(Event2vecFeaturizer):
     def __init__(
         self,
```

### Comparing `event2vec-0.0.32/event2vec/nomenclatures.py` & `event2vec-0.0.33/event2vec/nomenclatures.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/svd_ppmi.py` & `event2vec-0.0.33/event2vec/svd_ppmi.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/event2vec/utils.py` & `event2vec-0.0.33/event2vec/utils.py`

 * *Files identical despite different names*

### Comparing `event2vec-0.0.32/pyproject.toml` & `event2vec-0.0.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event2vec"
-version = "0.0.32"
+version = "0.0.33"
 description = "event2vec"
 authors = ["Matthieu Doutreligne <matt.dout@gmail.com>"]
 license = "EUPL-v1.2"
 readme = "README.md"
 repository = "https://gitlab.com/strayMat/event2vec"
 homepage = "https://gitlab.com/strayMat/event2vec"
 include = ["bin"]
```

### Comparing `event2vec-0.0.32/PKG-INFO` & `event2vec-0.0.33/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event2vec
-Version: 0.0.32
+Version: 0.0.33
 Summary: event2vec
 Home-page: https://gitlab.com/strayMat/event2vec
 License: EUPL-v1.2
 Author: Matthieu Doutreligne
 Author-email: matt.dout@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Intended Audience :: Developers
```

