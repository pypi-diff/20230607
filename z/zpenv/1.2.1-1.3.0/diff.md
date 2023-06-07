# Comparing `tmp/zpenv-1.2.1.tar.gz` & `tmp/zpenv-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpenv-1.2.1.tar", last modified: Wed Jun  7 12:14:05 2023, max compression
+gzip compressed data, was "zpenv-1.3.0.tar", last modified: Wed Jun  7 13:25:59 2023, max compression
```

## Comparing `zpenv-1.2.1.tar` & `zpenv-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 12:14:05.407000 zpenv-1.2.1/
--rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     5576 2023-06-07 12:14:05.351000 zpenv-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-06-07 09:51:42.000000 zpenv-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 12:14:05.392000 zpenv-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 12:14:04.836000 zpenv-1.2.1/zpenv/
--rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.2.1/zpenv/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.2.1/zpenv/__main__.py
--rw-rw-rw-   0        0        0    31764 2023-06-07 12:12:23.000000 zpenv-1.2.1/zpenv/zpenv.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:14:05.284000 zpenv-1.2.1/zpenv.egg-info/
--rw-rw-rw-   0        0        0     5576 2023-06-07 12:14:02.000000 zpenv-1.2.1/zpenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-07 12:14:04.000000 zpenv-1.2.1/zpenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 12:14:02.000000 zpenv-1.2.1/zpenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-07 12:14:03.000000 zpenv-1.2.1/zpenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-07 12:14:03.000000 zpenv-1.2.1/zpenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 12:14:03.000000 zpenv-1.2.1/zpenv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 13:25:59.402000 zpenv-1.3.0/
+-rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5576 2023-06-07 13:25:59.373000 zpenv-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-06-07 09:51:42.000000 zpenv-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 13:25:59.394000 zpenv-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 13:25:58.944000 zpenv-1.3.0/zpenv/
+-rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.3.0/zpenv/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.3.0/zpenv/__main__.py
+-rw-rw-rw-   0        0        0    33328 2023-06-07 13:24:08.000000 zpenv-1.3.0/zpenv/zpenv.py
+drwxrwxrwx   0        0        0        0 2023-06-07 13:25:59.295000 zpenv-1.3.0/zpenv.egg-info/
+-rw-rw-rw-   0        0        0     5576 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-07 13:25:58.000000 zpenv-1.3.0/zpenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-07 13:25:57.000000 zpenv-1.3.0/zpenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 13:25:58.000000 zpenv-1.3.0/zpenv.egg-info/top_level.txt
```

### Comparing `zpenv-1.2.1/LICENSE` & `zpenv-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpenv-1.2.1/PKG-INFO` & `zpenv-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.2.1
+Version: 1.3.0
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
```

### Comparing `zpenv-1.2.1/README.md` & `zpenv-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zpenv-1.2.1/zpenv/zpenv.py` & `zpenv-1.3.0/zpenv/zpenv.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,51 +169,86 @@
 		print_log(lang([f"Module {namemodule} déjà installé",f"Module {namemodule} already installed"]))
 		return
 	
 	cmd = [binpath, '-m', 'pip', 'install', namemodule]
 	if proxy!=None:
 		cmd.append('--proxy='+proxy)
 	proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-	stdout, stderr = proc.communicate()
-	if len(stdout)!=0:
-		print_log(lang([f"Module {namemodule} installé",f"Module {namemodule} installed"]))
-	else:
-		print_log(lang([f"ERREUR: Module {namemodule} non installé\nMessage d'erreur: {stderr.decode()}",f"ERROR: Module {namemodule} not installed\nError message: {stderr.decode()}"]))
+	while True:
+		output = proc.stdout.readline().decode("utf-8").strip()
+		if output == "":
+			break
+		print_log(output)
+
+	d_error = False
+	#Pour éviter les erreurs sur un pip pas à jour
+	if "A new release of pip available" not in proc.stderr.read().decode("utf-8").strip():
+		proc.stderr.seek(0)
+		for output in proc.stderr.readlines():
+			if len(output)>0 and d_error==False:
+				logs(f"ERREUR: Module {namemodule} non installé\nMessage d'erreur: {output.decode()}", "error")
+				d_error=True
+
+			print_log(output.decode("utf-8").strip(), "error")
 
 #Suppression d'un module dans un environnement
 def remove_module(binpath,namemodule):
 	if not get_package(binpath, namemodule):
 		print_log(lang([f"Module {namemodule} non installé",f"Module {namemodule} not installed"]))
 		return
 	
 	cmd = [binpath, '-m', 'pip', 'uninstall', '-y', namemodule]
 	proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-	stdout, stderr = proc.communicate()
