# Comparing `tmp/open-ephys-python-tools-0.1.4.tar.gz` & `tmp/open-ephys-python-tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-ephys-python-tools-0.1.4.tar", last modified: Wed Jan 18 01:19:08 2023, max compression
+gzip compressed data, was "open-ephys-python-tools-0.1.5.tar", last modified: Tue Jun  6 23:28:24 2023, max compression
```

## Comparing `open-ephys-python-tools-0.1.4.tar` & `open-ephys-python-tools-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.202680 open-ephys-python-tools-0.1.4/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)      137 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/.gitignore
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1577 2023-01-18 01:15:00.000000 open-ephys-python-tools-0.1.4/CHANGELOG.md
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1049 2020-11-10 21:10:52.000000 open-ephys-python-tools-0.1.4/LICENSE
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     5654 2023-01-18 01:19:08.202680 open-ephys-python-tools-0.1.4/PKG-INFO
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     5277 2022-11-03 20:39:10.000000 open-ephys-python-tools-0.1.4/README.md
--rw-r--r--   0 joshs     (1001) joshs     (1001)   367061 2020-11-10 22:41:18.000000 open-ephys-python-tools-0.1.4/logo.png
--rw-rw-r--   0 joshs     (1001) joshs     (1001)      664 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/pyproject.toml
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       38 2023-01-18 01:19:08.202680 open-ephys-python-tools-0.1.4/setup.cfg
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       68 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/setup.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.198680 open-ephys-python-tools-0.1.4/src/
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.198680 open-ephys-python-tools-0.1.4/src/open_ephys/
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       21 2023-01-18 01:15:05.000000 open-ephys-python-tools-0.1.4/src/open_ephys/__init__.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.198680 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     9037 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/README.md
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       63 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/__init__.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.198680 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)    14487 2023-01-18 01:17:43.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/BinaryRecording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8127 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/NwbRecording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)    18423 2022-12-14 18:27:04.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/OpenEphysRecording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)      134 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/__init__.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.198680 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/helpers/
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       75 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/helpers/__init__.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8848 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)    10642 2022-12-14 18:38:41.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/recording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     3048 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/recordnode.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     2984 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/analysis/session.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.198680 open-ephys-python-tools-0.1.4/src/open_ephys/control/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1926 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/control/README.md
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       88 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/control/__init__.py
--rw-rw-r--   0 joshs     (1001) joshs     (1001)    15469 2022-12-14 18:38:41.000000 open-ephys-python-tools-0.1.4/src/open_ephys/control/http_server.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     4888 2022-11-03 20:34:26.000000 open-ephys-python-tools-0.1.4/src/open_ephys/control/network_control.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.202680 open-ephys-python-tools-0.1.4/src/open_ephys/streaming/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     2123 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/streaming/README.md
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       41 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.4/src/open_ephys/streaming/__init__.py
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     4008 2022-11-02 23:58:43.000000 open-ephys-python-tools-0.1.4/src/open_ephys/streaming/event_listener.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-01-18 01:19:08.202680 open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     5654 2023-01-18 01:19:08.000000 open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/PKG-INFO
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1105 2023-01-18 01:19:08.000000 open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 joshs     (1001) joshs     (1001)        1 2023-01-18 01:19:08.000000 open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       31 2023-01-18 01:19:08.000000 open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/requires.txt
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       11 2023-01-18 01:19:08.000000 open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/top_level.txt
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)      137 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/.gitignore
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1577 2023-01-18 01:15:00.000000 open-ephys-python-tools-0.1.5/CHANGELOG.md
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1049 2020-11-10 21:10:52.000000 open-ephys-python-tools-0.1.5/LICENSE
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     5654 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/PKG-INFO
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     5277 2022-11-03 20:39:10.000000 open-ephys-python-tools-0.1.5/README.md
+-rw-r--r--   0 joshs     (1001) joshs     (1001)   367061 2020-11-10 22:41:18.000000 open-ephys-python-tools-0.1.5/logo.png
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)      664 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/pyproject.toml
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       38 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/setup.cfg
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       68 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/setup.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.812211 open-ephys-python-tools-0.1.5/src/
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys/
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       21 2023-06-06 23:24:33.000000 open-ephys-python-tools-0.1.5/src/open_ephys/__init__.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     9014 2023-06-06 22:43:04.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/README.md
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       63 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/__init__.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)    14487 2023-01-18 01:17:43.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/BinaryRecording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8271 2023-06-06 22:43:04.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/NwbRecording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)    18590 2023-06-06 22:43:04.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/OpenEphysRecording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)      134 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/__init__.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/helpers/
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       75 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/helpers/__init__.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8852 2023-06-06 22:43:04.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)    10547 2023-06-06 22:43:04.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/recording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     3048 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/recordnode.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     2984 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/analysis/session.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys/control/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1926 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/control/README.md
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       88 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/control/__init__.py
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)    15469 2022-12-14 18:38:41.000000 open-ephys-python-tools-0.1.5/src/open_ephys/control/http_server.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     4888 2022-11-03 20:34:26.000000 open-ephys-python-tools-0.1.5/src/open_ephys/control/network_control.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys/streaming/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     2123 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/streaming/README.md
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       41 2022-10-31 16:38:45.000000 open-ephys-python-tools-0.1.5/src/open_ephys/streaming/__init__.py
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     4008 2022-11-02 23:58:43.000000 open-ephys-python-tools-0.1.5/src/open_ephys/streaming/event_listener.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-06-06 23:28:24.816212 open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     5654 2023-06-06 23:28:24.000000 open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1105 2023-06-06 23:28:24.000000 open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)        1 2023-06-06 23:28:24.000000 open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       31 2023-06-06 23:28:24.000000 open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/requires.txt
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       11 2023-06-06 23:28:24.000000 open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/top_level.txt
```

### Comparing `open-ephys-python-tools-0.1.4/CHANGELOG.md` & `open-ephys-python-tools-0.1.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/LICENSE` & `open-ephys-python-tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/PKG-INFO` & `open-ephys-python-tools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-ephys-python-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Software tools for interfacing with the Open Ephys GUI
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `open-ephys-python-tools-0.1.4/README.md` & `open-ephys-python-tools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/logo.png` & `open-ephys-python-tools-0.1.5/logo.png`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/pyproject.toml` & `open-ephys-python-tools-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/README.md` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 The `open_ephys.analysis` module loads does not have a separate hierarchical level for experiments. Instead, each recording (regardless of the experiment index) is accessed through the `session.recordnodes[N].recordings` list.
 
 To view information about a specific recording
 
 Note that Open Ephys starts numbering experiments and recordings at 1, but the `Recording` object stores the zero-based indices:
 
 ```
