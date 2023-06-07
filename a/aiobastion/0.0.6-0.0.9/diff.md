# Comparing `tmp/aiobastion-0.0.6.tar.gz` & `tmp/aiobastion-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobastion-0.0.6.tar", last modified: Fri Aug 26 09:30:04 2022, max compression
+gzip compressed data, was "aiobastion-0.0.9.tar", last modified: Thu Jan 12 15:42:08 2023, max compression
```

## Comparing `aiobastion-0.0.6.tar` & `aiobastion-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 09:30:04.034674 aiobastion-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-26 09:29:51.000000 aiobastion-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-08-26 09:30:04.034674 aiobastion-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-08-26 09:29:51.000000 aiobastion-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 09:30:04.034674 aiobastion-0.0.6/aiobastion/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/accountgroup.py
--rw-r--r--   0 runner    (1001) docker     (121)    28083 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/applications.py
--rw-r--r--   0 runner    (1001) docker     (121)     9305 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13874 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/cyberark.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7448 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/platforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     9272 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/safe.py
--rw-r--r--   0 runner    (1001) docker     (121)     8123 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/users.py
--rw-r--r--   0 runner    (1001) docker     (121)    12791 2022-08-26 09:29:51.000000 aiobastion-0.0.6/aiobastion/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 09:30:04.034674 aiobastion-0.0.6/aiobastion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-08-26 09:30:04.000000 aiobastion-0.0.6/aiobastion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-08-26 09:30:04.000000 aiobastion-0.0.6/aiobastion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 09:30:04.000000 aiobastion-0.0.6/aiobastion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-26 09:30:04.000000 aiobastion-0.0.6/aiobastion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-26 09:29:51.000000 aiobastion-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-08-26 09:30:04.034674 aiobastion-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:42:08.024423 aiobastion-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-12 15:41:55.000000 aiobastion-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-01-12 15:42:08.024423 aiobastion-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-01-12 15:41:55.000000 aiobastion-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:42:08.024423 aiobastion-0.0.9/aiobastion/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/accountgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29628 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/cyberark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-01-12 15:41:55.000000 aiobastion-0.0.9/aiobastion/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:42:08.024423 aiobastion-0.0.9/aiobastion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-01-12 15:42:08.000000 aiobastion-0.0.9/aiobastion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-12 15:42:08.000000 aiobastion-0.0.9/aiobastion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:42:08.000000 aiobastion-0.0.9/aiobastion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-12 15:42:08.000000 aiobastion-0.0.9/aiobastion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-12 15:41:55.000000 aiobastion-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-12 15:42:08.024423 aiobastion-0.0.9/setup.cfg
```

### Comparing `aiobastion-0.0.6/LICENSE` & `aiobastion-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/PKG-INFO` & `aiobastion-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aiobastion
-Version: 0.0.6
+Version: 0.0.9
 Summary: Manage your Cyberark implementation
 Home-page: https://github.com/labanquepostale/aiobastion
 Author: Gautier Leveille
 Author-email: gautier.leveille@labanquepostale.fr
 Project-URL: Bug Tracker, https://github.com/labanquepostale/aiobastion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiobastion-0.0.6/README.md` & `aiobastion-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/abstract.py` & `aiobastion-0.0.9/aiobastion/abstract.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/accountgroup.py` & `aiobastion-0.0.9/aiobastion/accountgroup.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/accounts.py` & `aiobastion-0.0.9/aiobastion/accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 import asyncio
 import re
 from typing import List, Union, AsyncIterator
 import aiohttp
 
 from .abstract import Vault
-from .config import validate_ip
+from .config import validate_ip, flatten
 from .exceptions import (
     CyberarkAPIException, CyberarkException, AiobastionException
 )
 
 MAX_CONCURRENT_CALLS = 10
+
+
 # SEMAPHORE = None
 #
 # def get_sem():
 #     global SEMAPHORE
 #     if SEMAPHORE is None:
 #         SEMAPHORE = asyncio.Semaphore(MAX_CONCURRENT_CALLS)
 #     return SEMAPHORE
