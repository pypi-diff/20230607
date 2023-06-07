# Comparing `tmp/renard_pipeline-0.0.1.tar.gz` & `tmp/renard-pipeline-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renard_pipeline-0.0.1.tar", max compression
+gzip compressed data, was "renard-pipeline-0.1.0.tar", max compression
```

## Comparing `renard_pipeline-0.0.1.tar` & `renard-pipeline-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0    35149 2021-10-24 09:32:44.395062 renard_pipeline-0.0.1/LICENSE
--rw-r--r--   0        0        0      605 2023-02-07 16:34:12.347929 renard_pipeline-0.0.1/README.md
--rw-r--r--   0        0        0     1123 2023-05-09 20:47:28.681589 renard_pipeline-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      102 2022-01-20 08:10:14.365722 renard_pipeline-0.0.1/renard/gender.py
--rw-r--r--   0        0        0     2610 2023-04-22 14:29:03.111976 renard_pipeline-0.0.1/renard/graph_utils.py
--rw-r--r--   0        0        0      492 2023-01-07 16:22:16.537260 renard_pipeline-0.0.1/renard/nltk_utils.py
--rw-r--r--   0        0        0       35 2022-03-08 09:05:03.844457 renard_pipeline-0.0.1/renard/pipeline/__init__.py
--rw-r--r--   0        0        0    13068 2023-02-27 21:15:53.739021 renard_pipeline-0.0.1/renard/pipeline/characters_extraction.py
--rw-r--r--   0        0        0    19051 2023-04-26 07:22:50.834703 renard_pipeline-0.0.1/renard/pipeline/core.py
--rw-r--r--   0        0        0       44 2022-09-04 16:51:08.022976 renard_pipeline-0.0.1/renard/pipeline/corefs/__init__.py
--rw-r--r--   0        0        0    41569 2023-04-26 07:22:50.834703 renard_pipeline-0.0.1/renard/pipeline/corefs/bert_corefs.py
--rw-r--r--   0        0        0    10113 2023-03-19 20:56:15.562947 renard_pipeline-0.0.1/renard/pipeline/corefs/corefs.py
--rw-r--r--   0        0        0    16507 2023-02-21 11:53:52.947880 renard_pipeline-0.0.1/renard/pipeline/graph_extraction.py
--rw-r--r--   0        0        0     8435 2023-02-07 16:34:12.349929 renard_pipeline-0.0.1/renard/pipeline/ner.py
--rw-r--r--   0        0        0     1148 2023-02-07 16:34:12.349929 renard_pipeline-0.0.1/renard/pipeline/preconfigured.py
--rw-r--r--   0        0        0      848 2022-01-21 10:08:35.776619 renard_pipeline-0.0.1/renard/pipeline/preprocessing.py
--rw-r--r--   0        0        0     1684 2023-01-07 16:22:16.537260 renard_pipeline-0.0.1/renard/pipeline/progress.py
--rw-r--r--   0        0        0     1489 2023-01-07 16:22:16.537260 renard_pipeline-0.0.1/renard/pipeline/sentiment_analysis.py
--rw-r--r--   0        0        0     8048 2022-11-21 22:36:54.771428 renard_pipeline-0.0.1/renard/pipeline/stanford_corenlp.py
--rw-r--r--   0        0        0     5708 2023-02-07 16:34:12.349929 renard_pipeline-0.0.1/renard/pipeline/tokenization.py
--rw-r--r--   0        0        0     1895 2023-03-19 20:56:15.562947 renard_pipeline-0.0.1/renard/plot_utils.py
--rw-r--r--   0        0        0       55 2022-01-10 23:56:26.787317 renard_pipeline-0.0.1/renard/resources/hypocorisms/__init__.py
--rw-r--r--   0        0        0    11357 2022-01-10 15:42:43.716925 renard_pipeline-0.0.1/renard/resources/hypocorisms/datas/License.txt
--rw-r--r--   0        0        0    21470 2022-01-10 15:37:01.757761 renard_pipeline-0.0.1/renard/resources/hypocorisms/datas/hypocorisms.csv
--rw-r--r--   0        0        0     2319 2022-09-04 14:54:07.277083 renard_pipeline-0.0.1/renard/resources/hypocorisms/hypocorisms.py
--rw-r--r--   0        0        0       49 2022-01-20 08:10:14.365722 renard_pipeline-0.0.1/renard/resources/pronouns/__init__.py
--rw-r--r--   0        0        0      278 2022-01-20 08:10:14.365722 renard_pipeline-0.0.1/renard/resources/pronouns/pronouns.py
--rw-r--r--   0        0        0     2341 2023-02-21 12:25:20.939086 renard_pipeline-0.0.1/renard/utils.py
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 renard_pipeline-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-10-25 08:27:36.755236 renard-pipeline-0.1.0/LICENSE
+-rw-r--r--   0        0        0      700 2023-05-31 07:53:15.539674 renard-pipeline-0.1.0/README.md
+-rw-r--r--   0        0        0     1123 2023-06-07 13:32:37.283051 renard-pipeline-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2022-01-19 13:39:41.879749 renard-pipeline-0.1.0/renard/gender.py
+-rw-r--r--   0        0        0     5024 2023-05-31 07:53:15.607676 renard-pipeline-0.1.0/renard/graph_utils.py
+-rw-r--r--   0        0        0      977 2023-05-31 07:53:15.615676 renard-pipeline-0.1.0/renard/nltk_utils.py
+-rw-r--r--   0        0        0       35 2022-03-03 16:21:22.838555 renard-pipeline-0.1.0/renard/pipeline/__init__.py
+-rw-r--r--   0        0        0    13433 2023-06-07 11:43:03.784802 renard-pipeline-0.1.0/renard/pipeline/characters_extraction.py
+-rw-r--r--   0        0        0    20200 2023-05-31 09:38:26.059941 renard-pipeline-0.1.0/renard/pipeline/core.py
+-rw-r--r--   0        0        0       44 2022-09-05 14:31:10.104789 renard-pipeline-0.1.0/renard/pipeline/corefs/__init__.py
+-rw-r--r--   0        0        0    41569 2023-04-24 15:18:54.568236 renard-pipeline-0.1.0/renard/pipeline/corefs/bert_corefs.py
+-rw-r--r--   0        0        0    10113 2023-03-01 15:12:59.804044 renard-pipeline-0.1.0/renard/pipeline/corefs/corefs.py
+-rw-r--r--   0        0        0    15477 2023-05-31 09:18:44.562058 renard-pipeline-0.1.0/renard/pipeline/graph_extraction.py
+-rw-r--r--   0        0        0     8470 2023-05-31 07:53:15.615676 renard-pipeline-0.1.0/renard/pipeline/ner.py
+-rw-r--r--   0        0        0     1151 2023-05-31 09:18:47.390107 renard-pipeline-0.1.0/renard/pipeline/preconfigured.py
+-rw-r--r--   0        0        0      848 2022-02-02 08:44:12.496752 renard-pipeline-0.1.0/renard/pipeline/preprocessing.py
+-rw-r--r--   0        0        0     1684 2023-01-23 10:04:47.830213 renard-pipeline-0.1.0/renard/pipeline/progress.py
+-rw-r--r--   0        0        0     1489 2023-01-23 10:04:47.862214 renard-pipeline-0.1.0/renard/pipeline/sentiment_analysis.py
+-rw-r--r--   0        0        0     8048 2023-01-05 16:45:44.628245 renard-pipeline-0.1.0/renard/pipeline/stanford_corenlp.py
+-rw-r--r--   0        0        0     5707 2023-05-31 07:53:15.627676 renard-pipeline-0.1.0/renard/pipeline/tokenization.py
+-rw-r--r--   0        0        0     1931 2023-05-31 08:57:09.607082 renard-pipeline-0.1.0/renard/plot_utils.py
+-rw-r--r--   0        0        0       55 2022-01-19 09:47:58.225041 renard-pipeline-0.1.0/renard/resources/hypocorisms/__init__.py
+-rw-r--r--   0        0        0    11357 2022-01-19 09:47:58.225041 renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/License.txt
+-rw-r--r--   0        0        0    21470 2022-01-19 09:47:58.225041 renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/hypocorisms.csv
+-rw-r--r--   0        0        0     2720 2023-06-07 09:42:15.373329 renard-pipeline-0.1.0/renard/resources/hypocorisms/hypocorisms.py
+-rw-r--r--   0        0        0       49 2022-01-19 13:45:56.740454 renard-pipeline-0.1.0/renard/resources/pronouns/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-07 11:33:32.869182 renard-pipeline-0.1.0/renard/resources/pronouns/pronouns.py
+-rw-r--r--   0        0        0       45 2023-06-07 11:30:57.743062 renard-pipeline-0.1.0/renard/resources/titles/__init__.py
+-rw-r--r--   0        0        0      987 2023-06-07 11:40:28.186772 renard-pipeline-0.1.0/renard/resources/titles/titles.py
+-rw-r--r--   0        0        0     3459 2023-05-31 13:00:52.411873 renard-pipeline-0.1.0/renard/utils.py
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 renard-pipeline-0.1.0/setup.py
+-rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 renard-pipeline-0.1.0/PKG-INFO
```

### Comparing `renard_pipeline-0.0.1/LICENSE` & `renard-pipeline-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/pyproject.toml` & `renard-pipeline-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "renard-pipeline"
-version = "0.0.1"
+version = "0.1.0"
 description = "Relationships Extraction from NARrative Documents"
 authors = ["Arthur Amalvy <arthur.amalvy@univ-avignon.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "renard" }
 ]
