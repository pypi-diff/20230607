# Comparing `tmp/ssh-hosts-0.3.2.tar.gz` & `tmp/ssh-hosts-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh-hosts-0.3.2.tar", last modified: Mon Apr 10 17:22:02 2023, max compression
+gzip compressed data, was "ssh-hosts-0.4.0.tar", last modified: Wed Jun  7 18:51:20 2023, max compression
```

## Comparing `ssh-hosts-0.3.2.tar` & `ssh-hosts-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.158801 ssh-hosts-0.3.2/
--rw-rw-rw-   0        0        0     1100 2023-02-02 18:07:15.000000 ssh-hosts-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3802 2023-04-10 17:22:02.158801 ssh-hosts-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3084 2023-04-10 17:16:13.000000 ssh-hosts-0.3.2/README.md
--rw-rw-rw-   0        0        0      858 2023-04-10 17:16:10.000000 ssh-hosts-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 17:22:02.158801 ssh-hosts-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-02 18:07:15.000000 ssh-hosts-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.095526 ssh-hosts-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.143171 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/
--rw-rw-rw-   0        0        0     3802 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 17:22:02.000000 ssh-hosts-0.3.2/src/ssh_hosts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 17:22:02.143171 ssh-hosts-0.3.2/src/sshhosts/
--rw-rw-rw-   0        0        0        0 2023-02-02 18:07:15.000000 ssh-hosts-0.3.2/src/sshhosts/__init__.py
--rw-rw-rw-   0        0        0     9189 2023-04-10 17:16:17.000000 ssh-hosts-0.3.2/src/sshhosts/sshhosts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 18:51:20.868024 ssh-hosts-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-06-07 18:50:45.000000 ssh-hosts-0.4.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-07 18:51:20.868024 ssh-hosts-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3226 2023-06-07 18:50:45.000000 ssh-hosts-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-07 18:50:45.000000 ssh-hosts-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 18:51:20.868024 ssh-hosts-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-07 18:50:45.000000 ssh-hosts-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 18:51:20.865024 ssh-hosts-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 18:51:20.867025 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-07 18:51:20.000000 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-07 18:51:20.000000 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 18:51:20.000000 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-07 18:51:20.000000 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-07 18:51:20.000000 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-07 18:51:20.000000 ssh-hosts-0.4.0/src/ssh_hosts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 18:51:20.868024 ssh-hosts-0.4.0/src/sshhosts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 18:50:45.000000 ssh-hosts-0.4.0/src/sshhosts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10647 2023-06-07 18:50:45.000000 ssh-hosts-0.4.0/src/sshhosts/sshhosts.py
```

### Comparing `ssh-hosts-0.3.2/LICENSE.txt` & `ssh-hosts-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssh-hosts-0.3.2/README.md` & `ssh-hosts-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # SSH-Hosts
 
-Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one of them. This is handy if you organize a bunch of host entries in your SSH client config like, e.g.:
+Simple script to list all host entries in your SSH configuration. You can then choose to quickly connect to one or more of them. This is handy if you organize a bunch of host entries in your SSH client config like, e.g.:
 
 ```
+# Including files is also supported
+Include /path/to/my/other/config/file
+
 Host foo
   Hostname foohost
   User foouser
   IdentityFile fookey
 
 Host bar
   Hostname barhost
   User baruser
   IdentityFile barkey
 ```
 
-Note: It is also possible to use wildcards in your SSH client config to set values for multiple hosts at once. This script will *not* show these entries, since they cannot be used to connect to a host directly.
+Notes:
+
+* It is also possible to use wildcards in your SSH client config to set values for multiple hosts at once. This script will *not* show these entries, since they cannot be used to connect to a host directly.
 
 ## Installation
 
   * Install from pypi: ```pip install ssh-hosts```
 
   OR
 
   * Download the pip package from GitLab
-  * Install it with pip, e.g. pip install sshhosts-0.3.2-py3-none-any.whl
+  * Install it with pip, e.g. pip install sshhosts-0.4.0-py3-none-any.whl
 
 ## Basic usage
 
 Just run
 ```
 ssh-hosts
 ```
