# Comparing `tmp/osais-1.0.47.tar.gz` & `tmp/osais-1.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-d_3bmnv_\osais-1.0.47.tar", last modified: Mon Jun  5 21:05:21 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-dvy__r4l\osais-1.0.48.tar", last modified: Wed Jun  7 07:09:52 2023, max compression
```

## Comparing `osais-1.0.47.tar` & `osais-1.0.48.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 21:05:21.818984 osais-1.0.47/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.47/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-06-05 21:05:21.818984 osais-1.0.47/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.47/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 21:05:21.813985 osais-1.0.47/osais/
--rw-rw-rw-   0        0        0     1041 2023-06-05 20:59:14.000000 osais-1.0.47/osais/__init__.py
--rw-rw-rw-   0        0        0    55617 2023-06-05 20:59:01.000000 osais-1.0.47/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:05:21.817985 osais-1.0.47/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 21:05:21.000000 osais-1.0.47/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.47/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 21:05:21.819983 osais-1.0.47/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-06-05 20:59:29.000000 osais-1.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:09:52.242742 osais-1.0.48/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.48/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-06-07 07:09:52.242742 osais-1.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.48/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 07:09:52.236742 osais-1.0.48/osais/
+-rw-rw-rw-   0        0        0     1041 2023-06-07 07:09:17.000000 osais-1.0.48/osais/__init__.py
+-rw-rw-rw-   0        0        0    57528 2023-06-07 07:09:02.000000 osais-1.0.48/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:09:52.241742 osais-1.0.48/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.48/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 07:09:52.242742 osais-1.0.48/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-06-07 07:09:23.000000 osais-1.0.48/setup.py
```

### Comparing `osais-1.0.47/LICENSE` & `osais-1.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.47/PKG-INFO` & `osais-1.0.48/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.47
+Version: 1.0.48
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.47/osais/__init__.py` & `osais-1.0.48/osais/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.47"
+__version__="1.0.48"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isDebug
 from .osais import osais_isDocker
 from .osais import osais_isLocal
 from .osais import osais_isVirtualAI
```

### Comparing `osais-1.0.47/osais/osais.py` & `osais-1.0.48/osais/osais.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.47"
+__version__="1.0.48"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -157,16 +157,20 @@
     ip_address = socket.gethostbyname(hostname)
     return ip_address
 
 ## get our external ip address
 def get_external_ip():
     import requests
     url = "https://api.ipify.org"
-    response = requests.get(url)
-    return response.text.strip()
+    try: 
+        ## do not fail whole lib for this
+        response = requests.get(url)
+        return response.text.strip()
+    except: 
+        return "0.0.0.0"
 
 ## get our external port
 def get_port(): 
     import socket
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.bind(('localhost', 0))
     port = sock.getsockname()[1]
@@ -176,14 +180,35 @@
 def get_list_of_modules():
     installed_packages = pkg_resources.working_set
     installed_packages_list=[]
     for i in installed_packages:
         installed_packages_list.append({i.key: i.version})
     return installed_packages_list
 
+## create a tunnel via cloudflare
+def create_tunnel(port):
+    import subprocess
+    import re
+    try:
+        command = ['cloudflared', 'tunnel', '--url', f'http://localhost:{port}']
+        process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+
+        for line in process.stderr:
+            data = line.decode('utf-8')
+            output = re.search(r'https:\/\/.*\.trycloudflare\.com', data)
+            if output and output.group(0):
+                return f'{output.group(0)}/'
+
+        print('Could not create a Tunnel')
+        return None
+    
+    except Exception as err:
+        print('Could not create a Tunnel')
+        return None
+    
 ## ------------------------------------------------------------------------
 #       GPU utils
 ## ------------------------------------------------------------------------
 
 ## which GPU is this? (will require access to nvidia-smi)
 def get_gpu_attr(_attr):
    output_to_list = lambda x: x.decode('ascii').split('\n')[:-1]
