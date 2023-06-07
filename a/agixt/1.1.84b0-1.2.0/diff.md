# Comparing `tmp/agixt-1.1.84b0.tar.gz` & `tmp/agixt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.84b0.tar", max compression
+gzip compressed data, was "agixt-1.2.0.tar", max compression
```

## Comparing `agixt-1.1.84b0.tar` & `agixt-1.2.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1087 2023-06-07 01:58:40.913918 agixt-1.1.84b0/LICENSE
--rw-r--r--   0        0        0    19000 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    23585 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Agent.py
--rw-r--r--   0        0        0     9260 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Chain.py
--rw-r--r--   0        0        0     1099 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6105 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Extensions.py
--rw-r--r--   0        0        0     9492 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Memories.py
--rw-r--r--   0        0        0     1986 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7093 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0    16821 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/app.py
--rw-r--r--   0        0        0     2012 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1030 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0    11935 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0      145 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2329 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      493 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     1638 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      980 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1012 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      763 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      873 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     5631 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1194 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1007 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1438 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1091 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2048 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     1071 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1585 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1597 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      850 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3730 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3106 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0     2823 2023-06-07 01:58:40.913918 agixt-1.1.84b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0    11554 2023-06-07 01:58:40.917918 agixt-1.1.84b0/docs/README.md
--rw-r--r--   0        0        0     2880 2023-06-07 01:58:40.925918 agixt-1.1.84b0/pyproject.toml
--rw-r--r--   0        0        0    14491 1970-01-01 00:00:00.000000 agixt-1.1.84b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-07 20:13:22.746698 agixt-1.2.0/LICENSE
+-rw-r--r--   0        0        0    19409 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    23585 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Agent.py
+-rw-r--r--   0        0        0    10083 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Chain.py
+-rw-r--r--   0        0        0     1099 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6805 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Extensions.py
+-rw-r--r--   0        0        0     9489 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Memories.py
+-rw-r--r--   0        0        0     1986 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7093 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0    17835 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/app.py
+-rw-r--r--   0        0        0     2012 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0     7108 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1030 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0    11935 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6213 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0      151 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      181 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1017 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1178 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      378 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      430 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      270 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Score Response.txt
+-rw-r--r--   0        0        0      349 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      274 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      304 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      148 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      474 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      528 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      458 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      433 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      160 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      507 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      560 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      192 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      162 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      856 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      314 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1178 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1178 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      777 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      824 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      616 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2329 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      493 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     1638 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      980 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1012 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      763 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      873 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     5430 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1194 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1007 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1438 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1091 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2048 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     1071 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1585 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1597 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      850 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3730 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3106 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0    11848 2023-06-07 20:13:22.750698 agixt-1.2.0/docs/README.md
+-rw-r--r--   0        0        0     2781 2023-06-07 20:13:22.758698 agixt-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14782 1970-01-01 00:00:00.000000 agixt-1.2.0/PKG-INFO
```

### Comparing `agixt-1.1.84b0/LICENSE` & `agixt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/AGiXT.py` & `agixt-1.2.0/agixt/AGiXT.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,36 +67,36 @@
                 # replace the {STEPx} with the response
                 value = value.replace(f"{{STEP{step_number}}}", step_response)
             new_prompt_content[arg] = value
         return new_prompt_content
 
     async def format_prompt(
         self,
-        task: str = "",
+        user_input: str = "",
         top_results: int = 5,
         prompt="",
         chain_name="",
         step_number=0,
         memories=None,
         **kwargs,
     ):
         cp = Prompts()
         if prompt == "":
-            prompt = task
+            prompt = user_input
         else:
             try:
                 prompt = cp.get_prompt(prompt_name=prompt, model=self.agent.AI_MODEL)
             except:
                 prompt = prompt
         if top_results == 0:
             context = "None"
         else:
             try:
                 context = await memories.context_agent(
-                    query=task, top_results_num=top_results
+                    query=user_input, top_results_num=top_results
                 )
             except:
                 context = "None."
         command_list = self.agent.get_commands_string()
         if chain_name != "":
             try:
                 for arg, value in kwargs.items():
@@ -111,22 +111,22 @@
             except:
                 logging.info("No args to replace.")
             if "{STEP" in prompt:
                 step_response = self.get_step_response(
                     chain_name=chain_name, step_number=step_number
                 )
                 prompt = prompt.replace(f"{{STEP{step_number}}}", step_response)
-            if "{STEP" in task:
+            if "{STEP" in user_input:
                 step_response = self.get_step_response(
                     chain_name=chain_name, step_number=step_number
                 )
-                task = task.replace(f"{{STEP{step_number}}}", step_response)
+                user_input = user_input.replace(f"{{STEP{step_number}}}", step_response)
         formatted_prompt = self.custom_format(
             string=prompt,
-            task=task,
+            user_input=user_input,
             agent_name=self.agent_name,
             COMMANDS=self.agent_commands,
             context=context,
             command_list=command_list,
             date=datetime.now().strftime("%B %d, %Y %I:%M %p"),
             **kwargs,
         )