@@ -69,16 +71,31 @@
         return json_object
 
     def __str__(self):
         strrepr = self.to_json()
         return str(strrepr)
 
     def cpm_status(self):
-        return "automaticManagementEnabled" in self.secretManagement and \
-               self.secretManagement["automaticManagementEnabled"]
+        if "status" in self.secretManagement:
+            # 'success' for 'failure'
+            return self.secretManagement["status"]
+        elif "automaticManagementEnabled" in self.secretManagement and \
+                not self.secretManagement["automaticManagementEnabled"]:
+            return "Deactivated"
+        else:
+            return "No status (yet)"
+
+    def last_modified(self, days=True):
+        import time
+        if "lastModifiedTime" in self.secretManagement:
+            ts = self.secretManagement["lastModifiedTime"]
+            if days:
+                return int((int(time.time()) - ts) / 86400)
+            else:
+                return ts
 
 
 def _filter_account(account: dict, filters: dict):
     """
     This function helps to ensure that search accounts match with requested accounts
     :param account: one json cyberark repr of a privileged address
     :param filters: one dict like username: admin
@@ -106,50 +123,47 @@
 class Account:
     def __init__(self, epv: Vault):
         self.epv = epv
 
     async def handle_acc_list(self, api_call, account, *args, **kwargs):
         if isinstance(account, list):
             tasks = []
-            semaphore = asyncio.Semaphore(MAX_CONCURRENT_CALLS)
             for a in account:
                 if not isinstance(a, PrivilegedAccount) and not re.match('[0-9]*_[0-9*]', a):
                     raise AiobastionException("You must call the function with PrivilegedAccount or list of Privileged "
-                                           "Accounts")
+                                              "Accounts")
 
                 tasks.append(api_call(a, *args, **kwargs))
 
-            async def sem_task(task):
-                async with semaphore:
-                    return await task
-
-            return await asyncio.gather(*(sem_task(task) for task in tasks), return_exceptions=True)
+            return await asyncio.gather(*tasks, return_exceptions=True)
         elif isinstance(account, PrivilegedAccount) or re.match('[0-9]*_[0-9*]', account):
             return await api_call(account, *args, **kwargs)
         else:
             raise AiobastionException("You must call the function with PrivilegedAccount or list of Privileged Accounts"
-                                   "(or valid account_id for some functions)")
+                                      "(or valid account_id for some functions)")
 
     async def handle_acc_id_list(self, method, url, accounts, data=None):
         """
         Utility function for handling a list of accounts id in parameter of url
         :param method: http valid method
         :param url: lambda function that return the url with an account_id parameter
         :param accounts: list of address id
         :param data: if relevant, a dict that contains data
         :return: the result of the subsequent calls
         """
+
         async def api_call(acc_id):
             return await self.epv.handle_request(method, url(acc_id), data=data)
 
         return await self.handle_acc_list(api_call, accounts)
 
     async def add_account_to_safe(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]) -> str:
         async def api_call(acc):
-            return await self.epv.handle_request("post", 'API/Accounts', data=acc.to_json(), filter_func=lambda r: r["id"])
+            return await self.epv.handle_request("post", 'API/Accounts', data=acc.to_json(),
+                                                 filter_func=lambda r: r["id"])
 
         return await self.handle_acc_list(api_call, account)
 
     async def get_account(self, account_id) -> Union[PrivilegedAccount, List[PrivilegedAccount]]:
         acc = await self.handle_acc_id_list(
             "get",
             lambda a: f"API/Accounts/{a}",
@@ -162,47 +176,44 @@
             return [PrivilegedAccount(**a) for a in acc]
 
     async def get_privileged_account_id(self, account: PrivilegedAccount):
         if account.id == "":
             acc = await self.search_account_by(username=account.userName, safe=account.safeName,
                                                keywords=account.address)
             if len(acc) != 1:
-                raise CyberarkException(
-                    "More than one address (or no address) found here (same username in same safe with same address")
+                return [a.id for a in acc]
             else:
                 return acc[0].id
         else:
             return account.id
 
-    async def get_single_account_id(self, account, sema=None):
-        if sema is None:
-            sema = asyncio.Semaphore(10)
-        async with sema:
-            if type(account) is str:
-                if re.match(r'\d+_\d+', account) is not None:
-                    return account
-                else:
-                    raise AiobastionException("The account_id provided is not correct")
-            if isinstance(account, PrivilegedAccount):
-                return await self.get_privileged_account_id(account)
+    async def get_single_account_id(self, account):
+        if type(account) is str:
+            if re.match(r'\d+_\d+', account) is not None:
+                return account
             else:
-                raise AiobastionException("You must provide a valid PrivilegedAccount to function get_account_id")
+                raise AiobastionException("The account_id provided is not correct")
+        if isinstance(account, PrivilegedAccount):
+            return await self.get_privileged_account_id(account)
+        else:
+            raise AiobastionException("You must provide a valid PrivilegedAccount to function get_account_id")
 
     async def get_account_id(self, account: Union[PrivilegedAccount, str, List[PrivilegedAccount], List[str]]):
         if isinstance(account, list):
-            sema = asyncio.Semaphore(10)
-            tasks = [self.get_single_account_id(a, sema) for a in account]
-            return await asyncio.gather(*tasks, return_exceptions=False)
+            tasks = [self.get_single_account_id(a) for a in account]
+            return flatten(await asyncio.gather(*tasks, return_exceptions=False))
         else:
             return await self.get_single_account_id(account)
 
-    async def link_reconciliation_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]], reconcile_account: PrivilegedAccount):
+    async def link_reconciliation_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]],
+                                          reconcile_account: PrivilegedAccount):
         return await self.link_account(account, reconcile_account, 3)
 
-    async def link_logon_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]], logon_account: PrivilegedAccount):
+    async def link_logon_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]],
+                                 logon_account: PrivilegedAccount):
         return await self.link_account(account, logon_account, 2)
 
     async def link_reconcile_account_by_address(self, acc_username, rec_acc_username, address):
         acc, rec_acc = await asyncio.gather(
             self.search_account_by(username=acc_username, address=address),
             self.search_account_by(username=rec_acc_username, address=address))
 
@@ -223,15 +234,16 @@
 
     async def remove_reconcile_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
         return await self.unlink_account(account, 3)
 
     async def remove_logon_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
         return await self.unlink_account(account, 2)
 
-    async def unlink_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]], extra_password_index: int):
+    async def unlink_account(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]],
+                             extra_password_index: int):
         if extra_password_index not in [1, 2, 3]:
             raise AiobastionException("ExtraPasswordIndex must be between 1 and 3")
 
         return await self.handle_acc_id_list(
             "delete",
             lambda a: f"API/Accounts/{a}/LinkAccount/{extra_password_index}",
             await self.get_account_id(account)
@@ -267,15 +279,15 @@
         # async def api_call(acc_id):
         #     return await self.epv.handle_request("post", f"API/Accounts/{acc_id}/LinkAccount", data=data)
         #
         # return await self.handle_acc_list(api_call, account_id)
 
         return await self.handle_acc_id_list(
             "post",
-            lambda a:  f"API/Accounts/{a}/LinkAccount",
+            lambda a: f"API/Accounts/{a}/LinkAccount",
             account_id,
             data
         )
 
     async def change_password(self, account: Union[PrivilegedAccount, str], change_group=False):
         data = {
             "ChangeEntireGroup": change_group
@@ -348,15 +360,14 @@
         :param kwargs: any searchable key = value
         :return: a list of PrivilegedAccounts
         """
 
         return [account async for account in
                 self.search_account_iterator(keywords, username, address, safe, platform, **kwargs)]
 