@@ -432,44 +457,46 @@
 
 gVersionLibOSAIS=__version__    ## version of this library (to keep it latest everywhere)
 gUsername=None                  ## user owning this AI (necessary to claim VirtAI regs)
 
 gName=None                      ## name of this AI (name of engine)
 gVersion="0.0.0"                ## name of this AI's version (version of engine)
 gDescription=None               ## AI's quick description
-gOrigin=None                    ## where this AI came from (on internet)
+gGithub=None                    ## where this AI came from (on internet)
 gMachineName=get_machine_name() ## the name of the machine (will change all the time if inside docker, ot keep same if running on local server)
 gLastChecked_at=datetime.utcnow()  ## when was this AI last used for processing anything
 gLastProcessStart_at=None       ## when was this AI last start event for processing anything
 
 ## virtual AI / local /docker ? note: AI can act BOTH at the same time as VirtualAI and a LocalAI for a gateway
 gIsDocker=is_running_in_docker()   ## are we running in a Docker?
 gIsVirtualAI=False              ## are we working as a Virtual AI config?
 gIsLocal=False                  ## are we working locally (with a gateway)?
 gIsDebug=False                  ## are we working in debug (localhost server)? note: we cannot be PROD and DEBUG at the same time
+gAITunel=None                   ## tunnel for where to call this AI (caller in a docker cannot call localhost:port)
 
 ## OSAIS location
 gOriginOSAIS=None               ## location of OSAIS (Prod or debug)
 
 ## authenticate into OSAIS as a VAI
 gVAIToken=None                  ## VAI token used for authentication into OSAIS
 gVAISecret=None                 ## VAI secret used for authentication into OSAIS
 gVAIAuthToken=None              ## authToken into OSAIS for when working as virtual AI
 
 ## authenticate into OSAIS as a CLIENT (most likely DEMO CLIENT)
 gClientID=None                  ## ID of authenticated client into OSAIS 
 gClientAuthToken=None           ## the resulting Auth token as Client, after login
 
 ## Gateway
-gOriginGateway=None             ## location of the local gateway for this (local) AI, as http://{ip}:{port}
-gGatewayTunnel=None             ## tunnel for the gateway (to be used when inside a docker)
+gOriginGateway=None             ## location of the local gateway for this (local) AI, as http://{ip}:{port} or preferrably <tunnel>
 
 ## AWS related
 gS3=None
 gS3Bucket=None
+gAWSID=None
+gAWSSecret=None
 gAWSSession=None
 
 ## IP and Ports
 gExtIP=get_external_ip()        ## where this AI can be accessed from outside (IP)
 gIPLocal=get_container_ip()     ## where this AI can be accessed locally
 gPortAI=None                    ## port where this AI is accessed (will be set by AI config)
 gPortGateway=3023               ## port where the gateway can be accessed
@@ -504,15 +531,15 @@
 #       Load config
 ## ------------------------------------------------------------------------
 
 # load the config file into a JSON
 def _loadConfig(_name): 
     global gVersion
     global gDescription
-    global gOrigin
+    global gGithub
     global gDefaultCost
 
     _json = None
     _dirFile=None
     try:
         from pathlib import Path
         current_working_directory = Path.cwd()
@@ -523,15 +550,15 @@
         print(f'CRITICAL: No config file {_dirFile}')
         sys.exit()
 
     # do not set global vars for osais config
     if _name!= "osais":
         gVersion=_json["version"]
         gDescription=_json["description"]
-        gOrigin=_json["origin"]
+        gGithub=_json["github"]
         _cost=_json["default_cost"]
         if _cost!=None:
             gDefaultCost=_cost
 
     return _json
 
 # get the full AI config, including JSON params and hardware info
@@ -542,32 +569,41 @@
     global gVAIToken
     global gVAISecret
     global gOriginOSAIS
     global gIsVirtualAI
     global gIPLocal
     global gExtIP
     global gIsLocal
- 
+    global gAITunel
+
     _ip=gExtIP
     if gIsDebug:
         _ip=gIPLocal                ## we register with local ip if we are in local gateway mode
 
