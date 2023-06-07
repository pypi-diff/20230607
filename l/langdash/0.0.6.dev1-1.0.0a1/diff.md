# Comparing `tmp/langdash-0.0.6.dev1.tar.gz` & `tmp/langdash-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.6.dev1.tar", last modified: Sun Jun  4 02:53:44 2023, max compression
+gzip compressed data, was "langdash-1.0.0a1.tar", last modified: Wed Jun  7 03:27:37 2023, max compression
```

## Comparing `langdash-0.0.6.dev1.tar` & `langdash-1.0.0a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 02:53:44.085259 langdash-0.0.6.dev1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.6.dev1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.6.dev1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3651 2023-06-04 02:53:44.081259 langdash-0.0.6.dev1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2739 2023-06-04 02:42:37.000000 langdash-0.0.6.dev1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 02:53:44.081259 langdash-0.0.6.dev1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-06-04 02:41:16.000000 langdash-0.0.6.dev1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    21725 2023-06-04 00:21:14.000000 langdash-0.0.6.dev1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 02:53:44.077259 langdash-0.0.6.dev1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.6.dev1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.6.dev1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     4369 2023-06-04 00:10:44.000000 langdash-0.0.6.dev1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-04 02:21:56.000000 langdash-0.0.6.dev1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1544 2023-06-04 02:01:37.000000 langdash-0.0.6.dev1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     6751 2023-06-04 02:00:32.000000 langdash-0.0.6.dev1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 02:53:44.081259 langdash-0.0.6.dev1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.6.dev1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1807 2023-06-04 01:43:57.000000 langdash-0.0.6.dev1/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     4708 2023-06-04 00:10:44.000000 langdash-0.0.6.dev1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.6.dev1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     8066 2023-06-04 02:04:13.000000 langdash-0.0.6.dev1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      995 2023-06-04 00:37:03.000000 langdash-0.0.6.dev1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6924 2023-06-04 02:49:37.000000 langdash-0.0.6.dev1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      833 2023-06-04 00:10:44.000000 langdash-0.0.6.dev1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2591 2023-06-02 03:34:57.000000 langdash-0.0.6.dev1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 02:53:44.081259 langdash-0.0.6.dev1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.6.dev1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      841 2023-06-04 00:36:12.000000 langdash-0.0.6.dev1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.6.dev1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.6.dev1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 02:53:44.081259 langdash-0.0.6.dev1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3651 2023-06-04 02:53:44.000000 langdash-0.0.6.dev1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-04 02:53:44.000000 langdash-0.0.6.dev1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-04 02:53:44.000000 langdash-0.0.6.dev1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      163 2023-06-04 02:53:44.000000 langdash-0.0.6.dev1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-04 02:53:44.000000 langdash-0.0.6.dev1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-04 02:53:44.085259 langdash-0.0.6.dev1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1524 2023-06-03 07:05:33.000000 langdash-0.0.6.dev1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.303313 langdash-1.0.0a1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.0.0a1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.0.0a1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2510 2023-06-07 03:27:37.303313 langdash-1.0.0a1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1601 2023-06-07 03:10:35.000000 langdash-1.0.0a1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       63 2023-06-07 03:02:15.000000 langdash-1.0.0a1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21883 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.0.0a1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      779 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.303313 langdash-1.0.0a1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.0.0a1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6343 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7973 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6920 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2577 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.0.0a1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1117 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      947 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2787 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2510 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-07 03:27:37.303313 langdash-1.0.0a1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.0.0a1/setup.py
```

### Comparing `langdash-0.0.6.dev1/LICENSE.txt` & `langdash-1.0.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.6.dev1/langdash/chains.py` & `langdash-1.0.0a1/langdash/chains.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 from dataclasses import dataclass
 from collections import OrderedDict
-from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING
+from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING, cast
 import re
 import random
 import copy
 import warnings
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from langdash.infer import InferArgs
 
 if TYPE_CHECKING:
-  from langdash._langdash import Langdash
+  from langdash.core import Langdash
   from langdash.llm_session import LLMGenerationSession, LLMState
 
-RE_FIRST_CONST = re.compile(r'^((?:[^{]|{{)+)')
-RE_IDENT = re.compile(r'^({[a-zA-Z_][a-zA-Z0-9_]*})')
-RE_FORMAT_ARG = re.compile(r'^({[^}]+})')
+RE_FIRST_CONST = re.compile(r"^((?:[^{]|{{)+)")
+RE_IDENT = re.compile(r"^({[a-zA-Z_][a-zA-Z0-9_]*})")
+RE_FORMAT_ARG = re.compile(r"^({[^}]+})")
 
 LDNodeGenerator = Generator[Response, None, None]
 LDNodeArgs = Dict[str, Any]
 LDNodeArgsFrozen = FrozenSet[Tuple[str, Any]]
 TypeDict = Dict[str, Type]
 
+
 @dataclass(frozen=True)
 class CalledChain:
   """
   Data class used to store info about nodes previously called.
   
   Attributes:
     node: Node object
     args: Arguments passed to the node (for LDFormatArg)
     tokens_used: Number of tokens the node used (either number of tokens injected, or generated)
   """
   node: "LDNode"
   args: LDNodeArgs
   tokens_used: int
 
+
 class LDChain:
   """ Class used to represent language chains """
+
   def __init__(
     self,
     ld: "Langdash",
     nodes: List[Union["LDNode", str]],
     args: TypeDict = {},
     returns: TypeDict = {},
   ):
     self._ld = ld
     self._args = args
     self._returns = returns
     assert len(nodes) > 0, "at least one node must be given to chain"
     self._nodes = self._preprocess_nodes(nodes)
-  
+
   def cached(self, model: str, **model_kwargs) -> "LDChainCached":
     """
     Cache the chain for a specific model
     
     Args:
       model (str): The model name
       
@@ -65,27 +68,28 @@
       model=model,
       model_kwargs=model_kwargs,
       _ld=self._ld,
       _args=self._args,
       _returns=self._returns,
       _nodes=self._nodes,
     )
-  
+
   def argtype(self, name: str) -> Optional[Type]:
     """
     Return the type of the argument.
     """
     try:
       return self._args[name]
     except KeyError:
       return None
-  
-  def _preprocess_nodes(self, nodes: List[Union["LDNode", str]]) -> List["LDNode"]:
+
+  def _preprocess_nodes(self, nodes: List[Union["LDNode",
+                                                str]]) -> List["LDNode"]:
     pp_nodes: List[Optional[LDNode]] = []
-    
+
     def _preprocess_format_arg(node: LDFormatArg):
       text = node._text
       while text:
         matches = RE_FIRST_CONST.match(text)
         skip = 0
         if matches:
           skip = len(matches.group(0))
@@ -102,71 +106,79 @@
               fmt = matches.group(0)
               skip = len(matches.group(0))
               pp_nodes.append(self._ld.format_args(fmt))
             else:
               pp_nodes.append(self._ld.format_args(text))
               break
         text = text[skip:]
-    
+
     # create pp_nodes
     for node in nodes:
       if isinstance(node, str):
         pp_nodes.append(self._ld.text(node))
       elif isinstance(node, LDFormatArg):
         _preprocess_format_arg(node)
       else:
         pp_nodes.append(node)
-    
+
     # fuse text nodes
     for i in range(len(pp_nodes)):
-      if isinstance(pp_nodes[i], LDText):
+      pp_node_i = pp_nodes[i]
+      if isinstance(pp_node_i, LDText):
         for j in range(i + 1, len(pp_nodes)):
-          if not isinstance(pp_nodes[j], LDText):
+          pp_node_j = pp_nodes[j]
+          if not isinstance(pp_node_j, LDText):
             break
-          pp_nodes[i]._text += pp_nodes[j]._text
-          pp_nodes[j] = None
-    
+          pp_node_i._text += pp_node_j._text
+          pp_node_j = None
+
     # filter
     pp_nodes = [node for node in pp_nodes if node is not None]
-    
-    return pp_nodes
-    
+
+    return cast(List[LDNode], pp_nodes)
+
   def _node_pass(self, session: "LLMGenerationSession", args: LDNodeArgs):
     for node in self._nodes:
       session.tokens_counter = 0
       yield node
       session._append_called_chain(node, args, session.tokens_counter)
-  
-  def _load_session(self, ctx: Union[str, "LLMGenerationSession"]) -> "LLMGenerationSession":
+
+  def _load_session(
+    self, ctx: Union[str, "LLMGenerationSession"]
+  ) -> "LLMGenerationSession":
     from langdash.llm_session import LLMGenerationSession
     if isinstance(ctx, LLMGenerationSession):
-      return ctx
+      return cast(LLMGenerationSession, ctx)
     else:
-      return self._ld.session_for_model(ctx)
-  
+      session = self._ld.session_for_model(ctx)
+      assert isinstance(
+        session, LLMGenerationSession
+      ), "context must be LLMGenerationSession"
+      return session
+
   def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs) \
     -> Generator[Response, None, None]:
     for node in self._node_pass(session, args):
-      if isinstance(node, Union[LDReturns, LDChoice]):
+      if isinstance(node, (LDReturns, LDChoice)):
         yield RespReturns(key=node._returns)
       yield from node(session, args)
-  
+
   def stream(self, ctx: Union[str, "LLMGenerationSession"], **kwargs) \
     -> Generator[Response, None, None]:
     """
     Stream data generated from the LLM within the specified session.
     
     Args:
       session (Union[str, "LLMGenerationSession"]):
         The name of the model, or an existing LLM generation session.
       args (LDNodeArgs):
         Arguments to pass to the chain. This will be used by any argument or format nodes.
     """
     return self._stream(session=self._load_session(ctx), **kwargs)
-  
+
   def _call(
     self,
     session: "LLMGenerationSession",
     args: LDNodeArgs = {},
     return_session: bool = False,
     set_global_args: bool = False,
   ) -> Union["LDResult", Tuple["LDResult", "LLMGenerationSession"]]:
@@ -181,15 +193,15 @@
       else:
         result.update_stats(generator)
     if return_session:
       if set_global_args:
         session.global_args = args
       return result, session
     return result
-  
+
   def call(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
     """
     Returns data generated from the LLM within the specified session.
     
     Args:
       ctx (Union[str, "LLMGenerationSession"]):
         The name of the model, or an existing LLM generation session.