-	if len(stdout)!=0:
-		print_log(lang([f"Module {namemodule} supprimé",f"Module {namemodule} deleted"]))
-	else:
-		print_log(lang([f"ERREUR: Module {namemodule} non supprimé\nMessage d'erreur: {stderr.decode()}",f"ERROR: Module {namemodule} not deleted\nError message: {stderr.decode()}"]))
+	while True:
+		output = proc.stdout.readline().decode("utf-8").strip()
+		if output == "":
+			break
+
+		print_log(output)
+
+	d_error = False
+
+	proc.stderr.seek(0)
+	for output in proc.stderr.readlines():
+		if len(output)>0 and d_error==False:
+			print_log(lang([f"ERREUR: Module {namemodule} non supprimé\nMessage d'erreur: {stderr.decode()}",f"ERROR: Module {namemodule} not deleted\nError message: {stderr.decode()}"]))
+			d_error=True
+
+		print_log(output.decode("utf-8").strip(), "error")
+
 	
 	
 #Upgrade d'un module dans un environnement
 def upgrade_module(binpath,namemodule,proxy):
 	if not get_package(binpath, namemodule):
 		print_log(lang([f"Module {namemodule} non installé",f"Module {namemodule} not installed"]))
 		return
 
 	cmd = [binpath, '-m', 'pip', 'install', namemodule, '--upgrade']
 	if proxy!=None:
 		cmd.append('--proxy='+proxy)
 
 	proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-	stdout, stderr = proc.communicate()
-	if len(stdout)!=0:
-		print_log(lang([f"Module {namemodule} mis à jour",f"Module {namemodule} updated"]))
-	else:
-		print_log(lang([f"ERREUR: Module {namemodule} non mis à jour\nMessage d'erreur: {stderr.decode()}",f"ERROR: Module {namemodule} not updated\nError message: {stderr.decode()}"]))
+	while True:
+		output = proc.stdout.readline().decode("utf-8").strip()
+		if output == "":
+			break
+
+		print_log(output)
+
+	d_error = False
+	#Pour éviter les erreurs sur un pip pas à jour
+	if "A new release of pip available" not in proc.stderr.read().decode("utf-8").strip():
+		proc.stderr.seek(0)
+		for output in proc.stderr.readlines():
+			if len(output)>0 and d_error==False:
+				print_log(lang([f"ERREUR: Module {namemodule} non mis à jour\nMessage d'erreur: {stderr.decode()}",f"ERROR: Module {namemodule} not updated\nError message: {stderr.decode()}"]))
+				d_error=True
+
+			print_log(output.decode("utf-8").strip(), "error")
 
 
 def main():
 	parse = zpp_args.parser()
 	parse.set_description(lang(["Gestionnaire d'environnement virtuel","Virtual environment manager"]))
 	parse.set_argument(longname="install", description=lang(["Installer l'environnement","Install environment"]), default=False)
 	parse.set_argument(longname="remove", description=lang(["Supprimer un environnement","Remove environment"]), default=False)
@@ -234,14 +269,15 @@
 
 	parse.set_argument("n", longname="name", description=lang(["Nom de l'environnement","Environment name"]), store="value", default=None, category="Install")
 	parse.set_argument("S", longname="sitepackages", description=lang(["Accorde l'accès au system site-packages dir","Grant access to the system site-packages dir"]), default=False, category="Install")
 	if os.name != 'nt':
 		parse.set_argument("s", longname="symlinks", description=lang(["Tenter d'utiliser un symlink","Attempt to use a symlink"]), default=False, category="Install")
 	parse.set_argument("C", longname="clear", description=lang(["Nettoyer le dossier de l'environnement","Clear environment folder"]), default=False, category="Install")
 	parse.set_argument(longname="upgradepython", description=lang(["Mettre à jour la version de python","Upgrade Python version"]), default=False, category="Install/Management")
+	parse.set_argument(longname="installpip", description=lang(["Installer pip","Install pip"]), default=None, category="Install/Management")
 	parse.set_argument("U", longname="upgradepip", description=lang(["Mettre à jour pip pendant l'installation","Upgrade pip during installation"]), default=False, category="Install")
 	parse.set_argument("p", longname="nopip", description=lang(["Ne pas installer pip","Do not install pip"]), default=False, category="Install")
 	parse.set_argument(longname="prompt", description=lang(["Spécifier le message du prompt","Specify prompt message"]), store="value", default=None, category="Install")
 	parse.set_argument("t", longname="tag", description=lang(["Ajouter/Lister des tags","Add/List tags"]), store="value", default=None, category="Install/Management")
 	parse.set_argument("c", longname="comment", description=lang(["Ajouter un commentaire","Add a comment"]), store="value", default=None, category="Install/Management")
 	parse.set_argument("D", longname="projectfolder", description=lang(["Spécifier un dossier de projet","Specify a project folder"]), store="value", default=None, category="Install/Management")
 	parse.set_argument(longname="removecomment", description=lang(["Supprimer un commentaire","Remove a comment"]), default=None, category="Install/Management")
@@ -447,18 +483,18 @@
 						OSType = get_os()
 						if OSType=='cmd':
 							activate_file='activate.bat'
 							if os.path.exists(envc['bin_path']+path_rep[0]+activate_file):
 								cmd = ['cmd', '/k']
 								target = ""
 								### Add alias CMD
-								if 'projectfolder' in envc and len(envc['projectfolder']):
+								if 'projectfolder' in envc:
 									target+=f"doskey cdproject=cd {envc['projectfolder']} & "
 								else:
-									target+=f"doskey cdproject=echo '"+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+"'' & "
+									target+=f"doskey cdproject=echo "+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+" & "
 								target+=f"doskey cdenv=cd {envc['env_dir']} & "
 								target+=f"doskey shellenv={envc['env_exe']} & "
 								target+=f"doskey zpenv={sys.executable} -m zpenv $* & "
 								target+=f'doskey help=echo "'+lang(["cdenv      se déplacer dans le dossier de l\'environnement`ncdproject  se déplacer dans le dossier du projet`nshellenv   accéder au shell python`nzpenv      accéder à zpenv","cdenv      move to environment folder`ncdproject  move to project folder`nshellenv   access python shell`nzpenv      access zpenv"])+'" & '
 								### END Add alias
 								target+="pushd "+envc['bin_path']+" & "+activate_file+" & popd"
 								cmd.append(target)
@@ -468,18 +504,18 @@
 
 						elif OSType=='powershell.exe' or os.name=='nt':
 							activate_file='activate.ps1'
 							if os.path.exists(envc['bin_path']+path_rep[0]+activate_file):
 								cmd = ['powershell', '-NoExit', '-Command']
 								target = ""
 								### Add alias PS1
-								if 'projectfolder' in envc and len(envc['projectfolder']):
+								if 'projectfolder' in envc:
 									target+='function cdproject{cd "'+envc['projectfolder']+'"}; '
 								else:
-									target+='function cdproject{Write-Host "'+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+'"}; '
+									target+='function cdproject{Write-Host '+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+'}; '
 								target+='function cdenv{cd "'+envc['env_dir']+'"}; '
 								target+='function shellenv{'+envc['env_exe']+'}; '
 								target+='function zpenv{'+sys.executable+' -m zpenv}; '
 								target+='function help{Write-Host "'+lang(["cdenv      se déplacer dans le dossier de l\'environnement`ncdproject  se déplacer dans le dossier du projet`nshellenv   accéder au shell python`nzpenv      accéder à zpenv","cdenv      move to environment folder`ncdproject  move to project folder`nshellenv   access python shell`nzpenv      access zpenv"])+'"}; '
 								### END Add alias
 								target+='. "'+envc['bin_path']+path_rep[0]+activate_file+'"'
 								cmd.append(target)
@@ -489,15 +525,15 @@
 						
 						else:
 							activate_file='activate'
 							if os.path.exists(envc['bin_path']+path_rep[0]+activate_file):
 								cmd = []
 								target = ""
 								### Add alias Linux
-								if 'projectfolder' in envc and len(envc['projectfolder']):
+								if 'projectfolder' in envc:
 									target+=f"alias cdproject=\'cd {envc['projectfolder']}\' && "
 								else:
 									target+="alias cdproject=\'echo "+lang(["Le dossier de projet n'est pas configuré","Project Folder not configure"])+"\' && "
 								target+=f"alias cdenv='cd {envc['env_dir']}' && "
 								target+=f"alias shellenv='{envc['env_exe']}' && "
 								target+=f"alias zpenv='{sys.executable} -m zpenv $*' && "
 								target+=f'alias help=\'echo -e "'+lang(["cdenv      se déplacer dans le dossier de l\'environnement\ncdproject  se déplacer dans le dossier du projet\nshellenv   accéder au shell python\nzpenv      accéder à zpenv","cdenv      move to environment folder\ncdproject  move to project folder\nshellenv   access python shell\nzpenv      access zpenv"])+'"\' && '
@@ -653,8 +689,24 @@
 				print_log(lang([f"Environnement {paramenv}", f"Environment {paramenv}"]))
 				envc = load_venv(paramenv)
 				if envc!=False and envc!=None:
 					tag = envc['tag'].split(",")
 					tag.remove(argument.removetag)
 					edit_venv(paramenv,"tag",",".join(tag))
 				if envc==False:
-					print_log(lang([f"L'environnement {paramenv} n'existe pas", f"Environment {paramenv} doesn't exist"]))
+					print_log(lang([f"L'environnement {paramenv} n'existe pas", f"Environment {paramenv} doesn't exist"]))
+		
+		elif argument.installpip:
+			for paramenv in parameter[0].split(","):
+				print_log(lang([f"Environnement {paramenv}", f"Environment {paramenv}"]))
+				envc = load_venv(paramenv)
+				if envc!=False and envc!=None:
+					print_log(lang([f"Installation de pip", f"Install pip"]))
+					cmd = [envc['env_exe'], '-m', 'ensurepip']
+					if argument.proxy!=None:
+						cmd.append('--proxy='+argument.proxy)
+					proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+					stdout, stderr = proc.communicate()
+					if len(stdout)!=0:
+						print_log(lang([f"Pip installé",f"Pip installed"]))
+					else:
+						print_log(lang([f"ERREUR: Pip non installé\nMessage d'erreur: {stderr.decode()}",f"ERROR: Pip not installed\nError message: {stderr.decode()}"]))
```

### Comparing `zpenv-1.2.1/zpenv.egg-info/PKG-INFO` & `zpenv-1.3.0/zpenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.2.1
+Version: 1.3.0
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
```