-
     async def search_account_iterator(self, keywords=None, username=None, address=None, safe=None,
                                       platform=None, **kwargs) -> AsyncIterator[PrivilegedAccount]:
         """
         This function allow to search using one or more parameters and return list of address id
         :param keywords: free search
         :param username: username search (field "userName")
         :param address: IP address search (field "address")
@@ -422,15 +433,16 @@
             async with session.post(url, json=body, **self.epv.request_params) as req:
                 if req.status != 200:
                     content = await req.json()
                     raise CyberarkAPIException(req.status, content["ErrorCode"], content["ErrorMessage"])
 
                 return await req.read()
 
-    async def disable_password_management(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]], reason: str = ""):
+    async def disable_password_management(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]],
+                                          reason: str = ""):
         data = [
             {"op": "replace", "path": "/secretManagement/automaticManagementEnabled", "value": False},
             {"op": "add", "path": "/secretManagement/manualManagementReason", "value": reason}
         ]
 
         return await self.handle_acc_id_list(
             "patch",
@@ -488,40 +500,40 @@
             lambda account_id: f"API/Accounts/{account_id}/Password/Retrieve",
             await self.get_account_id(account)
         )
 
         # account_id = await self.get_account_id(address)
         # return await self.epv.handle_request("post", f"API/Accounts/{account_id}/Password/Retrieve")
 
-# a tester + documenter
+    # a tester + documenter
     async def get_ssh_key(self, account: Union[PrivilegedAccount, str, List[PrivilegedAccount], List[str]]):
         """
         Retrieve the SSH Key of an address
         :param account: Privileged Account or address id
