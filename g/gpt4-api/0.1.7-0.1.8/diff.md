# Comparing `tmp/gpt4-api-0.1.7.tar.gz` & `tmp/gpt4-api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.1.7.tar", last modified: Mon Jun  5 10:25:37 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.1.8.tar", last modified: Wed Jun  7 01:59:54 2023, max compression
```

## Comparing `gpt4-api-0.1.7.tar` & `gpt4-api-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.7/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    16557 2023-06-05 10:25:20.000000 gpt4-api-0.1.7/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-05 10:25:37.000000 gpt4-api-0.1.7/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.7/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.8/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    10292 2023-06-07 01:39:20.000000 gpt4-api-0.1.8/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-07 01:59:54.000000 gpt4-api-0.1.8/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.8/setup.py
```

### Comparing `gpt4-api-0.1.7/api/gpt.py` & `gpt4-api-0.1.8/api/gpt.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import openai
 import asyncio
 from pathlib import Path
 from multiprocessing import JoinableQueue
 from queue import Empty
 
 logging.basicConfig(filename='gpt.log', level=logging.INFO, format='%(asctime)s %(levelname)s: %(message)s')
+console_handler = logging.StreamHandler()
+console_handler.setLevel(logging.INFO)
+console_handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s: %(message)s'))
+logging = logging.getLogger()
+logging.addHandler(console_handler)
 
 
 class call_black_parameter(object):
     def __init__(self, response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name):
         self.response_str = response_str
         self.messages = messages
         self.elapsed_time = elapsed_time
@@ -24,15 +29,15 @@
 class GPTTaskManager:
     def __init__(self, num_thread, keys, stream=False, max_retries=3, key_limit=4096, model='gpt-4', temperature=0, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None, call_back=None):
         self.num_threads = num_thread
         self.stream = stream
         self.max_retries = max_retries
         self.task_queue = JoinableQueue()
         self.key_lock = threading.Lock()
-        self.usable_openai_keys = self.process_token(keys=keys) or []
+        self.usable_openai_keys = self.process_token(keys=keys)
         self.key_limit = key_limit
         # 模型
         self.model = model
         # 用于控制生成文本的随机性和创造性的参数。值越高，生成文本越随机和创造性；值越低，生成文本越可预测和保守
         self.temperature = temperature
         # 用于对生成文本进行选择的参数，它表示只选择所有可能的令牌中累计概率高于给定阈值的那些令牌。默认值为1，表示选择所有可能的令牌
         self.top_p = top_p
@@ -44,60 +49,56 @@
         self.n = n
         # 是否将生成的文本作为流返回，而不是一次性返回所有文本。默认为False，表示一次性返回所有文本
         # 系统默认内容
         self.system_content = system_content
         self.total_tokens = 0
         self.call_back = call_back
         self.threads = []
+        self.__worker_flag = True
 
     def __worker(self, run_func):
-        logging.disable(logging.NOTSET)
         while True:
             try:
                 task = self.task_queue.get(timeout=1)
-                content = task.get("ask")
-                messages = task.get("messages")
-                if "retry" not in task:
-                    task["retry"] = False
-                logging.info("active threads: %s" % self.get_active_thread_count())
-                run_func(task, content, messages)
-                self.task_queue.task_done()
+                if task:
+                    content = task.get("ask")
+                    messages = task.get("messages")
+                    run_func(task, content, messages)
+                    self.task_queue.task_done()
             except Empty:
                 break
             except Exception as e:
                 logging.error(e)
                 break
 
     def __run_tasks(self, tasks, run_func):
