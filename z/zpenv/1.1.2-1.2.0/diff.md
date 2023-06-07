# Comparing `tmp/zpenv-1.1.2.tar.gz` & `tmp/zpenv-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpenv-1.1.2.tar", last modified: Tue Jun  6 21:02:08 2023, max compression
+gzip compressed data, was "zpenv-1.2.0.tar", last modified: Wed Jun  7 09:37:46 2023, max compression
```

## Comparing `zpenv-1.1.2.tar` & `zpenv-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 21:02:08.737000 zpenv-1.1.2/
--rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     5522 2023-06-06 21:02:08.733000 zpenv-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4917 2022-12-26 19:01:11.000000 zpenv-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 21:02:08.736000 zpenv-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 21:02:08.688000 zpenv-1.1.2/zpenv/
--rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.1.2/zpenv/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.1.2/zpenv/__main__.py
--rw-rw-rw-   0        0        0    31382 2023-06-06 20:40:58.000000 zpenv-1.1.2/zpenv/zpenv.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:02:08.727000 zpenv-1.1.2/zpenv.egg-info/
--rw-rw-rw-   0        0        0     5522 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 21:02:08.000000 zpenv-1.1.2/zpenv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 09:37:46.316000 zpenv-1.2.0/
+-rw-rw-rw-   0        0        0     1106 2023-06-06 20:57:27.000000 zpenv-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5522 2023-06-07 09:37:46.312000 zpenv-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4917 2022-12-26 19:01:11.000000 zpenv-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 09:37:46.315000 zpenv-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 09:37:46.264000 zpenv-1.2.0/zpenv/
+-rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.2.0/zpenv/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.2.0/zpenv/__main__.py
+-rw-rw-rw-   0        0        0    31666 2023-06-07 09:35:55.000000 zpenv-1.2.0/zpenv/zpenv.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:37:46.306000 zpenv-1.2.0/zpenv.egg-info/
+-rw-rw-rw-   0        0        0     5522 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-07 09:37:46.000000 zpenv-1.2.0/zpenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-07 09:37:45.000000 zpenv-1.2.0/zpenv.egg-info/top_level.txt
```

### Comparing `zpenv-1.1.2/LICENSE` & `zpenv-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zpenv-1.1.2/PKG-INFO` & `zpenv-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.1.2
+Version: 1.2.0
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
```

### Comparing `zpenv-1.1.2/README.md` & `zpenv-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zpenv-1.1.2/zpenv/zpenv.py` & `zpenv-1.2.0/zpenv/zpenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,25 @@
 	if local=="fr_FR":
 		return data[0]
 	else:
 		return data[1]
 
 #Création du context
 class Context:
-	def __init__(self, virtdir, virtname = None):
+	def __init__(self, virtdir, virtname=None, prompt=None):
 		self.env_dir = virtdir
 		if virtname==None:
 			name = virtdir.split(path_rep[0])
 			self.env_name = name[len(name)-1]
 		else:
 			self.env_name = virtname
-		self.prompt = f'({self.env_name}) '
+		if prompt!=None:
+			self.prompt = f'({prompt}) '
+		else:
+			self.prompt = f'({self.env_name}) '
 		self.executable = sys.executable
 		self.python_dir = os.path.dirname(sys.executable)
 		self.python_exe = sys.executable.replace(self.python_dir,"").replace(path_rep[0],"")
 		self.inc_path = virtdir + path_rep[0] +'Include'
 		self.lib_path = virtdir + path_rep[0] +'Lib'
 		self.bin_path = virtdir + path_rep[0] +'Scripts'
 		self.bin_name = 'Scripts'
@@ -233,14 +236,15 @@
 	parse.set_argument("S", longname="sitepackages", description=lang(["Accorde l'accès au system site-packages dir","Grant access to the system site-packages dir"]), default=False, category="Install")
 	if os.name != 'nt':
 		parse.set_argument("s", longname="symlinks", description=lang(["Tenter d'utiliser un symlink","Attempt to use a symlink"]), default=False, category="Install")
 	parse.set_argument("C", longname="clear", description=lang(["Nettoyer le dossier de l'environnement","Clear environment folder"]), default=False, category="Install")
 	parse.set_argument(longname="upgradepython", description=lang(["Mettre à jour la version de python","Upgrade Python version"]), default=False, category="Install/Management")
 	parse.set_argument("U", longname="upgradepip", description=lang(["Mettre à jour pip pendant l'installation","Upgrade pip during installation"]), default=False, category="Install")
 	parse.set_argument("p", longname="nopip", description=lang(["Ne pas installer pip","Do not install pip"]), default=False, category="Install")
