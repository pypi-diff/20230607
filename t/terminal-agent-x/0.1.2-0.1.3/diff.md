# Comparing `tmp/terminal-agent-x-0.1.2.tar.gz` & `tmp/terminal-agent-x-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal-agent-x-0.1.2.tar", last modified: Tue May 30 03:21:18 2023, max compression
+gzip compressed data, was "terminal-agent-x-0.1.3.tar", last modified: Wed Jun  7 07:03:16 2023, max compression
```

## Comparing `terminal-agent-x-0.1.2.tar` & `terminal-agent-x-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3394 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2582 2023-05-30 03:17:04.000000 terminal-agent-x-0.1.2/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      914 2023-05-30 03:16:22.000000 terminal-agent-x-0.1.2/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/terminal_agent_x/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.2/terminal_agent_x/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5940 2023-05-30 03:06:35.000000 terminal-agent-x-0.1.2/terminal_agent_x/tax.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-30 03:21:18.426922 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3394 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      288 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-05-30 03:21:18.000000 terminal-agent-x-0.1.2/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3749 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2936 2023-06-07 07:01:35.000000 terminal-agent-x-0.1.3/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      915 2023-06-07 06:39:01.000000 terminal-agent-x-0.1.3/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/terminal_agent_x/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.3/terminal_agent_x/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5639 2023-06-07 06:56:18.000000 terminal-agent-x-0.1.3/terminal_agent_x/tax.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3749 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.3/tests/test.py
```

### Comparing `terminal-agent-x-0.1.2/LICENSE` & `terminal-agent-x-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal-agent-x-0.1.2/PKG-INFO` & `terminal-agent-x-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.2
+Version: 0.1.3
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -53,31 +53,28 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--default_url] [--claude] [--show_all] prompt [prompt ...]
+usage: tax [-h] [--key KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
 
-Description of your program
+Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
-  prompt                Prompt
+  prompt         Prompt
 
 options:
-  -h, --help            show this help message and exit
-  --openai_key OPENAI_KEY
-                        Your key for OpenAI, only for one-time request
-  --model MODEL         Model name. You can use all OpenAI models.
-  --file FILE           Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
-  --url URL             URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.
-  --default_url         Use default OpenAI API URL for request.
-  --claude              Use Claude API for request.
-  --show_all            Show all contents in the response
+  -h, --help     show this help message and exit
+  --key KEY      Your key for OpenAI//Claude, only for one-time request
+  --model MODEL  Model name. You can use all OpenAI models.
+  --file FILE    Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
+  --url URL      URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.
+  --show_all     Show all contents in the response
 ```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
 ## Attention
@@ -106,7 +103,23 @@
 <summary>0.1.1</summary>
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
 </details>
 
+<details>
+<summary>0.1.2</summary>
+
+- [WIP]Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
+- Add a timeout function.
+- Fix: C++ code block prefix.
+</details>
+
+<details>
+<summary>0.1.3</summary>
+
+- Fix: code block prefix bug (tax will act maybe a little faster).
+- Modify: simplify the code.
+- Test: test for multi-process. Now you can use tax more efficiently in terminal.
+</details>
```

### Comparing `terminal-agent-x-0.1.2/README.md` & `terminal-agent-x-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -34,31 +34,28 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--default_url] [--claude] [--show_all] prompt [prompt ...]
+usage: tax [-h] [--key KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
 
-Description of your program
+Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
-  prompt                Prompt
+  prompt         Prompt
 
 options:
-  -h, --help            show this help message and exit
-  --openai_key OPENAI_KEY
-                        Your key for OpenAI, only for one-time request
-  --model MODEL         Model name. You can use all OpenAI models.
-  --file FILE           Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
-  --url URL             URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.
-  --default_url         Use default OpenAI API URL for request.
-  --claude              Use Claude API for request.
-  --show_all            Show all contents in the response
+  -h, --help     show this help message and exit
+  --key KEY      Your key for OpenAI//Claude, only for one-time request
+  --model MODEL  Model name. You can use all OpenAI models.
+  --file FILE    Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
+  --url URL      URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.
+  --show_all     Show all contents in the response
 ```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
 ## Attention
@@ -87,7 +84,23 @@
 <summary>0.1.1</summary>
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
 </details>
 
+<details>
+<summary>0.1.2</summary>
+
+- [WIP]Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
+- Add a timeout function.
+- Fix: C++ code block prefix.
+</details>
+
+<details>
+<summary>0.1.3</summary>
+
+- Fix: code block prefix bug (tax will act maybe a little faster).
+- Modify: simplify the code.
+- Test: test for multi-process. Now you can use tax more efficiently in terminal.
+</details>
```

### Comparing `terminal-agent-x-0.1.2/pyproject.toml` & `terminal-agent-x-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal-agent-x"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="LyuLumos", email="lyujiuyang0@gmail.com" },
 ]
 description = "A terminal agent for terminal users."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -24,8 +24,8 @@
 ]
 
 [project.scripts]
 tax = "terminal_agent_x.tax:main"
 
 [project.urls]
 "Homepage" = "https://github.com/LyuLumos/Terminal-Agent-X"
