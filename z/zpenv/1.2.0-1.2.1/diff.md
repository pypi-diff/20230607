# Comparing `tmp/zpenv-1.2.0.tar.gz` & `tmp/zpenv-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpenv-1.2.0.tar", last modified: Wed Jun  7 09:37:46 2023, max compression
+gzip compressed data, was "zpenv-1.2.1.tar", last modified: Wed Jun  7 12:14:05 2023, max compression
```

## Comparing `zpenv-1.2.0.tar` & `zpenv-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 09:37:46.316000 zpenv-1.2.0/
--rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     5522 2023-06-07 09:37:46.312000 zpenv-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4917 2022-12-26 19:01:11.000000 zpenv-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 09:37:46.315000 zpenv-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 09:37:46.264000 zpenv-1.2.0/zpenv/
--rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.2.0/zpenv/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.2.0/zpenv/__main__.py
--rw-rw-rw-   0        0        0    31666 2023-06-07 09:35:55.000000 zpenv-1.2.0/zpenv/zpenv.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:37:46.306000 zpenv-1.2.0/zpenv.egg-info/
--rw-rw-rw-   0        0        0     5522 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-07 09:37:46.000000 zpenv-1.2.0/zpenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 12:14:05.407000 zpenv-1.2.1/
+-rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5576 2023-06-07 12:14:05.351000 zpenv-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-06-07 09:51:42.000000 zpenv-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 12:14:05.392000 zpenv-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 12:14:04.836000 zpenv-1.2.1/zpenv/
+-rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.2.1/zpenv/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.2.1/zpenv/__main__.py
+-rw-rw-rw-   0        0        0    31764 2023-06-07 12:12:23.000000 zpenv-1.2.1/zpenv/zpenv.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:14:05.284000 zpenv-1.2.1/zpenv.egg-info/
+-rw-rw-rw-   0        0        0     5576 2023-06-07 12:14:02.000000 zpenv-1.2.1/zpenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-07 12:14:04.000000 zpenv-1.2.1/zpenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 12:14:02.000000 zpenv-1.2.1/zpenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-07 12:14:03.000000 zpenv-1.2.1/zpenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-07 12:14:03.000000 zpenv-1.2.1/zpenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 12:14:03.000000 zpenv-1.2.1/zpenv.egg-info/top_level.txt
```

### Comparing `zpenv-1.2.0/LICENSE` & `zpenv-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zpenv-1.2.0/PKG-INFO` & `zpenv-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
@@ -43,14 +43,15 @@
 ```console
 [user@host ~]$ zpenv --install [NomEnvironnement]
 ```
 >- --name = Donner un nom Ã  notre environnement
 >- --tag = Ajouter des tags (sÃ©parÃ©s avec ,)
 >- --comment = Ajouter un commentaire
 >- --projectfolder = SpÃ©cifier le dossier du projet (emplacement du code)
