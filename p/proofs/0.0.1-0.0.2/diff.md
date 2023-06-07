# Comparing `tmp/proofs-0.0.1.tar.gz` & `tmp/proofs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofs-0.0.1.tar", last modified: Tue Jun  6 03:36:18 2023, max compression
+gzip compressed data, was "proofs-0.0.2.tar", last modified: Wed Jun  7 01:30:27 2023, max compression
```

## Comparing `proofs-0.0.1.tar` & `proofs-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-06 03:36:18.770922 proofs-0.0.1/
--rw-r--r--   0 max        (501) staff       (20)    11337 2023-06-01 10:05:52.000000 proofs-0.0.1/LICENSE
--rw-r--r--   0 max        (501) staff       (20)      111 2023-06-01 10:05:52.000000 proofs-0.0.1/MANIFEST.in
--rw-r--r--   0 max        (501) staff       (20)     7471 2023-06-06 03:36:18.770811 proofs-0.0.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     5212 2023-06-01 10:15:54.000000 proofs-0.0.1/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-06 03:36:18.769518 proofs-0.0.1/proofs/
--rw-r--r--   0 max        (501) staff       (20)       22 2023-06-01 10:15:51.000000 proofs-0.0.1/proofs/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     1094 2023-06-01 10:15:51.000000 proofs-0.0.1/proofs/_modidx.py
--rw-r--r--   0 max        (501) staff       (20)      146 2023-06-01 10:15:51.000000 proofs-0.0.1/proofs/assistant.py
--rw-r--r--   0 max        (501) staff       (20)     5276 2023-06-01 10:15:51.000000 proofs-0.0.1/proofs/core.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-06 03:36:18.770617 proofs-0.0.1/proofs.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     7471 2023-06-06 03:36:18.000000 proofs-0.0.1/proofs.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      334 2023-06-06 03:36:18.000000 proofs-0.0.1/proofs.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-06-06 03:36:18.000000 proofs-0.0.1/proofs.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       55 2023-06-06 03:36:18.000000 proofs-0.0.1/proofs.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-06-06 03:31:59.000000 proofs-0.0.1/proofs.egg-info/not-zip-safe
--rw-r--r--   0 max        (501) staff       (20)     1863 2023-06-06 03:36:18.000000 proofs-0.0.1/proofs.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        7 2023-06-06 03:36:18.000000 proofs-0.0.1/proofs.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)     3213 2023-06-06 03:30:45.000000 proofs-0.0.1/settings.ini
--rw-r--r--   0 max        (501) staff       (20)       38 2023-06-06 03:36:18.770963 proofs-0.0.1/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)     2596 2023-06-01 10:05:52.000000 proofs-0.0.1/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-07 01:30:27.976536 proofs-0.0.2/
+-rw-r--r--   0 max        (501) staff       (20)    11337 2023-06-01 10:05:52.000000 proofs-0.0.2/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)      111 2023-06-01 10:05:52.000000 proofs-0.0.2/MANIFEST.in
+-rw-r--r--   0 max        (501) staff       (20)     7552 2023-06-07 01:30:27.976380 proofs-0.0.2/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     5269 2023-06-07 01:25:51.000000 proofs-0.0.2/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-07 01:30:27.974910 proofs-0.0.2/proofs/
+-rw-r--r--   0 max        (501) staff       (20)       22 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     1336 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/_modidx.py
+-rw-r--r--   0 max        (501) staff       (20)      146 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/assistant.py
+-rw-r--r--   0 max        (501) staff       (20)     7706 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/core.py
+-rw-r--r--   0 max        (501) staff       (20)      155 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/polynomials.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-07 01:30:27.976112 proofs-0.0.2/proofs.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     7552 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      356 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       55 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-06-06 03:31:59.000000 proofs-0.0.2/proofs.egg-info/not-zip-safe
+-rw-r--r--   0 max        (501) staff       (20)     1863 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        7 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)     2768 2023-06-07 01:30:25.000000 proofs-0.0.2/settings.ini
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-06-07 01:30:27.976591 proofs-0.0.2/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)     2596 2023-06-01 10:05:52.000000 proofs-0.0.2/setup.py
```

### Comparing `proofs-0.0.1/LICENSE` & `proofs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proofs-0.0.1/PKG-INFO` & `proofs-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mathematical proof assistant for students and amateurs.
 Home-page: https://github.com/maxtheman/proofs
 Author: maxtheman
 Author-email: proofs@growth.wtf
 License: Apache Software License 2.0
 Description: # proofs
         
