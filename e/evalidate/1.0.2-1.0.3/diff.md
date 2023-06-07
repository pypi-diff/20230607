# Comparing `tmp/evalidate-1.0.2.tar.gz` & `tmp/evalidate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalidate-1.0.2.tar", last modified: Thu Oct 20 08:34:01 2022, max compression
+gzip compressed data, was "evalidate-1.0.3.tar", last modified: Wed Jun  7 10:57:35 2023, max compression
```

## Comparing `evalidate-1.0.2.tar` & `evalidate-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2022-10-20 08:34:01.668030 evalidate-1.0.2/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    15051 2022-10-20 08:34:01.668030 evalidate-1.0.2/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)    11978 2022-08-28 16:58:46.000000 evalidate-1.0.2/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2022-10-20 08:34:01.664030 evalidate-1.0.2/evalidate/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4279 2022-08-28 13:33:02.000000 evalidate-1.0.2/evalidate/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2376 2022-08-28 14:39:14.000000 evalidate-1.0.2/evalidate/security.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2022-10-20 08:34:01.668030 evalidate-1.0.2/evalidate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    15051 2022-10-20 08:34:01.000000 evalidate-1.0.2/evalidate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2022-10-20 08:34:01.000000 evalidate-1.0.2/evalidate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2022-10-20 08:34:01.000000 evalidate-1.0.2/evalidate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2022-08-10 17:45:22.000000 evalidate-1.0.2/evalidate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2022-10-20 08:34:01.000000 evalidate-1.0.2/evalidate.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2022-10-20 08:34:01.668030 evalidate-1.0.2/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)      580 2022-08-28 14:29:21.000000 evalidate-1.0.2/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-07 10:57:35.030697 evalidate-1.0.3/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    16301 2023-06-07 10:57:35.030697 evalidate-1.0.3/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    12915 2023-06-07 10:56:21.000000 evalidate-1.0.3/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-07 10:57:35.030697 evalidate-1.0.3/evalidate/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     5480 2023-05-30 08:23:52.000000 evalidate-1.0.3/evalidate/__init__.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2376 2023-05-30 08:23:52.000000 evalidate-1.0.3/evalidate/security.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-06-07 10:57:35.030697 evalidate-1.0.3/evalidate.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    16301 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2021-09-12 11:08:09.000000 evalidate-1.0.3/evalidate.egg-info/not-zip-safe
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-06-07 10:57:34.000000 evalidate-1.0.3/evalidate.egg-info/top_level.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-06-07 10:57:35.030697 evalidate-1.0.3/setup.cfg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      876 2023-06-07 10:56:28.000000 evalidate-1.0.3/setup.py
```

### Comparing `evalidate-1.0.2/PKG-INFO` & `evalidate-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe eval()'uating user-supplied (possible malicious) logical expressions in python syntax.
@@ -313,29 +313,35 @@
         
         [asteval](https://newville.github.io/asteval/)
         
         While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
         - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
         - user can provide source code which runs very long time and consumes many resources 
         
+        
+        [simpleeval](https://github.com/danthedeckie/simpleeval)
+        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
+        
+        
         evalidate is good to run short same code against different data.
         
         ## Benchmarking
-        We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository
+        We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository.
+        We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
+        
         ~~~
-        $ ./evalidate-vs-asteval.py 
-        Src: a+b
-        Context: {'a': 1, 'b': 2}
-        Runs: 100000
-        asteval: 3.538s
-        asteval (reuse interpreter): 1.232s
-        safeeval: 2.384s
-        evalidate/compile/eval (reuse compiled code): 0.017s
+        Products: 1000000 items
+        test_asteval_products(): 25.920s
+        test_simpleeval_products(): 1.779s
+        test_evalidate_products(): 0.160s
         ~~~
-        0.017s vs 1.232s
+        
+        As you see, evalidate is almost 10 times faster then simpleeval and both are much faster then asteval.
+        
+        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
         
         
         ## Read about eval() risks
         
         - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
         - https://netsec.expert/posts/breaking-python3-eval-protections/
         - https://realpython.com/python-eval-function/
@@ -348,8 +354,14 @@
         Want more info? Check source code of module, it's very short and simple, easy to modify
         
         ## Contact
         
         Write me: yaroslaff at gmail.com
         
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Interpreters
 Description-Content-Type: text/markdown
```

### Comparing `evalidate-1.0.2/README.md` & `evalidate-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -305,29 +305,35 @@
 
 [asteval](https://newville.github.io/asteval/)
 
 While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
 - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
 - user can provide source code which runs very long time and consumes many resources 
 
+
+[simpleeval](https://github.com/danthedeckie/simpleeval)
+Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
+
+
 evalidate is good to run short same code against different data.
 
 ## Benchmarking
-We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository
+We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository.
+We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
+
 ~~~
-$ ./evalidate-vs-asteval.py 
-Src: a+b
-Context: {'a': 1, 'b': 2}
-Runs: 100000
-asteval: 3.538s
-asteval (reuse interpreter): 1.232s
-safeeval: 2.384s
-evalidate/compile/eval (reuse compiled code): 0.017s
+Products: 1000000 items
+test_asteval_products(): 25.920s
+test_simpleeval_products(): 1.779s
+test_evalidate_products(): 0.160s
 ~~~
-0.017s vs 1.232s
+
+As you see, evalidate is almost 10 times faster then simpleeval and both are much faster then asteval.
+
+Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
 
 
 ## Read about eval() risks
 
 - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
 - https://netsec.expert/posts/breaking-python3-eval-protections/
 - https://realpython.com/python-eval-function/
```

### Comparing `evalidate-1.0.2/evalidate/__init__.py` & `evalidate-1.0.3/evalidate/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/python
 
 """Safe user-supplied python expression evaluation."""
 
 import ast
-import sys
+
+__version__ = '1.0.2'
 
 
 class EvalException(Exception):
     pass
 
+
 class ValidationException(EvalException):
     pass
 
+
 class CompilationException(EvalException):
     exc = None
     def __init__(self, exc):
         super().__init__(exc)
         self.exc = exc
 
+
 class ExecutionException(EvalException):
     exc = None
     def __init__(self, exc):
         super().__init__(exc)
         self.exc = exc
 
 
@@ -46,52 +50,51 @@
             # variable name
             variables = ['Name', 'Load']
             binop = ['BinOp']
             arithmetics = ['Add', 'Sub']
             subscript = ['Subscript', 'Index']  # person['name']
             boolop = ['BoolOp', 'And', 'Or', 'UnaryOp', 'Not']  # True and True
             inop = ["In", "NotIn"]  # "aaa" in i['list']
-            ifop = ["IfExp"] # for if expressions, like: expr1 if expr2 else expr3
-            nameconst = ["NameConstant"] # for True and False constants
+            ifop = ["IfExp"]  # for if expressions, like: expr1 if expr2 else expr3
+            nameconst = ["NameConstant"]  # for True and False constants
             div = ["Div", "Mod"]
 
             self.allowed = expression + constant + values + compare + \
                 variables + binop + arithmetics + subscript + boolop + \
                 inop + ifop + nameconst + div
 
         self.allowed_funcs = funcs or list()
         self.allowed_attrs = attrs or list()
 
         if addnodes is not None:
             self.allowed = self.allowed + addnodes
 
     def generic_visit(self, node):
         """Check node, raise exception if node is not in whitelist."""
-        
+
         if type(node).__name__ in self.allowed:
 
             if isinstance(node, ast.Attribute):
                 if node.attr not in self.allowed_attrs:
                     raise ValidationException(
                         "Attribute {aname} is not allowed".format(
-                            aname=node.attr))    
-                        
+                            aname=node.attr))
 
             if isinstance(node, ast.Call):
                 if isinstance(node.func, ast.Name):
                     if node.func.id not in self.allowed_funcs:
                         raise ValidationException(
                             "Call to function {fname}() is not allowed".format(
-                                fname=node.func.id))    
+                                fname=node.func.id))
                     else:
                         # Call to allowed function. good. No exception
