# Comparing `tmp/webexpython-0.2.16.tar.gz` & `tmp/webexpython-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexpython-0.2.16.tar", last modified: Thu May 11 14:48:16 2023, max compression
+gzip compressed data, was "webexpython-0.2.18.tar", last modified: Wed Jun  7 16:46:19 2023, max compression
```

## Comparing `webexpython-0.2.16.tar` & `webexpython-0.2.18.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-11 14:48:16.779152 webexpython-0.2.16/
--rw-r--r--   0 josh       (501) staff       (20)      198 2023-05-11 14:48:16.778724 webexpython-0.2.16/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-11 14:48:16.779289 webexpython-0.2.16/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      327 2023-05-11 14:47:24.000000 webexpython-0.2.16/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-11 14:48:16.775563 webexpython-0.2.16/webexpython/
--rw-r--r--   0 josh       (501) staff       (20)       20 2022-03-17 16:32:34.000000 webexpython-0.2.16/webexpython/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    24824 2023-05-11 14:47:05.000000 webexpython-0.2.16/webexpython/webex.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-11 14:48:16.778028 webexpython-0.2.16/webexpython.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      198 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      227 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        9 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       12 2023-05-11 14:48:16.000000 webexpython-0.2.16/webexpython.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:46:19.535113 webexpython-0.2.18/
+-rw-r--r--   0 josh       (501) staff       (20)      198 2023-06-07 16:46:19.534763 webexpython-0.2.18/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-07 16:46:19.535260 webexpython-0.2.18/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      327 2023-06-07 16:45:33.000000 webexpython-0.2.18/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:46:19.531553 webexpython-0.2.18/webexpython/
+-rw-r--r--   0 josh       (501) staff       (20)       20 2022-03-17 16:32:34.000000 webexpython-0.2.18/webexpython/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    22671 2023-06-07 16:45:25.000000 webexpython-0.2.18/webexpython/webex.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:46:19.534121 webexpython-0.2.18/webexpython.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      198 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      227 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        9 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       12 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/top_level.txt
```

### Comparing `webexpython-0.2.16/webexpython/webex.py` & `webexpython-0.2.18/webexpython/webex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,384 +1,360 @@
-import requests
-import json
-import time
-import pprint
+import requests, json, time, pprint
 
 # This is the master webex.py that we will publish
 
-
 def ppJson(jsonThing, sort=True, indents=4):
     if type(jsonThing) is str:
         print(json.dumps(json.loads(jsonThing), sort_keys=sort, indent=indents))
     else:
         print(json.dumps(jsonThing, sort_keys=sort, indent=indents))
     return None
 
-
 def timestamp():
     timestr = time.strftime("%Y%m%d-%H%M%S") + " "
     return timestr
 
-
-def getTokenFromCode(clientId, clientSecret, code, redirectUri):
+def getTokenFromCode(clientId,clientSecret,code,redirectUri):
     APIURI = "https://webexapis.com/v1/access_token"
 
     httpBodyText = {'grant_type': 'authorization_code',
-                    'client_id': clientId,
-                    'client_secret': clientSecret,
-                    'code': code,
-                    'redirect_uri': redirectUri}
-
-    httpBodyJSON = json.dumps(httpBodyText)
-    APIHEADERS = {'Content-Type': 'application/json'}
-    APIRESPONSE = requests.post(APIURI, headers=APIHEADERS, data=httpBodyJSON)
+            'client_id' : clientId,
+            'client_secret' : clientSecret,
+            'code' : code,
+            'redirect_uri' : redirectUri}
+            
+    httpBodyJSON = json.dumps(httpBodyText) 
+    APIHEADERS = { 'Content-Type' : 'application/json'}
+    APIRESPONSE = requests.post(APIURI, headers=APIHEADERS, data = httpBodyJSON) 
     results = APIRESPONSE.json()
-
+    
     if "error" in json.dumps(results):
         errorDescription = json.dumps(results['error_description'])
         return errorDescription
     else:
         return results
 
-# Usage for getTokenFromCode()
+#Usage for getTokenFromCode()
 
-# results = webex.getTokenFromCode(client_id, client_secret, code, redirect_uri)
+#results = webex.getTokenFromCode(client_id, client_secret, code, redirect_uri)
 