+    _location=gAITunel
+    if _location==None:
+        _location=f'http://{_ip}:{gPortAI}/'
+
     _jsonBase=_loadConfig("osais")
     _jsonAI=_loadConfig(_name)
 
     objCudaInfo=getCudaInfo()
     gpuName="no GPU"
     if objCudaInfo != 0 and "name" in objCudaInfo and objCudaInfo["name"]:
         gpuName=objCudaInfo["name"]
 
+    _jsonAI["ip"]=_ip
+    _jsonAI["port"]=gPortAI
+    _jsonAI["location"]=_location
     return {
         "username": gUsername,
         "os": get_os_name(),
         "gpu": gpuName,
         "machine": get_machine_name(),
+        "location": _location,
         "ip": _ip,
         "port": gPortAI,
         "osais": gOriginOSAIS,
         "gateway": "http://"+_ip+":3023/",
         "config_ai": _jsonAI,
         "config_base": _jsonBase
     }
@@ -587,122 +623,140 @@
     global gIsVirtualAI
     return gIsVirtualAI
 
 ## PUBLIC - load the config of this AI
 def osais_loadConfig(_name): 
     return _loadConfig(_name)
 
+def _setPropVal(key, val):
+    global gUsername
+    global gIsVirtualAI
+    global gIsDebug
+    global gIsLocal
+    global gName
+    global gVAIToken
+    global gVAISecret
+    global gAWSSession
+    global gS3
+    global gS3Bucket
+    global gOriginOSAIS
+
+    global gAWSID
+    global gAWSSecret
+
+    if key=='TUNNEL_OSAIS' and val!=None and gOriginOSAIS==None:
+        if gOriginOSAIS==None:
+            if gIsDebug: 
+                if val:
+                    gOriginOSAIS=val     # we prefer to get the tunnel location of osais
+                else:
+                    gOriginOSAIS="http://"+gIPLocal+":3022/"
+            else:
+                gOriginOSAIS="https://opensourceais.com/"
+
+    if key == "USERNAME" and val!=None and gUsername==None:
+        gUsername = val
+
+    if key == "IS_DEBUG" and val!=None:
+        _isDebug= (val=="True")
+        if _isDebug!=gIsDebug:
+            print(f'=> is DEBUG updated to {_isDebug}')
+            gIsDebug=_isDebug
+
+    if key == "IS_LOCAL" and val!=None:
+        _isLocal = (val=="True")
+        if _isLocal!=gIsLocal:
+            print(f'=> is Local updated to {_isLocal}')
+            gIsLocal=_isLocal
+                
+    if key == "IS_VIRTUALAI" and val!=None:
+        _isVirtualAI = (val=="True")
+        if _isVirtualAI!=gIsVirtualAI:
+            print(f'=> is Virtual updated to {_isVirtualAI}')
+            gIsVirtualAI=_isVirtualAI
+
+    if key == "ENGINE" and val!=None:
+        _name = val
+        if _name!=gName:
+            print(f"=> Engine name updated to '{_name}'")
+            gName=_name
+    
+    if key == "S3_BUCKET" and val!=None:
+        _s3 = val
+        if _s3!=gS3Bucket:
+            print(f"=> Set S3 bucket to '{_s3}'")
+            gS3Bucket=_s3
+                
+    if key == "VAI_ID" and val!=None and gVAIToken==None:
+        gVAIToken = val
+    
+    if key == "VAI_SECRET" and val!=None and gVAISecret==None:
+        gVAISecret = val
+    
+    if key == "AWS_ACCESS_KEY_ID" and val!=None and gAWSID==None:
+        gAWSID = val
+    
+    if key=='AWS_ACCESS_KEY_SECRET' and val!=None and gAWSSecret==None:
+        gAWSSecret=val
+
 ## PUBLIC - Get env from file (local or docker)
 def osais_getEnv(_filename):
     global gUsername
     global gIsVirtualAI
     global gIsDebug
     global gIsLocal
     global gName
     global gVAIToken
     global gVAISecret
     global gAWSSession
     global gS3
     global gS3Bucket
     global gOriginOSAIS
