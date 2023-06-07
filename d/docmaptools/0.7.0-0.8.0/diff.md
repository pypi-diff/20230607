# Comparing `tmp/docmaptools-0.7.0.tar.gz` & `tmp/docmaptools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmaptools-0.7.0.tar", last modified: Fri Apr 28 01:29:28 2023, max compression
+gzip compressed data, was "docmaptools-0.8.0.tar", last modified: Wed Jun  7 16:32:50 2023, max compression
```

## Comparing `docmaptools-0.7.0.tar` & `docmaptools-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-04-28 01:28:58.000000 docmaptools-0.7.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-04-28 01:28:58.000000 docmaptools-0.7.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-28 01:29:28.692159 docmaptools-0.7.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-04-28 01:28:58.000000 docmaptools-0.7.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/docmaptools/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-04-28 01:28:58.000000 docmaptools-0.7.0/docmaptools/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-04-28 01:28:58.000000 docmaptools-0.7.0/docmaptools/convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     8128 2023-04-28 01:28:58.000000 docmaptools-0.7.0/docmaptools/parse.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/docmaptools.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-04-28 01:28:58.000000 docmaptools-0.7.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-04-28 01:29:28.692159 docmaptools-0.7.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-04-28 01:28:58.000000 docmaptools-0.7.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/tests/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-04-28 01:28:58.000000 docmaptools-0.7.0/tests/test_convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-04-28 01:28:58.000000 docmaptools-0.7.0/tests/test_init.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    28557 2023-04-28 01:28:58.000000 docmaptools-0.7.0/tests/test_parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-06-07 16:32:18.000000 docmaptools-0.8.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-06-07 16:32:18.000000 docmaptools-0.8.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-06-07 16:32:50.566735 docmaptools-0.8.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-06-07 16:32:18.000000 docmaptools-0.8.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/docmaptools/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-06-07 16:32:18.000000 docmaptools-0.8.0/docmaptools/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-06-07 16:32:18.000000 docmaptools-0.8.0/docmaptools/convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8585 2023-06-07 16:32:18.000000 docmaptools-0.8.0/docmaptools/parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/docmaptools.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-06-07 16:32:50.000000 docmaptools-0.8.0/docmaptools.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-06-07 16:32:18.000000 docmaptools-0.8.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-07 16:32:50.566735 docmaptools-0.8.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-06-07 16:32:18.000000 docmaptools-0.8.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-07 16:32:50.566735 docmaptools-0.8.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-06-07 16:32:18.000000 docmaptools-0.8.0/tests/test_convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-06-07 16:32:18.000000 docmaptools-0.8.0/tests/test_init.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    33743 2023-06-07 16:32:18.000000 docmaptools-0.8.0/tests/test_parse.py
```

### Comparing `docmaptools-0.7.0/LICENSE` & `docmaptools-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docmaptools-0.7.0/PKG-INFO` & `docmaptools-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.7.0
+Version: 0.8.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.7.0/docmaptools/__init__.py` & `docmaptools-0.8.0/docmaptools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
 
 
 def configure_logging(filename, level=logging.INFO, format_string=None):
```

### Comparing `docmaptools-0.7.0/docmaptools/convert.py` & `docmaptools-0.8.0/docmaptools/convert.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.7.0/docmaptools/parse.py` & `docmaptools-0.8.0/docmaptools/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,27 +81,37 @@
 
 
 def docmap_preprint_history(d_json):
     "return a list of events in a preprint publication history from the docmap"
     step_json = docmap_first_step(d_json)
     preprint_events = []
     found_first_preprint = False