@@ -201,112 +213,123 @@
         Whether or not to set current arguments as global arguments.
     
     Returns:
       (LDResult) The result, or a tuple with (result, session).
     """
     return self._call(session=self._load_session(ctx), **kwargs)
 
+
 @dataclass
 class LDChainCacheState:
   state: "LLMState"
   skip_nodes: int
 
-LDChainCacheStoreDict = OrderedDict[FrozenSet[Tuple[str, Any]], LDChainCacheState]
+
+LDChainCacheStoreDict = OrderedDict[FrozenSet[Tuple[str, Any]],
+                                    LDChainCacheState]
+
 
 @dataclass(frozen=True)
 class LDChainCacheStore:
   _dict: LDChainCacheStoreDict
   _model: str
   _model_kwargs: dict
 
+
 class LDChainCached(LDChain):
-  
+
   def __init__(self, model: str, model_kwargs: dict, **kwargs):
     for k, v in kwargs.items():
       setattr(self, k, v)
-      
+
     self._model = model
     self._model_kwargs = model_kwargs
-    
+
     # track the first index where the argument is first used
-    _arg_first_used_at = { k: -1 for k in self._args.keys() }
+    _arg_first_used_at = {k: -1 for k in self._args.keys()}
     # track the first index where any argument is used
     self._any_arg_first_use = 0
     for idx, node in enumerate(self._nodes):
       if isinstance(node, LDArg) and _arg_first_used_at[node._arg] == -1:
         _arg_first_used_at[node._arg] = idx
-      if isinstance(node, (LDArg, LDFormatArg)) and self._any_arg_first_use == 0:
+      if isinstance(
+        node, (LDArg, LDFormatArg)
+      ) and self._any_arg_first_use == 0:
         self._any_arg_first_use = idx
     # set min(_arg_first_used_at.values) == self._any_arg_first_use
     for k, v in _arg_first_used_at.items():
       if v == -1:
         _arg_first_used_at[k] = self._any_arg_first_use
-    
+
     self._arg_first_used_at: Dict[str, int] = _arg_first_used_at
     self._arg_first_used_at_ordered: List[str] = list(_arg_first_used_at.keys())
     self._arg_first_used_at_ordered.sort(key=lambda k: _arg_first_used_at[k])
-    
+
     # cache session per argument use
     self._state_cache: LDChainCacheStoreDict = OrderedDict()
     if len(self._args) == 0:
       self.max_states_to_cache = 1
     else:
       self.max_states_to_cache = min(len(self._args) + 2, 8)
     self._skip_nodes = 0
-  
+
   # State cache functions
-  
+
   def load_cache_store(self, cache_store: LDChainCacheStore):
     """
     Loads the cache store from previous inference time.
     Raises `ValueError` if the model names mismatch.
     This function expects that the model data of the parent Langdash instance does not change across session. If it does, a `UserWarning` is raised.
     
     Args:
       cache_store (LDChainCacheStore): The cache store.
     """
     if self._model != cache_store._model:
       raise ValueError("model mismatch for LDChainCacheStore")
     if self._model_kwargs != cache_store._model_kwargs:
-      warnings.warn("model kwargs does not match LDChainCacheStore, unexpected behavior might occur", UserWarning)
+      warnings.warn(
+        "model kwargs does not match LDChainCacheStore, unexpected behavior might occur",
+        UserWarning
+      )
     self._state_cache = cache_store._dict
-  
+
   def save_cache_store(self) -> LDChainCacheStore:
     """ Saves the cache store into an object. """
     return LDChainCacheStore(
       _dict=copy.deepcopy(self._state_cache),
       _model=self._model,
       _model_kwargs=copy.deepcopy(self._model_kwargs)
     )
-  
+
   def _set_state_cache(
-    self,
-    key: FrozenSet[Tuple[str, Any]],
-    value: LDChainCacheState):
+    self, key: FrozenSet[Tuple[str, Any]], value: LDChainCacheState
+  ):
     self._state_cache[key] = value
     self._update_state_cache(key)
     if len(self._state_cache) > self.max_states_to_cache:
       self._state_cache.popitem(last=True)
-  
+
   def _update_state_cache(self, key: FrozenSet[Tuple[str, Any]]):
     self._state_cache.move_to_end(key, last=False)
-  
-  def _get_state_cache(self, key: FrozenSet[Tuple[str, Any]]) -> LDChainCacheState:
+
+  def _get_state_cache(
+    self, key: FrozenSet[Tuple[str, Any]]
+  ) -> LDChainCacheState:
     self._update_state_cache(key)
     return self._state_cache[key]
-      
+
   def _arg_subset_sorted_by_idx(self, args: LDNodeArgs):
     current_subset: LDNodeArgs = {}
     yield current_subset
     for arg in self._arg_first_used_at_ordered:
       current_subset[arg] = args[arg]
       yield current_subset
-  
+
   # Inference functions
-  
+
   def _node_pass(self, session: "LLMGenerationSession", args: LDNodeArgs):
     last_state_key: Optional[LDChainCacheState] = None
     for i in range(self._skip_nodes, len(self._nodes)):
       node = self._nodes[i]
       session.tokens_counter = 0
       yield node
       if isinstance(node, LDText) and last_state_key is not None:
@@ -324,87 +347,97 @@
           for k, v in args.items()
           if self._arg_first_used_at[k] <= cached_idx
         )
         if current_keys not in self._state_cache:
           self._set_state_cache(
             current_keys,
             LDChainCacheState(
-              state=session.clone_state(),
-              skip_nodes=(cached_idx + 1)
+              state=session.clone_state(), skip_nodes=(cached_idx + 1)
             )
           )
         else:
           self._update_state_cache(current_keys)
         last_state_key = self._state_cache[current_keys]
       else:
         last_state_key = None
       session._append_called_chain(node, args, session.tokens_counter)
 
   def _create_new_session(self) -> "LLMGenerationSession":
-    return self._ld.session_for_model(self._model, **self._model_kwargs)
-
-  def _load_session(
-    self,
-    args: Optional[LDNodeArgs] = None) -> "LLMGenerationSession":
+    ctx = self._ld.session_for_model(self._model, **self._model_kwargs)
+    from langdash.llm_session import LLMGenerationSession
+    assert isinstance(
+      ctx, LLMGenerationSession
+    ), "context must be LLMGenerationSession"
+    return ctx
+
+  def _load_gen_session(
+    self, args: Optional[LDNodeArgs] = None
+  ) -> "LLMGenerationSession":
     session = self._create_new_session()
-    
+
     if frozenset() not in self._state_cache:
       text_node = self._nodes[0]
-      assert isinstance(text_node, LDText)
-      session.inject(text_node._text)
-      
-      self._set_state_cache(
-        frozenset(),
-        LDChainCacheState(state=session.clone_state(), skip_nodes=1))
-      self._skip_nodes = 1
-      
+
+      if isinstance(text_node, LDText):
+        session.inject(text_node._text)
+        self._set_state_cache(
+          frozenset(),
+          LDChainCacheState(state=session.clone_state(), skip_nodes=1)
+        )
+        self._skip_nodes = 1
+
       return session
-    
+
     if args is None:
       old_state_cache = self._get_state_cache(frozenset())
       self._skip_nodes = old_state_cache.skip_nodes
       session.set_state(old_state_cache.state)
       return session
     else:
       for subset in self._arg_subset_sorted_by_idx(args):
         subset_frozen = frozenset(subset.items())
         if subset_frozen not in self._state_cache:
           break
         old_state_cache = self._get_state_cache(subset_frozen)
-      
+
       session.set_state(old_state_cache.state)
       self._skip_nodes = old_state_cache.skip_nodes
       return session
-  
+
   def stream(self, **kwargs):
-    return super()._stream(session=self._load_session(args=kwargs.get("args")), **kwargs)
-  
+    return super()._stream(
+      session=self._load_gen_session(args=kwargs.get("args")), **kwargs
+    )
+
   def call(self, **kwargs):
-    return super()._call(session=self._load_session(args=kwargs.get("args")), **kwargs)
+    return super()._call(
+      session=self._load_gen_session(args=kwargs.get("args")), **kwargs
+    )
+
 
 @dataclass
 class LDResult:
   """
   Class for storing the results of inference.
   
   Attributes:
     returns: Mapping of return keys to return values
     prompt_tokens: Number of tokens injected to the language model
     completion_tokens: Number of tokens generated by the language model
   """
-  
+
   returns: Dict[str, Any]
   prompt_tokens: int
   completion_tokens: int
-  
+
   def __init__(self):
     self.returns = {}
     self.prompt_tokens = 0
     self.completion_tokens = 0
-    
+
   def update_results(self, key: str, cast_function, generator: LDNodeGenerator):
     """
     Update the results with the given key.
     
     Args:
       key (str): The key of the language model.
       cast_function: The function to cast the results.
@@ -415,237 +448,268 @@
       if isinstance(resp, RespInfer):
         text = resp.running_infer
         if resp.tokid != -1:
           self.completion_tokens += 1
       else:
         raise NotImplementedError(resp.__class__.__name__)
     self.returns[key] = cast_function(text)
-    
-  def update_results_array(self, generator: LDNodeGenerator):
+
+  def update_results_array(self, key: str, generator: LDNodeGenerator):
     """
     Appends array in generator to result.
     
     Args:
       key (str): The key of the language model.
-      cast_function: The function to cast the results.
       generator (LDNodeGenerator): Node generator that runs to get the results.
     """
-    key = None
     text = ""
     for resp in generator:
       if isinstance(resp, RespInfer):
         text = resp.running_infer
         if resp.tokid != -1:
           self.completion_tokens += 1
         else:
           self.returns[key].append(text)
-          key = None
           text = ""
-      elif isinstance(resp, RespReturns):
-        key = resp.key
       else:
         raise NotImplementedError(resp.__class__.__name__)
-    
+
   def update_stats(self, generator: LDNodeGenerator):
     """
     Update the stats of the result, given a node generator.
     
     Args:
       generator (LDNodeGenerator): Node generator to get the results.
     """
     for resp in generator:
       if isinstance(resp, RespInject):
         self.prompt_tokens += resp.tokens_counter
       else:
         continue
 
+
 class LDNode:
   """ Base class for langdash nodes. """
