# Comparing `tmp/replicator-cli-0.0.5.tar.gz` & `tmp/replicator-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicator-cli-0.0.5.tar", last modified: Sat May 27 13:44:36 2023, max compression
+gzip compressed data, was "replicator-cli-0.0.6.tar", last modified: Wed Jun  7 19:20:55 2023, max compression
```

## Comparing `replicator-cli-0.0.5.tar` & `replicator-cli-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.5/README.md
--rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2772 2023-05-27 13:30:42.000000 replicator-cli-0.0.5/app.py
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       17 2023-05-27 13:42:14.000000 replicator-cli-0.0.5/meta.py
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      671 2023-05-27 13:01:13.000000 replicator-cli-0.0.5/notifier.py
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/replicator_cli.egg-info/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      275 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/entry_points.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/requires.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       18 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/top_level.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/setup.cfg
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      974 2023-05-27 13:37:07.000000 replicator-cli-0.0.5/setup.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     1091 2023-06-07 16:04:30.000000 replicator-cli-0.0.6/LICENSE
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2398 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-06-07 16:04:30.000000 replicator-cli-0.0.6/README.md
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       17 2023-06-07 16:09:14.000000 replicator-cli-0.0.6/meta.py
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      969 2023-06-07 18:23:00.000000 replicator-cli-0.0.6/notifier.py
+-rwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)     3666 2023-06-07 19:17:09.000000 replicator-cli-0.0.6/replicator.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/replicator_cli.egg-info/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2398 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      290 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       39 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/requires.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       25 2023-06-07 19:20:55.000000 replicator-cli-0.0.6/replicator_cli.egg-info/top_level.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-06-07 19:20:55.914887 replicator-cli-0.0.6/setup.cfg
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      981 2023-06-07 16:06:48.000000 replicator-cli-0.0.6/setup.py
```

### Comparing `replicator-cli-0.0.5/PKG-INFO` & `replicator-cli-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
-Description: Replicator is a task runner for backups.
-        
-        You can describe your tasks declarative with YAML file and run task files with CRON.
-        
-        Replicator supports notifications, it's useful for tasks that take a lot of time.
-        
-        ## Install
-        
-        Install from pip `pip install replicator-cli`
-        
-        Or build:
-        - Clone repository `git clone https://github.com/vitonsky/replicator.git`
-        - Build package with run `make build`
-        - Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
-        
-        ## Usage
-        
-        ```
-        usage: replicator [-h] config
-        
-        Util to replicate backups from primary storage to a mirrors
-        
-        positional arguments:
-          config      Path to config file
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        To use util, first create task file.
-        
-        Example task file for a local device
-        ```yml
-        tasks:
-            # Task may have name
-            - name: 'Copy files to backup disk'
-              run: rclone ./backups /path/to/local/mirror1
-        
-            - name: 'Upload to S3'
-              run: rclone ./backups s3Replica:backups
-        
-            - name: 'Replicate on server'
-              # Just run replicator on server with their own config and end locally
-              run: ssh replicator@backup-server 'nohup replicator ./backups.yml > ./replicator.log 2>&1 </dev/null &'
-        ```
-        
-        Example task file for backup server
-        ```yml
-        # Notifications config
-        notifications:
-            telegram:
-                # Define should notifications been sent
-                enabled: true
-                # Token for bot who will sent notifications
-                # How to: https://core.telegram.org/bots/tutorial#getting-ready
-                botToken: '123:token'
-                # User IDs to receive notifications
-                userIds:
-                    - 123456
-        
-        # Replicate backup from main storage
-        tasks:
-            - run: rclone s3Replica:backups s3Mirror1:backups
-            - run: rclone s3Replica:backups s3Mirror2:backups
-            - run: rclone s3Replica:backups s3Mirror3:backups
-        ```
-        
-        ## TODO
-        - [x] Support few entries for replication
-        - [x] Provide commands to run, instead of paths
-        - [x] Provide instructions to install as binary
-        - [ ] Split the code
-        - [ ] Add docker image
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Replicator is a task runner for backups.
+
+You can describe your tasks declarative with YAML file and run task files with CRON.
+
+Replicator supports notifications, it's useful for tasks that take a lot of time.
+
+## Install
+
+Install from pip `pip install replicator-cli`
+
+Or build:
+- Clone repository `git clone https://github.com/vitonsky/replicator.git`
+- Build package with run `make build`
+- Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
+
+## Usage
+
+```
+usage: replicator [-h] config
+
+Util to replicate backups from primary storage to a mirrors
+
+positional arguments:
+  config      Path to config file
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+To use util, first create task file.
+
+Example task file for a local device
+```yml
+tasks:
+    # Task may have name
+    - name: 'Copy files to backup disk'
+      run: rclone ./backups /path/to/local/mirror1
+
+    - name: 'Upload to S3'
+      run: rclone ./backups s3Replica:backups
+
+    - name: 'Replicate on server'
+      # Just run replicator on server with their own config and end locally
+      run: ssh replicator@backup-server 'nohup replicator ./backups.yml > ./replicator.log 2>&1 </dev/null &'
+```
+
+Example task file for backup server
+```yml
+# Notifications config
+notifications:
+    telegram:
+        # Define should notifications been sent
+        enabled: true
+        # Token for bot who will sent notifications
+        # How to: https://core.telegram.org/bots/tutorial#getting-ready
+        botToken: '123:token'
+        # User IDs to receive notifications
+        userIds:
+            - 123456
+
+# Replicate backup from main storage
+tasks:
+    - run: rclone s3Replica:backups s3Mirror1:backups
+    - run: rclone s3Replica:backups s3Mirror2:backups
+    - run: rclone s3Replica:backups s3Mirror3:backups
+```
+
+## TODO
+- [x] Support few entries for replication
+- [x] Provide commands to run, instead of paths
+- [x] Provide instructions to install as binary
+- [ ] Split the code
+- [ ] Add docker image
```