->> print(session.recordnodes[0].recording[0])
+>> print(session.recordnodes[0].recordings[0])
 
 Open Ephys GUI Recording
 ID: 0x7fe5c80babb0
 Format: Binary
 Directory: /path/to/session/2021-01-10_11-53-13/Record Node 103
 Experiment Index: 0
 Recording Index: 0
@@ -71,26 +71,26 @@
 - `sample_numbers` - a `numpy.ndarray` that holds the sample indices. This will have the same size as the first dimension of the `samples` array
 - `timestamps` - a `numpy.ndarray` that holds global timestamps (in seconds) for each sample, assuming all data streams were synchronized in this recording. This will have the same size as the first dimension of the `samples` array
 - `metadata` - a `dict` containing information about this data, such as the ID of the processor it originated from.
 
 Because the memory-mapped samples are stored as 16-bit integers in arbitrary units, all analysis should be done on a scaled version of these samples. To load the samples scaled to microvolts, use the `get_samples()` method:
 
 ```python
->> recording = session.recordnodes[0].recording[0]
+>> recording = session.recordnodes[0].recordings[0]
 >> data = recording.continuous[0].get_samples(start_sample_index=0, end_sample_index=10000)
 ```
 
 This will return the first 10,000 continuous samples for all channels in units of microvolts. Note that your computer may run out of memory when requesting a large number of samples for many channels at once.
 
 ### Using the Open Ephys data format
 
 Because the data files from the Open Ephys format cannot be memory-mapped effectively, all of the samples must be loaded into memory from the start. For long recordings, it may not be possible to fit all of the channels into memory at once. Before requesting the `samples` property of a `continuous` object in Open Ephys format, you can uses the following functions to restrict the data to a certain sample range or a certain set of channels:
 
 ```python
->> recording = session.recordnodes[0].recording[0] # loads the sample numbers, timestamps, and metadata
+>> recording = session.recordnodes[0].recordings[0] # loads the sample numbers, timestamps, and metadata
 >> recording.set_sample_range([10000, 50000])
 >> recording.set_selected_channels([np.arange(10,15)])
 >> recording.samples.shape  # loads the samples
 (40000, 5)
 
 ```
 