+    # add preprint first
+    if docmap_preprint(d_json):
+        # collect the preprint details
+        event_details = preprint_event_output(
+            docmap_preprint(d_json), step_json, found_first_preprint
+        )
+        # append the events details to the matser list
+        preprint_events.append(event_details)
+        found_first_preprint = True
     while step_json:
         for action_json in step_actions(step_json):
             for output_json in action_outputs(action_json):
                 if output_json.get("type") == "preprint":
                     # decide whether to record this step
                     if not output_json.get("identifier") and found_first_preprint:
                         continue
                     # collect the preprint details
                     event_details = preprint_event_output(
                         output_json, step_json, found_first_preprint
                     )
                     # append the events details to the matser list
-                    preprint_events.append(event_details)
+                    if event_details.get("date"):
+                        preprint_events.append(event_details)
 
                     # will have found the preprint from the first matched step
                     found_first_preprint = True
         # search the next step
         step_json = next_step(d_json, step_json)
     return preprint_events
 
@@ -129,29 +139,29 @@
 
 def preprint_happened_date(step_json):
     "happened date from a preprint step assertions"
     # look at assertions
     if not step_json or not step_json.get("assertions"):
         return None
     for assertion in step_json.get("assertions", []):
-        if assertion.get("happened"):
+        if assertion.get("status") == "manuscript-published" and assertion.get("happened"):
             return assertion.get("happened")
     return None
 
 
 def preprint_alternate_date(step_json):
     "date for a preprint from its step outputs when no happened date is available"
     # if no date is yet found, look at other action output
     if not step_json or not step_actions(step_json):
         return None
     for action_json in step_actions(step_json):
         for output_json in action_outputs(action_json):
             if (
                 output_json.get("published")
-                and output_json.get("type") == "evaluation-summary"
+                and output_json.get("type") == "preprint"
             ):
                 return output_json.get("published")
     return None
 
 
 def step_actions(step_json):
     "return the actions of the step"
```

### Comparing `docmaptools-0.7.0/docmaptools.egg-info/PKG-INFO` & `docmaptools-0.8.0/docmaptools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.7.0
+Version: 0.8.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.7.0/setup.py` & `docmaptools-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.7.0/tests/test_convert.py` & `docmaptools-0.8.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.7.0/tests/test_init.py` & `docmaptools-0.8.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.7.0/tests/test_parse.py` & `docmaptools-0.8.0/tests/test_parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -151,35 +151,23 @@
                 "identifier": "85111",
                 "versionIdentifier": "2",
                 "doi": "10.7554/eLife.85111.2",
             },
         )
 
     def test_docmap_preprint_history(self):
-        "list of preprint history event data"
+        "list of preprint history event data for steps with a published date"
         result = parse.docmap_preprint_history(self.d_json)
         expected = [
             {
                 "type": "preprint",
                 "doi": "10.1101/2022.11.08.515698",
                 "versionIdentifier": "2",
                 "date": "2022-11-22",
             },
-            {
-                "type": "reviewed-preprint",
-                "doi": "10.7554/eLife.85111.1",
-                "versionIdentifier": "1",
-                "date": "2022-11-28T11:30:05+00:00",
-            },
-            {
-                "type": "reviewed-preprint",
-                "doi": "10.7554/eLife.85111.2",
-                "versionIdentifier": "2",
-                "date": "2023-04-14T13:42:25.781585+00:00",
-            },
         ]
         self.assertEqual(result, expected)
 
     def test_step_actions(self):
         "get actions from the last step"
         step_2 = parse.next_step(
             self.d_json,
@@ -232,14 +220,169 @@
                     ),
                 ]
             ),
         ]
         self.assertEqual(result, expected)
 
 