### Comparing `replicator-cli-0.0.5/README.md` & `replicator-cli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.5/app.py` & `replicator-cli-0.0.6/replicator.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,67 +18,86 @@
     parser.add_argument('config', help="Path to config file")
 
     args = parser.parse_args()
 
     config = yaml.load(open(args.config), Loader=yaml.Loader)
 
     # Configure notifier
-    notifier = None
+    token = None
+    users = None
+    notifierPrefix = None
     if ('notifications' in config):
         token = config['notifications']['telegram']['botToken']
         users = config['notifications']['telegram']['userIds']
-
-        notifier = TelegramNotifier(token, users)
+        notifierPrefix = config['notifications'].get('prefix')
+    notifier = TelegramNotifier(token, users)
+    notifier.setPrefix(notifierPrefix)
 
     # Run tasks
-    for task in config['tasks']:
+    for taskId, task in enumerate(config['tasks']):
         taskName = task['name'] if 'name' in task else task['run']
+        escapedTaskName = notifier.escapeText(taskName)
+
+        newLinePrefix = '\n' if taskId != 0 else ''
+        print(newLinePrefix + f'Task "{taskName}"', flush=True)
 
-        print(f'Run command "{taskName}"', flush=True)
+        # Skip by condition
+        if 'if' in task:
+            ifCmd = subprocess.Popen(task['if'], shell=True)
+            ifCmd.wait()
+            if ifCmd.returncode != 0:
+                print(f'Skip task "{taskName}"', flush=True)
+                await notifier.notify(f'Skip task "{escapedTaskName}"')
+                continue
 
         # Run command
