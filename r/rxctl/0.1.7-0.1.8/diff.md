# Comparing `tmp/rxctl-0.1.7.tar.gz` & `tmp/rxctl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxctl-0.1.7.tar", max compression
+gzip compressed data, was "rxctl-0.1.8.tar", max compression
```

## Comparing `rxctl-0.1.7.tar` & `rxctl-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     4462 2023-03-03 08:32:21.460839 rxctl-0.1.7/README.md
--rw-r--r--   0        0        0      581 2023-03-03 08:36:33.410697 rxctl-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       49 2023-03-03 08:36:33.410697 rxctl-0.1.7/rxctl/__init__.py
--rw-r--r--   0        0        0      262 2022-12-12 10:21:43.256203 rxctl-0.1.7/rxctl/bin/__init
--rwxr-xr-x   0        0        0      356 2022-12-16 14:17:41.837487 rxctl-0.1.7/rxctl/bin/__run
--rwxr-xr-x   0        0        0      626 2022-12-21 06:45:47.235315 rxctl-0.1.7/rxctl/bin/__wait
--rwxr-xr-x   0        0        0     3986 2023-01-30 08:09:39.963436 rxctl-0.1.7/rxctl/lib/ansible.sh
--rw-r--r--   0        0        0      428 2023-03-03 08:35:34.726267 rxctl-0.1.7/rxctl/lib/links.json
--rw-r--r--   0        0        0      666 2022-12-18 17:03:07.749954 rxctl-0.1.7/rxctl/lib/links.py
--rwxr-xr-x   0        0        0     3085 2022-12-19 11:53:03.688191 rxctl-0.1.7/rxctl/lib/log.py
--rw-r--r--   0        0        0    13290 2023-03-03 08:24:41.521287 rxctl-0.1.7/rxctl/lib/main.py
--rwxr-xr-x   0        0        0      439 2023-01-03 10:08:29.507259 rxctl-0.1.7/rxctl/lib/scp.sh
--rw-r--r--   0        0        0     2099 2023-02-28 08:15:28.892300 rxctl-0.1.7/rxctl/lib/utils.py
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 rxctl-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 16:18:25.633562 rxctl-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4462 2023-03-03 08:32:21.460839 rxctl-0.1.8/README.md
+-rw-r--r--   0        0        0      590 2023-06-07 16:19:06.142349 rxctl-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 14:22:03.305033 rxctl-0.1.8/rxctl/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-07 16:19:06.142349 rxctl-0.1.8/rxctl/__version__.py
+-rw-r--r--   0        0        0      262 2022-12-12 10:21:43.256203 rxctl-0.1.8/rxctl/bin/__init
+-rwxr-xr-x   0        0        0      356 2022-12-16 14:17:41.837487 rxctl-0.1.8/rxctl/bin/__run
+-rwxr-xr-x   0        0        0      626 2022-12-21 06:45:47.235315 rxctl-0.1.8/rxctl/bin/__wait
+-rwxr-xr-x   0        0        0     3986 2023-01-30 08:09:39.963436 rxctl-0.1.8/rxctl/lib/ansible.sh
+-rw-r--r--   0        0        0      428 2023-03-03 08:36:35.590713 rxctl-0.1.8/rxctl/lib/links.json
+-rw-r--r--   0        0        0      703 2023-06-07 15:01:53.479017 rxctl-0.1.8/rxctl/lib/links.py
+-rwxr-xr-x   0        0        0     3096 2023-06-07 15:07:50.442648 rxctl-0.1.8/rxctl/lib/log.py
+-rw-r--r--   0        0        0    14813 2023-06-07 16:16:28.179133 rxctl-0.1.8/rxctl/lib/main.py
+-rwxr-xr-x   0        0        0      439 2023-01-03 10:08:29.507259 rxctl-0.1.8/rxctl/lib/scp.sh
+-rw-r--r--   0        0        0     2188 2023-06-07 15:15:48.552838 rxctl-0.1.8/rxctl/lib/utils.py
+-rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 rxctl-0.1.8/PKG-INFO
```

### Comparing `rxctl-0.1.7/README.md` & `rxctl-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.7/pyproject.toml` & `rxctl-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rxctl"
-version = "0.1.7"
+version = "0.1.8"
 description = "Linux remote execution tool"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/rxctl"
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -12,15 +12,15 @@
 prettytable = "*"
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "./rxctl/lib/links.py"
 
 [tool.poetry.scripts]