-# if "access_token" in results:
+#if "access_token" in results:
 #    print("Access Token: " + results['access_token'] + "\n")
 #    print("Refresh Token: " + results['refresh_token'] + "\n")
-# else:
+#else:
 #    print("Error: " + results + "\n")
 
 
-# Get a bearer token from the refresh token (the bearer tokens expire frequently, while the refresh tokens do not)
-def refreshToken(clientId, clientSecret, refreshToken):
+#Get a bearer token from the refresh token (the bearer tokens expire frequently, while the refresh tokens do not)
+def refreshToken(clientId,clientSecret,refreshToken):
     APIURI = "https://webexapis.com/v1/access_token"
-
+    
     httpBodyText = {'grant_type': 'refresh_token',
-                    'client_id': clientId,
-                    'client_secret': clientSecret,
-                    'refresh_token': refreshToken}
-
-    httpBodyJSON = json.dumps(httpBodyText)
-    APIHEADERS = {'Content-Type': 'application/json'}
-    APIRESPONSE = requests.post(APIURI, headers=APIHEADERS, data=httpBodyJSON)
+            'client_id' : clientId,
+            'client_secret' : clientSecret,
+            'refresh_token' : refreshToken}
+
+    httpBodyJSON = json.dumps(httpBodyText) 
+    APIHEADERS = {'Content-Type' : 'application/json'}
+    APIRESPONSE = requests.post(APIURI, headers=APIHEADERS, data = httpBodyJSON) 
     results = APIRESPONSE.json()
     if "error" in json.dumps(results):
         errorDescription = json.dumps(results['error_description'])
         return errorDescription
     else:
         return results
 
-# Usage for refreshToken()
+#Usage for refreshToken()
 # results = webex.refreshToken(client_id,client_secret,refresh_token)
 
 # if "access_token" in results:
 #     print("Access Token: " + results['access_token'] + "\n")
 #     print("Refresh Token: " + results['refresh_token'] + "\n")
 #     #print("Scope: " + results['scope'] + "\n")
-
+    
 # else:
 #     print("Error: " + results + "\n")
 
-# This function will get the Webex UserID value from a provided email address
-
-
-def getUserIdFromEmail(accessToken, emailAddress):
-    APIURIPARAMETERS = {'emailAddress': 'email=' + emailAddress}
+#This function will get the Webex UserID value from a provided email address
+def getUserIdFromEmail(accessToken, emailAddress): 
+    APIURIPARAMETERS = {'emailAddress' : 'email=' + emailAddress }
     APIURI = "https://webexapis.com/v1/people/"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "?" + APIURIPARAMETERS['emailAddress']
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True) 
     results = APIRESPONSE.json()
     return results
 
-# Usage for getUserId()
+#Usage for getUserId()
 # results = webex.getUserIdFromEmail(accessToken,emailAddress)
 
 # id = results["items"][0]["id"]
 # if "items" in results:
-#      print("ID: " + id + "\n")
+#      print("ID: " + id + "\n")    
 # else:
 #      print("Error: " + results + "\n")
 
 
-# List admin audit events in your organization
-def adminAuditEvents(accessToken, orgId, fromDateTime, toDateTime, actorId):
+#List admin audit events in your organization
+def adminAuditEvents(accessToken, orgId, fromDateTime, toDateTime, actorId): 
     APIURIPARAMETERS = {
-        'orgId': 'orgId=' + orgId,
-        'fromDateTime': 'from=' + fromDateTime,
-        'toDateTime': 'to=' + toDateTime,
-        'actorId': 'actorId=' + actorId
-    }
+        'orgId' : 'orgId=' + orgId,
+        'fromDateTime' : 'from=' + fromDateTime,
+        'toDateTime' : 'to=' + toDateTime,
+        'actorId' : 'actorId=' + actorId   
+     }
 
     APIURI = "https://webexapis.com/v1/adminAudit/events"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