@@ -135,15 +135,15 @@
             self.load_spacy_model()
         tokens = len(self.nlp(formatted_prompt))
         logging.info(f"FORMATTED PROMPT: {formatted_prompt}")
         return formatted_prompt, prompt, tokens
 
     async def run(
         self,
-        task: str = "",
+        user_input: str = "",
         prompt: str = "",
         context_results: int = 5,
         websearch: bool = False,
         websearch_depth: int = 3,
         learn_file: str = "",
         chain_name: str = "",
         step_number: int = 0,
@@ -152,24 +152,24 @@
         logging.info(f"KWARGS: {kwargs}")
         memories = self.agent.get_memories()
         if learn_file != "":
             learning_file = await memories.mem_read_file(file_path=learn_file)
             if learning_file == False:
                 return "Failed to read file."
         formatted_prompt, unformatted_prompt, tokens = await self.format_prompt(
-            task=task,
+            user_input=user_input,
             top_results=context_results,
             prompt=prompt,
             chain_name=chain_name,
             step_number=step_number,
             memories=memories,
             **kwargs,
         )
         if websearch:
-            await self.websearch_agent(task=task, depth=websearch_depth)
+            await self.websearch_agent(user_input=user_input, depth=websearch_depth)
         try:
             # Workaround for non-threaded providers
             run_response = await self.agent.instruct(formatted_prompt, tokens=tokens)
             self.response = (
                 run_response.result()
                 if isinstance(run_response, Future)
                 else run_response
@@ -184,26 +184,26 @@
                 logging.info("Failed to get a response 5 times in a row.")
                 return None
             logging.info(f"Retrying in 10 seconds...")
             time.sleep(10)
             if context_results > 0:
                 context_results = context_results - 1
             self.response = await self.run(
-                task=task,
+                user_input=user_input,
                 prompt=prompt,
                 context_results=context_results,
                 **kwargs,
             )
 
         # Handle commands if the prompt contains the {COMMANDS} placeholder
         # We handle command injection that DOESN'T allow command execution by using {command_list} in the prompt
         if "{COMMANDS}" in unformatted_prompt:
             execution_response = await self.execution_agent(
                 execution_response=self.response,
-                task=task,
+                user_input=user_input,
                 context_results=context_results,
                 **kwargs,
             )
             return_response = ""
             try:
                 self.response = json.loads(self.response)
                 if "response" in self.response:
@@ -219,34 +219,34 @@
                     )
             except:
                 return_response = self.response
             self.response = return_response
         logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
             try:
-                await memories.store_result(task_name=task, result=self.response)
+                await memories.store_result(input=user_input, result=self.response)
             except:
                 pass
-            self.agent.log_interaction(role="USER", message=task)
+            self.agent.log_interaction(role="USER", message=user_input)
             self.agent.log_interaction(role=self.agent_name, message=self.response)
         return self.response
 
     async def smart_instruct(
         self,
-        task: str = "Write a tweet about AI.",
+        user_input: str = "Write a tweet about AI.",
         shots: int = 3,
         learn_file: str = "",
         objective: str = None,
         **kwargs,
     ):
         answers = []
         # Do multi shots of prompt to get N different answers to be validated
         answers.append(
             await self.run(
-                task=task,
+                user_input=user_input,
                 prompt="SmartInstruct-StepByStep"
                 if objective == None
                 else "SmartTask-StepByStep",
                 context_results=6,
                 websearch=True,
                 websearch_depth=3,
                 shots=shots,
@@ -255,102 +255,101 @@
                 **kwargs,
             )
         )
         if shots > 1:
             for i in range(shots - 1):
                 answers.append(
                     await self.run(
-                        task=task,
+                        user_input=user_input,
                         prompt="SmartInstruct-StepByStep"
                         if objective == None
                         else "SmartTask-StepByStep",
                         context_results=6,
                         shots=shots,
                         objective=objective,
                         **kwargs,
                     )
                 )
         answer_str = ""
         for i, answer in enumerate(answers):
             answer_str += f"Answer {i + 1}:\n{answer}\n\n"
         researcher = await self.run(
-            task=answer_str,
+            user_input=answer_str,
             prompt="SmartInstruct-Researcher",
             shots=shots,
             **kwargs,
         )
         resolver = await self.run(
-            task=researcher,
+            user_input=researcher,
             prompt="SmartInstruct-Resolver",
             shots=shots,
             **kwargs,
         )
         execution_response = await self.run(
-            task=task,
-            prompt="SmartInstruct-Execution",
-            previous_response=resolver,
+            user_input=f"{user_input}\nContext:\n{resolver}",
+            prompt="instruct",
             **kwargs,
         )
         response = f"{resolver}\n\n{execution_response}"
         return response
 
     async def smart_chat(
         self,
-        task: str = "Write a tweet about AI.",
+        user_input: str = "Write a tweet about AI.",
         shots: int = 3,
         learn_file: str = "",
         **kwargs,
     ):
         answers = []
         answers.append(
             await self.run(
-                task=task,
+                user_input=user_input,
                 prompt="SmartChat-StepByStep",
                 context_results=6,
                 websearch=True,
                 websearch_depth=3,
                 shots=shots,
                 learn_file=learn_file,
                 **kwargs,
             )
         )
         # Do multi shots of prompt to get N different answers to be validated
         if shots > 1:
             for i in range(shots - 1):
                 answers.append(
                     await self.run(
-                        task=task,
+                        user_input=user_input,
                         prompt="SmartChat-StepByStep",
                         context_results=6,
                         shots=shots,
                         **kwargs,
                     )
                 )
         answer_str = ""
         for i, answer in enumerate(answers):
             answer_str += f"Answer {i + 1}:\n{answer}\n\n"
         researcher = await self.run(
-            task=answer_str,
+            user_input=answer_str,
             prompt="SmartChat-Researcher",
             context_results=6,
             shots=shots,
             **kwargs,
         )
         resolver = await self.run(
-            task=researcher,
+            user_input=researcher,
             prompt="SmartChat-Resolver",
             context_results=6,
             shots=shots,
             **kwargs,
         )
         return resolver
 
     # Worker Sub-Agents
     async def validation_agent(
-        self, task, execution_response, context_results, **kwargs
+        self, user_input, execution_response, context_results, **kwargs
     ):
         try:
             pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
             cleaned_json = pattern.findall(execution_response)
             if len(cleaned_json) == 0:
                 return {}
             if isinstance(cleaned_json, list):
@@ -362,28 +361,28 @@
             logging.info(execution_response)
             logging.info("... Trying again.")
             if context_results != 0:
                 context_results = context_results - 1
             else:
                 context_results = 0
             execution_response = await self.run(
-                task=task, context_results=context_results, **kwargs
+                user_input=user_input, context_results=context_results, **kwargs
             )
             return await self.validation_agent(
-                task=task,
+                user_input=user_input,
                 execution_response=execution_response,
                 context_results=context_results,
                 **kwargs,
             )
 
     async def execution_agent(
-        self, execution_response, task, context_results, **kwargs
+        self, execution_response, user_input, context_results, **kwargs
     ):
         validated_response = await self.validation_agent(
-            task=task,
+            user_input=user_input,
             execution_response=execution_response,
             context_results=context_results,
             **kwargs,
         )
         if "commands" in validated_response:
             for command_name, command_args in validated_response["commands"].items():
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
@@ -394,25 +393,25 @@
                             try:
                                 command_output = await self.agent.execute(
                                     command_name=command_name, command_args=command_args
                                 )
                             except Exception as e:
                                 logging.info("Command validation failed, retrying...")
                                 validate_command = await self.run(
-                                    task=task,
+                                    user_input=user_input,
                                     prompt="ValidationFailed",
                                     command_name=command_name,
                                     command_args=command_args,
                                     command_output=e,
                                     context_results=context_results,
                                     **kwargs,
                                 )
                                 return await self.execution_agent(
                                     execution_response=validate_command,
-                                    task=task,
+                                    user_input=user_input,
                                     context_results=context_results,
                                     **kwargs,
                                 )
                             logging.info(
                                 f"Command {command_name} executed successfully with args {command_args}. Command Output: {command_output}"
                             )
                             response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
@@ -422,19 +421,21 @@
                         return "\nNo commands were executed.\n"
                     else:
                         return f"\Command not recognized: `{command_name}`."
         else:
             return "\nNo commands were executed.\n"
 
     async def websearch_agent(
-        self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
+        self,
+        user_input: str = "What are the latest breakthroughs in AI?",
+        depth: int = 3,
     ):
         memories = self.agent.get_memories()
 
-        async def resursive_browsing(task, links):
+        async def resursive_browsing(user_input, links):
             try:
                 words = links.split()
                 links = [
                     word for word in words if urlparse(word).scheme in ["http", "https"]
                 ]
             except:
                 links = links
@@ -459,26 +460,28 @@
                             ) = await memories.read_website(url)
                             if link_list is not None:
                                 if len(link_list) > 0:
                                     if len(link_list) > 5:
                                         link_list = link_list[:3]
                                     try:
                                         pick_a_link = await self.run(
-                                            task=task,
+                                            user_input=user_input,
                                             prompt="Pick-a-Link",
                                             links=link_list,
                                         )
                                         if not pick_a_link.startswith("None"):
