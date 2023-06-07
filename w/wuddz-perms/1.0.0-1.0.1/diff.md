# Comparing `tmp/wuddz_perms-1.0.0.tar.gz` & `tmp/wuddz_perms-1.0.1.tar.gz`

## Comparing `wuddz_perms-1.0.0.tar` & `wuddz_perms-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 wuddz_perms-1.0.0/wudz_perms.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 wuddz_perms-1.0.0/LICENSE
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 wuddz_perms-1.0.0/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 wuddz_perms-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 wuddz_perms-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 wuddz_perms-1.0.1/wudz_perms.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 wuddz_perms-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 wuddz_perms-1.0.1/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 wuddz_perms-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 wuddz_perms-1.0.1/PKG-INFO
```

### Comparing `wuddz_perms-1.0.0/wudz_perms.py` & `wuddz_perms-1.0.1/wudz_perms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import argparse, re, sys
+import argparse, re, sys, string
 from os import system
 from itertools import product, permutations
 system('')
 
 
 def all_uplow_perms(pw):
     for w in map(''.join, product(*zip(pw.upper(), pw.lower()))):
         yield str(w)
 
-def all_norep_perms(pw,pl):
-    for w in map(''.join, permutations(pw, int(pl))):
+def all_norep_perms(pw):
+    for w in map(''.join, permutations(pw, len(pw))):
         yield str(w)
 
 def all_perms(pw,pl):
     for w in map(''.join, product(pw, repeat=int(pl))):
         yield str(w)
 
 def all_mac_perms(pre,suf,ml):
@@ -32,37 +32,40 @@
         except:pass
 
 def main(args):
     md = ''
     with open(args.output, 'a', encoding='utf-8') as fw:
         mc = {'pre':args.prefix,'suf':args.suffix}
         try:
-            if args.all or args.norep and args.length is None:args.length = len(args.string)
-            if args.all:md = all_perms(args.string,args.length)
+            if args.all:
+                if args.length is None:args.length = len(args.string)
+                if args.string is None:args.string = (string.ascii_letters+string.digits+string.punctuation).strip()
+                if args.string and args.length:md = all_perms(args.string,args.length)
             elif args.mac:
                 ms, ml, mi = mac_setup(args.prefix,args.suffix)
                 mc[str(mi)] = ms
                 md = all_mac_perms(mc['pre'],mc['suf'],ml)
                 mc = {'pre':'','suf':''}
             elif args.uplow:md = all_uplow_perms(args.string)
-            elif args.norep:md = all_norep_perms(args.string,args.length)
+            elif args.norep:md = all_norep_perms(args.string)
         except:pass
         if md:
             c = 0
             print("\033[1;37;40m[*] Generating Combinations...\033[0m")
             while True:
                 try:
                     fw.write('{}{}{}\n'.format(mc['pre'],next(md),mc['suf']))
                     c += 1
                 except:break
             print("\033[1;32;40m[+] Saved {} Combinations To {}\033[0m".format(c,args.output))
         else:print("\033[1;31;40m[-] Error Occurred\033[0m")
 
 def cli_main():
-    parser = argparse.ArgumentParser(add_help = True, description ="Generate All/Non-Repeat Character Permutations/Combinations Of String Or Mac Addresses With Prefix/Suffix Partial Address.")
+    parser = argparse.ArgumentParser(add_help = True, 
+             description="Generate All/Non-Repeat Character Permutations/Combinations Of String Or Mac Addresses With Prefix/Suffix Partial Address.")
     parser.add_argument('-a', '--string', type=str, default=None, help='String To Generate All Permutations/Combinations.')
     parser.add_argument('-p', '--prefix', type=str, default='', help='String To Prefix Each Generated Permutation With.')
     parser.add_argument('-s', '--suffix', type=str, default='', help='String To Suffix Each Generated Permutation With.')
     parser.add_argument('-o', '--output', type=str, default='perms_output.txt', help='Output File To Save Generated Permutations To.')
     parser.add_argument('-l', '--length', type=int, default=None, help='Integer Length Of Characters To Be Generated.')
     parser.add_argument('-all', '--all', action='store_true', help='Generate All Combinations Of String.')
     parser.add_argument('-upl', '--uplow', action='store_true', help='Generate All Lower & Upper Case Permutations Of String.')
```

### Comparing `wuddz_perms-1.0.0/LICENSE` & `wuddz_perms-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wuddz_perms-1.0.0/README.md` & `wuddz_perms-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 ## Installation
 Install using [PyPI](https://pypi.org/project/wuddz-perms):
 ```
 $ pip install wuddz-perms
 ```
 Install locally by cloning or downloading and extracting the repo, then cd into 'dist' directory and execute:
 ```
-$ pip install wuddz_perms-1.0.0.tar.gz
+$ pip install wuddz_perms-1.0.1.tar.gz
 ```
 Then to run it, execute the following in the terminal:
 ```
 $ wudz-perms
 ```
 
 ### Usage
+Generate All Lower, Upper & Punctuation 4 Character Length Combinations To Default "output.txt" File.
+```
+$ wudz-perms -all -l 4
+```
 Generate All Combinations Of String To Default "output.txt" File.
 ```
 $ wudz-perms -all -a wuddzdevs
 ```
 Generate All Lower & Upper Case Permutations Of String To Default "output.txt" File.
 ```
 $ wudz-perms -upl -a pythondev
```

### Comparing `wuddz_perms-1.0.0/pyproject.toml` & `wuddz_perms-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wuddz-perms"
-version = "1.0.0"
+version = "1.0.1"
 description = "Generate All/Non-Repeat Character Permutations/Combinations Of String Or Mac Addresses With Prefix/Suffix Partial Address"
 readme = "README.md"
 authors = [
   { name="Wuddz-Devs", email="wuddz_devs@protonmail.com" },
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `wuddz_perms-1.0.0/PKG-INFO` & `wuddz_perms-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wuddz-perms
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate All/Non-Repeat Character Permutations/Combinations Of String Or Mac Addresses With Prefix/Suffix Partial Address
 Project-URL: Homepage, https://github.com/wuddz-devs/wuddz-perms
 Author-email: Wuddz-Devs <wuddz_devs@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wuddz-Devs
         
@@ -49,22 +49,26 @@
 ## Installation
 Install using [PyPI](https://pypi.org/project/wuddz-perms):
 ```
 $ pip install wuddz-perms
 ```
 Install locally by cloning or downloading and extracting the repo, then cd into 'dist' directory and execute:
 ```
-$ pip install wuddz_perms-1.0.0.tar.gz
+$ pip install wuddz_perms-1.0.1.tar.gz
 ```
 Then to run it, execute the following in the terminal:
 ```
 $ wudz-perms
 ```
 
 ### Usage
+Generate All Lower, Upper & Punctuation 4 Character Length Combinations To Default "output.txt" File.
+```
+$ wudz-perms -all -l 4
+```
 Generate All Combinations Of String To Default "output.txt" File.
 ```
 $ wudz-perms -all -a wuddzdevs
 ```
 Generate All Lower & Upper Case Permutations Of String To Default "output.txt" File.
 ```
 $ wudz-perms -upl -a pythondev
```