-    APIURI = APIURI + "?" + APIURIPARAMETERS['orgId'] + "&" + APIURIPARAMETERS['fromDateTime'] + \
-        "&" + APIURIPARAMETERS['toDateTime'] + \
-        "&" + APIURIPARAMETERS['actorId']
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
+    APIURI = APIURI + "?" + APIURIPARAMETERS['orgId'] + "&" + APIURIPARAMETERS['fromDateTime'] + "&" + APIURIPARAMETERS['toDateTime'] + "&" + APIURIPARAMETERS['actorId']
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True) 
     results = APIRESPONSE.text
     return results
 
-# Usage for adminAuditEvents()
+#Usage for adminAuditEvents()
 # orgId = "your org id"
 # fromDateTime= "2022-01-01T13:12:11.789Z"
 # toDateTime = "2022-12-01T13:12:11.789Z"
 # actorId = "id of the user to audit"
 # results = webex.adminAuditEvents(accessToken, orgId, fromDateTime, toDateTime, actorId)
 # webex.ppJson(results)
 
-
-# Shows details for a person, by ID.
-def getUserDetails(accessToken, userId):
-
+        
+#Shows details for a person, by ID.
+def getUserDetails(accessToken, userId): 
+    
     APIURI = "https://webexapis.com/v1/people"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "/" + userId
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True) 
     results = APIRESPONSE.json()
     return results
 
-# Usage for getUserDetails()
+#Usage for getUserDetails()
 # results = webex.getUserDetails(accessToken, id)
 # webex.ppJson(results)
 
-# This function will get the licenses associated with an organization from a provided org id
-
-
+#This function will get the licenses associated with an organization from a provided org id
 def getLicenses(accessToken, orgId):
     APIURIPARAMETERS = {
-        'orgId': 'orgId=' + orgId
-    }
+        'orgId' : 'orgId=' + orgId  
+     }
     APIURI = "https://webexapis.com/v1/licenses"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "?" + APIURIPARAMETERS['orgId']
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True) 
     results = APIRESPONSE.text
     return results
 
-# Usage for getLicenses()
+#Usage for getLicenses()
 # results = webex.getLicenses(accessToken, orgId)
 # webex.ppJson(results)
-
+ 
 
 def getLocationIds(accessToken, orgId):
     APIURI = "https://webexapis.com/v1/locations"
     APIURIPARAMETERS = {
-        'orgId': 'orgId=' + orgId,
-    }
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+        'orgId' : 'orgId=' + orgId,
+     }
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "?" + APIURIPARAMETERS['orgId']
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)  
     results = APIRESPONSE.text
     return results
 
-# Usage for getLocationIds()
+#Usage for getLocationIds()
 # results = webex.getLocationIds(accessToken, orgId)
 # webex.ppJson(results)
 
-
 def toggleVoicemailEnable(accessToken, orgId, userId, state):
     APIURI = "https://webexapis.com/v1/people/"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "/" + userId + "/features/voicemail" + "?orgId=" + orgId
-
+    
     if state == "TRUE" or state == "true" or state == "True" or state == "t" or state == "T":
-        data = {
-            "enabled": True
-        }
+        data = { 
+                "enabled": True         
+            }
     elif state == "FALSE" or state == "false" or state == "False" or state == "f" or state == "F":
         data = {
-            "enabled": False
-        }
+                "enabled": False         
+            }
 
     httpBodyJSON = json.dumps(data)
 
-    APIRESPONSE = requests.put(
-        APIURI, headers=APIHEADER, verify=True, data=httpBodyJSON)
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, verify=True, data=httpBodyJSON)  
     results = APIRESPONSE.text
     return results
 
 
 def setVoicemailZeroOut(accessToken, orgId, userId, state, destination):
     APIURI = "https://webexapis.com/v1/people"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "/" + userId + "/features/voicemail" + "?orgId=" + orgId
 
     if state == "enable" or state == "ENABLE" or state == "TRUE" or state == "true" or state == "True" or state == "t" or state == "T":
-        data = {
-            "transferToNumber": {
-                "enabled": True,
-                "destination": destination
-            }
-        }
-
-    if state == "disable" or state == "DISABLE" or state == "FALSE" or state == "false" or state == "False" or state == "f" or state == "F":
-        data = {
-            "transferToNumber": {
-                "enabled": False
-            }
-        }
-
+        data = { 
+                "transferToNumber": {
+                    "enabled": True,
+                    "destination": destination
+                }
+            }        
+    
+    if state == "disable" or state == "DISABLE" or state == "FALSE" or state == "false" or state == "False" or state == "f" or state == "F": 
+        data = { 
+                "transferToNumber": {
+                    "enabled": False
+                }
+            }        
+    
     httpBodyJSON = json.dumps(data)
 