+
   def __init__(self, ld: "Langdash"):
     self._ld = ld
-    
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
     raise NotImplementedError("__call__")
-  
+
+
 class LDText(LDNode):
   """ Constant text node """
-  
+
   def __init__(self, ld: "Langdash", text: str):
     super().__init__(ld)
     self._text = text
-    
+
   def __repr__(self):
     return f"<Text>\n{self._text}\n</Text>"
-  
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
     tokens_counter = session.inject(self._text)
     yield RespInject(tokens_counter=tokens_counter)
-  
+
+
 class LDFormatArg(LDNode):
   """ Format argument node """
-  
+
   def __init__(self, ld: "Langdash", text: str):
     super().__init__(ld)
     self._text = text
-  
+
   def __repr__(self):
     return f"<FormatArgs>\n{self._text}\n</FormatArgs>"
-  
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
-    tokens_counter = session.inject(self._text.format(globals=session.global_args, **args))
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
+    tokens_counter = session.inject(
+      self._text.format(globals=session.global_args, **args)
+    )
     yield RespInject(tokens_counter=tokens_counter)
 
+
 class LDArg(LDNode):
   """ Argument node """
-  
-  def __init__(self, ld: "Langdash",
-               arg: str,
-               padleft: str = "",
-               padright: str = ""):
+
+  def __init__(
+    self, ld: "Langdash", arg: str, padleft: str = "", padright: str = ""
+  ):
     super().__init__(ld)
     self._arg = arg
     self._padleft = padleft
     self._padright = padright
-  
+
   def __repr__(self):
     return f"<Arg arg={self._arg}>"
-  
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
-    s =  ""
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
+    s = ""
     s += self._padleft
     if self._arg in args:
       s += str(args[self._arg])
     else:
       s += str(session.global_args[self._arg])
     s += self._padright
     tokens_counter = session.inject(s)
     yield RespInject(tokens_counter=tokens_counter)
-  
+
+
 class LDReturns(LDNode):
   """ Return node """
-  
-  def __init__(self, ld: "Langdash",
-               returns: str,
-               end: Optional[Union[str, int]],
-               padleft: str = "",
-               infer_args: Optional[InferArgs] = None):
+
+  def __init__(
+    self,
+    ld: "Langdash",
+    returns: str,
+    end: Optional[Union[str, int]],
+    padleft: str = "",
+    infer_args: Optional[InferArgs] = None
+  ):
     super().__init__(ld)
     self._returns = returns
     self._end = end
     self._padleft = padleft
     self._infer_args = infer_args
-  
+
   def __repr__(self):
     return f"<Returns arg={self._returns}>"
-  
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
-    for i, respinfer in enumerate(session.infer(end=self._end, args=self._infer_args)):
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
+    for i, respinfer in enumerate(
+      session.infer(end=self._end, args=self._infer_args)
+    ):
       if i == 0:
         if self._padleft and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       yield respinfer
-      
+
+
 class LDChoice(LDNode):
   """ Choice node """
-  
-  def __init__(self, ld: "Langdash",
-               returns: str,
-               choices: List[str],
-               padleft: str = "",
-               padright: str = "",
-               argmax: bool = False):
+
+  def __init__(
+    self,
+    ld: "Langdash",
+    returns: str,
+    choices: List[str],
+    padleft: str = "",
+    padright: str = "",
+    argmax: bool = False
+  ):
     super().__init__(ld)
     self._returns = returns
     self._choices = choices
     self._padleft = padleft
     self._padright = padright
     self._argmax = argmax
     self._choices_preprocessed = [
       f"{self._padleft}{choice}{self._padright}" for choice in self._choices
     ]
-    
+
   def __repr__(self):
     return f"<Choices {self._returns}>"
-  
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
     from langdash.llm_session import LLMGenerationSessionForRawText
-    
+
     tokids = [-1] * len(self._choices_preprocessed)
     has_multiple_tokens = False
-    
+
     heal_padleft: Optional[str] = None
     if session.token_healing and \
       isinstance(session, LLMGenerationSessionForRawText) and \
       session._next_token is not None:
       heal_padleft = session._next_token[1]
       session._next_token = None
-    
+
     for i, text in enumerate(self._choices_preprocessed):
       if heal_padleft is not None:
         text_tokids = session.tokenize(heal_padleft + text)
       else:
         text_tokids = session.tokenize(text)
       if len(text_tokids) > 1:
         has_multiple_tokens = True
         break
       tokids[i] = text_tokids[0]
-      
+
     if has_multiple_tokens:
       # TODO: handle multiple tokens
       raise NotImplementedError("handle multiple tokens not implemented")
     else:
       probs = session.next_token_probs()
       weights = [probs[tokid] for tokid in tokids]
       if self._argmax:
         inject_idx = self._choices.index(max(self._choices))
       else:
-        inject_idx = random.choices(range(len(self._choices)), weights=weights)[0]
+        inject_idx = random.choices(
+          range(len(self._choices)), weights=weights
+        )[0]
       tokid_inject = tokids[inject_idx]
       session.inject(tokid_inject)
       tokstr = self._choices[inject_idx]
       yield RespInfer(
         tokid=tokid_inject,
         tokstr=tokstr,
         running_infer=tokstr,
       )
       # for parity with RespInfer
       yield RespInfer(
         tokid=-1,
         tokstr="",
         running_infer=tokstr,
       )
-      
+
+
 class LDRepeat(LDNode):
   """ Repeat node """
-  
-  def __init__(self, ld: "Langdash",
-               subchain: LDChain,
-               append_source: str,
-               append_target: str,
-               end: str = "",
-               max_len: int = -1,
-               end_threshold: float = 0.5):
+
+  def __init__(
+    self,
+    ld: "Langdash",
+    subchain: LDChain,
+    append_source: str,
+    append_target: str,
+    end: str = "",
+    max_len: int = -1,
+    end_threshold: float = 0.5
+  ):
     super().__init__(ld)
     assert subchain._ld == ld
     self._subchain = subchain
     self._append_source = append_source
     self._append_target = append_target
     self._end = end
     self._max_len = max_len
     self._end_threshold = end_threshold
-  
-  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
+
+  def __call__(
+    self, session: "LLMGenerationSession", args: LDNodeArgs
+  ) -> LDNodeGenerator:
     if self._end:
       end_toks = session.tokenize(self._end)
       assert len(end_toks) == 1, "only supports 1 end token"
       end_tok = end_toks[0]
     else:
       end_tok = 0
     append_resp = RespReturns(key=self._append_target)
-    
+
     i = 0
     while True:
       in_append_source = False
       for resp in self._subchain.stream(session, args=args):
         if isinstance(resp, RespReturns):
           if resp.key == self._append_source:
             in_append_source = True
@@ -657,15 +721,15 @@
           if resp.tokid == -1:
             yield resp
             if in_append_source:
               in_append_source = False
         else:
           yield resp
           in_append_source = False
-      
+
       prob_dist = session.next_token_probs()
       if prob_dist[end_tok] > self._end_threshold:
         break
-      
+
       i += 1
       if i == self._max_len:
-        break
+        break
```

### Comparing `langdash-0.0.6.dev1/langdash/classify/token_qa.py` & `langdash-1.0.0a1/langdash/classify/token_qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-from typing import Union, List, Tuple, Dict, Optional
+from typing import Union, List, Tuple, Dict, Optional, cast
 from langdash.chains import LDChainCached, LDResult, LDNodeArgs
+from langdash.llm_session import LLMGenerationSession
+
 
 class TokenQA:
-  
-  def __init__(self,
-               prompt_chain: LDChainCached,
-               classes: Dict[str, Union[str, List[str]]]):
+  _classes_tok: Dict[str, List[int]]
+
+  def __init__(
+    self, prompt_chain: LDChainCached, classes: Dict[str, Union[str, List[str]]]
+  ):
     self._prompt_chain = prompt_chain
-    assert self._prompt_chain.argtype("query") == str, "prompt must have query argument"
-    
+    assert self._prompt_chain.argtype(
+      "query"
+    ) == str, "prompt must have query argument"
+
     self._classes = classes
-    self._classes_tok: Optional[Dict[str, List[int]]] = None
+    self._classes_tok = {}
     self._token_list_set = False
 
-  def _strs_to_token_list(session, str_or_list) -> List[int]:
+  @staticmethod
+  def _strs_to_token_list(
+    session: LLMGenerationSession, str_or_list: Union[str, List[str]]
+  ) -> List[int]:
     str_list = str_or_list if isinstance(str_or_list, list) else [str_or_list]
     token_list = []
     for str_ in str_list:
       token = session.tokenize(str_)
       assert len(token) == 1
       token_list.append(token[0])
     return token_list
-  
+
   def query(self,
             query: str,
             additional_args: Optional[LDNodeArgs] = None,
             return_result: bool = False) \
     -> Union[Dict[str, float], Tuple[Dict[str, float], LDResult]]:
-    args={"query":query}
+    args = {"query": query}
     if additional_args is not None:
       args.update(additional_args)
-    result, session = self._prompt_chain.call(
-      args=args,
-      return_session=True
-    )
+    result, session = self._prompt_chain.call(args=args, return_session=True)
     if not self._token_list_set:
       self._classes_tok = {}
       for k, v in self._classes.items():
         self._classes_tok[k] = TokenQA._strs_to_token_list(session, v)
       self._token_list_set = True
-      
+
     tok_probs = session.next_token_probs()
-    
-    prob = {}
+
+    prob: Dict[str, float] = {}
     for k, toks in self._classes_tok.items():
       prob[k] = sum(map(lambda tok: float(tok_probs[tok]), toks))
     prob_sum = sum(prob.values())
-    for k, v in prob.items():
-      prob[k] = v / prob_sum
-    
+    #FIXME: mypy gives wrong type inference for k and v
+    for k, v in prob.items():  # type: ignore
+      prob[k] = v / prob_sum  # type: ignore
+
     if return_result:
       return prob, result
-    return prob
+    return prob
```

### Comparing `langdash-0.0.6.dev1/langdash/core.py` & `langdash-1.0.0a1/langdash/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,75 @@
 import gc
 from typing import Dict, Callable, TypeVar
 from langdash.llm import LLM
 from langdash.llm_session import LLMSession, T_LLM
 import langdash.chains as chains
 
