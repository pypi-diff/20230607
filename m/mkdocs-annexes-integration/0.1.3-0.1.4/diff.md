# Comparing `tmp/mkdocs-annexes-integration-0.1.3.tar.gz` & `tmp/mkdocs-annexes-integration-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-annexes-integration-0.1.3.tar", last modified: Fri Mar 31 19:04:35 2023, max compression
+gzip compressed data, was "mkdocs-annexes-integration-0.1.4.tar", last modified: Wed Jun  7 12:12:56 2023, max compression
```

## Comparing `mkdocs-annexes-integration-0.1.3.tar` & `mkdocs-annexes-integration-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-10 07:58:44.062749 mkdocs-annexes-integration-0.1.3/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2023-05-09 09:20:19.000000 mkdocs-annexes-integration-0.1.3/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4620 2023-05-10 07:58:44.059748 mkdocs-annexes-integration-0.1.3/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1053 2023-05-10 07:55:00.000000 mkdocs-annexes-integration-0.1.3/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2023-04-28 08:21:37.000000 mkdocs-annexes-integration-0.1.3/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-10 07:58:43.930746 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8302 2023-05-10 07:57:05.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-10 07:58:44.042747 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4620 2023-05-10 07:58:43.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      441 2023-05-10 07:58:43.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2023-05-10 07:58:43.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2023-05-10 07:58:43.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2023-05-10 07:58:43.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2023-05-10 07:58:43.000000 mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3258 2023-05-09 09:31:00.000000 mkdocs-annexes-integration-0.1.3/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2023-05-10 07:58:44.063749 mkdocs-annexes-integration-0.1.3/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1201 2023-05-10 07:56:53.000000 mkdocs-annexes-integration-0.1.3/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-07 12:12:56.651112 mkdocs-annexes-integration-0.1.4/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-annexes-integration-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4948 2023-06-07 12:12:56.649112 mkdocs-annexes-integration-0.1.4/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1239 2023-05-17 10:31:00.000000 mkdocs-annexes-integration-0.1.4/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-annexes-integration-0.1.4/license
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-07 12:12:56.581717 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     9416 2023-05-17 10:35:24.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-07 12:12:56.638149 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4948 2023-06-07 12:12:56.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      441 2023-06-07 12:12:56.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-07 12:12:56.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       93 2023-06-07 12:12:56.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       32 2023-06-07 12:12:56.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       27 2023-06-07 12:12:56.000000 mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3477 2023-06-07 12:04:06.000000 mkdocs-annexes-integration-0.1.4/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-07 12:12:56.651112 mkdocs-annexes-integration-0.1.4/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1201 2023-05-17 10:29:33.000000 mkdocs-annexes-integration-0.1.4/setup.py
```

### Comparing `mkdocs-annexes-integration-0.1.3/PKG-INFO` & `mkdocs-annexes-integration-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-annexes-integration
         
@@ -54,22 +54,24 @@
                 - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
                 - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
                 - Title of the code file annex:
                     src: ../src/path/to/a/code/file1.py
                     dest: dest/path/to/a/code/file1.py
                 # others annexes...
               temp_dir: "folder_name" # Optional --> Default : temp_annexes
+              enabled_if_env: ENABLE_PDF_EXPORT # Optional
         ```
         
         As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
         
         Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
         
         - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
         - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
+        - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
         
         ## Usage
         
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
         
         This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
```

### Comparing `mkdocs-annexes-integration-0.1.3/changelog.md` & `mkdocs-annexes-integration-0.1.4/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.1.5] - 2023-05-17
+
+### Added
+
+- Support for enabling by environement variable
+
 ## [0.1.3] - 2023-05-10
 
 ### Added
 
 - Support for SQL (.sql) code files
 
 ## [0.1.2] - 2023-05-09