-                                            await resursive_browsing(task, pick_a_link)
+                                            await resursive_browsing(
+                                                user_input, pick_a_link
+                                            )
                                     except:
                                         logging.info(
                                             f"Issues reading {url}. Moving on..."
                                         )
 
-        results = await self.run(task=task, prompt="WebSearch")
+        results = await self.run(user_input=user_input, prompt="WebSearch")
         results = results.split("\n")
         for result in results:
             search_string = result.lstrip("0123456789. ")
             try:
                 searx_server = self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
             except:
                 searx_server = ""
@@ -487,8 +490,8 @@
                     search_string
                 )
                 if len(links) > depth:
                     links = links[:depth]
             except:
                 links = None
             if links is not None:
-                await resursive_browsing(task, links)
+                await resursive_browsing(user_input, links)
```

### Comparing `agixt-1.1.84b0/agixt/Agent.py` & `agixt-1.2.0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/Chain.py` & `agixt-1.2.0/agixt/Chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,23 +101,23 @@
                     step["step"] -= 1
         moved_step["step"] = new_step_number
         chain_data["steps"].append(moved_step)
         chain_data["steps"] = sorted(chain_data["steps"], key=lambda x: x["step"])
         with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
             json.dump(chain_data, f)
 
-    async def run_chain(self, chain_name):
+    async def run_chain(self, chain_name, user_input=None):
         chain_data = self.get_chain(chain_name=chain_name)
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
                 step_response = await self.run_chain_step(
-                    step=step_data, chain_name=chain_name
+                    step=step_data, chain_name=chain_name, user_input=user_input
                 )  # Get the response of the current step.
                 responses[step_data["step"]] = step_response  # Store the response.
                 logging.info(f"Response: {step_response}")
                 # Write the responses to the json file.
                 with open(
                     os.path.join("chains", f"{chain_name}_responses.json"), "w"
                 ) as f:
@@ -140,85 +140,101 @@
         try:
             with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
                 responses = json.load(f)
             return responses
         except:
             return {}
 
-    def get_step_content(self, chain_name, prompt_content):
+    def get_step_content(self, chain_name, prompt_content, user_input):
         new_prompt_content = {}
         if isinstance(prompt_content, dict):
             for arg, value in prompt_content.items():
+                if "{user_input}" in value:
+                    value = value.replace("{user_input}", user_input)
                 if "{STEP" in value:
+                    # Count how many times {STEP is in the value
+                    step_count = value.count("{STEP")
+                    for i in range(step_count):
+                        # Get the step number from value between {STEP and }
+                        new_step_number = int(value.split("{STEP")[1].split("}")[0])
+                        # get the response from the step number
+                        step_response = self.get_step_response(
+                            chain_name=chain_name, step_number=new_step_number
+                        )
+                        # replace the {STEPx} with the response
+                        value = value.replace(
+                            f"{{STEP{new_step_number}}}", step_response
+                        )
+                new_prompt_content[arg] = value
+        elif isinstance(prompt_content, str):
+            if "{user_input}" in prompt_content:
+                new_prompt_content = prompt_content.replace("{user_input}", user_input)
+            if "{STEP" in prompt_content:
+                step_count = value.count("{STEP")
+                for i in range(step_count):
                     # Get the step number from value between {STEP and }
