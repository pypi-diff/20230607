# Comparing `tmp/gpt-term-1.1.1.tar.gz` & `tmp/gpt-term-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.1.1.tar", last modified: Sat May 20 13:58:39 2023, max compression
+gzip compressed data, was "gpt-term-1.1.2.tar", last modified: Wed Jun  7 12:05:18 2023, max compression
```

## Comparing `gpt-term-1.1.1.tar` & `gpt-term-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.679308 gpt-term-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.683308 gpt-term-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-20 13:58:28.000000 gpt-term-1.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-20 13:58:28.000000 gpt-term-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 13:58:28.000000 gpt-term-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-05-20 13:58:39.687308 gpt-term-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.683308 gpt-term-1.1.1/README.assets/
--rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.assets/image-20230303233352970.png
--rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.assets/small.gif
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-20 13:58:28.000000 gpt-term-1.1.1/README.zh-CN.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-05-20 13:58:28.000000 gpt-term-1.1.1/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/gpt_term/locale/
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.de.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.en.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.jp.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale/gpt_term.zh_CN.yml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/locale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48431 2023-05-20 13:58:28.000000 gpt-term-1.1.1/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:58:39.687308 gpt-term-1.1.1/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 13:58:39.000000 gpt-term-1.1.1/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-20 13:58:28.000000 gpt-term-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 13:58:28.000000 gpt-term-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:58:39.687308 gpt-term-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.627585 gpt-term-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.631585 gpt-term-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 12:05:02.000000 gpt-term-1.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 12:05:02.000000 gpt-term-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 12:05:02.000000 gpt-term-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-07 12:05:18.635585 gpt-term-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.631585 gpt-term-1.1.2/README.assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.assets/image-20230303233352970.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.assets/small.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-07 12:05:02.000000 gpt-term-1.1.2/README.zh-CN.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-06-07 12:05:02.000000 gpt-term-1.1.2/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/gpt_term/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.de.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.en.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.jp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale/gpt_term.zh_CN.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/locale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48430 2023-06-07 12:05:02.000000 gpt-term-1.1.2/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:05:18.635585 gpt-term-1.1.2/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 12:05:18.000000 gpt-term-1.1.2/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-07 12:05:02.000000 gpt-term-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 12:05:02.000000 gpt-term-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:05:18.635585 gpt-term-1.1.2/setup.cfg
```

### Comparing `gpt-term-1.1.1/.github/workflows/pypi-publish.yml` & `gpt-term-1.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/LICENSE` & `gpt-term-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/PKG-INFO` & `gpt-term-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.1
+Version: 1.1.2
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -192,15 +192,15 @@
 - `Ctrl+W`: Delete the word to the left of the cursor
 
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments | Description | Examples |
-| ------------- | --------------------------------- | - ----------------------------------------------- |
+| ------------- | --------------------------------- | ------------------------------------------------ |
 | -h, --help | show this help message and exit | `gpt-term --help` |
 | --load FILE | Load chat history from file | `gpt-term --load chat_history_code_check.json` |
 | --key API_KEY | Select the API key to use in the config.ini file | `gpt-term --key OPENAI_API_KEY1` |
 | --model MODEL | Select AI model to use | `gpt-term --model gpt-3.5-turbo` |
 | --host HOST | Set the API Host address used in this run (this is usually used to configure proxy) | `gpt-term --host https://closeai.deno.dev` |
 | -m, --multi | Enable multiline mode | `gpt-term --multi` |
 | -r, --raw | Enable raw mode | `gpt-term --raw` |
