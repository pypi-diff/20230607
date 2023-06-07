# Comparing `tmp/alegrapy-0.0.1.tar.gz` & `tmp/alegrapy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alegrapy-0.0.1.tar", last modified: Mon Jun  5 01:19:26 2023, max compression
+gzip compressed data, was "alegrapy-0.0.2.tar", last modified: Wed Jun  7 15:47:23 2023, max compression
```

## Comparing `alegrapy-0.0.1.tar` & `alegrapy-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-05 01:19:26.812515 alegrapy-0.0.1/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 alegrapy-0.0.1/LICENSE.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)     2008 2023-06-05 01:19:26.812515 alegrapy-0.0.1/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)     1383 2023-03-09 17:24:08.000000 alegrapy-0.0.1/README.md
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-05 01:19:26.808514 alegrapy-0.0.1/alegrapy/
--rw-rw-r--   0 andres    (1000) andres    (1000)      224 2023-06-05 01:18:37.000000 alegrapy-0.0.1/alegrapy/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1421 2023-06-05 01:18:28.000000 alegrapy-0.0.1/alegrapy/actions.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      137 2023-06-05 01:18:43.000000 alegrapy-0.0.1/alegrapy/contacts.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      137 2023-06-05 01:18:47.000000 alegrapy-0.0.1/alegrapy/invoices.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      131 2023-06-05 01:18:52.000000 alegrapy-0.0.1/alegrapy/items.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      137 2023-06-05 01:19:01.000000 alegrapy-0.0.1/alegrapy/payments.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1738 2023-06-05 01:18:30.000000 alegrapy-0.0.1/alegrapy/session.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-05 01:19:26.812515 alegrapy-0.0.1/alegrapy.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     2008 2023-06-05 01:19:26.000000 alegrapy-0.0.1/alegrapy.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      331 2023-06-05 01:19:26.000000 alegrapy-0.0.1/alegrapy.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-05 01:19:26.000000 alegrapy-0.0.1/alegrapy.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-05 01:19:26.000000 alegrapy-0.0.1/alegrapy.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-05 01:19:26.000000 alegrapy-0.0.1/alegrapy.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-05 01:19:26.812515 alegrapy-0.0.1/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)     1037 2023-06-05 01:18:58.000000 alegrapy-0.0.1/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-07 15:47:23.926539 alegrapy-0.0.2/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 alegrapy-0.0.2/LICENSE.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2025 2023-06-07 15:47:23.926539 alegrapy-0.0.2/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1400 2023-06-05 01:23:02.000000 alegrapy-0.0.2/README.md
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-07 15:47:23.926539 alegrapy-0.0.2/alegrapy/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      224 2023-06-05 01:18:37.000000 alegrapy-0.0.2/alegrapy/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1449 2023-06-06 02:55:54.000000 alegrapy-0.0.2/alegrapy/actions.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      137 2023-06-05 01:18:43.000000 alegrapy-0.0.2/alegrapy/contacts.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      137 2023-06-05 01:18:47.000000 alegrapy-0.0.2/alegrapy/invoices.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      131 2023-06-05 01:18:52.000000 alegrapy-0.0.2/alegrapy/items.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      137 2023-06-05 01:19:01.000000 alegrapy-0.0.2/alegrapy/payments.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1748 2023-06-06 02:56:52.000000 alegrapy-0.0.2/alegrapy/session.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-07 15:47:23.926539 alegrapy-0.0.2/alegrapy.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2025 2023-06-07 15:47:23.000000 alegrapy-0.0.2/alegrapy.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      331 2023-06-07 15:47:23.000000 alegrapy-0.0.2/alegrapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-07 15:47:23.000000 alegrapy-0.0.2/alegrapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-07 15:47:23.000000 alegrapy-0.0.2/alegrapy.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-07 15:47:23.000000 alegrapy-0.0.2/alegrapy.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-07 15:47:23.926539 alegrapy-0.0.2/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1037 2023-06-07 15:46:52.000000 alegrapy-0.0.2/setup.py
```

### Comparing `alegrapy-0.0.1/LICENSE.txt` & `alegrapy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alegrapy-0.0.1/PKG-INFO` & `alegrapy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alegrapy
-Version: 0.0.1
+Version: 0.0.2
 Summary: alegra-api-client: Python package for consuming the Alegra API
 Home-page: https://github.com/andresroh/alegrapy_pkg
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
@@ -33,22 +33,24 @@
 
 - Ingresar a la aplicación de [Alegra](https://www.alegra.com/).
 - Haz clic sobre el vínculo "Configuración" en la parte superior derecha de la pantalla de Alegra y haz clic en la sección "API - Integraciones con otros sistemas"
 - En la nueva pantalla puedes encontrar el correo con el cual debes acceder al API y el token. Si aún no cuentas con un token puedes generarlo también.
 
 ### 2. Instalación
 
-En construcción...
+```
+pip install alegrapy==0.0.1
+```
 
 ### 3. Uso
 
 Un ejemplo para usar este paquete
 
 ```py
-from alegra import invoices,contacts, session
+from alegra import invoices, contacts, session
 
 session.user = "your_email@domnain.com"
 session.token = "your_token"
 
 invoice = invoices()
 invoice.read(1,fields='pdf')
 invoice.list(0,3)
```

### Comparing `alegrapy-0.0.1/README.md` & `alegrapy-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 
 - Ingresar a la aplicación de [Alegra](https://www.alegra.com/).
 - Haz clic sobre el vínculo "Configuración" en la parte superior derecha de la pantalla de Alegra y haz clic en la sección "API - Integraciones con otros sistemas"
 - En la nueva pantalla puedes encontrar el correo con el cual debes acceder al API y el token. Si aún no cuentas con un token puedes generarlo también.
 
 ### 2. Instalación
 
-En construcción...
+```
+pip install alegrapy==0.0.1
+```
 
 ### 3. Uso
 
 Un ejemplo para usar este paquete
 
 ```py
-from alegra import invoices,contacts, session
+from alegra import invoices, contacts, session
 
 session.user = "your_email@domnain.com"
 session.token = "your_token"
 
 invoice = invoices()
 invoice.read(1,fields='pdf')
 invoice.list(0,3)
```

### Comparing `alegrapy-0.0.1/alegrapy/actions.py` & `alegrapy-0.0.2/alegrapy/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         """
         params = {}
 
         if kwargs:
             params = kwargs
 
         endpoint = f"{session.url}{self.endpoint}/{id}"
-        session.query('get', endpoint, params=params)
+        return session.query('get', endpoint, params=params)
 
     def list(self, start, limit, **kwargs):
         """search multiples results and returns a list
 
         Args:
             start (int): initial position
             limit (int): list length (max 30)
@@ -36,28 +36,28 @@
                   'order_direction': 'ASC',
                   'order_field': 'id'
                   }
 
         if kwargs:
             params.update(kwargs)
 
-        session.query('get', endpoint, params=params)
+        return session.query('get', endpoint, params=params)
 
     def create(self, params):
         """send information to create in alegra
 
         Args:
             params (dict): data to create
         """
 
         endpoint = f"{session.url}{self.endpoint}"
-        session.query('post', endpoint, params=params)
+        return session.query('post', endpoint, params=params)
 
     def delete(self, id):
         """delete by id
 
         Args:
             id (int): query id
         """
 
         endpoint = f"{session.url}{self.endpoint}/{id}"
-        session.query('get', endpoint)
+        return session.query('get', endpoint)
```

### Comparing `alegrapy-0.0.1/alegrapy/session.py` & `alegrapy-0.0.2/alegrapy/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 
         response = request(method,
                            url,
                            params=params,
                            data=json.dumps(data),
                            headers=self.headers)
 
-        short_url = url.replace("alegra.com/api/v1", "...")
+        short_url = url.replace("https://api.alegra.com/api/v1", "")
+
         if response.status_code == 200:
 
             logging.info(f"{method} - {short_url} - Successful!")
             return json.loads(response.text)
 
         logging.warning(
             f"{method} - {short_url} - {response.json()['message']}")
```

### Comparing `alegrapy-0.0.1/alegrapy.egg-info/PKG-INFO` & `alegrapy-0.0.2/alegrapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alegrapy
-Version: 0.0.1
+Version: 0.0.2
 Summary: alegra-api-client: Python package for consuming the Alegra API
 Home-page: https://github.com/andresroh/alegrapy_pkg
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
@@ -33,22 +33,24 @@
 
 - Ingresar a la aplicación de [Alegra](https://www.alegra.com/).
 - Haz clic sobre el vínculo "Configuración" en la parte superior derecha de la pantalla de Alegra y haz clic en la sección "API - Integraciones con otros sistemas"
 - En la nueva pantalla puedes encontrar el correo con el cual debes acceder al API y el token. Si aún no cuentas con un token puedes generarlo también.
 
 ### 2. Instalación
 
-En construcción...
+```
+pip install alegrapy==0.0.1
+```
 
 ### 3. Uso
 
 Un ejemplo para usar este paquete
 
 ```py
-from alegra import invoices,contacts, session
+from alegra import invoices, contacts, session
 
 session.user = "your_email@domnain.com"
 session.token = "your_token"
 
 invoice = invoices()
 invoice.read(1,fields='pdf')
 invoice.list(0,3)
```

### Comparing `alegrapy-0.0.1/setup.py` & `alegrapy-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'alegra-api-client: Python package for consuming the Alegra API'
 PACKAGE_NAME = 'alegrapy'
 AUTHOR = 'Camilo Andrés Rodríguez'
 EMAIL = 'andres.roh@gmail.com'
 GITHUB_URL = 'https://github.com/andresroh/alegrapy_pkg'
 
 setup(
```

