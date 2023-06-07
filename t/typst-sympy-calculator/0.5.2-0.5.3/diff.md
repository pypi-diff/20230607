# Comparing `tmp/typst_sympy_calculator-0.5.2-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 35169 bytes, number of entries: 14
+Zip file size: 35273 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat     8110 b- defN 23-Jun-06 14:16 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     7723 b- defN 23-Jun-06 16:15 TypstCalculator.py
--rw-rw-rw-  2.0 fat    11040 b- defN 23-Jun-06 16:15 TypstCalculatorServer.py
--rw-rw-rw-  2.0 fat    25952 b- defN 23-Jun-06 14:16 TypstConverter.py
+-rw-rw-rw-  2.0 fat    11040 b- defN 23-Jun-07 02:50 TypstCalculatorServer.py
+-rw-rw-rw-  2.0 fat    26765 b- defN 23-Jun-07 02:49 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17703 b- defN 23-Jun-06 08:35 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-Jun-06 08:35 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-Jun-06 08:35 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-06 16:17 typst_sympy_calculator-0.5.2.dist-info/RECORD
-14 files, 197421 bytes uncompressed, 33229 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-07 02:52 typst_sympy_calculator-0.5.3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    13675 b- defN 23-Jun-07 02:52 typst_sympy_calculator-0.5.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 02:52 typst_sympy_calculator-0.5.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 02:52 typst_sympy_calculator-0.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1170 b- defN 23-Jun-07 02:52 typst_sympy_calculator-0.5.3.dist-info/RECORD
+14 files, 198234 bytes uncompressed, 33333 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.5.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.2.dist-info/METADATA
+Filename: typst_sympy_calculator-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.2.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.2.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.5.2.dist-info/RECORD
+Filename: typst_sympy_calculator-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstConverter.py