-    global gGatewayTunnel
-
-    AWSID=None
-    AWSSecret=None
+    global gAWSID
+    global gAWSSecret
 
     ## read env from config file
     if _filename!=None:
         try:
             with open(_filename, "r") as f:
                 content = f.read()
             print(f'=> Reading env vars from {_filename}')
             variables = content.split("\n")
             for var in variables:
                 if var!="":
                     key, value = var.split("=")
-                    if key == "USERNAME":
-                        gUsername = value
-                    elif key == "IS_DEBUG":
-                        gIsDebug = (value=="True")
-                    elif key == "IS_LOCAL":
-                        gIsLocal = (value=="True")
-                    elif key == "IS_VIRTUALAI":
-                        gIsVirtualAI = (value=="True")
-                    elif key == "ENGINE":
-                        gName = value
-                    elif key == "S3_BUCKET":
-                        gS3Bucket = value
-                    elif key == "VAI_ID":
-                        gVAIToken = value
-                    elif key == "VAI_SECRET":
-                        gVAISecret = value
-                    elif key == "AWS_ACCESS_KEY_ID":
-                        AWSID = value
-                    elif key == "AWS_ACCESS_KEY_SECRET":
-                        AWSSecret = value
-                    elif key == "TUNNEL_GATEWAY":
-                        gGatewayTunnel = value
+                    _setPropVal(key, value)
+
         except Exception as err: 
             consoleLog({"msg": f'No env file {_filename}'})
 
     # overload with env settings if any
-    print(f'=> Setting env vars from ENV...')
-    if os.environ.get('IS_DEBUG'):
-        _isDebug=(os.environ.get('IS_DEBUG')=="True")
-        if _isDebug!=gIsDebug:
-            print(f'=> is DEBUG updated to {_isDebug} from ENV var')
-            gIsDebug=_isDebug
-    if os.environ.get('IS_LOCAL'):
-        _isLocal=(os.environ.get('IS_LOCAL')=="True")
-        if _isLocal!=gIsLocal:
-            print(f'=> is Local updated to {_isLocal} from ENV var')
-            gIsLocal=_isLocal
-    if os.environ.get('IS_VIRTUALAI'):
-        _isVirtualAI=(os.environ.get('IS_VIRTUALAI')=="True")
-        if _isVirtualAI!=gIsVirtualAI:
-            print(f'=> is Virtual updated to {_isVirtualAI} from ENV var')
-            gIsVirtualAI=_isVirtualAI
-    if os.environ.get('ENGINE'):
-        _name=os.environ.get('ENGINE')
-        if _name!=gName:
-            print(f"=> Engine name updated to '{_name}' from ENV var")
-            gName=_name
-    if os.environ.get('S3_BUCKET'):
-        _s3=os.environ.get('S3_BUCKET')
-        if _s3!=gS3Bucket:
-            print(f"=> Set S3 bucket to '{_s3}' from ENV var")
-            gS3Bucket=_s3
-    if os.environ.get('USERNAME') and gUsername==None:
-        gUsername=os.environ.get('USERNAME')
-    if os.environ.get('VAI_ID') and gVAIToken==None:
-        gVAIToken=os.environ.get('VAI_ID')
-    if os.environ.get('VAI_SECRET') and gVAISecret==None:
-        gVAISecret=os.environ.get('VAI_SECRET')
-    if os.environ.get('AWS_ACCESS_KEY_ID') and AWSID==None:
-        AWSID=os.environ.get('AWS_ACCESS_KEY_ID')
-    if os.environ.get('AWS_ACCESS_KEY_SECRET') and AWSSecret==None:
-        AWSSecret=os.environ.get('AWS_ACCESS_KEY_SECRET')
+    print(f'=> Setting env vars from ENV...')    
+    _setPropVal("USERNAME", os.environ.get('USERNAME'))
+    _setPropVal("ENGINE", os.environ.get('ENGINE'))
+    _setPropVal("IS_VIRTUALAI", os.environ.get('IS_VIRTUALAI'))
+    _setPropVal("IS_LOCAL", os.environ.get('IS_LOCAL'))
+    _setPropVal("IS_DEBUG", os.environ.get('IS_DEBUG'))
+    _setPropVal("S3_BUCKET", os.environ.get('S3_BUCKET'))
+    _setPropVal("VAI_ID", os.environ.get('VAI_ID'))
+    _setPropVal("VAI_SECRET", os.environ.get('VAI_SECRET'))
+    _setPropVal("AWS_ACCESS_KEY_ID", os.environ.get('AWS_ACCESS_KEY_ID'))
+    _setPropVal("AWS_ACCESS_KEY_SECRET", os.environ.get('AWS_ACCESS_KEY_SECRET'))    
+    _setPropVal("TUNNEL_OSAIS", os.environ.get('TUNNEL_OSAIS'))
 
