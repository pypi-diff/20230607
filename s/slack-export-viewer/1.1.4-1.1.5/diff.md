# Comparing `tmp/slack-export-viewer-1.1.4.tar.gz` & `tmp/slack-export-viewer-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-export-viewer-1.1.4.tar", last modified: Sat Jul 23 03:40:17 2022, max compression
+gzip compressed data, was "slack-export-viewer-1.1.5.tar", last modified: Wed Jun  7 16:24:47 2023, max compression
```

## Comparing `slack-export-viewer-1.1.4.tar` & `slack-export-viewer-1.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-07-23 03:40:17.264637 slack-export-viewer-1.1.4/
--rw-rw-rw-   0        0        0     1078 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      185 2019-07-25 04:31:09.000000 slack-export-viewer-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      860 2022-07-23 03:40:17.263637 slack-export-viewer-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4448 2021-02-24 12:04:00.000000 slack-export-viewer-1.1.4/README.md
--rw-rw-rw-   0        0        0       44 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.4/requirements.txt
--rw-rw-rw-   0        0        0   158989 2018-03-18 08:48:39.000000 slack-export-viewer-1.1.4/screenshot.png
--rw-rw-rw-   0        0        0       42 2022-07-23 03:40:17.264637 slack-export-viewer-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1688 2022-04-23 22:53:24.000000 slack-export-viewer-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-23 03:40:17.180848 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/
--rw-rw-rw-   0        0        0      860 2022-07-23 03:40:17.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2022-07-23 03:40:17.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-23 03:40:17.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2022-07-23 03:40:17.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2019-07-25 04:12:23.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       40 2022-07-23 03:40:17.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-07-23 03:40:17.000000 slack-export-viewer-1.1.4/slack_export_viewer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-23 03:40:17.222856 slack-export-viewer-1.1.4/slackviewer/
--rw-rw-rw-   0        0        0       23 2022-07-23 03:38:33.000000 slack-export-viewer-1.1.4/slackviewer/__init__.py
--rw-rw-rw-   0        0        0     4147 2020-01-16 06:43:37.000000 slack-export-viewer-1.1.4/slackviewer/app.py
--rw-rw-rw-   0        0        0     3935 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/archive.py
--rw-rw-rw-   0        0        0     1923 2019-07-25 04:09:03.000000 slack-export-viewer-1.1.4/slackviewer/cli.py
--rw-rw-rw-   0        0        0      103 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/constants.py
--rw-rw-rw-   0        0        0     5682 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.4/slackviewer/formatter.py
--rw-rw-rw-   0        0        0     2853 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/main.py
--rw-rw-rw-   0        0        0     6611 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.4/slackviewer/message.py
--rw-rw-rw-   0        0        0    10508 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.4/slackviewer/reader.py
-drwxrwxrwx   0        0        0        0 2022-07-23 03:40:17.229629 slack-export-viewer-1.1.4/slackviewer/static/
--rw-rw-rw-   0        0        0     3289 2020-01-14 09:02:36.000000 slack-export-viewer-1.1.4/slackviewer/static/viewer.css
-drwxrwxrwx   0        0        0        0 2022-07-23 03:40:17.251634 slack-export-viewer-1.1.4/slackviewer/templates/
--rw-rw-rw-   0        0        0      990 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/templates/export_single.html
--rw-rw-rw-   0        0        0     4836 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/templates/util.html
--rw-rw-rw-   0        0        0     4178 2020-02-08 06:58:48.000000 slack-export-viewer-1.1.4/slackviewer/templates/viewer.html
--rw-rw-rw-   0        0        0     2261 2021-02-24 11:31:32.000000 slack-export-viewer-1.1.4/slackviewer/user.py
-drwxrwxrwx   0        0        0        0 2022-07-23 03:40:17.262637 slack-export-viewer-1.1.4/slackviewer/utils/
--rw-rw-rw-   0        0        0        0 2018-03-21 07:05:31.000000 slack-export-viewer-1.1.4/slackviewer/utils/__init__.py
--rw-rw-rw-   0        0        0      376 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/utils/click.py
--rw-rw-rw-   0        0        0      538 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.4/slackviewer/utils/six.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:24:47.866618 slack-export-viewer-1.1.5/
+-rw-rw-rw-   0        0        0     1078 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      185 2019-07-25 04:31:09.000000 slack-export-viewer-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      839 2023-06-07 16:24:47.866618 slack-export-viewer-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4448 2021-02-24 12:04:00.000000 slack-export-viewer-1.1.5/README.md
+-rw-rw-rw-   0        0        0       44 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.5/requirements.txt
+-rw-rw-rw-   0        0        0   158989 2018-03-18 08:48:39.000000 slack-export-viewer-1.1.5/screenshot.png
+-rw-rw-rw-   0        0        0       42 2023-06-07 16:24:47.866618 slack-export-viewer-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1688 2022-04-23 22:53:24.000000 slack-export-viewer-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:24:47.773618 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/
+-rw-rw-rw-   0        0        0      839 2023-06-07 16:24:47.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-06-07 16:24:47.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:24:47.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-07 16:24:47.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2019-07-25 04:12:23.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       40 2023-06-07 16:24:47.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 16:24:47.000000 slack-export-viewer-1.1.5/slack_export_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 16:24:47.824618 slack-export-viewer-1.1.5/slackviewer/
+-rw-rw-rw-   0        0        0       23 2023-06-07 16:20:56.000000 slack-export-viewer-1.1.5/slackviewer/__init__.py
+-rw-rw-rw-   0        0        0     4159 2023-06-07 16:17:52.000000 slack-export-viewer-1.1.5/slackviewer/app.py
+-rw-rw-rw-   0        0        0     4269 2023-06-07 16:17:52.000000 slack-export-viewer-1.1.5/slackviewer/archive.py
+-rw-rw-rw-   0        0        0     1923 2019-07-25 04:09:03.000000 slack-export-viewer-1.1.5/slackviewer/cli.py
+-rw-rw-rw-   0        0        0      103 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/slackviewer/constants.py
+-rw-rw-rw-   0        0        0     5682 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.5/slackviewer/formatter.py
+-rw-rw-rw-   0        0        0     2853 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/slackviewer/main.py
+-rw-rw-rw-   0        0        0     6611 2022-07-23 03:38:11.000000 slack-export-viewer-1.1.5/slackviewer/message.py
+-rw-rw-rw-   0        0        0    10516 2023-06-07 16:17:52.000000 slack-export-viewer-1.1.5/slackviewer/reader.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:24:47.825616 slack-export-viewer-1.1.5/slackviewer/static/
+-rw-rw-rw-   0        0        0     3545 2023-06-07 16:17:52.000000 slack-export-viewer-1.1.5/slackviewer/static/viewer.css
+drwxrwxrwx   0        0        0        0 2023-06-07 16:24:47.851616 slack-export-viewer-1.1.5/slackviewer/templates/
+-rw-rw-rw-   0        0        0      990 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/slackviewer/templates/export_single.html
+-rw-rw-rw-   0        0        0     4836 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/slackviewer/templates/util.html
+-rw-rw-rw-   0        0        0     4178 2020-02-08 06:58:48.000000 slack-export-viewer-1.1.5/slackviewer/templates/viewer.html
+-rw-rw-rw-   0        0        0     2261 2021-02-24 11:31:32.000000 slack-export-viewer-1.1.5/slackviewer/user.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:24:47.864620 slack-export-viewer-1.1.5/slackviewer/utils/
+-rw-rw-rw-   0        0        0        0 2018-03-21 07:05:31.000000 slack-export-viewer-1.1.5/slackviewer/utils/__init__.py
+-rw-rw-rw-   0        0        0      376 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/slackviewer/utils/click.py
+-rw-rw-rw-   0        0        0      538 2019-07-25 04:05:21.000000 slack-export-viewer-1.1.5/slackviewer/utils/six.py
```

### Comparing `slack-export-viewer-1.1.4/LICENSE` & `slack-export-viewer-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/PKG-INFO` & `slack-export-viewer-1.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: slack-export-viewer
-Version: 1.1.4
+Version: 1.1.5
 Summary: Slack Export Archive Viewer
 Home-page: https://github.com/hfaran/slack-export-viewer
 Author: Hamza Faran
 Author-email: hamzafaran@outlook.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 See README at https://github.com/hfaran/slack-export-viewer