@@ -76,15 +76,15 @@
             x + 1
         
         ``` python
         # select a few examples from the reals
         make_examples('real', 3, expression)
         ```
         
-            [(-92, -91), (59, 60), (80, 81)]
+            [(-57, -56), (-100, -99), (-31, -30)]
         
         Hopefully these examples convice us that the statement is false. This
         suggests that we can prove it by contradiction.
         
         ``` python
         # Then define your goal
         contradiction_goal = not_equals(expression, arbitrary_x)
@@ -95,39 +95,42 @@
         def proof_of_x_plus_one(x):
             # Given x, Assume x + 1 = x is true for arbitrary_x
             assumed_eq = equals(x + 1, x)
         
             # Calculate x + 1
             next = x + 1
         
-            # Observing x + 1 $\neq$ x, we have reached a contradiction
+            # Observing x + 1 != x, we have reached a contradiction
             return not_equals(next, assumed_eq.rhs)
         
         #Select an arbitrary x from the domain
         prove(contradiction_goal, proof_of_x_plus_one, arbitrary_x)
         ```
         
-            <IPython.core.display.Latex object>
+        $$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary\_x}}$$
         
         $$x + 1 = x$$
         
-            <IPython.core.display.Latex object>
+        $$\mathtt{\text{Calculate x + 1}}$$
         
         $$x + 1$$
         
-            <IPython.core.display.Latex object>
+        $$\mathtt{\text{Observing x + 1 != x, we have reached a contradiction}}$$
         
         $$\text \quad x + 1 \neq x \quad Q.E.D.$$
         
             True
         
-        With this, we get: 1. comments converted to latex, along with latex
-        rendering of the math we are doing in python 2. validation that what we
-        are returning from the proof matches the expected goal 3. some
-        additional helpful errors
+        With this, we get:
+        
+        1.  Complete latex rendering of the math we are doing in python and our
+            logic
+        2.  validation that what we are returning from the proof matches the
+            expected goal
+        3.  some additional helpful errors
         
         # Next steps
         
         Likes:
         
         - simple API
```

### Comparing `proofs-0.0.1/README.md` & `proofs-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     x + 1
 
 ``` python
 # select a few examples from the reals
 make_examples('real', 3, expression)
 ```
 
-    [(-92, -91), (59, 60), (80, 81)]
+    [(-57, -56), (-100, -99), (-31, -30)]
 
 Hopefully these examples convice us that the statement is false. This
 suggests that we can prove it by contradiction.
 
 ``` python
 # Then define your goal
 contradiction_goal = not_equals(expression, arbitrary_x)
@@ -87,39 +87,42 @@
 def proof_of_x_plus_one(x):
     # Given x, Assume x + 1 = x is true for arbitrary_x
     assumed_eq = equals(x + 1, x)
 
     # Calculate x + 1
     next = x + 1
 
-    # Observing x + 1 $\neq$ x, we have reached a contradiction
+    # Observing x + 1 != x, we have reached a contradiction
     return not_equals(next, assumed_eq.rhs)
 
 #Select an arbitrary x from the domain
 prove(contradiction_goal, proof_of_x_plus_one, arbitrary_x)
 ```
 
-    <IPython.core.display.Latex object>
+$$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary\_x}}$$
 
 $$x + 1 = x$$
 
-    <IPython.core.display.Latex object>
+$$\mathtt{\text{Calculate x + 1}}$$
 
 $$x + 1$$
 
-    <IPython.core.display.Latex object>
+$$\mathtt{\text{Observing x + 1 != x, we have reached a contradiction}}$$
 
 $$\text \quad x + 1 \neq x \quad Q.E.D.$$
 
     True
 
-With this, we get: 1. comments converted to latex, along with latex
-rendering of the math we are doing in python 2. validation that what we
-are returning from the proof matches the expected goal 3. some
-additional helpful errors
+With this, we get:
+
+1.  Complete latex rendering of the math we are doing in python and our
+    logic
+2.  validation that what we are returning from the proof matches the
+    expected goal
+3.  some additional helpful errors
 
 # Next steps
 
 Likes:
 
 - simple API