+
+def _llama_cpp_callback(*a, **k):
+  from .models.llama_cpp import LlamaCppModel
+  return LlamaCppModel(*a, **k)
+
+
+def _rwkv_cpp_callback(*a, **k):
+  from .models.rwkv_cpp import RwkvCppModel
+  return RwkvCppModel(*a, **k)
+
+
+def _transformers_callback(*a, **k):
+  from .models.transformers import TransformersModel
+  return TransformersModel(*a, **k)
+
+
+def _sentence_transformers_callback(*a, **k):
+  from .models.sentence_transformers import SentenceTransformersModel
+  return SentenceTransformersModel(*a, **k)
+
+
+MODEL_CALLBACKS = {
+  "llama_cpp": _llama_cpp_callback,
+  "rwkv_cpp": _rwkv_cpp_callback,
+  "transformers": _transformers_callback,
+  "sentence_transformers": _sentence_transformers_callback,
+}
+
 T_ModelInternal = TypeVar("T_ModelInternal")
 
+
 class Langdash:
   """
   Core Langdash instance.
   """
   _models: Dict[str, LLM]
-  
+
   def __init__(self):
     self._models = {}
     self._cached_models = {}
-  
-  def get_model_internal(self,
-                         model: T_LLM,
-                         default: Callable[[T_LLM], T_ModelInternal]) -> T_ModelInternal:
+
+  def _get_model_internal(
+    self, model: T_LLM, default: Callable[[T_LLM], T_ModelInternal]
+  ) -> T_ModelInternal:
     if model in self._cached_models:
       return self._cached_models[model]
     gc.collect()
     self._cached_models[model] = default(model)
     return self._cached_models[model]
-  
+
   def register_model(self, name: str, model: LLM):
     """
     Register a new language model to the Langdash instance.
     
     Args:
       name (str): The name of the model.
       model (LLM): The LLM object.
     """
     if name in self._models:
       raise KeyError(f"model '{name}' already exists")
     self._models[name] = model
-    
+
   def session_for_model(self, model: str, **kwargs) -> LLMSession:
     """
     Create a new session for a given model.
     
     Args:
       model (str): The name of the model to be used.
       default_infer_args (InferArgs): Default inference arguments.
@@ -48,15 +77,15 @@
       token_healing (bool): Whether or not to heal tokens.
       global_args (LDNodeArgs): Global arguments which can be read by every chain.
     
     Returns:
       (LLMSession) The session object.
     """
     return self._models[model].session(ld=self, **kwargs)
-      
+
   def chain(self, *args, **kwargs) -> chains.LDChain:
     """
     Chain a list of nodes together.
 
     Args:
       nodes (List[Union["LDNode", str]]):
         A list of nodes or constant text nodes (represented by strings) to chain together.
@@ -65,39 +94,39 @@
       returns (TypeDict):
         A dictionary of return value types for the chain function.
 
     Returns:
       (LDChain) The chain of nodes.
     """
     return chains.LDChain(self, *args, **kwargs)
-    
+
   def text(self, *args, **kwargs):
     """
     Creates a raw text node.
     
     Args:
       text (str): The raw text.
       
     Returns:
       The text node.
     """
     return chains.LDText(self, *args, **kwargs)
-    
+
   def format_args(self, *args, **kwargs):
     """
     Creates a format argument node.
     
     Args:
       text (str): The format text.
       
     Returns:
       The format text node.
     """
     return chains.LDFormatArg(self, *args, **kwargs)
-    
+
   def arg(self, *args, **kwargs):
     """
     Creates a new argument node with the specified argument.
     
     Args:
       arg (str): The argument.
       padleft (str):
@@ -105,15 +134,15 @@
       padright (str):
         The padding string to use for the right side of the argument.
     
     Returns:
       The argument node.
     """
     return chains.LDArg(self, *args, **kwargs)
-    
+
   def returns(self, *args, **kwargs):
     """
     Create a new return node for the specified return value.
 
     Args:
       returns (str): The name of the return value.
       end (str):
@@ -128,25 +157,62 @@
     Returns:
       The return node.
     """
     return chains.LDReturns(self, *args, **kwargs)
 
   def choice(self, *args, **kwargs):
     """
-    Creates a new choice node with the specified choices, and returns to the .
+    Creates a new choice node with the specified choices.
     
     Args:
       returns (str): The name of the return value.
       choices (List[str]): List of choice strings
       padleft (str):
         Left padding for every choice string.
       padright (str):
         Right padding for every choice string.
     
     Returns:
       The choice node.
     """
     return chains.LDChoice(self, *args, **kwargs)
-  
+
   def repeat(self, *args, **kwargs):
+    """
+    Creates a new repetition node that repeats a subchain.
+    
+    Args:
+      subchain (LDChain):
+        The subchain to be repeated.
+      append_source (str):
+        The return variable of the subchain, extracted into the parent chain's `append_target` list.
+      append_target (str):
+        The append target variable of the parent chain.
+      end (str):
+        Token used to mark the end of the repetition. This token will not be injected as a prompt after the loop.
+      max_len (int):
+        Maximum number of repetitions. `-1` means the chain will repeat until the next most likely token is `end`.
+      end_threshold (float):
+        Minimum probability of end token for the repetition to end.
+    
+    Returns:
+      The repeat node.
+    """
     return chains.LDRepeat(self, *args, **kwargs)
-    
+
+  @staticmethod
+  def model_from_type(type: str, *args, **kwargs) -> LLM:
+    """
+    Create an instance of a builtin model with specified type name.
+    Additional arguments will be passed to the model constructor.
+    
+    Args:
+      type (str): The type of the model.
+    
+    Returns:
+      The model.
+    """
+    model_cb = MODEL_CALLBACKS.get(type)
+    if model_cb:
+      return model_cb(*args, **kwargs)
+    else:
+      raise KeyError(f"model {type} doesn't exist")
```

### Comparing `langdash-0.0.6.dev1/langdash/infer.py` & `langdash-1.0.0a1/langdash/infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 
+
 @dataclass
 class InferArgs:
   """
   Data class for inference arguments.
   
   Attributes:
     min_new_tokens: Minimum number of new tokens to generate
@@ -16,8 +17,8 @@
   """
   min_new_tokens: int = 0
   max_new_tokens: int = 512
   temperature: float = 1.0
   top_p: float = 0.0
   typical_mass: float = 0.0
   max_rep_ctx: int = 64
-  rep_penalty: float = 1.0
+  rep_penalty: float = 1.0
```

### Comparing `langdash-0.0.6.dev1/langdash/llm.py` & `langdash-1.0.0a1/langdash/llm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from typing import TypeVar, Generic, Type, TYPE_CHECKING
 from enum import Flag, auto
 
+
 class LLMCapability(Flag):
   """
   Capability of language models.
   """
   Generative = auto()
   Embedding = auto()
 
 
 if TYPE_CHECKING:
   from langdash.llm_session import LLMSession, LLMEmbeddingSession
-  T_LLMSession = TypeVar('T_LLMSession', bound=LLMSession)
-  T_LLMEmbeddingSession = TypeVar('T_LLMEmbeddingSession', bound=LLMEmbeddingSession)
+  T_LLMSession = TypeVar("T_LLMSession", bound=LLMSession)
+  T_LLMEmbeddingSession = TypeVar(
+    "T_LLMEmbeddingSession", bound=LLMEmbeddingSession
+  )
 else:
-  T_LLMSession = TypeVar('T_LLMSession')
-  T_LLMEmbeddingSession = TypeVar('T_LLMEmbeddingSession')
+  T_LLMSession = TypeVar("T_LLMSession")
+  T_LLMEmbeddingSession = TypeVar("T_LLMEmbeddingSession")
+
 
 class LLM(Generic[T_LLMSession]):
   """
   A language model class for inference.
   """
   Session: Type["T_LLMSession"]
-  
+
   def session(self, *args, **kwargs) -> "T_LLMSession":
     """
     Create a new session for the given model.
     
     Args:
       default_infer_args (dict):
         Default arguments for the default inference engine.
@@ -44,13 +48,15 @@
 
   def get_capability(self) -> LLMCapability:
     """
     Returns the capability of the language model.
     """
     return LLMCapability.Generative
 
+
 class EmbeddingLLM(LLM[T_LLMEmbeddingSession]):
   """
   A language model class for generating embeddings.
   """
+
   def get_capability(self) -> LLMCapability:
-    return LLMCapability.Embedding
+    return LLMCapability.Embedding
```

### Comparing `langdash-0.0.6.dev1/langdash/llm_session.py` & `langdash-1.0.0a1/langdash/llm_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,127 +3,139 @@
 
 from langdash.response import RespInfer
 from langdash.chains import CalledChain, LDNodeArgs, LDNode
 from langdash.infer import InferArgs
 from langdash.llm import LLM
 
 if TYPE_CHECKING:
-  from langdash._langdash import Langdash
+  from langdash.core import Langdash
 
-class LLMSession:
+T_LLM = TypeVar("T_LLM", bound=LLM)
+
+
+class LLMSession(Generic[T_LLM]):
   """