+	parse.set_argument(longname="prompt", description=lang(["Spécifier le message du prompt","Specify prompt message"]), store="value", default=None, category="Install")
 	parse.set_argument("t", longname="tag", description=lang(["Ajouter/Lister des tags","Add/List tags"]), store="value", default=None, category="Install/Management")
 	parse.set_argument("c", longname="comment", description=lang(["Ajouter un commentaire","Add a comment"]), store="value", default=None, category="Install/Management")
 	parse.set_argument("D", longname="projectfolder", description=lang(["Spécifier un dossier de projet","Specify a project folder"]), store="value", default=None, category="Install/Management")
 	parse.set_argument(longname="removecomment", description=lang(["Supprimer un commentaire","Remove a comment"]), default=None, category="Install/Management")
 	parse.set_argument(longname="removetag", description=lang(["Supprimer un tag","Remove a tag"]), store="value", default=None, category="Install/Management")
 
 	parse.set_argument(longname="nopurge", description=lang(["Ne supprime pas le dossier de l'environnement","Does not delete environment folder"]), default=False, category="Remove")
@@ -262,15 +266,15 @@
 			argument.configfile = os.path.split(__file__)[0] + path_rep[0] + 'zpenv.cfg'
 
 		if argument.install:
 			for paramenv in parameter[0].split(","):
 				print_log(lang([f"Environnement {paramenv}", f"Environment {paramenv}"]))
 				print_log(lang(["Création du contexte","Create context"]))
 				virtdir = path_reg(paramenv)
-				context = Context(virtdir, argument.name)
+				context = Context(virtdir, argument.name, argument.prompt)
 
 				envc = load_venv(context.env_name)
 				if envc==False:
 					if os.path.exists(virtdir) and os.path.isdir(virtdir) and len(os.listdir(virtdir))!=0:
 						ch = input(lang(["Le dossier n'est pas vide. Nettoyer ? (y/N)","Folder is not empty. Clear ? (y/N)"]))
 						if ch=="y":
 							argument.clear=True
@@ -283,15 +287,15 @@
 					if argument.clear and argument.upgradepython:
 						print_log(lang(['vous ne pouvez pas fournir --upgrade et --clear ensemble','you cannot supply --upgrade and --clear together']))
 					
 					if argument.nopip and argument.installmodule!=None:
 						print_log(lang(['vous ne pouvez pas fournir --nopip et --installmodule ensemble','you cannot supply --nopip and --installmodule together']))
 					
 					print_log(lang(["Init builder","Init builder"]))
-					virtual = venv.EnvBuilder(system_site_packages=argument.sitepackages, clear=argument.clear, symlinks=argument.symlinks, upgrade=argument.upgradepython, upgrade_deps=argument.upgradepip)
+					virtual = venv.EnvBuilder(system_site_packages=argument.sitepackages, clear=argument.clear, symlinks=argument.symlinks, upgrade=argument.upgradepython, upgrade_deps=argument.upgradepip, prompt=argument.prompt)
 					
 					print_log(lang(["Création du dossier de l'environnement","Create environment directory"]))
 					virtual.ensure_directories(virtdir)
 					if not os.path.exists(context.inc_path) or not os.path.exists(context.bin_path) or not os.path.exists(context.lib_path):
 						print_log(lang(["ERREUR: Le dossier de l'environnement n'a pas été créé","ERROR: Environent directory not created"]))
 						sys.exit()
```

### Comparing `zpenv-1.1.2/zpenv.egg-info/PKG-INFO` & `zpenv-1.2.0/zpenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpenv
-Version: 1.1.2
+Version: 1.2.0
 Summary: Gestionnaire d'environnement virtuel
 Home-page: https://github.com/ZephyrOff/py-zpenv
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpenv
 Keywords: venv virtualenv terminal zephyroff
 Platform: ALL
```