```

### Comparing `gpt-term-1.1.1/README.assets/image-20230303233352970.png` & `gpt-term-1.1.2/README.assets/image-20230303233352970.png`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/README.assets/small.gif` & `gpt-term-1.1.2/README.assets/small.gif`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/README.md` & `gpt-term-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 - `Ctrl+W`: Delete the word to the left of the cursor
 
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments | Description | Examples |
-| ------------- | --------------------------------- | - ----------------------------------------------- |
+| ------------- | --------------------------------- | ------------------------------------------------ |
 | -h, --help | show this help message and exit | `gpt-term --help` |
 | --load FILE | Load chat history from file | `gpt-term --load chat_history_code_check.json` |
 | --key API_KEY | Select the API key to use in the config.ini file | `gpt-term --key OPENAI_API_KEY1` |
 | --model MODEL | Select AI model to use | `gpt-term --model gpt-3.5-turbo` |
 | --host HOST | Set the API Host address used in this run (this is usually used to configure proxy) | `gpt-term --host https://closeai.deno.dev` |
 | -m, --multi | Enable multiline mode | `gpt-term --multi` |
 | -r, --raw | Enable raw mode | `gpt-term --raw` |
@@ -330,8 +330,8 @@
 │   └── main.py               # Main program
 ├── requirements.txt          # List of dependencies
 └── setup.py
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `gpt-term-1.1.1/README.zh-CN.md` & `gpt-term-1.1.2/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/gpt_term/config.ini` & `gpt-term-1.1.2/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/gpt_term/locale/gpt_term.de.yml` & `gpt-term-1.1.2/gpt_term/locale/gpt_term.de.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/gpt_term/locale/gpt_term.en.yml` & `gpt-term-1.1.2/gpt_term/locale/gpt_term.en.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/gpt_term/locale/gpt_term.jp.yml` & `gpt-term-1.1.2/gpt_term/locale/gpt_term.jp.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/gpt_term/locale/gpt_term.zh_CN.yml` & `gpt-term-1.1.2/gpt_term/locale/gpt_term.zh_CN.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/gpt_term/main.py` & `gpt-term-1.1.2/gpt_term/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
         self.endpoint = self.host + "/v1/chat/completions"
 
     def modify_system_prompt(self, new_content: str):
         if self.messages[0]['role'] == 'system':
             old_content = self.messages[0]['content']
             self.messages[0]['content'] = new_content
             console.print(
-                _("gpt_term.system_prompt_moodified",old_content=old_content,new_content=new_content))
+                _("gpt_term.system_prompt_modified",old_content=old_content,new_content=new_content))
             self.current_tokens = count_token(self.messages)
             # recount current tokens
             if len(self.messages) > 1:
                 console.print(
                     _("gpt_term.system_prompt_note"))
         else:
             console.print(
```

### Comparing `gpt-term-1.1.1/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.1.2/gpt_term.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.1
+Version: 1.1.2
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -192,15 +192,15 @@
 - `Ctrl+W`: Delete the word to the left of the cursor
 
 > Original chat logs will be saved to `~/.gpt-term/chat.log`
 
 ### Available Arguments
 
 | Arguments | Description | Examples |
-| ------------- | --------------------------------- | - ----------------------------------------------- |
+| ------------- | --------------------------------- | ------------------------------------------------ |
 | -h, --help | show this help message and exit | `gpt-term --help` |
 | --load FILE | Load chat history from file | `gpt-term --load chat_history_code_check.json` |
 | --key API_KEY | Select the API key to use in the config.ini file | `gpt-term --key OPENAI_API_KEY1` |
 | --model MODEL | Select AI model to use | `gpt-term --model gpt-3.5-turbo` |
 | --host HOST | Set the API Host address used in this run (this is usually used to configure proxy) | `gpt-term --host https://closeai.deno.dev` |
 | -m, --multi | Enable multiline mode | `gpt-term --multi` |
 | -r, --raw | Enable raw mode | `gpt-term --raw` |
```

### Comparing `gpt-term-1.1.1/gpt_term.egg-info/SOURCES.txt` & `gpt-term-1.1.2/gpt_term.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.1/pyproject.toml` & `gpt-term-1.1.2/pyproject.toml`

 * *Files identical despite different names*