-        :return: Account password value
+        :return: SSH key value
         """
 
         return await self.handle_acc_id_list(
             "post",
             lambda account_id: f"API/Accounts/{account_id}/Secret/Retrieve",
             await self.get_account_id(account)
         )
 
-# a tester
+    # a tester
     async def get_secret(self, account: Union[PrivilegedAccount, str, List[PrivilegedAccount], List[str]]):
         if isinstance(account, list):
             tasks = []
             for a in account:
                 if a.secretType == "key":
                     tasks.append(self.get_ssh_key(a))
                 else:
                     tasks.append(self.get_password(a))
             return await asyncio.gather(*tasks)
         else:
-            if a.secretType == "key":
+            if account.secretType == "key":
                 return await self.get_ssh_key(account)
             else:
                 return await self.get_password(account)
 
     async def set_password(self, account, password):
         """
         Set the password for the given address in the vault
@@ -556,15 +568,50 @@
 
     async def get_cpm_status(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
         if isinstance(account, list):
             return [a.secretManagement for a in account]
         else:
             return account.secretManagement
 
-    async def add_member_to_group(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]], group_name: str = "") -> str:
+    async def activity(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
+        """
+        Get account(s) activity
+        """
+        activities = await self.handle_acc_id_list(
+            "get",
+            lambda account_id: f"WebServices/PIMServices.svc/Accounts/{account_id}/Activities/",
+            await self.get_account_id(account)
+        )
+
+        if isinstance(activities, list):
+            return [a["GetAccountActivitiesSlashResult"] for a in activities]
+        else:
+            return activities["GetAccountActivitiesSlashResult"]
+
+    async def last_cpm_error_message(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
+        """
+        Get account(s) activity
+        """
+        activities = await self.activity(account)
+
+        def single_cpm_error(activity):
+            for a in activity:
+                if "CPM" in a["Activity"]:
+                    if "Failure" in a["Reason"]:
+                        reason = a["Reason"].split("Error:")
+                        return reason[1]
+
+        # List of list
+        if any(isinstance(el, list) for el in activities):
+            return [single_cpm_error(_activity) for _activity in activities]
+        else:
+            return single_cpm_error(activities)
+
+    async def add_member_to_group(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]],
+                                  group_name: str = "") -> str:
         """
         Add an address to a group
         :param account: a PrivilegedAccount object
         :param group_name: name of the group (or try the address username if empty)
         :return: AccountID
         """
         groups = await self.epv.accountgroup.list_by_safe(account.safeName)