-                    new_step_number = int(value.split("{STEP")[1].split("}")[0])
+                    new_step_number = int(
+                        prompt_content.split("{STEP")[1].split("}")[0]
+                    )
                     # get the response from the step number
                     step_response = self.get_step_response(
                         chain_name=chain_name, step_number=new_step_number
                     )
                     # replace the {STEPx} with the response
-                    value = value.replace(f"{{STEP{new_step_number}}}", step_response)
-                new_prompt_content[arg] = value
-        elif isinstance(prompt_content, str):
-            if "{STEP" in prompt_content:
-                # Get the step number from value between {STEP and }
-                new_step_number = int(prompt_content.split("{STEP")[1].split("}")[0])
-                # get the response from the step number
-                step_response = self.get_step_response(
-                    chain_name=chain_name, step_number=new_step_number
-                )
-                # replace the {STEPx} with the response
-                new_prompt_content = prompt_content.replace(
-                    f"{{STEP{new_step_number}}}", step_response
-                )
+                    new_prompt_content = prompt_content.replace(
+                        f"{{STEP{new_step_number}}}", step_response
+                    )
+            if new_prompt_content == {}:
+                new_prompt_content = prompt_content
         return new_prompt_content
 
-    async def run_chain_step(self, step: dict = {}, chain_name=""):
+    async def run_chain_step(self, step: dict = {}, chain_name="", user_input=""):
         logging.info(step)
         if step:
             if "prompt_type" in step:
                 agent_name = step["agent_name"]
                 agent = AGiXT(agent_name)
                 prompt_type = step["prompt_type"]
                 step_number = step["step"]
                 if "prompt_name" in step["prompt"]:
                     prompt_name = step["prompt"]["prompt_name"]
                 else:
                     prompt_name = ""
                 args = self.get_step_content(
-                    chain_name=chain_name, prompt_content=step["prompt"]
+                    chain_name=chain_name,
+                    prompt_content=step["prompt"],
+                    user_input=user_input,
                 )
                 if prompt_type == "Command":
                     return await Extensions(
                         agent_config=agent.agent.agent_config
                     ).execute_command(
                         command_name=args["command_name"], command_args=args
                     )
                 elif prompt_type == "Prompt":
                     result = await agent.run(
+                        user_input=user_input,
                         prompt=prompt_name,
                         chain_name=chain_name,
                         step_number=step_number,
                         **args,
                     )
                 elif prompt_type == "Chain":
-                    result = await self.run_chain(step["prompt"]["chain_name"])
-                elif prompt_type == "Smart Instruct":
-                    result = await agent.smart_instruct(**args)
-                elif prompt_type == "Smart Chat":
-                    result = await agent.smart_chat(**args)
-                elif prompt_type == "Task":
-                    result = await agent.run_task(**args)
+                    result = await self.run_chain(
+                        chain_name=step["prompt"]["chain_name"], user_input=user_input
+                    )
         if result:
             return result
         else:
             return None
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--chain", type=str, default="")
+    parser.add_argument("--user_input", type=str, default="")
     args = parser.parse_args()
     chain_name = args.chain
+    user_input = args.user_input
     import asyncio
 
-    asyncio.run(Chain().run_chain(chain_name=chain_name))
+    asyncio.run(Chain().run_chain(chain_name=chain_name, user_input=user_input))
```

### Comparing `agixt-1.1.84b0/agixt/Config.py` & `agixt-1.2.0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/Embedding.py` & `agixt-1.2.0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/Extensions.py` & `agixt-1.2.0/agixt/Extensions.py`

 * *Files 15% similar despite different names*

```diff
@@ -142,7 +142,20 @@
                 del args[param]
         try:
             output = await getattr(module(), command_function.__name__)(**args)
         except Exception as e:
             output = f"Error: {str(e)}"
         logging.info(f"Command Output: {output}")
         return output
+
+    def get_extensions(self):
+        commands = []
+        command_files = glob.glob("extensions/*.py")
+        for command_file in command_files:
+            module_name = os.path.splitext(os.path.basename(command_file))[0]
+            module = importlib.import_module(f"extensions.{module_name}")
+            command_class = getattr(module, module_name.lower())()
+            if hasattr(command_class, "commands"):
+                for command_name, command_function in command_class.commands.items():
+                    params = self.get_command_params(command_function)
+                    commands.append((command_name, command_function.__name__, params))
+        return commands
```

### Comparing `agixt-1.1.84b0/agixt/Memories.py` & `agixt-1.2.0/agixt/Memories.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,24 +95,24 @@
                 record=record,
             )
             self.chroma_client._client.persist()
         except Exception as e:
             logging.info(f"Failed to store memory: {e}")
 
     async def store_result(
-        self, task_name: str, result: str, external_source_name: str = None
+        self, input: str, result: str, external_source_name: str = None
     ):
         if result:
             if not isinstance(result, str):
                 result = str(result)
-            chunks = await self.chunk_content(result, task_name)
+            chunks = await self.chunk_content(result, input)
             for chunk in chunks:
                 await self.store_memory(
                     content=chunk,
-                    description=task_name,
+                    description=input,
                     external_source_name=external_source_name,
                 )
 
     async def context_agent(self, query: str, top_results_num: int) -> List[str]:
         embedder, chunk_size = await self.get_embedder()
         collection = await self.get_collection()
         if collection == None:
@@ -209,15 +209,15 @@
             elif file_path.endswith(".doc") or file_path.endswith(".docx"):
                 content = docx2txt.process(file_path)
             # TODO: If file is an image, classify it in text.
             # Otherwise just read the file
             else:
                 with open(file_path, "r") as f:
                     content = f.read()