-"Bug Tracker" = "https://github.com/LyuLumos/Terminal-Agent-X/issues"
+"Bug Tracker" = "https://github.com/LyuLumos/Terminal-Agent-X/issues"
```

### Comparing `terminal-agent-x-0.1.2/terminal_agent_x/tax.py` & `terminal-agent-x-0.1.3/terminal_agent_x/tax.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import signal
 import subprocess
 import os
 import argparse
-import psutil
 import re
 import json
+import psutil
 
 
 def check_terminal():
     # check the terminal type
     parent_process_name = psutil.Process(os.getppid()).name()
     if parent_process_name in ['pwsh', 'powershell', 'powershell.exe']:
         return 'powershell'
-    elif parent_process_name in ['cmd', 'cmd.exe']:
+    if parent_process_name in ['cmd', 'cmd.exe']:
         return 'cmd'
 
 
 def run_command_with_timeout(command, timeout):
     p = subprocess.Popen(command, stdout=subprocess.PIPE,
                          stderr=subprocess.PIPE, shell=True)
     try:
@@ -39,17 +39,21 @@
         for child in children:
             child.kill()
         parent.kill()
     except psutil.NoSuchProcess:
         pass
 
 
-def fetch_code(openai_key, model, prompt, args):
-    url = "https://api.lyulumos.space/v1/chat/completions" if not args.default_url else "https://api.openai.com/v1/chat/completions"
-    url = "https://claude-api.lyulumos.space/v1/chat/completions" if args.claude else url
+def fetch_code(openai_key, model, prompt, url):
+    urls = {
+        'openai_gfw': 'https://api.lyulumos.space/v1/chat/completions',
+        'openai': 'https://api.openai.com/v1/chat/completions',
+        'claude': 'https://claude-api.lyulumos.space/v1/chat/completions'
+    }
+    url = urls[url] if url in urls else url
     headers = [
         f"Authorization: Bearer {openai_key}",
         "Content-Type: application/json"
     ]
     terminal_headers = [
         f"Authorization='Bearer {openai_key}'",
         "'Content-Type'='application/json'"
@@ -58,72 +62,66 @@
 
     if os.name == 'nt':  # Windows
         if check_terminal() == 'powershell':
             wt_command = f'Invoke-WebRequest -Uri "{url}" -Method POST -Headers @{{{terminal_headers[0]};{terminal_headers[1]}}} -Body \'{data}\' -UseBasicParsing | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty choices | Select-Object -First 1 | Select-Object -ExpandProperty message | Select-Object -ExpandProperty content'
             print(
                 f'Current version does not fully support Windows PowerShell. Please copy command below and paste:\n\n{wt_command}')
             return ''
-        else:  # Windows cmd
-            headers = [h.replace('"', '\\"') for h in headers]
-            data = data.replace('"', '\\"')
-            command = f'curl -s "{url}" -H "{headers[0]}" -H "{headers[1]}" -d "{data}"'
+        # Windows cmd
+        headers = [h.replace('"', '\\"') for h in headers]
+        data = data.replace('"', '\\"')
+        command = f'curl -s "{url}" -H "{headers[0]}" -H "{headers[1]}" -d "{data}"'
     else:  # Linux
         command = f"curl -s --location '{url}' --header '{headers[0]}' --header '{headers[1]}' --data '{data}'"
     # print(command)
 
     try:
         res, err = run_command_with_timeout(command, 60)
-        # print(res, err)
         # res = os.popen(command).read().encode('utf-8').decode('utf-8', 'ignore')
         return json.loads(res)['choices'][0]['message']['content']
     except KeyError:
-        assert False, 'This is most likely due to poor internet. Please retry.'
+        assert False, 'This is most likely due to poor internet or invalid key. Please retry.'
+    except json.decoder.JSONDecodeError:
+        assert False, 'This URL may be invalid or the response cannot be parsed'
 
 
 def find_code(text):
     pattern = r"```(.*?)```"
     match = re.search(pattern, text, re.DOTALL)
     if match:
-        return delete_prefix(match.group(0))  # with ``` pairs
+        codes = match.group(0)
+        first_n = codes.find('\n')
+        return codes[first_n+1:-3].strip()  # without ``` pairs
     return None
 
 
-def delete_prefix(text):
-    # text: ```python\nprint('Hello, world!')\n``` or ```\nprint('Hello, world!')\n```
-    s_new = re.sub(r'```[\w-]*[+]*\n', '```', text)
-    return s_new.strip('`').strip()
-
-
 def main():
-    parser = argparse.ArgumentParser(description='Description of your program')
+    parser = argparse.ArgumentParser(
+        description='Tax: A terminal agent using OpenAI/Claude API')
     parser.add_argument("prompt", nargs='+', type=str, help="Prompt")
-    parser.add_argument('--openai_key', type=str,
-                        help='Your key for OpenAI, only for one-time request')
+    parser.add_argument('-k', '--key', type=str,
+                        help='Your key for OpenAI/Claude.')
     parser.add_argument('--model', type=str,
                         default='gpt-3.5-turbo', help='Model name. You can use all OpenAI models.')
     parser.add_argument(
-        '--file', type=str, help='Output file. If specified, the output will be written to this file. Tax will act like ChatGPT')
-    parser.add_argument('--url', type=str, default='https://api.lyulumos.space/v1/chat/completions',
-                        help='URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.')
-    parser.add_argument('--default_url', action='store_true',
-                        help='Use default OpenAI API URL for request.')
-    parser.add_argument('--claude', action='store_true',
-                        help='Use Claude API for request.')
+        '--file', type=str, help='Output file. If specified, the output will be written to this file. Tax will act like ChatGPT.')
+    parser.add_argument('--url', type=str, default='openai_gfw',
+                        help="URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.")
     parser.add_argument('--show_all', action='store_true',
-                        help='Show all contents in the response')
+                        help='Show all contents in the response.')
     args = parser.parse_args()
 
     prompt = ' '.join(args.prompt)
     prompt = f'{prompt}. Answer me with markdown'
