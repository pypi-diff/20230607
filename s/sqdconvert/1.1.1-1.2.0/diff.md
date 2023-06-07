# Comparing `tmp/sqdconvert-1.1.1.tar.gz` & `tmp/sqdconvert-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqdconvert-1.1.1.tar", last modified: Wed May 31 23:29:11 2023, max compression
+gzip compressed data, was "sqdconvert-1.2.0.tar", last modified: Wed Jun  7 09:05:34 2023, max compression
```

## Comparing `sqdconvert-1.1.1.tar` & `sqdconvert-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:11.328006 sqdconvert-1.1.1/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1740 2023-05-31 23:29:11.325824 sqdconvert-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.1.1/README.md
--rw-rw-rw-   0        0        0      601 2023-05-31 23:28:21.000000 sqdconvert-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 23:29:11.328006 sqdconvert-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:11.212113 sqdconvert-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:11.265822 sqdconvert-1.1.1/src/sqdconvert/
--rw-rw-rw-   0        0        0      388 2023-05-31 23:28:14.000000 sqdconvert-1.1.1/src/sqdconvert/__init__.py
--rw-rw-rw-   0        0        0     2637 2023-05-31 23:27:43.000000 sqdconvert-1.1.1/src/sqdconvert/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.1.1/src/sqdconvert/color.py
--rw-rw-rw-   0        0        0     2739 2023-05-31 23:23:10.000000 sqdconvert-1.1.1/src/sqdconvert/config.py
--rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.1.1/src/sqdconvert/errors.py
--rw-rw-rw-   0        0        0     2995 2023-05-31 23:08:08.000000 sqdconvert-1.1.1/src/sqdconvert/start.py
--rw-rw-rw-   0        0        0      291 2023-05-31 22:26:26.000000 sqdconvert-1.1.1/src/sqdconvert/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:29:11.320844 sqdconvert-1.1.1/src/sqdconvert.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-05-31 23:29:11.000000 sqdconvert-1.1.1/src/sqdconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-31 23:29:11.000000 sqdconvert-1.1.1/src/sqdconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:29:11.000000 sqdconvert-1.1.1/src/sqdconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-31 23:29:11.000000 sqdconvert-1.1.1/src/sqdconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 23:29:11.000000 sqdconvert-1.1.1/src/sqdconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 23:29:11.000000 sqdconvert-1.1.1/src/sqdconvert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 09:05:34.376250 sqdconvert-1.2.0/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-06-07 09:05:34.371712 sqdconvert-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.2.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-06-07 04:50:59.000000 sqdconvert-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 09:05:34.377268 sqdconvert-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:05:34.243121 sqdconvert-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 09:05:34.321304 sqdconvert-1.2.0/src/sqdconvert/
+-rw-rw-rw-   0        0        0      388 2023-06-07 04:25:28.000000 sqdconvert-1.2.0/src/sqdconvert/__init__.py
+-rw-rw-rw-   0        0        0     2637 2023-05-31 23:27:43.000000 sqdconvert-1.2.0/src/sqdconvert/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.2.0/src/sqdconvert/color.py
+-rw-rw-rw-   0        0        0     2749 2023-06-07 09:05:10.000000 sqdconvert-1.2.0/src/sqdconvert/config.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.2.0/src/sqdconvert/errors.py
+-rw-rw-rw-   0        0        0     3379 2023-06-07 07:39:41.000000 sqdconvert-1.2.0/src/sqdconvert/start.py
+-rw-rw-rw-   0        0        0      471 2023-06-07 07:37:30.000000 sqdconvert-1.2.0/src/sqdconvert/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:05:34.368721 sqdconvert-1.2.0/src/sqdconvert.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-06-07 09:05:34.000000 sqdconvert-1.2.0/src/sqdconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-07 09:05:34.000000 sqdconvert-1.2.0/src/sqdconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:05:34.000000 sqdconvert-1.2.0/src/sqdconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-07 09:05:34.000000 sqdconvert-1.2.0/src/sqdconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-06-07 09:05:34.000000 sqdconvert-1.2.0/src/sqdconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 09:05:34.000000 sqdconvert-1.2.0/src/sqdconvert.egg-info/top_level.txt
```

### Comparing `sqdconvert-1.1.1/LICENSE` & `sqdconvert-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.1.1/PKG-INFO` & `sqdconvert-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.1.1
+Version: 1.2.0
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `sqdconvert-1.1.1/pyproject.toml` & `sqdconvert-1.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqdconvert"
-version = "1.1.1"
+version = "1.2.0"
 description = "convert any audio or video files from one extension to another!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `sqdconvert-1.1.1/src/sqdconvert/__main__.py` & `sqdconvert-1.2.0/src/sqdconvert/__main__.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.1.1/src/sqdconvert/color.py` & `sqdconvert-1.2.0/src/sqdconvert/color.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.1.1/src/sqdconvert/config.py` & `sqdconvert-1.2.0/src/sqdconvert/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,20 @@
             
         except Exception as e:
             raise errors.ConfigLoadError(e)
 
 def make_default_config():
     t = datetime.now()
     return """{
-    "ffmpeg_path": "ffmpeg",
+    "ffmpeg_path": "path to ffmpeg",
     "update_notification": true
 }
-""", f"""// Default Config -- Generated on {t.day}/{t.month}/{t.year}"""
-"""{
-    "ffmpeg_path": "ffmpeg", // path to ffmpeg
+""", f"""// Default Config -- Generated on {t.day}/{t.month}/{t.year}
+""""""{
+    "ffmpeg_path": "./ffmpeg", // path to ffmpeg
     "update_notification": true // whether to turn on notification for updates or not
 }
 """
 
 def get_config(path: str = default_config_path):
     os.makedirs(path, exist_ok=True)
     config_path = os.path.join(path, "config.json")
