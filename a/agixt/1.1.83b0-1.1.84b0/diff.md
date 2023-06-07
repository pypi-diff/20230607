# Comparing `tmp/agixt-1.1.83b0.tar.gz` & `tmp/agixt-1.1.84b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.83b0.tar", max compression
+gzip compressed data, was "agixt-1.1.84b0.tar", max compression
```

## Comparing `agixt-1.1.83b0.tar` & `agixt-1.1.84b0.tar`

### file list

```diff
@@ -1,111 +1,92 @@
--rw-r--r--   0        0        0     1087 2023-06-06 13:56:09.220190 agixt-1.1.83b0/LICENSE
--rw-r--r--   0        0        0    20599 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    23651 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Agent.py
--rw-r--r--   0        0        0    10664 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/ApiClient.py
--rw-r--r--   0        0        0     9260 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Chain.py
--rw-r--r--   0        0        0     1099 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6507 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Extensions.py
--rw-r--r--   0        0        0      599 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Main.py
--rw-r--r--   0        0        0     9492 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Memories.py
--rw-r--r--   0        0        0     1986 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7093 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0    16976 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-06-06 13:56:09.220190 agixt-1.1.83b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1030 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0     1428 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0     9976 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2156 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2449 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13323 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2457 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     2603 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1481 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5567 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2329 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      493 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     1638 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      980 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1012 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      763 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      873 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     5025 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1194 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1007 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1438 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1091 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2048 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0      975 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1585 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1597 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      850 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3730 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3106 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2823 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0    51470 2023-06-06 13:56:09.224190 agixt-1.1.83b0/agixt/tests.ipynb
--rw-r--r--   0        0        0    13384 2023-06-06 13:56:09.228190 agixt-1.1.83b0/docs/README.md
--rw-r--r--   0        0        0     2880 2023-06-06 13:56:09.236190 agixt-1.1.83b0/pyproject.toml
--rw-r--r--   0        0        0    16321 1970-01-01 00:00:00.000000 agixt-1.1.83b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-07 01:58:40.913918 agixt-1.1.84b0/LICENSE
+-rw-r--r--   0        0        0    19000 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    23585 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Agent.py
+-rw-r--r--   0        0        0     9260 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1099 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6105 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Extensions.py
+-rw-r--r--   0        0        0     9492 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1986 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7093 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0    16821 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/app.py
+-rw-r--r--   0        0        0     2012 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1030 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0    11935 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0      145 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2329 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      493 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     1638 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      980 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1012 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      763 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      873 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     5631 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1194 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1007 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1438 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1091 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2048 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     1071 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1585 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1597 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      850 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3730 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3106 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0     2823 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0    11554 2023-06-07 01:58:40.917918 agixt-1.1.84b0/docs/README.md
+-rw-r--r--   0        0        0     2880 2023-06-07 01:58:40.925918 agixt-1.1.84b0/pyproject.toml
+-rw-r--r--   0        0        0    14491 1970-01-01 00:00:00.000000 agixt-1.1.84b0/PKG-INFO
```

### Comparing `agixt-1.1.83b0/LICENSE` & `agixt-1.1.84b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/AGiXT.py` & `agixt-1.1.84b0/agixt/AGiXT.py`

 * *Files 5% similar despite different names*

```diff
@@ -348,15 +348,15 @@
     async def validation_agent(
         self, task, execution_response, context_results, **kwargs
     ):
         try:
             pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
             cleaned_json = pattern.findall(execution_response)
             if len(cleaned_json) == 0:
-                return False
+                return {}
             if isinstance(cleaned_json, list):
                 cleaned_json = cleaned_json[0]
             response = json.loads(cleaned_json)
             return response
         except:
             logging.info("INVALID JSON RESPONSE")
             logging.info(execution_response)
@@ -365,103 +365,68 @@
                 context_results = context_results - 1
             else:
                 context_results = 0
             execution_response = await self.run(
                 task=task, context_results=context_results, **kwargs
             )
             return await self.validation_agent(
-                task, execution_response, context_results, **kwargs
+                task=task,
+                execution_response=execution_response,
+                context_results=context_results,
+                **kwargs,
             )
 