-    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=httpBodyJSON)
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=httpBodyJSON)     
     results = APIRESPONSE.text
     return results
 
-# Usage for setVoicemailZeroOut()
+#Usage for setVoicemailZeroOut()
 # results = webex.setVoicemailZeroOut(accessToken, enableOrDisable, userId, destination)
 
-
 def setVoicemailEmailNotify(accessToken, orgId, userId, state, destination):
     APIURI = "https://webexapis.com/v1/people"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "/" + userId + "/features/voicemail" + "?orgId=" + orgId
 
     if state == "enable" or state == "ENABLE" or state == "TRUE" or state == "true" or state == "True" or state == "t" or state == "T":
         print("Enabling Email Notification")
-        data = {"messageStorage": {
-            "storageType": "INTERNAL"
-        },
-            "emailCopyOfMessage": {
+        data = {"messageStorage" : {
+                    "storageType": "INTERNAL" 
+                    },  
+                "emailCopyOfMessage": {
                 "enabled": True,
                 "emailId": destination
-        }
-        }
+                }
+            }        
 
-    if state == "disable" or state == "DISABLE" or state == "FALSE" or state == "false" or state == "False" or state == "f" or state == "F":
+    if state == "disable" or state == "DISABLE" or state == "FALSE" or state == "false" or state == "False" or state == "f" or state == "F": 
         print("Disabling Email Notification")
-        data = {
-            "emailCopyOfMessage": {
+        data = { 
+                "emailCopyOfMessage": {
                 "enabled": False
-            }
-        }
-
-    httpBodyJSON = json.dumps(data)
+                }
+            }          
+    
+    httpBodyJSON = json.dumps(data) 
 
-    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=httpBodyJSON)
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=httpBodyJSON)     
     results = APIRESPONSE.text
     return results
 
-# Usage for setVoicemailEmailNotify()
-# results = webex.setVoicemailEmailNotify(accessToken, enableOrDisable, userId, destination)
-
+#Usage for setVoicemailEmailNotify()
+#results = webex.setVoicemailEmailNotify(accessToken, enableOrDisable, userId, destination)
 
 def addPstnNumber(accessToken, number, orgId, location):
     APIURI = "https://webexapis.com/v1/telephony/config/locations/"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + location + "/numbers" + "?orgId=" + orgId
 
-    data = {
-        "phoneNumbers": [number],
-        "state": "ACTIVE"
+    data = { 
+        "phoneNumbers": [ number],
+     "state": "ACTIVE"  
     }
 
-    httpBodyJSON = json.dumps(data)
+    httpBodyJSON = json.dumps(data) 
 
-    APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data=httpBodyJSON)
+    APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data=httpBodyJSON) 
     if APIRESPONSE.text == "":
         results = ""
-    else:
+    else: 
         results = APIRESPONSE.json()
     return results
 
-# Usage for addPstnNumber()
-# results = webex.addPstnNumber(accessToken, number, orgId, location)
+#Usage for addPstnNumber()
+#results = webex.addPstnNumber(accessToken, number, orgId, location)
 
 
 def getLicenses(accessToken, orgId):
     APIURI = "https://webexapis.com/v1/licenses"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "?orgId=" + orgId
-
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER)
+  
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER) 
     results = APIRESPONSE.text
     return results
 
-# Usage for getLicenses()
-# results = webex.getLicenses(accessToken, orgId)
-
+#Usage for getLicenses()
+#results = webex.getLicenses(accessToken, orgId)
 
 def updateUser(accessToken, userId, orgId, jsondata):
     APIURI = "https://webexapis.com/v1/people/"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + userId + "?callingData=true" + "&orgId=" + orgId
 
-    APIRESPONSE = requests.put(
-        APIURI, headers=APIHEADER, data=json.dumps(jsondata))
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data = json.dumps(jsondata))
     return APIRESPONSE.json()
 
 
 def getOrganizations(accessToken):
     APIURI = "https://webexapis.com/v1/organizations"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