-  A session for LLM.
+  Base class for a session for a language model.
   """
+
+  def __init__(self, llm: T_LLM, ld: "Langdash"):
+    self._ld = ld
+    self._llm = llm
+
   def clone(self) -> "LLMSession":
+    """
+    Clone the current session.
+    """
     raise NotImplementedError("clone")
 
+
 class LLMState:
   """
   A state class for a language model.
   """
   pass
 
-T_LLM = TypeVar('T_LLM', bound=LLM)
+
 T_LLMState = TypeVar("T_LLMState", bound=LLMState)
 
+
 class LLMGenerationSession(LLMSession, Generic[T_LLM, T_LLMState]):
   """ Generation session for a language model. """
-  
-  def __init__(self,
-               llm: T_LLM,
-               ld: "Langdash",
-               default_infer_args: InferArgs = InferArgs(),
-               track_called_chains: bool = True,
-               token_healing: bool = True,
-               global_args: LDNodeArgs = {}):
-    self._ld = ld
-    self.llm = llm
+
+  def __init__(
+    self,
+    llm: T_LLM,
+    ld: "Langdash",
+    default_infer_args: InferArgs = InferArgs(),
+    track_called_chains: bool = True,
+    token_healing: bool = True,
+    global_args: LDNodeArgs = {}
+  ):
+    super().__init__(llm, ld)
     self.default_infer_args = default_infer_args
-    self.called_chains: Optional[List[CalledChain]] = (
-      [] if track_called_chains else None
-    )
+    self.called_chains: Optional[List[CalledChain]
+                                ] = ([] if track_called_chains else None)
     self.token_healing = token_healing
     self.global_args = global_args
     self.tokens_counter = 0
-    
+
   def set_state(self, state: Optional[T_LLMState]):
     """
     Set the state of the language model.
 
     Args:
       state (Optional[T_LLMState]):
         The state of the language model, or None to clear the state.
     """
     raise NotImplementedError("set_state")
-  
+
   def clone_state(self) -> T_LLMState:
     """
     Clone the current state of the language model.
     """
     raise NotImplementedError("clone_state")
-  
+
   def clone(self) -> "LLMGenerationSession":
-    """
-    Clone the current session.
-    """
     session = self.__class__(
-      llm=self.llm,
+      llm=self._llm,
       ld=self._ld,
       default_infer_args=self.default_infer_args,
       track_called_chains=False,
+      token_healing=self.token_healing,
       global_args=copy.copy(self.global_args)
     )
     session.set_state(self.clone_state())
     if self.called_chains is not None:
       session.called_chains = copy.copy(self.called_chains)
     return session
-  
-  def _append_called_chain(self,
-                           node: LDNode,
-                           args: LDNodeArgs,
-                           tokens_used: int):
+
+  def _append_called_chain(
+    self, node: LDNode, args: LDNodeArgs, tokens_used: int
+  ):
     if self.called_chains is None:
       pass
     else:
-      self.called_chains.append(CalledChain(node=node, args=args, tokens_used=tokens_used))
-  
+      self.called_chains.append(
+        CalledChain(node=node, args=args, tokens_used=tokens_used)
+      )
+
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     """
     Tokenize the given text into a list of tokens.
 
     Args:
       text (str): The text to tokenize.
       add_special_tokens (bool): Whether to add special tokens to the output.
 
     Returns:
       (List[int]) The list of tokens.
     """
     raise NotImplementedError("tokenize")
-  
+
   def decode(self, tokids: List[int]) -> str:
     raise NotImplementedError("decode")
-  
+
   def next_token_probs(self) -> List[float]:
     """
     Returns the probabilities for next token.
     """
     raise NotImplementedError("next_token_probs")
-  
+
   def flush_token(self):
     raise NotImplementedError("flush_token")
-  
-  def _infer(
-    self,
-    end: Optional[Union[str, int]],
-    args: InferArgs) -> Generator[RespInfer, None, None]:
+
+  def _infer(self, end: Optional[Union[str, int]],
+             args: InferArgs) -> Generator[RespInfer, None, None]:
     raise NotImplementedError("_infer")
 
-  def infer(self,
-            end: Optional[Union[str, int]],
-            args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
+  def infer(
+    self,
+    end: Optional[Union[str, int]],
+    args: Optional[InferArgs] = None
+  ) -> Generator[RespInfer, None, None]:
     """
     Infer the next token from the input sequence.
 
     Args:
       end (Optional[Union[str, int]]):
         The end of the output sequence.
         If set to None, the output sequence will be generated until the maximum number of tokens is reached.
@@ -132,95 +144,116 @@
         
     Returns:
       Inference response
     """
     if not args:
       args = self.default_infer_args
     yield from self._infer(end, args)
-    
-  def inject(self, text: Union[str, int], add_special_tokens: bool = False) -> int:
+
+  def inject(
+    self, text: Union[str, int], add_special_tokens: bool = False
+  ) -> int:
     raise NotImplementedError("inject")
 
-T_Logits = TypeVar('T_Logits')
 
-class LLMGenerationSessionForRawText(LLMGenerationSession, Generic[T_LLM, T_LLMState, T_Logits]):
+T_Tensor = TypeVar("T_Tensor")
+
+
+class LLMGenerationSessionForRawText(
+  LLMGenerationSession, Generic[T_LLM, T_LLMState, T_Tensor]
+):
   """ Generation session for a language model that processes raw text. """
-  
-  _logits: Optional[T_Logits]
+
+  _logits: Optional[T_Tensor]
   _next_token: Optional[Tuple[int, str]]
-  
-  def _eval(self, tokid: int) -> T_Logits:
+
+  def __init__(self, *args, **kwargs):
+    super().__init__(*args, **kwargs)
+    self._logits = None
+    self._next_token = None
+
+  def _eval(self, tokid: int) -> T_Tensor:
     raise NotImplementedError("_eval")
-  
+
   def _eval_mult(self, tokens: List[int]):
     assert tokens, "tokens must not be empty"
     for tokid in tokens:
       logits = self._eval(tokid)
     return logits
-  
+
   def flush_token(self):
     """
     Flushes the previous token into the language model if healing is enabled.
     
     **Warning:** unexpected behavior if the previous token is a "boundary" token
     like spaces.
     """
     if self._next_token is None:
       return
     self.inject(self._next_token[0])
     self._next_token = None
-  
+
   def next_token_probs(self, *args, **kwargs) -> List[float]:
     raise NotImplementedError("next_token_probs")
-  
-  def inject(self, text: Union[str, int], add_special_tokens: bool = False) -> int:
+
+  def _on_first_inject(self):
+    return
+
+  def inject(
+    self, text: Union[str, int], add_special_tokens: bool = False
+  ) -> int:
     if isinstance(text, str):
       tokens = self.tokenize(text, add_special_tokens=add_special_tokens)
     else:
       tokens = [text]
     if not tokens:
       return 0
-    
+
+    if self._logits is None:
+      self._on_first_inject()
+
     num_toks = 0
-      
+
     if self.token_healing:
       if self._next_token is not None:
         tokid, _ = self._next_token
-        tokens = self.tokenize(self.decode([tokid, *tokens]), add_special_tokens=add_special_tokens)
+        tokens = self.tokenize(
+          self.decode([tokid, *tokens]), add_special_tokens=add_special_tokens
+        )
       if len(tokens) > 1:
         self._logits = self._eval_mult(tokens[:-1])
         num_toks += len(tokens) - 1
       self._next_token = (tokens[-1], self.decode([tokens[-1]]))
     else:
       if self._next_token is not None:
         tokid, tokstr = self._next_token
         self._eval(tokid)
         num_toks += 1
       self._logits = self._eval_mult(tokens)
       num_toks += len(tokens)
 
     return num_toks
 
-T_Embedding = TypeVar('T_Embedding')
+
+T_Embedding = TypeVar("T_Embedding")
+
 
 class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Embedding]):
   """ Session for a language model that outputs an embedding for raw text. """
-  
-  def __init__(self,
-               llm: T_LLM,
-               ld: "Langdash"):
+
+  def __init__(self, llm: T_LLM, ld: "Langdash"):
     self._ld = ld
-    self.llm = llm
-    
+    self._llm = llm
+
   def embedding_size(self) -> int:
     """
     Returns the embedding size of the model.
     """
     raise NotImplementedError("embedding_size")
-    
+
   def embed(self, documents: List[str]) -> T_Embedding:
     """
     Infer the embedding of a list of text.
     
     Args:
       documents (List[str]): The text to be embedded.
```

### Comparing `langdash-0.0.6.dev1/langdash/models/_bpe.py` & `langdash-1.0.0a1/langdash/models/_bpe.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,37 +10,44 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Extracted from transformers/src/transformers/models/gpt2/tokenization_gpt2.py
 
+
 def _byte_encode_dict():
   """
   Returns list of utf-8 byte and a mapping to unicode strings. We specifically avoids mapping to whitespace/control
   characters the bpe code barfs on.
   The reversible bpe codes work on unicode strings. This means you need a large # of unicode characters in your vocab
   if you want to avoid UNKs. When you're at something like a 10B token dataset you end up needing around 5K for
   decent coverage. This is a significant percentage of your normal, say, 32K bpe vocab. To avoid that, we want lookup
   tables between utf-8 bytes and unicode strings.
   """
   bs = (
-    list(range(ord("!"), ord("~") + 1)) + list(range(ord("¡"), ord("¬") + 1)) + list(range(ord("®"), ord("ÿ") + 1))
+    list(range(ord("!"),
+               ord("~") + 1)) + list(range(ord("¡"),
+                                           ord("¬") + 1)) +
+    list(range(ord("®"),
+               ord("ÿ") + 1))
   )
   cs = bs[:]
   n = 0
   for b in range(2**8):
     if b not in bs:
       bs.append(b)
       cs.append(2**8 + n)
       n += 1
   cs = [chr(n) for n in cs]
   return dict(zip(bs, cs))
 
+
 BYTE_ENCODE_DICT = _byte_encode_dict()
-BYTE_DECODE_DICT = { v: chr(k) for k, v in BYTE_ENCODE_DICT.items() }
+BYTE_DECODE_DICT = {v: chr(k) for k, v in BYTE_ENCODE_DICT.items()}
+
 
 def decode(s: str) -> str:
-  rs = ''
+  rs = ""
   for c in s:
     rs += BYTE_DECODE_DICT.get(c, c)
-  return rs
+  return rs
```

### Comparing `langdash-0.0.6.dev1/langdash/models/mock.py` & `langdash-1.0.0a1/langdash/models/mock.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Generator, Dict, Any
 from langdash.response import RespInfer
 from langdash.llm import LLM
 from langdash.llm_session import LLMSession
 
+
 class MockSession(LLMSession):
+
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
-  
+
   def inject(self, text: str) -> int:
     return 0
-  
-  def _infer(self, end: str, args: Dict[str, Any]) -> Generator[RespInfer, None, None]:
-    yield RespInfer(tokid=0, tokstr="", running_infer=self.llm._mockret)
+
+  def _infer(self, end: str,
+             args: Dict[str, Any]) -> Generator[RespInfer, None, None]:
+    yield RespInfer(tokid=0, tokstr="", running_infer=self._llm._mockret)
+
 
 class MockModel(LLM[MockSession]):
   Session = MockSession
-  
+
   def __init__(self, mockret: str):
     self._mockret = mockret
-  
+
   def session(self, **kwargs):
     return MockSession(self, **kwargs)