-        if len(self.threads) == 0:
-            logging.info("Total threads: %s" % self.num_threads)
-            for _ in range(self.num_threads):
-                thread = threading.Thread(target=self.__worker, args=(run_func,))
-                thread.start()
-                self.threads.append(thread)
-            logging.info("Total tasks: %s" % len(tasks))
-            for task in tasks:
-                self.task_queue.put(task)
-            # self.task_queue.join()
-            for thread in self.threads:
-                thread.join()
-            logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
-        else:
-            logging.info("Successfully added tasks for the second time, totaling: %s" % len(tasks))
-            for task in tasks:
-                self.task_queue.put(task)
+        logging.info("total tasks: %s" % len(tasks))
+        for task in tasks:
+            task["retry"] = False
+            self.task_queue.put(task)
+        if len(tasks) * 2 < self.num_threads:
+            self.num_threads = len(tasks) * 2
+        logging.info("Total threads: %s" % self.num_threads)
+        for _ in range(self.num_threads):
+            thread = threading.Thread(target=self.__worker, args=(run_func,))
+            thread.start()
+            self.threads.append(thread)
+        for thread in self.threads:
+            thread.join()
+        # if self.task_is_empty():
+        #     self.__worker_flag = False
+        logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
 
     @staticmethod
     def process_token(keys):
-        usable_openai_keys = []
+        usable_openai_keys = {}
         for key in keys:
-            usable_openai_keys.append({"api_key": key, "token_limit": 0})
+            usable_openai_keys[key] = 0
         if len(usable_openai_keys) == 0:
             raise Exception("Unable to execute gpt task without token")
-        logging.info("Total tokens: %s" % len(usable_openai_keys))
         return usable_openai_keys
 
     @staticmethod
     def read_prompt(path):
         return Path(path).read_text()
 
     def __retry_on_error(self, task, ask_content, messages, retries):
@@ -105,55 +106,49 @@
         if retries <= self.max_retries:
             task["retry"] = True
             self.__process_task(task, ask_content, messages, retries=retries)
         else:
             self.task_queue.put(task)
 
     def __get_key(self):
-        with self.key_lock:
-            sorted_data = sorted(self.usable_openai_keys, key=lambda x: x['token_limit'], reverse=True)
-            if len(sorted_data) <= 0:
-                return False
-            open_ai_key = sorted_data[0].get("api_key")
-            token_limit = sorted_data[0].get("token_limit")
-            if open_ai_key and token_limit >= self.key_limit:
-                logging.info("Token re election")
-                return self.__get_key()
-            return open_ai_key
+        open_ai_key = None
+        for token, token_limit in self.usable_openai_keys.items():
+            if token_limit < self.key_limit:
+                open_ai_key = token
+                break
+            else:
+                logging.info("token: %s limit: %s" % (token, token_limit))
+        return open_ai_key
 
     def __release_token(self, open_ai_key):
-        for openaiKey in self.usable_openai_keys:
-            if openaiKey.get("api_key", None) == open_ai_key:
-                openaiKey["token_limit"] = 0
+        self.usable_openai_keys[open_ai_key] = 0
 
     @staticmethod
     def get_active_thread_count():
         return threading.active_count() - 1
 
     def task_is_empty(self):
         return self.task_queue.empty()
 
     def add_task(self, tasks):
-        if tasks is None:
-            tasks = []
-        if len(tasks) == 0:
-            logging.info("The second additional task is empty")
-        self.task_run_tasks(tasks=tasks)
+        logging.info("Successfully added tasks: %s" % len(tasks))
+        for task in tasks:
+            self.task_queue.put(task)
 
     def __process_task(self, task, ask_content, messages, retries=1):
         open_ai_key = self.__get_key()
         if open_ai_key:
             case_name = task.get("case", None)
             need_system = task.get("need_system", False)
             call_back_func = task.get("call_back", None)
             retry = task.get("retry", False)
-            logging.info("case run: %s" % case_name)
+            logging.info("case run: 【%s】" % case_name)
             if self.system_content and need_system and not retry:
                 messages.append({"role": "system", "content": self.system_content})