```

### Comparing `renard_pipeline-0.0.1/renard/pipeline/characters_extraction.py` & `renard-pipeline-0.1.0/renard/pipeline/characters_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import re
 from itertools import combinations
 from collections import defaultdict, Counter
 from dataclasses import dataclass
 from nameparser import config
 from nameparser import HumanName
 from renard.gender import Gender
-from renard.pipeline.ner import NEREntity, ner_entities
+from renard.pipeline.ner import ner_entities
 from renard.pipeline.core import Mention, PipelineStep
+from renard.pipeline.progress import ProgressReporter
 from renard.resources.hypocorisms import HypocorismGazetteer
-from renard.resources.pronouns.pronouns import is_a_female_pronoun, is_a_male_pronoun
+from renard.resources.pronouns import is_a_female_pronoun, is_a_male_pronoun
+from renard.resources.titles import is_a_male_title, is_a_female_title
 
 
 @dataclass(eq=True, frozen=True)
 class Character:
 
     names: FrozenSet[str]
     mentions: List[Mention]
@@ -169,22 +171,30 @@
             character for it to be extracted.
         :param additional_hypocorisms: a tuple of additional
             hypocorisms.  Each hypocorism is a tuple where the first
             element is a name, and the second element is a set of
             nicknames associated with it
         """
         self.min_appearances = min_appearances
-
-        self.hypocorism_gazetteer = HypocorismGazetteer()
-        if not additional_hypocorisms is None:
-            for name, nicknames in additional_hypocorisms:
-                self.hypocorism_gazetteer._add_hypocorism_(name, nicknames)
+        self.additional_hypocorisms = additional_hypocorisms
 
         super().__init__()
 
+    def _pipeline_init_(self, lang: str, progress_reporter: ProgressReporter):
+
+        if lang in HypocorismGazetteer.supported_langs:
+            self.hypocorism_gazetteer = HypocorismGazetteer(lang=lang)
+            if not self.additional_hypocorisms is None:
+                for name, nicknames in self.additional_hypocorisms:
+                    self.hypocorism_gazetteer._add_hypocorism_(name, nicknames)
+        else:
+            self.hypocorism_gazetteer = None
+
+        return super()._pipeline_init_(lang, progress_reporter)
+
     def __call__(
         self,
         tokens: List[str],
         bio_tags: List[str],
         corefs: Optional[List[List[Mention]]] = None,
         **kwargs: dict,
     ) -> Dict[str, Any]:
@@ -201,17 +211,18 @@
         for mention_str in mentions_str:
             G.add_node(mention_str)
 
         # * link nodes based on several rules
         for (name1, name2) in combinations(G.nodes(), 2):
 
             # is one name a known hypocorism of the other ?
-            if self.hypocorism_gazetteer.are_related(name1, name2):
-                G.add_edge(name1, name2)
-                continue
+            if not self.hypocorism_gazetteer is None:
+                if self.hypocorism_gazetteer.are_related(name1, name2):
+                    G.add_edge(name1, name2)
+                    continue
 
             # if we remove the title, is one name related to the other
             # ?
             if self.names_are_related_after_title_removal(name1, name2):
                 G.add_edge(name1, name2)
                 continue
 
@@ -308,14 +319,16 @@
         return {"characters": characters}
 
     def names_are_related_after_title_removal(self, name1: str, name2: str) -> bool:
         config.CONSTANTS.string_format = "{first} {middle} {last}"
         raw_name1 = HumanName(name1).full_name
         raw_name2 = HumanName(name2).full_name
 
+        if self.hypocorism_gazetteer is None:
+            return raw_name1 == raw_name2
         return raw_name1 == raw_name2 or self.hypocorism_gazetteer.are_related(
             raw_name1, raw_name2
         )
 
     def names_are_in_coref(self, name1: str, name2: str, corefs: List[List[Mention]]):
         for coref_chain in corefs:
             if any([name1 == " ".join(m.tokens) for m in coref_chain]) and any(
@@ -323,30 +336,19 @@
             ):
                 return True
         return False
 
     def infer_name_gender(self, name: str, corefs: List[List[Mention]]) -> Gender:
         """Try to infer a name's gender"""
         # 1. try to infer gender based on honorifics