```

### Comparing `sqdconvert-1.1.1/src/sqdconvert/errors.py` & `sqdconvert-1.2.0/src/sqdconvert/errors.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.1.1/src/sqdconvert/start.py` & `sqdconvert-1.2.0/src/sqdconvert/start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 import os
+import time
 import argparse
 
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
 from . import __name__ as name
 from . import color
-from .utils import fs
+from .utils import fs, convert
 from .config import Config
 
 __all__ = [
     "main"
 ]
 
 def main(args: argparse.ArgumentParser, config: Config) -> None:
-    if args.interactive:
-        args.input = input(f"{color.bright_blue}File to convert: {color.bright_white}").strip()
-        args.output = input(f"{color.bright_blue}Convert to: {color.bright_white}").strip()
-
-        if args.input.startswith('"') and args.input.endswith('"'):
-            args.input = args.input.lstrip('"').rstrip('"')
-        
-        if args.output.startswith('"') and args.output.endswith('"'):
-            args.output = args.output.lstrip('"').rstrip('"')
-    
-    if args.input is None or args.output is None:
-        print(f"{color.bright_red}💥 Provide atleast one argument! {color.bright_green}Maybe you want to try using '{color.bright_yellow}{name} -i{color.bright_green}'?{color.reset}")
-        return print(f"{color.bright_green}❓ Use '{color.bright_yellow}{name} -h{color.bright_green}' for a list of commands.{color.reset}")
-    
-    with yaspin(Spinners.dots12, text=f"{color.bright_white}Converting your file...{color.reset}", color="blue") as spinner:
-        inp = os.path.normpath(args.input)
-        if os.path.exists(inp):
-            if not os.path.isfile(inp):
-                spinner.text = f"{color.red}Input at the specified location is not a file: {color.bright_yellow}'{inp}'{color.reset}"
-                spinner.fail(f"💥")
+    try:
+        if args.interactive:
+            args.input = input(f"{color.bright_blue}File to convert: {color.bright_white}").strip()
+            args.output = input(f"{color.bright_blue}Convert to: {color.bright_white}").strip()
+
+            if args.input.startswith('"') and args.input.endswith('"'):
+                args.input = args.input.lstrip('"').rstrip('"')
+
+            if args.output.startswith('"') and args.output.endswith('"'):
+                args.output = args.output.lstrip('"').rstrip('"')
+
+        if args.input is None or args.output is None:
+            print(f"{color.bright_red}💥 Provide atleast one argument! {color.bright_green}Maybe you want to try using '{color.bright_yellow}{name} -i{color.bright_green}'?{color.reset}")
+            return print(f"{color.bright_green}❓ Use '{color.bright_yellow}{name} -h{color.bright_green}' for a list of commands.{color.reset}")
+
+        with yaspin(Spinners.dots12, text=f"{color.bright_white}Converting your file...{color.reset}", color="blue") as spinner:
+            inp = os.path.normpath(args.input)
+            if os.path.exists(inp):
+                if not os.path.isfile(inp):
+                    spinner.text = f"{color.red}Input at the specified location is not a file: {color.bright_yellow}'{inp}'{color.reset}"
+                    spinner.fail("💥")
+                    exit()
+            else:
+                spinner.text = f"{color.red}File not found: {color.bright_yellow}'{inp}'{color.reset}"
+                spinner.fail("💥")
+                exit()
+
+            out = os.path.normpath(args.output)
+            if os.path.exists(out):
+                spinner.text = f"{color.red}File already exists: {color.bright_yellow}'{out}'{color.reset}"
+                spinner.fail("💥")
                 exit()