-rxctl = "rxctl:cli"
+rxctl = "rxctl.lib.main:cli"
 
 [tool.poetry-dynamic-versioning]
 enable = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `rxctl-0.1.7/rxctl/bin/__wait` & `rxctl-0.1.8/rxctl/bin/__wait`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.7/rxctl/lib/ansible.sh` & `rxctl-0.1.8/rxctl/lib/ansible.sh`

 * *Files identical despite different names*

### Comparing `rxctl-0.1.7/rxctl/lib/log.py` & `rxctl-0.1.8/rxctl/lib/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 
 import logging
 import sys
 import click
 import os
 
+
 class CustomFormatter(logging.Formatter):
 
     colors = {
         logging.NOTSET: 'reset',
         logging.DEBUG: 'cyan',
         logging.INFO: 'green',
         logging.WARNING: 'yellow',
         logging.ERROR: 'red',
         logging.CRITICAL: 'red'
     }
 
-    
     level = logging.INFO
     prompt = '-->'
 
     def set_label(self, label):
         if label:
             self.label = label
         else:
@@ -34,31 +34,32 @@
         msg0 = msg[0]
         if len(msg) > 1:
             msg1 = '\n{}'.format('\n'.join(msg[1:]))
         else:
             msg1 = ''
         # Colorize only first line off message
         record.msg = '{}{}'.format(click.style(msg0, fg=c), msg1)
-        
+
         # Timestamp if debug enabled
         if self.level == logging.DEBUG:
             ts = click.style(' %(asctime)s', fg=c)
         else:
             ts = ''
 
         level = click.style('%(levelname)s', fg=c, bold=True)
         if self.label.endswith(self.prompt):
             label = self.label
         else:
             label = '[{}]'.format(click.style(self.label, fg=c))
-        
+
         log_fmt = '{}{} {}: %(message)s'.format(label, ts, level)
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
+
 class Logger(logging.Logger):
     def __init__(self, name):
         super().__init__(name)
         self.setLevel(logging.INFO)
         self.fmt = CustomFormatter()
         lh = logging.StreamHandler(sys.stderr)
         lh.setFormatter(self.fmt)
@@ -70,18 +71,20 @@
         else:
             self.setLevel(logging.INFO)
         self.fmt.level = self.level
 
     def set_label(self, label=None):
         self.fmt.set_label(label)
 
+
 logging.setLoggerClass(Logger)
 LOG = logging.getLogger(__name__)
 
-if 'RX_LOG_VERBOSITY' in os.environ and int(os.environ['RX_LOG_VERBOSITY']) > 0:
+if 'RX_LOG_VERBOSITY' in os.environ \
+        and int(os.environ['RX_LOG_VERBOSITY']) > 0:
     LOG.enable_debug()
 
 if 'RX_HOST' in os.environ:
     label = os.environ['RX_HOST']
     if 'RX_TASK' in os.environ:
         label = '{}/{}'.format(os.environ['RX_HOST'], os.environ['RX_TASK'])
 else:
@@ -102,15 +105,16 @@
     if len(sys.argv) >= 2 and level[-1] in levelmap:
         level = level[-1]
         msg = ' '.join(sys.argv[1:])
     elif len(sys.argv) >= 3 and sys.argv[1] in levelmap:
         level = sys.argv[1]
         msg = ' '.join(sys.argv[2:])
     else:
-        print('{} {} message'.format(os.path.basename(__file__), '|'.join(levelmap.keys()))) 
+        print('{} {} message'.format(
+            os.path.basename(__file__), '|'.join(levelmap.keys())
+        ))
         sys.exit(2)
 
     LOG.log(levelmap[level], msg)
 
     if level == 'error':
         sys.exit(1)
-
```

### Comparing `rxctl-0.1.7/rxctl/lib/main.py` & `rxctl-0.1.8/rxctl/lib/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,118 @@
 
 from .log import LOG
 from . import links
 from .utils import *
+from ..__version__ import __version__
 
 import sys
 import os
 import subprocess
 import getpass
 import shlex
 from multiprocessing import Pool
 from types import SimpleNamespace
 
 from prettytable import PrettyTable
 import click
 
+
 def get_config(ctx, param, value):
     ctx.default_map = get_environment(value, 'config')
     return value
 
+
 @click.command(
     context_settings=dict(
-        ignore_unknown_options = True,
-        allow_interspersed_args = False
+        ignore_unknown_options=True,
+        allow_interspersed_args=False
     ),
 )
 @click.option(
-    '-E', '--environment', 
-    default='./environment', 
-    show_default=True, 
+    '-E', '--environment',
+    default='./environment',
+    show_default=True,
     help='Script to generate environment (config & inventory)',
     type=click.Path(),
     callback=get_config,
     is_eager=True
 )