@@ -121,30 +121,30 @@
 If your recording contains data from multiple streams that were not synchronized during the recording, you'll likely want to synchronize their timestamps prior to further analysis.
 
 Assuming they each have one event channel that was connected to the same _physical digital input line_, synchronization is straightforward.
 
 First, indicate which event lines share the sync input (this will depend on your recording configuration):
 
 ```python
-recording = session.recordnodes[0].recording[0]
+recording = session.recordnodes[0].recordings[0]
 
-recording.add_sync_line(8,          # TTL line number
-                        102,        # processor ID
-                        0,          # stream index (defaults to 0)
-                        main=True)  # use as the main stream
-
-recording.add_sync_line(1,          # TTL line number
-                        100,        # processor ID
-                        0,          # stream index (defaults to 0)
-                        main=False) # align to the main stream
-
-recording.add_sync_line(1,          # TTL line number
-                        100,        # processor ID
-                        1,          # stream index (defaults to 0)
-                        main=False) # align to the main stream
+recording.add_sync_line(8,            # TTL line number
+                        102,          # processor ID
+                        'Probe-A-AP', # stream name
+                        main=True)    # use as the main stream
+
+recording.add_sync_line(1,            # TTL line number
+                        100,          # processor ID
+                        'Probe-A-LFP',# stream name
+                        main=False)   # align to the main stream
+
+recording.add_sync_line(1,            # TTL line number
+                        100,          # processor ID
+                        'PXI-6133',   # stream name
+                        main=False)   # align to the main stream
 ```
 
 You must have one and only one "main" stream, and at least one "auxiliary" stream for synchronization to work.
 
 Next, running:
 
 ```python
```

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/BinaryRecording.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/BinaryRecording.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/NwbRecording.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/NwbRecording.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         processor_ids = []
         
         for dataset in datasets:
             
             if (dataset[-4:] == '.TTL'):
 
                 processor_id = int(dataset.split('.')[0].split('-')[1])
+                stream_name = dataset.split('.')[1]
 
                 if processor_id not in processor_ids:
                     processor_ids.append(processor_id)
                     stream_id = 0
                 else:
                     stream_id += 1
                 
@@ -158,28 +159,27 @@
                 
                 events.append(pd.DataFrame(
                     data = {'line' : np.abs(channel_states),
                             'timestamp' : timestamps,
                             'sample_number' : sample_numbers,
                             'processor_id' : [processor_id] * len(channel_states),
                             'stream_index' : [stream_id] * len(channel_states),
+                            'stream_name' : [stream_name] * len(channel_states),
                             'state' : (np.sign(channel_states) + 1 / 2).astype('int')}))
-        
-        self._events = pd.concat(events)
-        self._events.sort_values(by='timestamp')
+        self._events = pd.concat(events).sort_values(by=['sample_number', 'stream_index'], ignore_index=True)
 
     def load_messages(self):
         pass
         
     def __str__(self):
         """Returns a string with information about the Recording"""
         
         return "Open Ephys GUI Recording\n" + \
                 "ID: " + hex(id(self)) + '\n' + \
-                "Format: NWB 1.0\n" + \
+                "Format: NWB 2.0\n" + \
                 "Directory: " + self.directory + "\n" + \
                 "Experiment Index: " + str(self.experiment_index) + "\n" + \
                 "Recording Index: " + str(self.recording_index)