-        else:
-            spinner.text = f"{color.red}File not found: {color.bright_yellow}'{inp}'{color.reset}"
-            spinner.fail(f"💥")
-            exit()
-
-        out = os.path.normpath(args.output)
-        if os.path.exists(out):
-            spinner.text = f"{color.red}File already exists: {color.bright_yellow}'{out}'{color.reset}"
-            spinner.fail(f"💥")
-            exit()
-
-        filename = out.split(fs)[-1]
-        if fs in out:
-            _out = out.split(fs)
-            _out.pop(-1)
-            out_path = fs.join(_out)
-        else:
-            out_path = "."
-
-        os.makedirs(out_path, exist_ok=True)    
-
-        status = os.system(f'{config.ffmpeg_path} -i "{inp}" "{out}" {"" if args.verbose else "-hide_banner -loglevel error"}')
-
-        if status == 0:
-            if out_path == ".":
-                saved_txt = f"Saved as {color.bright_yellow}{filename}{color.bright_green}"
+
+            filename = out.split(fs)[-1]
+            if fs in out:
+                _out = out.split(fs)
+                _out.pop(-1)
+                out_path = fs.join(_out)
+            else:
+                out_path = "."
+
+            os.makedirs(out_path, exist_ok=True)
+
+            t = time.time()
+            status = convert(ffmpeg=config.ffmpeg_path, input=inp, output=out, verbose=args.verbose)
+            end = round(time.time() - t, 2)
+
+            if status == 0:
+                if out_path == ".":
+                    saved_txt = f"Saved as {color.bright_yellow}{filename}{color.bright_green}"
+                else:
+                    saved_txt = f"Saved in {color.bright_yellow}{out_path}{color.bright_green} as {color.bright_yellow}{filename}{color.bright_green}"
+
+                spinner.text = f"{color.bright_green}File converted successfully. {saved_txt}. {color.bright_blue}Took {color.bright_yellow}{end}s{color.bright_blue}.{color.reset}"
+                spinner.ok("✅")
             else:
-                saved_txt = f"Saved in {color.bright_yellow}{out_path}{color.bright_green} as {color.bright_yellow}{filename}{color.bright_green}"
-            
-            spinner.text = f"{color.bright_green}File converted successfully. {saved_txt}.{color.reset}"
-            spinner.ok(f"✅")
-        else:
-            spinner.text = f"{color.red}Error occurred while converting {color.bright_yellow}{args.input}{color.reset}"
-            spinner.fail(f"💥")
+                spinner.text = f"{color.red}Error occurred while converting {color.bright_yellow}{args.input}{color.reset}"
+                spinner.fail("💥")
+    except KeyboardInterrupt:
+        print(f"\n{color.reset}{color.red}exiting...{color.reset}")
```

### Comparing `sqdconvert-1.1.1/src/sqdconvert.egg-info/PKG-INFO` & `sqdconvert-1.2.0/src/sqdconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.1.1
+Version: 1.2.0
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