-    async def revalidation_agent(
-        self,
-        task,
-        command_name,
-        command_args,
-        command_output,
-        context_results,
-        **kwargs,
-    ):
-        logging.info(
-            f"Command {command_name} did not execute as expected with args {command_args}. Trying again.."
-        )
-        revalidate = await self.run(
-            task=task,
-            prompt="ValidationFailed",
-            command_name=command_name,
-            command_args=command_args,
-            command_output=command_output,
-            **kwargs,
-        )
-        return await self.execution_agent(revalidate, task, context_results, **kwargs)
-
     async def execution_agent(
         self, execution_response, task, context_results, **kwargs
     ):
         validated_response = await self.validation_agent(
-            task, execution_response, context_results, **kwargs
+            task=task,
+            execution_response=execution_response,
+            context_results=context_results,
+            **kwargs,
         )
-        try:
+        if "commands" in validated_response:
             for command_name, command_args in validated_response["commands"].items():
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.agent.available_commands:
-                        if command_name in [
-                            available_command["friendly_name"],
-                            available_command["name"],
-                        ]:
-                            command_name = available_command["friendly_name"]
+                        if command_name == available_command["friendly_name"]:
+                            # Check if the command is a valid command in the self.avent.available_commands list
                             try:
-                                # Check if the command is a valid command in the self.avent.available_commands list
                                 command_output = await self.agent.execute(
                                     command_name=command_name, command_args=command_args
                                 )
-                                logging.info("Running Command Execution Validation...")
+                            except Exception as e:
+                                logging.info("Command validation failed, retrying...")
                                 validate_command = await self.run(
                                     task=task,
-                                    prompt="Validation",
+                                    prompt="ValidationFailed",
                                     command_name=command_name,
                                     command_args=command_args,
-                                    command_output=command_output,
+                                    command_output=e,
+                                    context_results=context_results,
                                     **kwargs,
                                 )