-        #    TODO: add more gendered honorifics to renard.resources
         title = HumanName(name).title
         if title != "":
-            if any(
-                [
-                    re.match(pattern, title)
-                    for pattern in (r"[Mm]r\.?", r"[Mm]\.?", r"[Ss]ir", r"[Ll]ord")
-                ]
-            ):
+            if is_a_male_title(title, lang=self.lang):
                 return Gender.MALE
-            elif any(
-                [
-                    re.match(pattern, title)
-                    for pattern in (r"[Mm]iss", r"[Mm]r?s\.?", r"[Ll]ady")
-                ]
-            ):
+            elif is_a_female_title(title, lang=self.lang):
                 return Gender.FEMALE
 
         # 2. if 1. didn't succeed, inspect coreferences chain
         #    to see if if the name was coreferent with a
         #    gendered pronoun
         female_count = 0
         male_count = 0
@@ -367,9 +369,12 @@
 
     def needs(self) -> Set[str]:
         return {"tokens", "bio_tags"}
 
     def optional_needs(self) -> Set[str]:
         return {"corefs"}
 
+    def supported_langs(self) -> Union[Set[str], Literal["any"]]:
+        return {"eng", "fra"}
+
     def production(self) -> Set[str]:
         return {"characters"}
```

### Comparing `renard_pipeline-0.0.1/renard/pipeline/core.py` & `renard-pipeline-0.1.0/renard/pipeline/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,26 @@
     Optional,
     Union,
     TypeVar,
     Type,
     TYPE_CHECKING,
 )
 import os
-from torch._C import Value
 
-from tqdm import tqdm
 from transformers.tokenization_utils_base import BatchEncoding
 import networkx as nx
-from renard.pipeline.progress import ProgressReporter, get_progress_reporter, progress_
+from networkx.readwrite.gexf import GEXFWriter
 
+from renard.pipeline.progress import ProgressReporter, get_progress_reporter, progress_
 from renard.plot_utils import plot_nx_graph_reasonably, layout_nx_graph_reasonably
-from renard.graph_utils import cumulative_graph, graph_with_names
+from renard.graph_utils import (
+    cumulative_graph,
+    graph_with_names,
+    dynamic_graph_to_gephi_graph,
+)
 
 if TYPE_CHECKING:
     from renard.pipeline.characters_extraction import Character
     import matplotlib.pyplot as plt
 
 
 @dataclass
@@ -218,20 +221,40 @@
     ):
         """Export characters graph to Gephi's gexf format
 
         :param path: export file path
         :param name_style: see :func:`.graph_with_names`
             for more details
         """