@@ -593,14 +640,15 @@
     async def get_account_group(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
         """
         Returns the GroupID of a given PrivilegedAccount
         :param account: Privileged Account
         :type account: PrivilegedAccount, list
         :return: accountID
         """
+
         async def api_call(acc):
             for group in await self.epv.accountgroup.list_by_safe(acc.safeName):
                 groupid = group.id
                 for member in await self.epv.accountgroup.members(groupid):
                     if member.id == acc.id:
                         return groupid
             return None
@@ -609,14 +657,15 @@
 
     async def del_account_group_membership(self, account: Union[PrivilegedAccount, List[PrivilegedAccount]]):
         """
         Find AccountGroup for an account_group and delete it
         returns False if no group was remove, True is a group was deleted
         raise an Exception if a group was found but deletion didn't worked
         """
+
         async def _del_accountgroup(acc):
             groupid = await self.get_account_group(acc)
             if groupid is None:
                 return False
             else:
                 try:
                     await self.epv.accountgroup.delete_member(acc, groupid)
@@ -645,8 +694,7 @@
             try:
                 await self.delete(old_id)
             except CyberarkAPIException as err:
                 raise CyberarkException(f"Unable to delete {acc.name} old address : {str(err)}")
             return new_account_id
 
         return await self.handle_acc_list(_move, account)
-
```

### Comparing `aiobastion-0.0.6/aiobastion/applications.py` & `aiobastion-0.0.9/aiobastion/applications.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/config.py` & `aiobastion-0.0.9/aiobastion/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 if "AppId" in document["Connection"].keys():
                     self.appid = document["Connection"]["AppId"]
                 else:
                     self.appid = None
                 if "Authtype" in document["Connection"].keys():
                     self.authtype = document["Connection"]["Authtype"]
                 else:
-                    self.authtype = "Cyberark"
+                    self.authtype = None
 
             if "PVWA" in document:
                 if "Host" in document["PVWA"].keys():
                     self.PVWA = document["PVWA"]["Host"]
                 if "CA" in document["PVWA"].keys():
                     self.PVWA_CA = document["PVWA"]["CA"]
                 else:
@@ -237,14 +237,20 @@
         if not x.isdigit():
             return False
         i = int(x)
         if i < 0 or i > 255:
             return False
     return True
 
+def flatten(A):
+    rt = []
+    for i in A:
+        if isinstance(i,list): rt.extend(flatten(i))
+        else: rt.append(i)
+    return rt
 
 def permissions(profile: str) -> dict:
     if "admin" in profile.lower():
         return ADMIN_PERMISSIONS
     if "use" in profile.lower():
         return USE_PERMISSIONS
     if "show" in profile.lower():
```

### Comparing `aiobastion-0.0.6/aiobastion/cyberark.py` & `aiobastion-0.0.9/aiobastion/cyberark.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,30 +31,53 @@
             if self.config.PVWA_CA is not False:
                 self.request_params = {"timeout": self.config.timeout,
                                        "ssl": ssl.create_default_context(cafile=self.config.PVWA_CA)}
             else:
                 self.request_params = {"timeout": self.config.timeout, "ssl": False}
 
             self.api_host = self.config.PVWA
+            self.authtype = self.config.authtype
             self.cpm = self.config.CPM
             self.retention = self.config.retention
             self.max_concurrent_tasks = self.config.max_concurrent_tasks
             self.__token = token
 
         if serialized is not None:
-            if serialized["verify"] is not False:
-                self.request_params = {"timeout": serialized["timeout"],
-                                       "ssl": ssl.create_default_context(cafile=serialized["verify"])}
+            if "Verify" in serialized:
+                if serialized["verify"] is not False:
+                    self.request_params = {"timeout": serialized["timeout"],
+                                           "ssl": ssl.create_default_context(cafile=serialized["verify"])}
+                else:
+                    self.request_params = {"timeout": serialized["timeout"], "ssl": False}
             else:
-                self.request_params = {"timeout": serialized["timeout"], "ssl": False}
+                self.request_params = {"timeout": 10, "ssl": False}
+
             self.api_host = serialized['api_host']
-            self.cpm = serialized['cpm']
-            self.retention = serialized['retention']
-            self.max_concurrent_tasks = serialized['max_concurrent_tasks']
-            self.__token = serialized['token']
+
+            if "authtype" in serialized:
+                self.authtype = serialized["authtype"]
+            else:
+                self.authtype = None
+
+            if "cpm" in serialized:
+                self.cpm = serialized['cpm']
+            else:
+                self.cpm = ""
+            if "retention" in serialized:
+                self.retention = serialized['retention']
+            else:
+                self.retention = 10
+            if "max_concurrent_tasks" in serialized:
+                self.max_concurrent_tasks = serialized['max_concurrent_tasks']
+            else:
+                self.max_concurrent_tasks = 10
+            if "token" in serialized:
+                self.__token = serialized['token']
+            else:
+                self.__token = None
 
         # self.session = requests.Session()
 
         self.user_list = None
 
         # Session management
         self.session = None
@@ -97,16 +120,19 @@
                             raise CyberarkException(await req.text())
                         except Exception as err:
                             await self.close_session()
                             # Old session reused ?
                             raise CyberarkException(f"Unknown error, HTTP {str(req.status)}, ERR : {str(err)}")
 
                 tok = await req.text()
+                # Closing session because now we are connected and we need to update headers which can be done
+                # only by recreating a new session (or passing the headers on each request)
+                await session.close()
                 return tok.replace('"', '')
-            # req = self.session.post(url, headers=head, data=json.dumps(request_data), **self.request_params)
+
             # Cleaning password after authentication
             self.__password = ""
         except (ConnectionError, TimeoutError):
             raise CyberarkException("Network problem connecting to PVWA")
         except Exception as err:
             raise CyberarkException(err)
 
@@ -120,21 +146,20 @@
         self.__token = None
         return True
 
     async def check_token(self) -> bool or None:
         if self.__token is None:
             return None
         url, head = self.get_url("api/LoginsInfo")
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=head, **self.request_params) as req:
-                # req = self.session.get(url, headers=head, **self.request_params)
-                if req.status != 200:
-                    self.__token = None
-                    return False
-                return True
+        session = self.get_session()
+        async with session.get(url, headers=head, **self.request_params) as req:
+            if req.status != 200:
+                self.__token = None
+                return False
+            return True
 
     async def get_aim_secret(self, aim_host, appid, username, cert_file: str, cert_key: str, ca_file):
         if appid is None:
             raise AiobastionException("Missing mandatory parameter : AppID")
 
         if cert_file is None and cert_key is None:
             raise AiobastionException("Provide cert_file and cert_key arguments in order to connect")
