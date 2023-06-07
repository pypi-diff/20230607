# Comparing `tmp/prelude-cli-1.2.2.tar.gz` & `tmp/prelude-cli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.2.2.tar", last modified: Fri Jun  2 17:13:20 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.3.tar", last modified: Wed Jun  7 21:04:54 2023, max compression
```

## Comparing `prelude-cli-1.2.2.tar` & `prelude-cli-1.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.814235 prelude-cli-1.2.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-02 17:13:20.814289 prelude-cli-1.2.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.811526 prelude-cli-1.2.2/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.2/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.2/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.812461 prelude-cli-1.2.2/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.2/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.814038 prelude-cli-1.2.2/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3405 2023-06-02 13:58:42.000000 prelude-cli-1.2.2/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.2/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7430 2023-05-30 20:30:23.000000 prelude-cli-1.2.2/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3478 2023-05-18 20:31:39.000000 prelude-cli-1.2.2/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.2/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.2/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.812274 prelude-cli-1.2.2/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-02 17:13:20.814501 prelude-cli-1.2.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.064973 prelude-cli-1.2.3/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-07 21:04:54.065024 prelude-cli-1.2.3/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.3/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.061793 prelude-cli-1.2.3/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.3/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.3/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.062585 prelude-cli-1.2.3/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.3/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.064779 prelude-cli-1.2.3/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     4036 2023-06-06 22:22:58.000000 prelude-cli-1.2.3/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.3/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7960 2023-06-07 20:52:19.000000 prelude-cli-1.2.3/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3879 2023-06-07 20:52:19.000000 prelude-cli-1.2.3/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.3/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.3/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.062405 prelude-cli-1.2.3/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-07 21:04:54.065247 prelude-cli-1.2.3/setup.cfg
```

### Comparing `prelude-cli-1.2.2/LICENSE` & `prelude-cli-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.2/PKG-INFO` & `prelude-cli-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.2
+Version: 1.2.3
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.2/prelude_cli/cli.py` & `prelude-cli-1.2.3/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.2/prelude_cli/views/build.py` & `prelude-cli-1.2.3/prelude_cli/views/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import uuid
 import click
 import prelude_cli.templates as templates
 import importlib.resources as pkg_resources
 
+from rich import print_json
 from datetime import datetime
 from pathlib import Path, PurePath
 
 from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.build_controller import BuildController
 
 
@@ -19,47 +20,67 @@
 def build(ctx):
     """ Custom security tests """
     ctx.obj = BuildController(account=ctx.obj)
 
 
 @build.command('create-test')
 @click.argument('name')
-@click.option('-t', '--test', help='test identifier', default=None, type=str)
-@click.option('-u', '--unit', required=True, help='unit identifier', default=None, type=str)
+@click.option('-u', '--unit', required=True, help='unit identifier', type=str)
 @click.option('-a', '--advisory', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, type=str)
+@click.option('-t', '--test', help='test identifier', default=None, type=str)
 @click.pass_obj
 @handle_api_error
-def create_test(controller, name, test, unit, advisory):
+def create_test(controller, name, unit, advisory, test):
     """ Create or update a security test """
-    test_id = test or str(uuid.uuid4())
     with Spinner():
-        controller.create_test(
-            test_id=test_id,
+        t = controller.create_test(
             name=name,
             unit=unit,
-            advisory=advisory
+            advisory=advisory,
+            test_id=test
         )
 
     if not test:
-        basename = f'{test_id}.go'
+        basename = f'{t["id"]}.go'
         template = pkg_resources.read_text(templates, 'template.go')
-        template = template.replace('$ID', test_id)
+        template = template.replace('$ID', t['id'])
         template = template.replace('$NAME', name)
         template = template.replace('$UNIT', unit or '')
         template = template.replace('$CREATED', str(datetime.utcnow()))
         
         with Spinner():
-            controller.upload(test_id=test_id, filename=basename, data=template)
+            controller.upload(test_id=t['id'], filename=basename, data=template)
+            t['attachments'] = [basename]
 
-        test_dir = PurePath(test_id, basename)
-        Path(test_id).mkdir(parents=True, exist_ok=True)
+        test_dir = PurePath(t['id'], basename)
+        Path(t['id']).mkdir(parents=True, exist_ok=True)
         
         with open(test_dir, 'w', encoding='utf8') as test_code:
             test_code.write(template)
-            click.secho(f'Created {basename}', fg='green')
+
+    print_json(data=t)
+
+
+@build.command('update-test')
+@click.argument('test')
+@click.option('-n', '--name', help='test name', default=None, type=str)
+@click.option('-u', '--unit', help='unit identifier', default=None, type=str)
+@click.option('-a', '--advisory', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, type=str)
+@click.pass_obj
+@handle_api_error
+def update_test(controller, test, name, unit, advisory):
+    """ Create or update a security test """
+    with Spinner():
+        test = controller.update_test(
+            test_id=test,
+            name=name,
+            unit=unit,
+            advisory=advisory
+        )
+    print_json(data=test)
 
 
 @build.command('delete-test')
 @click.argument('test')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
```

### Comparing `prelude-cli-1.2.2/prelude_cli/views/configure.py` & `prelude-cli-1.2.3/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.2/prelude_cli/views/detect.py` & `prelude-cli-1.2.3/prelude_cli/views/detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,46 @@
     ctx.obj = DetectController(account=ctx.obj)
 
 
 @detect.command('create-endpoint')
 @click.option('-h', '--host', help='hostname of this machine', type=str, required=True)
 @click.option('-s', '--serial_num', help='serial number of this machine', type=str, required=True)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default='')
-@click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default='')
-@click.option('-i', '--endpoint_id', help='update a specific endpoint_id with the provided values', type=str, default='')
+@click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
 @click.pass_obj
 @handle_api_error