@@ -37,8 +43,9 @@
 
 ### Added
 
 - `plugin.py`
 - Support for PDF, CSharp (.cs), CSS (.css), Dart (.dart), HTML (.html), Javascript (.js), JSON (.json), PHP (.php) code files
 
 [0.1.2]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integrations/-/releases/v0.1.2
-[0.1.3]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integrations/-/releases/v0.1.3
+[0.1.3]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integrations/-/releases/v0.1.3
+[0.1.4]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integrations/-/releases/v0.1.4
```

### Comparing `mkdocs-annexes-integration-0.1.3/license` & `mkdocs-annexes-integration-0.1.4/license`

 * *Files identical despite different names*

### Comparing `mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration/plugin.py` & `mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,148 @@
 """
 File: mkdocs_annexes_integration/plugin.py
 Desc: This file contain the plugin used by mkdocs to integrate annexes as markdown file
 Author: Thibaud Briard - BRT, <thibaud.brrd@eduge.ch>
-Version: 0.1.3 - 2023-05-10
+Version: 0.1.4 - 2023-05-10
 """
 # Imports...
 import os, shutil # used to handle path, dicrectory and file creation, deletion and validation.
 import logging # used to log warning and errors for MkDocs among other things
 from pdf2image import convert_from_path # used to tranform pdf pages into images
 
 from mkdocs.config.base import Config as base_config # used to create an MkDocs config class derived from MkDocs config base
 from mkdocs.plugins import BasePlugin as base_plugin # used to create an MkDocs plugin class derived from MkDocs plugin base
 from mkdocs.config import config_options as c # used for config schema type safety
 from mkdocs.structure.files import File # used to create File in documentation
 
 # The plugin config options
 class AnnexesIntegrationConfig(base_config):
+    enabled_if_env = c.Type(str, default='')
+    enable = c.Type(bool, default=True)
     temp_dir = c.Type(str, default='temp_annexes')
     annexes = c.ListOfItems(c.Type(dict))
 
 # The plugin itself
 class AnnexesIntegration(base_plugin[AnnexesIntegrationConfig]):
 
     def __init__(self):
         self._logger = logging.getLogger('mkdocs.annexes-integration')
         self._logger.setLevel(logging.INFO)
 
-        self.enabled = True
+        self.enabled = False
         self.total_time = 0
     
     def on_config(self, config):
+        # Allow user to enable or disable using environment variable
+        if 'enabled_if_env' in self.config:
+            env_name = self.config['enabled_if_env']
+            if env_name:
+                self.enabled = os.environ.get(env_name) == '1'
+                if not self.enabled:
+                    self._logger.warning(
+                        'without annexes integration'
+                        f'(set environment variable {env_name} to 1 to enable)'
+                    )
+                    return
+            else:
+                self.enabled = True
+        else:
+            self.enabled = True
+
         # Create temp_dir in directory of mkdocs.yml
-        self.config.temp_dir = os.path.join(os.path.dirname(config.docs_dir), self.config.temp_dir)
-        if not os.path.exists(self.config.temp_dir):
-            os.mkdir(self.config.temp_dir)
+        if self.enabled:
+            self.config.temp_dir = os.path.join(os.path.dirname(config.docs_dir), self.config.temp_dir)
+            if not os.path.exists(self.config.temp_dir):
+                os.mkdir(self.config.temp_dir)
         return config
 
     def on_files(self, files, config):