-        # TODO: add timeout to stop process
-        cmd = task['run']
-        replicationProcess = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-        outLines = []
-        for rawLine in iter(replicationProcess.stdout.readline, b''):
-            line = rawLine.decode('utf-8')
-
-            # Print output to console
-            sys.stdout.write(line)
-
-            # Remove old lines out of limit
-            if (reportLinesLimit > 0):
-                freeSlots = reportLinesLimit - len(outLines)
-                if (freeSlots <= 0):
-                    slotsToRemove = -freeSlots + 1
-                    outLines = outLines[slotsToRemove:]
-
-            # Add lines
-            outLines.append(line)
-        replicationProcess.stdout.close()
-        replicationProcess.wait()
-
-        isRunSuccessful = replicationProcess.returncode == 0
-
-        # Notify result
-        if notifier is not None:
-            notifications = config['notifications']
-            notificationPrefix = '*' + notifications['prefix'] + '*: ' if 'prefix' in notifications else ''
+        commands = task['run'] if isinstance(task['run'], list) else [task['run']]
+        for cmdIndex, command in enumerate(commands):
+            print(f'Run command "{command}"', flush=True)
+
+            # TODO: add timeout to stop process
+            replicationProcess = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            outLines = []
+            for rawLine in iter(replicationProcess.stdout.readline, b''):
+                line = rawLine.decode('utf-8')
+
+                # Print output to console
+                sys.stdout.write(line)
+
+                # Remove old lines out of limit
+                if (reportLinesLimit > 0):
+                    freeSlots = reportLinesLimit - len(outLines)
+                    if (freeSlots <= 0):
+                        slotsToRemove = -freeSlots + 1
+                        outLines = outLines[slotsToRemove:]
+
+                # Add lines
+                outLines.append(line)
+            replicationProcess.stdout.close()
+            replicationProcess.wait()
+
+            isRunSuccessful = replicationProcess.returncode == 0
+
+            # Notify result
+            totalCommandsLen = len(commands)
+            messageTargetSuffix = f'- command {cmdIndex + 1}/{totalCommandsLen}' if totalCommandsLen > 1 else ''
+            messageTarget = f'Task "{escapedTaskName}"' + notifier.escapeText(messageTargetSuffix)
 
-            escapedTaskName = notifier.escapeText(taskName)
             if isRunSuccessful:
-                await notifier.notify(notificationPrefix + f'Task "{escapedTaskName}" final successful')
+                await notifier.notify(f'{messageTarget} final successful')
             else:
                 # add last few lines to explain context
                 lastLog = notifier.escapeText(''.join(outLines))
-                await notifier.notify(notificationPrefix + f'⚠️ Task "{escapedTaskName}" are failed\n\n```\n...\n{lastLog}\n```')
+                await notifier.notify(f'⚠️ {messageTarget} has failed\n\n```\n...\n{lastLog}\n```')
+
+            # Stop the program for fails
+            if not isRunSuccessful:
+                exit(replicationProcess.returncode)
 
-        # Stop the program for fails
-        if not isRunSuccessful:
-            exit(replicationProcess.returncode)
+    # Final
+    await notifier.notify(f'🎉 All tasks has final successful')
 
 
 def cli():
     asyncio.run(main())
```

### Comparing `replicator-cli-0.0.5/notifier.py` & `replicator-cli-0.0.6/notifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 import telegram
 
 class TelegramNotifier:
     _bot = None
     _users = []
 
     def __init__(self, token, users):
-        self._bot = telegram.Bot(token)
-        self._users = users
+        if token is not None and users is not None:
+            self._bot = telegram.Bot(token)
+            self._users = users
+
+    _prefix = None
+    def setPrefix(self, prefix: str):
+        self._prefix = prefix
 
     def escapeText(self, text: str):
         chars = '|'.join(list(map(lambda char: re.escape(char), r'_*[]()~`>#+-=|{}.!')))
         return re.sub(r'(' + chars + r')', r'\\\1', text)
     
     async def notify(self, text):
         # Skip if can't notify
         if not self._bot or len(self._users) == 0: return
 
         async with self._bot:
             for userId in self._users:
-                await self._bot.send_message(text=text, chat_id=userId, parse_mode='MarkdownV2')
+                notificationPrefix = f'*{self._prefix}*: ' if self._prefix is not None else ''
+                message = notificationPrefix + text
+                await self._bot.send_message(text=message, chat_id=userId, parse_mode='MarkdownV2')
```

### Comparing `replicator-cli-0.0.5/replicator_cli.egg-info/PKG-INFO` & `replicator-cli-0.0.6/replicator_cli.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
-Description: Replicator is a task runner for backups.
-        
-        You can describe your tasks declarative with YAML file and run task files with CRON.
-        
-        Replicator supports notifications, it's useful for tasks that take a lot of time.
-        
-        ## Install
-        
-        Install from pip `pip install replicator-cli`
-        
-        Or build:
-        - Clone repository `git clone https://github.com/vitonsky/replicator.git`
-        - Build package with run `make build`
-        - Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
-        
-        ## Usage
-        
-        ```
-        usage: replicator [-h] config
-        
-        Util to replicate backups from primary storage to a mirrors
-        
-        positional arguments:
-          config      Path to config file
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        To use util, first create task file.
-        
-        Example task file for a local device
-        ```yml
-        tasks:
-            # Task may have name
-            - name: 'Copy files to backup disk'
-              run: rclone ./backups /path/to/local/mirror1
-        
-            - name: 'Upload to S3'
-              run: rclone ./backups s3Replica:backups
-        
-            - name: 'Replicate on server'
-              # Just run replicator on server with their own config and end locally
-              run: ssh replicator@backup-server 'nohup replicator ./backups.yml > ./replicator.log 2>&1 </dev/null &'
-        ```
-        
-        Example task file for backup server
-        ```yml
-        # Notifications config
-        notifications:
-            telegram:
-                # Define should notifications been sent
-                enabled: true
-                # Token for bot who will sent notifications
-                # How to: https://core.telegram.org/bots/tutorial#getting-ready
-                botToken: '123:token'
-                # User IDs to receive notifications
-                userIds:
-                    - 123456
-        
-        # Replicate backup from main storage
-        tasks:
-            - run: rclone s3Replica:backups s3Mirror1:backups
-            - run: rclone s3Replica:backups s3Mirror2:backups
-            - run: rclone s3Replica:backups s3Mirror3:backups
-        ```
-        
-        ## TODO
-        - [x] Support few entries for replication
-        - [x] Provide commands to run, instead of paths
-        - [x] Provide instructions to install as binary
-        - [ ] Split the code
-        - [ ] Add docker image
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Replicator is a task runner for backups.
+
+You can describe your tasks declarative with YAML file and run task files with CRON.
+
+Replicator supports notifications, it's useful for tasks that take a lot of time.
+
+## Install
+
+Install from pip `pip install replicator-cli`
+
+Or build:
+- Clone repository `git clone https://github.com/vitonsky/replicator.git`
+- Build package with run `make build`
+- Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
+
+## Usage
+
+```
+usage: replicator [-h] config
+
+Util to replicate backups from primary storage to a mirrors
+
+positional arguments:
+  config      Path to config file
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+To use util, first create task file.
+
+Example task file for a local device
+```yml
+tasks:
+    # Task may have name
+    - name: 'Copy files to backup disk'
+      run: rclone ./backups /path/to/local/mirror1
+
+    - name: 'Upload to S3'
+      run: rclone ./backups s3Replica:backups
+
+    - name: 'Replicate on server'
+      # Just run replicator on server with their own config and end locally
+      run: ssh replicator@backup-server 'nohup replicator ./backups.yml > ./replicator.log 2>&1 </dev/null &'
+```
+
+Example task file for backup server
+```yml
+# Notifications config
+notifications:
+    telegram:
+        # Define should notifications been sent
+        enabled: true
+        # Token for bot who will sent notifications
+        # How to: https://core.telegram.org/bots/tutorial#getting-ready
+        botToken: '123:token'
+        # User IDs to receive notifications
+        userIds:
+            - 123456
+
+# Replicate backup from main storage
+tasks:
+    - run: rclone s3Replica:backups s3Mirror1:backups
+    - run: rclone s3Replica:backups s3Mirror2:backups
+    - run: rclone s3Replica:backups s3Mirror3:backups
+```
+
+## TODO
+- [x] Support few entries for replication
+- [x] Provide commands to run, instead of paths
+- [x] Provide instructions to install as binary
+- [ ] Split the code
+- [ ] Add docker image
```

### Comparing `replicator-cli-0.0.5/setup.py` & `replicator-cli-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     author_email = 'rob@vitonsky.net',
     license = 'MIT',
     description = 'Task runner for backups',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/vitonsky/replicator',
     py_modules = [
-        'app',
+        'replicator',
         'meta',
         'notifier',
     ],
     packages = find_packages(),
     install_requires = [requirements],
     python_requires='>=3.7',
     classifiers=[
```