-            await self.store_result(task_name=file_path, result=content)
+            await self.store_result(input=file_path, result=content)
             return True
         except:
             return False
 
     async def read_website(self, url):
         try:
             async with async_playwright() as p:
@@ -236,11 +236,11 @@
                     link_list.append((title, href))
 
                 await browser.close()
                 soup = BeautifulSoup(content, "html.parser")
                 text_content = soup.get_text()
                 text_content = " ".join(text_content.split())
                 if text_content:
-                    await self.store_result(url, text_content)
+                    await self.store_result(input=url, result=text_content)
                 return text_content, link_list
         except:
             return None, None
```

### Comparing `agixt-1.1.84b0/agixt/Prompts.py` & `agixt-1.2.0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/Tasks.py` & `agixt-1.2.0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/app.py` & `agixt-1.2.0/agixt/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,22 @@
     agent_name: str
 
 
 class AgentNewName(BaseModel):
     new_name: str
 
 
+class AgentPrompt(BaseModel):
+    prompt_name: str
+    prompt_args: dict
+    websearch: bool
+    websearch_depth: int
+    context_results: int
+
+
 class Objective(BaseModel):
     objective: str
 
 
 class Prompt(BaseModel):
     prompt: str
 
@@ -247,38 +255,59 @@
     return ResponseMessage(message=f"Memories for agent {agent_name} deleted.")
 
 
 @app.post("/api/agent/{agent_name}/instruct", tags=["Agent"])
 async def instruct(agent_name: str, prompt: Prompt):
     agent = AGiXT(agent_name=agent_name)
     response = await agent.run(
-        task=prompt.prompt,
+        user_input=prompt.prompt,
         prompt="instruct",
     )
     return {"response": str(response)}
 
 
+@app.post("/api/agent/{agent_name}/prompt", tags=["Agent"])
+async def prompt_agent(agent_name: str, agent_prompt: AgentPrompt):
+    agent = AGiXT(agent_name=agent_name)
+    user_input = (
+        agent_prompt.prompt_args["user_input"]
+        if "user_input" in agent_prompt.prompt_args
+        else ""
+    )
+    response = await agent.run(
+        user_input=user_input,
+        prompt=agent_prompt.prompt_name,
+        websearch=agent_prompt.websearch,
+        websearch_depth=agent_prompt.websearch_depth,
+        context_results=agent_prompt.context_results,
+        **agent_prompt.prompt_args,
+    )
+    return {"response": str(response)}
+
+
 @app.post("/api/agent/{agent_name}/smartinstruct/{shots}", tags=["Agent"])
 async def smartinstruct(agent_name: str, shots: int, prompt: Prompt):
     agent = AGiXT(agent_name=agent_name)
-    response = await agent.smart_instruct(task=prompt.prompt, shots=int(shots))
+    response = await agent.smart_instruct(user_input=prompt.prompt, shots=int(shots))
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/chat", tags=["Agent"])
 async def chat(agent_name: str, prompt: Prompt):
     agent = AGiXT(agent_name=agent_name)
-    response = await agent.run(task=prompt.prompt, prompt="Chat", context_results=6)
+    response = await agent.run(
+        user_input=prompt.prompt, prompt="Chat", context_results=6
+    )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartchat/{shots}", tags=["Agent"])
 async def smartchat(agent_name: str, shots: int, prompt: Prompt):
     agent = AGiXT(agent_name=agent_name)
-    response = await agent.smart_chat(task=prompt.prompt, shots=shots)
+    response = await agent.smart_chat(user_input=prompt.prompt, shots=shots)
     return {"response": str(response)}
 
 
 @app.get("/api/agent/{agent_name}/command", tags=["Agent"])
 async def get_commands(agent_name: str):
     agent = Agent(agent_name=agent_name)
     return {"commands": agent.agent_config["commands"]}
@@ -387,16 +416,16 @@
         chain_data = Chain().get_step_response(chain_name=chain_name, step_number="all")
         return {"chain": chain_data}
     except:
         raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
-async def run_chain(chain_name: str) -> ResponseMessage:
-    await Chain().run_chain(chain_name=chain_name)
+async def run_chain(chain_name: str, user_input: Prompt) -> ResponseMessage:
+    await Chain().run_chain(chain_name=chain_name, user_input=user_input.prompt)
     return {"message": f"Chain '{chain_name}' completed."}
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
     Chain().add_chain(chain_name=chain_name.chain_name)
     return ResponseMessage(message=f"Chain '{chain_name.chain_name}' created.")
@@ -520,9 +549,14 @@
 
 
 @app.get("/api/extensions/{command_name}/args", tags=["Extension"])
 async def get_command_args(command_name: str):
     return {"command_args": Extensions().get_command_args(command_name=command_name)}
 
 
+@app.get("/api/extensions", tags=["Extension"])
+async def get_extensions():
+    return {"extensions": Extensions().get_extensions()}
+
+
 if __name__ == "__main__":
     uvicorn.run(app, host="0.0.0.0", port=7437)
```

### Comparing `agixt-1.1.84b0/agixt/chains/Smart Chat.json` & `agixt-1.2.0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/chains/Write a Poem.json` & `agixt-1.2.0/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/example.ipynb` & `agixt-1.2.0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/agixt_agent.py` & `agixt-1.2.0/agixt/extensions/agixt_agent.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     async def create_command(
         self, function_description: str, agent: str = "AGiXT"
     ) -> List[str]:
         with open(f"prompts/Create New Command.txt", "r") as f:
             prompt = f.read()
         prompt = prompt.replace("{{NEW_FUNCTION_DESCRIPTION}}", function_description)
