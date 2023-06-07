# Comparing `tmp/alienpy-1.5.0.tar.gz` & `tmp/alienpy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alienpy-1.5.0.tar", last modified: Fri May  5 05:26:56 2023, max compression
+gzip compressed data, was "alienpy-1.5.1.tar", last modified: Wed Jun  7 06:54:00 2023, max compression
```

## Comparing `alienpy-1.5.0.tar` & `alienpy-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.444389 alienpy-1.5.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.5.0/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-05-05 05:26:56.443390 alienpy-1.5.0/PKG-INFO
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2022-12-20 08:02:48.000000 alienpy-1.5.0/README.md
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.442389 alienpy-1.5.0/alienpy/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2022-11-03 18:03:32.000000 alienpy-1.5.0/alienpy/__init__.py
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)    93304 2023-05-04 21:21:13.000000 alienpy-1.5.0/alienpy/alien.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2821 2023-03-16 23:03:24.000000 alienpy-1.5.0/alienpy/async_tools.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    13461 2023-05-02 22:25:03.000000 alienpy-1.5.0/alienpy/connect_ssl.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6900 2023-03-17 15:40:29.000000 alienpy-1.5.0/alienpy/data_structs.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1903 2023-05-02 22:31:24.000000 alienpy-1.5.0/alienpy/global_vars.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1491 2023-03-17 15:53:13.000000 alienpy-1.5.0/alienpy/setup_cwd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     2120 2023-05-02 22:41:20.000000 alienpy-1.5.0/alienpy/setup_logging.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    19706 2023-05-03 16:31:20.000000 alienpy-1.5.0/alienpy/tools_files.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    18022 2023-05-04 17:31:44.000000 alienpy-1.5.0/alienpy/tools_misc.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1719 2023-03-17 16:31:32.000000 alienpy-1.5.0/alienpy/tools_shell.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      851 2023-03-17 10:35:43.000000 alienpy-1.5.0/alienpy/tools_stackcmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2023-05-04 21:26:56.000000 alienpy-1.5.0/alienpy/version.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    16919 2023-05-04 16:55:53.000000 alienpy-1.5.0/alienpy/wb_api.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8986 2023-03-17 15:01:28.000000 alienpy-1.5.0/alienpy/wb_async.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    56632 2023-05-04 21:10:51.000000 alienpy-1.5.0/alienpy/xrd_core.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)    23884 2023-05-03 18:13:23.000000 alienpy-1.5.0/alienpy/xrd_tools.py
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.443390 alienpy-1.5.0/alienpy.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    10431 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      604 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      761 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/entry_points.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       56 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        8 2023-05-05 05:26:56.000000 alienpy-1.5.0/alienpy.egg-info/top_level.txt
-drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-05-05 05:26:56.443390 alienpy-1.5.0/examples/
--rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-12-20 08:02:48.000000 alienpy-1.5.0/examples/alien_wbtime
--rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2023-05-05 05:26:56.444389 alienpy-1.5.0/setup.cfg
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3343 2023-03-17 11:15:21.000000 alienpy-1.5.0/setup.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.756305 alienpy-1.5.1/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1538 2020-05-18 21:36:32.000000 alienpy-1.5.1/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-06-07 06:54:00.756305 alienpy-1.5.1/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     9570 2022-12-20 08:02:48.000000 alienpy-1.5.1/README.md
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.755305 alienpy-1.5.1/alienpy/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       17 2023-05-15 09:29:38.000000 alienpy-1.5.1/alienpy/__init__.py
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)    83476 2023-06-07 06:39:48.000000 alienpy-1.5.1/alienpy/alien.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2821 2023-06-06 09:00:33.000000 alienpy-1.5.1/alienpy/async_tools.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    14486 2023-06-06 15:39:51.000000 alienpy-1.5.1/alienpy/connect_ssl.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5936 2023-06-06 17:01:56.000000 alienpy-1.5.1/alienpy/data_structs.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3684 2023-06-06 17:18:24.000000 alienpy-1.5.1/alienpy/global_vars.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1671 2023-06-06 10:10:16.000000 alienpy-1.5.1/alienpy/setup_cwd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     2031 2023-06-06 10:37:54.000000 alienpy-1.5.1/alienpy/setup_logging.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1688 2023-06-06 17:02:39.000000 alienpy-1.5.1/alienpy/tools_history.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    44208 2023-06-06 20:30:18.000000 alienpy-1.5.1/alienpy/tools_nowb.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1875 2023-06-06 17:09:11.000000 alienpy-1.5.1/alienpy/tools_shell.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      881 2023-06-06 10:31:28.000000 alienpy-1.5.1/alienpy/tools_stackcmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      289 2023-06-07 06:53:28.000000 alienpy-1.5.1/alienpy/version.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    25028 2023-06-07 05:34:32.000000 alienpy-1.5.1/alienpy/wb_api.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10260 2023-06-06 17:09:39.000000 alienpy-1.5.1/alienpy/wb_async.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    58020 2023-06-06 19:23:52.000000 alienpy-1.5.1/alienpy/xrd_core.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    24075 2023-06-07 06:49:20.000000 alienpy-1.5.1/alienpy/xrd_tools.py
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.756305 alienpy-1.5.1/alienpy.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)    10431 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/PKG-INFO
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      606 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/SOURCES.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        1 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/dependency_links.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      828 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/entry_points.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       56 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/requires.txt
+-rw-r--r--   0 adrian    (1000) adrian    (1000)        8 2023-06-07 06:54:00.000000 alienpy-1.5.1/alienpy.egg-info/top_level.txt
+drwxr-xr-x   0 adrian    (1000) adrian    (1000)        0 2023-06-07 06:54:00.756305 alienpy-1.5.1/examples/
+-rwxr-xr-x   0 adrian    (1000) adrian    (1000)     2169 2022-12-20 08:02:48.000000 alienpy-1.5.1/examples/alien_wbtime
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       38 2023-06-07 06:54:00.756305 alienpy-1.5.1/setup.cfg
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4160 2023-06-06 11:45:37.000000 alienpy-1.5.1/setup.py
```

### Comparing `alienpy-1.5.0/LICENSE` & `alienpy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.0/PKG-INFO` & `alienpy-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.5.0/README.md` & `alienpy-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.0/alienpy/alien.py` & `alienpy-1.5.1/alienpy/alien.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,105 +8,82 @@
     sys.exit(1)
 
 import atexit
 import collections
 import datetime
 import difflib
 import json
-import re
 import signal
 from pathlib import Path
 import subprocess  # nosec
 import logging
 import shlex
 import statistics
-from typing import NamedTuple
 from typing import Union
-from typing import Optional
-from typing import Callable
-from typing import Iterator
-import traceback
 import time
-import urllib.request as urlreq
 from urllib.parse import urlparse
-import xml.dom.minidom as MD  # nosec
-import xml.etree.ElementTree as ET  # nosec
 
 # External imports
 try:
     import requests
 except Exception:
     print("requests module could not be imported! Make sure you can do:\npython3 -c 'import requests'", file = sys.stderr, flush = True)
     sys.exit(1)
 
-HAS_PPRINT = False
-try:
-    from rich.pretty import pprint
-    HAS_PPRINT = True
-except Exception:
-    print("rich module could not be imported! Not fatal, but some pretty print features will not be available.\n Make sure you can do:\npython3 -c 'from rich.pretty import pprint'", file = sys.stderr, flush = True)
-
-HAS_READLINE = False
-try:
-    import readline as rl  # type: ignore
-    HAS_READLINE = True
-except ImportError:
-    try:
-        import gnureadline as rl  # type: ignore  # mypy: no-redef
-        HAS_READLINE = True
-    except ImportError:
-        pass
-
-
-##################################################
-#   GLOBAL POINTER TO WB CONNECTION  #############
-ALIENPY_GLOBAL_WB = None
-##################################################
-##################################################
-#   GLOBAL VARS
-##################################################
-ALIENPY_EXECUTABLE = ''
+###############################################################
+##   IMPORT ALIENPY SUB-MODULES
 
+##   IMPORT GLOBAL VARIABLES
 from .global_vars import *  # nosec PYL-W0614
 
 ##   START LOGGING BEFORE ANYTHING ELSE
 from .setup_logging import print_out, print_err, setup_logging
-setup_logging(DEBUG, DEBUG_FILE)
+setup_logging(bool(DEBUG), DEBUG_FILE)
 
-##   Data strucutures definitons
-from .data_structs import *  # nosec PYL-W0614
+### Complex dependencies
 
-##   VERSION STRINGS
-from .version import *  # nosec PYL-W0614
+#########################
+#   ASYNCIO MECHANICS
+#########################
+from .wb_api import SendMsg, InitConnection, cd, retf_print, get_help_srv, token_regen, wb_ping
+#########################
 
 ##   SSL RELATED VARIABLES: TOKEN AND CERT NAMES
-from .connect_ssl import TOKENCERT_NAME, TOKENKEY_NAME, TOKENCERT_VALID, TOKENKEY_VALID, USERCERT_VALID, USERKEY_VALID, CertInfo, CertVerify, CertKeyMatch
+from .connect_ssl import CertInfo, CertVerify, CertKeyMatch
 
 ##   General misc functions library
-from .tools_misc import *  # nosec PYL-W0614
+from .tools_nowb import (exitcode, signal_handler, cleanup_temp, import_aliases, list_remove_item, convert_trace2dict, convert_jdl2dict,
+                         ccdb_json_cleanup, unixtime2local, file2list, queryML, convert_time, check_port, exit_message,
+                         get_arg, get_arg_value, PrintColor, is_help, get_lfn_key, name2regex, deltat_ms_perf, getCAcerts,
+                         mk_xml_local, file2file_dict, md5)
 
 # commands stack tools
 from .tools_stackcmd import push2stack, deque_pop_pos
 
-# shell related toold
-from .tools_shell import *  # nosec PYL-W0614
+# shell related tools
+from .tools_shell import runShellCMD
 
 # Session save
 from .setup_cwd import SessionSave, SessionRestore
 
-#########################
-#   ASYNCIO MECHANICS
-#########################
-from .wb_api import *  # nosec PYL-W0614
+# Setup history
+from .tools_history import setupHistory
 
 # XRootD functions
-from .xrd_core import *  # nosec PYL-W0614
+from .xrd_tools import lfn2meta, lfn2uri, expand_path_grid, extract_glob_pattern, list_files_grid
+from .xrd_core import (xrd_config_init, HAS_XROOTD, xrd_client, DO_XrootdCp,
+                       xrdfs_ping, xrdfs_q_config, xrdfs_q_stats, xrdstat2dict, xrdfs_stat, xrdstat_flags2dict,
+                       download_tmp, upload_tmp)
 # Global XRootD preferences
 xrd_config_init()
 
+##################################
+#   START FUNCTIONS DEFINITIONS
+##################################
+
 
 def DO_dirs(wb, args: Union[str, list, None] = None) -> RET:
     """dirs"""
     return DO_path_stack(wb, 'dirs', args)
 
 
 def DO_popd(wb, args: Union[str, list, None] = None) -> RET:
@@ -169,15 +146,15 @@
             if position > len(AlienSessionInfo['pathq']) - 1: return RET(0)  # type: ignore [call-arg]
             deque_pop_pos(AlienSessionInfo['pathq'], pos)
             msg = " ".join(AlienSessionInfo['pathq'])
             return RET(0, msg)  # type: ignore [call-arg]
 
         if not arg_list:
             AlienSessionInfo['pathq'].popleft()
-            if not do_not_cd: cd(wb, AlienSessionInfo['pathq'][0])  # cd to the new top of stack
+            if not do_not_cd and AlienSessionInfo['pathq']: cd(wb, AlienSessionInfo['pathq'][0])  # cd to the new top of stack
         msg = " ".join(AlienSessionInfo['pathq'])
         return RET(0, msg)  # type: ignore [call-arg]  # end of popd
 
     if cmd == "pushd":
         if position and sign:
             if position > len(AlienSessionInfo['pathq']) - 1: return RET(0)  # type: ignore [call-arg]
             if sign == "+":
@@ -534,15 +511,15 @@
 
     select_list = []
     if select_name:
         select_list = [ce for ce in ce_list_dict if match_name(ce, select_name) ]
 
     if select_host:
         if select_list: ce_list_dict = select_list[:]
-        select_list = [ce for ce in ce_list_dict if match_name(ce, select_host) ]
+        select_list = [ce for ce in ce_list_dict if match_host(ce, select_host) ]
 
     if select_part:
         if select_list: ce_list_dict = select_list[:]
         select_list = [ce for ce in ce_list_dict if match_part(ce, select_part) ]
 
     if not select_list:
         return RET(0, 'Empty selection results')
@@ -593,15 +570,15 @@
     if show_only_running: select_status = 'RUNNING'
 
     def match_status(job: Union[dict, None] = None, status: str = '') -> bool:
         if job is None or not status: return False
         return status.casefold() in job['status'].casefold()
 
     def match_user(job: Union[dict, None] = None, user: str = '') -> bool:
-        if job is None or not status: return False
+        if job is None or not user: return False
         return user.casefold() in job['owner'].casefold()
 
     select_list = []
     if select_status:
         select_list = [job for job in jobs_list_dict if match_status(job, select_status) ]
 
     if select_user:
@@ -660,73 +637,14 @@
             trace_info = f'Trace info:\n{f"{os.linesep}".join(new_j["trace"]["trace"])}\n\n'
             proc_info = f'Proc info:\n{f"{os.linesep}".join(new_j["trace"]["proc"])}\n\n'
             job_list_messages.append(f'{job_info}{machine_info}{state_info}{trace_info if show_trace else ""}{proc_info if show_proc else ""}')
 
     return RET(0, f'{os.linesep}'.join(job_list_messages), '', job_processed_list)
 
 
-def queryML(args: list = None) -> RET:
-    """submit: process submit commands for local jdl cases"""
-    alimon = 'http://alimonitor.cern.ch/rest/'
-    type_json = '?Accept=application/json'
-    type_xml = '?Accept=text/xml'
-    type_plain = '?Accept=text/plain'
-    type_default = ''
-    predicate = ''
-
-    if 'text' in args:
-        type_default = type_plain
-        args.remove('text')
-    if 'xml' in args:
-        type_default = type_xml
-        args.remove('xml')
-    if 'json' in args:
-        type_default = type_json
-        args.remove('json')
-
-    if args: predicate = args[0]
-    url = f'{alimon}{predicate}{type_default}'
-    exitcode = stdout = stderr = ansdict = ansraw = None
-
-    url_req = urlreq.Request(url)
-    with urlreq.urlopen(url_req) as req:  # nosec
-        ansraw = req.read().decode()
-        exitcode = 0 if (req.getcode() == 200) else req.getcode()
-
-    if type_default == type_json:
-        stdout = stderr = ''
-        ansdict = json.loads(ansraw)
-    else:
-        stdout, stderr = (ansraw, '') if exitcode == 0 else ('', ansraw)
-    return RET(exitcode, stdout, stderr, ansdict)
-
-
-def ccdb_json_cleanup(item_dict: dict) -> None:
-    item_dict.pop('createTime', None)
-    item_dict.pop('lastModified', None)
-    item_dict.pop('id', None)  # replaced by ETag
-    item_dict.pop('validFrom', None)
-    item_dict.pop('validUntil', None)
-    item_dict.pop('initialValidity', None)  # replaced by InitialValidityLimit
-    item_dict.pop('MD5', None)  # replaced by Content-MD5
-    item_dict.pop('fileName', None)  # replaced by Content-Disposition
-    content_disposition = item_dict.pop('Content-Disposition')
-    filename = content_disposition.replace('inline;filename=', '').replace('"', '')
-    item_dict['filename'] = filename
-
-    item_dict.pop('contentType', None)
-    item_dict.pop('size', None)  # replaced by Content-Length
-    item_dict.pop('Created', None)  #  no need (??) to be shown (mail2dev if needed)
-    item_dict.pop('Content-Type', None)  #  useless for this application
-    item_dict.pop('UploadedFrom', None)  #  useless for this application
-    item_dict.pop('UploadedBy', None)  #  useless for this application
-    item_dict.pop('partName', None)  #  useless for this application
-    item_dict.pop('InitialValidityLimit', None)  #  unclear use for this field
-
-
 def DO_ccdb_query(args: list = None) -> RET:
     """Query CCDB for object data"""
     if not args: return RET(2, '', 'empty query! Use at least a "/" as argument')
 
     if is_help(args):
         return RET(0, '''ccdb [-host FQDN] [-history] [-nicetime] QUERY
 where query has the form of:
@@ -737,21 +655,20 @@
 -host: specify other ccdb server than alice-ccdb.cern.ch
 -history: use browse to list the whole history of the object
 -unixtime: print the unixtime
 -get: download the specified object/objects - full path will be kept
 -dst: set a specific destination for download
 ''' )
 
-    headers = { 'user-agent': f'alien.py/{ALIENPY_VERSION_STR}', 'Accept': 'application/json', 'Accept-encoding': 'gzip, deflate', }  
+    headers = { 'user-agent': f'alien.py/{ALIENPY_VERSION_STR}', 'Accept': 'application/json', 'Accept-encoding': 'gzip, deflate', }
 
     listing_type = 'browse/' if get_arg(args, '-history') else 'latest/'
     ccdb_default_host = 'http://alice-ccdb.cern.ch/'
     host_arg = get_arg_value(args, '-host')
     do_unixtime = get_arg(args, '-unixtime')
-    do_compact = get_arg(args, '-compact')
     do_download = get_arg(args, '-get')
 
     dest_arg = get_arg_value(args, '-dst')
     if not dest_arg: dest_arg = '.'
     if not dest_arg.endswith('/'): dest_arg = f'{dest_arg}/'
 
     ccdb = host_arg if host_arg else ccdb_default_host
@@ -759,33 +676,31 @@
     if not ccdb.startswith('http://') and not ccdb.startswith('https://'): ccdb = f'http://{ccdb}'
 
     if not args: return RET(2, '', 'empty query!')
     query_str = args[0]  # after removal of args assume the rest is the query
 
     q = requests.get(f'{ccdb}{listing_type}{query_str}', headers = headers, timeout = 5)
     q_dict = q.json()
-    q_path = q_dict.pop('path')
-    q_latest = q_dict.pop('latest')
-    q_patternMatching = q_dict.pop('patternMatching')
+    # q_path = q_dict.pop('path')
+    # q_latest = q_dict.pop('latest')
+    # q_patternMatching = q_dict.pop('patternMatching')
     list(map(ccdb_json_cleanup, q_dict['objects']))
 
     if not do_unixtime:
         if 'validAt' in q_dict: q_dict['validAt'] = unixtime2local(q_dict['validAt'])
         for i in q_dict['objects']:
             i['Last-Modified'] = unixtime2local(i['Last-Modified'])
             i['Valid-From'] = unixtime2local(i['Valid-From'])
             i['Valid-Until'] = unixtime2local(i['Valid-Until'])
 
     dir_list = [f'{d}/' for d in q_dict['subfolders']]
     msg_dirs = f'{os.linesep}'.join(dir_list) if dir_list else ''
 
-    from rich import print
-
     def get_alien_endpoint(obj):
-        if not 'replicas' in obj: return ''
+        if 'replicas' not in obj: return ''
         for i in obj['replicas']:
             if i.startswith('alien'): return i
 
     header = f'Filename{" "*39}Type{" "*24}LastMod{" "*27}Valid'
     download_list = []
     dest_list = []
     msg_obj_list = []
@@ -800,39 +715,14 @@
     msg_obj = f'{os.linesep}'.join(msg_obj_list)
     if msg_obj: msg_obj = f'{header}\n{msg_obj}'
     msg = f'{msg_dirs}\n{msg_obj}'
 
     return RET(0, msg, '', q_dict)
 
 