-    openai_key = args.openai_key or os.environ.get('OpenAI_KEY')
-    if not openai_key:
+    key = args.key or os.environ.get('OpenAI_KEY')
+    if not key:
         assert False, 'Error: OpenAI key not found. Please specify it in system environment variables or pass it as an argument.'
 
     # res = get_model_response(openai_key, args.model, prompt)
-    res = fetch_code(openai_key, args.model, prompt, args)
+    res = fetch_code(key, args.model, prompt, args.url)
 
     if args.file:
         with open(args.file, 'w', encoding='utf-8') as f:
             f.write(res)
         f.close()
     elif args.show_all:
         print(res)
```

### Comparing `terminal-agent-x-0.1.2/terminal_agent_x.egg-info/PKG-INFO` & `terminal-agent-x-0.1.3/terminal_agent_x.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.2
+Version: 0.1.3
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -53,31 +53,28 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax.py [-h] [--openai_key OPENAI_KEY] [--model MODEL] [--file FILE] [--url URL] [--default_url] [--claude] [--show_all] prompt [prompt ...]
+usage: tax [-h] [--key KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
 
-Description of your program
+Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
-  prompt                Prompt
+  prompt         Prompt
 
 options:
-  -h, --help            show this help message and exit
-  --openai_key OPENAI_KEY
-                        Your key for OpenAI, only for one-time request
-  --model MODEL         Model name. You can use all OpenAI models.
-  --file FILE           Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
-  --url URL             URL for API request which can be accessd under GFW. When your network environment is NOT under GFW, you can use OpenAI API directly.
-  --default_url         Use default OpenAI API URL for request.
-  --claude              Use Claude API for request.
-  --show_all            Show all contents in the response
+  -h, --help     show this help message and exit
+  --key KEY      Your key for OpenAI//Claude, only for one-time request
+  --model MODEL  Model name. You can use all OpenAI models.
+  --file FILE    Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
+  --url URL      URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.
+  --show_all     Show all contents in the response
 ```
 
 ## Support
 
 I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
 
 ## Attention
@@ -106,7 +103,23 @@
 <summary>0.1.1</summary>
 
 - Add `--show_all` option for showing all contents of the response.
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
 </details>
 
+<details>
+<summary>0.1.2</summary>
+
+- [WIP]Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
+- Add a timeout function.
+- Fix: C++ code block prefix.
+</details>
+
+<details>
+<summary>0.1.3</summary>
+
+- Fix: code block prefix bug (tax will act maybe a little faster).
+- Modify: simplify the code.
+- Test: test for multi-process. Now you can use tax more efficiently in terminal.
+</details>
```