@@ -171,15 +196,15 @@
         password = await self.get_aim_secret(aim_host, appid, username, cert_file, cert_key, root_ca)
 
         try:
             self.__token = self.__login_cyberark(username, password, self.config.authtype)
         except CyberarkException as err:
             raise GetTokenException(err)
 
-    async def login(self, username=None, password=None, auth_type="Cyberark"):
+    async def login(self, username=None, password=None, auth_type=""):
         if await self.check_token():
             return
 
         if username is None:
             if self.config.username is None:
                 raise AiobastionException("Username must be provided on login call or in configuration file")
             username = self.config.username
@@ -195,41 +220,42 @@
                         raise AiobastionException(
                             "Missing AIM information to perform AIM authentication, see documentation")
                 else:
                     raise AiobastionException("Password must be provided on login call or in configuration file")
             else:
                 password = self.config.password
 
-        if self.config.authtype is not None:
-            auth_type = self.config.authtype
+        if auth_type == "":
+            if self.authtype is not None:
+                auth_type = self.authtype
+            else:
+                auth_type = "Cyberark"
+
 
         try:
             self.__token = await self.__login_cyberark(username, password, auth_type)
             head = {'Content-type': 'application/json',
                     'Authorization': self.__token}
 
             # update the session
-            await self.session.close()
             self.session = aiohttp.ClientSession(headers=head)