```

### Comparing `proofs-0.0.1/proofs/_modidx.py` & `proofs-0.0.2/proofs/_modidx.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,13 +4,16 @@
                 'doc_baseurl': '/proofs',
                 'doc_host': 'https://maxtheman.github.io',
                 'git_url': 'https://github.com/maxtheman/proofs',
                 'lib_path': 'proofs'},
   'syms': { 'proofs.assistant': {},
             'proofs.core': { 'proofs.core.constant': ('core.html#constant', 'proofs/core.py'),
                              'proofs.core.contradiction_proof': ('core.html#contradiction_proof', 'proofs/core.py'),
+                             'proofs.core.direct_proof': ('core.html#direct_proof', 'proofs/core.py'),
                              'proofs.core.equals': ('core.html#equals', 'proofs/core.py'),
                              'proofs.core.equation': ('core.html#equation', 'proofs/core.py'),
                              'proofs.core.make_examples': ('core.html#make_examples', 'proofs/core.py'),
                              'proofs.core.not_equals': ('core.html#not_equals', 'proofs/core.py'),
+                             'proofs.core.print_proof': ('core.html#print_proof', 'proofs/core.py'),
                              'proofs.core.prove': ('core.html#prove', 'proofs/core.py'),
-                             'proofs.core.variable': ('core.html#variable', 'proofs/core.py')}}}
+                             'proofs.core.variable': ('core.html#variable', 'proofs/core.py')},
+            'proofs.polynomials': {}}}
```

### Comparing `proofs-0.0.1/proofs/core.py` & `proofs-0.0.2/proofs/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['Var', 'Const', 'Func', 'Goal', 'Expression', 'variable', 'constant', 'equation', 'equals', 'not_equals',
-           'make_examples', 'prove', 'contradiction_proof']
+           'make_examples', 'prove', 'print_proof', 'contradiction_proof', 'direct_proof']
 
 # %% ../nbs/00_core.ipynb 3
 from typing import Callable, List, Tuple, Union
 from sympy import Equality, Unequality
 from sympy.core.relational import Relational
 from sympy.core.basic import Basic
 from random import randint, seed
 import sympy as sp
 
-from IPython.display import display, Latex
+from IPython.display import display, Latex, HTML
 
 import typing
 import inspect
 
-# %% ../nbs/00_core.ipynb 4
+# %% ../nbs/00_core.ipynb 5
 # Basic types
 Var = sp.Symbol
 Const = sp.Number
 Func = Callable[[Var], sp.Expr]
 Goal = Union[Equality, Unequality, Relational]
 Expression = Union[sp.Expr, Basic]
 
@@ -39,16 +39,19 @@
 
 def equals(lhs: sp.Expr, rhs: sp.Expr) -> Equality:
     return sp.Eq(lhs, rhs, evaluate=False)
 
 def not_equals(lhs: Expression, rhs: Expression) -> Unequality:
     return sp.Ne(lhs, rhs, evaluate=False)
 
-# %% ../nbs/00_core.ipynb 5
-def make_examples(domain: str, N: int, equation: str) -> List[Tuple[sp.Expr, sp.Expr]]:
+# %% ../nbs/00_core.ipynb 7
+def make_examples(domain: str, #Domain of the example equation
+                  N: int, #Number of examples
+                  equation: str #Equation to generate examples for
+                  ) -> List[Tuple[sp.Expr, sp.Expr]]: #List of input-output pairs
     """For a given domain and equation, select N examples and generate a list of N input-output pairs.
     Currently, the domain can be either 'real' or 'integer', and one variable is assumed."""
     examples = []
     if domain == 'real':
         # select N random real numbers
         for _ in range(N):
             x = sp.Symbol('x')
@@ -58,71 +61,119 @@
     elif domain == 'integer':
         # select N random integers
         for _ in range(N):
             x = sp.Symbol('x', integer=True)
             x_val = randint(-100, 100)
             y_val = sp.sympify(equation).subs(x, x_val)
             examples.append((x_val, y_val))
+    else:
+        raise ValueError(f"Domain {domain} not supported.")
     return examples
 
-# %% ../nbs/00_core.ipynb 7
-def prove(goal: Goal, proof_func: Callable[..., Goal], *args) -> bool:
+# %% ../nbs/00_core.ipynb 12
+def prove(goal: Goal, #Goal to prove
+          proof_func: Callable[..., Goal], #Proof function
+          *args #Arguments to proof function
+          ) -> bool: #True if proof succeeds, False otherwise
+    """Prove a goal using a proof function and arguments.
+    The proof function should take the goal as the last argument and return the derived result.
+    The goal is proved if the derived result matches the goal."""
     try:
-        derived_goal = proof_func(*args)
-        if goal == derived_goal:
+        derived_result = proof_func(*args)
+        if goal == derived_result:
             display(Latex(f"$$\\text \\quad {sp.latex(goal)} \\quad Q.E.D.$$"))
             return True
+        else:
+            raise Exception(f"Derived result {derived_result} does not match goal {goal}")
     except Exception as e:
-        print(f"Proof error: {str(e)}")
+        print(f"Proof failed: {str(e)}")
         print("Check your assumptions and proof function for errors.")
         return False
 
-# %% ../nbs/00_core.ipynb 8
-def contradiction_proof(proof):
+# %% ../nbs/00_core.ipynb 16
+def print_proof(proof: Callable[..., Goal], # the proof function
+                 *args # the arguments to the proof function
+                 ) -> None: # no return value
+    """Print a proof step by step. Mostly used when defining a proof evaluation function.
+    The proof function should take the goal as the last argument and return the derived result.
+    The goal is proved if the derived result matches the goal.
+    Comments do not support latex formatting, but the rest of the proof does."""
+    # add all of the arguments to the local namespace with their existing names that are passed in.
+    args_list = lambda args: [_arg for _arg in args]
+    _printed = ['_formatted_comment','_i', '_arg', 'line', 'var_name','args_list', '_printed', 'var_value', 'proof', 'args', 'kwargs', 'hints']
+    #build latex string progressively and render at the end
+    for _i, _arg in enumerate(args_list(args)):
+        exec(f"{_arg} = args[{_i}]", globals(), locals())
+        _printed.append(str(_arg))
+    for _i, line in enumerate(inspect.getsourcelines(proof)[0]):
+        #print each varaible only once, and add opt outs
+        line = line.strip()
+        if line.startswith('#'):
+            # Nicely formatted representation of the comment
+            _formatted_comment = line[1:].strip()
+            display(Latex(f"$${sp.latex(_formatted_comment)}$$"))
+        if line.startswith('def'):
+            continue
+        if line.startswith('@'):
+            continue
+        if line.startswith('return'):
+            line = line[7:]
+        if line == '':
+            continue
+        exec(line, globals(), locals())
+        # print(f"\nProof state after line {i+1}: {line}")
+        for var_name, var_value in locals().items():
+            if var_name in _printed:
+                continue
+            else:
+                _printed.append(var_name)
+            # if isinstance(var_value, (Var, Const, Func)):
+            display(Latex(f"$${sp.latex(var_value)}$$"))
+
+# %% ../nbs/00_core.ipynb 19
+def contradiction_proof(proof: Callable[..., Goal] # the proof function
+                        ) -> Callable[..., Unequality]: # the wrapped contradiction proof function to evaluate
+    """Wrap a proof function to prove a contradiction.
+    The proof function should take the goal as the last argument and return the derived result.
+    The goal is proved if the derived result matches the goal."""
     def wrapper(*args, **kwargs):
         hints = typing.get_type_hints(proof)
         if hints != {}:
             if hints.get('return') != Unequality:
                 print(hints.get('return'))
                 raise TypeError("Proof function must return Unequality")
         else:
             try:
-                # add all of the arguments to the local namespace with their existing names that are passed in.
-                args_list = lambda args: [_arg for _arg in args]
-                _printed = ['_i', '_arg', 'line', 'var_name','args_list', '_printed', 'var_value', 'proof', 'args', 'kwargs', 'hints']
-                for _i, _arg in enumerate(args_list(args)):
-                    exec(f"{_arg} = args[{_i}]", globals(), locals())
-                    _printed.append(str(_arg))
-                for _i, line in enumerate(inspect.getsourcelines(proof)[0]):
-                    #print each varaible only once, and add opt outs
-                    line = line.strip()
-                    if line.startswith('#'):
-                        # in future concatenate all the strings into one doc and format nicely.
-                        # first attempt didn't work out, had weird formatting issues.
-                        display(Latex(f"{line[1:].strip()}"))
-                        continue
-                    if line.startswith('def'):
-                        continue
-                    if line.startswith('@'):
-                        continue
-                    if line.startswith('return'):
-                        line = line[7:]
-                    if line == '':
-                        continue
-                    exec(line, globals(), locals())
-                    # print(f"\nProof state after line {i+1}: {line}")
-                    for var_name, var_value in locals().items():
-                        if var_name in _printed:
-                            continue
-                        else:
-                            _printed.append(var_name)
-                        # if isinstance(var_value, (Var, Const, Func)):
-                        display(Latex(f"$${sp.latex(var_value)}$$"))
+                print_proof(proof, *args, **kwargs)
             except Exception as e:
                 print(f"Error in proof function: {str(e)}")
                 raise
             # there might be something weird around result that would prevent it from being printed if it's in the proof. check that later
             result = proof(*args, **kwargs)
             if not isinstance(result, Unequality):
                 raise TypeError("Proof function must return Unequality")
             return result
     return wrapper