+class TestDocmapSteps86628Sample(unittest.TestCase):
+    def setUp(self):
+        docmap_string = read_fixture("sample_docmap_for_86628.json", mode="r")
+        self.d_json = json.loads(docmap_string)
+
+    def test_docmap_steps(self):
+        "get the steps of the docmap"
+        result = parse.docmap_steps(self.d_json)
+        self.assertEqual(len(result), 6)
+
+    def test_docmap_first_step(self):
+        "get the first step according to the first-step value"
+        result = parse.docmap_first_step(self.d_json)
+
+        self.assertEqual(len(result), 4)
+        self.assertEqual(
+            sorted(result.keys()), ["actions", "assertions", "inputs", "next-step"]
+        )
+
+    def test_step_inputs(self):
+        "get inputs from the first step"
+        first_step = parse.docmap_first_step(self.d_json)
+        result = parse.step_inputs(first_step)
+        self.assertEqual(len(result), 1)
+        # step _:b1
+        step_1 = parse.next_step(self.d_json, first_step)
+        result = parse.step_inputs(step_1)
+        self.assertEqual(len(result), 1)
+        # step _:b2
+        step_2 = parse.next_step(self.d_json, step_1)
+        result = parse.step_inputs(step_2)
+        self.assertEqual(len(result), 3)
+        # step _:b3
+        step_3 = parse.next_step(self.d_json, step_2)
+        result = parse.step_inputs(step_3)
+        self.assertEqual(len(result), 1)
+        # step _:b4
+        step_4 = parse.next_step(self.d_json, step_3)
+        result = parse.step_inputs(step_4)
+        self.assertEqual(len(result), 1)
+        # step _:b5
+        step_5 = parse.next_step(self.d_json, step_4)
+        result = parse.step_inputs(step_5)
+        self.assertEqual(len(result), 4)
+        self.assertEqual(step_5.get("next-step"), None)
+
+    def test_docmap_preprint(self):
+        "preprint data from the first step inputs"
+        result = parse.docmap_preprint(self.d_json)
+        self.assertDictEqual(
+            result,
+            {
+                "type": "preprint",
+                "doi": "10.1101/2023.02.14.528498",
+                "url": "https://www.biorxiv.org/content/10.1101/2023.02.14.528498v2",
+                "versionIdentifier": "2",
+                "published": "2023-02-21",
+                "_tdmPath": "s3://transfers-elife/biorxiv_Current_Content/February_2023/22_Feb_23_Batch_1531/c27a22b7-6c43-1014-aa80-efc7cf011f1d.meca",
+            },
+        )
+
+    def test_docmap_latest_preprint(self):
+        "preprint data from the most recent step inputs"
+        result = parse.docmap_latest_preprint(self.d_json)
+        self.assertDictEqual(
+            result,
+            {
+                "type": "preprint",
+                "identifier": "86628",
+                "doi": "10.7554/eLife.86628.2",
+                "versionIdentifier": "2",
+                "license": "http://creativecommons.org/licenses/by/4.0/",
+                "published": "TBC",
+            },
+        )
+
+    def test_docmap_preprint_history(self):
+        "list of preprint history event data"
+        result = parse.docmap_preprint_history(self.d_json)
+        expected = [
+            {
+                "type": "preprint",
+                "doi": "10.1101/2023.02.14.528498",
+                "versionIdentifier": "2",
+                "date": "2023-02-21",
+            },
+            {
+                "type": "reviewed-preprint",
+                "doi": "10.7554/eLife.86628.1",
+                "versionIdentifier": "1",
+                "date": "TBC",
+            },
+            {
+                "type": "reviewed-preprint",
+                "doi": "10.7554/eLife.86628.2",
+                "versionIdentifier": "2",
+                "date": "TBC",
+            },
+        ]
+        self.assertEqual(result, expected)
+
+    def test_step_actions(self):
+        "get actions from the second step"
+        step_2 = parse.next_step(
+            self.d_json,
+            parse.next_step(self.d_json, parse.docmap_first_step(self.d_json)),
+        )
+        result = parse.step_actions(step_2)
+        self.assertEqual(len(result), 1)
+
+    def test_action_outputs(self):
+        "outputs from a step action"
+        first_step = parse.docmap_first_step(self.d_json)
+        first_action = parse.step_actions(first_step)[0]
+        result = parse.action_outputs(first_action)
+        self.assertEqual(len(result), 1)
+
+    def test_docmap_content(self):
+        "test parsing docmap JSON into docmap content structure"
+        result = parse.docmap_content(self.d_json)
+        expected = [
+            OrderedDict(
+                [
+                    ("type", "reply"),
+                    ("published", "2023-05-11T11:34:27.242112+00:00"),
+                    (
+                        "web-content",
+                        "https://sciety.org/evaluations/hypothesis:yVioUu_vEe2vQTPxYtnZSw/content",
+                    ),
+                ]
+            ),
+            OrderedDict(
+                [
+                    ("type", "review-article"),
+                    ("published", "2023-05-11T11:34:28.135284+00:00"),
+                    (
+                        "web-content",
+                        "https://sciety.org/evaluations/hypothesis:yeEcZO_vEe2Dxo8DxUJqTw/content",
+                    ),
+                ]
+            ),
+            OrderedDict(
+                [
+                    ("type", "evaluation-summary"),
+                    ("published", "2023-05-11T11:34:28.903631+00:00"),
+                    (
+                        "web-content",
+                        "https://sciety.org/evaluations/hypothesis:ylaROO_vEe2VSj_o0Xi_gA/content",
+                    ),
+                ]
+            ),
+        ]
+        self.assertEqual(result, expected)
+
+
 class TestDocmapPreprint(unittest.TestCase):
     def test_docmap_preprint(self):
         "test case for when there is empty input"
         self.assertEqual(parse.docmap_preprint({}), {})
 
 
 class TestDocmapSteps446694(unittest.TestCase):