-
         except CyberarkException as err:
             raise GetTokenException(err)
 
     def get_session(self):
         if self.__token is None:
             head = {"Content-type": "application/json", "Authorization": "None"}
             self.session = aiohttp.ClientSession(headers=head)
         elif self.session is None:
             head = {'Content-type': 'application/json',
                     'Authorization': self.__token}
             self.session = aiohttp.ClientSession(headers=head)
 
         if self.__sema is None:
             self.__sema = asyncio.Semaphore(self.max_concurrent_tasks)
-
         return self.session
 
     async def close_session(self):
         try:
             await self.session.close()
         except (CyberarkException, AttributeError):
             pass
@@ -245,14 +271,15 @@
                     'Authorization': self.__token}
 
         return addr, head
 
     def to_json(self):
         serialized = {
             "api_host": self.config.PVWA,
+            "authtype": self.config.authtype,
             "timeout": self.config.timeout,
             "verify": self.config.PVWA_CA,
             "cpm": self.config.CPM,
             "retention": self.config.retention,
             "max_concurrent_tasks": self.config.max_concurrent_tasks,
             "token": self.__token,
         }
@@ -277,35 +304,30 @@
         :param data: valid json data if needed
         :return:
         """
         assert method.lower() in ("post", "delete", "get", "patch")
 
         url, head = self.get_url(short_url)
 
-        # try:
-
         session = self.get_session()
-        # async with __sema
+
         async with self.__sema:
             async with session.request(method, url, json=data, params=params, **self.request_params) as req:
                 if req.status in (200, 201, 204):
                     try:
                         if len(await req.read()) == 0:
                             return True
                         else:
                             return filter_func(await req.json())
                         # return filter_func(await req.json())
                     except ContentTypeError:
                         response = await req.text()
                         try:
                             return json.loads(response)
                         except (ContentTypeError, json.decoder.JSONDecodeError):
-                            # if response.startswith('"') and response.endswith('"'):
-                            #     # remove double quotes from string
-                            #     return response[1:-1]
                             if len(response) > 0:
                                 return response
                             else:
                                 return True
                         except:
                             raise
                 else:
```

### Comparing `aiobastion-0.0.6/aiobastion/exceptions.py` & `aiobastion-0.0.9/aiobastion/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/platforms.py` & `aiobastion-0.0.9/aiobastion/platforms.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/safe.py` & `aiobastion-0.0.9/aiobastion/safe.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/users.py` & `aiobastion-0.0.9/aiobastion/users.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion/utilities.py` & `aiobastion-0.0.9/aiobastion/utilities.py`

 * *Files identical despite different names*

### Comparing `aiobastion-0.0.6/aiobastion.egg-info/PKG-INFO` & `aiobastion-0.0.9/aiobastion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aiobastion
-Version: 0.0.6
+Version: 0.0.9
 Summary: Manage your Cyberark implementation
 Home-page: https://github.com/labanquepostale/aiobastion
 Author: Gautier Leveille
 Author-email: gautier.leveille@labanquepostale.fr
 Project-URL: Bug Tracker, https://github.com/labanquepostale/aiobastion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiobastion-0.0.6/setup.cfg` & `aiobastion-0.0.9/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = aiobastion
-version = 0.0.6
+version = 0.0.9
 author = Gautier Leveille
 author_email = gautier.leveille@labanquepostale.fr
 description = Manage your Cyberark implementation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/labanquepostale/aiobastion
 project_urls = 
 	Bug Tracker = https://github.com/labanquepostale/aiobastion/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
 
 [options]
 package_dir = 
 packages = find:
```