-
```

### Comparing `langdash-0.0.6.dev1/langdash/models/rwkv_cpp.py` & `langdash-1.0.0a1/langdash/models/rwkv_cpp.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,244 +15,253 @@
 import torch
 import pathlib
 
 _rwkv_lib: Optional[str] = None
 
 RWKV_CPP_COMMIT = "9e2a0de8436a956c5ef80fbd5f4184311a7a568d"
 
+
 def _load_rwkv_import():
   global _rwkv_lib
-  
+
   import subprocess
   import shutil
 
   import langdash
-  rwkv_cpp_folder = os.path.join(os.path.dirname(langdash.__file__), "extern/rwkv.cpp")
+  rwkv_cpp_folder = os.path.join(
+    os.path.dirname(langdash.__file__), "extern/rwkv.cpp"
+  )
 
   if not os.path.isdir(rwkv_cpp_folder):
     print("rwkv.cpp isn't installed, clone and install? (requires git, cmake)")
-    do_install = input("Type 'y' (without quotes) to install: ") == 'y'
+    do_install = input("Type 'y' (without quotes) to install: ") == "y"
     if not do_install:
       raise ImportError("rwkv.cpp is not installed")
-    
+
     os.makedirs(rwkv_cpp_folder, exist_ok=True)
     git = shutil.which("git")
-    if git == None:
+    if git is None:
       raise ImportError("git is needed for compiling rwkv.cpp")
     subprocess.check_call(
-      [git, "clone", "--recursive", "https://github.com/saharNooby/rwkv.cpp", rwkv_cpp_folder]
+      [
+        git, "clone", "--recursive", "https://github.com/saharNooby/rwkv.cpp",
+        rwkv_cpp_folder
+      ]
     )
     subprocess.check_call(
-      [git, "checkout", RWKV_CPP_COMMIT],
-      cwd=rwkv_cpp_folder
+      [git, "checkout", RWKV_CPP_COMMIT], cwd=rwkv_cpp_folder
     )
-    subprocess.check_call(
-      [git, "submodule", "update"],
-      cwd=rwkv_cpp_folder
-    )
-    
-  if 'win32' in sys.platform or 'cygwin' in sys.platform:
-    file_name = 'rwkv.dll'
-  elif 'darwin' in sys.platform:
-    file_name = 'librwkv.dylib'
+    subprocess.check_call([git, "submodule", "update"], cwd=rwkv_cpp_folder)
+
+  if "win32" in sys.platform or "cygwin" in sys.platform:
+    file_name = "rwkv.dll"
+  elif "darwin" in sys.platform:
+    file_name = "librwkv.dylib"
   else:
-    file_name = 'librwkv.so'
-  
+    file_name = "librwkv.so"
+
   _rwkv_lib = os.path.join(rwkv_cpp_folder, file_name)
-    
+
   if not os.path.isfile(_rwkv_lib):
     cmake = shutil.which("cmake")
-    if cmake == None:
+    if cmake is None:
       raise ImportError("cmake is needed for compiling rwkv.cpp")
+    subprocess.check_call([cmake, "."], cwd=rwkv_cpp_folder)
     subprocess.check_call(
-      [cmake, "."],
-      cwd=rwkv_cpp_folder
-    )
-    subprocess.check_call(
-      [cmake, "--build", ".", "--config", "Release"],
-      cwd=rwkv_cpp_folder
+      [cmake, "--build", ".", "--config", "Release"], cwd=rwkv_cpp_folder
     )
   sys.path.append(os.path.join(rwkv_cpp_folder, "rwkv"))
 
+
 _load_rwkv_import()
 
-import tokenizers # type: ignore
-import rwkv_cpp_model # type: ignore
-import rwkv_cpp_shared_library # type: ignore
+import tokenizers  # type: ignore
+import rwkv_cpp_model  # type: ignore
+import rwkv_cpp_shared_library  # type: ignore
+
 
 @dataclass
-class RWKVCppState(LLMState):
+class RwkvCppState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _state: Optional[torch.Tensor] = None
   _next_token: Optional[Tuple[int, str]] = None
 
+
 @dataclass
-class RWKVCppExtras:
+class RwkvCppExtras:
   tokenizer: tokenizers.Tokenizer
   vocab: Dict[str, int]
 
-class RWKVCppSession(LLMGenerationSessionForRawText["RWKVCppModel", RWKVCppState, torch.Tensor]):
+
+class RwkvCppSession(
+  LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor]
+):
   """
   Session for rwkv.cpp model.
   """
-  
+
   _rwkv: rwkv_cpp_model.RWKVModel
   _tokenizer: tokenizers.Tokenizer
-  
+
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
-    
-    def load_model(llm: RWKVCppModel):
+
+    def load_model(llm: RwkvCppModel):
       assert _rwkv_lib is not None
       model = rwkv_cpp_model.RWKVModel(
-        rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib),
-        llm._model_path
+        rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib), llm._model_path
       )
       tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