@@ -47,14 +52,15 @@
                         SSH command
   -l, --loop            Do not exit when ssh session ends, show host list again instead
   -t, --terminal_tab_mode
                         Attempt to start ssh session in new tab/window of terminal
   -o, --sort_host_entries
                         Sort host entries
   -r, --reverse_order   Reverse sorting order
+  -g, --gui             Use a curses-like input dialog
 ```
 
 ## Arguments
 
 ### Path to SSH configuration
 
 ```
```

### Comparing `ssh-hosts-0.3.2/pyproject.toml` & `ssh-hosts-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 [project]
 name = "ssh-hosts"
 description = "Quickly connect to host entries from your SSH config file"
 authors = [
     {name = "Christoph Stein" }
 ]
 requires-python = ">=3.9"
-version = "0.3.2"
+version = "0.4.0"
+dependencies = [
+    "Pygments==2.14.0",
+    "wcwidth==0.2.6",
+    "prompt-toolkit==3.0.38",
+]
 
 keywords = ["SSH", "Hosts", "Network"]
 readme = "README.md"
 #license = {file = "LICENSE.txt"}
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ssh-hosts-0.3.2/src/sshhosts/sshhosts.py` & `ssh-hosts-0.4.0/src/sshhosts/sshhosts.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 from os.path import expanduser
 from os import environ
 import platform
 import subprocess
 import logging
 import argparse
 import re
+from prompt_toolkit.shortcuts import checkboxlist_dialog
+from prompt_toolkit.styles import Style
 
 # ---- Argument parser ----
 def GetVersion() -> str:
-    return "0.3.2"
+    return "0.4.0"
 
 def GetArgParser() -> argparse.ArgumentParser:
     tArgParser = argparse.ArgumentParser(usage="%(prog)s [OPTIONS]",
                                          description="List and connect to host entries from your ssh configuration")
 
     tArgParser.add_argument("-v", "--version", action="version", version = f"{tArgParser.prog} version {GetVersion()}")
     tArgParser.add_argument("-c", "--config", help="Path to configuration file", type=str, default=None, required=False)
     tArgParser.add_argument("-e", "--exclude", help="Exclude hosts based on python regular expression", type=str, default=None, required=False)
     tArgParser.add_argument("-s", "--ssh_command", help="SSH command", type=str, default="ssh", required=False)
     tArgParser.add_argument("-l", "--loop", help="Do not exit when ssh session ends, show host list again instead", action="store_true")
     tArgParser.add_argument("-t", "--terminal_tab_mode", help="Attempt to start ssh session in new tab/window of terminal", action="store_true")
     tArgParser.add_argument("-o", "--sort_host_entries", help="Sort host entries", action="store_true")
     tArgParser.add_argument("-r", "--reverse_order", help="Reverse sorting order", action="store_true")