-
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER)
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
+     
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER) 
     return APIRESPONSE.text
 
-
 def getOrganizationDetails(accessToken, orgId):
     APIURI = "https://webexapis.com/v1/organizations"
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     APIURI = APIURI + "/" + orgId
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True) 
     return APIRESPONSE.text
 
-
 def listHuntGroups(accessToken, orgId):
     APIURI = "https://webexapis.com/v1/telephony/config/huntGroups"
     APIURLPARAMETERS = "?orgId=" + orgId
     APIURI = APIURI + APIURLPARAMETERS
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER)
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER) 
     huntGroups = APIRESPONSE.text
     return huntGroups
 
-
-def getHuntGroupDetails(accessToken, locationId, huntGroupId, orgId):
-    APIURI = "https://webexapis.com/v1/telephony/config/locations/" + \
-        locationId + "/huntGroups/" + huntGroupId
+def getHuntGroupDetails(accessToken, locationId, huntGroupId, orgId): 
+    APIURI = "https://webexapis.com/v1/telephony/config/locations/" + locationId + "/huntGroups/" + huntGroupId
     APIURLPARAMETERS = "?orgId=" + orgId
     APIURI = APIURI + APIURLPARAMETERS
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
-    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True)
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER, verify=True) 
     results = APIRESPONSE.json()
     return results
 
-
 def addHuntGroupAgent(accessToken, locationId, huntGroupId, jsonData, orgId):
-    APIURI = "https://webexapis.com/v1/telephony/config/locations/" + \
-        locationId + "/huntGroups/" + huntGroupId
+    APIURI = "https://webexapis.com/v1/telephony/config/locations/" + locationId + "/huntGroups/" + huntGroupId
     APIURLPARAMETERS = "?orgId=" + orgId
     APIURI = APIURI + APIURLPARAMETERS
-    APIHEADER = {'Authorization': 'Bearer ' + accessToken,
-                 'Content-Type': 'application/json', 'Accept': '*/*'}
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
     API_DATA = jsonData
-
-    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=API_DATA)
+        
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data = API_DATA)
     results = APIRESPONSE.text
     return results
 
+def listCallerId(accessToken, userId, orgId):
+    APIURI = "https://webexapis.com/v1/people/"
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
+    APIURI = APIURI + userId + "/features/callerId" + "?orgId=" + orgId
+    APIRESPONSE = requests.get(APIURI, headers=APIHEADER) 
+    callerId = APIRESPONSE.json()
+    return callerId
+
+def updateCallerId(accessToken, userId, orgId, jsondata):
+    APIURI = "https://webexapis.com/v1/people/"
+    APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
+    APIURI = APIURI + userId + "/features/callerId" + "?orgId=" + orgId
+
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data = json.dumps(jsondata))
+    return APIRESPONSE.text
+
 
 def createWorkspaceAccessCode(accessToken, workspaceId, orgId, code, description):
     APIURI = "https://webexapis.com/v1/workspaces/" + \
         workspaceId + "/features/outgoingPermission/accessCodes"
     APIURLPARAMETERS = "?orgId=" + orgId
     APIURI = APIURI + APIURLPARAMETERS
     APIHEADER = {'Authorization': 'Bearer ' + accessToken,
@@ -396,149 +372,91 @@
     APIURI = "https://webexapis.com/v1/telephony/config/locations/" + \
         locationId + "/outgoingPermission/accessCodes"
     APIURLPARAMETERS = "?orgId=" + orgId
     APIURI = APIURI + APIURLPARAMETERS
     APIHEADER = {'Authorization': 'Bearer ' + accessToken,
                  'Content-Type': 'application/json', 'Accept': '*/*'}
     API_DATA = {
-        "code": code,
-        "description": description
+        "accessCodes": [
+            {
+                "code": code,
+                "description": description
+            }
+        ]
     }
-    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=API_DATA)
+    httpBodyJSON = json.dumps(API_DATA)
+
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=httpBodyJSON)
     results = APIRESPONSE.text
     return results
 
 
 def createVoicemailGroup(accessToken,
-                              locationId,
-                              orgId,
-                              voicemailGroupName,
-                              phoneNumber,
-                              extension,
-                              firstName,
-                              lastName,
-                              passcode,
-                              languageCode,
-                              messageStorageType,
-                              messageStorageExternalEmail,
-                              notificationsEnabled,
-                              notificationsDestination,
-                              faxMessageEnabled,
-                              faxMessagePhoneNumber,
-                              faxMessageExtension,
-                              transferToNumberEnabled,
-                              transferToNumberDestination,
-                              emailCopyOfMessageEnabled,
-                              emailCopyOfMessageEmailId
-                              ):
-
-    APIURI = "https://webexapis.com/v1/telephony/config/locations/" + locationId + "/voicemailGroups"
+                         locationId,
+                         orgId,
+                         voicemailGroupName,
+                         phoneNumber,
+                         extension,
+                         firstName,
+                         lastName,
+                         passcode,
+                         languageCode,
+                         messageStorageType,
+                         messageStorageExternalEmail,
+                         notificationsEnabled,
+                         notificationsDestination,
+                         faxMessageEnabled,
+                         faxMessagePhoneNumber,
+                         faxMessageExtension,
+                         transferToNumberEnabled,
+                         transferToNumberDestination,
+                         emailCopyOfMessageEnabled,
+                         emailCopyOfMessageEmailId
+                         ):
+    APIURI = "https://webexapis.com/v1/telephony/config/locations/" + \
+        locationId + "/voicemailGroups"
     APIURLPARAMETERS = "?orgId=" + orgId
     APIURI = APIURI + APIURLPARAMETERS