+>- --prompt = SpÃ©cifier le message dans le prompt
 (D'autres options sont disponibles)
 <br>
 
 ## Suppression d'un environnement
 ```console
 [user@host ~]$ zpenv --remove [NomEnvironnement]
 ```
```

### Comparing `zpenv-1.2.0/README.md` & `zpenv-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ```console
 [user@host ~]$ zpenv --install [NomEnvironnement]
 ```
 >- --name = Donner un nom à notre environnement
 >- --tag = Ajouter des tags (séparés avec ,)
 >- --comment = Ajouter un commentaire
 >- --projectfolder = Spécifier le dossier du projet (emplacement du code)
+>- --prompt = Spécifier le message dans le prompt
 (D'autres options sont disponibles)
 <br>
 
 ## Suppression d'un environnement
 ```console
 [user@host ~]$ zpenv --remove [NomEnvironnement]
 ```
```

### Comparing `zpenv-1.2.0/zpenv/zpenv.py` & `zpenv-1.2.1/zpenv/zpenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,18 +447,18 @@
 						OSType = get_os()
 						if OSType=='cmd':
 							activate_file='activate.bat'
 							if os.path.exists(envc['bin_path']+path_rep[0]+activate_file):
 								cmd = ['cmd', '/k']
 								target = ""
 								### Add alias CMD
-								if 'projectfolder' in envc:
+								if 'projectfolder' in envc and len(envc['projectfolder']):
 									target+=f"doskey cdproject=cd {envc['projectfolder']} & "
 								else:
-									target+=f"doskey cdproject=echo "+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+" & "
+									target+=f"doskey cdproject=echo '"+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+"'' & "
 								target+=f"doskey cdenv=cd {envc['env_dir']} & "
 								target+=f"doskey shellenv={envc['env_exe']} & "
 								target+=f"doskey zpenv={sys.executable} -m zpenv $* & "
 								target+=f'doskey help=echo "'+lang(["cdenv      se déplacer dans le dossier de l\'environnement`ncdproject  se déplacer dans le dossier du projet`nshellenv   accéder au shell python`nzpenv      accéder à zpenv","cdenv      move to environment folder`ncdproject  move to project folder`nshellenv   access python shell`nzpenv      access zpenv"])+'" & '
 								### END Add alias
 								target+="pushd "+envc['bin_path']+" & "+activate_file+" & popd"
 								cmd.append(target)
@@ -468,18 +468,18 @@
 
 						elif OSType=='powershell.exe' or os.name=='nt':
 							activate_file='activate.ps1'
 							if os.path.exists(envc['bin_path']+path_rep[0]+activate_file):
 								cmd = ['powershell', '-NoExit', '-Command']
 								target = ""
 								### Add alias PS1
-								if 'projectfolder' in envc:
+								if 'projectfolder' in envc and len(envc['projectfolder']):
 									target+='function cdproject{cd "'+envc['projectfolder']+'"}; '
 								else:
-									target+='function cdproject{Write-Host '+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+'}; '
+									target+='function cdproject{Write-Host "'+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+'"}; '
 								target+='function cdenv{cd "'+envc['env_dir']+'"}; '
 								target+='function shellenv{'+envc['env_exe']+'}; '
 								target+='function zpenv{'+sys.executable+' -m zpenv}; '
 								target+='function help{Write-Host "'+lang(["cdenv      se déplacer dans le dossier de l\'environnement`ncdproject  se déplacer dans le dossier du projet`nshellenv   accéder au shell python`nzpenv      accéder à zpenv","cdenv      move to environment folder`ncdproject  move to project folder`nshellenv   access python shell`nzpenv      access zpenv"])+'"}; '
 								### END Add alias
 								target+='. "'+envc['bin_path']+path_rep[0]+activate_file+'"'
 								cmd.append(target)
@@ -489,15 +489,15 @@
 						
 						else:
 							activate_file='activate'
 							if os.path.exists(envc['bin_path']+path_rep[0]+activate_file):
 								cmd = []
 								target = ""
 								### Add alias Linux
-								if 'projectfolder' in envc:
+								if 'projectfolder' in envc and len(envc['projectfolder']):
 									target+=f"alias cdproject=\'cd {envc['projectfolder']}\' && "
 								else:
 									target+="alias cdproject=\'echo "+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+"\' && "
 								target+=f"alias cdenv='cd {envc['env_dir']}' && "
 								target+=f"alias shellenv='{envc['env_exe']}' && "
 								target+=f"alias zpenv='{sys.executable} -m zpenv $*' && "
 								target+=f'alias help=\'echo -e "'+lang(["cdenv      se déplacer dans le dossier de l\'environnement\ncdproject  se déplacer dans le dossier du projet\nshellenv   accéder au shell python\nzpenv      accéder à zpenv","cdenv      move to environment folder\ncdproject  move to project folder\nshellenv   access python shell\nzpenv      access zpenv"])+'"\' && '
```

### Comparing `zpenv-1.2.0/zpenv.egg-info/PKG-INFO` & `zpenv-1.2.1/zpenv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.2.0
+Version: 1.2.1
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
@@ -43,14 +43,15 @@
 ```console
 [user@host ~]$ zpenv --install [NomEnvironnement]
 ```
 >- --name = Donner un nom Ã  notre environnement
 >- --tag = Ajouter des tags (sÃ©parÃ©s avec ,)
 >- --comment = Ajouter un commentaire
 >- --projectfolder = SpÃ©cifier le dossier du projet (emplacement du code)
+>- --prompt = SpÃ©cifier le message dans le prompt
 (D'autres options sont disponibles)
 <br>
 
 ## Suppression d'un environnement
 ```console
 [user@host ~]$ zpenv --remove [NomEnvironnement]
 ```
```