-                logging.info("auto add role:system content: %s" % self.system_content)
+                logging.info("auto add role = system success ")
             if not retry:
                 messages.append({"role": "user", "content": ask_content})
             try:
                 start_time = time.time()
                 response = openai.ChatCompletion.create(
                     model=self.model,
                     messages=messages,
@@ -163,21 +158,19 @@
                 elapsed_time = time.time() - start_time
                 response_str = response['choices'][0]['message']['content']
                 messages.append({"role": response['choices'][0]['message']['role'], "content": response_str})
                 completion_tokens = response['usage']['completion_tokens']
                 prompt_tokens = response['usage']['prompt_tokens']
                 total_tokens = response['usage']['total_tokens']
                 self.total_tokens += total_tokens
-                logging.info("request case %s cost time: %s second" % (case_name, int(elapsed_time)))
+                logging.info("request case 【%s】 cost time: %s second" % (case_name, int(elapsed_time)))
                 logging.info("prompt tokens: %s" % prompt_tokens)
                 logging.info("completion tokens: %s" % completion_tokens)
                 logging.info("total tokens: %s" % total_tokens)
-                for openaiKey in self.usable_openai_keys:
-                    if openaiKey.get("api_key", None) == open_ai_key:
-                        openaiKey["token_limit"] += total_tokens
+                self.usable_openai_keys[open_ai_key] = total_tokens
                 if call_back_func and self.call_back:
                     call_back_func = self.call_back.get(call_back_func, None)
                     if call_back_func:
                         call_back_func(call_black_parameter(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name))
             except openai.error.RateLimitError as e:
                 logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
                 self.__release_token(open_ai_key)
@@ -200,127 +193,18 @@
 
 class GPTAsyncTaskManager(GPTTaskManager):
     def __init__(self, num_thread, keys, stream, max_retries, key_limit, model, temperature, top_p, presence_penalty, frequency_penalty, n, system_content, call_back=None):
         self.loop = asyncio.get_event_loop()
         self.task_queue = asyncio.Queue(maxsize=0)
         super(GPTAsyncTaskManager, self).__init__(num_thread, keys, stream=stream, max_retries=max_retries, key_limit=key_limit, model=model, temperature=temperature, top_p=top_p, presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, n=n, system_content=system_content, call_back=call_back)
 
-    async def __worker(self, run_func):
-        logging.disable(logging.NOTSET)
-        while True:
-            try:
-                task = await self.task_queue.get()
-                if task is None:
-                    break
-                content = task.get("ask")
-                messages = task.get("messages")
-                await run_func(task, content, messages)
-                self.task_queue.task_done()
-            except Empty:
-                break
-
-    async def __run_tasks(self, tasks, run_func):
-        workers = []
-        print("Total workers: %s" % self.num_threads)
-        print("Total tasks: %s" % len(tasks))
-        for task in tasks:
-            await self.task_queue.put(task)
-        for _ in range(self.num_threads):
-            worker = asyncio.create_task(self.__worker(run_func))
-            workers.append(worker)
-        await self.task_queue.join()
-        for worker in workers:
-            worker.cancel()
-
-    async def async_task_run_tasks(self, tasks):
-        await self.__run_tasks(tasks=tasks, run_func=self.__process_task)
-
-    async def __get_key(self):
-        async with self.key_lock:
-            while True:
-                sorted_data = sorted(self.usable_openai_keys, key=lambda x: x['token_limit'], reverse=True)
-                if len(sorted_data) <= 0:
-                    return False
-                open_ai_key = sorted_data[0].get("api_key")
-                token_limit = sorted_data[0].get("token_limit")
-                if open_ai_key and token_limit >= self.key_limit:
-                    logging.info("Token re election")
-                    continue
-                return open_ai_key
-
-    async def __process_task(self, task, ask_content, messages, retries=1, retry=False):
-        open_ai_key = await self.__get_key()
-        print(open_ai_key)
-        if open_ai_key:
-            case_name = task.get("case", None)
-            need_system = task.get("need_system", False)
-            call_back_func = task.get("call_back", None)
-            logging.info("case run: %s" % case_name)
-            if len(messages) == 0 and self.system_content and need_system:
-                messages.append({"role": "system", "content": self.system_content})
-                logging.info("auto add role:system content: %s" % self.system_content)
-            if not retry:
-                messages.append({"role": "user", "content": ask_content})
-            try:
-                start_time = time.time()
-                print(start_time)
-                completion_task = asyncio.create_task(
-                    openai.ChatCompletion.create(
-                        model=self.model,
-                        messages=messages,
-                        temperature=self.temperature,
-                        api_key=open_ai_key
-                    )
-                )
-                response = await completion_task
-                print(response)
-                # elapsed_time = time.time() - start_time
-                # response_str = response['choices'][0]['message']['content']
-                # messages.append({"role": response['choices'][0]['message']['role'], "content": response_str})
-                # completion_tokens = response['usage']['completion_tokens']
-                # prompt_tokens = response['usage']['prompt_tokens']
-                # total_tokens = response['usage']['total_tokens']
-                # self.total_tokens += total_tokens
-                # logging.info("request case %s cost time: %s second" % (case_name, int(elapsed_time)))
-                # logging.info("prompt tokens: %s" % prompt_tokens)
-                # logging.info("completion tokens: %s" % completion_tokens)
-                # logging.info("total tokens: %s" % total_tokens)
-                # for openaiKey in self.usable_openai_keys:
-                #     if openaiKey.get("api_key", None) == open_ai_key:
-                #         openaiKey["token_limit"] += total_tokens
-                # logging.info("active threads: %s" % self.get_active_thread_count())
-                # if self.task_is_empty():
-                #     logging.info("Total tokens consumed in this round: %s" % self.total_tokens)
-                # if call_back_func:
-                #     call_back_func(
-                #         call_black_parameter(response_str, messages, elapsed_time, completion_tokens, prompt_tokens,
-                #                              total_tokens, case_name))
-            except openai.error.RateLimitError as e:
-                logging.error(
-                    f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
-            #     self.__release_token(open_ai_key)
-            #     self.retry_on_error(task, ask_content, messages, retries=retries)
-            # except openai.error.Timeout as e:
-            #     logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request timed out: {e} ")
-            #     self.retry_on_error(task, ask_content, messages, retries=retries)
-            # except openai.error.APIConnectionError as e:
-            #     logging.error(
-            #         f"Retrying: {case_name}/{retries}, OpenAI API request timed out, OpenAI API request failed to connect: {e}")
-            #     self.retry_on_error(task, ask_content, messages, retries=retries)
-            # except openai.error.APIError as e:
-            #     logging.error(f"Retrying: {case_name}/{retries}, OpenAI API returned an API Error: {e}")
-            #     self.retry_on_error(task, ask_content, messages, retries=retries)
-        else:
-            await self.task_queue.put(task)
-
 
 class GPT4(GPTAsyncTaskManager):
     def __init__(self, keys=None, model='gpt-4', temperature=0, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, stream=False, system_content=None, num_threads=50, key_limit=4096, max_retries=3, call_back=None):
+        self.keys = keys
         super(GPT4, self).__init__(num_thread=num_threads, keys=keys, stream=stream, max_retries=max_retries, key_limit=key_limit, model=model, temperature=temperature, top_p=top_p, presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, n=n, system_content=system_content, call_back=call_back)
 
     def run_tasks(self, tasks):
         if not self.stream:
             logging.info("Mode: Multi threaded synchronous request gpt")
+            logging.info("total tokens: %s" % len(self.keys))
             self.task_run_tasks(tasks=tasks)
-        else:
-            logging.info("Mode: Multi threaded asynchronous request gpt")
-            self.loop.run_until_complete(self.async_task_run_tasks(tasks=tasks))
```

### Comparing `gpt4-api-0.1.7/setup.py` & `gpt4-api-0.1.8/setup.py`

 * *Files identical despite different names*

