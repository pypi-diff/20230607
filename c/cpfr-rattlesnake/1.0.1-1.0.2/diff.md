# Comparing `tmp/cpfr-rattlesnake-1.0.1.tar.gz` & `tmp/cpfr-rattlesnake-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpfr-rattlesnake-1.0.1.tar", last modified: Tue Feb  7 21:59:00 2023, max compression
+gzip compressed data, was "cpfr-rattlesnake-1.0.2.tar", last modified: Wed Jun  7 21:39:08 2023, max compression
```

## Comparing `cpfr-rattlesnake-1.0.1.tar` & `cpfr-rattlesnake-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-02-07 21:59:00.114005 cpfr-rattlesnake-1.0.1/
--rw-rw-r--   0 carsten   (1000) carsten   (1000)      854 2023-02-02 19:41:19.000000 cpfr-rattlesnake-1.0.1/LICENSE
--rw-rw-r--   0 carsten   (1000) carsten   (1000)     3287 2023-02-07 21:59:00.114005 cpfr-rattlesnake-1.0.1/PKG-INFO
-drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-02-07 21:59:00.114005 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/
--rw-rw-r--   0 carsten   (1000) carsten   (1000)     3287 2023-02-07 21:59:00.000000 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/PKG-INFO
--rw-rw-r--   0 carsten   (1000) carsten   (1000)      298 2023-02-07 21:59:00.000000 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/SOURCES.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)        1 2023-02-07 21:59:00.000000 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/dependency_links.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       48 2023-02-07 21:59:00.000000 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/entry_points.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       84 2023-02-07 21:59:00.000000 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/requires.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       12 2023-02-07 21:59:00.000000 cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/top_level.txt
--rw-rw-r--   0 carsten   (1000) carsten   (1000)      738 2023-02-07 21:56:39.000000 cpfr-rattlesnake-1.0.1/pyproject.toml
-drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-02-07 21:59:00.114005 cpfr-rattlesnake-1.0.1/rattlesnake/
--rw-rw-r--   0 carsten   (1000) carsten   (1000)    14727 2023-02-07 21:55:21.000000 cpfr-rattlesnake-1.0.1/rattlesnake/__init__.py
--rw-rw-r--   0 carsten   (1000) carsten   (1000)     2923 2023-02-02 20:41:17.000000 cpfr-rattlesnake-1.0.1/readme.md
--rw-rw-r--   0 carsten   (1000) carsten   (1000)       38 2023-02-07 21:59:00.114005 cpfr-rattlesnake-1.0.1/setup.cfg
+drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)      854 2023-02-02 19:41:19.000000 cpfr-rattlesnake-1.0.2/LICENSE
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)     3531 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/PKG-INFO
+drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)     3531 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/PKG-INFO
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)      298 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/SOURCES.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)        1 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/dependency_links.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       48 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/entry_points.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       84 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/requires.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       12 2023-06-07 21:39:08.000000 cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/top_level.txt
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)      738 2023-06-07 21:38:43.000000 cpfr-rattlesnake-1.0.2/pyproject.toml
+drwxrwxr-x   0 carsten   (1000) carsten   (1000)        0 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/rattlesnake/
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)    15400 2023-06-07 20:32:12.000000 cpfr-rattlesnake-1.0.2/rattlesnake/__init__.py
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)     3166 2023-06-07 21:38:53.000000 cpfr-rattlesnake-1.0.2/readme.md
+-rw-rw-r--   0 carsten   (1000) carsten   (1000)       38 2023-06-07 21:39:08.850902 cpfr-rattlesnake-1.0.2/setup.cfg
```

### Comparing `cpfr-rattlesnake-1.0.1/LICENSE` & `cpfr-rattlesnake-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpfr-rattlesnake-1.0.1/PKG-INFO` & `cpfr-rattlesnake-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpfr-rattlesnake
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple static-site generator for Python3, using markdown and the Jinja2 templating engine
 Author-email: Carsten Pfeffer <pfeffer.carsten@gmail.com>
 Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -44,7 +44,14 @@
 
 - By default, `./src` is used as the input directory. This can be changed by specifying a different path as the first argument.
 - By default, `./build` is used as the output directory. This can be changed by specifying a different path using the `--output-dir` option.
 - By default, `./config.yml` is used as the config file for parameters and template variables. This can be changed by specifying a different file path using the `--config-file` option.
 - The `--watch` option keeps the script running after the build process and watches the source directory for file changes. Further, it starts an HTTP server that serves the built website.
 - The `--port` option allows the user to specify a port if the --watch flag is given. If no custom port is provided, port `8000` is used.
 - The `--additional-config` option can be used in order to load an additional config yaml file that supplement or overrides the default values. This can be useful for different deployment targets.