-        if not isinstance(self.characters_graph, nx.Graph):
-            raise RuntimeError(
-                f"characters graph cant be exported : {self.characters_graph}"
+        path = os.path.expanduser(path)
+        if isinstance(self.characters_graph, list):
+            G = dynamic_graph_to_gephi_graph(self.characters_graph)
+            G = graph_with_names(G, name_style)
+            # HACK: networkx cannot set a dynamic "weight" attribute
+            # in gexf since "weight" has a specific meaning in
+            # networkx. the following code hacks the XML tree
+            # outputted by GEXFWriter to force the attribute name to
+            # be "weight" (instead of "dweight", as outputted by
+            # dynamic_graph_to_gephi_graph)
+            writer = GEXFWriter()
+            writer.add_graph(G)
+            attribute_dweight = writer.xml.find(
+                ".//graph/attributes/attribute[@title='dweight']"
             )
-        G = graph_with_names(self.characters_graph, name_style)
-        nx.write_gexf(G, path)
+            dweight_old_id = attribute_dweight.get("id")
+            attribute_dweight.set("id", "weight")
+            attribute_dweight.set("title", "Weight")
+            for attvalue in writer.xml.findall(
+                f".//graph/edges/edge/attvalues/attvalue[@for='{dweight_old_id}']"
+            ):
+                attvalue.set("for", "weight")
+            writer.write(path)
+        else:
+            G = graph_with_names(self.characters_graph, name_style)
+            nx.write_gexf(G, path)
 
     def plot_graphs_to_dir(
         self,
         directory: str,
         name_style: Union[
             Literal["longest", "shortest", "most_frequent"], Callable[[Character], str]
         ] = "longest",
@@ -254,14 +277,15 @@
         import matplotlib.pyplot as plt
 
         assert not self.characters_graph is None
         if isinstance(self.characters_graph, nx.Graph):
             raise ValueError("this function is supposed to be used on a dynamic graph")
 
         directory = directory.rstrip("/")
+        directory = os.path.expanduser(directory)
         os.makedirs(directory, exist_ok=True)
 
         graphs = self.characters_graph
         if cumulative:
             graphs = cumulative_graph(self.characters_graph)
 
         layout = None
@@ -269,19 +293,20 @@
             layout_graph = (
                 graphs[-1]
                 if cumulative
                 else cumulative_graph(self.characters_graph)[-1]
             )
             layout = layout_nx_graph_reasonably(graph_with_names(layout_graph))
 
-        for i, G in enumerate(self.characters_graph):
+        for i, G in enumerate(graphs):
             fig, ax = plt.subplots()
             G = graph_with_names(G, name_style=name_style)
             plot_nx_graph_reasonably(G, ax=ax, layout=layout)
             plt.savefig(f"{directory}/{i}.png")
+            plt.close()
 
     def plot_graph_to_file(
         self,
         path: str,
         name_style: Union[
             Literal["longest", "shortest", "most_frequent"], Callable[[Character], str]
         ] = "longest",
@@ -297,14 +322,15 @@
         assert not self.characters_graph is None
         if isinstance(self.characters_graph, list):
             raise ValueError("this function is supposed to be used on a static graph")
 
         G = graph_with_names(self.characters_graph, name_style=name_style)
         plot_nx_graph_reasonably(G)
         plt.savefig(path)
+        plt.close()
 
     def plot_graph(
         self,
         name_style: Union[
             Literal["longest", "shortest", "most_frequent"], Callable[[Character], str]
         ] = "longest",
         fig: Optional[plt.Figure] = None,
@@ -464,15 +490,14 @@
 
         pipeline_state = set(args).union({"text"})
         warnings = []
 
         steps = self._non_ignored_steps(ignored_steps)
 
         for i, step in enumerate(steps):
-
             if not step.needs().issubset(pipeline_state):
                 return (
                     False,
                     [
                         f"step {i + 1} ({step.__class__.__name__}) has unsatisfied needs (needs : {step.needs()}, available : {pipeline_state})"
                     ],
                 )
@@ -483,15 +508,18 @@
                 )
 
             pipeline_state = pipeline_state.union(step.production())
 
         return (True, warnings)
 
     def __call__(
-        self, text: Optional[str], ignored_steps: Optional[List[str]] = None, **kwargs
+        self,
+        text: Optional[str] = None,
+        ignored_steps: Optional[List[str]] = None,
+        **kwargs,
     ) -> PipelineState:
         """Run the pipeline sequentially.
 
         :param ignored_steps: a list of steps production.  All steps
             with a production in ``ignored_steps`` will be ignored.
 
         :return: the output of the last step of the pipeline
@@ -508,15 +536,14 @@
         self._pipeline_init_steps(ignored_steps)
 
         state = PipelineState(text, **kwargs)
 
         steps = self._non_ignored_steps(ignored_steps)
 
         for step in progress_(self.progress_reporter, steps):
-
             self.progress_reporter.update_message_(f"{step.__class__.__name__}")
 
             out = step(**state.__dict__)
             for key, value in out.items():
                 setattr(state, key, value)
 
         return state
```

### Comparing `renard_pipeline-0.0.1/renard/pipeline/corefs/bert_corefs.py` & `renard-pipeline-0.1.0/renard/pipeline/corefs/bert_corefs.py`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/pipeline/corefs/corefs.py` & `renard-pipeline-0.1.0/renard/pipeline/corefs/corefs.py`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/pipeline/graph_extraction.py` & `renard-pipeline-0.1.0/renard/pipeline/graph_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,74 +63,64 @@
     return [
         m
         for m in mentions
         if m[1].start_idx >= chapter_start_idx and m[1].end_idx <= chapter_end_idx
     ]
 
 
-class CoOccurencesGraphExtractor(PipelineStep):
+class CoOccurrencesGraphExtractor(PipelineStep):
     """A simple character graph extractor using co-occurences"""
 
     def __init__(
         self,
         co_occurences_dist: Union[int, Tuple[int, Literal["tokens", "sentences"]]],
-        dynamic: Optional[Literal["nx", "gephi"]] = None,
+        dynamic: bool = False,
         dynamic_window: Optional[int] = None,
         dynamic_overlap: int = 0,
     ) -> None:
         """
         :param co_occurences_dist: max accepted distance between two
             character appearances to form a co-occurence interaction.
 
                 - if an ``int`` is given, the distance is in number of
                   tokens
 
                 - if a ``tuple`` is given, the first element of the
                   tuple is a distance while the second is an unit.
                   Examples : ``(1, "sentences")``, ``(3, "tokens")``.
 
-        :param dynamic: either ``None``, or one of ``{'nx', 'gephi'}``
+        :param dynamic:
 
-                - if ``None`` (the default), a ``nx.graph`` is
-                  extracted
+            - if ``False`` (the default), a static ``nx.graph`` is
+              extracted
 
-                - if ``'nx'``, several ``nx.graph`` are extracted.  In
-                  that case, ``dynamic_window`` and
-                  ``dynamic_overlap``*can* be specified.  If
-                  ``dynamic_window`` is not specified, this step is
-                  expecting the text to be cut into chapters', and a
-                  graph will be extracted for each 'chapter'.  In that
-                  case, ``chapters`` must be passed to the pipeline as
-                  a ``List[str]`` at runtime.
-
-                - if ``'gephi'``, a single ``nx.graph`` is extracted.
-                  This graph has the nice property that exporting it
-                  to `gexf` format using ``G.write_gexf()`` will
-                  produce a correct dynamic graph that can be read by
-                  Gephi.  Because of a limitation in networkx, the
-                  dynamic weight attribute is stored as ``dweight``
-                  instead of ``weight``.
+            - if ``True``, several ``nx.graph`` are extracted.  In
+              that case, ``dynamic_window`` and
+              ``dynamic_overlap``*can* be specified.  If
+              ``dynamic_window`` is not specified, this step is
+              expecting the text to be cut into chapters', and a graph
+              will be extracted for each 'chapter'.  In that case,
+              ``chapters`` must be passed to the pipeline as a
+              ``List[str]`` at runtime.
 
         :param dynamic_window: dynamic window, in number of
             interactions.  a dynamic window of `n` means that each
             returned graph will be formed by `n` interactions.
 
         :param dynamic_overlap: overlap, in number of interactions.
         """
 
         if isinstance(co_occurences_dist, int):
             co_occurences_dist = (co_occurences_dist, "tokens")
         self.co_occurences_dist = co_occurences_dist
 
-        if not dynamic is None:
-            assert dynamic in {"nx", "gephi"}
-            if dynamic == "nx":
-                if not dynamic_window is None:
-                    assert dynamic_window > 0
-                    assert dynamic_window > dynamic_overlap
+        if dynamic:
+            if not dynamic_window is None:
+                assert dynamic_window > 0
+                assert dynamic_window > dynamic_overlap
         self.dynamic = dynamic
         self.dynamic_window = dynamic_window
         self.dynamic_overlap = dynamic_overlap
         self.dynamic_needs_chapter = dynamic == "nx" and dynamic_window is None
         super().__init__()
 
     def __call__(
@@ -158,36 +148,25 @@
 
         mentions = []
         for character in characters:
             for mention in character.mentions:
                 mentions.append((character, mention))
         mentions = sorted(mentions, key=lambda cm: cm[1].start_idx)
 
-        if self.dynamic == "gephi":
-            if not sentences_polarities is None:
-                print("[warning] 'gephi' does not support sentence polarities")
-            return {
-                "characters_graph": self._extract_gephi_dynamic_graph(
-                    mentions, sentences
-                )
-            }
-
-        elif self.dynamic == "nx":
+        if self.dynamic:
             return {
                 "characters_graph": self._extract_dynamic_graph(
                     mentions,
                     self.dynamic_window,
                     self.dynamic_overlap,
                     chapter_tokens,
                     sentences,
                     sentences_polarities,
                 )
             }
-
-        # static extraction
         return {
             "characters_graph": self._extract_graph(
                 mentions, sentences, sentences_polarities
             )
         }
 
     def _mentions_interact(
@@ -259,17 +238,15 @@
 
         # * Construct graph from co-occurence matrix
         G = nx.Graph()
         for character, _ in mentions:
             G.add_node(character)
 
         for i, (char1, mention1) in enumerate(mentions):
-
             for j, (char2, mention2) in enumerate(mentions):
-
                 # no co-occurences for these two mentions: we are out
                 if C[i][j] == 0:
                     continue
 
                 if not G.has_edge(char1, char2):
                     G.add_edge(char1, char2, weight=0)
                 G.edges[char1, char2]["weight"] += 1
@@ -328,15 +305,14 @@
             ]
 
         assert not chapter_tokens is None
 
         graphs = []
 
         for chapter_i, chapter in enumerate(chapter_tokens):
-
             # TODO: optim
             chapter_mentions = mentions_for_chapter(chapter_tokens, chapter_i, mentions)
             chapter_start_idx = sum(
                 [len(c) for i, c in enumerate(chapter_tokens) if i < chapter_i]
             )
             # make mentions coordinates chapter local
             chapter_mentions = [
```

### Comparing `renard_pipeline-0.0.1/renard/pipeline/ner.py` & `renard-pipeline-0.1.0/renard/pipeline/ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import List, Dict, Any, Set, Tuple, Optional, Union, Literal
 from dataclasses import dataclass
 from torch._C import Value
 from transformers.tokenization_utils_base import BatchEncoding
 from seqeval.metrics import precision_score, recall_score, f1_score
-from renard.nltk_utils import NLTK_ISO_STRING_TO_LANG
+from renard.nltk_utils import NLTK_ISO_STRING_TO_LANG, nltk_fix_bio_tags
 from renard.pipeline.core import PipelineStep, Mention
 from renard.pipeline.progress import ProgressReporter
 
 
 @dataclass
 class NEREntity(Mention):
     #: NER class (without BIO prefix as in ``PER`` and not ``B-PER``)
@@ -38,15 +38,14 @@
     assert len(tokens) == len(bio_tags)
 
     entities = []
     current_tag: Optional[str] = None
     current_tag_start_idx: Optional[int] = None
 
     for i, tag in enumerate(bio_tags):
-
         if not current_tag is None and not tag.startswith("I-"):
             assert not current_tag_start_idx is None
             entities.append(
                 NEREntity(
                     tokens[current_tag_start_idx:i],
                     current_tag_start_idx,
                     i - 1,
@@ -125,15 +124,15 @@
         """
         import nltk
         from nltk.chunk import tree2conlltags
 
         word_tag_iobtags = tree2conlltags(
             nltk.ne_chunk(nltk.pos_tag(tokens, lang=self.lang))
         )
-        return {"bio_tags": [wti[2] for wti in word_tag_iobtags]}
+        return {"bio_tags": nltk_fix_bio_tags([wti[2] for wti in word_tag_iobtags])}
 
     def supported_langs(self) -> Union[Set[str], Literal["any"]]:
         # POS Tagging only supports english and russian
         return {"eng", "rus"}
 
     def needs(self) -> Set[str]:
         return {"tokens"}
@@ -239,15 +238,15 @@
         of word piece tokens.
 
         :param wp_tokens: word piece tokens
         :param wp_labels: word piece labels
         """
         assert len(wp_tokens) == len(wp_labels)
         labels = []
-        for (wp_token, wp_label) in zip(wp_tokens, wp_labels):
+        for wp_token, wp_label in zip(wp_tokens, wp_labels):
             if wp_token in {"[CLS]", "[SEP]", "[PAD]"}:
                 continue
             if not wp_token.startswith("##"):
                 labels.append(wp_label)
         return labels
 
     def supported_langs(self) -> Union[Set[str], Literal["any"]]:
```

### Comparing `renard_pipeline-0.0.1/renard/pipeline/preconfigured.py` & `renard-pipeline-0.1.0/renard/pipeline/preconfigured.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from renard.pipeline.core import Pipeline
 from renard.pipeline.characters_extraction import GraphRulesCharactersExtractor
-from renard.pipeline.graph_extraction import CoOccurencesGraphExtractor
+from renard.pipeline.graph_extraction import CoOccurrencesGraphExtractor
 
 
 def nltk_pipeline(**kwargs) -> Pipeline:
     from renard.pipeline.tokenization import NLTKTokenizer
     from renard.pipeline.ner import NLTKNamedEntityRecognizer
     from renard.pipeline.sentiment_analysis import NLTKSentimentAnalyzer
 
     return Pipeline(
         [
             NLTKTokenizer(),
             NLTKNamedEntityRecognizer(),
             NLTKSentimentAnalyzer(),
             GraphRulesCharactersExtractor(),
-            CoOccurencesGraphExtractor(co_occurences_dist=(1, "sentences")),
+            CoOccurrencesGraphExtractor(co_occurences_dist=(1, "sentences")),
         ],
         **kwargs
     )
 
 
 def bert_pipeline(**kwargs) -> Pipeline:
     from renard.pipeline.tokenization import BertTokenizer
     from renard.pipeline.ner import BertNamedEntityRecognizer
 
     return Pipeline(
         [
             BertTokenizer(),
             BertNamedEntityRecognizer(),
             GraphRulesCharactersExtractor(),
-            CoOccurencesGraphExtractor(co_occurences_dist=(1, "sentences")),
+            CoOccurrencesGraphExtractor(co_occurences_dist=(1, "sentences")),
         ],
         **kwargs
     )
```

### Comparing `renard_pipeline-0.0.1/renard/pipeline/preprocessing.py` & `renard-pipeline-0.1.0/renard/pipeline/preprocessing.py`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/pipeline/progress.py` & `renard-pipeline-0.1.0/renard/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/pipeline/sentiment_analysis.py` & `renard-pipeline-0.1.0/renard/pipeline/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/pipeline/stanford_corenlp.py` & `renard-pipeline-0.1.0/renard/pipeline/stanford_corenlp.py`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/pipeline/tokenization.py` & `renard-pipeline-0.1.0/renard/pipeline/tokenization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict, Any, List, Optional, Set, Union, Literal
+import itertools
 import torch
 import nltk
 from more_itertools.recipes import flatten
 from renard.pipeline.core import PipelineStep
 from renard.pipeline.progress import ProgressReporter
 from renard.nltk_utils import NLTK_ISO_STRING_TO_LANG
 
@@ -16,40 +17,34 @@
 
     def __call__(
         self, text: str, chapters: Optional[List[str]] = None, **kwargs
     ) -> Dict[str, Any]:
         """
         :param text:
         """
+        if not chapters is None:
+            out_dicts = [self.__call__(chapter, None) for chapter in chapters]
+            return {
+                "tokens": list(itertools.chain([d["tokens"] for d in out_dicts])),
+                "sentences": list(itertools.chain([d["sentences"] for d in out_dicts])),
+                "chapter_tokens": [d["tokens"] for d in out_dicts],
+            }
+
+        sentences = nltk.sent_tokenize(
+            text, language=NLTK_ISO_STRING_TO_LANG[self.lang]
+        )
 
-        if chapters is None:
-            chapters = [text]
-
-        chapters_sentences: List[List[str]] = [
-            nltk.sent_tokenize(c, language=NLTK_ISO_STRING_TO_LANG[self.lang])
-            for c in chapters
-        ]
-
-        sentences = []
         tokens = []
-        chapter_tokens = []
-        for chapter_sentences in self._progress_(chapters_sentences):
-            tokenized_chapter_sentences = [
-                nltk.word_tokenize(s) for s in chapter_sentences
-            ]
-            sentences += tokenized_chapter_sentences
-            flattened_tokens = list(flatten(tokenized_chapter_sentences))
-            tokens += flattened_tokens
-            chapter_tokens.append(flattened_tokens)
+        tokenized_sentences = []
+        for sent in sentences:
+            sent_tokens = nltk.word_tokenize(sent)
+            tokenized_sentences.append(sent_tokens)
+            tokens += sent_tokens
 
-        return {
-            "tokens": tokens,
-            "chapter_tokens": chapter_tokens,
-            "sentences": sentences,
-        }
+        return {"tokens": tokens, "sentences": tokenized_sentences}
 
     def supported_langs(self) -> Union[Set[str], Literal["any"]]:
         return set(NLTK_ISO_STRING_TO_LANG.keys())
 
     def needs(self) -> Set[str]:
         return {"text"}
 
@@ -95,55 +90,50 @@
 
     def __call__(
         self, text: str, chapters: Optional[List[str]] = None, **kwargs
     ) -> Dict[str, Any]:
         """
         :param text:
         """
-        if chapters is None:
-            chapters = [text]
+        if not chapters is None:
+            out_dicts = [self.__call__(chapter, None) for chapter in chapters]
+            out_batchs = [d["bert_batch_encoding"] for d in out_dicts]
+            batchs = out_batchs[0]
+            for b in batchs[1:]:
+                batchs = {k: torch.cat([v, b[k]], dim=0) for k, v in batchs.items()}
+            return {
+                "tokens": list(itertools.chain([d["tokens"] for d in out_dicts])),
+                "sentences": list(itertools.chain([d["sentences"] for d in out_dicts])),
+                "chapter_tokens": [d["tokens"] for d in out_dicts],
+                "wp_tokens": list(itertools.chain([d["tokens"] for d in out_dicts])),
+                "bert_batch_encoding": batchs,
+            }
+
+        # NOTE: it's possible that some input tokens are discarded
+        # here because of truncation.
+        batchs = self.tokenizer(
+            nltk.sent_tokenize(text, language=NLTK_ISO_STRING_TO_LANG[self.lang]),
+            return_tensors="pt",
+            padding=True,
+            truncation=True,
+        )
 
-        chapter_tokens: List[List[str]] = []
-        sentences: List[List[str]] = []
-        wp_tokens: List[str] = []
-        batchs = {}
-
-        for chapter in chapters:
-
-            # NOTE: it's possible that some input tokens are discarded
-            # here because of truncation.
-            batch = self.tokenizer(
-                nltk.sent_tokenize(
-                    chapter, language=NLTK_ISO_STRING_TO_LANG[self.lang]
-                ),
-                return_tensors="pt",
-                padding=True,
-                truncation=True,
-            )
-            if len(batchs) == 0:
-                batchs = batch
-            else:
-                batchs = {k: torch.cat([v, batch[k]], dim=0) for k, v in batch.items()}
+        nested_wp_tokens: List[List[str]] = [
+            batchs.tokens(i) for i in range(len(batchs["input_ids"]))
+        ]
+        wp_tokens = [wp_t for s in nested_wp_tokens for wp_t in s]
 
-            nested_wp_tokens: List[List[str]] = [
-                batch.tokens(i) for i in range(len(batch["input_ids"]))
-            ]
-            chapter_wp_tokens = [wp_t for s in nested_wp_tokens for wp_t in s]
-            wp_tokens += chapter_wp_tokens
-
-            chapter_sentences = [
-                BertTokenizer.wp_tokens_to_tokens(wp_tokens)
-                for wp_tokens in nested_wp_tokens
-            ]
-            chapter_tokens.append(list(flatten(chapter_sentences)))
-            sentences += chapter_sentences
+        sentences = [
+            BertTokenizer.wp_tokens_to_tokens(wp_tokens)
+            for wp_tokens in nested_wp_tokens
+        ]
+        tokens = list(flatten(sentences))
 
         return {
-            "tokens": list(flatten(chapter_tokens)),
-            "chapter_tokens": chapter_tokens,
+            "tokens": tokens,
             "sentences": sentences,
             "bert_batch_encoding": batchs,
             "wp_tokens": wp_tokens,
         }
 
     def supported_langs(self) -> Union[Set[str], Literal["any"]]:
         return {"eng", "fra"}
```

### Comparing `renard_pipeline-0.0.1/renard/plot_utils.py` & `renard-pipeline-0.1.0/renard/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import networkx as nx
 import numpy as np
 import matplotlib.pyplot as plt
 from renard.graph_utils import graph_edges_attributes
 
 
 def layout_nx_graph_reasonably(G: nx.Graph) -> Dict[Any, np.ndarray]:
-    return nx.spring_layout(G, k=0.75 * math.sqrt(len(G.nodes)))  # type: ignore
+    return nx.spring_layout(G, k=2 / math.sqrt(len(G.nodes)))  # type: ignore
 
 
 def plot_nx_graph_reasonably(
     G: nx.Graph, ax=None, layout: Optional[Dict[Any, np.ndarray]] = None
 ):
     """Try to plot a :class:`nx.Graph` with 'reasonable' parameters
 
@@ -52,8 +52,10 @@
         edge_vmax=1,
         edge_vmin=-1,
         width=[1 + math.log(d["weight"]) for _, _, d in G.edges.data()],  # type: ignore
         alpha=0.35,
         ax=ax,
     )
 
-    nx.draw_networkx_labels(G, pos=pos, ax=ax, verticalalignment="top")
+    nx.draw_networkx_labels(
+        G, pos=pos, ax=ax, verticalalignment="top", font_size=8, alpha=0.75
+    )
```

### Comparing `renard_pipeline-0.0.1/renard/resources/hypocorisms/datas/License.txt` & `renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/License.txt`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/resources/hypocorisms/datas/hypocorisms.csv` & `renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/hypocorisms.csv`

 * *Files identical despite different names*

### Comparing `renard_pipeline-0.0.1/renard/resources/hypocorisms/hypocorisms.py` & `renard-pipeline-0.1.0/renard/resources/hypocorisms/hypocorisms.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,25 @@
     .. note::
 
         datas used for this gazeeter come from
         https://github.com/carltonnorthern/nickname-and-diminutive-names-lookup
         and are licensed under the Apache 2.0 License
     """
 
-    def __init__(self):
+    supported_langs = {"eng"}
+
+    def __init__(self, lang: str = "eng"):
+        """
+        :param lang: gazetteer language.  Must be in
+            ``HypocorismGazetteer.supported_langs``.
+        """
+        if not lang in HypocorismGazetteer.supported_langs:
+            raise ValueError(
+                f"{lang} not supported by {type(self)} (supported languages: {HypocorismGazetteer.supported_langs})"
+            )
 
         self.name_to_nicknames = defaultdict(set)
         self.nickname_to_names = defaultdict(set)
 
         with open(f"{script_dir}/datas/hypocorisms.csv") as f:
 
             for line in f:
```

### Comparing `renard_pipeline-0.0.1/renard/utils.py` & `renard-pipeline-0.1.0/renard/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List, Tuple, TypeVar, Collection, Iterable, cast
+from typing import List, Tuple, TypeVar, Collection, Iterable, Optional, Dict, cast
+import re, os
+from more_itertools import flatten
 from more_itertools.more import windowed
 import torch
 
 
 T = TypeVar("T")
 
 
@@ -73,7 +75,42 @@
     :return: a list of patterns start index
     """
     start_indices = []
     for subseq_i, subseq in enumerate(windowed(seq, len(pattern))):
         if list(subseq) == pattern:
             start_indices.append(subseq_i)
     return start_indices
+
+
+def load_conll2002_bio(
+    path: str, tag_conversion_map: Optional[Dict[str, str]] = None
+) -> Tuple[List[List[str]], List[str], List[str]]:
+    """Load a file under CoNLL2022 BIO format.  Sentences are expected
+    to be separated by end of lines.
+
+    :param path: path to the CoNLL-2002 formatted file
+    :param tag_conversion_map: conversion map for tags found in the
+        input file. Example : ``{'B': 'B-PER', 'I': 'I-PER'}``
+
+    :return: ``(sentences, tokens, tag)``
+    """
+
+    if tag_conversion_map is None:
+        tag_conversion_map = {}
+
+    with open(os.path.expanduser(path)) as f:
+        raw_data = f.read()
+
+    sents = []
+    sent_tokens = []
+    tags = []
+    for line in raw_data.split("\n"):
+        line = line.strip("\n")
+        if re.fullmatch(r"\s*", line):
+            sents.append(sent_tokens)
+            sent_tokens = []
+            continue
+        token, tag = line.split("\t")
+        sent_tokens.append(token)
+        tags.append(tag_conversion_map.get(tag, tag))
+
+    return sents, list(flatten(sents)), tags
```

### Comparing `renard_pipeline-0.0.1/PKG-INFO` & `renard-pipeline-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 Metadata-Version: 2.1
 Name: renard-pipeline
-Version: 0.0.1
+Version: 0.1.0
 Summary: Relationships Extraction from NARrative Documents
 License: GPL-3.0-only
 Author: Arthur Amalvy
 Author-email: arthur.amalvy@univ-avignon.fr
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: spacy
 Provides-Extra: stanza
-Requires-Dist: coreferee (>=1.4.0,<2.0.0) ; extra == "spacy"
+Requires-Dist: coreferee (>=1.4.0,<2.0.0); extra == "spacy"
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: more-itertools (>=8.12.0,<9.0.0)
 Requires-Dist: nameparser (>=1.1.0,<2.0.0)
 Requires-Dist: networkx (>=2.6.3,<3.0.0)
 Requires-Dist: nltk (>=3.6.5,<4.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: seqeval (==1.2.2)
-Requires-Dist: spacy (>=3.5.0,<4.0.0) ; extra == "spacy"
-Requires-Dist: spacy-transformers (>=1.2.1,<2.0.0) ; extra == "spacy"
-Requires-Dist: stanza (>=1.3.0,<2.0.0) ; extra == "stanza"
+Requires-Dist: spacy (>=3.5.0,<4.0.0); extra == "spacy"
+Requires-Dist: spacy-transformers (>=1.2.1,<2.0.0); extra == "spacy"
+Requires-Dist: stanza (>=1.3.0,<2.0.0); extra == "stanza"
 Requires-Dist: torch (>=1.10.2,<2.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.11.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Renard
 
 Relationships Extraction from NARrative Documents
 
 
+# Installation
+
+You can install the latest version using pip:
+
+> pip install renard-pipeline
+
+
 # Documentation
 
 Documentation, including installation instructions, can be found at https://compnet.github.io/Renard/
 
 If you need local documentation, it can be generated using `Sphinx`. From the `docs` directory, `make html` should create documentation under `docs/_build/html`.
```