```diff
@@ -30,19 +30,27 @@
     def _print_Mul(self, expr):
         def mul(x, y):
             if x == '1':
                 return y
             if x == '-1':
                 return '-' + y
             return x + ' ' + y
-        x = expr.args[0]
-        if x.is_Pow and x.args[1].is_Number and x.args[1] < 0:
-            return (reduce(mul, [self.paren(arg) for arg in expr.args[1:]]) if len(expr.args) > 1 else '1') + ' / ' + self.paren(sympy.simplify(x ** -1))
+        if len(expr.args) >= 2 and expr.args[0].is_Number:
+            num = expr.args[0]
+            x = expr.args[1]
+            if x.is_Pow and x.args[1].is_Number and x.args[1] < 0:
+                return (reduce(mul, [self.paren(arg) for arg in [num] + list(expr.args[2:])])) + ' / ' + self.paren(sympy.simplify(x ** -1))
+            else:
+                return reduce(mul, [self.paren(arg) for arg in expr.args])
         else:
-            return reduce(mul, [self.paren(arg) for arg in expr.args])
+            x = expr.args[0]
+            if x.is_Pow and x.args[1].is_Number and x.args[1] < 0:
+                return (reduce(mul, [self.paren(arg) for arg in expr.args[1:]]) if len(expr.args) > 1 else '1') + ' / ' + self.paren(sympy.simplify(x ** -1))
+            else:
+                return reduce(mul, [self.paren(arg) for arg in expr.args])
     
     # matrix form: mat(1, 2; 3, 4)
     def _print_MatrixBase(self, expr):
         n, m, mat_flattern = expr.args
         res = 'mat('
         rows = [mat_flattern[i:i+m] for i in range(0, n*m, m)]
         res += '; '.join(map(lambda row: ', '.join(map(self.doprint, row)), rows))
@@ -216,56 +224,59 @@
                 assert op in self.id2func, f'function for {op} not found'
                 return self.id2func[op](additive)
             else:
                 raise Exception(f'unknown additive operator {op}')
         else:
             return self.convert_mp(additive.mp())
 
-    def convert_mp(self, mp):
+    def convert_mp(self, mp, is_denominator=False):
         mp_op = mp.MP_OP()
         if mp_op:
             mps = mp.mp()
             assert len(mps) == 2
             op = mp_op.getText()
 
-            def mp_at(i):
-                return self.convert_mp(mps[i])
+            def mp_at(i, is_denominator=False):
+                return self.convert_mp(mps[i], is_denominator=is_denominator)
             if op == '*':
                 return mp_at(0) * mp_at(1)
             elif op == '/':
-                return mp_at(0) / mp_at(1)
+                return mp_at(0) / mp_at(1, True)
             elif op == '\\/':
-                return mp_at(0) / mp_at(1)
+                return mp_at(0) / mp_at(1, True)
             elif op in self.id2type and self.id2type[op] == 'MP_OP':
                 assert op in self.id2func, f'function for {op} not found'
                 return self.id2func[op](mp)
             else:
                 raise Exception(f'unknown mp operator {op}')
         else:
-            return self.convert_unary(mp.unary())
+            return self.convert_unary(mp.unary(), is_denominator=is_denominator)
 
-    def convert_unary(self, unary):
+    def convert_unary(self, unary, is_denominator=False):
         additive_op = unary.ADDITIVE_OP()
         if additive_op:
             unary = unary.unary()
             assert unary
             op = additive_op.getText()
             if op == '+':
-                return self.convert_unary(unary)
+                return self.convert_unary(unary, is_denominator=is_denominator)
             elif op == '-':
-                return -self.convert_unary(unary)
+                return -self.convert_unary(unary, is_denominator=is_denominator)
             else:
                 raise Exception(f'unsupport unary operator {op}')
         else:
             postfixes = [self.convert_postfix(pos) for pos in unary.postfix()]
             assert len(postfixes) >= 1
             if len(postfixes) == 1:
                 return postfixes[0]
             else:
-                return reduce(lambda x, y: x * y, postfixes)
+                if is_denominator:
+                    return  postfixes[0] / reduce(lambda x, y: x * y, postfixes[1:])
+                else:
+                    return reduce(lambda x, y: x * y, postfixes)
     
     def convert_eval_at(self, expr, eval_at):
         # eval_at: EVAL_BAR subsupassign;
         symbol, sub, sup = self.convert_subsupassign(eval_at.subsupassign())
         if symbol is None:
             symbol = expr.free_symbols.pop()
         assert sub or sup
```

## Comparing `typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.5.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.5.2.dist-info/METADATA` & `typst_sympy_calculator-0.5.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.5.2
+Version: 0.5.3
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `typst_sympy_calculator-0.5.2.dist-info/RECORD` & `typst_sympy_calculator-0.5.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DefaultTypstCalculator.py,sha256=2hvQfvtzwC13K_BSAjjCWB6G-wbWxW4-m1f6ms46dMA,8110
 TypstCalculator.py,sha256=CX9m-vm7nR-Enk57mQoK6BYGuIilkprGhibWnK42Oy4,7723
 TypstCalculatorServer.py,sha256=2QF971STzxJYSH04aGKM7OkkMt3Y3TgfwR1ddu8MnVs,11040
-TypstConverter.py,sha256=0t7M-irkUo4eHlv18adxABEhsR9CkvWrbhGH7TZ7XiM,25952
+TypstConverter.py,sha256=89TGsTKtySiyYehqq3x6qS_gLT3q5MnZBg8HwKK_B3o,26765
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=GVL1rcChdiQif2X-Fd7qnooKPUWtMCjInIOkJ8rzf7M,17703
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.5.2.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.5.2.dist-info/METADATA,sha256=C0YMCBpxnTmLZLlGBpjihJQkZRfO6iNcB0NKN-OTyhU,13675
-typst_sympy_calculator-0.5.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.5.2.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.5.2.dist-info/RECORD,,
+typst_sympy_calculator-0.5.3.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.5.3.dist-info/METADATA,sha256=gbT99RCNpPt60QFnGGG-zcE_2BZmC-iZnaUBFB9oUkI,13675
+typst_sympy_calculator-0.5.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.5.3.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.5.3.dist-info/RECORD,,
```