+
+# %% ../nbs/00_core.ipynb 21
+def direct_proof(proof: Callable[..., Goal] # the proof function
+                        ) -> Callable[..., Equality]: # the wrapped proof function to evaluate
+    """Wrap a proof function to prove a direct proof.
+    The proof function should take the goal as the last argument and return the derived result.
+    The goal is proved if the derived result matches the goal."""
+    def wrapper(*args, **kwargs):
+        hints = typing.get_type_hints(proof)
+        if hints != {}:
+            if hints.get('return') != Equality:
+                print(hints.get('return'))
+                raise TypeError("Proof function must return Equality")
+        else:
+            try:
+                print_proof(proof, *args, **kwargs)
+            except Exception as e:
+                print(f"Error in proof function: {str(e)}")
+                raise
+            result = proof(*args, **kwargs)
+            if not isinstance(result, Equality):
+                raise TypeError("Proof function must return Equality")
+            return result
+    return wrapper
```

### Comparing `proofs-0.0.1/proofs.egg-info/PKG-INFO` & `proofs-0.0.2/proofs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mathematical proof assistant for students and amateurs.
 Home-page: https://github.com/maxtheman/proofs
 Author: maxtheman
 Author-email: proofs@growth.wtf
 License: Apache Software License 2.0
 Description: # proofs
         
@@ -76,15 +76,15 @@
             x + 1
         
         ``` python
         # select a few examples from the reals
         make_examples('real', 3, expression)
         ```
         
-            [(-92, -91), (59, 60), (80, 81)]
+            [(-57, -56), (-100, -99), (-31, -30)]
         
         Hopefully these examples convice us that the statement is false. This
         suggests that we can prove it by contradiction.
         
         ``` python
         # Then define your goal
         contradiction_goal = not_equals(expression, arbitrary_x)
@@ -95,39 +95,42 @@
         def proof_of_x_plus_one(x):
             # Given x, Assume x + 1 = x is true for arbitrary_x
             assumed_eq = equals(x + 1, x)
         
             # Calculate x + 1
             next = x + 1
         
-            # Observing x + 1 $\neq$ x, we have reached a contradiction
+            # Observing x + 1 != x, we have reached a contradiction
             return not_equals(next, assumed_eq.rhs)
         
         #Select an arbitrary x from the domain
         prove(contradiction_goal, proof_of_x_plus_one, arbitrary_x)
         ```
         
-            <IPython.core.display.Latex object>
+        $$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary\_x}}$$
         
         $$x + 1 = x$$
         
-            <IPython.core.display.Latex object>
+        $$\mathtt{\text{Calculate x + 1}}$$
         
         $$x + 1$$
         
-            <IPython.core.display.Latex object>
+        $$\mathtt{\text{Observing x + 1 != x, we have reached a contradiction}}$$
         
         $$\text \quad x + 1 \neq x \quad Q.E.D.$$
         
             True
         
-        With this, we get: 1. comments converted to latex, along with latex
-        rendering of the math we are doing in python 2. validation that what we
-        are returning from the proof matches the expected goal 3. some
-        additional helpful errors
+        With this, we get:
+        
+        1.  Complete latex rendering of the math we are doing in python and our
+            logic
+        2.  validation that what we are returning from the proof matches the
+            expected goal
+        3.  some additional helpful errors
         
         # Next steps
         
         Likes:
         
         - simple API
```

### Comparing `proofs-0.0.1/proofs.egg-info/requires.txt` & `proofs-0.0.2/proofs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `proofs-0.0.1/setup.py` & `proofs-0.0.2/setup.py`

 * *Files identical despite different names*