-        response = await AGiXT(agent).run(prompt)
+        response = await AGiXT(agent_name=agent).run(user_input=prompt)
         file_name = response.split("class ")[1].split("(")[0]
         code = code.replace("```", "")
 
         if not self.command_exists(file_name):
             with open(f"commands/{file_name}.py", "w") as f:
                 f.write(code)
             return f"Created new command: {file_name}."
@@ -55,74 +55,74 @@
             return f"Command {file_name} already exists. No changes were made."
 
     async def evaluate_code(self, code: str, agent: str = "AGiXT") -> List[str]:
         args = [code]
         function_string = "def analyze_code(code: str) -> List[str]:"
         description_string = "Analyzes the given code and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(prompt)
+        return await AGiXT(agent).run(user_input=prompt)
 
     async def analyze_pull_request(
         self, pr_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [pr_url]
         function_string = "def analyze_pr(pr_url: str) -> List[str]:"
         description_string = "Analyzes the given pull request and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(prompt)
+        return await AGiXT(agent).run(user_input=prompt)
 
     async def perform_automated_testing(
         self, test_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [test_url]
         function_string = "def perform_testing(test_url: str) -> List[str]:"
         description_string = "Performs automated testing using AI-driven tools and returns a list of test results."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(prompt)
+        return await AGiXT(agent).run(user_input=prompt)
 
     async def improve_code(
         self, suggestions: List[str], code: str, agent: str = "AGiXT"
     ) -> str:
         args = [json.dumps(suggestions), code]
         function_string = (
             "def generate_improved_code(suggestions: List[str], code: str) -> str:"
         )
         description_string = "Improves the provided code based on the suggestions provided, making no other changes."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(prompt)
+        return await AGiXT(agent).run(user_input=prompt)
 
     async def write_tests(
         self,
         code: str,
         focus: Optional[List[str]] = None,
         agent: str = "AGiXT",
     ) -> str:
         args = [code, json.dumps(focus) if focus else "None"]
         function_string = "def create_test_cases(code: str, focus: Optional[List[str]] = None) -> str:"
         description_string = "Generates test cases for the existing code, focusing on specific areas if required."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(prompt)
+        return await AGiXT(agent).run(user_input=prompt)
 
     async def run_ci_cd_pipeline(self, repo_url: str, agent: str = "AGiXT") -> str:
         args = [repo_url]
         function_string = "def run_pipeline(repo_url: str) -> str:"
         description_string = (
             "Runs the entire CI/CD pipeline for the given repository URL."
         )
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(prompt)
+        return await AGiXT(agent).run(user_input=prompt)
 
-    async def run_chain(self, chain_name):
-        await Chain().run_chain(chain_name)
+    async def run_chain(self, chain_name: str = "", user_input: str = ""):
+        await Chain().run_chain(chain_name=chain_name, user_input=user_input)
         return "Chain started successfully."
 
-    async def ask(self, prompt: str, agent: str = "AGiXT") -> str:
+    async def ask(self, user_input: str, agent: str = "AGiXT") -> str:
         response = await AGiXT(agent).run(
-            prompt, prompt="chat", websearch=True, websearch_depth=4
+            user_input=user_input, prompt="chat", websearch=True, websearch_depth=4
         )
         return response
 
-    async def instruct(self, prompt: str, agent: str = "AGiXT") -> str:
+    async def instruct(self, user_input: str, agent: str = "AGiXT") -> str:
         response = await AGiXT(agent).run(
-            task=prompt, prompt="instruct", websearch=True, websearch_depth=8
+            user_input=user_input, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
```

### Comparing `agixt-1.1.84b0/agixt/extensions/briantts.py` & `agixt-1.2.0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/dalle.py` & `agixt-1.2.0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/discord.py` & `agixt-1.2.0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/elevenlabs.py` & `agixt-1.2.0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/file_system.py` & `agixt-1.2.0/agixt/extensions/file_system.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,20 @@
         **kwargs,
     ):
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
         self.WORKING_DIRECTORY_RESTRICTED = WORKING_DIRECTORY_RESTRICTED
         if not os.path.exists(self.WORKING_DIRECTORY):
             os.makedirs(self.WORKING_DIRECTORY)
         self.commands = {
-            "Read File": self.read_file,
             "Write to File": self.write_to_file,
-            "Append to File": self.append_to_file,
-            "Delete File": self.delete_file,
+            "Read File": self.read_file,
             "Search Files": self.search_files,
+            "Append to File": self.append_to_file,
             "Execute Python File": self.execute_python_file,
+            "Delete File": self.delete_file,
             "Execute Shell": self.execute_shell,
         }
         self.WORKING_DIRECTORY = WORKING_DIRECTORY
 
     async def execute_python_file(self, file: str):
         logging.info(f"Executing file '{file}' in workspace '{self.WORKING_DIRECTORY}'")
```

### Comparing `agixt-1.1.84b0/agixt/extensions/github.py` & `agixt-1.2.0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/google.py` & `agixt-1.2.0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/gtts.py` & `agixt-1.2.0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/huggingface.py` & `agixt-1.2.0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/macostts.py` & `agixt-1.2.0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/microsoft_365.py` & `agixt-1.2.0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/searxng.py` & `agixt-1.2.0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/sendgrid_email.py` & `agixt-1.2.0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/twitter.py` & `agixt-1.2.0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/extensions/web_playwright.py` & `agixt-1.2.0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/prompts/Create New Command.txt` & `agixt-1.2.0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/prompts/Execution.txt` & `agixt-1.2.0/agixt/prompts/Execution.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Your role is to do anything asked of you with precision. You have the following constraints:
 1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.
 2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.
 3. No user assistance.
 
 Take into account these previously completed tasks from context.
 
-Your task: {task}
+Your task: {user_input}
 
 {COMMANDS}
 
 RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
 ```JSON
 {
     "response": "Your response to the task.",
```

### Comparing `agixt-1.1.84b0/agixt/prompts/Instruction.txt` & `agixt-1.2.0/agixt/prompts/Instruction.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
 
-Your task: {task}
+Your task: {user_input}
```

### Comparing `agixt-1.1.84b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.0/agixt/prompts/SmartTask-Execution.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 {COMMANDS}
 
+Primary Objective: {objective}
+
 Task: 
 ```
-{task}
+{user_input}
 ```
 
 Task Response: 
 ```
 {previous_response}
 ```
```

### Comparing `agixt-1.1.84b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.0/agixt/prompts/ValidationFailed.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {context}
 {command_list}
 
 Task:
-{task}
+{user_input}
 
 We attempted to run the following command with the Arguments:
 {command_name}
 
 Arguments:
 {command_args}
```

### Comparing `agixt-1.1.84b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
 
-Your task: {task}
+Your task: {user_input}
```

### Comparing `agixt-1.1.84b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.0/agixt/prompts/gpt-4/instruct.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
 
-Your task: {task}
+Your task: {user_input}
```

### Comparing `agixt-1.1.84b0/agixt/prompts/instruct.txt` & `agixt-1.2.0/agixt/prompts/starchat/instruct.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<|system|>
 {COMMANDS}
 You have the following constraints:
 ~500 word limit for short term memory. Your short term memory is short, so immediately save important information to files.
 If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.
 No user assistance.
 
 RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
@@ -17,9 +18,8 @@
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
-
-Your task: {task}
+<|end|><|user|>Your task: {user_input}<|end|>\n<|assistant|>
```

### Comparing `agixt-1.1.84b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.0/agixt/prompts/instruct.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-<|system|>
 {COMMANDS}
 You have the following constraints:
 ~500 word limit for short term memory. Your short term memory is short, so immediately save important information to files.
 If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.
 No user assistance.
 
 RESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.
@@ -18,8 +17,9 @@
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
-<|end|><|user|>Your task: {task}<|end|>\n<|assistant|>
+
+Your task: {user_input}
```

### Comparing `agixt-1.1.84b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.0/agixt/prompts/vicuna/instruct.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,9 +19,9 @@
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
 
-Task: {task}
+Task: {user_input}
 ###Assistant:
```

### Comparing `agixt-1.1.84b0/agixt/provider/__init__.py` & `agixt-1.2.0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/azure.py` & `agixt-1.2.0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/bing.py` & `agixt-1.2.0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/chatgpt.py` & `agixt-1.2.0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/claude.py` & `agixt-1.2.0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/fastchat.py` & `agixt-1.2.0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/gpt4all.py` & `agixt-1.2.0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/gpt4free.py` & `agixt-1.2.0/agixt/provider/gpt4free.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,26 +86,24 @@
                             if provider == "UseLess":
                                 if "text" in response:
                                     response = response["text"]
                                 if (
                                     "status" in response
                                     and response["status"] == "Fail"
                                 ):
-                                    await self.provider_failure(provider=provider)
                                     response = None
                             if (
                                 response
                                 == "Unable to fetch the response, Please try again."
                             ):
-                                await self.provider_failure(provider=provider)
                                 response = None
-                            if final_response == None:
-                                final_response = response
-                            else:
-                                await self.provider_failure(provider=provider)
+                        if response:
+                            final_response = response
+                        else:
+                            await self.provider_failure(provider)
                     if final_response:
                         if len(final_response) > 1:
                             return final_response
                     else:
                         logging.info(f"Failed to use {provider}")
                         self.FAILED_PROVIDERS.append(provider)
                         if len(self.FAILED_PROVIDERS) == len(self.providers):
```

### Comparing `agixt-1.1.84b0/agixt/provider/gpugpt4all.py` & `agixt-1.2.0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/huggingchat.py` & `agixt-1.2.0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/huggingface.py` & `agixt-1.2.0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/kobold.py` & `agixt-1.2.0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/llamacpp.py` & `agixt-1.2.0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/llamacppapi.py` & `agixt-1.2.0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/oobabooga.py` & `agixt-1.2.0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/openai.py` & `agixt-1.2.0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/palm.py` & `agixt-1.2.0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/runpod.py` & `agixt-1.2.0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/agixt/provider/transformer.py` & `agixt-1.2.0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.84b0/docs/README.md` & `agixt-1.2.0/docs/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Quickstart using docker](#quickstart-using-docker)
-  - [Local Development](#local-development)
-    - [Setup AGiXT](#setup-agixt)
-    - [API Endpoints](#api-endpoints)
+  - [Quick Start Guide](#quick-start-guide)
+    - [Local Quick Start Guide](#local-quick-start-guide)
+    - [Docker Quick Start Guide](#docker-quick-start-guide)
+      - [Update Docker Containers](#update-docker-containers)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [History](#history)
 
@@ -55,46 +55,53 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Quickstart using docker
+## Quick Start Guide
+You have two options for running AGiXT currently, you can either run it with Python locally or you can run it with Docker.
 
-Visit our [Quick Start](https://josh-xt.github.io/AGiXT/1-Getting%20started/Quick%20Start.html) documentation.
+### Local Quick Start Guide
+To get started quickly locally, you will need at least Python 3.10.6 installed.  If using Windows, we recommend installing [Windows Subsystem For Linux](https://learn.microsoft.com/en-us/windows/wsl/install) first.
 
-## Local Development
-### Setup AGiXT
-We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
+Open a terminal and run the following commands:
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-pip install poetry==1.5.1
-export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
-poetry install --with gpt4free
-poetry run playwright install
-cd streamlit
-poetry run streamlit run Main.py &
-cd ../agixt
-poetry run uvicorn app:app --host 0.0.0.0 --port 7437 --workers 2
+./AGiXT.sh
 ```
 
-Access the web interface at http://localhost:8501
+Any time you want to run AGiXT after that, you can just run `./AGiXT.sh` from the AGiXT directory.  This will pull the latest changes from the main branch then launch AGiXT.
 
-### API Endpoints
+You may have to press `Ctrl+C` multiple times to stop AGiXT running in the terminal due to it running multiple processes.
 
-AGiXT provides several API endpoints for managing agents, prompts and chains.
+- Access the web interface at http://localhost:8501
+- Access the AGiXT API documentation at http://localhost:7437
 
-To learn more about the API endpoints and their usage, visit the API documentation at 
-- [Swagger](http://localhost:7437)
-- [Redoc](http://localhost:7437/redoc)
+### Docker Quick Start Guide
+To get started quickly with Docker, you will need at least Docker 24.0.2 installed. You can check your version by running `docker --version` in a terminal. You can install Docker by following the instructions [here](https://docs.docker.com/get-docker/).
+
+Open a terminal and run the following commands:
+```
+git clone https://github.com/Josh-XT/AGiXT
+cd AGiXT
+docker-compose up
+```
+
+- Access the web interface at http://localhost:8501
+- Access the AGiXT API documentation at http://localhost:7437
+#### Update Docker Containers
+
+```
+docker compose pull
+```
 
-This documentation is hosted locally and the back end must be running for these links to work.
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Need more information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details to get a better understanding of the concepts and features of AGiXT.
```

### Comparing `agixt-1.1.84b0/pyproject.toml` & `agixt-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.84-beta"
+version = "v1.2.0"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
@@ -52,30 +52,23 @@
 # jsonschema = "*"
 openai = "^0.27.7"
 pandas = "^2.0.1"
 pdfplumber = "^0.9.0"
 playwright = "^1.33.0"
 playsound = "1.2.2"
 PyYAML = "^6.0"
-# pre-commit = "*"
-# pytz = "*"
-# pynacl = "*"
-# python-git = "*"
 PyGithub = "^1.58.2"
 random-password-generator = "^2.2.0"
 revChatGPT = "^5.2.0"
 requests = "^2.31.0"
 selenium = "^4.9.1"
 sendgrid = "^6.10.0"
 spacy = "^3.5.3"
-####
 streamlit = "^1.22.0"
 protobuf = "3.20.*"
-####
-# tiktoken = "*"
 tweepy = "^4.14.0"
 uvicorn = "^0.22.0"
 webdriver_manager = "^3.8.6"
 
 
 ## see https://pytorch.org/get-started/locally/ for weird torch combinations
 ## this installs all cpu versions for pytorch on lin, win, mac/arm64
```

### Comparing `agixt-1.1.84b0/PKG-INFO` & `agixt-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.84b0
+Version: 1.2.0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: Josh XT
@@ -85,18 +85,18 @@
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Quickstart using docker](#quickstart-using-docker)
-  - [Local Development](#local-development)
-    - [Setup AGiXT](#setup-agixt)
-    - [API Endpoints](#api-endpoints)
+  - [Quick Start Guide](#quick-start-guide)
+    - [Local Quick Start Guide](#local-quick-start-guide)
+    - [Docker Quick Start Guide](#docker-quick-start-guide)
+      - [Update Docker Containers](#update-docker-containers)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [History](#history)
 
@@ -120,46 +120,53 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Quickstart using docker
+## Quick Start Guide
+You have two options for running AGiXT currently, you can either run it with Python locally or you can run it with Docker.
 
-Visit our [Quick Start](https://josh-xt.github.io/AGiXT/1-Getting%20started/Quick%20Start.html) documentation.
+### Local Quick Start Guide
+To get started quickly locally, you will need at least Python 3.10.6 installed.  If using Windows, we recommend installing [Windows Subsystem For Linux](https://learn.microsoft.com/en-us/windows/wsl/install) first.
 
-## Local Development
-### Setup AGiXT
-We will install AGiXT in a virtual environment. This will ensure that the dependencies of AGiXT do not interfere with other Python projects on your system.  We will also use playwright for web scraping.  This requires a browser to be installed on your system.  If you do not have a browser installed, you can install one with `playwright install`.
+Open a terminal and run the following commands:
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-pip install poetry==1.5.1
-export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
 cd AGiXT
-poetry install --with gpt4free
-poetry run playwright install
-cd streamlit
-poetry run streamlit run Main.py &
-cd ../agixt
-poetry run uvicorn app:app --host 0.0.0.0 --port 7437 --workers 2
+./AGiXT.sh
 ```
 
-Access the web interface at http://localhost:8501
+Any time you want to run AGiXT after that, you can just run `./AGiXT.sh` from the AGiXT directory.  This will pull the latest changes from the main branch then launch AGiXT.
 
-### API Endpoints
+You may have to press `Ctrl+C` multiple times to stop AGiXT running in the terminal due to it running multiple processes.
 
-AGiXT provides several API endpoints for managing agents, prompts and chains.
+- Access the web interface at http://localhost:8501
+- Access the AGiXT API documentation at http://localhost:7437
 
-To learn more about the API endpoints and their usage, visit the API documentation at 
-- [Swagger](http://localhost:7437)
-- [Redoc](http://localhost:7437/redoc)
+### Docker Quick Start Guide
+To get started quickly with Docker, you will need at least Docker 24.0.2 installed. You can check your version by running `docker --version` in a terminal. You can install Docker by following the instructions [here](https://docs.docker.com/get-docker/).
+
+Open a terminal and run the following commands:
+```
+git clone https://github.com/Josh-XT/AGiXT
+cd AGiXT
+docker-compose up
+```
+
+- Access the web interface at http://localhost:8501
+- Access the AGiXT API documentation at http://localhost:7437
+#### Update Docker Containers
+
+```
+docker compose pull
+```
 
-This documentation is hosted locally and the back end must be running for these links to work.
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Need more information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details to get a better understanding of the concepts and features of AGiXT.
```