-    pprint.pprint(APIURI)
     APIHEADER = {'Authorization': 'Bearer ' + accessToken,
                  'Content-Type': 'application/json', 'Accept': '*/*'}
-   
-    baseSettings = {"name": voicemailGroupName,
-                    "phoneNumber": phoneNumber,
-                    "extension": extension,
-                    "firstName": firstName,
-                    "lastName": lastName,
-                    "passcode": passcode,
-                    "languageCode": languageCode,
-                    }
-    
-    if messageStorageExternalEmail != "":
-          messageStorageSettings = {
-            "messageStorage": {
-               "storageType": messageStorageType,
-               "externalEmail": messageStorageExternalEmail
-        }
-     }
-    elif messageStorageExternalEmail == "":
-          messageStorageSettings = {
-            "messageStorage": {
-               "storageType": messageStorageType,
-        }
-     }
-
-    if notificationsEnabled == "TRUE" or notificationsEnabled == "true" or notificationsEnabled == "True" or notificationsEnabled == "t" or notificationsEnabled == "T":
-        notificationsEnabledSettings = {
-            "notifications": {
-            "enabled": True,
+    API_DATA = {
+        "name": voicemailGroupName,
+        "phoneNumber": phoneNumber,
+        "extension": extension,
+        "firstName": firstName,
+        "lastName": lastName,
+        "passcode": passcode,
+        "languageCode": languageCode,
+        "messageStorage": {
+            "storageType": messageStorageType,
+            "externalEmail": messageStorageExternalEmail
+        },
+        "notifications": {
+            "enabled": notificationsEnabled,
             "destination": notificationsDestination,
-        }
-        }
-    elif notificationsEnabled == "FALSE" or notificationsEnabled == "false" or notificationsEnabled == "False" or notificationsEnabled == "f" or notificationsEnabled == "F":
-        notificationsEnabledSettings = {
-            "notifications": {
-            "enabled": False
-        }
-        }
-
-    if faxMessageEnabled == "TRUE" or faxMessageEnabled == "true" or faxMessageEnabled == "True" or faxMessageEnabled == "t" or faxMessageEnabled == "T":
-        faxMessageEnabledSettings = {
-            "faxMessage": {
-            "enabled": True,
+        },
+        "faxMessage": {
+            "enabled": faxMessageEnabled,
             "phoneNumber": faxMessagePhoneNumber,
             "extension": faxMessageExtension
-        }
-        }
-    elif faxMessageEnabled == "FALSE" or faxMessageEnabled == "false" or faxMessageEnabled == "False" or faxMessageEnabled == "f" or faxMessageEnabled == "F":
-        faxMessageEnabledSettings = {
-            "faxMessage": {
-            "enabled": False
-        }
-        }
-
-    if transferToNumberEnabled == "TRUE" or transferToNumberEnabled == "true" or transferToNumberEnabled == "True" or transferToNumberEnabled == "t" or transferToNumberEnabled == "T":
-        transferToNumberEnabledSettings = {
-            "transferToNumber": {
-            "enabled": True,
+        },
+        "transferToNumber": {
+            "enabled": transferToNumberEnabled,
             "destination": transferToNumberDestination
-        }
-        }
-    elif transferToNumberEnabled == "FALSE" or transferToNumberEnabled == "false" or transferToNumberEnabled == "False" or transferToNumberEnabled == "f" or transferToNumberEnabled == "F":
-        transferToNumberEnabledSettings = {
-            "transferToNumber": {
-            "enabled": False
-        }
-        }
-
-    if emailCopyOfMessageEnabled == "TRUE" or emailCopyOfMessageEnabled == "true" or emailCopyOfMessageEnabled == "True" or emailCopyOfMessageEnabled == "t" or emailCopyOfMessageEnabled == "T":
-        emailCopyOfMessageEnabledSettings = {
-            "emailCopyOfMessage": {
-            "enabled": True,
+        },
+        "emailCopyOfMessage": {
+            "enabled": emailCopyOfMessageEnabled,
             "emailId": emailCopyOfMessageEmailId
         }
-        }
-    elif emailCopyOfMessageEnabled == "FALSE" or emailCopyOfMessageEnabled == "false" or emailCopyOfMessageEnabled == "False" or emailCopyOfMessageEnabled == "f" or emailCopyOfMessageEnabled == "F":
-        emailCopyOfMessageEnabledSettings = {
-            "emailCopyOfMessage": {
-            "enabled": False
-        }
-        }
-
-    voicemailGroupSettings = {}
-    voicemailGroupSettings.update(baseSettings)
-    voicemailGroupSettings.update(messageStorageSettings)
-    voicemailGroupSettings.update(notificationsEnabledSettings)
-    voicemailGroupSettings.update(faxMessageEnabledSettings)   
-    voicemailGroupSettings.update(transferToNumberEnabledSettings)
-    voicemailGroupSettings.update(emailCopyOfMessageEnabledSettings)
-
-    API_DATA = json.dumps(voicemailGroupSettings)
-
-    #webex.ppJson(API_DATA)
-    APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data=API_DATA)
+    }
+    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=API_DATA)
     results = APIRESPONSE.text
     return results
 
 