+
+# Version History
+
+- 1.0.2: Bugfixes
+  - directories starting with an underscore are also skipped (not just files)
+  - adding date formatting filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`)
+- 1.0.0: Initial Implementation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.1 Summary: A simple
+Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.2 Summary: A simple
 static-site generator for Python3, using markdown and the Jinja2 templating
 engine Author-email: Carsten Pfeffer
 carsten@gmail.com> Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Rattlesnake Static Site Generator Rattlesnake is a static website
 generator. It is written in the Python programming language and utilizes the
 Jinja templating engine, pySCSS for SCSS support, as well as the pyYaml library
@@ -36,8 +36,11 @@
 using the `--config-file` option. - The `--watch` option keeps the script
 running after the build process and watches the source directory for file
 changes. Further, it starts an HTTP server that serves the built website. - The
 `--port` option allows the user to specify a port if the --watch flag is given.
 If no custom port is provided, port `8000` is used. - The `--additional-config`
 option can be used in order to load an additional config yaml file that
 supplement or overrides the default values. This can be useful for different
-deployment targets.
+deployment targets. # Version History - 1.0.2: Bugfixes - directories starting
+with an underscore are also skipped (not just files) - adding date formatting
+filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0:
+Initial Implementation
```

### Comparing `cpfr-rattlesnake-1.0.1/cpfr_rattlesnake.egg-info/PKG-INFO` & `cpfr-rattlesnake-1.0.2/cpfr_rattlesnake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpfr-rattlesnake
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple static-site generator for Python3, using markdown and the Jinja2 templating engine
 Author-email: Carsten Pfeffer <pfeffer.carsten@gmail.com>
 Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -44,7 +44,14 @@
 
 - By default, `./src` is used as the input directory. This can be changed by specifying a different path as the first argument.
 - By default, `./build` is used as the output directory. This can be changed by specifying a different path using the `--output-dir` option.
 - By default, `./config.yml` is used as the config file for parameters and template variables. This can be changed by specifying a different file path using the `--config-file` option.
 - The `--watch` option keeps the script running after the build process and watches the source directory for file changes. Further, it starts an HTTP server that serves the built website.
 - The `--port` option allows the user to specify a port if the --watch flag is given. If no custom port is provided, port `8000` is used.
 - The `--additional-config` option can be used in order to load an additional config yaml file that supplement or overrides the default values. This can be useful for different deployment targets.
+
+# Version History
+
+- 1.0.2: Bugfixes
+  - directories starting with an underscore are also skipped (not just files)
+  - adding date formatting filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`)
+- 1.0.0: Initial Implementation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.1 Summary: A simple
+Metadata-Version: 2.1 Name: cpfr-rattlesnake Version: 1.0.2 Summary: A simple
 static-site generator for Python3, using markdown and the Jinja2 templating
 engine Author-email: Carsten Pfeffer
 carsten@gmail.com> Keywords: static site generator,website,gitlab pages,jinja
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Rattlesnake Static Site Generator Rattlesnake is a static website
 generator. It is written in the Python programming language and utilizes the
 Jinja templating engine, pySCSS for SCSS support, as well as the pyYaml library
@@ -36,8 +36,11 @@
 using the `--config-file` option. - The `--watch` option keeps the script
 running after the build process and watches the source directory for file
 changes. Further, it starts an HTTP server that serves the built website. - The
 `--port` option allows the user to specify a port if the --watch flag is given.
 If no custom port is provided, port `8000` is used. - The `--additional-config`
 option can be used in order to load an additional config yaml file that
 supplement or overrides the default values. This can be useful for different
-deployment targets.
+deployment targets. # Version History - 1.0.2: Bugfixes - directories starting
+with an underscore are also skipped (not just files) - adding date formatting
+filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0:
+Initial Implementation
```

### Comparing `cpfr-rattlesnake-1.0.1/pyproject.toml` & `cpfr-rattlesnake-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [project]
 name = "cpfr-rattlesnake"
 authors = [
     { name = "Carsten Pfeffer", email = "pfeffer.carsten@gmail.com" }
 ]
 description = "A simple static-site generator for Python3, using markdown and the Jinja2 templating engine"