-def register_endpoint(controller, host, serial_num, edr_id, tags, endpoint_id):
+def register_endpoint(controller, host, serial_num, edr_id, tags):
     """ Register a new endpoint """
     with Spinner():
         token = controller.register_endpoint(
             host=host, 
             serial_num=serial_num, 
             edr_id=edr_id, 
-            tags=tags, 
-            endpoint_id=endpoint_id
+            tags=tags
         )
-        click.secho(token)
+    click.secho(token)
+
+
+@detect.command('update-endpoint')
+@click.argument('endpoint_id')
+@click.option('-h', '--host', help='hostname of this machine', type=str, default=None)
+@click.option('-e', '--edr_id', help='EDR id', type=str, default=None)
+@click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
+@click.pass_obj
+@handle_api_error
+def update_endpoint(controller, endpoint_id, host, edr_id, tags):
+    """ Register a new endpoint """
+    with Spinner():
+        ep = controller.update_endpoint(
+            endpoint_id=endpoint_id,
+            host=host,
+            edr_id=edr_id,
+            tags=tags
+        )
+    print_json(data=ep)
 
 
 @detect.command('tests')
 @click.pass_obj
 @handle_api_error
 def list_tests(controller):
     """ List all security tests """
@@ -52,15 +69,16 @@
 @detect.command('test')
 @click.argument('test_id')
 @click.pass_obj
 @handle_api_error
 def get_test(controller, test_id):
     """ List properties for a test """
     with Spinner():
-        print_json(data=controller.get_test(test_id=test_id))
+        data = controller.get_test(test_id=test_id)
+    print_json(data=data)
 
 
 @detect.command('download')
 @click.argument('test')
 @click.pass_obj
 @handle_api_error
 def download(controller, test):
@@ -131,15 +149,15 @@
 @click.pass_obj
 @handle_api_error
 def queue(controller):
     """ List all tests in your active queue """
     with Spinner():
         iam = IAMController(account=controller.account)
         queue = iam.get_account().get('queue')
-        print_json(data=queue)
+    print_json(data=queue)
 
 
 @detect.command('endpoints')
 @click.option('-d', '--days', help='only show endpoints that have run at least once in the past DAYS days', default=90, type=int)
 @click.pass_obj
 @handle_api_error
 def endpoints(controller, days):
@@ -152,15 +170,16 @@
 @detect.command('advisories')
 @click.pass_obj
 @click.option('-y', '--year', help='View advisories from a specific year', default=None, type=int)
 @handle_api_error
 def advisories(controller, year):
     """ List all Prelude advisories """
     with Spinner():
-        print_json(data=controller.list_advisories(year=year))
+        data = controller.list_advisories(year=year)
+    print_json(data=data)
 
 
 @detect.command('clone')
 @click.pass_obj
 @handle_api_error
 def clone(controller):
     """ Download all tests to your local environment """
```

### Comparing `prelude-cli-1.2.2/prelude_cli/views/iam.py` & `prelude-cli-1.2.3/prelude_cli/views/iam.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,31 +19,40 @@
 @click.pass_obj
 @handle_api_error
 @click.confirmation_option(prompt='Overwrite local account credentials for selected profile?')
 def register_account(controller):
     """ Register a new account """
     email = click.prompt('Enter your email')
     name = click.prompt('(Optional) Enter your name', default='', show_default=False)
+    company = click.prompt('(Optional) Enter your associated company', default='', show_default=False)
     with Spinner():
-        data = controller.new_account(user_email=email, user_name=name)
+        data = controller.new_account(user_email=email, user_name=name, company=company)
     print_json(data=data)
     print("\nCheck your email to verify your account.\n")
 
 
 @iam.command('update-account')
 @click.option('-m', '--mode',
               help='provide a mode',
-              default=Mode.MANUAL.name, show_default=True,
+              default=None, show_default=False,
               type=click.Choice([m.name for m in Mode], case_sensitive=False))
+@click.option('-c', '--company',
+              help='provide your associated company',
+              default=None, show_default=False,
+              type=str)
 @click.pass_obj
 @handle_api_error
-def update_account(controller, mode):
+def update_account(controller, mode, company):
     """ Update an account """
     with Spinner():
-        controller.update_account(mode=Mode[mode.upper()].value)
+        data = controller.update_account(
+            mode=Mode[mode.upper()].value if mode else None,
+            company=company
+        )
+    print_json(data=data)
 
 
 @iam.command('account')
 @click.pass_obj
 @handle_api_error
 def describe_account(controller):
     """ Get account details """
@@ -51,15 +60,15 @@
         print_json(data=controller.get_account())
 
 
 @iam.command('create-user')
 @click.option('-d', '--days', help='days this user will remain active', default=365, type=int)
 @click.option('-p', '--permission', help='user permission level', default=Permission.SERVICE.name,
               type=click.Choice([p.name for p in Permission if p != Permission.INVALID], case_sensitive=False), show_default=True)
-@click.option('-n', '--name', help='name of user', default='', type=str)
+@click.option('-n', '--name', help='name of user', default=None, show_default=False, type=str)
 @click.argument('email')
 @click.pass_obj
 @handle_api_error
 def create_user(controller, days, permission, name, email):
     """ Create a new user in your account """
     expires = datetime.utcnow() + timedelta(days=days)
     with Spinner():
```

### Comparing `prelude-cli-1.2.2/prelude_cli/views/partner.py` & `prelude-cli-1.2.3/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.2/prelude_cli/views/shared.py` & `prelude-cli-1.2.3/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.2/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.3/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.2
+Version: 1.2.3
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.2/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.3/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.2/setup.cfg` & `prelude-cli-1.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.2.2
+version = 1.2.3
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.2.2
+	prelude-sdk == 1.2.3
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