-                        pass            
+                        pass
                 elif isinstance(node.func, ast.Attribute):
                     pass
-                    # print("attr:", node.func.attr)                                        
+                    # print("attr:", node.func.attr)
                 else:
                     raise ValidationException('Indirect function call')
 
             ast.NodeVisitor.generic_visit(self, node)
         else:
             raise ValidationException(
                 "Operation type {optype} is not allowed".format(
@@ -105,22 +108,60 @@
     or pass exception from SafeAST visit.
     """
     try:
         node = ast.parse(expression, '<usercode>', 'eval')
     except SyntaxError as e:
         raise CompilationException(e)
 
-
     v = SafeAST(safenodes, addnodes, funcs, attrs)
     v.visit(node)
     return node
 
 
 def safeeval(expression, context={}, safenodes=None, addnodes=None, funcs=None, attrs=None):
-    """C-style simplified wrapper, eval() replacement."""
+    """C-style simplified wrapper, eval() replacement.
+
+    Args:
+        expr (str): the expression to evaluate
+
+        safenodes (List[str] | None):
+            Specify the name of allowed AST nodes, if unspecified a default list is used.
+
+        addnodes (List[str] | None):
+            List of additional AST node names to allow in addition to safenodes.
+
+        funcs (List[str]):
+            list of allowed function names.
+
+        attrs (List[str]):
+            list of allowed attribute names.
+
+    Returns:
+        Any: the result of the expression
+
+    Raises:
+        ExecutionException - if the expression fails to execute
+        CompilationException - if the expression fails to parse
+        ValidationException - if the expression fails safety checks
+
+    Example:
+        >>> import evalidate
+        >>> evalidate.safeeval('3 + 2')
+        5
+        >>> evalidate.safeeval('max(3, 2)')
+        Traceback (most recent call last):
+            ...
+        evalidate.ValidationException: Operation type Call is not allowed
+        >>> evalidate.safeeval('max(3, 2)', addnodes=['Call'])
+        Traceback (most recent call last):
+            ...
+        evalidate.ValidationException: Call to function max() is not allowed
+        >>> evalidate.safeeval('max(3, 2)', addnodes=['Call'], funcs=['max'])
+        3
+    """
 
     # ValidationException thrown here
     node = evalidate(expression, safenodes, addnodes, funcs, attrs)
 
     code = compile(node, '<usercode>', 'eval')
 
     wcontext = context.copy()
```

### Comparing `evalidate-1.0.2/evalidate/security.py` & `evalidate-1.0.3/evalidate/security.py`

 * *Files identical despite different names*

### Comparing `evalidate-1.0.2/evalidate.egg-info/PKG-INFO` & `evalidate-1.0.3/evalidate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalidate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Validation and secure evaluation of untrusted python expressions
 Home-page: http://github.com/yaroslaff/evalidate
 Author: Yaroslav Polyakov
 Author-email: xenon@sysattack.com
 License: MIT
 Description: ﻿# Evalidate
         Evalidate is simple python module for safe eval()'uating user-supplied (possible malicious) logical expressions in python syntax.
@@ -313,29 +313,35 @@
         
         [asteval](https://newville.github.io/asteval/)
         
         While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
         - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
         - user can provide source code which runs very long time and consumes many resources 
         
+        
+        [simpleeval](https://github.com/danthedeckie/simpleeval)
+        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is ~10 times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
+        
+        
         evalidate is good to run short same code against different data.
         
         ## Benchmarking
-        We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository
+        We use `evalidate-vs-asteval.py` which is in benchmark/ directory of repository.
+        We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
+        
         ~~~
-        $ ./evalidate-vs-asteval.py 
-        Src: a+b
-        Context: {'a': 1, 'b': 2}
-        Runs: 100000
-        asteval: 3.538s
-        asteval (reuse interpreter): 1.232s
-        safeeval: 2.384s
-        evalidate/compile/eval (reuse compiled code): 0.017s
+        Products: 1000000 items
+        test_asteval_products(): 25.920s
+        test_simpleeval_products(): 1.779s
+        test_evalidate_products(): 0.160s
         ~~~
-        0.017s vs 1.232s
+        
+        As you see, evalidate is almost 10 times faster then simpleeval and both are much faster then asteval.
+        
+        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. But benchmark code must assume expression as unknown and untrusted.
         
         
         ## Read about eval() risks
         
         - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
         - https://netsec.expert/posts/breaking-python3-eval-protections/
         - https://realpython.com/python-eval-function/
@@ -348,8 +354,14 @@
         Want more info? Check source code of module, it's very short and simple, easy to modify
         
         ## Contact
         
         Write me: yaroslaff at gmail.com
         
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Interpreters
 Description-Content-Type: text/markdown
```