-@click.option('-H', '--host', default=[], help='Comma separated list of host (can be used multiple times)', multiple=True)
-@click.option('-S', '--selector', default=[], help='Inventory selector (can be used multiple times)', multiple=True)
-@click.option('--use-ssh-password', default=False, is_flag=True, help='Ask for ssh password')
-@click.option('--use-sudo-password', default=False, is_flag=True, help='Ask for sudo password')
-@click.option('--ssh-opt', default='-o ControlMaster=auto -o ControlPath=/dev/shm/rx-ssh-%h -o ControlPersist=5m -o ConnectTimeout=1', show_default=True, help='SSH options')
-@click.option('--password-envvar', default='LC_PASSWD', show_default=True, help='Environment variable used to pass password to sudo')
-@click.option('-u', '--user', default=os.environ['USER'], show_default=True, help='SSH user')
-@click.option('-P', '--parallel', default=1, show_default=True, help='How many threads to use to run hosts in parallel')
-@click.option('-A', '--ad-hoc', default=False, is_flag=True, help='Task list is a remote ad-hoc command')
-@click.option('-I', '--inventory', default=False, is_flag=True, help='Show environment inventory')
-@click.option('-c', '--check-only', default=False, is_flag=True, help='Show valid inventory')
-@click.option('-l', '--task-list', default=False, is_flag=True, help='List tasks in local directory')
-@click.option('-t', '--task-help', default=None, help='Show help for a task')
-@click.option('-w', '--warning-only', default=False, is_flag=True, help="Don't exit if a host fails check, evict host from inventory")
-@click.option('-x', '--exclude', default=[], help='Comma separated list of host to exclude from inventory (can be used multiple times)', multiple=True)
-@click.option('-i', '--inline-check', default=False, is_flag=True, help="Don't check hosts before tasks, do it for each host at the begining of the task list")
-@click.option('--set-env', default=[], show_default=True, help='Set environment variable (can be used multiple times)', multiple=True)
-@click.option('-v', '--verbosity', count=True, default=0, help='Verbosity level, up to 3')
+@click.option('-H', '--host', default=[],
+              help='Comma separated list of host (can be used multiple times)',
+              multiple=True)
+@click.option('-S', '--selector', default=[],
+              help='Inventory selector (can be used multiple times)',
+              multiple=True)
+@click.option('--use-ssh-password', default=False, is_flag=True,
+              help='Ask for ssh password')
+@click.option('--use-sudo-password', default=False, is_flag=True,
+              help='Ask for sudo password')
+@click.option('--ssh-opt', default='-o ControlMaster=auto'
+              ' -o ControlPath=/dev/shm/rx-ssh-%h'
+              ' -o ControlPersist=5m -o ConnectTimeout=1',
+              show_default=True, help='SSH options')
+@click.option('--password-envvar', default='LC_PASSWD', show_default=True,
+              help='Environment variable used to pass password to sudo')
+@click.option('-u', '--user', default=os.environ['USER'], show_default=True,
+              help='SSH user')
+@click.option('-P', '--parallel', default=False, is_flag=True,
+              help='Run hosts in parallel')
+@click.option('--max-parallel', default=0, show_default=True,
+              help='How many threads to use to run hosts in parallel,'
+              ' 0 - run everithing in parralel')
+@click.option('-A', '--ad-hoc', default=False, is_flag=True,
+              help='Task list is a remote ad-hoc command')
+@click.option('-I', '--inventory', default=False, is_flag=True,
+              help='Show environment inventory')
+@click.option('-c', '--check-only', default=False, is_flag=True,
+              help='Show valid inventory')
+@click.option('-l', '--task-list', default=False, is_flag=True,
+              help='List tasks in local directory')
+@click.option('-t', '--task-help', default=None,
+              help='Show help for a task')
+@click.option('-w', '--warning-only', default=False, is_flag=True,
+              help="Don't exit if a host fails check,"
+              " evict host from inventory")
+@click.option('-x', '--exclude', default=[],
+              help='Comma separated list of host to exclude from inventory'
+              ' (can be used multiple times)',
+              multiple=True)
+@click.option('-i', '--inline-check', default=False, is_flag=True,
+              help="Don't check hosts before tasks,"
+              " do it for each host at the begining of the task list")
+@click.option('--set-env', default=[], show_default=True,
+              help='Set environment variable (can be used multiple times)',
+              multiple=True)
+@click.option('-v', '--verbosity', count=True, default=0,
+              help='Verbosity level, up to 3')
 @click.argument('tasks', nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
-def cli(cc, environment, host, selector, use_ssh_password, use_sudo_password, ssh_opt, password_envvar, user, parallel, ad_hoc, inventory, check_only, task_list, task_help, warning_only, exclude, inline_check, set_env, verbosity, tasks):
+@click.version_option(__version__, '-V', '--version')
+def cli(cc,
+        environment,
+        host,
+        selector,
+        use_ssh_password,
+        use_sudo_password,
+        ssh_opt,
+        password_envvar,
+        user,
+        parallel,
+        max_parallel,
+        ad_hoc,
+        inventory,
+        check_only,
+        task_list,
+        task_help,
+        warning_only,
+        exclude,
+        inline_check,
+        set_env,
+        verbosity,
+        tasks):
 
     # Non-configurable parameters
     remote_shell = '/bin/sh'
     passwd_script = 'rx-passwd'
     passwd_code = '#!/bin/bash\necho "${}"\n'.format(password_envvar)
 
     # Debug logging
@@ -66,78 +121,83 @@
     if verbosity > 0:
         LOG.enable_debug()
         if verbosity > 2:
             ssh_opt = '{} -v'.format(ssh_opt)
 
     # Restore bin links
     links.restore()
-    
-    # Debug parameters, actual values 
-    for k,v in cc.params.items():
+
+    # Debug parameters, actual values
+    for k, v in cc.params.items():
         LOG.debug('{}: {}'.format(k, v))
 
     # Check arguments - 1
-    if (len(selector) == 0 and len(host) == 0) and not (task_list or task_help or inventory):
-        LOG.error('At least one of -l, -t, -I, -H, -S or --help must be specified.')
+    if (len(selector) == 0 and len(host) == 0) and \
+            not (task_list or task_help or inventory):
+        LOG.error('At least one of'
+                  ' -l, -t, -I, -H, -S, -V'
+                  ' or --help must be specified.')
         sys.exit(1)
 
     # Set path
     basedir = os.path.dirname(os.path.realpath(__file__ + '/..'))
-    path = '{}:{}/bin'.format(os.getcwd(),basedir)
+    path = '{}:{}/bin'.format(os.getcwd(), basedir)
     LOG.info('Path: {}:$PATH'.format(path))
     os.environ['PATH'] = '{}:{}'.format(path, os.environ['PATH'])
 
     # List tasks in current director
     if task_list:
         p = PrettyTable()
         p.field_names = ['Task', 'Description']
         p.align['Task'] = 'r'
         p.align['Description'] = 'l'
         for t in get_tasks():
-            p.add_row([click.style(t, fg='blue', bold=True), task_doc(t, short=True)])
+            p.add_row([click.style(t, fg='blue', bold=True),
+                      task_doc(t, short=True)])
         print(p)
         sys.exit()
 
     # Task help
     if task_help:
         LOG.info('Task help:')
         print()
         print(click.style(task_help, fg='blue', bold=True))
         print(task_doc(task_help))
         sys.exit()
 
     # Inventory summary
     if inventory and not selector:
-        LOG.info('Inventory summary:\n{}'.format(get_environment(environment, 'inventory')))
+        LOG.info('Inventory summary:\n{}'.format(
+            get_environment(environment, 'inventory')))
         sys.exit()
 
     # Check arguments - 2
     if not (inventory or check_only) and len(tasks) == 0:
         LOG.error('At least one of -I, -c, -A or a task must be specified.')
         sys.exit(1)
 
-    # Build inventory, each host is added only once, first occurence, -H has priority over -S
+    # Build inventory, each host is added only once,
+    # first occurence, -H has priority over -S
     INVENTORY = []
     for hlist in host:
         for h in hlist.split(','):
-            if not h in INVENTORY:
+            if h not in INVENTORY:
                 INVENTORY.append(h)
     for s in selector:
         host = get_environment(environment, 'inventory', s)
         if host:
             for h in host:
-                if not h in INVENTORY:
+                if h not in INVENTORY:
                     INVENTORY.append(h)
     for xlist in exclude:
         for x in xlist.split(','):
             if x in INVENTORY:
                 LOG.debug("Remove '{}' from inventory".format(x))
                 INVENTORY.remove(x)
-    
-    
+
     # Show inventory
     if inventory:
         LOG.info('Inventory:\n{}'.format(INVENTORY))
         sys.exit()
 
     # Get password
     passwd = []
@@ -147,15 +207,15 @@
         passwd.append('SUDO')
     if len(passwd) > 0:
         passwd = getpass.getpass('--> {} password : '.format('/'.join(passwd)))
 
     # Build environment
     os.environ['RX_SHELL'] = remote_shell
     os.environ['RX_BASEDIR'] = basedir
-    if parallel > 1:
+    if parallel:
         os.environ['RX_PARALLEL'] = 'yes'
     os.environ['RX_PASSWD_SCRIPT'] = passwd_script
     os.environ['RX_USER'] = user
     os.environ['RX_PASSWD_ENVVAR'] = password_envvar
     ssh_opt = '{} -o User={}'.format(ssh_opt, user)
     os.environ['RX_SSH_OPT'] = ssh_opt
     ssh_cmd = 'ssh {}'.format(ssh_opt)
@@ -181,23 +241,26 @@
     ctx = SimpleNamespace()
     ctx.ssh_cmd = ssh_cmd
     ctx.sudo_cmd = sudo_cmd
     ctx.use_sudo_password = use_sudo_password
     ctx.passwd_script = passwd_script
     ctx.passwd_code = passwd_code
     ctx.ad_hoc = ad_hoc
-    ctx.parallel = parallel > 1
+    ctx.parallel = parallel
     ctx.warning_only = warning_only
     ctx.inline_check = inline_check
 
     # Check hosts
-    if check_only or not inline_check: 
+    if check_only or not inline_check:
         LOG.info('Check hosts connectivity')
         invalid_hosts = []
-        with click.progressbar(INVENTORY, bar_template='    [%(bar)s] %(info)s', show_eta=False, item_show_func=lambda x : x) as pbar:
+        with click.progressbar(INVENTORY,
+                               bar_template='    [%(bar)s] %(info)s',
+                               show_eta=False,
+                               item_show_func=lambda x: x) as pbar:
             for h in pbar:
                 LOG.set_label(h)
                 if verbosity > 0:
                     print()
                 valid_host, msg = check(h, ctx)
                 if not valid_host:
                     if verbosity == 0:
@@ -214,131 +277,155 @@
             LOG.warning('Remove from inventory:\n{}'.format(invalid_hosts))
         LOG.info('Valid inventory:\n{}'.format(INVENTORY))
     if check_only:
         sys.exit()
 
     # Build TASK list
     if ad_hoc:
-       TASKS = ' '.join(tasks) 
+        TASKS = ' '.join(tasks)
     else:
         TASKS = []
         cmd = {}
         for t in tasks:
             if t.startswith('__'):
                 if not check_task(t):
                     LOG.error('Invalid task: {}'.format(t))
                     sys.exit(1)
                 if len(cmd) > 0:
                     TASKS.append(cmd)
-                cmd = {'name':t, 'args':''}
+                cmd = {'name': t, 'args': ''}
             else:
                 if ' ' in t:
                     cmd['args'] = '{}"{}" '.format(cmd['args'], t)
                 else:
                     cmd['args'] = '{}{} '.format(cmd['args'], t)
         if cmd:
             TASKS.append(cmd)
         LOG.info('Task list:\n{}'.format(TASKS))
 
     worker_parameters = []
     common_parameters = [TASKS, ctx]
     for h in INVENTORY:
-             worker_parameters.append([h] + common_parameters)
+        worker_parameters.append([h] + common_parameters)
 
-    if parallel > 1:
+    if parallel:
+        if max_parallel == 0:
+            max_parallel = len(INVENTORY)
         LOG.debug('Parralel processing')
-        with Pool(processes=parallel, maxtasksperchild=1) as pool:
+        with Pool(processes=max_parallel, maxtasksperchild=1) as pool:
             pool.starmap(worker, worker_parameters)
     else:
         for p in worker_parameters:
             worker(*p)
 
 
 def worker(host, task_list, ctx):
     def run(cmd, label):
         LOG.debug('Worker cmd: {}'.format(cmd))
         if label:
-            p = subprocess.Popen(cmd, shell=True, encoding='utf-8', errors='ignore', bufsize=0, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-            for l in iter(p.stdout.readline,''):
-                if l.startswith('['):
-                    print(l, end='')
+            p = subprocess.Popen(cmd, shell=True, encoding='utf-8',
+                                 errors='ignore', bufsize=0,
+                                 stdout=subprocess.PIPE,
+                                 stderr=subprocess.STDOUT)
+            for ln in iter(p.stdout.readline, ''):
+                if ln.startswith('['):
+                    print(ln, end='')
                 else:
-                    print('[{}] {}'.format(label, l), end='')
+                    print('[{}] {}'.format(label, ln), end='')
             p.wait()
         else:
-            p = subprocess.run(cmd, shell=True, encoding='utf-8', errors='ignore', bufsize=0)
+            p = subprocess.run(cmd, shell=True,
+                               encoding='utf-8',
+                               errors='ignore',
+                               bufsize=0)
         return p.returncode
 
     os.environ['RX_HOST'] = host
     LOG.set_label(host)
     LOG.info(click.style('START', reverse=True))
 
     if ctx.parallel:
         llabel = host
     else:
         llabel = None
 
     if ctx.inline_check:
         LOG.info('Check host connectivity')
-        valid_host,msg = check(host, ctx)
+        valid_host, msg = check(host, ctx)
         if not valid_host:
             rc = -1
             if ctx.parallel or ctx.warning_only:
                 LOG.warning(msg)
             else:
                 LOG.error(msg)
-                #sys.exit(1)
+                # sys.exit(1)
     else:
         valid_host = True
 
     if valid_host:
         if ctx.ad_hoc:
             LOG.info('Ad-hoc task')
             rc = run("__run '{}'".format(task_list), llabel)
         else:
             for t in task_list:
                 rc = run('{} {}'.format(t['name'], t['args']), llabel)
                 if rc != 0:
                     break
-    
+
     if rc != 0:
-        if ctx.parallel: #or ctx.warning_only:
-            LOG.warning(click.style('Task terminated with error', reverse=True))
+        if ctx.parallel:  # or ctx.warning_only:
+            LOG.warning(click.style(
+                'Task terminated with error', reverse=True))
         else:
-            LOG.error(click.style('Task terminated with error, aborting', reverse=True))
+            LOG.error(click.style(
+                'Task terminated with error, aborting', reverse=True))
             sys.exit(1)
     else:
         LOG.info(click.style('OK', reverse=True))
 
+
 def check(host, ctx):
-    cmd_template = 'set -x ; LOG=$(mktemp -p /tmp rx-XXXXXXXX) ; exec 3>&1 4>&2 1>$LOG 2>&1 ; {} ; RC=$? ; exec 1>&3 2>&4 ; cat $LOG ; rm -fv $LOG ; exit $RC'
+    cmd_template = 'set -x ; LOG=$(mktemp -p /tmp rx-XXXXXXXX) ; \
+        exec 3>&1 4>&2 1>$LOG 2>&1 ; {} ; RC=$? ; exec 1>&3 2>&4 ; \
+        cat $LOG ; rm -fv $LOG ; exit $RC'
     valid_host = True
     cmd = '{} -v {} true'.format(ctx.ssh_cmd, host)
     cmd = cmd_template.format(cmd)
     LOG.debug('SSH:\n{}'.format(cmd))
-    p = subprocess.run(cmd, shell=True, encoding='utf-8', errors='ignore', bufsize=0, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL) #stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    p = subprocess.run(cmd, shell=True, encoding='utf-8',
+                       errors='ignore', bufsize=0,
+                       stdout=subprocess.PIPE,
+                       stderr=subprocess.DEVNULL)
     if p.returncode != 0:
         valid_host = False
         msg = "Can't do ssh"
     if valid_host and ctx.use_sudo_password:
-        cmd = 'cat>{} && chmod 700 {}'.format(ctx.passwd_script, ctx.passwd_script)
-        cmd = '{} -v {} /bin/sh -c {}'.format(ctx.ssh_cmd, host, shlex.quote(cmd))
+        cmd = 'cat>{} && chmod 700 {}'.format(
+            ctx.passwd_script, ctx.passwd_script)
+        cmd = '{} -v {} /bin/sh -c {}'.format(
+            ctx.ssh_cmd, host, shlex.quote(cmd))
         cmd = cmd_template.format(cmd)
-        LOG.debug('Install password script:\n{} | {}'.format(ctx.passwd_code, cmd))
-        p = subprocess.run(cmd, shell=True, encoding='utf-8', errors='ignore', bufsize=0, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, input=ctx.passwd_code)
+        LOG.debug('Install password script:\n{} | {}'.format(
+            ctx.passwd_code, cmd))
+        p = subprocess.run(cmd, shell=True, encoding='utf-8',
+                           errors='ignore', bufsize=0,
+                           stdout=subprocess.PIPE,
+                           stderr=subprocess.DEVNULL,
+                           input=ctx.passwd_code)
         if p.returncode != 0:
             valid_host = False
             msg = "Can't copy password script"
     if valid_host:
-        cmd = '{} -v {} {} true'.format(ctx.ssh_cmd, host , ctx.sudo_cmd)
+        cmd = '{} -v {} {} true'.format(ctx.ssh_cmd, host, ctx.sudo_cmd)
         cmd = cmd_template.format(cmd)
         LOG.debug('Sudo:\n{}'.format(cmd))
-        p = subprocess.run(cmd, shell=True, encoding='utf-8', errors='ignore', bufsize=0, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL)
+        p = subprocess.run(cmd, shell=True, encoding='utf-8', errors='ignore',
+                           bufsize=0, stdout=subprocess.PIPE,
+                           stderr=subprocess.DEVNULL)
         if p.returncode != 0:
             valid_host = False
             msg = "Can't do sudo"
     if not valid_host:
-        msg = '{}: rc={}:\n{}'.format(msg, p.returncode,p.stdout)
+        msg = '{}: rc={}:\n{}'.format(msg, p.returncode, p.stdout)
     else:
         msg = None
     return valid_host, msg
-
```

### Comparing `rxctl-0.1.7/rxctl/lib/utils.py` & `rxctl-0.1.8/rxctl/lib/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,47 @@
 import glob
 import os
 
 import click
 
 
 def get_environment(env, cmd, selector=None):
-    LOG.debug("get_environment: env='{}', cmd='{}', selector='{}'".format(env, cmd, selector))
+    LOG.debug("get_environment: env='{}', cmd='{}', selector='{}'".format(
+        env, cmd, selector))
     if not os.path.isfile(env):
         LOG.warning("'{}' missing".format(env))
         return
     if not os.access(env, os.X_OK):
         LOG.warning("'{}' not executable".format(env))
         return
     if cmd == 'inventory' and selector:
         cmd = "{} '{}'".format(cmd, selector)
     LOG.info('Get {} from {}'.format(cmd, env))
-    p = subprocess.run('{} {}'.format(env, cmd), capture_output=True, shell=True, encoding='utf-8', errors='ignore')
+    p = subprocess.run('{} {}'.format(env, cmd), capture_output=True,
+                       shell=True, encoding='utf-8', errors='ignore')
     LOG.debug("get_environment: out:\n{}".format(p.stdout))
     if cmd == 'inventory':
         data1 = p.stdout.strip()
     else:
         try:
             data1 = json.loads(p.stdout)
-        except:
+        except Exception:
             LOG.error("{} {} didn't return a valid json".format(env, cmd))
             sys.exit(1)
     if cmd == 'config':
         data2 = {}
-        for k,v in data1.items():
-            data2[k.replace('-','_')] = v
+        for k, v in data1.items():
+            data2[k.replace('-', '_')] = v
         return data2
     return data1
 
 
 def check_task(t):
-    c = subprocess.run('{} __name__'.format(t), shell=True, encoding='utf-8', errors='ignore', bufsize=0, capture_output=True)
+    c = subprocess.run('{} __name__'.format(t), shell=True, encoding='utf-8',
+                       errors='ignore', bufsize=0, capture_output=True)
     if c.stdout.strip() == t:
         return True
     return False
 
 
 def get_tasks():
     tasks = []
@@ -56,18 +59,18 @@
             else:
                 LOG.debug('Invalid task: {}'.format(f))
     tasks.sort()
     return tasks
 
 
 def task_doc(task, short=False):
-    p = subprocess.run(task, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='utf-8', errors='ignore')
+    p = subprocess.run(task, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
+                       encoding='utf-8', errors='ignore')
     if short:
         if p.returncode == 0:
             h = p.stdout.split('\n')
             h = h[0]
         else:
             h = click.style("ERROR, can't get help", fg='red')
     else:
         h = p.stdout
     return h
-
```

### Comparing `rxctl-0.1.7/PKG-INFO` & `rxctl-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxctl
-Version: 0.1.7
+Version: 0.1.8
 Summary: Linux remote execution tool
 Home-page: https://github.com/mihaiush/rxctl
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