@@ -476,20 +619,14 @@
         expected = [
             {
                 "type": "preprint",
                 "doi": "10.1101/2022.10.17.512253",
                 "versionIdentifier": "1",
                 "date": "2022-10-17",
             },
-            {
-                "type": "reviewed-preprint",
-                "doi": "10.7554/eLife.84364.1",
-                "versionIdentifier": "1",
-                "date": "2022-11-08T07:01:52+00:00",
-            },
         ]
         self.assertEqual(result, expected)
 
     def test_step_actions(self):
         "get actions from the last step"
         step_2 = parse.next_step(
             self.d_json,
@@ -555,15 +692,19 @@
 
 class TestPreprintEventOutput(unittest.TestCase):
     def setUp(self):
         self.output_type = "preprint"
         self.output_doi = "10.7554/eLife.85111.1"
         self.output_version_identifier = "1"
         self.output_date_string = "2023-04-27T15:30:00+00:00"
-        self.step_json = {"assertions": [{"happened": self.output_date_string}]}
+        self.step_json = {
+            "assertions": [
+                {"status": "manuscript-published", "happened": self.output_date_string}
+            ]
+        }
 
     def test_not_found(self):
         "test if first preprint is not yet found"
         found_first_preprint = False
         output_json = {
             "type": self.output_type,
             "doi": self.output_doi,
@@ -601,15 +742,17 @@
         )
         self.assertDictEqual(result, expected)
 
 
 class TestPreprintHappenedDate(unittest.TestCase):
     def test_preprint_happened_date(self):
         date_string = "2023-04-27T15:30:00+00:00"
-        step_json = {"assertions": [{"happened": date_string}]}
+        step_json = {
+            "assertions": [{"status": "manuscript-published", "happened": date_string}]
+        }
         self.assertEqual(parse.preprint_happened_date(step_json), date_string)
 
     def test_none(self):
         step_json = None
         self.assertEqual(parse.preprint_happened_date(step_json), None)
 
 
@@ -617,15 +760,15 @@
     def test_preprint_alternate_date(self):
         date_string = "2023-04-27T15:30:00+00:00"
         step_json = {
             "actions": [
                 {
                     "outputs": [
                         {
-                            "type": "evaluation-summary",
+                            "type": "preprint",
                             "published": date_string,
                         }
                     ]
                 }
             ]
         }
         self.assertEqual(parse.preprint_alternate_date(step_json), date_string)
```