-version = "1.0.1"
+version = "1.0.2"
 readme = "readme.md"
 requires-python = ">= 3.7"
 keywords = ["static site generator", "website", "gitlab pages", "jinja"]
 dependencies = [
     "watchdog",
     "jinja2",
     "pyyaml",
```

### Comparing `cpfr-rattlesnake-1.0.1/rattlesnake/__init__.py` & `cpfr-rattlesnake-1.0.2/rattlesnake/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,26 @@
 import datetime
 from dateutil.parser import parse as parse_date
 from email.utils import formatdate
 import xml.sax.saxutils
 import re
 
 content_block_regex = re.compile("{% block content %}(.*?){% endblock %}", re.MULTILINE | re.DOTALL | re.IGNORECASE)
+underscore_dir_regex = re.compile("(.*?)/_(.*?)", re.DOTALL | re.IGNORECASE)
 
 def date_to_rfc822(date):
     if not isinstance(date, datetime.datetime) and not isinstance(date, datetime.date):
         date = parse_date(date)
     return formatdate(float(date.strftime("%s")))
 
+def format_date(date, format="%Y-%m-%d"):
+    if not isinstance(date, datetime.datetime) and not isinstance(date, datetime.date):
+        date = parse_date(date)
+    return date.strftime(format)
+
 # available colors: blue, red, green, yellow, blue, magenta, cyan, white
 
 class DictObject:
     def __init__(self, **entries):
         self.__dict__.update(entries)
     
     def __repr__(self):
@@ -67,27 +73,29 @@
     env = jj.Environment(
         loader = TemplateLoader(path, dependencies, file_path),
         autoescape = jj.select_autoescape()
     )
 
     env.filters["xml_escape"] = xml.sax.saxutils.escape
     env.filters["date_to_rfc822"] = date_to_rfc822
+    env.filters["format_date"] = format_date
 
     template = env.get_template(file_path)
     rendered = template.render(**config)
     return rendered
 
 def render_template_from_string(text_content, path, config, file_path, dependencies):
     env = jj.Environment(
         loader = TemplateLoader(path, dependencies, file_path),
         autoescape = jj.select_autoescape()
     )
 
     env.filters["xml_escape"] = xml.sax.saxutils.escape
     env.filters["date_to_rfc822"] = date_to_rfc822
+    env.filters["format_date"] = format_date
 
     template = env.from_string(text_content)
     rendered = template.render(**config)
     return rendered
 
 
 def get_target_path(file_path, source_dir, target_dir):
@@ -225,28 +233,38 @@
             
             if process_dependencies:
                 # check if any of the files has a dependency to the current one
                 dependent_files = [key for key, value in dependencies.items() if rel_path in value]
                 for dependent_file in dependent_files:
                     process_file(source_path, target_path, os.path.join(source_path, dependent_file), config, process_dependencies)
 
+    
+    def is_underscore_directory(dir_path):
+        return dir_path.startswith("_") or underscore_dir_regex.match(dir_path) is not None
 
     # process files
     pages = []
     config["_pages"] = pages
     config["_generation_time"] = datetime.datetime.now()
 
     for dir_path, sub_dirs, file_paths in os.walk(args.source_dir):
+        if is_underscore_directory(dir_path):
+            continue
+        print("DIR: " + dir_path)
+
         for file_path in file_paths:
             full_path = os.path.join(dir_path, file_path)
             page_metadata = collect_file_meta_information(args.source_dir, full_path)
             if page_metadata is not None:
                 pages.append(DictObject(**page_metadata))
 
     for dir_path, sub_dirs, file_paths in os.walk(args.source_dir):
+        if is_underscore_directory(dir_path):
+            continue
+
         for file_path in file_paths:
             full_path = os.path.join(dir_path, file_path)
             process_file(args.source_dir, args.output_dir, full_path, config, False)
 
     def delete_empty_dirs(target_dir_path):
         while len(os.listdir(target_dir_path)) == 0:
             print(colored("deleting empty directory " + target_dir_path, "blue"))
```

### Comparing `cpfr-rattlesnake-1.0.1/readme.md` & `cpfr-rattlesnake-1.0.2/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,7 +34,14 @@
 
 - By default, `./src` is used as the input directory. This can be changed by specifying a different path as the first argument.
 - By default, `./build` is used as the output directory. This can be changed by specifying a different path using the `--output-dir` option.
 - By default, `./config.yml` is used as the config file for parameters and template variables. This can be changed by specifying a different file path using the `--config-file` option.
 - The `--watch` option keeps the script running after the build process and watches the source directory for file changes. Further, it starts an HTTP server that serves the built website.
 - The `--port` option allows the user to specify a port if the --watch flag is given. If no custom port is provided, port `8000` is used.
 - The `--additional-config` option can be used in order to load an additional config yaml file that supplement or overrides the default values. This can be useful for different deployment targets.
+
+# Version History
+
+- 1.0.2: Bugfixes
+  - directories starting with an underscore are also skipped (not just files)
+  - adding date formatting filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`)
+- 1.0.0: Initial Implementation
```

#### html2text {}

```diff
@@ -31,8 +31,11 @@
 using the `--config-file` option. - The `--watch` option keeps the script
 running after the build process and watches the source directory for file
 changes. Further, it starts an HTTP server that serves the built website. - The
 `--port` option allows the user to specify a port if the --watch flag is given.
 If no custom port is provided, port `8000` is used. - The `--additional-config`
 option can be used in order to load an additional config yaml file that
 supplement or overrides the default values. This can be useful for different
-deployment targets.
+deployment targets. # Version History - 1.0.2: Bugfixes - directories starting
+with an underscore are also skipped (not just files) - adding date formatting
+filter to Jinja parser (`{{ some_date | format_date("%d.%m.%Y") }}`) - 1.0.0:
+Initial Implementation
```