-        # Generate markdown files for each annex
-        try:
-            for annex in self.config.annexes:
-                title, path = list(annex.items())[0]
-                self._logger.info(f'Integrating annex "{title}"')
-                # Determine source and destination path from path option
-                src, dest = self.get_src_and_dest(path)
-                # Get extension of file
-                extension = os.path.splitext(src)[1][1:]
-                # Get absolute path to original file
-                original = os.path.join(config.docs_dir, src)
-                # Get absolute path to generated markdown
-                embedded = f'{os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])}.md'
-                # skip if original file don't exist
-                if os.path.exists(original):
-                    # Check if file is code file or pdf
-                    if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php', 'py', 'sql']:
-                        # For code files content are put ina codeblock
-                        self._logger.info(f'    With content as code block')
-                        with open(original, 'r') as file:
-                            content = file.read()
-                        # Create a markdown file that take care of showing source code annex
-                        if not os.path.exists(os.path.dirname(embedded)):
-                            os.makedirs(os.path.dirname(embedded))
-                        with open(embedded, 'w') as f:
-                            # write the title and the content to the file
-                            f.write(f'# {title}\n\n``` {extension}\n{content}\n```\n')
-                    elif extension in ['pdf']:
-                        # For PDF files each page are transformed into images
-                        self._logger.info(f'    With each pages as images')
-                        # Get absolute path for PDF directory
-                        root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
-                        # Get absolute path for PDF images directory
-                        source = os.path.join(root, 'source')
-                        # Create a root folder containing the annex
-                        if not os.path.exists(root):
-                            os.makedirs(root)
-                        # Save pages as images in the pdf
-                        images = convert_from_path(original)
-                        # Create source folder to save images
-                        if not os.path.exists(source):
-                            os.mkdir(source)
-                        # Create a markdown file that take care of showing PDF annex
-                        with open(embedded, 'w') as f:
-                            # Write the title to the file
-                            f.write(f'# {title}\n\n')
-
-                            for i in range(len(images)):
-                                # Add leading zeros to the page number
-                                filename = f'page_{i + 1:04}.jpg'
-                                images[i].save(f'{source}/{filename}', 'JPEG')
-                                files.append(File(os.path.join(os.path.splitext(dest)[0], f'source/{filename}'), src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
-
-                                # Write the image link to the file
-                                f.write(f'![Page {i+1}](./{os.path.basename(os.path.splitext(dest)[0])}/source/{filename})\n')
+        if self.enabled:
+            # Generate markdown files for each annex
+            try:
+                for annex in self.config.annexes:
+                    title, path = list(annex.items())[0]
+                    self._logger.info(f'Integrating annex "{title}"')
+                    # Determine source and destination path from path option
+                    src, dest = self.get_src_and_dest(path)
+                    # Get extension of file
+                    extension = os.path.splitext(src)[1][1:]
+                    # Get absolute path to original file
+                    original = os.path.join(config.docs_dir, src)
+                    # Get absolute path to generated markdown
+                    embedded = f'{os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])}.md'
+                    # skip if original file don't exist
+                    if os.path.exists(original):
+                        # Check if file is code file or pdf
+                        if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php', 'py', 'sql']:
+                            # For code files content are put ina codeblock
+                            self._logger.info(f'    With content as code block')
+                            with open(original, 'r') as file:
+                                content = file.read()
+                            # Create a markdown file that take care of showing source code annex
+                            if not os.path.exists(os.path.dirname(embedded)):
+                                os.makedirs(os.path.dirname(embedded))
+                            with open(embedded, 'w') as f:
+                                # write the title and the content to the file
+                                f.write(f'# {title}\n\n``` {extension}\n{content}\n```\n')
+                        elif extension in ['pdf']:
+                            # For PDF files each page are transformed into images
+                            self._logger.info(f'    With each pages as images')
+                            # Get absolute path for PDF directory
+                            root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
+                            # Get absolute path for PDF images directory
+                            source = os.path.join(root, 'source')
+                            # Create a root folder containing the annex
+                            if not os.path.exists(root):
+                                os.makedirs(root)
+                            # Save pages as images in the pdf
+                            images = convert_from_path(original)
+                            # Create source folder to save images
+                            if not os.path.exists(source):
+                                os.mkdir(source)
+                            # Create a markdown file that take care of showing PDF annex
+                            with open(embedded, 'w') as f:
+                                # Write the title to the file
+                                f.write(f'# {title}\n\n')
+
+                                for i in range(len(images)):
+                                    # Add leading zeros to the page number
+                                    filename = f'page_{i + 1:04}.png'
+                                    images[i].save(f'{source}/{filename}', 'PNG')
+                                    files.append(File(os.path.join(os.path.splitext(dest)[0], f'source/{filename}'), src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
+
+                                    # Write the image link to the file
+                                    f.write(f'![Page {i+1}](./{os.path.basename(os.path.splitext(dest)[0])}/source/{filename})\n')
+                        else:
+                            self._logger.warning(f'file {src} extension isn\'t supported (yet) --> skipped')
+                        # Removing originals files from list of mkdocs files if they were in the docs directory originaly
+                        if os.path.isfile(os.path.join(config.docs_dir, dest)):
+                            self._logger.info(f'    Remvoing original annex {src} from processed files list')
+                            files.remove(files.get_file_from_path(src))
+                        # Adding embedded files in list of mkdocs files
+                        path = f'{os.path.splitext(dest)[0]}.md'
+                        self._logger.info(f'    Adding embedded annex {dest} to processed files list')
+                        files.append(File(path, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
                     else:
-                        self._logger.warning(f'file {src} extension isn\'t supported (yet) --> skipped')
-                    # Removing originals files from list of mkdocs files if they were in the docs directory originaly
-                    if os.path.isfile(os.path.join(config.docs_dir, dest)):
-                        self._logger.info(f'    Remvoing original annex {src} from processed files list')
-                        files.remove(files.get_file_from_path(src))
-                    # Adding embedded files in list of mkdocs files
-                    path = f'{os.path.splitext(dest)[0]}.md'
-                    self._logger.info(f'    Adding embedded annex {dest} to processed files list')
-                    files.append(File(path, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
-                else:
-                    self._logger.warning(f'{src} file doesn\'t exist at {original} --> skipped')
-        except Exception as e:
-            # Remove temp directory in case of any error before raising error
-            self._logger.error(f'error with the annexes-integration plugin : {e}')
-            if os.path.exists(self.config.temp_dir):
-                shutil.rmtree(self.config.temp_dir)
-            raise e
+                        self._logger.warning(f'{src} file doesn\'t exist at {original} --> skipped')
+            except Exception as e:
+                # Remove temp directory in case of any error before raising error
+                self._logger.error(f'error with the annexes-integration plugin : {e}')
+                if os.path.exists(self.config.temp_dir):
+                    shutil.rmtree(self.config.temp_dir)
+                raise e
         return files
     
     def on_post_build(self, config):
-        # Removing temp_dir directory
-        self._logger.info(f'Removin annexes temporary directory {self.config.temp_dir}')
-        if os.path.exists(self.config.temp_dir):
-            shutil.rmtree(self.config.temp_dir)
-        return
+        if self.enabled:
+            # Removing temp_dir directory
+            self._logger.info(f'Removin annexes temporary directory {self.config.temp_dir}')
+            if os.path.exists(self.config.temp_dir):
+                shutil.rmtree(self.config.temp_dir)
+            return
     
     def get_src_and_dest(self, path):
         # Get src and dest path from path
         if type(path) is dict:
             src = path['src']
             dest = src
             # Remove every ../ from dest if they exist
```

### Comparing `mkdocs-annexes-integration-0.1.3/mkdocs_annexes_integration.egg-info/PKG-INFO` & `mkdocs-annexes-integration-0.1.4/mkdocs_annexes_integration.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-annexes-integration
         
@@ -54,22 +54,24 @@
                 - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
                 - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
                 - Title of the code file annex:
                     src: ../src/path/to/a/code/file1.py
                     dest: dest/path/to/a/code/file1.py
                 # others annexes...
               temp_dir: "folder_name" # Optional --> Default : temp_annexes
+              enabled_if_env: ENABLE_PDF_EXPORT # Optional
         ```
         
         As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
         
         Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
         
         - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
         - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
+        - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
         
         ## Usage
         
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
         
         This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
```

### Comparing `mkdocs-annexes-integration-0.1.3/readme.md` & `mkdocs-annexes-integration-0.1.4/readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,96 @@
-# mkdocs-annexes-integration
-
-This is a plugin that transforms annex files into images to be integrated in Markdown pages for MkDocs.
-
-## Setup
-
-### Before installing
-
-Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
-
-#### Install on Linux :
-
-Note: *It depend on your Linux OS*
-
-``` sh
-sudo apt-get install poppler-utils
-```
-
-``` sh
-sudo yum install poppler-utils
-```
-
-#### Install on MacOS :
-
-``` sh
-brew install poppler
-```
-
-#### Install on Windows :
-
-On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
-
-### Installing using pip:
-
-`pip install mkdocs-annexes-integration`
-
-## Config
-
-You need to activate the plugin in `mkdocs.yml`:
-
-```yaml
-plugins:
-  - annexes-integration:
-      annexes: # Required (at least 1)
-        - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
-        - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
-        - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
-        - Title of the code file annex:
-            src: ../src/path/to/a/code/file1.py
-            dest: dest/path/to/a/code/file1.py
-        # others annexes...
-      temp_dir: "folder_name" # Optional --> Default : temp_annexes
-```
-
-As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
-
-Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
-
-- `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
-- `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
-
-## Usage
-
-Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
-
-This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
-
-## Support
-
-This plugin currently support two type of files :
-
-- **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
-
-- **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
-
-Currently supported code files are :
- - CSharp (.cs)
- - CSS (.css)
- - Dart (.dart)
- - HTML (.html)
- - Javascript (.js)
- - JSON (.json)
- - PHP (.php)
- - Python (.py)
-
-## License
-
-This project is under MIT license see: `license` file for more detail.
-
-## See Also
-
-- [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
-- [mkdocs website](http://www.mkdocs.org/)
+# mkdocs-annexes-integration
+
+This is a plugin that transforms annex files into images to be integrated in Markdown pages for MkDocs.
+
+## Setup
+
+### Before installing
+
+Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
+
+#### Install on Linux :
+
+Note: *It depend on your Linux OS*
+
+``` sh
+sudo apt-get install poppler-utils
+```
+
+``` sh
+sudo yum install poppler-utils
+```
+
+#### Install on MacOS :
+
+``` sh
+brew install poppler
+```
+
+#### Install on Windows :
+
+On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
+
+### Installing using pip:
+
+`pip install mkdocs-annexes-integration`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+```yaml
+plugins:
+  - annexes-integration:
+      annexes: # Required (at least 1)
+        - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
+        - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
+        - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
+        - Title of the code file annex:
+            src: ../src/path/to/a/code/file1.py
+            dest: dest/path/to/a/code/file1.py
+        # others annexes...
+      temp_dir: "folder_name" # Optional --> Default : temp_annexes
+      enabled_if_env: ENABLE_PDF_EXPORT # Optional
+```
+
+As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
+
+Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
+
+- `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
+- `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
+- `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+
+## Usage
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
+
+This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
+
+## Support
+
+This plugin currently support two type of files :
+
+- **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
+
+- **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
+
+Currently supported code files are :
+ - CSharp (.cs)
+ - CSS (.css)
+ - Dart (.dart)
+ - HTML (.html)
+ - Javascript (.js)
+ - JSON (.json)
+ - PHP (.php)
+ - Python (.py)
+
+## License
+
+This project is under MIT license see: `license` file for more detail.
+
+## See Also
+
+- [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
+- [mkdocs website](http://www.mkdocs.org/)
 - [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
```

### Comparing `mkdocs-annexes-integration-0.1.3/setup.py` & `mkdocs-annexes-integration-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-annexes-integration',
-    version='0.1.3',
+    version='0.1.4',
     description='A MkDocs plugin transforming annexes files into images to be integrated in markdown pages',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