-                                if validate_command.startswith("Yes"):
-                                    # Failed command execution
-                                    return await self.revalidation_agent(
-                                        task=task,
-                                        command_name=command_name,
-                                        command_args=command_args,
-                                        command_output=command_output,
-                                        context_results=context_results,
-                                        **kwargs,
-                                    )
-                                else:
-                                    # Successful command execution
-                                    logging.info(
-                                        f"Command {command_name} executed successfully with args {command_args}. Command Output: {command_output}"
-                                    )
-                                    response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
-                                    return response
-                            except:
-                                return await self.revalidation_agent(
+                                return await self.execution_agent(
+                                    execution_response=validate_command,
                                     task=task,
-                                    command_name=command_name,
-                                    command_args=command_args,
-                                    command_output=command_output,
                                     context_results=context_results,
                                     **kwargs,
                                 )
+                            logging.info(
+                                f"Command {command_name} executed successfully with args {command_args}. Command Output: {command_output}"
+                            )
+                            response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
+                            return response
                 else:
                     if command_name == "None.":
                         return "\nNo commands were executed.\n"
                     else:
-                        return f"\Command not recognized: {command_name} ."
-        except:
-            logging.info("\nERROR IN EXECUTION_AGENT, validated_response:\n")
-            logging.info(validated_response)
+                        return f"\Command not recognized: `{command_name}`."
+        else:
             return "\nNo commands were executed.\n"
 
     async def websearch_agent(
         self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
     ):
         memories = self.agent.get_memories()
```

### Comparing `agixt-1.1.83b0/agixt/Agent.py` & `agixt-1.1.84b0/agixt/Agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # with it, managing its configuration and memory, and executing commands.
 import os
 import json
 import glob
 import shutil
 import importlib
 import yaml
-import time
 from pathlib import Path
 from inspect import signature, Parameter
 from provider import Provider
 from Memories import Memories
 from Extensions import Extensions
 
 DEFAULT_SETTINGS = {
@@ -62,31 +61,31 @@
                         self.EMBEDDER = "default"
                 if "MAX_TOKENS" in self.PROVIDER_SETTINGS:
                     self.MAX_TOKENS = self.PROVIDER_SETTINGS["MAX_TOKENS"]
                 else:
                     self.MAX_TOKENS = 4000
             self.commands = self.load_commands()
             self.available_commands = Extensions(
-                agent_config=self.AGENT_CONFIG, agent_name=self.agent_name
+                agent_config=self.AGENT_CONFIG
             ).get_available_commands()
             self.clean_agent_config_commands()
 
-            # Yaml Memory
-            self.memory_file = f"agents/{self.agent_name}.yaml"
-            self._create_parent_directories(self.memory_file)
-            self.memory = self.load_memory()
+            # Yaml History
+            self.history_file = f"agents/{self.agent_name}/history.yaml"
+            self._create_parent_directories(self.history_file)
+            self.history = self.load_history()
             self.agent_instances = {}
             self.agent_config = self.load_agent_config(self.agent_name)
 
     def get_memories(self):
         return Memories(self.agent_name, self.AGENT_CONFIG)
 
     async def execute(self, command_name, command_args):
-        return await Extensions(self.AGENT_CONFIG).execute_command(
-            command_name=command_name, command_args=command_args, agent=self
+        return await Extensions(agent_config=self.AGENT_CONFIG).execute_command(
+            command_name=command_name, command_args=command_args
         )
 
     async def instruct(self, prompt, tokens):
         """
         This function takes a prompt and tokens as input, sends the prompt to a provider for a response,
         logs the request if enabled, and returns the response.
 
@@ -332,53 +331,49 @@
         self.create_agent_folder(agent_name)
         commands_list = self.load_commands()
         command_dict = {}
         for command in commands_list:
             friendly_name, command_name, command_args = command
             command_dict[friendly_name] = False
         self.create_agent_config_file(agent_name, provider_settings, command_dict)
-        with open(os.path.join("agents", f"{agent_name}.yaml"), "w") as f:
+        with open(os.path.join("agents", f"{agent_name}/history.yaml"), "w") as f:
             f.write("")
-        return {"agent_file": f"{agent_name}.yaml"}
+        return {"agent_file": f"{agent_name}/history.yaml"}
 
     def rename_agent(self, agent_name, new_name):
         """
         This function renames an agent by updating the agent's name in a YAML file and renaming the agent's
         folder.
 
         :param agent_name: The current name of the agent that needs to be renamed
         :param new_name: The new name that the agent will be renamed to
         """
         self.agent_name = new_name
-        agent_file = f"agents/{agent_name}.yaml"
         agent_folder = f"agents/{agent_name}/"
-        agent_file = os.path.abspath(agent_file)
         agent_folder = os.path.abspath(agent_folder)
-        if os.path.exists(agent_file):
-            os.rename(agent_file, os.path.join("agents", f"{new_name}.yaml"))
         if os.path.exists(agent_folder):
+            # Check if the new name is already taken
+            if os.path.exists(f"agents/{new_name}"):
+                # Add a number to the end of the new name
+                i = 1
+                while os.path.exists(f"agents/{new_name}_{i}"):
+                    i += 1
+                new_name = f"{new_name}_{i}"
             os.rename(agent_folder, os.path.join("agents", f"{new_name}"))
 
     def delete_agent(self, agent_name):
         """
         This function deletes an agent's YAML file and returns an error message if the file is not found.
 
         :param agent_name: The name of the agent that needs to be deleted
         :return: If the agent file is not found, a dictionary with a "message" key and a 404 status code is
         returned.
         """
-        agent_file = f"agents/{agent_name}.yaml"
         agent_folder = f"agents/{agent_name}/"
-        agent_file = os.path.abspath(agent_file)
         agent_folder = os.path.abspath(agent_folder)
-        try:
-            os.remove(agent_file)
-        except FileNotFoundError:
-            return {"message": f"Agent file {agent_file} not found."}, 404
-
         if os.path.exists(agent_folder):
             shutil.rmtree(agent_folder)
 
         return {"message": f"Agent {agent_name} deleted."}, 200
 
     def get_agent_config(self):
         """
@@ -445,20 +440,20 @@
 
         :param agent_name: The name of the agent whose chat history is being retrieved
         :return: a list of dictionaries representing the chat history for a given agent. If the agent's chat
         history file does not exist, an empty list is returned. If there is an error while reading the file,
         an empty list is also returned.
         """
         # If it doesn't exist, create it
-        if not os.path.exists(f"agents/{agent_name}.yaml"):
-            with open(f"agents/{agent_name}.yaml", "w") as f:
+        if not os.path.exists(f"agents/{agent_name}/history.yaml"):
+            with open(f"agents/{agent_name}/history.yaml", "w") as f:
                 f.write("")
             return []
         try:
-            with open(f"agents/{agent_name}.yaml", "r") as f:
+            with open(f"agents/{agent_name}/history.yaml", "r") as f:
                 yaml_history = yaml.safe_load(f)
             chat_history = []
             for interaction in yaml_history["interactions"]:
                 role = interaction["role"]
                 message = interaction["message"]
                 chat_history.append({role: message})
             return chat_history
@@ -473,47 +468,48 @@
         """
         agent_folder = f"agents/{agent_name}/"
         agent_folder = os.path.abspath(agent_folder)
         memories_folder = os.path.join(agent_folder, "memories")
         if os.path.exists(memories_folder):
             shutil.rmtree(memories_folder)
 
-    def load_memory(self):
+    def load_history(self):
         """
-        This function loads a YAML file containing memory data and returns it, or creates a new file with
-        default data if the file does not exist.
-        :return: a dictionary object called `memory` which contains a list of interactions. The interactions
-        are loaded from a YAML file if it exists, otherwise an empty list is created and saved to the file.
+        This function loads the history of interactions from a YAML file if it exists, otherwise it creates
+        a new file and returns an empty list.
+        :return: The `load_history` function returns a dictionary containing the interactions stored in a
+        YAML file. If the file exists, it loads the interactions from the file. If the file does not exist,
+        it creates a new file and returns an empty dictionary.
         """
-        if os.path.exists(self.memory_file):
-            with open(self.memory_file, "r") as file:
+        if os.path.exists(self.history_file):
+            with open(self.history_file, "r") as file:
                 memory = yaml.safe_load(file)
         else:
-            with open(self.memory_file, "w") as file:
+            with open(self.history_file, "w") as file:
                 yaml.safe_dump({"interactions": []}, file)
             memory = {"interactions": []}
         return memory
 
     def save_memory(self):
         """
         This Python function saves the memory of an object to a YAML file.
         """
-        with open(self.memory_file, "w") as file:
-            yaml.safe_dump(self.memory, file)
+        with open(self.history_file, "w") as file:
+            yaml.safe_dump(self.history, file)
 
     def log_interaction(self, role: str, message: str):
         """
         This function logs an interaction by appending the role and message to a memory dictionary and
         saving it.
 
         :param role: The role of the person or entity that is interacting with the program. It could be a
         user, an administrator, a system, etc
         :type role: str
         :param message: The message parameter is a string that represents the interaction message that is
         being logged. It could be a user's input, a system response, or any other message exchanged during
         the interaction
         :type message: str
         """
-        if self.memory is None:
-            self.memory = {"interactions": []}
-        self.memory["interactions"].append({"role": role, "message": message})
+        if self.history is None:
+            self.history = {"interactions": []}
+        self.history["interactions"].append({"role": role, "message": message})
         self.save_memory()
```

### Comparing `agixt-1.1.83b0/agixt/Chain.py` & `agixt-1.1.84b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/Config.py` & `agixt-1.1.84b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/Embedding.py` & `agixt-1.1.84b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/Extensions.py` & `agixt-1.1.84b0/agixt/Extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import importlib
 import os
 import glob
-import json
 from inspect import signature, Parameter
 import logging
 
 
 class Extensions:
-    def __init__(
-        self, agent_config=None, load_commands_flag: bool = True, agent_name=""
-    ):
+    def __init__(self, agent_config=None, load_commands_flag: bool = True):
         self.agent_config = agent_config
         if load_commands_flag:
             self.commands = self.load_commands()
         else:
             self.commands = []
         if agent_config != None:
             self.available_commands = self.get_available_commands()
@@ -35,23 +32,14 @@
                         {
                             "friendly_name": friendly_name,
                             "name": command_name,
                             "args": command_args,
                             "enabled": True,
                         }
                     )
-                else:
-                    available_commands.append(
-                        {
-                            "friendly_name": friendly_name,
-                            "name": command_name,
-                            "args": command_args,
-                            "enabled": False,
-                        }
-                    )
         return available_commands
 
     def get_enabled_commands(self):
         enabled_commands = []
         for command in self.available_commands:
             if command["enabled"]:
                 enabled_commands.append(command)
```

### Comparing `agixt-1.1.83b0/agixt/Memories.py` & `agixt-1.1.84b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/Prompts.py` & `agixt-1.1.84b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/Tasks.py` & `agixt-1.1.84b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/app.py` & `agixt-1.1.84b0/agixt/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,11 +521,8 @@
 
 @app.get("/api/extensions/{command_name}/args", tags=["Extension"])
 async def get_command_args(command_name: str):
     return {"command_args": Extensions().get_command_args(command_name=command_name)}
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--workers", type=int, default=None)
-    args = parser.parse_args()
-    uvicorn.run(app, host="127.0.0.1", port=7437, workers=args.workers)
+    uvicorn.run(app, host="0.0.0.0", port=7437)
```

### Comparing `agixt-1.1.83b0/agixt/chains/Smart Chat.json` & `agixt-1.1.84b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/chains/Test_Commands.json` & `agixt-1.1.84b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/chains/Write a Poem.json` & `agixt-1.1.84b0/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/example.ipynb` & `agixt-1.1.84b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.84b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/briantts.py` & `agixt-1.1.84b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/dalle.py` & `agixt-1.1.84b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/discord.py` & `agixt-1.1.84b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.84b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/file_system.py` & `agixt-1.1.84b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/github.py` & `agixt-1.1.84b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/google.py` & `agixt-1.1.84b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/gtts.py` & `agixt-1.1.84b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/huggingface.py` & `agixt-1.1.84b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/macostts.py` & `agixt-1.1.84b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.84b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/searxng.py` & `agixt-1.1.84b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.84b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/twitter.py` & `agixt-1.1.84b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/extensions/web_playwright.py` & `agixt-1.1.84b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.84b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/Execution.txt` & `agixt-1.1.84b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/Instruction.txt` & `agixt-1.1.84b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.84b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.84b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.84b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.84b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.84b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/instruct.txt` & `agixt-1.1.84b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.84b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.84b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/__init__.py` & `agixt-1.1.84b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/azure.py` & `agixt-1.1.84b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/bing.py` & `agixt-1.1.84b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/chatgpt.py` & `agixt-1.1.84b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/claude.py` & `agixt-1.1.84b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/fastchat.py` & `agixt-1.1.84b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/gpt4all.py` & `agixt-1.1.84b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/gpt4free.py` & `agixt-1.1.84b0/agixt/provider/gpt4free.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,40 @@
         **kwargs,
     ):
         self.requirements = ["gpt4free"]
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.FAILED_PROVIDERS = []
-        self.providers = ["DeepAI", "You", "UseLess", "ForeFront", "Theb"]
+        self.providers = ["DeepAI", "You", "UseLess", "ForeFront", "Theb", "Poe"]
         self.account_tokens = {}
 
     def create_account(self, provider, module):
         try:
             # the following call will not terminate the program even if it calls quit()
             return module.Account.create()
         except SystemExit:
             logging.error(f"Account creation for {provider} called quit(), ignoring")
             return None
         except Exception as e:
             # handle other exceptions here
             logging.error(f"Failed to create account for {provider}: {e}")
             return None
 
+    async def provider_failure(self, provider):
+        if provider not in self.FAILED_PROVIDERS:
+            self.FAILED_PROVIDERS.append(provider)
+            logging.info(f"[GPT4Free] Failed provider: {provider}")
+            if len(self.FAILED_PROVIDERS) == len(self.providers):
+                self.FAILED_PROVIDERS = []
+                logging.info(
+                    "All providers failed, sleeping for 10 seconds before trying again..."
+                )
+                time.sleep(10)
+
     async def instruct(self, prompt, tokens: int = 0):
         final_response = None
         while final_response is None:
             for provider in self.providers:
                 try:
                     if provider not in self.FAILED_PROVIDERS:
                         logging.info(f"[GPT4Free] Using: {provider}")
@@ -75,35 +86,36 @@
                             if provider == "UseLess":
                                 if "text" in response:
                                     response = response["text"]
                                 if (
                                     "status" in response
                                     and response["status"] == "Fail"
                                 ):
-                                    self.FAILED_PROVIDERS.append(provider)
-                                    logging.info(
-                                        f"Failed to use {provider}: {response}"
-                                    )
+                                    await self.provider_failure(provider=provider)
                                     response = None
                             if (
                                 response
                                 == "Unable to fetch the response, Please try again."
                             ):
-                                self.FAILED_PROVIDERS.append(provider)
-                                logging.info(f"Failed to use {provider}: {response}")
+                                await self.provider_failure(provider=provider)
                                 response = None
                             if final_response == None:
                                 final_response = response
+                            else:
+                                await self.provider_failure(provider=provider)
                     if final_response:
                         if len(final_response) > 1:
                             return final_response
+                    else:
+                        logging.info(f"Failed to use {provider}")
+                        self.FAILED_PROVIDERS.append(provider)
+                        if len(self.FAILED_PROVIDERS) == len(self.providers):
+                            self.FAILED_PROVIDERS = []
+                            logging.info(
+                                "All providers failed, sleeping for 10 seconds before trying again..."
+                            )
+                            time.sleep(10)
                 except Exception as e:
-                    logging.info(f"Failed to use {provider}: {e}")
-                    self.FAILED_PROVIDERS.append(provider)
+                    await self.provider_failure(provider=provider)
                     final_response = None
 
-            if len(self.FAILED_PROVIDERS) == len(self.providers):
-                self.FAILED_PROVIDERS = []
-                logging.info(
-                    "All providers failed, sleeping for 10 seconds before trying again..."
-                )
-                time.sleep(10)
+            await self.provider_failure(provider=provider)
```

### Comparing `agixt-1.1.83b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.84b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/huggingchat.py` & `agixt-1.1.84b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/huggingface.py` & `agixt-1.1.84b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/kobold.py` & `agixt-1.1.84b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/llamacpp.py` & `agixt-1.1.84b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/llamacppapi.py` & `agixt-1.1.84b0/agixt/provider/llamacppapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,21 @@
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.AI_MODEL = AI_MODEL
         self.STOP_SEQUENCE = STOP_SEQUENCE
         self.MAX_TOKENS = int(self.MAX_TOKENS)
 
-    async def instruct(self, prompt, tokens: int = 0):
+    def instruct(self, prompt, tokens: int = 0):
         params = {
             "prompt": prompt,
             "temperature": float(self.AI_TEMPERATURE),
             "stop": self.STOP_SEQUENCE,
             "seed": random.randint(1, 1000000000),
         }
-        response = requests.post(f"{self.AI_PROVIDER_URI}/v1/completion", json=params)
+        response = requests.post(f"{self.AI_PROVIDER_URI}/v1/completions", json=params)
         data = response.json()
-        return data["content"]
+        print(data)
+        choices = data["choices"]
+        if choices:
+            return choices[0]["text"]
+        return None
```

### Comparing `agixt-1.1.83b0/agixt/provider/oobabooga.py` & `agixt-1.1.84b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/openai.py` & `agixt-1.1.84b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/palm.py` & `agixt-1.1.84b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/runpod.py` & `agixt-1.1.84b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/provider/transformer.py` & `agixt-1.1.84b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/agixt/test-commands.ipynb` & `agixt-1.1.84b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.83b0/docs/README.md` & `agixt-1.1.84b0/docs/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 # AGiXT
-![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
-[![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
+[![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
-[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
-
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
+[![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
+
+
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
-[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
-[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
+[![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-![Logo](images/AGiXT.svg)
+[![Logo](images/AGiXT.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quickstart using docker](#quickstart-using-docker)
-  - [Development using docker](#development-using-docker)
-  - [Development using poetry](#development-using-poetry)
-      - [Install poetry](#install-poetry)
-      - [Setup AGiXT](#setup-agixt)
-      - [Run AGiXT Locally](#run-agixt-locally)
+  - [Local Development](#local-development)
+    - [Setup AGiXT](#setup-agixt)
     - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
-  - [Acknowledgments](#acknowledgments)
   - [History](#history)
 
 ## ⚠️ Disclaimers!
 ### Monitor Your Usage!
 Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
 
 ### Under Development!
@@ -65,46 +59,29 @@
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart using docker
 
 Visit our [Quick Start](https://josh-xt.github.io/AGiXT/1-Getting%20started/Quick%20Start.html) documentation.
 
-## Development using docker
-```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
-docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
-```
-
-## Development using poetry
-#### Setup AGiXT
+## Local Development
+### Setup AGiXT
 We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
+
 ```
 git clone https://github.com/Josh-XT/AGiXT
 pip install poetry==1.5.1
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
 poetry install --with gpt4free
 poetry run playwright install
-```
-
-#### Run AGiXT Locally
-You will need to run two different terminals, one for the back end, one for the front end.
-
-First terminal will be the back end:
-```
-cd AGiXT/agixt
-poetry run python app.py
-```
-
-Second terminal will be the front end:
-```
-cd AGiXT/agixt
-poetry run streamlit run Main.py
+cd streamlit
+poetry run streamlit run Main.py &
+cd ../agixt
+poetry run uvicorn app:app --host 0.0.0.0 --port 7437 --workers 2
 ```
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
@@ -115,38 +92,29 @@
 
 This documentation is hosted locally and the back end must be running for these links to work.
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
-Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
+Need more information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details to get a better understanding of the concepts and features of AGiXT.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
-We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
+We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
 
 ## Donations and Sponsorships
-We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT).
+We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT).
 
 We're always looking for ways to improve AGiXT and make it more useful for our users. Your support will help us continue to develop and enhance the application. Thank you for considering to support us!
 
 ## Our Team 🧑‍💻
 | Josh (@Josh-XT)                    | James (@JamesonRGrieve) | 
 |-----------------------------------|-----------------------------------|
 |[![GitHub](https://img.shields.io/badge/GitHub-Follow_@Josh--XT-white?logo=github&style=plastic)](https://github.com/Josh-XT)|[![GitHub](https://img.shields.io/badge/GitHub-Follow_@JamesonRGrieve-white?logo=github&style=plastic)](https://github.com/JamesonRGrieve)|
 |[![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh__XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT)|[![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve)|
 |[![LinkedIn](https://img.shields.io/badge/LinkedIn-Follow_@JoshXT-blue?logo=linkedin&style=plastic)](https://www.linkedin.com/in/joshxt/)|[![LinkedIn](https://img.shields.io/badge/LinkedIn-Follow_@JamesonRGrieve-blue?logo=linkedin&style=plastic)](https://www.linkedin.com/in/jamesonrgrieve/)|
 
-## Acknowledgments
-
-This project was inspired by and is built using code from the following open-source repositories:
-
-- [![BabyAGI](https://img.shields.io/badge/GitHub-babyagi-white?logo=github&style=plastic) ![BabyAGI](https://img.shields.io/github/stars/yoheinakajima/babyagi?style=social)](https://github.com/yoheinakajima/babyagi)
-- [![Auto-GPT](https://img.shields.io/badge/GitHub-Auto--GPT-white?logo=github&style=plastic) ![Auto-GPT](https://img.shields.io/github/stars/Significant-Gravitas/Auto-GPT?style=social)](https://github.com/Significant-Gravitas/Auto-GPT)
-
-Please consider exploring and contributing to these projects if you like what we are doing.
-
 ## History
 ![Star History Chart](https://api.star-history.com/svg?repos=Josh-XT/AGiXT&type=Dat)
```

### Comparing `agixt-1.1.83b0/pyproject.toml` & `agixt-1.1.84b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.83-beta"
+version = "v1.1.84-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.1.83b0/PKG-INFO` & `agixt-1.1.84b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.83b0
+Version: 1.1.84b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: Josh XT
@@ -60,54 +60,48 @@
 Requires-Dist: tweepy (>=4.14.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: webdriver_manager (>=3.8.6,<4.0.0)
 Project-URL: Documentation, https://AGiXT.com
 Description-Content-Type: text/markdown
 
 # AGiXT
-![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
-[![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
+[![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
-[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
-
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
+[![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
+
+
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
-[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
-[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
+[![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-![Logo](images/AGiXT.svg)
+[![Logo](images/AGiXT.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quickstart using docker](#quickstart-using-docker)
-  - [Development using docker](#development-using-docker)
-  - [Development using poetry](#development-using-poetry)
-      - [Install poetry](#install-poetry)
-      - [Setup AGiXT](#setup-agixt)
-      - [Run AGiXT Locally](#run-agixt-locally)
+  - [Local Development](#local-development)
+    - [Setup AGiXT](#setup-agixt)
     - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
-  - [Acknowledgments](#acknowledgments)
   - [History](#history)
 
 ## ⚠️ Disclaimers!
 ### Monitor Your Usage!
 Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
 
 ### Under Development!
@@ -130,46 +124,29 @@
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart using docker
 
 Visit our [Quick Start](https://josh-xt.github.io/AGiXT/1-Getting%20started/Quick%20Start.html) documentation.
 
-## Development using docker
-```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
-docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
-```
-
-## Development using poetry
-#### Setup AGiXT
+## Local Development
+### Setup AGiXT
 We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
+
 ```
 git clone https://github.com/Josh-XT/AGiXT
 pip install poetry==1.5.1
 export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
 poetry install --with gpt4free
 poetry run playwright install
-```
-
-#### Run AGiXT Locally
-You will need to run two different terminals, one for the back end, one for the front end.
-
-First terminal will be the back end:
-```
-cd AGiXT/agixt
-poetry run python app.py
-```
-
-Second terminal will be the front end:
-```
-cd AGiXT/agixt
-poetry run streamlit run Main.py
+cd streamlit
+poetry run streamlit run Main.py &
+cd ../agixt
+poetry run uvicorn app:app --host 0.0.0.0 --port 7437 --workers 2
 ```
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
@@ -180,39 +157,30 @@
 
 This documentation is hosted locally and the back end must be running for these links to work.
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
-Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
+Need more information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details to get a better understanding of the concepts and features of AGiXT.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
-We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
+We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
 
 ## Donations and Sponsorships
-We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT).
+We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT).
 
 We're always looking for ways to improve AGiXT and make it more useful for our users. Your support will help us continue to develop and enhance the application. Thank you for considering to support us!
 
 ## Our Team 🧑‍💻
 | Josh (@Josh-XT)                    | James (@JamesonRGrieve) | 
 |-----------------------------------|-----------------------------------|
 |[![GitHub](https://img.shields.io/badge/GitHub-Follow_@Josh--XT-white?logo=github&style=plastic)](https://github.com/Josh-XT)|[![GitHub](https://img.shields.io/badge/GitHub-Follow_@JamesonRGrieve-white?logo=github&style=plastic)](https://github.com/JamesonRGrieve)|
 |[![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh__XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT)|[![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve)|
 |[![LinkedIn](https://img.shields.io/badge/LinkedIn-Follow_@JoshXT-blue?logo=linkedin&style=plastic)](https://www.linkedin.com/in/joshxt/)|[![LinkedIn](https://img.shields.io/badge/LinkedIn-Follow_@JamesonRGrieve-blue?logo=linkedin&style=plastic)](https://www.linkedin.com/in/jamesonrgrieve/)|
 
-## Acknowledgments
-
-This project was inspired by and is built using code from the following open-source repositories:
-
-- [![BabyAGI](https://img.shields.io/badge/GitHub-babyagi-white?logo=github&style=plastic) ![BabyAGI](https://img.shields.io/github/stars/yoheinakajima/babyagi?style=social)](https://github.com/yoheinakajima/babyagi)
-- [![Auto-GPT](https://img.shields.io/badge/GitHub-Auto--GPT-white?logo=github&style=plastic) ![Auto-GPT](https://img.shields.io/github/stars/Significant-Gravitas/Auto-GPT?style=social)](https://github.com/Significant-Gravitas/Auto-GPT)
-
-Please consider exploring and contributing to these projects if you like what we are doing.
-
 ## History
 ![Star History Chart](https://api.star-history.com/svg?repos=Josh-XT/AGiXT&type=Dat)
```