-      extras = RWKVCppExtras(
+      extras = RwkvCppExtras(
         tokenizer=tokenizer,
         vocab={
           bpe.decode(logits_tokstr): logits_tokid
           for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
         }
       )
       return model, extras
-      
-    self._rwkv, self._extras = self._ld.get_model_internal(self.llm, load_model)
+
+    self._rwkv, self._extras = self._ld._get_model_internal(
+      self._llm, load_model
+    )
     self._logits, self._state = None, None
     self._next_token = None
-  
+
   def _eval(self, tokid: int) -> torch.Tensor:
     self._logits, self._state = self._rwkv.eval(tokid, self._state)
     return self._logits
-  
-  def set_state(self, state: Optional[RWKVCppState]):
+
+  def set_state(self, state: Optional[RwkvCppState]):
     if state is None:
       self._logits, self._state = None, None
       self._next_token = None
     else:
       self._logits = copy.deepcopy(state._logits)
       self._state = copy.deepcopy(state._state)
       self._next_token = state._next_token
-    
-  def clone_state(self) -> RWKVCppState:
-    return RWKVCppState(
-      _logits = copy.deepcopy(self._logits),
-      _state = copy.deepcopy(self._state),
-      _next_token = self._next_token,
+
+  def clone_state(self) -> RwkvCppState:
+    return RwkvCppState(
+      _logits=copy.deepcopy(self._logits),
+      _state=copy.deepcopy(self._state),
+      _next_token=self._next_token,
     )
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return self._extras.tokenizer.encode(text, add_special_tokens=add_special_tokens).ids
-  
+    return self._extras.tokenizer.encode(
+      text, add_special_tokens=add_special_tokens
+    ).ids
+
   def decode(self, tokids: List[int]) -> str:
     return self._extras.tokenizer.decode(tokids)
-  
-  def next_token_probs(self) -> torch.Tensor:
+
+  def next_token_probs(self) -> List[float]:
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits, _ = self._rwkv.eval(self._next_token[0], self._state)
     return sampling.logits_to_probs(logits).tolist()
 
-  def _infer(
-    self,
-    end: Optional[Union[str, int]],
-    args: InferArgs) -> Generator[RespInfer, None, None]:
+  def _infer(self, end: Optional[Union[str, int]],
+             args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
-    
+
     assert args.min_new_tokens >= 0, "min_new_tokens must be at least 0"
-    
+
     if isinstance(end, str):
       if len(end) == 0:
         end = 0
       elif args.min_new_tokens > 0:
         endtoks = self.tokenize(end)
         assert len(endtoks) == 1
         end = endtoks[0]
-    
+
     if self._logits is None:
-      raise ValueError("no prompt provided for RWKVCppModel")
-    
+      raise ValueError("no prompt provided for RwkvCppModel")
+
     for i in range(args.max_new_tokens):
       strip_left = None
-      
+
       if i == 0 and self._next_token is not None:
         tokid, tokstr = self._next_token
 
         for logits_tokstr, logits_tokid in self._extras.vocab.items():
           if not logits_tokstr.startswith(tokstr):
             self._logits[logits_tokid] = -inf
-            
+
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
           self._logits, self._state = self._rwkv.eval(tokid, self._state)
         else:
           strip_left = tokstr
-        
-      if end != 0: # no early endoftext
+
+        self._next_token = None
+
+      if end != 0:  # no early endoftext
         self._logits[0] = -inf
       elif args.min_new_tokens > 0 and i < args.min_new_tokens:
         self._logits[end] = -inf
-      
+
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
-      
-      if tokid == end: # implies end is int
+
+      if tokid == end:  # implies end is int
         break
-      
+
       tokstr = self._extras.tokenizer.decode([tokid])
-      
+
       if "\ufffd" in tokstr:
         buffered_tokens.append(tokid)
         self._next_token = (tokid, "")
       else:
         if buffered_tokens:
           tokstr = self._extras.tokenizer.decode(buffered_tokens)
           tokstr += self._extras.tokenizer.decode([tokid])
           buffered_tokens.clear()
         else:
           if strip_left and tokstr.startswith(strip_left):
             tokstr = tokstr[len(strip_left):]
-      
+
         self._next_token = (tokid, tokstr)
-        
+
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
-        
+
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
-        
+
       self._logits, self._state = self._rwkv.eval(tokid, self._state)
-    
+
     if buffered_tokens:
       generated += self._extras.tokenizer.decode(buffered_tokens)
     yield RespInfer(tokid=-1, tokstr="", running_infer=generated)
 
-class RWKVCppModel(LLM[RWKVCppSession]):
+
+class RwkvCppModel(LLM[RwkvCppSession]):
   """
   rwkv.cpp model
   """
-  
-  Session = RWKVCppSession
-  
+
+  Session = RwkvCppSession
+
   def __init__(self, model_path: str, tokenizer_path: Optional[str] = None):
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
     
     Args:
       model_path (str): Path to the model file.
       tokenizer_path (Optional[str]):
         Path to the tokenizer file.
         If None is given, the tokenizer is assumed to be the model_path / '20B_tokenizer.json'.
     """
     self._model_path = model_path
     if tokenizer_path is None:
-      self._tokenizer_path = str(pathlib.Path(os.path.abspath(model_path)).parent / '20B_tokenizer.json')
+      self._tokenizer_path = str(
+        pathlib.Path(os.path.abspath(model_path)).parent / "20B_tokenizer.json"
+      )
     else:
       self._tokenizer_path = tokenizer_path
-
```

### Comparing `langdash-0.0.6.dev1/langdash/models/sentence_transformers.py` & `langdash-1.0.0a1/langdash/models/sentence_transformers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from typing import List
 from sentence_transformers import SentenceTransformer
 import torch
 from langdash.llm import EmbeddingLLM
 from langdash.llm_session import LLMEmbeddingSession
 
-class SentenceTransformersSession(LLMEmbeddingSession["SentenceTransformersModel", torch.Tensor]):
+
+class SentenceTransformersSession(
+  LLMEmbeddingSession["SentenceTransformersModel", torch.Tensor]
+):
   """
   Session for sentence_transformers embedding model.
   """
+
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
-      
-    self._model = self._ld.get_model_internal(
-      self.llm,
-      lambda llm: SentenceTransformer(llm._model_name)
+
+    self._model = self._ld._get_model_internal(
+      self._llm, lambda llm: SentenceTransformer(llm._model_name)
     )
-  
+
   def embedding_size(self) -> int:
     return self._model.get_sentence_embedding_dimension()
-  
-  def embed(self, documents: List[str]) -> T_Embedding:
+
+  def embed(self, documents: List[str]) -> torch.Tensor:
     return self._model.encode(documents)
 
+
 class SentenceTransformersModel(EmbeddingLLM[SentenceTransformersSession]):
   """
   sentence_transformers embedding model.
   """
   Session = SentenceTransformersSession
 
   def __init__(self, model_name: str):
```

### Comparing `langdash-0.0.6.dev1/langdash/models/transformers.py` & `langdash-1.0.0a1/langdash/models/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,122 +6,128 @@
 from langdash.response import RespInfer
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
 import langdash.models._bpe as bpe
 
-import transformers
+import transformers  # type: ignore
 import torch
 
 try:
   from transformers import RwkvForCausalLM as t_RwkvForCausalLM
+
   def model_is_rwkv(model):
     return isinstance(model, t_RwkvForCausalLM)
 except ImportError:
+
   def model_is_rwkv(model):
     return False
 
+
 @dataclass
 class TransformersState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _state: Any = None
   _next_token: Optional[Tuple[int, str]] = None
 
+
 @dataclass
 class TransformersExtras:
   tokenizer: Any
   vocab: Dict[str, int]
   buffered_token_head: Set[int]
 
-class TransformersSession(LLMGenerationSessionForRawText["TransformersModel", TransformersState, torch.Tensor]):
+
+class TransformersSession(
+  LLMGenerationSessionForRawText["TransformersModel", TransformersState,
+                                 torch.Tensor]
+):
   """
   Session for transformers model.
   """
-  
+
   _next_token: Optional[Tuple[int, str]]
-  
+
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
-    
+
     def load_model(llm: TransformersModel):
       model = transformers.AutoModelForCausalLM.from_pretrained(llm._model_name)
-      tokenizer = transformers.AutoTokenizer.from_pretrained(llm._tokenizer_name)
-      
+      tokenizer = transformers.AutoTokenizer.from_pretrained(
+        llm._tokenizer_name
+      )
+
       if isinstance(
-        tokenizer,
-        (
-          transformers.GPT2Tokenizer,
-          transformers.GPT2TokenizerFast
-        )
+        tokenizer, (transformers.GPT2Tokenizer, transformers.GPT2TokenizerFast)
       ):
         buffered_token_head = set(
           v for k, v in tokenizer.get_vocab().items() if "\u0122" in k
         )
       else:
         buffered_token_head = set()
-      
+
       extras = TransformersExtras(
         tokenizer=tokenizer,
         vocab={
           bpe.decode(logits_tokstr): logits_tokid
           for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
         },
         buffered_token_head=buffered_token_head
       )
       return model, extras
-      
-    self._model, self._extras = self._ld.get_model_internal(self.llm, load_model)
+
+    self._model, self._extras = self._ld._get_model_internal(
+      self._llm, load_model
+    )
     self._logits = None
     self._state = None
     self._next_token = None
-  
+
   def _heal_token(self, tok_a: int, tok_b: int) -> str:
     return self._extras.tokenizer.decode([tok_a, tok_b])
-  
+
   def set_state(self, state: Optional[TransformersState]):
     if state is None:
       self._logits = None
       self._state = None
       self._next_token = None
     else:
       self._logits = copy.deepcopy(state._logits)
       self._state = copy.deepcopy(state._state)
       self._next_token = state._next_token
-    
+
   def clone_state(self) -> TransformersState:
     return TransformersState(
-      _logits = copy.deepcopy(self._logits),
-      _state = copy.deepcopy(self._state),
-      _next_token = self._next_token,
+      _logits=copy.deepcopy(self._logits),
+      _state=copy.deepcopy(self._state),
+      _next_token=self._next_token,
     )
-  
+
   def _eval(self, tokid: int):
     if model_is_rwkv(self._model):
       outputs = self._model.forward(
-        torch.IntTensor([tokid]),
-        state=self._state,
-        use_cache=True
+        torch.IntTensor([tokid]), state=self._state, use_cache=True
       )
       self._state = outputs.state
     else:
       outputs = self._model.forward(
-        torch.IntTensor([tokid]),
-        past_key_values=self._state,
-        use_cache=True
+        torch.IntTensor([tokid]), past_key_values=self._state, use_cache=True
       )
       self._state = outputs.past_key_values
     return outputs.logits[-1]
-  
+
   def decode(self, tokids: List[int]) -> str:
     return self._extras.tokenizer.decode(tokids)
-  
+
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return self._extras.tokenizer.encode(text, add_special_tokens=add_special_tokens).tolist()
-  
+    return self._extras.tokenizer.encode(
+      text, add_special_tokens=add_special_tokens
+    ).tolist()
+
   def next_token_probs(self):
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       if model_is_rwkv(self._model):
@@ -133,82 +139,87 @@
       else:
         logits = self._model.forward(
           torch.IntTensor([self._next_token[0]]),
           past_key_values=self._state,
           use_cache=True
         )._logits[-1]
     return sampling.logits_to_probs(logits).tolist()
-  
-  def _infer(self,
-            end: Optional[Union[str, int]],
-            args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
+
+  def _infer(self, end: Optional[Union[str, int]],
+             args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
     stops_at_eot = (
       (isinstance(end, str) and len(end) == 0) or
       (isinstance(end, int) and end == self._extras.tokenizer.eos_token_id)
     )
     eot_tok = self._extras.tokenizer.eos_token_id
-    
+
+    if self._logits is None:
+      raise ValueError("no prompt provided for TransformersModel")
+
     for i in range(args.max_new_tokens):
       strip_left = None
-      
+
       if i == 0 and self._next_token is not None:
         tokid, tokstr = self._next_token
-        
+
         for logits_tokstr, logits_tokid in self._extras.vocab:
           if not logits_tokstr.startswith(tokstr):
             self._logits[logits_tokid] = -inf
-          
+
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
           self._logits = self._eval(tokid)
         else:
           strip_left = tokstr
-      
-      if not stops_at_eot: # no early endoftext
+
+        self._next_token = None
+
+      if not stops_at_eot:  # no early endoftext
         self._logits[0] = -inf
-      
+
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
-      
+
       if stops_at_eot and tokid == eot_tok:
         break
       elif tokid in self._extras.buffered_token_head:
         buffered_tokens.append(tokid)
       else:
         if buffered_tokens:
           tokstr = self._extras.tokenizer.decode(buffered_tokens + [tokid])
           buffered_tokens = []
         else:
           tokstr = self._extras.tokenizer.decode([tokid])
-        
+
         if strip_left and tokstr.startswith(tokstr):
           tokstr = tokstr[len(strip_left):]
-        
+
         self._next_token = (tokid, tokstr)
-        
+
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
-      
+
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
-      
+
       self._logits = self._eval(tokid)
-    
+
     yield RespInfer(tokid=-1, tokstr="", running_infer=generated)
 
+
 class TransformersModel(LLM[TransformersSession]):
   """
   transformers model.
   """
   Session = TransformersSession
-  
+
   def __init__(self, model_name: str, tokenizer_name: Optional[str] = None):
     """
     Creates a template for a language model powered by the transformers library.
     
     Args:
       model_name (str):
         The name of the model.
```

### Comparing `langdash-0.0.6.dev1/langdash/response.py` & `langdash-1.0.0a1/langdash/response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from dataclasses import dataclass
 
+
 class Response:
   """ Base class for responses from language model """
   pass
 
+
 @dataclass
 class RespReturns(Response):
   """
   Returns response. Acts as a header for return values.
   
   Attributes:
     key: Return key
   """
   key: str
 
+
 @dataclass
 class RespInfer(Response):
   """
   Inference response. Will be emitted on every token generated.
   
   Attributes:
     tokid: Token ID, or -1 if last inference
     tokstr: Token string representation, or empty string if last inference
     running_infer: Current generated string
   """
   tokid: int
   tokstr: str
   running_infer: str
 
+
 @dataclass
 class RespInject(Response):
   """
   Injected response. Will be emitted every time new context is injected.
   
   Attributes:
     tokens_counter: Number of tokens injected to model
```

### Comparing `langdash-0.0.6.dev1/langdash/sampling.py` & `langdash-1.0.0a1/langdash/sampling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 from typing import List
 from langdash.infer import InferArgs
 
 import torch
 from torch.nn import functional as F
 
+
 @torch.jit.script
 def _sample_top_p(logits: torch.Tensor, top_p: float) -> torch.Tensor:
   assert 0.0 <= top_p <= 1.0, "top_p must be in [0.0, 1.0]"
   probs = F.softmax(logits, dim=-1)
   sorted_probs = torch.sort(probs, descending=True)[0]
   cumulative_probs = torch.cumsum(sorted_probs, dim=-1)
   cutoff = float(sorted_probs[torch.argmax((cumulative_probs > top_p).long())])
   probs[probs < cutoff] = 0
   return probs
 
+
 @torch.jit.script
 def _sample_typical(logits: torch.Tensor, mass: float) -> torch.Tensor:
   # https://github.com/huggingface/transformers/compare/main...cimeister:typicalsampling:typical-pr
   assert 0.0 <= mass <= 1.0, "typical mass must be in [0.0, 1.0]"
-  
+
   probs = F.softmax(logits, dim=-1)
   normalized = -torch.log(probs)
   ent = torch.nansum(normalized * probs, dim=-1, keepdim=True)
-  
+
   shifted_scores = torch.abs(logits - ent)
   sorted_scores, sorted_indices = torch.sort(shifted_scores, descending=False)
   sorted_logits = logits.gather(-1, sorted_indices)
   cumulative_probs = sorted_logits.softmax(dim=-1).cumsum(dim=-1)
-  
+
   I = (cumulative_probs < mass).sum()
   probs[shifted_scores > sorted_scores[I]] = 0.
   return probs
 
+
 def _output_probs(
-  logits: torch.FloatTensor,
-  args: InferArgs,
-  ctx: List[int]
+  logits: torch.FloatTensor, args: InferArgs, ctx: List[int]
 ) -> torch.Tensor:
   # apply repetition penalty
   if args.rep_penalty != 1.0:
     rep_penalty = args.rep_penalty
     assert 0.0 <= rep_penalty, "rep_penalty must be in [0.0, inf]"
     for _, tok in zip(range(args.max_rep_ctx), reversed(ctx)):
       if logits[tok] < 0.0:
         logits[tok] *= rep_penalty
       else:
         logits[tok] /= rep_penalty
-  
+
   # probabilities
   if args.typical_mass > 0.0:
     # typical
     probs = _sample_typical(logits, args.typical_mass)
   else:
     # top-p
     probs = _sample_top_p(logits, args.top_p)
-  
+
   # apply temperature
   if args.temperature != 1.0:
     probs = probs.pow(1.0 / args.temperature)
-    
+
   return probs
 
+
 def sample(*args, **kwargs) -> int:
   """
   Sample from a distribution of tokens specified by *logits*.
   
   Args:
     logits (torch.FloatTensor): Logits to sample from.
     args (InferArgs): Sampling arguments.
     ctx (List[int]): List of tokens generated so far.
   
   Returns:
     The token sampled.
   """
   probs = _output_probs(*args, **kwargs)
   return int(torch.multinomial(probs, num_samples=1)[0])
-  
+
+
 def logits_to_probs(logits: torch.Tensor):
   """ Converts logit tensor to probability tensor using softmax. """
-  return torch.nn.functional.softmax(logits, dim=-1)
+  return torch.nn.functional.softmax(logits, dim=-1)
```

### Comparing `langdash-0.0.6.dev1/langdash/search/embedding_search.py` & `langdash-1.0.0a1/langdash/search/embedding_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import faiss
-from typing import Generator, Tuple
-  
+from typing import Generator, Tuple, List, Union
+
 from langdash.llm_session import LLMEmbeddingSession
 from langdash.search.engine import Engine
 
+
 class EmbeddingSearch(Engine):
-  
+  """ A search engine that uses vector embeddings from a language model. """
+
+  _documents: List[str]
+
   def __init__(
     self,
     embd_session: LLMEmbeddingSession,
   ):
     self._embd_session = embd_session
     self._embds = faiss.IndexFlatIP(self._embd_session.embedding_size())
     self._documents = []
-  
-  def add(self, text: str):
-    self._documents.append(text)
-    self._embds.add(self._embd_session.embed([text]))
-    
-  def search(self, text: str, max_documents: int = 1) -> Generator[Tuple[str, float], None, None]:
-    embd = self._embd_model.embed([text])
+
+  def add(self, texts: Union[str, List[str]]):
+    if isinstance(texts, str):
+      self._documents.append(texts)
+      self._embds.add(self._embd_session.embed([texts]))
+    else:
+      self._documents += texts
+      self._embds.add(self._embd_session.embed(texts))
+
+  def search(
+    self,
+    text: str,
+    max_documents: int = 1
+  ) -> Generator[Tuple[str, float], None, None]:
+    embd = self._embd_session.embed([text])
     if max_documents == -1:
       max_documents = len(self._documents)
     D, I = self._embds.search(embd, max_documents)
     for d, i in zip(D[0], I[0]):
       yield self._documents[i], d
```

### Comparing `langdash-0.0.6.dev1/langdash/search/multichoice_search.py` & `langdash-1.0.0a1/langdash/search/multichoice_search.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,97 @@
-from typing import Generator, Callable, Tuple
+from typing import Generator, Callable, Tuple, List, Union
 from langdash.chains import LDChainCached
 from langdash.search.engine import Engine
 
-def number_based_prompt(search: "MultichoiceSearch", key: int, document: str) -> Tuple[str, str]:
+
+def number_based_prompt(search: "MultichoiceSearch", key: int,
+                        document: str) -> Tuple[str, str]:
   return str(key), f"{key}. {document}\n"
 
+
 class MultichoiceSearch(Engine):
-  
-  def __init__(self,
-               prompt_chain: LDChainCached,
-               document_prompt: Callable[["MultichoiceSearch", int, str], Tuple[str, str]] = number_based_prompt):
+  """
+  A search engine that uses multiple choice questions to ask the most
+  relevant documents from a generative language model.
+  """
+
+  _documents: List[str]
+  _keys: List[str]
+  _key_tokens: List[int]
+
+  def __init__(
+    self,
+    prompt_chain: LDChainCached,
+    document_prompt: Callable[["MultichoiceSearch", int, str],
+                              Tuple[str, str]] = number_based_prompt
+  ):
     self._prompt_chain = prompt_chain
-    assert self._prompt_chain.argtype("prompts") == str, "prompt must have prompts argument"
-    assert self._prompt_chain.argtype("query") == str, "prompt must have query argument"
+    assert self._prompt_chain.argtype(
+      "prompts"
+    ) == str, "prompt must have prompts argument"
+    assert self._prompt_chain.argtype(
+      "query"
+    ) == str, "prompt must have query argument"
     self._needs_update = False
     self._prompts = ""
     self._documents = []
     self._document_prompt = document_prompt
     self._keys = []
     self._key_tokens = []
-  
-  def add(self, text: str):
-    self._documents.append(text)
+
+  def add(self, texts: Union[str, List[str]]):
+    if isinstance(texts, str):
+      self._documents.append(texts)
+    else:
+      self._documents += texts
     self._needs_update = True
-  
+
   def _update_session(self):
     self._keys.clear()
     self._key_tokens.clear()
     self._prompts = ""
     for idx, document in enumerate(self._documents):
       key, prompt = self._document_prompt(self, idx, document)
       self._prompts += prompt
       self._keys.append(key)
-  
-  def search(self, text: str, max_documents: int = 1) -> Generator[Tuple[str, float], None, None]:
+
+  def search(
+    self,
+    text: str,
+    max_documents: int = 1
+  ) -> Generator[Tuple[str, float], None, None]:
     if not self._documents:
       return
-    
+
     if self._needs_update:
       self._update_session()
       self._needs_update = False
-      
-    _, session = self._prompt_chain.call(args={
-      "prompts":self._prompts,
-      "query":text
-    }, return_session=True)
-    
+
+    _, session = self._prompt_chain.call(
+      args={
+        "prompts": self._prompts,
+        "query": text
+      }, return_session=True
+    )
+
     if not self._key_tokens:
       for token in self._keys:
         tokens = session.tokenize(token)
         assert len(tokens) == 1
         self._key_tokens.append(tokens[0])
-    
+
     tok_probs = session.next_token_probs()
-    
-    doc_probs = [0.] * len(self._documents)
-    for idx, token in enumerate(self._key_tokens):
-      doc_probs[idx] = float(tok_probs[token])
-      
+
+    doc_probs: List[float] = [0.] * len(self._documents)
+    for idx, token in enumerate(self._key_tokens):  # type: ignore
+      doc_probs[idx] = tok_probs[token]
+
     doc_probs_sum = sum(doc_probs)
     for idx in range(len(doc_probs)):
       doc_probs[idx] /= doc_probs_sum
-      
-    doc_probs_with_text = list(zip(doc_probs, self._documents))
-    doc_probs_with_text.sort(key=lambda x: x[0], reverse=True)
+
+    doc_probs_with_text = list(zip(self._documents, doc_probs))
+    doc_probs_with_text.sort(key=lambda x: x[1], reverse=True)
     if max_documents == -1:
       yield from iter(doc_probs_with_text)
     else:
-      yield from iter(doc_probs_with_text[0:max_documents])
+      yield from iter(doc_probs_with_text[0:max_documents])
```

### Comparing `langdash-0.0.6.dev1/langdash.egg-info/SOURCES.txt` & `langdash-1.0.0a1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.6.dev1/setup.py` & `langdash-1.0.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,35 +15,36 @@
     description='A simple library for interfacing with language models.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Nana Mochizuki',
     author_email='nana@mysymphony.jp.net',
     url='https://git.mysymphony.jp.net/nana/langdash',
     classifiers=[
-      'Development Status :: 3 - Alpha',
-      'Intended Audience :: Developers',
-      'Topic :: Software Development :: Libraries',
-      'License :: OSI Approved :: Apache Software License',
-      'Programming Language :: Python :: 3',
-      'Programming Language :: Python :: 3.8',
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries',
+        'License :: OSI Approved :: Apache Software License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
     ],
     project_urls={
-      'Source': 'https://git.mysymphony.jp.net/nana/langdash',
-      'Documentation': 'https://langdash.readthedocs.io/en/latest/',
+        'Source': 'https://git.mysymphony.jp.net/nana/langdash',
+        'Documentation': 'https://langdash.readthedocs.io/en/latest/',
     },
     # requirements
     python_requires='>=3.8',
-    packages=find_packages(include=['langdash', 'langdash.*'], exclude=['extern']),
+    packages=find_packages(
+        include=['langdash', 'langdash.*'], exclude=['extern']),
     install_requires=[
-      'torch',
+        'torch',
     ],
     extras_require={
-      # Modules
-      "embeddings": ["faiss"],
-          
-      # Backend
-      "rwkv_cpp": ["tokenizers"],
-      "llama_cpp": ["llama-cpp-python==0.1.57"],
-      "transformers": ["transformers"],
-      "sentence_transformers": ["sentence_transformers"],
+        # Modules
+        "embeddings": ["faiss-cpu"],
+
+        # Backend
+        "rwkv_cpp": ["tokenizers"],
+        "llama_cpp": ["llama-cpp-python==0.1.57"],
+        "transformers": ["transformers"],
+        "sentence_transformers": ["sentence_transformers"],
     },
-)
+)
```