-    if AWSID!=None and AWSSecret!=None:
+    ## log into S3
+    if gAWSID!=None and gAWSSecret!=None:
         gAWSSession = boto3.Session(
             region_name="eu-west-2",            ## todo : externalise this
-            aws_access_key_id=AWSID,
-            aws_secret_access_key=AWSSecret
+            aws_access_key_id=gAWSID,
+            aws_secret_access_key=gAWSSecret
         )
         gS3 = gAWSSession.resource('s3')
         print(f'=> Logged into AWS S3')
         
-    if gIsDebug: 
-        gOriginOSAIS="http://"+gIPLocal+":3022/"
-    else:
-        gOriginOSAIS="https://opensourceais.com/"
-
-    if os.environ.get('TUNNEL_GATEWAY') and gGatewayTunnel==None:
-        gGatewayTunnel=os.environ.get('TUNNEL_GATEWAY')
-
     return {
         "name": gName,
         "osais": gOriginOSAIS,
         "username": gUsername,
         "isLocal": gIsLocal,
         "isVirtualAI": gIsVirtualAI,
         "isDebug": gIsDebug
@@ -799,21 +853,21 @@
     global gIsDocker
     global gMachineName
     global gUsername
     global gIsBusy
     global gLastProcessStart_at
     global gLastChecked_at
     global gAverageCostInUSD
+    global gAITunel
 
     objConf=_getFullConfig(gName)
-
     return {
         "name": gName,
         "version": gVersion,
-        "location": f'http://{objConf["ip"]}:{objConf["port"]}/',
+        "location": objConf["location"],
         "osais": objConf["osais"],
         "gateway": objConf["gateway"],
         "isRunning": True,    
         "isDocker": gIsDocker,    
         "lastActive_at": gLastChecked_at,
         "lastProcessStart_at": gLastProcessStart_at,
         "machine": gMachineName,
@@ -841,25 +895,47 @@
     objParam=_getFullConfig(gName)
 
     ## notify gateway
     try:
         response = requests.post(f"{gOriginGateway}api/v1/public/ai/config", headers=headers, data=json.dumps(objParam))
         objRes=response.json()["data"]
         if objRes is None:
-            raise ValueError("CRITICAL: could not notify Gateway")
+            raise ValueError("CRITICAL: could not notify Gateway on "+gOriginGateway)
 
     except Exception as err:
-        consoleLog({"msg":"could not notify Gateway"})
+        consoleLog({"msg":"could not notify Gateway on "+gOriginGateway})
         raise err
     return True
 
 ## PUBLIC - Reset connection to local gateway
-def osais_resetGateway(_localGateway):
+def osais_resetGateway():
     global gOriginGateway
-    gOriginGateway=_localGateway
+    global gOriginOSAIS
+    global gUsername
+
+    ## note: if in Docker, we can only call the gateway on its tunnel
+    ## ask OSAIS the gateways (and tunnel location) for the same owner of this AI
+    try:
+        headers = {
+            "Content-Type": 'application/json', 
+            'Accept': 'text/plain',
+        }
+        response = requests.get(f"{gOriginOSAIS}api/v1/public/user/{gUsername}/gateways", headers=headers)
+        objRes=response.json()["data"]
+        if objRes is None:
+            raise ValueError("could not access OSAIS on "+gOriginOSAIS)
+
+        ## take the first gateway and notify
+        ## todo later ... maybe we update ALL gateways with this AI? (the AI is a slave of all this user's gatyeways?)
+        gOriginGateway=objRes[0]["domain"]
+
+    except Exception as err:
+        consoleLog({"msg":"could not notify OSAIS on "+gOriginOSAIS})
+        raise err
+
     try:
         _connectWithGateway()
     except Exception as err:
         consoleLog({"msg":"Could not reset connection to Gateway"})
         raise err
     
     return True
@@ -1485,56 +1561,51 @@
     global gPortLocalOSAIS
     global gIPLocal
     global gExtIP
     global gOriginGateway
     global gVAIAuthToken
     global gOriginOSAIS
     global gClientAuthToken
-    global gGatewayTunnel
+    global gAITunel
 
     ## load env 
     obj=osais_getEnv(_envFile)
     obj2=osais_getEnv(_envSecret)
     gIsLocal=obj["isLocal"]
     gIsVirtualAI=obj["isVirtualAI"]
     gUsername=obj["username"]
     gName=obj["name"]
 
     ## from env, load AI config
     gConfig=osais_loadConfig(gName)
     gPortAI = gConfig["port"]
     gVersion = gConfig["version"]
 
+    ## try to create a tunnel
+    gAITunel=create_tunnel(gPortAI)
 
     ## make sure we have a config file
     _loadConfig(gName)
 
-    ## where is the Gateway for us? if in Docker, we can only call the gateway on its tunnel
-    gOriginGateway=f"http://{gIPLocal}:{gPortGateway}/"         ## config for local gateway (local and not virtual)
-    if gIsDocker:
-        gOriginGateway=gGatewayTunnel
-
-
     ## where is OSAIS for us?
     ## we set OSAIS location in all cases (even if in gateway) because this AI can generate it s own page for sending reqs (needs a client logged into OSAIS)
-    if gIsDebug:
-        osais_resetOSAIS(f"http://{gIPLocal}:{gPortLocalOSAIS}/")
-    else:
+    if gIsDebug==False:
         osais_resetOSAIS("https://opensourceais.com/")
     
     if gIsVirtualAI:
         try:
             osais_authenticateAI()
         except Exception as err:
             print("=> CRITICAL: Could not connect virtual AI "+gName+ " to OSAIS")
             return None
     
     if gIsLocal:
         try:
-            osais_resetGateway(gOriginGateway)
+            ## where is the Gateway for us? 
+            osais_resetGateway()
         except Exception as err:
             print("CRITICAL: could not notify Gateway at "+gOriginGateway)
             return None
 
     dataClient=authenticateClientAsDemo()
 
     ## init default cost
@@ -1544,18 +1615,21 @@
     print("\r\n<===== Config =====>\r\n")
     print("=> engine:                  "+str(gName) + " v"+str(gVersion))
     if gIsDocker:
         print("=> in Docker:               True")
     else:
         print("=> in Docker:               False")
     print("=> is Debug:                "+str(gIsDebug))
+    print("=> OSAIS:                   "+str(gOriginOSAIS))
     print("\r\n=> is Local:                "+str(gIsLocal))
     if gIsLocal:
         print(" > gateway:                 "+gOriginGateway)
-        print(" > local AI location:       "+str(gIPLocal)+":"+str(gPortAI))
+        print(" > AI location:             "+str(gIPLocal)+":"+str(gPortAI))
+        if gAITunel!=None:
+            print(" > AI tunnel :              "+gAITunel)
     print("\r\n=> is Virtual:              "+str(gIsVirtualAI))
     if gIsVirtualAI:
         print(" > virtAI location (ext.):  "+str(gExtIP)+":"+str(gPortAI))
         print(" > OSAIS location:          "+gOriginOSAIS)
         if gVAIAuthToken!=None:
             print(" > is connected to OSAIS:   True")
         else:
```

### Comparing `osais-1.0.47/osais.egg-info/PKG-INFO` & `osais-1.0.48/osais.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.47
+Version: 1.0.48
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.47/setup.py` & `osais-1.0.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.47',
+    version='1.0.48',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