-
 def createCallPickup(accessToken,
                      locationId,
                      orgId,
                      name,
                      agents
                      ):
     APIURI = "https://webexapis.com/v1/telephony/config/locations/" + \
@@ -553,115 +471,116 @@
             "Y2lzY29zcGFyazovL3VzL1BFT1BMRS80YTc2ZmVmNC1mZjlmLTExZWItYWYwZC00M2YwZjY1NTdjYWI",
             "Y2lzY29zcGFyazovL3VzL1BMQUNFLzU1YjUyZThhLWZmOWYtMTFlYi05ZjRhLTAzZDY1NzdhYzg1Yg",
             "Y2lzY29zcGFyazovL3VzL1ZJUlRVQUxfTElORS85ODFlNTQ0Yy0xOGI0LTQ2MzItYmFkZi1iYWMwZjFkOGJkYWY="]
     }
     APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data=API_DATA)
     results = APIRESPONSE.text
     return results
-
-# Functions below this point are in progress
+#Functions below this point are in progress
 
 # def getAutoAttendants(accessToken, orgId):
 
 #     API_URL_ENDPOINT = "telephony/config/autoAttendants"
 #     APIURLPARAMETERS = "?orgId=" + orgId
 #     FULL_URL = API_URL_PATH + API_URL_ENDPOINT + APIURLPARAMETERS
-
+  
 #     APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
-
+          
 #     #bodyPayloadText = json.dumps(data) # This formats the contents of 'data' into proper JSON for sending in the request body