-
```

### Comparing `slack-export-viewer-1.1.4/README.md` & `slack-export-viewer-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/screenshot.png` & `slack-export-viewer-1.1.5/screenshot.png`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/setup.py` & `slack-export-viewer-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slack_export_viewer.egg-info/PKG-INFO` & `slack-export-viewer-1.1.5/slack_export_viewer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: slack-export-viewer
-Version: 1.1.4
+Version: 1.1.5
 Summary: Slack Export Archive Viewer
 Home-page: https://github.com/hfaran/slack-export-viewer
 Author: Hamza Faran
 Author-email: hamzafaran@outlook.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 See README at https://github.com/hfaran/slack-export-viewer
-
```

### Comparing `slack-export-viewer-1.1.4/slack_export_viewer.egg-info/SOURCES.txt` & `slack-export-viewer-1.1.5/slack_export_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/app.py` & `slack-export-viewer-1.1.5/slackviewer/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                                  mpim_users=mpim_users,
                                  no_sidebar=app.no_sidebar,
                                  no_external_references=app.no_external_references)
 
 
 @app.route("/mpim/<name>/")
 def mpim_name(name):
-    messages = flask._app_ctx_stack.mpims[name]
+    messages = flask._app_ctx_stack.mpims.get(name, list())
     channels = list(flask._app_ctx_stack.channels.keys())
     groups = list(flask._app_ctx_stack.groups.keys())
     dm_users = list(flask._app_ctx_stack.dm_users)
     mpim_users = list(flask._app_ctx_stack.mpim_users)
 
     return flask.render_template("viewer.html", messages=messages,
                                  name=name.format(name=name),
```

### Comparing `slack-export-viewer-1.1.4/slackviewer/archive.py` & `slack-export-viewer-1.1.5/slackviewer/archive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,130 +1,135 @@
-import hashlib
-import json
-import os
-import zipfile
-import io
-
-from os.path import basename, splitext
-
-import slackviewer
-from slackviewer.constants import SLACKVIEWER_TEMP_PATH
-from slackviewer.utils.six import to_unicode, to_bytes
-
-
-def SHA1_file(filepath, extra=b''):
-    """
-    Returns hex digest of SHA1 hash of file at filepath
-
-    :param str filepath: File to hash
-
-    :param bytes extra: Extra content added to raw read of file before taking hash
-
-    :return: hex digest of hash
-
-    :rtype: str
-    """
-    h = hashlib.sha1()
-    with io.open(filepath, 'rb') as f:
-        for chunk in iter(lambda: f.read(h.block_size), b''):
-            h.update(chunk)
-    h.update(extra)
-    return h.hexdigest()
-
-
-def extract_archive(filepath):
-    """
-    Returns the path of the archive
-
-    :param str filepath: Path to file to extract or read
-
-    :return: path of the archive
-
-    :rtype: str
-    """
-
-    # Checks if file path is a directory
-    if os.path.isdir(filepath):
-        path = os.path.abspath(filepath)
-        print("Archive already extracted. Viewing from {}...".format(path))
-        return path
-
-    # Checks if the filepath is a zipfile and continues to extract if it is
-    # if not it raises an error
-    elif not zipfile.is_zipfile(filepath):
-        # Misuse of TypeError? :P
-        raise TypeError("{} is not a zipfile".format(filepath))
-
-    archive_sha = SHA1_file(
-        filepath=filepath,
-        # Add version of slackviewer to hash as well so we can invalidate the cached copy
-        #  if there are new features added
-        extra=to_bytes(slackviewer.__version__)
-    )
-
-    extracted_path = os.path.join(SLACKVIEWER_TEMP_PATH, archive_sha)
-
-    if os.path.exists(extracted_path):
-        print("{} already exists".format(extracted_path))
-    else:
-        # Extract zip
-        with zipfile.ZipFile(filepath) as zip:
-            print("{} extracting to {}...".format(filepath, extracted_path))
-            zip.extractall(path=extracted_path)
-
-        print("{} extracted to {}".format(filepath, extracted_path))
-
-        # Add additional file with archive info
-        create_archive_info(filepath, extracted_path, archive_sha)
-
-    return extracted_path
-
-
-# Saves archive info
-# When loading empty dms and there is no info file then this is called to
-# create a new archive file
-def create_archive_info(filepath, extracted_path, archive_sha=None):
-    """
-    Saves archive info to a json file
-
-    :param str filepath: Path to directory of archive
-
-    :param str extracted_path: Path to directory of archive
-
-    :param str archive_sha: SHA string created when archive was extracted from zip
-    """
-
-    archive_info = {
-        "sha1": archive_sha,
-        "filename": os.path.split(filepath)[1],
-    }
-
-    with io.open(
-        os.path.join(
-            extracted_path,
-            ".slackviewer_archive_info.json",
-        ), 'w+', encoding="utf-8"
-    ) as f:
-        s = json.dumps(archive_info, ensure_ascii=False)
-        s = to_unicode(s)
-        f.write(s)
-
-
-def get_export_info(archive_name):
-    """
-    Given a file or directory, extract it and return information that will be used in
-    an export printout: the basename of the file, the name stripped of its extension, and
-    our best guess (based on Slack's current naming convention) of the name of the
-    workspace that this is an export of.
-    """
-    extracted_path = extract_archive(archive_name)
-    base_filename = basename(archive_name)
-    (noext_filename, _) = splitext(base_filename)
-    # Typical extract name: "My Friends and Family Slack export Jul 21 2018 - Sep 06 2018"
-    # If that's not the format, we will just fall back to the extension-free filename.
-    (workspace_name, _) = noext_filename.split(" Slack export ", 1)
-    return {
-        "readable_path": extracted_path,
-        "basename": base_filename,
-        "stripped_name": noext_filename,
-        "workspace_name": workspace_name,
-    }
+import hashlib
+import json
+import os
+import zipfile
+import io
+
+from os.path import basename, splitext
+
+import slackviewer
+from slackviewer.constants import SLACKVIEWER_TEMP_PATH
+from slackviewer.utils.six import to_unicode, to_bytes
+
+
+def SHA1_file(filepath, extra=b''):
+    """
+    Returns hex digest of SHA1 hash of file at filepath
+
+    :param str filepath: File to hash
+
+    :param bytes extra: Extra content added to raw read of file before taking hash
+
+    :return: hex digest of hash
+
+    :rtype: str
+    """
+    h = hashlib.sha1()
+    with io.open(filepath, 'rb') as f:
+        for chunk in iter(lambda: f.read(h.block_size), b''):
+            h.update(chunk)
+    h.update(extra)
+    return h.hexdigest()
+
+
+def extract_archive(filepath):
+    """
+    Returns the path of the archive
+
+    :param str filepath: Path to file to extract or read
+
+    :return: path of the archive
+
+    :rtype: str
+    """
+
+    # Checks if file path is a directory
+    if os.path.isdir(filepath):
+        path = os.path.abspath(filepath)
+        print("Archive already extracted. Viewing from {}...".format(path))
+        return path
+
+    # Checks if the filepath is a zipfile and continues to extract if it is
+    # if not it raises an error
+    elif not zipfile.is_zipfile(filepath):
+        # Misuse of TypeError? :P
+        raise TypeError("{} is not a zipfile".format(filepath))
+
+    archive_sha = SHA1_file(
+        filepath=filepath,
+        # Add version of slackviewer to hash as well so we can invalidate the cached copy
+        #  if there are new features added
+        extra=to_bytes(slackviewer.__version__)
+    )
+
+    extracted_path = os.path.join(SLACKVIEWER_TEMP_PATH, archive_sha)
+
+    if os.path.exists(extracted_path):
+        print("{} already exists".format(extracted_path))
+    else:
+        # Extract zip
+        with zipfile.ZipFile(filepath) as zip:
+            print("{} extracting to {}...".format(filepath, extracted_path))
+            for info in zip.infolist():
+                print(info.filename)
+                info.filename = info.filename.encode("cp437").decode("utf-8")
+                print(info.filename)
+                zip.extract(info,path=extracted_path)
+
+
+        print("{} extracted to {}".format(filepath, extracted_path))
+
+        # Add additional file with archive info
+        create_archive_info(filepath, extracted_path, archive_sha)
+
+    return extracted_path
+
+
+# Saves archive info
+# When loading empty dms and there is no info file then this is called to
+# create a new archive file
+def create_archive_info(filepath, extracted_path, archive_sha=None):
+    """
+    Saves archive info to a json file
+
+    :param str filepath: Path to directory of archive
+
+    :param str extracted_path: Path to directory of archive
+
+    :param str archive_sha: SHA string created when archive was extracted from zip
+    """
+
+    archive_info = {
+        "sha1": archive_sha,
+        "filename": os.path.split(filepath)[1],
+    }
+
+    with io.open(
+        os.path.join(
+            extracted_path,
+            ".slackviewer_archive_info.json",
+        ), 'w+', encoding="utf-8"
+    ) as f:
+        s = json.dumps(archive_info, ensure_ascii=False)
+        s = to_unicode(s)
+        f.write(s)
+
+
+def get_export_info(archive_name):
+    """
+    Given a file or directory, extract it and return information that will be used in
+    an export printout: the basename of the file, the name stripped of its extension, and
+    our best guess (based on Slack's current naming convention) of the name of the
+    workspace that this is an export of.
+    """
+    extracted_path = extract_archive(archive_name)
+    base_filename = basename(archive_name)
+    (noext_filename, _) = splitext(base_filename)
+    # Typical extract name: "My Friends and Family Slack export Jul 21 2018 - Sep 06 2018"
+    # If that's not the format, we will just fall back to the extension-free filename.
+    (workspace_name, _) = noext_filename.split(" Slack export ", 1)
+    return {
+        "readable_path": extracted_path,
+        "basename": base_filename,
+        "stripped_name": noext_filename,
+        "workspace_name": workspace_name,
+    }
```

### Comparing `slack-export-viewer-1.1.4/slackviewer/cli.py` & `slack-export-viewer-1.1.5/slackviewer/cli.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/formatter.py` & `slack-export-viewer-1.1.5/slackviewer/formatter.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/main.py` & `slack-export-viewer-1.1.5/slackviewer/main.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/message.py` & `slack-export-viewer-1.1.5/slackviewer/message.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/reader.py` & `slack-export-viewer-1.1.5/slackviewer/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                 if 'reply_count' in message._message or 'replies' in message._message:
                     #   Identify and save where we are
                     reply_list = []
                     for reply in message._message.get('replies', []):
                         reply_list.append(reply)
                     reply_objects = []
                     for item in reply_list:
-                        item_lookup_key = (item['user'], item['ts'])
+                        item_lookup_key = (item.get('user'), item.get('ts'))
                         item_replies = user_ts_lookup.get(item_lookup_key)
                         if item_replies is not None:
                             reply_objects.extend(item_replies)
 
                     if not reply_objects:
                         continue
```

### Comparing `slack-export-viewer-1.1.4/slackviewer/static/viewer.css` & `slack-export-viewer-1.1.5/slackviewer/static/viewer.css`

 * *Files 7% similar despite different names*

```diff
@@ -55,28 +55,34 @@
 #sidebar h3.arrow::after {
   margin-left: 10px;
   -webkit-transform: none;
   transform: none;
 }
 
 .messages {
-    width: calc(100vw - 305px);
+    width: calc(100vw - 325px);
     height: 100vh;
     text-align: left;
     display: inline-block;
     padding-left: 20px;
+    padding-right: 20px;
     overflow-y: scroll;
 }
 
 .message-container {
     clear: left;
     min-height: 56px; // height of image plus 20px padding
 }