```

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/OpenEphysRecording.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/OpenEphysRecording.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             self._samples = None
             self.sample_numbers = self._sample_numbers_internal
             self.sample_range = [self.sample_numbers[0], self.sample_numbers[-1]+1]
             self.selected_channels = np.arange(len(files))
 
             self.metadata = {}
 
-            self.metadata['source_node_id'] = info['source_node_id']
+            self.metadata['source_node_id'] = int(info['source_node_id'])
             self.metadata['source_node_name'] = info['source_node_name']
 
             self.metadata['stream_name'] = info['stream_name']
 
             self.metadata['sample_rate'] = info['sample_rate']
             self.metadata['num_channels'] = len(files)
 
@@ -204,20 +204,21 @@
 
             start = np.searchsorted(self._sample_numbers_internal, self.sample_range[0])
             end = np.searchsorted(self._sample_numbers_internal, self.sample_range[1])
             self.timestamps = self._timestamps_internal[start:end]
 
         def _load_timestamps(self):
 
-            data = np.array(np.memmap(self.timestamps_file, dtype='<f8', offset=0, mode='r'))[self.valid_records]
+            data = np.memmap(self.timestamps_file, dtype='<f8', offset=0, mode='r')[self.valid_records]
             data = np.append(data, 2 * data[-1] - data[-2])
 
-            self._timestamps_internal = np.array([])
+            self._timestamps_internal = []
+
             for i in range(len(data)-1):
-                self._timestamps_internal = np.append(self._timestamps_internal, np.linspace(data[i], data[i+1], 1024, endpoint=True))
+                self._timestamps_internal.extend(np.linspace(data[i], data[i+1], 1024, endpoint=True))
             
             self.timestamps = self._timestamps_internal
 
    
             
     def __init__(self, directory, experiment_index=0, recording_index=0):
         
@@ -271,24 +272,26 @@
         events = []
         
         for recording_index, child in enumerate(root):
             if (recording_index == self.recording_index):
                 for stream_index, stream in enumerate(child):
                     for file_index, file in enumerate(stream):
                         if file.tag == 'EVENTS':
+                            stream_name = file.get('filename').replace('_','.').split('.')[1]
                             sample_number, processor_id, state, channel, header = \
                                 load(os.path.join(self.directory, 
                                       file.get('filename')), self.recording_index)
                             events.append(pd.DataFrame(data = {'line' : channel + 1,
                               'sample_number' : sample_number,
                               'processor_id' : processor_id,
                               'stream_index' : [stream_index] * len(sample_number),
+                              'stream_name' : [stream_name] * len(sample_number),
                               'state' : state}))
 
-        self._events = pd.concat(events).sort_values(by='sample_number')
+        self._events = pd.concat(events).sort_values(by=['sample_number', 'stream_index'], ignore_index=True)
 
     def load_messages(self):
         
         if len(self.experiment_id) == 0:
             messages_file = os.path.join(self.directory, 'messages' + '.events')
         else:
             messages_file = os.path.join(self.directory, 'messages_' + str(self.experiment_id) + '.events')
```

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     
     """
     
     header = readHeader(filename)
 
     sample_numbers = np.array(np.memmap(filename, dtype='<i8', offset=1024, mode='r')[::2])
     
-    data = np.memmap(filename, dtype='<u1', offset=1024, mode='r', shape=(len(timestamps), EVENT_RECORD_SIZE //2))
+    data = np.memmap(filename, dtype='<u1', offset=1024, mode='r', shape=(len(sample_numbers), EVENT_RECORD_SIZE //2))
     
     recording_number = np.array(data[:,14])
     
     mask = recording_number == recording_index
     processor_id = np.array(data[mask,11])
     state = np.array(data[mask,12])
     channel = np.array(data[mask,13])
```

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/recording.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/recording.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,31 +158,31 @@
         pass
     
     @abstractmethod
     def __str__(self):
         """Returns a string with information about the Recording"""
         pass
     
-    def add_sync_line(self, line, processor_id, stream_name=0, main=False):
+    def add_sync_line(self, line, processor_id, stream_name=None, main=False):
         """Specifies an event channel to use for timestamp synchronization. Each 
         sync line in a recording should receive its input from the same 
         physical digital input line.
         
         For synchronization to work, there must be one (and only one) 'main' 
         sync line, to which all timestamps will be aligned.
         
         Parameters
         ----------
         channel : int
             event channel number
         processor_id : int
-            ID for the processor receiving sync events
-        stream_index : int
-            index of the stream receiving sync events
-            default = 0
+            ID for the processor receiving sync events (eg 101)
+        stream_name : str
+            name of the stream receiving sync events (eg 'Probe-A-AP')
+            default = None
         main : bool
             if True, this stream's timestamps will be treated as the 
             main clock
         
         """
         
         if main:
@@ -269,31 +269,29 @@
                 if (continuous.metadata['source_node_id'] == sync['processor_id']) and \
                    (continuous.metadata['stream_name'] == main['stream_name']):
                        
                     continuous.global_timestamps = \
                         ((continuous.sample_numbers - sync['start']) * sync['scaling'] \
                             + sync['offset']) 
                             
-                    if self.format != 'nwb': # already scaled to seconds
-                        continuous.global_timestamps = continuous.global_timestamps / sync['sample_rate']
+                    continuous.global_timestamps = continuous.global_timestamps / sync['sample_rate'] / sync['scaling']
                             
             event_inds = self.events[(self.events.processor_id == sync['processor_id']) & 
                    (self.events.stream_name == sync['stream_name'])].index.values
 
             global_timestamps = (self.events.loc[event_inds].sample_number - sync['start']) \
                                   * sync['scaling'] \
                                    + sync['offset']
                                    
-            if self.format != 'nwb': #already scaled to seconds
-                global_timestamps = global_timestamps / sync['sample_rate']
+            global_timestamps = global_timestamps / sync['sample_rate']
             
             for ind, ts in zip(event_inds, global_timestamps):
                 self.events.at[ind, 'global_timestamp'] = ts
             
             
                             
                                               
         
         
     
         
-    
+
```

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/recordnode.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/recordnode.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/analysis/session.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/analysis/session.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/control/README.md` & `open-ephys-python-tools-0.1.5/src/open_ephys/control/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/control/http_server.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/control/http_server.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/control/network_control.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/control/network_control.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/streaming/README.md` & `open-ephys-python-tools-0.1.5/src/open_ephys/streaming/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys/streaming/event_listener.py` & `open-ephys-python-tools-0.1.5/src/open_ephys/streaming/event_listener.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/PKG-INFO` & `open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-ephys-python-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Software tools for interfacing with the Open Ephys GUI
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `open-ephys-python-tools-0.1.4/src/open_ephys_python_tools.egg-info/SOURCES.txt` & `open-ephys-python-tools-0.1.5/src/open_ephys_python_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