-def file2xml_el(filepath: str) -> ALIEN_COLLECTION_EL:
-    """Get a file and return an XML element structure"""
-    if not filepath or not os.path.isfile(filepath): return ALIEN_COLLECTION_EL()
-    p = Path(filepath).expanduser().resolve(strict = True)
-    if p.is_dir(): return ALIEN_COLLECTION_EL()
-    p_stat = p.stat()
-    turl = f'file://{p.as_posix()}'
-    return ALIEN_COLLECTION_EL(
-        name = p.name, aclId = "", broken = "0", ctime = time_unix2simple(p_stat.st_ctime),
-        dir = '', entryId = '', expiretime = '', gowner = p.group(), guid = '', guidtime = '', jobid = '', lfn = turl,
-        md5 = md5(p.as_posix()), owner = p.owner(), perm = str(oct(p_stat.st_mode))[5:], replicated = "0",
-        size = str(p_stat.st_size), turl = turl, type = 'f')
-
-
-def mk_xml_local(filepath_list: list):
-    xml_root = ET.Element('alien')
-    collection = ET.SubElement(xml_root, 'collection', attrib={'name': 'tempCollection'})
-    for idx, item in enumerate(filepath_list, start = 1):
-        e = ET.SubElement(collection, 'event', attrib={'name': str(idx)})
-        ET.SubElement(e, 'file', attrib = file2xml_el(lfn_prefix_re.sub('', item))._asdict())
-    oxml = ET.tostring(xml_root, encoding = 'ascii')
-    dom = MD.parseString(oxml)  # nosec B318:blacklist
-    return dom.toprettyxml()
-
-
 def DO_2xml(wb, args: Union[list, None] = None) -> RET:
     if args is None: args = []
     if not args or is_help(args):
         central_help = SendMsg(wb, 'toXml', ['-h'], opts = 'nokeys')
         central_help_msg = central_help.out
         msg_local = ('\nAdditionally the client implements these options:'
                      '\n-local: specify that the target lfns are local files'
@@ -969,15 +859,15 @@
         value_list = [row.get(key) for key in keys]
         msg = f'{msg}\n{row_format.format(*value_list)}'
     return RET(0, msg, '', q_dict)
 
 
 def DO_submit(wb, args: Union[list, None] = None) -> RET:
     """submit: process submit commands for local jdl cases"""
-    if not args or args is None: args = ['-h']
+    if not args: args = ['-h']
     if is_help(args): return get_help_srv(wb, 'submit')
     if args[0].startswith("file:"):
         msg = ("Specifications as where to upload the jdl to be submitted and with what parameters are not yet defined"
                "Upload first the jdl to a suitable location (with a safe number of replicas) and then submit")
         return RET(0, msg)
     args[0] = expand_path_grid(args[0])
     return SendMsg(wb, 'submit', args)
@@ -991,28 +881,31 @@
         nice_lines = [convert_time(str(msgline)) for item in ret_obj.ansdict['results'] for msgline in item['message'].split('\n')]
         return ret_obj._replace(out = '\n'.join(nice_lines))
     return ret_obj
 
 
 def DO_cat(wb, args: Union[list, None] = None) -> RET:
     """cat lfn :: apply cat on a downloaded lfn as a temporary file"""
+    if not args: return RET(1, '', 'DO_cat:: empty args!!')
     args.insert(0, '-noout')  # keep app open, do not terminate
     args.insert(0, 'cat')
     return DO_run(wb, args, external = True)
 
 
 def DO_less(wb, args: Union[list, None] = None) -> RET:
     """less lfn :: apply less on a downloaded lfn as a temporary file"""
+    if not args: return RET(1, '', 'DO_less:: empty args!!')
     args.insert(0, '-noout')  # keep app open, do not terminate
     args.insert(0, 'less')
     return DO_run(wb, args, external = True)
 
 
 def DO_more(wb, args: Union[list, None] = None) -> RET:
     """more lfn :: apply more on a downloaded lfn as a temporary file"""
+    if not args: return RET(1, '', 'DO_more:: empty args!!')
     args.insert(0, '-noout')  # keep app open, do not terminate
     args.insert(0, 'more')
     return DO_run(wb, args, external = True)
 
 
 def DO_lfn2uri(wb, args: Union[list, None] = None) -> RET:
     if args is None: args = []
@@ -1049,81 +942,14 @@
     else:
         out = lfn2uri(wb, lfn, local_file, specs, isWrite, strictspec, httpurl)
     if not out:
         return RET(1, '', f'Could not not create URIs for: {lfn}')
     return RET(0, out)
 
 
-def token(wb, args: Union[None, list] = None) -> int:
-    """(Re)create the tokencert and tokenkey files"""
-    global AlienSessionInfo
-    if not wb: return 1
-    if not args: args = []
-
-    ret_obj = SendMsg(wb, 'token', args, opts = 'nomsg')
-    if ret_obj.exitcode != 0:
-        logging.error('Token request returned error')
-        return retf_print(ret_obj, 'err')
-    tokencert_content = ret_obj.ansdict.get('results')[0].get('tokencert', '')
-    tokenkey_content = ret_obj.ansdict.get('results')[0].get('tokenkey', '')
-    if not tokencert_content or not tokenkey_content:
-        logging.error('Token request valid but empty fields!!')
-        return int(42)  # ENOMSG
-
-    try:
-        if path_readable(TOKENCERT_NAME):
-            os.chmod(TOKENCERT_NAME, 0o600)  # make it writeable
-            os.remove(TOKENCERT_NAME)
-        with open(TOKENCERT_NAME, "w", encoding = "ascii", errors = "replace") as tcert: print(f"{tokencert_content}", file = tcert)  # write the tokencert
-        os.chmod(TOKENCERT_NAME, 0o400)  # make it readonly
-    except Exception:
-        print_err(f'Error writing to file the aquired token cert; check the log file {DEBUG_FILE}!')
-        logging.debug(traceback.format_exc())
-        return 5  # EIO
-
-    try:
-        if path_readable(TOKENKEY_NAME):
-            os.chmod(TOKENKEY_NAME, 0o600)  # make it writeable
-            os.remove(TOKENKEY_NAME)
-        with open(TOKENKEY_NAME, "w", encoding = "ascii", errors = "replace") as tkey: print(f"{tokenkey_content}", file = tkey)  # write the tokenkey
-        os.chmod(TOKENKEY_NAME, 0o400)  # make it readonly
-    except Exception:
-        print_err(f'Error writing to file the aquired token key; check the log file {DEBUG_FILE}!')
-        logging.debug(traceback.format_exc())
-        return 5  # EIO
-
-    return int(0)
-
-
-def token_regen(wb, args: Union[None, list] = None):
-    global AlienSessionInfo
-    wb_usercert = None
-    if not args: args = []
-    if not AlienSessionInfo['use_usercert']:
-        wb_close(wb, code = 1000, reason = 'Lets connect with usercert to be able to generate token')
-        try:
-            wb_usercert = InitConnection(wb, args, use_usercert = True)  # we have to reconnect with the new token
-        except Exception:
-            logging.debug(traceback.format_exc())
-            return None  # we failed usercert connection
-
-    # now we are connected with usercert, so we can generate token
-    if token(wb_usercert, args) != 0: return wb_usercert
-    # we have to reconnect with the new token
-    wb_close(wb_usercert, code = 1000, reason = 'Re-initialize the connection with the new token')
-    AlienSessionInfo['use_usercert'] = False
-    wb_token_new = None
-    try:
-        wb_token_new = InitConnection(wb_token_new, args)
-        __ = SendMsg(wb_token_new, 'pwd', [], opts = 'nokeys')  # just to refresh cwd
-    except Exception:
-        logging.exception('token_regen:: error re-initializing connection')
-    return wb_token_new
-
-
 def DO_token(wb, args: Union[list, None] = None) -> RET:
     if args is None: args = []
     msg = "Print only command!!! Use >token-init< for token (re)generation, see below the arguments\n"
     ret_obj = SendMsg(wb, 'token', args, opts = 'nokeys')
     return ret_obj._replace(out = f'{msg}{ret_obj.out}')
 
 
@@ -1134,15 +960,15 @@
         return ret_obj._replace(out = ret_obj.out.replace('usage: token', 'INFO: token is automatically created, use this for token customization\nusage: token-init'))
     wb = token_regen(wb, args)
     return CertInfo(TOKENCERT_NAME)
 
 
 def DO_edit(wb, args: Union[list, None] = None, editor: str = '') -> RET:
     """Edit a grid lfn; download a temporary, edit with the specified editor and upload the new file"""
-    if not args or args is None: args = ['-h']
+    if not args: args = ['-h']
     if is_help(args):
         msg = """Command format: edit lfn\nAfter editor termination the file will be uploaded if md5 differs
 -datebck : the backup filename will be date based
 N.B. EDITOR env var must be set or fallback will be mcedit (not checking if exists)"""
         return RET(0, msg)
     if not editor:
         editor = os.getenv('EDITOR')
@@ -1255,14 +1081,23 @@
     if isinstance(args, str): args = args.split()
     if not cmd: return RET(1, '', 'No system command specified!')
     new_arg_list = [download_tmp(wb, arg) if arg.startswith('alien:') else arg for arg in args]
     new_arg_list.index(0, cmd)
     return runShellCMD(' '.join(new_arg_list), captureout = True, do_shell = True)
 
 
+def DO_gethome(wb, args: Union[None, list, str] = None) -> RET:
+    if args is None: args = []
+    if isinstance(args, str):
+        args = args.split() if args else []
+    if is_help(args):
+        return RET(0, 'Return user home')
+    return RET(0, AlienSessionInfo['alienHome'])
+
+
 def DO_find2(wb, args: Union[None, list, str] = None) -> RET:
     if args is None: args = []
     if isinstance(args, str):
         args = args.split() if args else []
     if is_help(args):
         msg_client = (f'''Client-side implementation of find, it contain the following helpers.
 Command formant: find2 <options> <directory>
@@ -1362,50 +1197,59 @@
             return RET(0, msg)
 
     jquota_out = SendMsg(wb, f'jquota -nomsg list {user}')
     jquota_dict = jquota_out.ansdict
     fquota_out = SendMsg(wb, f'fquota -nomsg list {user}')
     fquota_dict = fquota_out.ansdict
 
-    username = jquota_dict['results'][0]["username"]
+    if 'results' not in jquota_dict or 'results' not in fquota_dict or not jquota_dict['results'] or not fquota_dict['results']:
+        msg = f'jquota exitcode: {jquota_dict["metadata"]["exitcode"]}\n{jquota_dict["metadata"]["error"]}\nfquota exitcode: {fquota_dict["metadata"]["exitcode"]}\n{fquota_dict["metadata"]["error"]}'
+        return RET(1, '', f'Something went wrong with the command arguments and got empty results\n{msg}')
+
+    # It is possible to do this for multiple users, but no use-case for this
+    jquota_info = jquota_dict['results'][0]
+    fquota_info = fquota_dict['results'][0]
+    quota_sum = [{**j, **q} for j,q in zip(jquota_dict['results'], fquota_dict['results'])]
+
+    username = jquota_info["username"]
 
-    running_time = float(jquota_dict['results'][0]["totalRunningTimeLast24h"]) / 3600
-    running_time_max = float(jquota_dict['results'][0]["maxTotalRunningTime"]) / 3600
+    running_time = float(jquota_info["totalRunningTimeLast24h"]) / 3600
+    running_time_max = float(jquota_info["maxTotalRunningTime"]) / 3600
     running_time_perc = (running_time / running_time_max) * 100
 
-    cpucost = float(jquota_dict['results'][0]["totalCpuCostLast24h"]) / 3600
-    cpucost_max = float(jquota_dict['results'][0]["maxTotalCpuCost"]) / 3600
+    cpucost = float(jquota_info["totalCpuCostLast24h"]) / 3600
+    cpucost_max = float(jquota_info["maxTotalCpuCost"]) / 3600
     cpucost_perc = (cpucost / cpucost_max) * 100
 
-    unfinishedjobs_max = int(jquota_dict['results'][0]["maxUnfinishedJobs"])
-    waiting = int(jquota_dict['results'][0]["waiting"])
-    running = int(jquota_dict['results'][0]["running"])
+    unfinishedjobs_max = int(jquota_info["maxUnfinishedJobs"])
+    waiting = int(jquota_info["waiting"])
+    running = int(jquota_info["running"])
     unfinishedjobs_perc = ((waiting + running) / unfinishedjobs_max) * 100
 
-    pjobs_nominal = int(jquota_dict['results'][0]["nominalparallelJobs"])
-    pjobs_max = int(jquota_dict['results'][0]["maxparallelJobs"])
+    pjobs_nominal = int(jquota_info["nominalparallelJobs"])
+    pjobs_max = int(jquota_info["maxparallelJobs"])
 
-    size = float(fquota_dict['results'][0]["totalSize"])
+    size = float(fquota_info["totalSize"])
     size_MiB = size / (1024 * 1024)
-    size_max = float(fquota_dict['results'][0]["maxTotalSize"])
+    size_max = float(fquota_info["maxTotalSize"])
     size_max_MiB = size_max / (1024 * 1024)
     size_perc = (size / size_max) * 100
 
-    files = float(fquota_dict['results'][0]["nbFiles"])
-    files_max = float(fquota_dict['results'][0]["maxNbFiles"])
+    files = float(fquota_info["nbFiles"])
+    files_max = float(fquota_info["maxNbFiles"])
     files_perc = (files / files_max) * 100
 
     msg = (f"""Quota report for user : {username}
 Unfinished jobs(R + W / Max):\t\t{running} + {waiting} / {unfinishedjobs_max} --> {unfinishedjobs_perc:.2f}% used
 Running time (last 24h) used/max:\t{running_time:.2f}/{running_time_max:.2f}(h) --> {running_time_perc:.2f}% used
 CPU Cost (last 24h) used/max:\t\t{cpucost:.2f}/{cpucost_max:.2f}(h) --> {cpucost_perc:.2f}% used
 ParallelJobs (nominal/max) :\t{pjobs_nominal}/{pjobs_max}
 Storage size :\t\t\t{size_MiB:.2f}/{size_max_MiB:.2f} MiB --> {size_perc:.2f}%
 Number of files :\t\t{files}/{files_max} --> {files_perc:.2f}%""")
-    return RET(0, msg)
+    return RET(0, msg, '', quota_sum)
 
 
 def DO_checkAddr(args: Union[list, None] = None) -> RET:
     global AlienSessionInfo
     if is_help(args):
         msg = ('checkAddr [reference] fqdn/ip port\n'
                'defaults are: alice-jcentral.cern.ch 8097\n'
@@ -1472,54 +1316,14 @@
         return RET(0, msg)
 
     if 'date' in args: AlienSessionInfo['show_date'] = (not AlienSessionInfo['show_date'])
     if 'pwd' in args: AlienSessionInfo['show_lpwd'] = (not AlienSessionInfo['show_lpwd'])
     return RET(0)
 
 
-def get_list_entries(wb, lfn, fullpath: bool = False) -> list:
-    """return a list of entries of the lfn argument, full paths if 2nd arg is True"""
-    key = 'path' if fullpath else 'name'
-    ret_obj = SendMsg(wb, 'ls', ['-nomsg', '-a', '-F', os.path.normpath(lfn)])
-    if ret_obj.exitcode != 0: return []
-    return [item[key] for item in ret_obj.ansdict['results']]
-
-
-def lfn_list(wb, lfn: str = ''):
-    """Completer function : for a given lfn return all options for latest leaf"""
-    if not wb: return []
-    if not lfn: lfn = '.'  # AlienSessionInfo['currentdir']
-    list_lfns = []
-    lfn_path = Path(lfn)
-    base_dir = '/' if lfn_path.parent.as_posix() == '/' else f'{lfn_path.parent.as_posix()}/'
-    name = f'{lfn_path.name}/' if lfn.endswith('/') else lfn_path.name
-
-    def item_format(base_dir, name, item):
-        # print_out(f'\nbase_dir: {base_dir} ; name: {name} ; item: {item}')
-        if name.endswith('/') and name != '/':
-            return f'{name}{item}' if base_dir == './' else f'{base_dir}{name}{item}'
-        return item if base_dir == './' else f'{base_dir}{item}'
-
-    if lfn.endswith('/'):
-        listing = get_list_entries(wb, lfn)
-        list_lfns = [item_format(base_dir, name, item) for item in listing]
-    else:
-        listing = get_list_entries(wb, base_dir)
-        list_lfns = [item_format(base_dir, name, item) for item in listing if item.startswith(name)]
-    return list_lfns
-
-
-def wb_ping(wb) -> float:
-    """Websocket ping function, it will return rtt in ms"""
-    init_begin = time.perf_counter()
-    if IsWbConnected(wb):
-        return float(deltat_ms_perf(init_begin))
-    return float(-1)
-
-
 def DO_ping(wb, args: Union[list, None] = None) -> RET:
     """Command implementation for ping functionality"""
     if args is None: args = []
     if is_help(args): return RET(0, "ping <count>\nwhere count is integer")
 
     if len(args) > 0 and args[0].isdigit():
         count = int(args[0])
@@ -1541,88 +1345,71 @@
     msg = (f'Websocket ping/pong(s) : {count} time(s) to {endpoint}\nrtt min/avg/max/mdev (ms) = {rtt_min:.3f}/{rtt_avg:.3f}/{rtt_max:.3f}/{rtt_stddev:.3f}')
     return RET(0, msg)
 
 
 def DO_tokendestroy(args: Union[list, None] = None) -> RET:
     if args is None: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Delete the token{cert,key}.pem files")
-    if os.path.exists(TOKENCERT_VALID): os.remove(TOKENCERT_VALID)
-    if os.path.exists(TOKENKEY_VALID): os.remove(TOKENKEY_VALID)
+    if os.path.exists(AlienSessionInfo['token_cert']): os.remove(AlienSessionInfo['token_cert'])
+    if os.path.exists(AlienSessionInfo['token_key']): os.remove(AlienSessionInfo['token_key'])
     return RET(0, "Token was destroyed! Re-connect for token re-creation.")
 
 
 def DO_certinfo(args: Union[list, None] = None) -> RET:
     if args is None: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Print user certificate information", "")
-    return CertInfo(USERCERT_VALID)
+    return CertInfo(AlienSessionInfo['user_cert'])
 
 
 def DO_tokeninfo(args: Union[list, None] = None) -> RET:
     if not args: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Print token certificate information", "")
-    return CertInfo(TOKENCERT_VALID)
+    return CertInfo(AlienSessionInfo['token_cert'])
 
 
 def DO_certverify(args: Union[list, None] = None) -> RET:
     if args is None: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Verify the user cert against the found CA stores (file or directory)", "")
-    return CertVerify(USERCERT_VALID)
+    return CertVerify(AlienSessionInfo['user_cert'])
 
 
 def DO_tokenverify(args: Union[list, None] = None) -> RET:
     if not args: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Print token certificate information", "")
-    return CertVerify(TOKENCERT_VALID)
+    return CertVerify(AlienSessionInfo['token_cert'])
 
 
 def DO_certkeymatch(args: Union[list, None] = None) -> RET:
     if args is None: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Check match of user cert with key cert", "")
-    return CertKeyMatch(USERCERT_VALID, USERKEY_VALID)
+    return CertKeyMatch(AlienSessionInfo['user_cert'], AlienSessionInfo['user_key'])
 
 
 def DO_tokenkeymatch(args: Union[list, None] = None) -> RET:
     if args is None: args = []
     if len(args) > 0 and is_help(args): return RET(0, "Check match of user token with key token", "")
-    return CertKeyMatch(TOKENCERT_VALID, TOKENKEY_VALID)
-
-
-def make_func_map_clean_server():
-    """Remove from server list the client-side re-implementations"""
-    global AlienSessionInfo
-    del AlienSessionInfo['cmd2func_map_srv']['cd']
-    list_remove_item(AlienSessionInfo['commandlist'], 'cd')
-
-    del AlienSessionInfo['cmd2func_map_srv']['cp']
-    list_remove_item(AlienSessionInfo['commandlist'], 'cp')
+    return CertKeyMatch(AlienSessionInfo['token_cert'], AlienSessionInfo['token_key'])
 
-    del AlienSessionInfo['cmd2func_map_srv']['ping']
-    list_remove_item(AlienSessionInfo['commandlist'], 'ping')
-
-    del AlienSessionInfo['cmd2func_map_srv']['ps']
-    list_remove_item(AlienSessionInfo['commandlist'], 'ps')
-
-    del AlienSessionInfo['cmd2func_map_srv']['submit']
-    list_remove_item(AlienSessionInfo['commandlist'], 'submit')
-
-    del AlienSessionInfo['cmd2func_map_srv']['token']
-    list_remove_item(AlienSessionInfo['commandlist'], 'token')
-
-    del AlienSessionInfo['cmd2func_map_srv']['user']
-    list_remove_item(AlienSessionInfo['commandlist'], 'user')
 
-    del AlienSessionInfo['cmd2func_map_srv']['cat']
-    list_remove_item(AlienSessionInfo['commandlist'], 'cat')
-
-    del AlienSessionInfo['cmd2func_map_srv']['toXml']
-    list_remove_item(AlienSessionInfo['commandlist'], 'toXml')
+def DO_getCAcerts(args: Union[list, None] = None) -> RET:
+    if args is None: args = []
+    if len(args) > 0 and is_help(args): return RET(0, """Download CA certificates from ALICE alien-cas repository in ~/.globus/certificates
+-h/-help : this help information
+1st argument string will be taken as destination for certificates directory
+to use them preferentially do:
+export X509_CERT_DIR=$HOME/.globus/certificates
+or just
+export ALIENPY_USE_LOCAL_CAS=1""", "")
+    dest_dir = args[0] if len(args) > 0 else ''
+    return getCAcerts(dest_dir)
 
 
 def make_func_map_nowb():
     """client side functions (new commands) that do not require connection to jcentral"""
+    if 'AlienSessionInfo' not in globals(): return
     if AlienSessionInfo['cmd2func_map_nowb']: return
     AlienSessionInfo['cmd2func_map_nowb']['prompt'] = DO_prompt
     AlienSessionInfo['cmd2func_map_nowb']['token-info'] = DO_tokeninfo
     AlienSessionInfo['cmd2func_map_nowb']['token-verify'] = DO_tokenverify
     AlienSessionInfo['cmd2func_map_nowb']['token-destroy'] = DO_tokendestroy
     AlienSessionInfo['cmd2func_map_nowb']['cert-info'] = DO_certinfo
     AlienSessionInfo['cmd2func_map_nowb']['cert-verify'] = DO_certverify
@@ -1633,18 +1420,20 @@
     AlienSessionInfo['cmd2func_map_nowb']['version'] = DO_version
     AlienSessionInfo['cmd2func_map_nowb']['queryML'] = DO_queryML
     AlienSessionInfo['cmd2func_map_nowb']['exit'] = DO_exit
     AlienSessionInfo['cmd2func_map_nowb']['quit'] = DO_exit
     AlienSessionInfo['cmd2func_map_nowb']['logout'] = DO_exit
     AlienSessionInfo['cmd2func_map_nowb']['checkAddr'] = DO_checkAddr
     AlienSessionInfo['cmd2func_map_nowb']['ccdb'] = DO_ccdb_query
+    AlienSessionInfo['cmd2func_map_nowb']['getCAcerts'] = DO_getCAcerts
 
 
 def make_func_map_client():
     """client side functions (new commands) that DO require connection to jcentral"""
+    if 'AlienSessionInfo' not in globals(): return
     if AlienSessionInfo['cmd2func_map_client']: return
 
     # client side function (overrides) with signature : (wb, args, opts)
     AlienSessionInfo['cmd2func_map_client']['cd'] = cd
     AlienSessionInfo['cmd2func_map_client']['cp'] = DO_XrootdCp
     AlienSessionInfo['cmd2func_map_client']['ping'] = DO_ping
     AlienSessionInfo['cmd2func_map_client']['ps'] = DO_ps
@@ -1679,242 +1468,199 @@
     AlienSessionInfo['cmd2func_map_client']['nano'] = DO_nano
     AlienSessionInfo['cmd2func_map_client']['vi'] = DO_vi
     AlienSessionInfo['cmd2func_map_client']['vim'] = DO_vim
     AlienSessionInfo['cmd2func_map_client']['SEqos'] = DO_SEqos
     AlienSessionInfo['cmd2func_map_client']['less'] = DO_less
     AlienSessionInfo['cmd2func_map_client']['more'] = DO_more
     AlienSessionInfo['cmd2func_map_client']['lfn2uri'] = DO_lfn2uri
+    AlienSessionInfo['cmd2func_map_client']['home'] = DO_gethome
 
 
-def getSessionVars(wb):
-    """Initialize the global session variables : cleaned up command list, user, home dir, current dir"""
-    global AlienSessionInfo
-    if AlienSessionInfo['user']: return  # user session variable is already set, then return
-    if not wb: return
-    # get the command list just once per session connection (a reconnection will skip this)
-    ret_obj = SendMsg(wb, 'commandlist', [])
-    # first executed commands, let's initialize the following (will be re-read at each ProcessReceivedMessage)
-    if not ret_obj.ansdict or 'results' not in ret_obj.ansdict:
-        print_err("Start session:: could not get command list, let's exit.")
-        sys.exit(1)
-    csd_cmds_re = re.compile(r'.*_csd$')
-    AlienSessionInfo['commandlist'] = [cmd["commandlist"] for cmd in ret_obj.ansdict["results"] if not csd_cmds_re.match(cmd["commandlist"])]
+def constructCmdList():
+    """Construct the command to function mappings and the command list"""
+    if 'AlienSessionInfo' not in globals(): return
+    if AlienSessionInfo['cmd2func_map_client']: return
+
+    # remove client side re-implementations of server commands
+    list_remove_item(AlienSessionInfo['commandlist'], 'cat')
+    list_remove_item(AlienSessionInfo['commandlist'], 'cd')
+    list_remove_item(AlienSessionInfo['commandlist'], 'cp')
+    list_remove_item(AlienSessionInfo['commandlist'], 'ping')
+    list_remove_item(AlienSessionInfo['commandlist'], 'ps')
+    list_remove_item(AlienSessionInfo['commandlist'], 'submit')
+    list_remove_item(AlienSessionInfo['commandlist'], 'token')
+    list_remove_item(AlienSessionInfo['commandlist'], 'toXml')
+    list_remove_item(AlienSessionInfo['commandlist'], 'user')
 
     # server commands, signature is : (wb, command, args, opts)
     for cmd in AlienSessionInfo['commandlist']: AlienSessionInfo['cmd2func_map_srv'][cmd] = SendMsg
-    make_func_map_clean_server()
 
-    make_func_map_nowb()  # GLOBAL!! add to the list of client-side no-connection implementations
-    make_func_map_client()  # GLOBAL!! add to cmd2func_map_client the list of client-side implementations
+    # add command to function mappins for client-side command implementations
+    make_func_map_client()
 
     # these are aliases, or directly interpreted
     AlienSessionInfo['commandlist'].extend(['ll', 'la', 'lla'])
     AlienSessionInfo['commandlist'].extend(AlienSessionInfo['cmd2func_map_client'])  # add clien-side cmds to list
     AlienSessionInfo['commandlist'].extend(AlienSessionInfo['cmd2func_map_nowb'])    # add nowb cmds to list
     AlienSessionInfo['commandlist'] = sorted(set(AlienSessionInfo['commandlist']))
 
 
-def InitConnection(wb = None, token_args: Union[None, list] = None, use_usercert: bool = False, localConnect: bool = False):
-    """Create a session to AliEn services, including session globals and token regeneration"""
-    global AlienSessionInfo, ALIENPY_GLOBAL_WB
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
-    wb = AlienConnect(wb, token_args, use_usercert, localConnect)
-    ALIENPY_GLOBAL_WB = wb
-
-    # NO MATTER WHAT BEFORE ENYTHING ELSE SESSION MUST BE INITIALIZED   !!!!!!!!!!!!!!!!
-    if not AlienSessionInfo['session_started']:  # this is beggining of session, let's get session vars ONLY ONCE
-        AlienSessionInfo['session_started'] = True
-        session_begin = time.perf_counter() if (TIME_CONNECT or DEBUG) else None
-        getSessionVars(wb)  # no matter if command or interactive mode, we need alienHome, currentdir, user and commandlist
-        if session_begin:
-            msg = f">>>   Time for session initialization: {deltat_us_perf(session_begin)} us"
-            if DEBUG: logging.debug(msg)
-            if TIME_CONNECT: print_out(msg)
-
-    # this is a reconnection, make sure on the server we are in the last known current directory
-    if AlienSessionInfo['currentdir']: cd(wb, AlienSessionInfo['currentdir'], 'log')
-
-    # if usercert connection always regenerate token if connected with usercert
-    if AlienSessionInfo['use_usercert'] and token(wb, token_args) != 0: print_err(f'The token could not be created! check the logfile {DEBUG_FILE}')
-    return wb
-
-
 def ProcessInput(wb, cmd: str, args: Union[list, None] = None, shellcmd: Union[str, None] = None) -> RET:
     """Process a command line within shell or from command line mode input"""
     global AlienSessionInfo
     if not cmd: return RET(1, '', 'ProcessInput:: Empty input')
+    if 'AlienSessionInfo' not in globals(): return RET(1, '', 'ProcessInput needs presence of global dict AlienSessionInfo')
     if args is None: args = []
-    ret_obj = None
+
+    if cmd not in AlienSessionInfo['commandlist'] and not os.getenv('ALIENPY_ALLOW_UNKNOWN_CMDS'):
+        similar_list = difflib.get_close_matches(cmd, AlienSessionInfo['commandlist'])
+        similar_cmds = None
+        if similar_list: similar_cmds = ' '.join(similar_list)
+        msg = f'WARNING! command >>> {cmd} <<< not in the list of known commands!'
+        if similar_cmds: msg = f'{msg}\nSimilar commands: {similar_cmds}'
+        return RET(1, '', msg)
+
+    opts = ''  # let's proccess special server args
+    if get_arg(args, '-nokeys') or get_arg(args, 'nokeys'): opts = f'{opts} nokeys'
+    if get_arg(args, '-nomsg') or get_arg(args, 'nomsg'): opts = f'{opts} nomsg'
+    if get_arg(args, '-showkeys') or get_arg(args, 'showkeys'): opts = f'{opts} showkeys'
+    if get_arg(args, '-showmsg') or get_arg(args, 'showmsg'): opts = f'{opts} showmsg'
+
+    # these commands do NOT need wb connection
+    if cmd in AlienSessionInfo['cmd2func_map_nowb']:
+        return AlienSessionInfo['cmd2func_map_nowb'][cmd](args)
 
     # implement a time command for measurement of sent/recv delay; for the commands above we do not use timing
-    time_begin = msg_timing = None
+    time_begin = None
     if cmd == 'time':  # first to be processed is the time token, it will start the timing and be removed from command
         if not args or is_help(args): return RET(0, 'Command format: time command arguments')
         cmd = args.pop(0)
         time_begin = time.perf_counter()
 
     # early command aliases and default flags
-    if cmd == 'ls': args[0:0] = ['-F']
-    if cmd == 'll':
-        cmd = 'ls'
-        args[0:0] = ['-F', '-l']
-    if cmd == 'la':
-        cmd = 'ls'
-        args[0:0] = ['-F', '-a']
-    if cmd == 'lla':
-        cmd = 'ls'
-        args[0:0] = ['-F', '-l', '-a']
-
-    if cmd in AlienSessionInfo['cmd2func_map_nowb']:  # these commands do NOT need wb connection
-        get_arg(args, '-nokeys')
-        get_arg(args, '-nomsg')
-        return AlienSessionInfo['cmd2func_map_nowb'][cmd](args)
-
-    opts = ''  # let's proccess special server args
-    if get_arg(args, '-nokeys'): opts = f'{opts} nokeys'
-    if get_arg(args, '-nomsg'): opts = f'{opts} nomsg'
-    if get_arg(args, '-showkeys'): opts = f'{opts} showkeys'
-    if get_arg(args, '-showmsg'): opts = f'{opts} showmsg'
+    if cmd == 'ls':
+        args[0:0] = ['-F']
+    elif cmd == 'll':
+        cmd = 'ls'; args[0:0] = ['-F', '-l']
+    elif cmd == 'la':
+        cmd = 'ls'; args[0:0] = ['-F', '-a']
+    elif cmd == 'lla':
+        cmd = 'ls'; args[0:0] = ['-F', '-l', '-a']
 
+    ret_obj = None
     # We will not check for websocket connection as: 1. there is keep alive mechanism 2. there is recovery in SendMsg
     if cmd in AlienSessionInfo['cmd2func_map_client']:  # lookup in clien-side implementations list
         ret_obj = AlienSessionInfo['cmd2func_map_client'][cmd](wb, args)
     elif cmd in AlienSessionInfo['cmd2func_map_srv']:  # lookup in server-side list
         ret_obj = AlienSessionInfo['cmd2func_map_srv'][cmd](wb, cmd, args, opts)
+    if ret_obj is None: return RET(1, '', 'ProcessInput:: there was no return object!! Invalid state, contact developer!')
 
-    if time_begin: msg_timing = f">>>ProcessInput time: {deltat_ms_perf(time_begin)} ms"
+    msg_timing = f'>>>ProcessInput time: {deltat_ms_perf(time_begin)} ms' if time_begin else ''
 
-    if cmd not in AlienSessionInfo['commandlist']:
-        similar_list = difflib.get_close_matches(cmd, AlienSessionInfo['commandlist'])
-        similar_cmds = None
-        if similar_list: similar_cmds = ' '.join(similar_list)
-        msg = f'WARNING! command >>> {cmd} <<< not in the list of known commands!'
-        if similar_cmds: msg = f'{msg}\nSimilar commands: {similar_cmds}'
-        print_err(msg)
-    if ret_obj is None: return RET(1, '', f"NO RETURN from command: {cmd} {chr(32).join(args)}")
+    # make the assumption that only valid output (exitcode == 0) have a reason to be processed by a shell command
+    if ret_obj.exitcode != 0: return ret_obj
 
-    if shellcmd:
-        if ret_obj.exitcode != 0: return ret_obj
-        if not ret_obj.out:
-            return RET(1, '', f'Command >>>{cmd} {chr(32).join(args)}<<< do not have output but exitcode == 0')
-        print_out(ret_obj.out)
+    # client side commands will not have metadata so neither 'timing_ms'
+    if 'metadata' in ret_obj.ansdict and 'timing_ms' in ret_obj.ansdict['metadata']:
+        ret_obj = ret_obj._replace(out = f"{ret_obj.out}\ntiming_ms = {ret_obj.ansdict['metadata']['timing_ms']}")
+
+    if shellcmd and ret_obj.out:
         shell_run = subprocess.run(shellcmd, stdout = subprocess.PIPE, stderr = subprocess.PIPE, input = f'{ret_obj.out}\n', encoding = 'ascii', shell = True)  # pylint: disable=subprocess-run-check # env=os.environ default is already the process env  # nosec
         if msg_timing: shell_run.stdout = f'{shell_run.stdout}\n{msg_timing}'
-        return RET(shell_run.returncode, shell_run.stdout, shell_run.stderr)
+        return RET(shell_run.returncode, shell_run.stdout, shell_run.stderr, ret_obj.ansdict)
 
     if msg_timing: ret_obj = ret_obj._replace(out = f'{ret_obj.out}\n{msg_timing}')
-    if ret_obj.ansdict and 'metadata' in ret_obj.ansdict and 'timing_ms' in ret_obj.ansdict['metadata']:
-        ret_obj = ret_obj._replace(out = f"{ret_obj.out}\ntiming_ms = {ret_obj.ansdict['metadata']['timing_ms']}")
     return ret_obj
 
 
 def ProcessCommandChain(wb = None, cmd_chain: str = '') -> int:
+    """Process a chain of commands delimited by ; or new line"""
     global AlienSessionInfo, ALIENPY_GLOBAL_WB
-    if not cmd_chain: return int(1)
-    JSON_OUT_GLOBAL = os.getenv('ALIENPY_JSON_OUT_GLOBAL')
+    if 'AlienSessionInfo' not in globals() or not cmd_chain:
+        print_err('ProcessCommandChain needs presence of global dict AlienSessionInfo and cmd_chain')
+        return 1
 
     # translate aliases in place in the whole string
     if AlienSessionInfo['alias_cache']:
         for alias, alias_value in AlienSessionInfo['alias_cache'].items(): cmd_chain = cmd_chain.replace(alias, alias_value)
 
-    cmdline_list = [str(cmd).strip() for cmd in cmds_split.split(cmd_chain)]  # split commands on ; and \n
-
     # for each command, save exitcode and RET of the command
+    exitcode = -1
+    cmdline_list = [str(cmd).strip() for cmd in cmds_split.split(cmd_chain)]  # split commands on ; and \n with regex
     for cmdline in cmdline_list:
         if not cmdline: continue
         if DEBUG: logging.info('>>> RUN COMMAND: %s', cmdline)
-        if cmdline.startswith('!'):  # if shell command, just run it and return
-            capture_out = True
-            if '-noout' in cmdline:
-                cmdline = cmdline.replace(' -noout', '')
-                capture_out = False
+
+        # if shell command, just run it and return
+        if cmdline.startswith('!'):
+            capture_out = '-noout' in cmdline
+            if not capture_out: cmdline.replace(' -noout', '')
             ret_obj = runShellCMD(cmdline, capture_out)
-            AlienSessionInfo['exitcode'] = retf_print(ret_obj, 'debug')
+            exitcode = retf_print(ret_obj, 'debug')
+            AlienSessionInfo['exitcode'] = exitcode
             continue
 
         # process the input and take care of pipe to shell
         input_alien, __, pipe_to_shell_cmd = cmdline.partition(' | ')
         if not input_alien:
-            print_out("AliEn command before the | token was not found")
+            logging.error(f'AliEn command before the | token was not found\n{cmdline}')
             continue
 
         args = shlex.split(input_alien.strip())
         cmd = args.pop(0)
 
         # if globally enabled then enable per command OR if enabled for this command
         JSON_OUT_CMD = None
         if get_arg(args, '-json'):
             os.environ['ALIENPY_JSON_OUT'] = '1'
             JSON_OUT_CMD = '1'
+        JSON_OUT_GLOBAL = os.getenv('ALIENPY_JSON_OUT_GLOBAL')
         JSON_OUT = JSON_OUT_GLOBAL or JSON_OUT_CMD
 
-        print_opts = 'debug'
+        print_opts = 'debug' if DEBUG else ''
         if JSON_OUT: print_opts = f'{print_opts} json'
 
+        ret_obj = None
         if cmd in AlienSessionInfo['cmd2func_map_nowb']:
             ret_obj = AlienSessionInfo['cmd2func_map_nowb'][cmd](args)
         else:
             if wb is None:
-                # we are doing the connection recovery and exception treatment in AlienConnect()
-                wb = InitConnection(wb, args, use_usercert = (cmd == 'token-init' and not is_help(args)))
+                # If not prezent init connection and if command is token-init (without help being invoked) then use usercert
+                wb = InitConnection(wb, args, use_usercert = (cmd == 'token-init' and not is_help(args)), cmdlist_func = constructCmdList)
                 ALIENPY_GLOBAL_WB = wb
             args.append('-nokeys')  # Disable return of the keys. ProcessCommandChain is used for user-based communication so json keys are not needed
             ret_obj = ProcessInput(wb, cmd, args, pipe_to_shell_cmd)
 
-        AlienSessionInfo['exitcode'] = retf_print(ret_obj, print_opts)  # save exitcode for easy retrieval
+        exitcode = retf_print(ret_obj, print_opts)  # save exitcode for easy retrieval
+        AlienSessionInfo['exitcode'] = exitcode
+
         if cmd == 'cd': SessionSave()
 
         # reset JSON_OUT if it's not globally enabled (env var or argument to alien.py)
         if not JSON_OUT_GLOBAL and 'ALIENPY_JSON_OUT' in os.environ: del os.environ['ALIENPY_JSON_OUT']
-        
-    return AlienSessionInfo['exitcode']
-
-
-def setupHistory() -> None:
-    """Setup up history mechanics for readline module"""
-    if not HAS_READLINE: return
-    histfile = os.path.join(os.path.expanduser("~"), ".alienpy_history")
-    if not os.path.exists(histfile): Path(histfile).touch(exist_ok = True)
-    rl.set_history_length(-1)  # unlimited history
-    rl.read_history_file(histfile)
-
-    def startup_hook() -> None: rl.append_history_file(1, histfile)  # before next prompt save last line
-    rl.set_startup_hook(startup_hook)
+    return exitcode
 
 
 def JAlien(commands: str = '') -> int:
     """Main entry-point for interaction with AliEn"""
     global AlienSessionInfo, ALIENPY_GLOBAL_WB
     import_aliases()
 
     # Command mode interaction
     if commands: return ProcessCommandChain(ALIENPY_GLOBAL_WB, commands)
 
     # Start interactive/shell mode
-    ALIENPY_GLOBAL_WB = InitConnection()  # we are doing the connection recovery and exception treatment in AlienConnect()
+    ALIENPY_GLOBAL_WB = InitConnection(cmdlist_func = constructCmdList)  # we are doing the connection recovery and exception treatment in AlienConnect()
     # Begin Shell-like interaction
-    if HAS_READLINE:
-        rl.parse_and_bind("tab: complete")
-        rl.set_completer_delims(" ")
-
-        def complete(text, state):
-            prompt_line = rl.get_line_buffer()
-            tokens = prompt_line.split()
-            results = []
-            if len(tokens) == 0:
-                results = [f'{x} ' for x in AlienSessionInfo['commandlist']]
-            elif len(tokens) == 1 and not prompt_line.endswith(' '):
-                results = [f'{x} ' for x in AlienSessionInfo['commandlist'] if x.startswith(text)] + [None]
-            else:
-                results = lfn_list(ALIENPY_GLOBAL_WB, text) + [None]
-            return results[state]
-        rl.set_completer(complete)
-        setupHistory()  # enable history saving
+
+    setupHistory(ALIENPY_GLOBAL_WB)  # Setup command history
 
     print_out('Welcome to the ALICE GRID\nsupport mail: adrian.sevcenco@cern.ch\n')
+    if DEBUG:
+        print_out(f'Debug enabled, logfile is: {DEBUG_FILE}')
     if os.getenv('ALIENPY_PROMPT_DATE'): AlienSessionInfo['show_date'] = True
     if os.getenv('ALIENPY_PROMPT_CWD'): AlienSessionInfo['show_lpwd'] = True
     if not os.getenv('ALIENPY_NO_CWD_RESTORE'): SessionRestore(ALIENPY_GLOBAL_WB)
 
     while True:
         INPUT = None
         prompt = f"AliEn[{AlienSessionInfo['user']}]:{AlienSessionInfo['currentdir']}"
@@ -1932,15 +1678,15 @@
 
 
 class AliEn:
     """Class to be used as advanced API for interaction with central servers"""
     __slots__ = ('internal_wb', 'opts')
 
     def __init__(self, opts = ''):
-        self.internal_wb = InitConnection()
+        self.internal_wb = InitConnection(cmdlist_func = constructCmdList)
         self.opts = opts
 
     def run(self, cmd, opts = '') -> Union[RET, str]:
         """SendMsg to server a string command, a RET object will be returned"""
         if not opts: opts = self.opts
         return SendMsg(self.internal_wb, cmd, opts = opts)
 
@@ -1962,14 +1708,18 @@
                   '.wb() : return the session WebSocket to be used with other function within alien.py')
 
 
 ###################################################
 ###   CODE TO BE RUN BEFORE MAIN STARTS
 ###################################################
 
+#####################
+make_func_map_nowb()  # GLOBAL!! add to the list of client-side no-connection implementations
+#####################
+
 
 ###################################################
 def main():
     global ALIENPY_EXECUTABLE, DEBUG, DEBUG_FILE
     signal.signal(signal.SIGINT, signal_handler)
     # signal.signal(sig, signal.SIG_DFL)  # register the default signal handler usage for a sig signal
     # at exit delete all temporary files
@@ -1987,15 +1737,14 @@
     if DEBUGFILE_ARG:
         os.environ['ALIENPY_DEBUG_FILE'] = DEBUGFILE_ARG
         DEBUG_FILE = DEBUGFILE_ARG
 
     # start the logging
     setup_logging(bool(DEBUG), DEBUG_FILE)
     if DEBUG:
-        print_out(f'Debug enabled, logfile is: {DEBUG_FILE}')
         ret_obj = DO_version()
         logging.debug('%s\n', ret_obj.out)
 
     arg_list_expanded = []
     for arg in sys.argv:
         for item in shlex.split(arg):
             arg_list_expanded.append(item)
@@ -2042,14 +1791,17 @@
 
 
 def _cmd(what):
     sys.argv = [sys.argv[0]] + [what] + sys.argv[1:]
     main()
 
 
+def cmd_home(): _cmd('home')
+
+
 def cmd_cert_info(): _cmd('cert-info')
 
 
 def cmd_token_info(): _cmd('token-info')
 
 
 def cmd_token_destroy(): _cmd('token-destroy')
```

### Comparing `alienpy-1.5.0/alienpy/async_tools.py` & `alienpy-1.5.1/alienpy/async_tools.py`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.0/alienpy/connect_ssl.py` & `alienpy-1.5.1/alienpy/connect_ssl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,91 @@
 '''alienpy:: SSL and certificate tooling'''
 
 import sys
 import os
 import logging
 import uuid
-from pathlib import Path
 import traceback
+import datetime
 
 try:
     import ssl
 except Exception:
     print("Python ssl module could not be imported! Make sure you can do:\npython3 -c 'import ssl'", file = sys.stderr, flush = True)
     sys.exit(1)
 
-try:
-    import cryptography
-except Exception:
-    print("cryptography module could not be imported! Make sure you can do:\npython3 -c 'import cryptography'", file = sys.stderr, flush = True)
-    sys.exit(1)
+import warnings
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    try:
+        import cryptography
+    except Exception:
+        print("cryptography module could not be imported! Make sure you can do:\npython3 -c 'import cryptography'", file = sys.stderr, flush = True)
+        sys.exit(1)
 
 try:
     import OpenSSL
 except Exception:
     print("OpenSSL module could not be loaded", file = sys.stderr, flush = True)
     sys.exit(1)
 
 ##   GLOBALS
 from .global_vars import *  # nosec PYL-W0614
-from .data_structs import *  # nosec PYL-W0614
-from .tools_misc import *  # nosec PYL-W0614
-from .tools_files import *  # nosec PYL-W0614
-
-# Have global variables for certificate file names, defaults being over-ridden by env vars
-USERCERT_NAME = os.getenv('X509_USER_CERT', f'{Path.home().as_posix()}/.globus/usercert.pem')
-USERKEY_NAME  = os.getenv('X509_USER_KEY',  f'{Path.home().as_posix()}/.globus/userkey.pem')
-
-TOKENCERT_NAME = os.getenv('JALIEN_TOKEN_CERT', f'{TMPDIR}/tokencert_{str(os.getuid())}.pem')
-TOKENKEY_NAME  = os.getenv('JALIEN_TOKEN_KEY',  f'{TMPDIR}/tokenkey_{str(os.getuid())}.pem')
+from .tools_nowb import PrintColor, path_readable
+from .setup_logging import print_err
 
 
 def get_ca_path() -> str:
-    """Return either the CA path or file; bailout application if not found"""
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
-
+    """Return either the CA path or file, priority given to X509_CERT_FILE and X509_CERT_DIR"""
     system_ca_path = '/etc/grid-security/certificates'
     alice_cvmfs_ca_path_lx = '/cvmfs/alice.cern.ch/etc/grid-security/certificates'
     alice_cvmfs_ca_path_macos = f'/Users/Shared{alice_cvmfs_ca_path_lx}'
+    local_ca_certs_dir = f'{USER_HOME}/.globus/certificates'
 
-    x509file = os.getenv('X509_CERT_FILE') if os.path.isfile(str(os.getenv('X509_CERT_FILE'))) else ''
-    if x509file:
-        if DEBUG: logging.debug('X509_CERT_FILE = %s', x509file)
-        return x509file
-
-    x509dir = os.getenv('X509_CERT_DIR') if os.path.isdir(str(os.getenv('X509_CERT_DIR'))) else ''
-    if x509dir:
-        if DEBUG: logging.debug('X509_CERT_DIR = %s', x509dir)
-        return x509dir
+    x509file = os.getenv('X509_CERT_FILE', default = '')
+    x509dir = os.getenv('X509_CERT_DIR', default = '')
 
+    use_local_cas_dir = os.getenv('ALIENPY_USE_LOCAL_CAS', default = '')
     capath_default = None
-    if os.path.exists(alice_cvmfs_ca_path_lx):
+    if use_local_cas_dir:
+        if os.path.isfile(f'{local_ca_certs_dir}/CERN-GridCA.pem'):
+            capath_default = local_ca_certs_dir
+            os.environ['X509_CERT_DIR'] = local_ca_certs_dir
+        else:
+            msg = 'usage of local CAs was requested by presence of ALIENPY_USE_LOCAL_CAS, but no certificates found there!!!\nrun: "alien.py getCAcerts" first'
+            print_err(msg)
+            logging.error(msg)
+            sys.exit(2)
+    elif x509file:
+        if os.path.isfile(x509file):
+            capath_default = x509file
+            if DEBUG: logging.debug('X509_CERT_FILE = %s', x509file)
+        else:
+            logging.error('X509_CERT_FILE set to %s but file is not accessible', x509file)
+    elif x509dir:
+        if os.path.isdir(x509dir):
+            capath_default = x509dir
+            if DEBUG: logging.debug('X509_CERT_DIR = %s', x509dir)
+        else:
+            logging.error('X509_CERT_DIR set to %s but directory is not accessible', x509dir)
+    elif os.path.exists(alice_cvmfs_ca_path_lx):
         capath_default = alice_cvmfs_ca_path_lx
     elif os.path.exists(alice_cvmfs_ca_path_macos):
         capath_default = alice_cvmfs_ca_path_macos
+    elif os.path.isfile(f'{local_ca_certs_dir}/CERN-GridCA.pem'):
+        capath_default = local_ca_certs_dir
+        os.environ['X509_CERT_DIR'] = local_ca_certs_dir
+    elif os.path.exists(system_ca_path):
+        capath_default = system_ca_path
     else:
-        if os.path.exists(system_ca_path): capath_default = system_ca_path
-
-    if not capath_default:
-        msg = "No CA location or files specified or found!!! Connection will not be possible!!"
+        msg = "No CA location or files specified or found!!! Connection will not be possible!! Run:\nalien.py getCAcerts\nto download CAs to local ~/.globus/certificates"
         print_err(msg)
         logging.error(msg)
         sys.exit(2)
-    if DEBUG: logging.debug('CApath = %s', capath_default)
+    if DEBUG: logging.debug('CApath/file = %s', capath_default)
     return capath_default
 
 
 def IsValidCert(fname: str) -> bool:
     """Check if the certificate file (argument) is present and valid. It will return false also for less than 5min of validity"""
     try:
         with open(fname, encoding="ascii", errors="replace") as f:
@@ -97,113 +108,123 @@
     if time_remaining < 1:
         logging.error('IsValidCert:: Expired certificate %s', fname)
     return time_remaining > 300
 
 
 def get_valid_certs() -> tuple:
     """Return valid names for user certificate or None"""
-    if AlienSessionInfo['verified_cert']: return USERCERT_NAME, USERKEY_NAME
+    if 'AlienSessionInfo' in globals() and AlienSessionInfo['verified_cert']: return AlienSessionInfo['user_cert'], AlienSessionInfo['user_key']
+
     FOUND = path_readable(USERCERT_NAME) and path_readable(USERKEY_NAME)
     if not FOUND:
-        msg = f'User certificate files NOT FOUND or NOT accessible!!! Connection will not be possible!!\nCheck content of {os.path.expanduser("~")}/.globus'
+        msg = f'User certificate files NOT FOUND or NOT accessible!!! Connection might be not be possible!!\nCheck content of {os.path.expanduser("~")}/.globus'
         logging.error(msg)
         return None, None
 
     INVALID = not IsValidCert(USERCERT_NAME)
     if INVALID:
         msg = f'Invalid/expired user certificate!! Check the content of {USERCERT_NAME}'
         logging.error(msg)
         return None, None
 
-    AlienSessionInfo['verified_cert'] = True  # This means that we already checked
+    if 'AlienSessionInfo' in globals():
+        AlienSessionInfo['verified_cert'] = True  # This means that we already checked
+        AlienSessionInfo['user_cert'] = USERCERT_NAME
+        AlienSessionInfo['user_key'] = USERKEY_NAME
     return USERCERT_NAME, USERKEY_NAME
 
 
-# Have global variables for checked at the load time of user certificates
-USERCERT_VALID, USERKEY_VALID = get_valid_certs()
-
-
 def get_valid_tokens() -> tuple:
     """Get the token filenames, including the temporary ones used as env variables"""
     global TOKENCERT_NAME, TOKENKEY_NAME
     random_str = None
     cert_suffix = None
+    ENV_TOKENCERT = ENV_TOKENKEY = None
     if not path_readable(TOKENCERT_NAME) and TOKENCERT_NAME.startswith('-----BEGIN CERTIFICATE-----'):  # and is not a file
         random_str = str(uuid.uuid4())
         cert_suffix = f'_{str(os.getuid())}_{random_str}.pem'
         temp_cert = tempfile.NamedTemporaryFile(prefix = 'tokencert_', suffix = cert_suffix, delete = False)
         temp_cert.write(TOKENCERT_NAME.encode(encoding = "ascii", errors = "replace"))
-        temp_cert.seek(0)
+        temp_cert.close()
         TOKENCERT_NAME = temp_cert.name  # temp file was created, let's give the filename to tokencert
-        AlienSessionInfo['templist'].append(TOKENCERT_NAME)  # type: ignore[attr-defined]
+        ENV_TOKENCERT = True
     if not path_readable(TOKENKEY_NAME) and TOKENKEY_NAME.startswith('-----BEGIN RSA PRIVATE KEY-----'):  # and is not a file
         if random_str is None: random_str = str(uuid.uuid4())
         temp_key = tempfile.NamedTemporaryFile(prefix = 'tokenkey_', suffix = cert_suffix, delete = False)
         temp_key.write(TOKENKEY_NAME.encode(encoding = "ascii", errors = "replace"))
-        temp_key.seek(0)
+        temp_key.close()
         TOKENKEY_NAME = temp_key.name  # temp file was created, let's give the filename to tokenkey
-        AlienSessionInfo['templist'].append(TOKENKEY_NAME)  # type: ignore[attr-defined]
+        ENV_TOKENKEY = True
 
     if (IsValidCert(TOKENCERT_NAME) and path_readable(TOKENKEY_NAME)):
-        AlienSessionInfo['verified_token'] = True
+        if 'AlienSessionInfo' in globals():
+            AlienSessionInfo['verified_token'] = True
+            AlienSessionInfo['token_cert'] = TOKENCERT_NAME
+            AlienSessionInfo['token_key'] = TOKENKEY_NAME
+            if ENV_TOKENCERT: AlienSessionInfo['templist'].append(TOKENKEY_NAME)  # type: ignore[attr-defined]
+            if ENV_TOKENKEY: AlienSessionInfo['templist'].append(TOKENCERT_NAME)  # type: ignore[attr-defined]
         return (TOKENCERT_NAME, TOKENKEY_NAME)
     return (None, None)
 
 
-# Check the presence of user certs and bailout before anything else
-TOKENCERT_VALID, TOKENKEY_VALID = get_valid_tokens()
-if not USERCERT_VALID and not TOKENCERT_VALID:
-    print_err(f'No valid user certificate or token found!! check {DEBUG_FILE} for further information and contact the developer if the information is not clear.')
-    sys.exit(126)
+def renewCredFilesInfo() -> CertsInfo:
+    """Recheck and refresh the values of valid credential definitions"""
+    token_cert, token_key = get_valid_tokens()
+    user_cert, user_key = get_valid_certs()
+    return CertsInfo(user_cert, user_key, token_cert, token_key)
+
 
+# Populate information in AlienSessionInfo
+_ = renewCredFilesInfo()
 
-def create_ssl_context(use_usercert: bool = False) -> ssl.SSLContext:
+
+def create_ssl_context(use_usercert: bool = False, user_cert: str = '', user_key: str = '', token_cert: str = '', token_key: str = '') -> ssl.SSLContext:
     """Create SSL context using either the default names for user certificate and token certificate or X509_USER_{CERT,KEY} JALIEN_TOKEN_{CERT,KEY} environment variables"""
-    if use_usercert or not TOKENCERT_VALID:
-        AlienSessionInfo['use_usercert'] = True
-        cert, key = USERCERT_VALID, USERKEY_VALID
+
+    if use_usercert or not token_cert:
+        if AlienSessionInfo: AlienSessionInfo['use_usercert'] = True
+        cert, key = user_cert, user_key
     else:
-        cert, key = TOKENCERT_VALID, TOKENKEY_VALID
+        cert, key = token_cert, token_key
 
-    if not cert:
+    if not cert or not key:
         print_err('create_ssl_context:: no certificate to be used for SSL context. This message should not be printed, contact the developer if you see this!!!')
-        os._exit(126)
+        return None
 
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     if DEBUG: logging.debug('\nCert = %s\nKey = %s\nCreating SSL context .. ', cert, key)
     ssl_protocol = ssl.PROTOCOL_TLS if sys.version_info[1] < 10 else ssl.PROTOCOL_TLS_CLIENT
     ctx = ssl.SSLContext(ssl_protocol)
     ctx.options |= ssl.OP_NO_SSLv3
     ctx.verify_mode = ssl.CERT_REQUIRED  # CERT_NONE, CERT_OPTIONAL, CERT_REQUIRED
     ctx.check_hostname = False
-    if DEBUG: logging.debug("SSL context:: Load verify locations")
 
     ca_verify_location = get_ca_path()
     cafile = capath = None
     if os.path.isfile(ca_verify_location):
         cafile = ca_verify_location
     else:
         capath = ca_verify_location
 
+    if DEBUG: logging.debug('SSL context:: Loading verify location:\n%s', ca_verify_location)
     try:
         ctx.load_verify_locations(cafile = cafile, capath = capath)
     except Exception:
-        logging.exception('Could not load verify location >>> %s <<<\n', ca_verify_location)  # EIO /* I/O error */
+        logging.exception('Could not load verify location!!!\n')
         print_err(f'Verify location could not be loaded!!! check content of >>> {ca_verify_location} <<< and the log')
-        os._exit(126)
+        return None  # EIO /* I/O error */
 
-    if DEBUG: logging.debug('SSL context:: Loading cert,key pair\n%s\n%s', cert, key)
+    if DEBUG: logging.debug('SSL context:: Loading cert,key pair:\n%s\n%s', cert, key)
     try:
         ctx.load_cert_chain(certfile = cert, keyfile = key)
     except Exception:
-        logging.exception('Could not load certificates!!!\n')  # EIO /* I/O error */
-        print_err('Error loading certificate pair!! Check the content of {DEBUG_FILE}')
-        os._exit(126)
+        logging.exception('Could not load certificates!!!\n')
+        print_err(f'Error loading certificate pair!! Check the content of {DEBUG_FILE}')
+        return None  # EIO /* I/O error */
 
-    if DEBUG: logging.debug('... SSL context done.')
+    if DEBUG: logging.debug('\n... SSL context done.')
     return ctx
 
 
 def CertInfo(fname: str) -> RET:
     """Print certificate information (subject, issuer, notbefore, notafter)"""
     try:
         with open(fname, encoding = "ascii", errors = "replace") as f:
@@ -291,21 +312,19 @@
     else:
         capath = ca_verify_location
 
     try:
         ctx.load_verify_locations(cafile = cafile, capath = capath)
     except Exception:
         logging.debug(traceback.format_exc())
-        return RET(5, "", f"Could not load verify location >>>{ca_verify_location}<<<")  # EIO /* I/O error */    
-    
+        return RET(5, "", f"Could not load verify location >>>{ca_verify_location}<<<")  # EIO /* I/O error */
+
     try:
         ctx.check_privatekey()
         return RET(0, f'Cert/key {PrintColor(COLORS.BIGreen)}match{PrintColor(COLORS.ColorReset)}')
     except OpenSSL.SSL.Error:
         return RET(0, '', f'Cert/key {PrintColor(COLORS.BIRed)}DO NOT match{PrintColor(COLORS.ColorReset)}')
 
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
-
```

### Comparing `alienpy-1.5.0/alienpy/data_structs.py` & `alienpy-1.5.1/alienpy/data_structs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 '''alienpy:: Definitions of data structures'''
 
-import os
 import sys
 from typing import NamedTuple
-from typing import Union
-# import shlex
-import json
-import logging
 
 
 ##############################################
 ##   Start of data structures definitons
 ##############################################
 
 class COLORS_COLL(NamedTuple):  # pylint: disable=inherit-non-class
@@ -115,46 +110,29 @@
 
 class KV(NamedTuple):  # pylint: disable=inherit-non-class
     """Assign a value to a key"""
     key: str = ''
     val: str = ''
 
 
+class CertsInfo(NamedTuple):  # pylint: disable=inherit-non-class
+    """Store name information on certificates used for SSL context"""
+    user_cert: str = ''
+    user_key: str = ''
+    token_cert: str = ''
+    token_key: str = ''
+
+
 class RET(NamedTuple):  # pylint: disable=inherit-non-class
     """Structure for POSIX like function return: exitcode, stdout, stderr, dictionary of server reply"""
     exitcode: int = -1
     out: str = ''
     err: str = ''
     ansdict: dict = {}
 
-    def print(self, opts: str = '') -> None:
-        """Print the in json format the content of ansdict, if existent"""
-        if 'json' in opts:
-            if self.ansdict:
-                json_out = json.dumps(self.ansdict, sort_keys = True, indent = 4)
-                print(json_out, flush = True)
-                DEBUG = os.getenv('ALIENPY_DEBUG', '')
-                if DEBUG: logging.debug(json_out)
-            else:
-                print('This command did not return a json dictionary', file = sys.stderr, flush = True)
-            return
-
-        if self.exitcode != 0:
-            if 'info' in opts: logging.info(self.err)
-            if 'warn' in opts: logging.warning(self.err)
-            if 'err' in opts: logging.error(self.err)
-            if 'debug' in opts: logging.debug(self.err)
-            if self.err and not ('noerr' in opts or 'noprint' in opts):
-                print(f'{self.err.strip()}', file = sys.stderr, flush = True)
-        else:
-            if self.out and not ('noout' in opts or 'noprint' in opts):
-                print(f'{self.out.strip()}', flush = True)
-
-    __call__ = print
-
     def __bool__(self) -> bool:
         return bool(self.exitcode == 0)
 
 
 class ALIEN_COLLECTION_EL(NamedTuple):  # pylint: disable=inherit-non-class
     """AliEn style xml collection element strucure"""
     name: str = ''
```

### Comparing `alienpy-1.5.0/alienpy/setup_cwd.py` & `alienpy-1.5.1/alienpy/setup_cwd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """alienpy:: setup cwd restoration"""
 
+import os
+import logging
 from .global_vars import *  # nosec PYL-W0614
+from .tools_nowb import read_conf_file
 from .wb_api import cd
-from .tools_misc import read_conf_file
 
 
 def GetSessionFilename() -> str: return os.path.join(os.path.expanduser("~"), ".alienpy_session")
 
 
 def SessionSave():
+    """Save CWD and previous CWD in .alienpy_session file"""
     session_filename = GetSessionFilename()
+    if 'AlienSessionInfo' not in globals(): return
     try:
         with open(session_filename, "w", encoding="ascii", errors="replace") as f:
             line1 = f"CWD = {AlienSessionInfo['currentdir']}\n"
             if not AlienSessionInfo['prevdir']: AlienSessionInfo['prevdir'] = AlienSessionInfo['currentdir']
             line2 = f"CWDPREV = {AlienSessionInfo['prevdir']}\n"
             f.writelines([line1, line2])
     except Exception as e:
@@ -21,19 +25,18 @@
         if DEBUG: logging.exception(e)
 
 
 def SessionRestore(wb):
     if os.getenv('ALIENPY_NO_CWD_RESTORE'): return
     session = read_conf_file(GetSessionFilename())
     if not session: return
-    sys_cur_dir = AlienSessionInfo['currentdir']
-    if 'CWD' in session: AlienSessionInfo['currentdir'] = session['CWD']
-    if 'CWDPREV' in session: AlienSessionInfo['prevdir'] = session['CWDPREV']
-    if AlienSessionInfo['currentdir'] and (sys_cur_dir != AlienSessionInfo['currentdir']):
-        cd(wb, AlienSessionInfo['currentdir'], opts = 'nocheck')
+    if 'AlienSessionInfo' in globals():
+        sys_cur_dir = AlienSessionInfo['currentdir']
+        if 'CWD' in session: AlienSessionInfo['currentdir'] = session['CWD']
+        if 'CWDPREV' in session: AlienSessionInfo['prevdir'] = session['CWDPREV']
+        if AlienSessionInfo['currentdir'] and (sys_cur_dir != AlienSessionInfo['currentdir']): cd(wb, AlienSessionInfo['currentdir'], opts = 'nocheck')
 
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
- 
+
```

### Comparing `alienpy-1.5.0/alienpy/setup_logging.py` & `alienpy-1.5.1/alienpy/setup_logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 '''alienpy:: Setup logging'''
 
 import os
 import sys
 import logging
-from pathlib import Path
 from .global_vars import *  # nosec PYL-W0614
 
 
 #############################################
 ###   ENABLE LOGGING BEFORE ANYTHIN ELSE
 #############################################
 def print_out(msg: str, toLog: bool = False):
@@ -20,21 +19,20 @@
 def print_err(msg: str, toLog: bool = False):
     if toLog:
         logging.log(95, msg)
     else:
         print(msg, file = sys.stderr, flush = True)
 
 
-def setup_logging(debug: bool = False, debug_file:str = ''):
+def setup_logging(debug: bool = False, debug_file:str = f'{USER_HOME}/alien_py.log'):
     """Setup logging machinery"""
-    if not debug_file: debug_file = f'{Path.home().as_posix()}/alien_py.log'
 
     logging.addLevelName(90, 'STDOUT')
     logging.addLevelName(95, 'STDERR')
-    
+
     MSG_LVL = logging.DEBUG if debug else logging.INFO
     line_fmt = '%(levelname)s:%(asctime)s %(message)s'
     file_mode = 'a' if os.getenv('ALIENPY_DEBUG_APPEND', '') else 'w'
     try:
         logging.basicConfig(format = line_fmt, filename = debug_file, filemode = file_mode, level = MSG_LVL)
     except Exception:
         print_err(f'Could not write the log file {debug_file}; falling back to detected tmp dir')
@@ -54,9 +52,8 @@
     if os.getenv('ALIENPY_DEBUG_STAGGER'):
         logging.getLogger('async_stagger').setLevel(MSG_LVL)
 
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
-    
+
```

### Comparing `alienpy-1.5.0/alienpy/tools_shell.py` & `alienpy-1.5.1/alienpy/tools_shell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 '''alienpy:: Misc tooling functions'''
 
 import re
 import sys
 import subprocess  # nosec B404:blacklist
 import shlex
+from typing import Union
+from shutil import which
 from .data_structs import *  # nosec PYL-W0614
 from .setup_logging import print_err
 
 
 def runShellCMD(INPUT: str = '', captureout: bool = True, do_shell: bool = False, timeout: Union[str, int, None] = None) -> RET:
     """Run shell command in subprocess; if exists, print stdout and stderr"""
     if not INPUT: return RET(1, '', 'No command to be run provided')
@@ -33,12 +35,16 @@
         if status.stdout: msg_out = status.stdout.strip()
         if status.stderr: msg_err = status.stderr.strip()
         exitcode = status.returncode
     if except_msg: msg_err = f'{except_msg}\n{msg_err}'
     return RET(exitcode, msg_out, msg_err)
 
 
+def is_cmd(cmd:str = ''):
+    """Check if cmd is available in shell"""
+    return which(cmd) is not None
+
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
```

### Comparing `alienpy-1.5.0/alienpy/tools_stackcmd.py` & `alienpy-1.5.1/alienpy/tools_stackcmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """alienpy:: command stack manipulation"""
 
-import collections
+from collections import deque
 from .global_vars import *  # nosec PYL-W0614
 
 
-deque = collections.deque
-
 def push2stack(path: str):
-    if not str: return
+    if not str or 'AlienSessionInfo' not in globals(): return
     home = ''
     if AlienSessionInfo['alienHome']: home = AlienSessionInfo['alienHome'][:-1]
     if home and home in path: path = path.replace(home, '~')
     AlienSessionInfo['pathq'].appendleft(path)
 
 
 def deque_pop_pos(dq: deque, pos: int = 1) -> str:
     if abs(pos) > len(dq) - 1: return ''
     pos = - pos
     dq.rotate(pos)
+    val = ''
     if pos > 0:
         val = dq.pop()
         if len(dq) > 1: dq.rotate(- (pos - 1))
     else:
         val = dq.popleft()
         if len(dq) > 1: dq.rotate(abs(pos) - 1)
     return val  # noqa: R504
 
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
-
```

### Comparing `alienpy-1.5.0/alienpy/wb_api.py` & `alienpy-1.5.1/alienpy/wb_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,39 @@
 """WEBSOCKET:: API for WebSOcket communications"""
 
+import sys
 import os
 import json
 import shlex
+import logging
+import traceback
+from typing import Union
+import time
+
+try:
+    import websockets.exceptions as wb_exceptions
+except Exception:
+    print("websockets module could not be imported! Make sure you can do:\npython3 -c 'import websockets.exceptions as wb_exceptions'", file = sys.stderr, flush = True)
+    sys.exit(1)
 
 from .global_vars import *  # nosec PYL-W0614
-from .tools_misc import *  # nosec PYL-W0614
-from .wb_async import *  # nosec PYL-W0614
-from .tools_stackcmd import push2stack
 from .setup_logging import print_out, print_err
 
-
-class Msg:
-    """Class to create json messages to be sent to server"""
-    __slots__ = ('cmd', 'args', 'opts')
-
-    def __init__(self, cmd: str = '', args: Union[str, list, None] = None, opts: str = '') -> None:
-        self.cmd = cmd
-        self.opts = opts
-        if not args:
-            self.args = []
-        elif isinstance(args, str):
-            self.args = shlex.split(args)
-        elif isinstance(args, list):
-            self.args = args.copy()
-
-    def add_arg(self, arg: Union[str, list, None]) -> None:
-        if not arg: return
-        if isinstance(arg, str): self.args.extend(shlex.split(arg))
-        if isinstance(arg, list): self.args.extend(arg)
-
-    def msgdict(self) -> dict:
-        return CreateJsonCommand(self.cmd, self.args, self.opts, True)
-
-    def msgstr(self) -> str:
-        return CreateJsonCommand(self.cmd, self.args, self.opts)
-
-    def __call__(self) -> tuple:
-        return (self.cmd, self.args, self.opts)
-
-    def __bool__(self):
-        return bool(self.cmd)
+from .async_tools import syncify
+from .wb_async import wb_create, wb_close, wb_sendmsg, wb_sendmsg_multi, IsWbConnected
+from .tools_nowb import deltat_ms_perf, deltat_us_perf, is_help, writePidFile, read_conf_file, is_my_pid, isReachable, path_readable
+from .tools_stackcmd import push2stack  # , deque_pop_pos
+from .connect_ssl import get_certs_names
 
 
 def wb_create_tryout(host: str, port: Union[str, int], path: str = '/', use_usercert: bool = False, localConnect: bool = False):
     """WebSocket creation with tryouts (configurable by env ALIENPY_CONNECT_TRIES and ALIENPY_CONNECT_TRIES_INTERVAL)"""
     wb = None
     nr_tries = 0
     init_begin = None
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
 
     if TIME_CONNECT or DEBUG: init_begin = time.perf_counter()
     connect_tries = int(os.getenv('ALIENPY_CONNECT_TRIES', '3'))
     connect_tries_interval = float(os.getenv('ALIENPY_CONNECT_TRIES_INTERVAL', '0.5'))
 
     while wb is None:
         nr_tries += 1
@@ -77,24 +58,23 @@
         writePidFile(pid_filename)
     return wb
 
 
 def AlienConnect(wb = None, token_args: Union[None, list] = None, use_usercert: bool = False, localConnect: bool = False):
     """Create a websocket connection to AliEn services either directly to alice-jcentral.cern.ch or trough a local found jbox instance"""
     if not token_args: token_args = []
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     init_begin = time.perf_counter() if (TIME_CONNECT or DEBUG) else None
 
     jalien_server = os.getenv("ALIENPY_JCENTRAL", 'alice-jcentral.cern.ch')  # default value for JCENTRAL
     jalien_websocket_port = os.getenv("ALIENPY_JCENTRAL_PORT", '8097')  # websocket port
     jalien_websocket_path = '/websocket/json'
     jclient_env = f'{TMPDIR}/jclient_token_{str(os.getuid())}'
 
     # If presentent with existing socket, let's try to close it
-    if wb: wb_close(wb, code = 1000, reason = 'Close previous websocket')
+    if wb: _ = wb_close(wb, code = 1000, reason = 'Close previous websocket')
 
     # let's try to get a websocket
     if localConnect:
         wb = wb_create(localConnect = True)
     else:
         if not os.getenv("ALIENPY_JCENTRAL") and os.path.exists(jclient_env):  # If user defined ALIENPY_JCENTRAL the intent is to set and use the endpoint
             # lets check JBOX availability
@@ -122,114 +102,78 @@
         msg = f'Check the logfile: {DEBUG_FILE}\nCould not get a websocket connection to {jalien_server}:{jalien_websocket_port}'
         logging.error(msg)
         print_err(msg)
         sys.exit(107)  # ENOTCONN - Transport endpoint is not connected
     return wb
 
 
-def CreateJsonCommand(cmdline: Union[str, dict], args: Union[None, list] = None, opts: str = '', get_dict: bool = False) -> Union[str, dict]:
-    """Return a json with command and argument list"""
-    if args is None: args = []
-    if isinstance(cmdline, dict):
-        out_dict = cmdline.copy()
-        if 'showmsg' in opts: opts = opts.replace('nomsg', '')
-        if 'showkeys' in opts: opts = opts.replace('nokeys', '')
-        if 'nomsg' in opts: out_dict["options"].insert(0, '-nomsg')
-        if 'nokeys' in opts: out_dict["options"].insert(0, '-nokeys')
-        return out_dict if get_dict else json.dumps(out_dict)
-
-    if not args:
-        args = shlex.split(cmdline)
-        cmd = args.pop(0) if args else ''
-    else:
-        cmd = cmdline
-    if 'nomsg' in opts: args.insert(0, '-nomsg')
-    if 'nokeys' in opts: args.insert(0, '-nokeys')
-    jsoncmd = {"command": cmd, "options": args}
-    return jsoncmd if get_dict else json.dumps(jsoncmd)
+def InitConnection(wb = None, token_args: Union[None, list] = None, use_usercert: bool = False, localConnect: bool = False, cmdlist_func = None):
+    """Create a session to AliEn services, including session globals and token regeneration"""
+    global ALIENPY_GLOBAL_WB
+
+    wb = AlienConnect(wb, token_args, use_usercert, localConnect)
+    ALIENPY_GLOBAL_WB = wb
+
+    # NO MATTER WHAT BEFORE ENYTHING ELSE SESSION MUST BE INITIALIZED   !!!!!!!!!!!!!!!!
+    if 'AlienSessionInfo' in globals():
+        if not AlienSessionInfo['session_started']:  # this is beggining of session, let's get session vars ONLY ONCE
+            AlienSessionInfo['session_started'] = True
+            session_begin = time.perf_counter() if (TIME_CONNECT or DEBUG) else None
+
+            ret_obj = SendMsg(wb, 'commandlist', [])  # it will automatically initialize user, currentdir, prevdir, alienHome (as each SendMsg does)
+            if not ret_obj.ansdict or 'results' not in ret_obj.ansdict:
+                print_err("Start session:: could not get command list, let's exit.")
+                sys.exit(1)
+
+            csd_cmds_re = re.compile(r'.*_csd$')
+            AlienSessionInfo['commandlist'] = [cmd["commandlist"] for cmd in ret_obj.ansdict["results"] if not csd_cmds_re.match(cmd["commandlist"])]
+
+            if session_begin:
+                msg = f">>>   Time for session initialization: {deltat_ms_perf(session_begin)} ms"
+                if DEBUG: logging.debug(msg)
+                if TIME_CONNECT: print_out(msg)
 
+        # construct command list with function in main module
+        if cmdlist_func: cmdlist_func()
 
-def session_state_update (out_dict: dict) -> None:
-    """Update global AlienSessionInfo with status of the latest command"""
-    if AlienSessionInfo:  # update global state of session
-        AlienSessionInfo['user'] = out_dict["metadata"]["user"]  # always update the current user
-        current_dir = out_dict["metadata"]["currentdir"]
+        # if this is a reconnection, make sure on the server we are in the last known current directory
+        if AlienSessionInfo['currentdir']: cd(wb, AlienSessionInfo['currentdir'], 'log')
 
-        # if this is first connection, current dir is alien home
-        if not AlienSessionInfo['alienHome']: AlienSessionInfo['alienHome'] = current_dir
-
-        # update the current current/previous dir status
-        # previous/current have the meaning of before and after command execution
-        prev_dir = AlienSessionInfo['currentdir']  # last known current dir
-        if prev_dir != current_dir:
-            AlienSessionInfo['currentdir'] = current_dir
-            AlienSessionInfo['prevdir'] = prev_dir
-
-        # update directory stack (pushd/popd/dirs)
-        short_current_dir = current_dir.replace(AlienSessionInfo['alienHome'][:-1], '~')
-        short_current_dir = short_current_dir[:-1]  # remove the last /
-        if AlienSessionInfo['pathq']:
-            if AlienSessionInfo['pathq'][0] != short_current_dir: AlienSessionInfo['pathq'][0] = short_current_dir
-        else:
-            push2stack(short_current_dir)
-
-
-def retf_result2ret(result: Union[str, dict, None]) -> RET:
-    """Convert AliEn answer dictionary to RET object"""
-    if not result: return RET(61, '', 'Empty input')  # type: ignore [call-arg]
-    out_dict = None
-    if isinstance(result, str):
-        try:
-            out_dict = json.loads(result)
-        except Exception as e:
-            msg = f'retf_result2ret:: Could not load argument as json!\n{e!r}'
-            logging.error(msg)
-            return RET(22, '', msg)  # type: ignore [call-arg]
-    else:
-        out_dict = result.copy()
-
-    if 'metadata' not in out_dict or 'results' not in out_dict:  # these works only for AliEn responses
-        msg = 'retf_results2ret:: Dictionary does not have AliEn answer format'
-        logging.error(msg)
-        return RET(52, '', msg)  # type: ignore [call-arg]
-
-    session_state_update(out_dict)
-    message_list = [str(item['message']) for item in out_dict['results'] if 'message' in item]
-    output = '\n'.join(message_list)
-    return RET(int(out_dict["metadata"]["exitcode"]), output.strip(), out_dict["metadata"]["error"], out_dict)  # type: ignore [call-arg]
+        # if usercert connection always regenerate token if connected with usercert
+        if AlienSessionInfo['use_usercert'] and token(wb, token_args) != 0: print_err(f'The token could not be created! check the logfile {DEBUG_FILE}')
+    return wb
 
 
-def SendMsg(wb, cmdline: str, args: Union[None, list] = None, opts: str = '') -> Union[RET, str]:
+def SendMsg(wb, cmdline: str, args: Union[None, list] = None, opts: str = '') -> RET:
     """Send a json message to the specified websocket; it will return the server answer"""
     if not wb:
         msg = "SendMsg:: websocket not initialized"
         logging.info(msg)
-        return '' if 'rawstr' in opts else RET(1, '', msg)  # type: ignore [call-arg]
+        return RET(1, '', msg)  # type: ignore [call-arg]
     if not args: args = []
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')    
     JSON_OUT_GLOBAL = os.getenv('ALIENPY_JSON_OUT_GLOBAL')
     JSON_OUT = os.getenv('ALIENPY_JSON_OUT')
 
     time_begin = time.perf_counter() if DEBUG or DEBUG_TIMING else None
 
-    if JSON_OUT_GLOBAL or JSON_OUT:  
-        opts = opts.replace('nokeys', '')
+    if JSON_OUT_GLOBAL or JSON_OUT:
+        opts = opts.replace('-nokeys', '').replace('nokeys', '')
         if 'nomsg' not in opts: opts = f'{opts} nomsg'
 
     # if DEBUG then make sure we get the full answer
     if DEBUG:
-        opts = opts.replace('nokeys', '').replace('nomsg', '')
+        opts = opts.replace('-nokeys', '').replace('-nomsg', '').replace('nokeys', '').replace('nomsg', '')
 
     json_signature = ['{"command":', '"options":']
     # if already json format just use it as is; nomsg/nokeys will be passed to CreateJsonCommand
     jsonmsg = cmdline if all(x in cmdline for x in json_signature) else CreateJsonCommand(cmdline, args, opts)
 
     if not jsonmsg:
         logging.info("SendMsg:: json message is empty!")
-        return '' if 'rawstr' in opts else RET(1, '', f"SendMsg:: empty json with args:: {cmdline} {' '.join(args)} /opts= {opts}")  # type: ignore [call-arg]
+        return RET(1, '', f"SendMsg:: empty json with args:: {cmdline} {' '.join(args)} /opts= {opts}")  # type: ignore [call-arg]
 
     if DEBUG:
         logging.debug(f"Called from: {sys._getframe().f_back.f_code.co_name}\n>>>   SEND COMMAND:: {jsonmsg}")  # pylint: disable=protected-access
 
     nr_tries = int(1)
     result = None
     while result is None:
@@ -243,31 +187,83 @@
         if result is None: time.sleep(0.2)
 
     if time_begin: logging.debug('SendMsg::Result received: %s ms', deltat_ms_perf(time_begin))
     if not result:
         msg = f"SendMsg:: could not send command: {jsonmsg}\nCheck {DEBUG_FILE}"
         print_err(msg)
         logging.error(msg)
-        return RET(70, '', 'SendMsg:: Empty result received from server')  # type: ignore [call-arg]  # ECOMM  
+        return RET(70, '', 'SendMsg:: Empty result received from server')  # type: ignore [call-arg]  # ECOMM
 
-    if 'rawstr' in opts: return result
     time_begin_decode = time.perf_counter() if DEBUG or DEBUG_TIMING else None
     ret_obj = retf_result2ret(result)
     if time_begin_decode: logging.debug('SendMsg::Result decoded: %s us', deltat_us_perf(time_begin_decode))
     return ret_obj  # noqa: R504
 
 
+def retf_result2ret(result: Union[str, dict, None]) -> RET:
+    """Convert AliEn answer dictionary to RET object"""
+    if not result: return RET(61, '', 'Empty input')  # type: ignore [call-arg]
+    out_dict = None
+    if isinstance(result, str):
+        try:
+            out_dict = json.loads(result)
+        except Exception as e:
+            msg = f'retf_result2ret:: Could not load argument as json!\n{e!r}'
+            logging.error(msg)
+            return RET(22, '', msg)  # type: ignore [call-arg]
+    elif isinstance(result, dict):
+        out_dict = result
+    else:
+        msg = 'retf_result2ret:: Wrong type of argument'
+        logging.error(msg)
+        return RET(42, '', msg)  # type: ignore [call-arg]
+
+    if 'metadata' not in out_dict or 'results' not in out_dict:  # these works only for AliEn responses
+        msg = 'retf_results2ret:: Dictionary does not have AliEn answer format'
+        logging.error(msg)
+        return RET(42, '', msg)  # type: ignore [call-arg]
+
+    session_state_update(out_dict)  # ALWAYS UPDATE GLOBAL STATE
+    message_list = [str(item['message']) for item in out_dict['results'] if 'message' in item]
+    output = '\n'.join(message_list)
+    return RET(int(out_dict["metadata"]["exitcode"]), output.strip(), out_dict["metadata"]["error"], out_dict)  # type: ignore [call-arg]
+
+
+def session_state_update(out_dict: dict) -> None:
+    """Update global AlienSessionInfo with status of the latest command"""
+    if 'AlienSessionInfo' in globals():  # update global state of session
+        AlienSessionInfo['user'] = out_dict["metadata"]["user"]  # always update the current user
+        current_dir = out_dict["metadata"]["currentdir"]
+
+        # if this is first connection, current dir is alien home
+        if not AlienSessionInfo['alienHome']: AlienSessionInfo['alienHome'] = current_dir
+
+        # update the current current/previous dir status
+        # previous/current have the meaning of before and after command execution
+        prev_dir = AlienSessionInfo['currentdir']  # last known current dir
+        if prev_dir != current_dir:
+            AlienSessionInfo['currentdir'] = current_dir
+            AlienSessionInfo['prevdir'] = prev_dir
+
+        # update directory stack (pushd/popd/dirs)
+        short_current_dir = current_dir.replace(AlienSessionInfo['alienHome'][:-1], '~')
+        short_current_dir = short_current_dir[:-1]  # remove the last /
+        if AlienSessionInfo['pathq']:
+            if AlienSessionInfo['pathq'][0] != short_current_dir: AlienSessionInfo['pathq'][0] = short_current_dir
+        else:
+            push2stack(short_current_dir)
+
+
 def SendMsgMulti(wb, cmds_list: list, opts: str = '') -> list:
     """Send a json message to the specified websocket; it will return the server answer"""
     if not wb:
         msg = "SendMsg:: websocket not initialized"
         logging.info(msg)
-        return '' if 'rawstr' in opts else RET(1, '', msg)  # type: ignore [call-arg]
+        return RET(1, '', msg)  # type: ignore [call-arg]
     if not cmds_list: return []
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     JSON_OUT_GLOBAL = os.getenv('ALIENPY_JSON_OUT_GLOBAL')
     JSON_OUT = os.getenv('ALIENPY_JSON_OUT')
 
     time_begin = time.perf_counter() if DEBUG or DEBUG_TIMING else None
     if JSON_OUT_GLOBAL or JSON_OUT or DEBUG:  # if jsout output was requested, then make sure we get the full answer
         opts = opts.replace('nokeys', '').replace('nomsg', '')
 
@@ -294,93 +290,270 @@
                 wb = AlienConnect(wb)
             except Exception:
                 logging.exception('SendMsgMulti:: Could not recover connection when disconnected!!')
         except Exception:
             logging.exception('SendMsgMulti:: Abnormal connection status!!!')
         if result_list is None: time.sleep(0.2)
 
-    if time_begin: logging.debug('SendMsg::Result received: %s ms', deltat_ms(time_begin))
+    if time_begin: logging.debug('SendMsg::Result received: %s ms', deltat_ms_perf(time_begin))
     if not result_list: return []
-    if 'rawstr' in opts: return result_list
     time_begin_decode = time.perf_counter() if DEBUG or DEBUG_TIMING else None
     ret_obj_list = [retf_result2ret(result) for result in result_list]
-    if time_begin_decode: logging.debug('SendMsg::Result decoded: %s ms', deltat_ms(time_begin_decode))
+    if time_begin_decode: logging.debug('SendMsg::Result decoded: %s ms', deltat_ms_perf(time_begin_decode))
     return ret_obj_list  # noqa: R504
 
 
+def PrintDict(in_arg: Union[str, dict, list, None] = None, compact: bool = False):
+    """Print a dictionary in a nice format"""
+    if not in_arg: return
+    if isinstance(in_arg, str):
+        try:
+            in_arg = json.loads(in_arg)
+        except Exception as e:
+            print_err(f'PrintDict:: Could not load argument as json!\n{e!r}')
+            return
+    if isinstance(in_arg, (dict, list)):
+        indent = None if compact else 2
+        separators = (',', ':') if compact else None
+        if 'HAS_PPRINT' in globals() and HAS_PPRINT:
+            print_json(data = in_arg)
+        else:
+            print_out(json.dumps(in_arg, sort_keys = True, indent = indent, separators = separators, skipkeys = False))
+
+
 def retf_print(ret_obj: RET, opts: str = '') -> int:
     """Process a RET object; it will return the exitcode
     opts content will steer the logging and message printing:
      - noprint : silence all stdout/stderr printing
      - noerr/noout : silence the respective messages
      - info/warn/err/debug : will log the stderr to that facility
      - json : will print just the json (if present)
     """
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     if 'json' in opts:
         if ret_obj.ansdict:
-            json_out = json.dumps(ret_obj.ansdict, sort_keys = True, indent = 3)
-            if DEBUG: logging.debug(json_out)
-            print_out(json_out)
+            PrintDict(ret_obj.ansdict)
         else:
             print_err('This command did not return a json dictionary')
         return ret_obj.exitcode
 
     if ret_obj.exitcode != 0:
-        if 'info' in opts: logging.info(ret_obj.err)
-        if 'warn' in opts: logging.warning(ret_obj.err)
-        if 'err' in opts: logging.error(ret_obj.err)
-        if 'debug' in opts: logging.debug(ret_obj.err)
-        if ret_obj.err and not ('noerr' in opts or 'noprint' in opts):
-            print_err(f'{ret_obj.err.strip()}')
+        if 'debug' in opts:
+            logging.debug(ret_obj.err)
+        elif 'info' in opts:
+            logging.info(ret_obj.err)
+        elif 'warn' in opts:
+            logging.warning(ret_obj.err)
+        else:
+            logging.error(ret_obj.err)
+        if ret_obj.err and not ('noerr' in opts or 'noprint' in opts): print_err(f'{ret_obj.err.strip()}')
     else:
-        if ret_obj.out and not ('noout' in opts or 'noprint' in opts):
-            print_out(f'{ret_obj.out.strip()}')
+        if ret_obj.out and not ('noout' in opts or 'noprint' in opts): print_out(f'{ret_obj.out.strip()}')
     return ret_obj.exitcode
 
 
 def GetMeta(result: dict) -> dict:
-    """Converta metadata field of an JAliEn response to a dict"""
-    output = { 'cwd': None, 'user': None, 'error': None, 'exitcode': None }
-    if not result: return output
-    if isinstance(result, dict) and 'metadata' in result:  # these works only for AliEn responses
-        output['cwd'] = result['metadata']['currentdir']
-        output['user'] = result['metadata']['user']
-        output['error'] = result['metadata']['error']
-        output['exitcode'] = result['metadata']['exitcode']
-    return output
+    """Return metadata of an JAliEn response"""
+    if not result: return {}
+    if isinstance(result, dict) and 'metadata' in result: return result['metadata']
+    return {}
+
+
+def CreateJsonCommand(cmdline: Union[str, dict], args: Union[None, list] = None, opts: str = '', get_dict: bool = False) -> Union[str, dict]:
+    """Return a json with command and argument list"""
+    if not cmdline: return ''
+    if args is None: args = []
+    if isinstance(cmdline, dict):
+        if 'command' not in cmdline or 'options' not in cmdline: return ''
+        out_dict = cmdline.copy()
+        if 'showmsg' in opts: opts = opts.replace('nomsg', '')
+        if 'showkeys' in opts: opts = opts.replace('nokeys', '')
+        if 'nomsg' in opts: out_dict["options"].insert(0, '-nomsg')
+        if 'nokeys' in opts: out_dict["options"].insert(0, '-nokeys')
+        return out_dict if get_dict else json.dumps(out_dict)
+
+    if not args:
+        args = shlex.split(cmdline)
+        cmd = args.pop(0) if args else ''
+    else:
+        cmd = cmdline
+    if 'nomsg' in opts: args.insert(0, '-nomsg')
+    if 'nokeys' in opts: args.insert(0, '-nokeys')
+    jsoncmd = {"command": cmd, "options": args}
+    return jsoncmd if get_dict else json.dumps(jsoncmd)
 
 
-def cd(wb, args: Union[str, list] = None, opts: str = '') -> RET:
+def token(wb, args: Union[None, list] = None) -> int:
+    """(Re)create the tokencert and tokenkey files"""
+    if not wb: return 1
+    if not args: args = []
+    certs_info = get_certs_names()
+    _ = is_help(args, clean_args = True)
+
+    ret_obj = SendMsg(wb, 'token', args, opts = 'nomsg')
+    if ret_obj.exitcode != 0:
+        logging.error('Token request returned error')
+        return retf_print(ret_obj, 'err')
+    tokencert_content = tokenkey_content = None
+    ret_results = ret_obj.ansdict['results'] if ret_obj.ansdict and 'results' in ret_obj.ansdict else []
+    if len(ret_results) > 0:
+        tokencert_content = ret_results[0].get('tokencert', '')
+        tokenkey_content = ret_results[0].get('tokenkey', '')
+    if not tokencert_content or not tokenkey_content:
+        logging.error('Token request valid but empty fields!!')
+        return int(42)  # ENOMSG
+
+    try:
+        if path_readable(certs_info.token_cert):
+            os.chmod(certs_info.token_cert, 0o600)  # make it writeable
+            os.remove(certs_info.token_cert)
+        with open(certs_info.token_cert, "w", encoding = "ascii", errors = "replace") as tcert: print(f"{tokencert_content}", file = tcert)  # write the tokencert
+        os.chmod(certs_info.token_cert, 0o400)  # make it readonly
+    except Exception:
+        print_err(f'Error writing to file the aquired token cert; check the log file {DEBUG_FILE}!')
+        logging.debug(traceback.format_exc())
+        return 5  # EIO
+
+    try:
+        if path_readable(certs_info.token_key):
+            os.chmod(certs_info.token_key, 0o600)  # make it writeable
+            os.remove(certs_info.token_key)
+        with open(certs_info.token_key, "w", encoding = "ascii", errors = "replace") as tkey: print(f"{tokenkey_content}", file = tkey)  # write the tokenkey
+        os.chmod(certs_info.token_key, 0o400)  # make it readonly
+    except Exception:
+        print_err(f'Error writing to file the aquired token key; check the log file {DEBUG_FILE}!')
+        logging.debug(traceback.format_exc())
+        return 5  # EIO
+    if 'AlienSessionInfo' in globals():
+        AlienSessionInfo['token_cert'] = certs_info.token_cert
+        AlienSessionInfo['token_key'] = certs_info.token_key
+    return int(0)
+
+
+def token_regen(wb, args: Union[None, list] = None):
+    """Do the disconnect, connect with user cert, generate token, re-connect with token procedure"""
+    wb_usercert = None
+    if not args: args = []
+
+    if 'AlienSessionInfo' in globals() and not AlienSessionInfo['use_usercert']:
+        _ = wb_close(wb, code = 1000, reason = 'Lets connect with usercert to be able to generate token')
+        try:
+            wb_usercert = InitConnection(wb, args, use_usercert = True)  # we have to reconnect with the new token
+        except Exception:
+            logging.debug(traceback.format_exc())
+            return None  # we failed usercert connection
+
+    # now we are connected with usercert, so we can generate token
+    if token(wb_usercert, args) != 0: return wb_usercert
+    # we have to reconnect with the new token
+    _ = wb_close(wb_usercert, code = 1000, reason = 'Re-initialize the connection with the new token')
+    if 'AlienSessionInfo' in globals(): AlienSessionInfo['use_usercert'] = False
+    wb_token_new = None
+    try:
+        wb_token_new = InitConnection(wb_token_new, args)
+        __ = SendMsg(wb_token_new, 'pwd', [], opts = 'nokeys')  # just to refresh cwd
+    except Exception:
+        logging.exception('token_regen:: error re-initializing connection')
+    return wb_token_new
+
+
+def cd(wb, args: Union[str, list, None] = None, opts: str = '') -> RET:
     """Override cd to add to home and to prev functions"""
     if args is None: args = []
     if isinstance(args, str): args = args.split()
     if is_help(args): return get_help_srv(wb, 'cd')
     if args:
         if args[0] == '-': args = [AlienSessionInfo['prevdir']]
         if 'nocheck' not in opts and AlienSessionInfo['currentdir'].rstrip('/') == args[0].rstrip('/'): return RET(0)  # type: ignore [call-arg]
     return SendMsg(wb, 'cd', args, opts)
 
 
+def get_list_entries(wb, lfn, fullpath: bool = False) -> list:
+    """return a list of entries of the lfn argument, full paths if 2nd arg is True"""
+    key = 'path' if fullpath else 'name'
+    ret_obj = SendMsg(wb, 'ls', ['-nomsg', '-a', '-F', os.path.normpath(lfn)])
+    if ret_obj.exitcode != 0: return []
+    return [item[key] for item in ret_obj.ansdict['results']]
+
+
+def lfn_list(wb, lfn: str = ''):
+    """Completer function : for a given lfn return all options for latest leaf"""
+    if not wb: return []
+    if not lfn: lfn = '.'  # AlienSessionInfo['currentdir']
+    list_lfns = []
+    lfn_path = Path(lfn)
+    base_dir = '/' if lfn_path.parent.as_posix() == '/' else f'{lfn_path.parent.as_posix()}/'
+    name = f'{lfn_path.name}/' if lfn.endswith('/') else lfn_path.name
+
+    def item_format(base_dir, name, item):
+        # print_out(f'\nbase_dir: {base_dir} ; name: {name} ; item: {item}')
+        if name.endswith('/') and name != '/':
+            return f'{name}{item}' if base_dir == './' else f'{base_dir}{name}{item}'
+        return item if base_dir == './' else f'{base_dir}{item}'
+
+    if lfn.endswith('/'):
+        listing = get_list_entries(wb, lfn)
+        list_lfns = [item_format(base_dir, name, item) for item in listing]
+    else:
+        listing = get_list_entries(wb, base_dir)
+        list_lfns = [item_format(base_dir, name, item) for item in listing if item.startswith(name)]
+    return list_lfns
+
+
+def wb_ping(wb) -> float:
+    """Websocket ping function, it will return rtt in ms"""
+    init_begin = time.perf_counter()
+    if IsWbConnected(wb):
+        return float(deltat_ms_perf(init_begin))
+    return float(-1)
+
+
 def get_help_srv(wb, cmd: str = '') -> RET:
     """Return the help option for server-side known commands"""
     if not cmd: return RET(1, '', 'No command specified for help request')
     return SendMsg(wb, f'{cmd} -h')
 
 
+class Msg:
+    """Class to create json messages to be sent to server"""
+    __slots__ = ('cmd', 'args', 'opts')
+
+    def __init__(self, cmd: str = '', args: Union[str, list, None] = None, opts: str = '') -> None:
+        self.cmd = cmd
+        self.opts = opts
+        if not args:
+            self.args = []
+        elif isinstance(args, str):
+            self.args = shlex.split(args)
+        elif isinstance(args, list):
+            self.args = args.copy()
+
+    def add_arg(self, arg: Union[str, list, None]) -> None:
+        if not arg: return
+        if isinstance(arg, str): self.args.extend(shlex.split(arg))
+        if isinstance(arg, list): self.args.extend(arg)
+
+    def msgdict(self) -> dict:
+        return CreateJsonCommand(self.cmd, self.args, self.opts, True)
+
+    def msgstr(self) -> str:
+        return CreateJsonCommand(self.cmd, self.args, self.opts)
+
+    def __call__(self) -> tuple:
+        return (self.cmd, self.args, self.opts)
+
+    def __bool__(self):
+        return bool(self.cmd)
+
+
 @syncify
 async def msg_proxy(websocket, use_usercert = False):
     """Proxy messages from a connection point to another"""
     wb_jalien = AlienConnect(None, use_usercert)
     local_query = await websocket.recv()
     jalien_answer = SendMsg(wb_jalien, local_query)
     await websocket.send(jalien_answer.ansdict)
 
 
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
-    
-    
-    
-
```

### Comparing `alienpy-1.5.0/alienpy/wb_async.py` & `alienpy-1.5.1/alienpy/wb_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """WEBSOCKET:: main async functions"""
 
 import os
 import sys
-# import asyncio
 import socket
+import logging
+import time
+from typing import Union
 
 try:
     import websockets.client as wb_client
     import websockets.exceptions as wb_exceptions
     import websockets.version as wb_version
     from websockets.extensions import permessage_deflate as _wb_permessage_deflate
 except Exception:
@@ -18,43 +20,43 @@
 if not os.getenv('ALIENPY_NO_STAGGER'):
     try:
         import async_stagger  # type: ignore
     except Exception:
         print("async_stagger module could not be imported! Make sure you can do:\npython3 -c 'import async_stagger'", file = sys.stderr, flush = True)
         sys.exit(1)
 
-from .version import *  # nosec PYL-W0614
 from .global_vars import *  # nosec PYL-W0614
-from .data_structs import *  # nosec PYL-W0614
+from .version import ALIENPY_VERSION_STR  # nosec PYL-W0614
+from .tools_nowb import deltat_ms_perf
+
 from .setup_logging import print_err
-from .connect_ssl import create_ssl_context
-from .tools_misc import *  # nosec PYL-W0614
+from .connect_ssl import create_ssl_context, renewCredFilesInfo
 
 #########################
 #   ASYNCIO MECHANICS
 #########################
 from .async_tools import start_asyncio, syncify
 # Let's start the asyncio main thread
 start_asyncio()
 
 
 @syncify
 async def wb_create(host: str = 'localhost', port: Union[str, int] = '8097', path: str = '/', use_usercert: bool = False, localConnect: bool = False):
     """Create a websocket to wss://host:port/path (it is implied a SSL context)"""
+
     if not host:
         msg = 'wb_create:: provided host argument is empty'
         print_err(msg)
         logging.error(msg)
         return None
     if not port or not str(port).isdigit() or abs(int(port)) > 65535:
         msg = 'wb_create:: provided port argument is empty, 0 or invalid integer'
         print_err(msg)
         logging.error(msg)
         return None
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     port = str(abs(int(port)))  # make sure the port argument is positive
 
     QUEUE_SIZE = int(128)  # maximum length of the queue that holds incoming messages
     MSG_SIZE = None  # int(20 * 1024 * 1024)  # maximum size for incoming messages in bytes. The default value is 1 MiB. None disables the limit
     PING_TIMEOUT = int(os.getenv('ALIENPY_TIMEOUT', '20'))  # If the corresponding Pong frame isn’t received within ping_timeout seconds, the connection is considered unusable and is closed
     PING_INTERVAL = PING_TIMEOUT  # Ping frame is sent every ping_interval seconds
     CLOSE_TIMEOUT = int(10)  # maximum wait time in seconds for completing the closing handshake and terminating the TCP connection
@@ -78,49 +80,75 @@
         except Exception as e:
             msg = f'Could NOT establish connection (local socket) to {socket_filename}\n{e!r}'
             logging.error(msg)
             print_err(f'{msg}\nCheck the logfile: {DEBUG_FILE}')
             return None
     else:
         fHostWSUrl = f'wss://{host}:{port}{path}'  # conection url
-        ctx = create_ssl_context(use_usercert)  # will check validity of token and if invalid cert will be usercert
+
+        # create/refresh the definitions of cert files
+        certs_info = renewCredFilesInfo()
+
+        # Check the presence of user certs and bailout before anything else
+        if not certs_info.token_cert and not certs_info.user_cert:
+            print_err(f'No valid user certificate or token found!! check {DEBUG_FILE} for further information and contact the developer if the information is not clear.')
+            sys.exit(126)
+
+        try:
+            ctx = create_ssl_context(use_usercert,
+                                     user_cert = certs_info.user_cert, user_key = certs_info.user_key,
+                                     token_cert = certs_info.token_cert, token_key = certs_info.token_key)
+        except Exception as e:
+            msg = f'Could NOT create SSL context with cert files:\n{certs_info.user_cert} ; {certs_info.user_key}\n{certs_info.token_cert} ; {certs_info.token_key}\n{e!r}'
+            logging.error(msg)
+            print_err(f'{msg}\nCheck the logfile: {DEBUG_FILE}')
+            return None
+
+        if not ctx:
+            msg = f'Could NOT create SSL context with cert files:\n{certs_info.user_cert} ; {certs_info.user_key}\n{certs_info.token_cert} ; {certs_info.token_key}'
+            logging.error(msg)
+            print_err(f'{msg}\nCheck the logfile: {DEBUG_FILE}')
+            return None
+
         logging.info('Request connection to: %s:%s%s', host, port, path)
 
         socket_endpoint = None
         # https://async-stagger.readthedocs.io/en/latest/reference.html#async_stagger.create_connected_sock
         # AI_* flags --> https://linux.die.net/man/3/getaddrinfo
+        init_begin_socket = None
         try:
             if DEBUG:
                 logging.debug('TRY ENDPOINT: %s:%s', host, port)
-                init_begin = time.perf_counter()
+                init_begin_socket = time.perf_counter()
             if os.getenv('ALIENPY_NO_STAGGER'):
                 socket_endpoint = socket.create_connection((host, int(port)))
             else:
                 socket_endpoint = await async_stagger.create_connected_sock(host, int(port), async_dns = True, delay = 0, resolution_delay = 0.050, detailed_exceptions = True)
-            if DEBUG:
-                logging.debug('TCP SOCKET DELTA: %s ms', deltat_ms_perf(init_begin))
+            if init_begin_socket:
+                logging.debug('TCP SOCKET DELTA: %s ms', deltat_ms_perf(init_begin_socket))
         except Exception as e:
             msg = f'Could NOT establish connection (TCP socket) to {host}:{port}\n{e!r}'
             logging.error(msg)
             print_err(f'{msg}\nCheck the logfile: {DEBUG_FILE}')
             return None
 
         if socket_endpoint:
             socket_endpoint_addr = socket_endpoint.getpeername()[0]
             socket_endpoint_port = socket_endpoint.getpeername()[1]
             logging.info('GOT SOCKET TO: %s:%s', socket_endpoint_addr, socket_endpoint_port)
             try:
-                if DEBUG: init_begin = time.perf_counter()
+                init_begin_wb = None
+                if DEBUG: init_begin_wb = time.perf_counter()
                 wb = await wb_client.connect(fHostWSUrl, sock = socket_endpoint, server_hostname = host, ssl = ctx, extensions=[deflateFact],
                                              max_queue=QUEUE_SIZE, max_size=MSG_SIZE,
                                              ping_interval=PING_INTERVAL, ping_timeout=PING_TIMEOUT,
                                              close_timeout=CLOSE_TIMEOUT, extra_headers=headers_list)
 
-                if DEBUG:
-                    logging.debug('WEBSOCKET DELTA: %s ms', deltat_ms_perf(init_begin))
+                if init_begin_wb:
+                    logging.debug('WEBSOCKET DELTA: %s ms', deltat_ms_perf(init_begin_wb))
 
             except wb_exceptions.InvalidStatusCode as e:
                 msg = f'Invalid status code {e.status_code} connecting to {socket_endpoint_addr}:{socket_endpoint_port}\n{e!r}'
                 logging.error(msg)
                 print_err(f'{msg}\nCheck the logfile: {DEBUG_FILE}')
                 if int(e.status_code) == 401:
                     print_err('The status code indicate that your certificate is not authorized.\nCheck the correct certificate registration into ALICE VO')
@@ -134,15 +162,14 @@
         if wb: logging.info('CONNECTED: %s:%s', wb.remote_address[0], wb.remote_address[1])
     return wb
 
 
 @syncify
 async def IsWbConnected(wb) -> bool:
     """Check if websocket is connected with the protocol ping/pong"""
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     time_begin = time.perf_counter() if DEBUG_TIMING else None
     if DEBUG:
         logging.info('Called from: %s', sys._getframe().f_back.f_code.co_name)  # pylint: disable=protected-access
     try:
         pong_waiter = await wb.ping()
         await pong_waiter
     except Exception:
```

### Comparing `alienpy-1.5.0/alienpy/xrd_core.py` & `alienpy-1.5.1/alienpy/xrd_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 '''alienpy:: XRootD mechanics'''
 
 import datetime
 import sys
-import xml.dom.minidom as MD  # nosec B408:blacklist
 import zipfile
 import traceback
 from urllib.parse import urlparse
+import logging
+import shlex
+import subprocess
+import uuid
+import time
+import xml.dom.minidom as MD  # nosec B408:blacklist
+from typing import Union
+
 from .global_vars import *  # nosec PYL-W0614
-from .data_structs import *  # nosec PYL-W0614
-from .version import *  # nosec PYL-W0614
-from .tools_files import *  # nosec PYL-W0614
-from .xrd_tools import *  # nosec PYL-W0614
-from .tools_misc import *  # nosec PYL-W0614
 from .setup_logging import print_out, print_err
-from .tools_shell import runShellCMD
+# from .tools_shell import runShellCMD
+from .wb_api import retf_print, SendMsg
+from .tools_nowb import (path_local_stat, path_writable_any, common_path,
+                         format_dst_fn, fileIsValid, create_metafile,
+                         make_tmp_fn, get_hash_meta, list_files_local, md5, get_size_meta, get_lfn_name,
+                         is_help, get_arg, get_arg_value, valid_regex, get_lfn_key, is_int, name2regex,
+                         fileline2list, PrintColor, GetHumanReadableSize, deltat_ms_perf, now_str)
+from .xrd_tools import path_type, pathtype_grid, expand_path_grid, path_grid_stat, lfn2fileTokens, extract_glob_pattern, list_files_grid, xrdcp_help, commitFileList
+
 
 HAS_XROOTD = False
 try:
     from XRootD import client as xrd_client  # type: ignore
     HAS_XROOTD = True
 except Exception:
     print("XRootD module could not be imported! Not fatal, but XRootD transfers will not work (or any kind of file access)\n Make sure you can do:\npython3 -c 'from XRootD import client as xrd_client'", file = sys.stderr, flush = True)
 
 
 def _is_valid_xrootd() -> bool:
     if not HAS_XROOTD: return False
     xrd_ver_arr = xrd_client.__version__.split(".")
+    _XRDVER_1 = _XRDVER_2 = None
     if len(xrd_ver_arr) > 1:
         _XRDVER_1 = xrd_ver_arr[0][1:] if xrd_ver_arr[0].startswith('v') else xrd_ver_arr[0]  # take out the v if present
         _XRDVER_2 = xrd_ver_arr[1]
         return int(_XRDVER_1) >= 5 and int(_XRDVER_2) > 2
 
     # version is not of x.y.z form, this is git based form
     xrdver_git = xrd_ver_arr[0].split("-")
@@ -56,15 +67,14 @@
         return val  # noqa: R504
 
     # Override the application name reported to the xrootd server.
     XRD_EnvPut('XRD_APPNAME', f'alien.py/{ALIENPY_VERSION_STR} xrootd/{xrd_client.__version__}')
     HAS_XROOTD_GETDEFAULT = hasattr(xrd_client, 'EnvGetDefault')
 
 
-
 def xrd_config_init():
     """Initialize generic XRootD client vars/timeouts"""
     if not HAS_XROOTD: return
     # xrdcp parameters (used by ALICE tests)
     # http://xrootd.org/doc/man/xrdcp.1.html
     # https://xrootd.slac.stanford.edu/doc/xrdcl-docs/www/xrdcldocs.html#x1-100004.2
     # xrootd defaults https://github.com/xrootd/xrootd/blob/master/src/XrdCl/XrdClConstants.hh
@@ -170,16 +180,16 @@
         if not dst.endswith('/'): dst = f"{dst}/"  # if src is dir, dst must be dir
 
     isSrcDir = (src_stat.type == 'd')
     if isSrcDir and not src_glob and not slashend_src: parent = parent + 1  # cp/rsync convention: with / copy the contents, without it copy the actual dir
 
     # prepare destination locations
     if isDownload:
+        mk_path = Path(dst) if dst.endswith('/') else Path(dst).parent  # if destination is file create it dir parent
         try:  # we can try anyway, this is like mkdir -p
-            mk_path = Path(dst) if dst.endswith('/') else Path(dst).parent  # if destination is file create it dir parent
             mk_path.mkdir(parents=True, exist_ok=True)
         except Exception:
             logging.error(traceback.format_exc())
             msg = f"Could not create local destination directory: {mk_path.as_posix()}\ncheck log file {DEBUG_FILE}"
             return RET(42, '', msg)  # ENOMSG /* No message of desired type */
     else:  # this is upload to GRID
         mk_path = dst if dst.endswith('/') else Path(dst).parent.as_posix()
@@ -216,15 +226,15 @@
 
             for lfn_obj in results_list.ansdict["results"]:  # make CopyFile objs for each lfn
                 lfn = get_lfn_key(lfn_obj)
                 dst_filename = format_dst_fn(src, lfn, dst, parent)
                 # if overwrite the file validity checking will do md5
                 skip_file = (retf_print(fileIsValid(dst_filename, lfn_obj['size'], lfn_obj['md5'], shallow_check = not overwrite), opts = 'noerr') == 0)
                 if skip_file: continue  # destination exists and is valid, no point to re-download
-                
+
                 tokens = lfn2fileTokens(wb, lfn2file(lfn, dst_filename), specs_list, isWrite, strictspec, httpurl)
                 if not tokens or 'answer' not in tokens: continue
                 copy_list.append(CopyFile(lfn, dst_filename, isWrite, tokens['answer'], lfn))
 
     else:  # src is LOCAL, we are UPLOADING
         results_list = list_files_local(src, pattern, is_regex, " ".join(find_args))
         if "results" not in results_list.ansdict or len(results_list.ansdict["results"]) < 1:
@@ -288,31 +298,30 @@
 
 
 def DO_XrootdCp(wb, xrd_copy_command: Union[None, list] = None, printout: str = '', api_src: Union[None, list] = None, api_dst: Union[None, list] = None) -> RET:
     """XRootD cp function :: process list of arguments for a xrootd copy command"""
     if not HAS_XROOTD: return RET(1, "", 'DO_XrootdCp:: python XRootD module not found or lower than 5.3.3, the copy process cannot continue')
 
     if xrd_copy_command is None: xrd_copy_command = []
-    if api_src is None: api_src =[]
-    if api_dst is None: api_dst =[]
+    if api_src is None: api_src = []
+    if api_dst is None: api_dst = []
 
     if bool(api_src) ^ bool(api_dst): return RET(1, '', 'API _src,_dst used but only one is defined')
     if len(api_src) != len(api_dst): return RET(1, '', 'API _src,_dst used but not of equal lenght')
 
     if not wb: return RET(107, "", 'DO_XrootdCp:: websocket not found')  # ENOTCONN /* Transport endpoint is not connected */
 
     if is_help(xrd_copy_command):
         help_msg = xrdcp_help()
         return RET(0, help_msg)
 
     if (not api_src) and (len(xrd_copy_command) < 2):
         help_msg = xrdcp_help()
         return RET(22, '', f'\n{help_msg}')  # 22 /* Invalid argument */
 
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
     xrd_config_init()  # reset XRootD preferences to cp oriented settings
 
     # XRootD copy parameters
     # inittimeout: copy initialization timeout(int)
     # tpctimeout: timeout for a third-party copy to finish(int)
     # coerce: ignore file usage rules, i.e. apply `FORCE` flag to open() (bool)
     # :param checksummode: checksum mode to be used #:type    checksummode: string
@@ -376,23 +385,23 @@
         retry = abs(int(retry_arg))
         XRD_EnvPut('CpRetry', retry)
 
     _use_system_xrdcp = get_arg(xrd_copy_command, '-xrdcp')
     f_arg = get_arg(xrd_copy_command, '-f')
     if f_arg:
         print_out('No longer used flag! md5 verification of present destination is default; disable with -fastcheck')
-    
+
     fastcheck = get_arg(xrd_copy_command, '-fastcheck')
-    overwrite = not fastcheck 
-    
+    overwrite = not fastcheck
+
     get_arg(xrd_copy_command, '-cksum')
     cksum = True
- 
+
     dryrun = get_arg(xrd_copy_command, '-dryrun')
- 
+
     tpc = 'none'
     if get_arg(xrd_copy_command, '-tpc'): tpc = 'first'
     if tpc != 'none': return RET(1, "", 'DO_XrootdCp:: TPC is not allowed!!')
 
     y_arg_val = get_arg_value(xrd_copy_command, '-y')
     # sources = int(y_arg_val)
     if y_arg_val: print_out("Ignored option! multiple source usage is known to break the files stored in zip files, so better to be ignored")
@@ -509,38 +518,50 @@
     inputfile_arg = get_arg_value(xrd_copy_command, '-input')  # input file with <source, destination> pairs
 
     # Start of resolving src to dst pairs
     copy_lfnlist = []  # list of lfn copy tasks
 
     if api_src and api_dst:
         for src,dst in zip(api_src, api_dst):
-            retobj = makelist_lfn(wb, src, dst, find_args = find_args, parent = parent, overwrite = overwrite, pattern = pattern, is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
+            retobj = makelist_lfn(wb, arg_source = src, arg_target = dst,
+                                  find_args = find_args, parent = parent,
+                                  overwrite = overwrite, pattern = pattern,
+                                  is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
             if retobj.exitcode != 0: print_err(retobj.err)  # if any error let's just return what we got  # noqa: R504
     elif inputfile_arg:
         cp_arg_list = fileline2list(inputfile_arg)
         if not cp_arg_list: return RET(1, '', f'Input file {inputfile_arg} not found or invalid content')
         for cp_line in cp_arg_list:
             cp_line_items = cp_line.strip().split()
             if len(cp_line_items) > 2:
                 print_out(f'Line skipped, it has more than 2 arguments => f{cp_line.strip()}')
                 continue
-            retobj = makelist_lfn(wb, cp_line_items[0], cp_line_items[1], find_args, parent, overwrite, pattern, use_regex, copy_lfnlist, strictspec, httpurl)
+            retobj = makelist_lfn(wb, arg_source = cp_line_items[0], arg_target = cp_line_items[1],
+                                  find_args = find_args, parent = parent,
+                                  overwrite = overwrite, pattern = pattern,
+                                  is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
             retf_print(retobj, "noout err")  # print error and continue with the other files
     elif dst_arg_specified:
-            # the assumption is that every argument from arg list was removed and what remain is a list of sources
-            common_root_path = common_path(xrd_copy_command)
-            for src in xrd_copy_command:
-                retobj = makelist_lfn(wb, src, f'{dst_arg_specified}/{src.replace(common_root_path, "")}', find_args = find_args, parent = parent, overwrite = overwrite, pattern = pattern, is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
-                if retobj.exitcode != 0: print_err(retobj.err)  # if any error let's just return what we got  # noqa: R504
+        # the assumption is that every argument from arg list was removed and what remain is a list of sources
+        common_root_path = common_path(xrd_copy_command)
+        for src in xrd_copy_command:
+            retobj = makelist_lfn(wb, arg_source = src, arg_target = f'{dst_arg_specified}/{src.replace(common_root_path, "")}',
+                                  find_args = find_args, parent = parent,
+                                  overwrite = overwrite, pattern = pattern,
+                                  is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
+            if retobj.exitcode != 0: print_err(retobj.err)  # if any error let's just return what we got  # noqa: R504
     else:
         if len(xrd_copy_command) < 2:
-            return RET(1, '', 'Argument list invalid (less then 2 arguments)')    
+            return RET(1, '', 'Argument list invalid (less then 2 arguments)')
         src = xrd_copy_command[-2]
         dst = xrd_copy_command[-1]
-        retobj = makelist_lfn(wb, src, dst, find_args = find_args, parent = parent, overwrite = overwrite, pattern = pattern, is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
+        retobj = makelist_lfn(wb, arg_source = src, arg_target = dst,
+                              find_args = find_args, parent = parent,
+                              overwrite = overwrite, pattern = pattern,
+                              is_regex = use_regex, strictspec = strictspec, httpurl = httpurl, copy_list = copy_lfnlist)
         if retobj.exitcode != 0: return retobj  # if any error let's just return what we got  # noqa: R504
 
     # at this point if any errors, the processing was already stopped
     if not copy_lfnlist: return RET(0, 'No copy jobs to be done!')
 
     if DEBUG:
         logging.debug("We are going to copy these files:")
@@ -569,15 +590,15 @@
     msg1 = msg2 = msg3 = msg_sum = ''
     copy_jobs_nr = copy_jobs_nr1 = copy_jobs_nr2 = 0
     copy_jobs_failed_nr = copy_jobs_failed_nr1 = copy_jobs_failed_nr2 = 0
     copy_jobs_success_nr = copy_jobs_success_nr1 = copy_jobs_success_nr2 = 0
 
     my_cp_args = XrdCpArgs(overwrite, batch, tpc, hashtype, cksum, timeout, rate)
     # defer the list of url and files to xrootd processing - actual XRootD copy takes place
-    copy_failed_list = XrdCopy(wb, xrdcopy_job_list, my_cp_args, printout) if not _use_system_xrdcp else XrdCopy_xrdcp(xrdcopy_job_list, my_cp_args)
+    copy_failed_list = XrdCopy(wb, xrdcopy_job_list, my_cp_args, printout)  # if not _use_system_xrdcp else XrdCopy_xrdcp(xrdcopy_job_list, my_cp_args)
     copy_jobs_nr = len(xrdcopy_job_list)
     copy_jobs_failed_nr = len(copy_failed_list)
     copy_jobs_success_nr = copy_jobs_nr - copy_jobs_failed_nr
     msg1 = f"Succesful jobs (1st try): {copy_jobs_success_nr}/{copy_jobs_nr}" if not ('quiet' in printout or 'silent' in printout) else ''
 
     copy_failed_list2 = []
     if copy_failed_list:
@@ -599,15 +620,15 @@
             tokens_retry1 = lfn2fileTokens(wb, lfn2file(job_lfn, job_file), specs_list, job_isWrite, strictspec, httpurl)
             if not tokens_retry1 or 'answer' not in tokens_retry1: continue
             to_recover_list_try1.append(CopyFile(job_file, job_lfn, job_isWrite, tokens_retry1['answer'], job_lfn))
 
         if to_recover_list_try1:
             xrdcopy_job_list_2 = []
             makelist_xrdjobs(to_recover_list_try1, xrdcopy_job_list_2)
-            copy_failed_list2 = XrdCopy(wb, xrdcopy_job_list_2, my_cp_args, printout)
+            copy_failed_list2 = XrdCopy(wb, xrdcopy_job_list_2, my_cp_args, printout)  # if not _use_system_xrdcp else XrdCopy_xrdcp(xrdcopy_job_list_2, my_cp_args)
             copy_jobs_nr1 = len(xrdcopy_job_list_2)
             copy_jobs_failed_nr1 = len(copy_failed_list2)
             copy_jobs_success_nr1 = copy_jobs_nr1 - copy_jobs_failed_nr1
             msg2 = f"Succesful jobs (2nd try): {copy_jobs_success_nr1}/{copy_jobs_nr1}" if not ('quiet' in printout or 'silent' in printout) else ''
 
     copy_failed_list3 = []
     if copy_failed_list2:
@@ -623,21 +644,21 @@
             excluded_SEs = ','.join(set(excluded_SEs_list))  # exclude already used SEs
             specs_list = f'disk:{failed_replica_nr},{excluded_SEs}'  # request N replicas (in place of failed ones), and exclude anything used
 
             job_file = failed_lfn_copy_jobs2[0].token_request['file']
             job_lfn = failed_lfn_copy_jobs2[0].token_request['lfn']
             job_isWrite = failed_lfn_copy_jobs2[0].isUpload
             tokens_retry2 = lfn2fileTokens(wb, lfn2file(job_lfn, job_file), specs_list, job_isWrite, strictspec, httpurl)
-            if not tokens_retry2 or 'answer' not in tokens_retry1: continue
+            if not tokens_retry2 or 'answer' not in tokens_retry2: continue
             to_recover_list_try2.append(CopyFile(job_file, job_lfn, job_isWrite, tokens_retry2['answer'], job_lfn))
 
         if to_recover_list_try2:
             xrdcopy_job_list_3 = []
             makelist_xrdjobs(to_recover_list_try2, xrdcopy_job_list_3)
-            copy_failed_list3 = XrdCopy(wb, xrdcopy_job_list_3, my_cp_args, printout)
+            copy_failed_list3 = XrdCopy(wb, xrdcopy_job_list_3, my_cp_args, printout)  # if not _use_system_xrdcp else XrdCopy_xrdcp(xrdcopy_job_list_3, my_cp_args)
             copy_jobs_nr2 = len(xrdcopy_job_list_3)
             copy_jobs_failed_nr2 = len(copy_failed_list3)
             copy_jobs_success_nr2 = copy_jobs_nr2 - copy_jobs_failed_nr2
             msg3 = f'Succesful jobs (3rd try): {copy_jobs_success_nr2}/{copy_jobs_nr2}' if not ('quiet' in printout or 'silent' in printout) else ''
 
     # copy_jobs_failed_total = copy_jobs_failed_nr + copy_jobs_failed_nr1 + copy_jobs_failed_nr2
     copy_jobs_nr_total = copy_jobs_nr + copy_jobs_nr1 + copy_jobs_nr2
@@ -792,22 +813,25 @@
     if DEBUG: handler.debug = True
 
     process = xrd_client.CopyProcess()
     process.parallel(int(batch))
     for copy_job in job_list:
         if DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
         if copy_job.isUpload:
-            cksum_mode = 'source'; cksum_type = 'md5' ; cksum_preset = ''; # copy_job.token_request['md5']
+            cksum_mode = 'source'
+            cksum_type = 'md5'
+            cksum_preset = ''
         else:  # for downloads we already have the md5 value, lets use that
-            cksum_mode = 'target';
+            cksum_mode = 'target'
             cksum_type, cksum_preset = get_hash_meta(copy_job.src)
             # If the remote file had no hash registered
             if not cksum_type or not cksum_preset:
-                logging.error(f'COPY:: MD5 missing for {copy_job.lfn}')
-                cksum_mode = 'none'; cksum_type = cksum_preset = '';
+                logging.error('COPY:: MD5 missing for %s', copy_job.lfn)
+                cksum_mode = 'none'
+                cksum_type = cksum_preset = ''
 
         delete_invalid_cksum = (not cksum_mode == 'none')  # if no checksumming mode, disable rmBadCksum
         if 'xrateThreshold' in process.add_job.__code__.co_varnames:
             process.add_job(copy_job.src, copy_job.dst, sourcelimit = sources, posc = posc, mkdir = makedir, force = overwrite, thirdparty = tpc,
                             checksummode = cksum_mode, checksumtype = cksum_type, checksumpreset = cksum_preset, rmBadCksum = delete_invalid_cksum,
                             retry = xrd_client.EnvGetInt('CpRetry'), cptimeout = xrd_client.EnvGetInt('CPTimeout'), xrateThreshold = xrd_client.EnvGetInt('XRateThreshold') )
         else:
@@ -824,60 +848,62 @@
 
     if handler.succesful_writes:  # if there were succesful uploads/remote writes, let's commit them to file catalogue
         ret_list = commitFileList(wb, handler.succesful_writes)
         for ret in ret_list: retf_print(ret, 'noout err')
     return handler.copy_failed_list  # lets see what failed and try to recover
 
 
-def _xrdcp_sysproc(cmdline: str, timeout: Union[str, int, None] = None) -> RET:
-    """xrdcp stanalone system command"""
-    if not cmdline: return RET(1, '', '_xrdcp_sysproc :: no cmdline')  # type: ignore [call-arg]
-    if timeout is not None: timeout = int(timeout)
-    # --nopbar --posc
-    xrdcp_cmdline = f'xrdcp -N -P {cmdline}'
-    return runShellCMD(xrdcp_cmdline, captureout = True, do_shell = False, timeout = timeout)
-
-
-def _xrdcp_copyjob(copy_job: CopyFile, xrd_cp_args: XrdCpArgs) -> int:  # , printout: str = ''
-    """xrdcp based task that process a copyfile and it's arguments"""
-    if not copy_job: return int(2)
-    # overwrite = xrd_cp_args.overwrite
-    # batch = xrd_cp_args.batch
-    # tpc = xrd_cp_args.tpc
-    # hashtype = xrd_cp_args.hashtype
-    # cksum = xrd_cp_args.cksum
-    timeout = xrd_cp_args.timeout
-    # rate = xrd_cp_args.rate
-    cmdline = f'{copy_job.src} {copy_job.dst}'
-    return retf_print(_xrdcp_sysproc(cmdline, timeout))
-
-
-def XrdCopy_xrdcp(job_list: list, xrd_cp_args: XrdCpArgs) -> list:  # , printout: str = ''
-    """XRootD copy command :: the actual XRootD copy process"""
-    if not HAS_XROOTD:
-        print_err("XRootD not found or lower version thant 5.3.3")
-        return []
-    if not xrd_cp_args:
-        print_err("cp arguments are not set, XrdCpArgs tuple missing")
-        return []
-    # overwrite = xrd_cp_args.overwrite
-    # batch = xrd_cp_args.batch
-    # makedir = xrd_cp_args.makedir
-
-    # ctx = mp.get_context('forkserver')
-    # q = ctx.JoinableQueue()
-    # p = ctx.Process(target=_xrdcp_copyjob, args=(q,))
-    # p.start()
-    # print(q.get())
-    # p.join()
-    for copy_job in job_list:
-        if DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
-        # xrdcp_cmd = f' {copy_job.src} {copy_job.dst}'
-        if DEBUG: print_out(copy_job)
-    return []
+# keep it commented until is needed - dead code for now
+# def _xrdcp_sysproc(cmdline: str, timeout: Union[str, int, None] = None) -> RET:
+#     """xrdcp stanalone system command"""
+#     if not cmdline: return RET(1, '', '_xrdcp_sysproc :: no cmdline')  # type: ignore [call-arg]
+#     if timeout is not None: timeout = int(timeout)
+#     # --nopbar --posc
+#     xrdcp_cmdline = f'xrdcp -N -P {cmdline}'
+#     return runShellCMD(xrdcp_cmdline, captureout = True, do_shell = False, timeout = timeout)
+
+
+# keep it commented until is needed - dead code for now
+# def _xrdcp_copyjob(copy_job: CopyFile, xrd_cp_args: XrdCpArgs) -> int:  # , printout: str = ''
+#     """xrdcp based task that process a copyfile and it's arguments"""
+#     if not copy_job: return int(2)
+#     # overwrite = xrd_cp_args.overwrite
+#     # batch = xrd_cp_args.batch
+#     # tpc = xrd_cp_args.tpc
+#     # hashtype = xrd_cp_args.hashtype
+#     # cksum = xrd_cp_args.cksum
+#     timeout = xrd_cp_args.timeout
+#     # rate = xrd_cp_args.rate
+#     cmdline = f'{copy_job.src} {copy_job.dst}'
+#     return retf_print(_xrdcp_sysproc(cmdline, timeout))
+
+# keep it commented until is needed - dead code for now
+# def XrdCopy_xrdcp(job_list: list, xrd_cp_args: XrdCpArgs) -> list:  # , printout: str = ''
+#     """XRootD copy command :: the actual XRootD copy process"""
+#     if not HAS_XROOTD:
+#         print_err("XRootD not found or lower version thant 5.3.3")
+#         return []
+#     if not xrd_cp_args:
+#         print_err("cp arguments are not set, XrdCpArgs tuple missing")
+#         return []
+#     # overwrite = xrd_cp_args.overwrite
+#     # batch = xrd_cp_args.batch
+#     # makedir = xrd_cp_args.makedir
+#
+#     # ctx = mp.get_context('forkserver')
+#     # q = ctx.JoinableQueue()
+#     # p = ctx.Process(target=_xrdcp_copyjob, args=(q,))
+#     # p.start()
+#     # print(q.get())
+#     # p.join()
+#     for copy_job in job_list:
+#         if DEBUG: logging.debug('\nadd copy job with\nsrc: %s\ndst: %s\n', copy_job.src, copy_job.dst)
+#         # xrdcp_cmd = f' {copy_job.src} {copy_job.dst}'
+#         if DEBUG: print_out(copy_job)
+#     return []
 
 
 def xrd_response2dict(response_status) -> dict:
     """Convert a XRootD response status answer to a dict"""
     if not response_status: return {}
     if not HAS_XROOTD:
         print_err('XRootD not present')
@@ -939,16 +965,14 @@
         print_err(f'xrdfs_q_stats:: query error to {fqdn_port} : {status["message"]}')
         return ''
 
     response = response.decode('ascii').strip().strip('\x00')
     # if xml is requested or xmltodict missing
     if xml:
         if xml_raw: return response
-        # xml_stats = ET.fromstring(response)
-        # return ET.dump(xml_stats)
         xml_stats = MD.parseString(response)  # nosec B318:blacklist
         indent = '  '
         newl = '\n'
         if compact: indent = newl = ''
         return xml_stats.toprettyxml(indent = indent, newl = newl).replace('&quot;', '"')
 
     try:
```

### Comparing `alienpy-1.5.0/alienpy/xrd_tools.py` & `alienpy-1.5.1/alienpy/xrd_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 '''alienpy:: XRootD related tooling/helpers'''
 
 import os
+import subprocess
+import shlex
+from typing import Union
+
 from .global_vars import *  # nosec PYL-W0614
-from .data_structs import *  # nosec PYL-W0614
-from .tools_files import *  # nosec PYL-W0614
-from .wb_api import *  # nosec PYL-W0614
+from .setup_logging import print_err
+from .wb_api import SendMsg, SendMsgMulti, CreateJsonCommand, retf_print
+from .tools_nowb import get_arg, PrintColor, create_metafile, make_tmp_fn, valid_regex, get_arg_value, get_lfn_key, filter_file_prop
 
 
 def lfnAccessUrl(wb, lfn: str, local_file: str = '', specs: Union[None, list, str] = None, isWrite: bool = False, strictspec: bool = False, httpurl: bool = False) -> dict:
     """Query central services for the access envelope of a lfn, it will return a lfn:server answer with envelope pairs"""
     if not wb: return {}
     if not lfn: return {}
     if not specs: specs = []
     if specs and isinstance(specs, str): specs = specs_split.split(specs)
     if isWrite:
         if not local_file or not os.path.exists(local_file):
             print_err(f'lfnAccessUrl/write token:: invalid local file: {local_file}')
             return {}
         access_type = 'write'
         size = int(os.stat(local_file).st_size)
-        md5sum = '' # md5(local_file)
+        md5sum = ''  # md5(local_file)
         files_with_default_replicas = ['.sh', '.C', '.jdl', '.xml']
         if any(lfn.endswith(ext) for ext in files_with_default_replicas) and size < 1048576 and not specs:  # we have a special lfn
             specs.append('disk:4')  # and no specs defined then default to disk:4
         get_envelope_arg_list = ['-s', size, '-m', md5sum, access_type, lfn]
         if not specs: specs.append('disk:2')  # hard default if nothing is specified
     else:
         access_type = 'read'
@@ -154,14 +158,16 @@
 
 
 def xrdcp_help() -> str:
     return f'''Command format is of the form of (with the strict order of arguments):
         cp <options> src dst
         or
         cp <options> -input input_file
+        or
+        cp <options> -dst dest_dir file1 file2 ... fileN
 where src|dst are local files if prefixed with file:// or file: or grid files otherwise
 and -input argument is a file with >src dst< pairs
 after each src,dst can be added comma separated specifiers list in the form of: @<QOS>:N,SE1,SE2,!SE3
 QOS is a tag of the storage element (usually "disk") followed by the N requested replicas
 Additional replicas can be requested by the name of storage elements. (additional to QOS specifications),
 or exclusion of storages (prefixing with exclamation mark).
 %ALIEN alias have the special meaning of AliEn user home directory
@@ -245,15 +251,14 @@
 
 
 def list_files_grid(wb, search_dir: str, pattern: Union[None, REGEX_PATTERN_TYPE, str] = None, is_regex: bool = False, find_args: Union[str, list, None] = None) -> RET:
     """Return a list of files(lfn/grid files) that match pattern found in search_dir
     Returns a RET object (from find), and takes: wb, directory, pattern, is_regex, find_args
     """
     if not search_dir: return RET(-1, "", "No search directory specified")
-    DEBUG = os.getenv('ALIENPY_DEBUG', '')
 
     if find_args is None: find_args = []
     find_args_list = find_args.split() if isinstance(find_args, str) else find_args.copy()
 
     # lets process the pattern: extract it from src if is in the path globbing form
     is_single_file = False  # dir actually point to a file
 
@@ -435,12 +440,11 @@
 
 def path_type(path_arg: str) -> tuple:
     """Check if path is local or grid; default is grid and local must have file: prefix"""
     location = 'local' if path_arg.startswith('file:') else 'grid'
     return (path_arg, location)
 
 
-
 if __name__ == '__main__':
     print('This file should not be executed!', file = sys.stderr, flush = True)
     sys.exit(95)
```

### Comparing `alienpy-1.5.0/alienpy.egg-info/PKG-INFO` & `alienpy-1.5.1/alienpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alienpy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Websocket based cli interface for ALICE experiment GRID infrastructure
 Home-page: https://gitlab.cern.ch/jalien/xjalienfs
 Author: Adrian Sevcenco
 Author-email: adrian.sevcenco@cern.ch
 Project-URL: Dev git, https://github.com/adriansev/jalien_py
 Project-URL: Issues, https://github.com/adriansev/jalien_py/issues
 Project-URL: Changelog, https://github.com/adriansev/jalien_py/commits/master
```

### Comparing `alienpy-1.5.0/alienpy.egg-info/SOURCES.txt` & `alienpy-1.5.1/alienpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 alienpy/alien.py
 alienpy/async_tools.py
 alienpy/connect_ssl.py
 alienpy/data_structs.py
 alienpy/global_vars.py
 alienpy/setup_cwd.py
 alienpy/setup_logging.py
-alienpy/tools_files.py
-alienpy/tools_misc.py
+alienpy/tools_history.py
+alienpy/tools_nowb.py
 alienpy/tools_shell.py
 alienpy/tools_stackcmd.py
 alienpy/version.py
 alienpy/wb_api.py
 alienpy/wb_async.py
 alienpy/xrd_core.py
 alienpy/xrd_tools.py
```

### Comparing `alienpy-1.5.0/alienpy.egg-info/entry_points.txt` & `alienpy-1.5.1/alienpy.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 alien-token-info = alienpy.alien:cmd_token_info
 alien-token-init = alienpy.alien:cmd_token_init
 alien.py = alienpy.alien:main
 alien_cmd = alienpy.alien:main
 alien_cp = alienpy.alien:main
 alien_find = alienpy.alien:main
 alien_guid2lfn = alienpy.alien:main
+alien_home = alienpy.alien:cmd_home
 alien_lfn2guid = alienpy.alien:main
 alien_ls = alienpy.alien:main
 alien_mirror = alienpy.alien:main
 alien_mkdir = alienpy.alien:main
 alien_mv = alienpy.alien:main
 alien_pfn = alienpy.alien:main
 alien_ps = alienpy.alien:main
+alien_pwd = alienpy.alien:main
 alien_rm = alienpy.alien:main
 alien_rmdir = alienpy.alien:main
 alien_stat = alienpy.alien:main
 alien_submit = alienpy.alien:main
 alien_whereis = alienpy.alien:main
```

### Comparing `alienpy-1.5.0/examples/alien_wbtime` & `alienpy-1.5.1/examples/alien_wbtime`

 * *Files identical despite different names*

### Comparing `alienpy-1.5.0/setup.py` & `alienpy-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import sys
 import setuptools
 import traceback
 
 
 try:
-    from alienpy.version import *  # nosec PYL-W0614
+    from alienpy.version import ALIENPY_VERSION_HASH, ALIENPY_VERSION_DATE, ALIENPY_VERSION_STR
 except Exception:
     try:
-        from xjalienfs.version import *  # nosec PYL-W0614
+        from xjalienfs.version import ALIENPY_VERSION_HASH, ALIENPY_VERSION_DATE, ALIENPY_VERSION_STR
     except Exception:
         traceback.print_exc()
         print('Failed to get version from file. Using 0.0.0')
         ALIENPY_VERSION_STR = '0.0.0'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
@@ -53,38 +53,37 @@
     project_urls = {
         "Dev git": "https://github.com/adriansev/jalien_py",
         "Issues": "https://github.com/adriansev/jalien_py/issues",
         "Changelog": "https://github.com/adriansev/jalien_py/commits/master",
         "Documentation": "https://jalien.docs.cern.ch",
         "CERN Mattermost/JAliEn": "https://mattermost.web.cern.ch/alice/channels/jalien",
         },
-    entry_points = {
-        'console_scripts': [
-            'alien.py = alienpy.alien:main',
-            'alien_cmd = alienpy.alien:main',
-            'alien_cp = alienpy.alien:main',
-            'alien_find = alienpy.alien:main',
-            'alien_guid2lfn = alienpy.alien:main',
-            'alien_lfn2guid = alienpy.alien:main',
-            'alien_ls = alienpy.alien:main',
-            'alien_mirror = alienpy.alien:main',
-            'alien_mkdir = alienpy.alien:main',
-            'alien_mv = alienpy.alien:main',
-            'alien_pfn = alienpy.alien:main',
-            'alien_ps = alienpy.alien:main',
-            'alien_rm = alienpy.alien:main',
-            'alien_rmdir = alienpy.alien:main',
-            'alien_stat = alienpy.alien:main',
-            'alien_submit = alienpy.alien:main',
-            'alien_whereis = alienpy.alien:main',
-            'alien-cert-info = alienpy.alien:cmd_cert_info',
-            'alien-token-info = alienpy.alien:cmd_token_info',
-            'alien-token-init = alienpy.alien:cmd_token_init',
-            'alien-token-destroy = alienpy.alien:cmd_token_destroy',
-            ]
-        },
-    scripts = [
-        'examples/alien_wbtime',
-        ],
+    entry_points = {'console_scripts': [
+                                       'alien.py = alienpy.alien:main',
+                                       'alien_cmd = alienpy.alien:main',
+                                       'alien_cp = alienpy.alien:main',
+                                       'alien_find = alienpy.alien:main',
+                                       'alien_guid2lfn = alienpy.alien:main',
+                                       'alien_lfn2guid = alienpy.alien:main',
+                                       'alien_ls = alienpy.alien:main',
+                                       'alien_mirror = alienpy.alien:main',
+                                       'alien_mkdir = alienpy.alien:main',
+                                       'alien_mv = alienpy.alien:main',
+                                       'alien_pfn = alienpy.alien:main',
+                                       'alien_ps = alienpy.alien:main',
+                                       'alien_pwd = alienpy.alien:main',
+                                       'alien_rm = alienpy.alien:main',
+                                       'alien_rmdir = alienpy.alien:main',
+                                       'alien_stat = alienpy.alien:main',
+                                       'alien_submit = alienpy.alien:main',
+                                       'alien_whereis = alienpy.alien:main',
+                                       'alien-cert-info = alienpy.alien:cmd_cert_info',
+                                       'alien-token-info = alienpy.alien:cmd_token_info',
+                                       'alien-token-init = alienpy.alien:cmd_token_init',
+                                       'alien-token-destroy = alienpy.alien:cmd_token_destroy',
+                                       'alien_home = alienpy.alien:cmd_home'
+                                       ]
+                    },
+    scripts = [ 'examples/alien_wbtime', ],
     keywords = 'CERN ALICE JAliEn GRID',
 )
```