-#     APIRESPONSE = requests.get(FULL_URL, headers=APIHEADER)
+#     APIRESPONSE = requests.get(FULL_URL, headers=APIHEADER) 
 #     autoAttendants = APIRESPONSE.text
 #     return autoAttendants
 
 
 # def createUser(accessToken, email, extension, DID, firstName, lastName, location, license, orgId):
-#     data = {
+#     data = { 
 #         "emails": email,
-#         #"phoneNumbers":
+#         #"phoneNumbers": 
 #         #{
 #          #"type" : "work",
 #          #"value" : DID
 #         #},
 #         "extension": extension,
 #         "firstName": firstName,
 #         "lastName": lastName,
 #         "orgId": orgId,
 #         "location": location,
 #         "licenses": license
-
+        
 #     }
-
+   
 #     APIURI = APIURI + "people/" + "?" + "callingData=true"
 #     APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
 
-#     bodyPayloadText = json.dumps(data)
+#     bodyPayloadText = json.dumps(data) 
 #     print(bodyPayloadText)
-#     APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data = bodyPayloadText)
+#     APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data = bodyPayloadText) 
 #     results = APIRESPONSE.text
 #     return results
 
-#     bodyPayloadText = json.dumps(data)
+#     bodyPayloadText = json.dumps(data) 
+
+
 
 
 # def deleteUser(accessToken, userId):
 #     APIURI = APIURI + "people/"+ userId
 #     APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
-#     APIRESPONSE = requests.delete(APIURI, headers=APIHEADER, verify=True)
-
+#     APIRESPONSE = requests.delete(APIURI, headers=APIHEADER, verify=True) 
+    
 #     if APIRESPONSE.status_code == 204:
-#         print("Deleted Successfully")
+#         print("Deleted Successfully") 
 #         return("User Found")
 #     else:
 #         return("No User Found")
-
+   
 # def createCallQueue(accessToken, locationId, name, phoneNumber, extension, firstName, lastName, callPolicies, agents):
 #     data = {
-#         "locationId" : locationId,
+#         "locationId" : locationId, 
 #         "name": name,
 #         "phoneNumber": phoneNumber,
 #         "extension": extension,
 #         "firstName": firstName,
 #         "lastName": lastName,
 #         "callPolicies": callPolicies,
 #         "agents": agents,
 #         "enabled": "true",
-#         #"phoneNumbers":
+#         #"phoneNumbers": 
 #         #{
 #          #"type" : "work",
 #          #"value" : DID
 #         #},
-
-
+          
+        
 #     }
 #     APIURI = APIURI + "telephony/config/locations/"+ locationId + "/queues"
 #     APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
-#     APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data = bodyPayloadText)
+#     APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data = bodyPayloadText) 
 
 
 # def getLicenseDetails(accessToken, licenseId):
 
 #     API_URL_ENDPOINT = "licenses"
 #     APIURLPARAMETERS = "/" + licenseId
 #     FULL_URL = API_URL_PATH + API_URL_ENDPOINT + APIURLPARAMETERS
 
 #     APIHEADER =   {'Authorization': 'Bearer ' + accessToken,
 #                 'Content-Type' : 'application/json',
 #                 'Accept' : '*/*'}
 
-#     APIRESPONSE = requests.get(FULL_URL, headers=APIHEADER)
-
+#     APIRESPONSE = requests.get(FULL_URL, headers=APIHEADER) 
+    
 #     return APIRESPONSE
 
 
 # def getLicenses(accessToken, orgId):
 
 #     API_URL_ENDPOINT = "licenses"
 #     APIURLPARAMETERS = "?orgId=" + orgId
 #     FULL_URL = API_URL_PATH + API_URL_ENDPOINT + APIURLPARAMETERS
-
+  
 #     APIHEADER = {'Authorization': 'Bearer ' + accessToken, 'Content-Type' : 'application/json', 'Accept' : '*/*'}
-
+          
 #     #bodyPayloadText = json.dumps(data) # This formats the contents of 'data' into proper JSON for sending in the request body
-#     APIRESPONSE = requests.get(FULL_URL, headers=APIHEADER)
+#     APIRESPONSE = requests.get(FULL_URL, headers=APIHEADER) 
 #     licenses = APIRESPONSE.text
 #     return licenses
```