+
 .message-container:first-child {
-  margin-top: 20px;
+    margin-top: 20px;
+}
+
+.message-container:last-child {
+    margin-bottom: 20px;
 }
 
 .message-container .user_icon {
     background-color: rgb(248, 244, 240);
     width: 36px;
     height: 36px;
     border-radius: 0.2em;
@@ -119,17 +125,22 @@
     white-space: pre-wrap;
 }
 
 .message-container .message .msg {
     line-height: 1.5;
 }
 
+.message-container .message .msg a {
+    overflow-wrap: anywhere;
+}
+
 .message-container .message-attachment {
     padding-left: 5px;
     border-left: 2px gray solid;
+    overflow-wrap: anywhere;
 }
 
 .message-container .message-attachment .service-name {
     color: #999999;
 }
 
 .message-container .icon {
@@ -192,7 +203,12 @@
 .close {
   display: none;
 }
 
 @media screen {
     .print-only { display: none }
 }
+
+img.preview {
+    max-width: 100%;
+    height: auto;
+}
```

### Comparing `slack-export-viewer-1.1.4/slackviewer/templates/export_single.html` & `slack-export-viewer-1.1.5/slackviewer/templates/export_single.html`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/templates/util.html` & `slack-export-viewer-1.1.5/slackviewer/templates/util.html`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/templates/viewer.html` & `slack-export-viewer-1.1.5/slackviewer/templates/viewer.html`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/user.py` & `slack-export-viewer-1.1.5/slackviewer/user.py`

 * *Files identical despite different names*

### Comparing `slack-export-viewer-1.1.4/slackviewer/utils/six.py` & `slack-export-viewer-1.1.5/slackviewer/utils/six.py`

 * *Files identical despite different names*