+    tArgParser.add_argument("-g", "--gui", help="Use a curses-like input dialog", action="store_true")
     return tArgParser
 
 # -- Logger setup ---
 def setuplogging():
     # Set application wide debug level and format
     #logging.basicConfig(format='%(asctime)s - %(levelname)s: %(message)s',
     logging.basicConfig(format='%(levelname)s: %(message)s',
@@ -94,44 +97,65 @@
         return True
 
     # -- Sort list --
     def SortHosts(self, ReverseOrder = False):
         self.FilteredHosts.sort(key = str.lower, reverse = ReverseOrder)
 
 class ConsoleFuncs:
+
+    Prompt_toolkit_style = {
+        'dialog': 'bg:#284A6B',
+        'button': 'bg:#e8612c',
+        'checkbox': '#073B6B',
+        'dialog shadow': 'bg:#073B6B',
+    }
+
     def __init__(self):
         self.Platform = platform.system().lower()
 
     # -- List strings and get choice from user ---
     @staticmethod
-    def PickChoice(ChoicesList, Prompt: str = "Choose: "):
-        Message = str()
-        for index, item in enumerate(ChoicesList):
-            Message += f'{index + 1}) {item}\n'
-        Message = Message.replace('"','') # Quotes not needed for display, looks a bit more clean
+    def PickChoice(ChoicesList, Prompt: str = "? ", Caption: str = "", Gui: bool = True):
+        if Gui:
+            # Use prompt toolkit to show a curses-like dialog
+            ChoicesToShow = list()
+            for index, item in enumerate(ChoicesList):
+                ChoicesToShow.append( (index, item) )
+            Results = checkboxlist_dialog(title=Prompt,
+                                          text=Caption,
+                                          values=ChoicesToShow,
+                                          style = Style.from_dict(ConsoleFuncs.Prompt_toolkit_style)
+                                          ).run()
+            return Results
+        else:
+            # Simple input: Show list and let user input a number
+            Message = str()
+            for index, item in enumerate(ChoicesList):
+                Message += f'{index + 1}) {item}\n'
+            Message = Message.replace('"','') # Quotes not needed for display, looks a bit more clean
 
-        try:
-            # User may input more than one number, separated by whitespaces.
-            # Thus: Split string, try to convert every substring into an integer and check
-            # if it is a valid index value. Return a list of valid choices.
-            Input = input(f'\n{Message}{Prompt}')
-            Choices = Input.split()
-            ChoicesChecked = []
-            for i in Choices:
-                try:
-                    if 0 < int(i) <= len(ChoicesList): ChoicesChecked.append(int(i) - 1)
-                except ValueError: pass # Ignore ValueError - those entries will not be added to the ChoicesChecked list because the exception hits before the 'append' happens. No need to take further action here.
-            return ChoicesChecked
-        except KeyboardInterrupt:
-            return []
+            try:
+                # User may input more than one number, separated by whitespaces.
+                # Thus: Split string, try to convert every substring into an integer and check
+                # if it is a valid index value. Return a list of valid choices.
+                Input = input(f'\n{Caption}\n{Message}{Prompt}')
+                Choices = Input.split()
+                ChoicesChecked = []
+                for i in Choices:
+                    try:
+                        if 0 < int(i) <= len(ChoicesList): ChoicesChecked.append(int(i) - 1)
+                    except ValueError: pass # Ignore ValueError - those entries will not be added to the ChoicesChecked list because the exception hits before the 'append' happens. No need to take further action here.
+                return ChoicesChecked
+            except KeyboardInterrupt:
+                return []
 
     # -- Clear console on supported platforms --
     def Clear(self):
-        if 'windows' in self.Platform: subprocess.run('cls',   shell = True)
-        if 'linux'   in self.Platform: subprocess.run('clear', shell = True)
+        if 'windows' in self.Platform: subprocess.run('cls',   shell = True, check = False)
+        if 'linux'   in self.Platform: subprocess.run('clear', shell = True, check = False)
         return
 
 # -- Get ssh config from users home directory if no path was supplied ---
 def GetHomeSSHConfigPath():
     return expanduser('~/.ssh/config')
 
 # -- Get commandline to start new ssh connection --
@@ -165,16 +189,21 @@
         return 1
     if len(ConfHosts.FilteredHosts) == 0:
         logging.info("No hosts, exit.")
         return 0
 
     # Let user choose a host and start ssh connection
     Console = ConsoleFuncs()
+    Caption_message = "Choose one or more hosts"
+    if not targs.ssh_command == 'ssh': Caption_message += f"\n(SSH command: \"{targs.ssh_command}\")"
     while True:
-        Choice = Console.PickChoice(ConfHosts.FilteredHosts, 'Connect to: ')
+        Choice = Console.PickChoice(ConfHosts.FilteredHosts,
+                                    'Connect to: ',
+                                    Caption_message,
+                                    targs.gui)
         if not Choice:  # Abort right away if list of choices is empty
             logging.info('Abort')
             return 0
         for i in Choice: # loop through list of chosen host indices, and run the ssh command for each one
             logging.info(f'Connecting to "{ConfHosts.FilteredHosts[i]}"')
             try:
                 Completed = subprocess.run(CommandLine(targs.ssh_command,
```

