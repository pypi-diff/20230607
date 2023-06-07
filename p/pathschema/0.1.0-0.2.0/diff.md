# Comparing `tmp/pathschema-0.1.0.tar.gz` & `tmp/pathschema-0.2.0.tar.gz`

## Comparing `pathschema-0.1.0.tar` & `pathschema-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pathschema-0.1.0/.pylintrc
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pathschema-0.1.0/requirements.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathschema-0.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pathschema-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pathschema-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pathschema-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/__main__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/exceptions.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/models.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/parser.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/utils.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pathschema-0.1.0/pathschema/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_DirPathNode.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_FilePathNode.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_Parser.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_PathNode.py
--rw-r--r--   0        0        0    14023 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/test_Validator.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/.gitignore
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/generate_massive.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_invalid_schema.txt
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_schema.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/CommunityAssets/sdfasdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Globals/Materials/brick.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Globals/Materials/water.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Globals/Textures/robot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Notes.md/this should not be evaluated
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/not_allowed.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Materials/solid_metal.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Textures/body.jpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Scenes/test.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_fail/Assets/Scenes/level1/first.unity
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Notes.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/CommunityAssets/sdfasdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Globals/Materials/solid_brick.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Globals/Materials/trans_water.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Globals/Textures/robot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/model.fbx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/solid_material.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/texture.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Materials/solid_metal.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Textures/body.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.1.0/tests/experimentations/test_directory_ok/Assets/Scenes/level1/first.unity
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pathschema-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pathschema-0.1.0/LICENSE
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pathschema-0.1.0/README.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pathschema-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 pathschema-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pathschema-0.2.0/.pylintrc
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pathschema-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pathschema-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pathschema-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pathschema-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pathschema-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/__main__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/exceptions.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/models.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/parser.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/utils.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pathschema-0.2.0/pathschema/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/test_DirPathNode.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/test_FilePathNode.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/test_Parser.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/test_PathNode.py
+-rw-r--r--   0        0        0    14023 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/test_Validator.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/.gitignore
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/generate_massive.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_invalid_schema.txt
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_schema.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/CommunityAssets/sdfasdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Globals/Materials/brick.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Globals/Materials/water.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Globals/Textures/robot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Notes.md/this should not be evaluated
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/not_allowed.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Materials/solid_metal.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Prefabs/Robot/Textures/body.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Scenes/test.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_fail/Assets/Scenes/level1/first.unity
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Notes.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/CommunityAssets/sdfasdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Globals/Materials/solid_brick.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Globals/Materials/trans_water.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Globals/Textures/robot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/model.fbx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/solid_material.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Planet/texture.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Materials/solid_metal.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Prefabs/Robot/Textures/body.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathschema-0.2.0/tests/experimentations/test_directory_ok/Assets/Scenes/level1/first.unity
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pathschema-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pathschema-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 pathschema-0.2.0/README.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pathschema-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pathschema-0.2.0/PKG-INFO
```

### Comparing `pathschema-0.1.0/.github/workflows/build.yml` & `pathschema-0.2.0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
   buildAndTest:
     name: Build And Test
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: ['3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11']
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         name: Set up Python ${{ matrix.python-version }}
         with:
```

### Comparing `pathschema-0.1.0/.github/workflows/publish.yml` & `pathschema-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/pathschema/__main__.py` & `pathschema-0.2.0/pathschema/__main__.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/pathschema/models.py` & `pathschema-0.2.0/pathschema/models.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/pathschema/parser.py` & `pathschema-0.2.0/pathschema/parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,36 +12,72 @@
 	indentation_token = '\t'
 	directory_token = '/'
 	required_token = '+'
 	forbidden_token = '-'
 	any_token = '...'
 	comment_token = '#'
 
-	def _detect_indentation(self):
-		raise NotImplementedError()
+	def _detect_indentation(self, schema: str) -> str:
+		for line in schema.split('\n'):
 
-	def _indentation_count(self,  string: str):
-		num_of_indentation = 0
-		for character in string:
-			if character == self.indentation_token:
-				num_of_indentation += 1
-			else:
-				break
+			# ignore empty lines
+			if not line.strip():
+				continue
+			
+			leading_whitespace = len(line) - len(line.lstrip())
 
-		return num_of_indentation
+			# impossible to evaluate if no leading whitespace, continue to next line
+			if leading_whitespace == 0:
+				continue
+			
+			# indentation is tabs
+			if line.startswith('\t'):
+				return '\t' * leading_whitespace
+			
+			# indentation is spaces
+			if line.startswith(' '):
+				return ' ' * leading_whitespace
+		
+		# if not evaluated, assume default
+		return self.indentation_token
+
+	def _indentation_count(self,  string: str, line_num: int) -> int:
+		"""Counts the indentation at the beginning of a string using the indentation token"""
+		tmp_str = string
+		count = 0
+		
+		while tmp_str.startswith(self.indentation_token):
+			count += 1
+			tmp_str = tmp_str[len(self.indentation_token):]
+
+		# if there is still some whitespace
+		# can happen if indentation token is 4 space and there are 3 spaces instead
+		if len(tmp_str) > len(tmp_str.lstrip()):
+			raise SchemaError('Inconsistent indentation.', line_num)
+		
+		return count
 
 	def schema_to_node_tree(self, schema: str) -> DirPathNode:
 
+		self.indentation_token = self._detect_indentation(schema)
+
 		root_node: DirPathNode = DirPathNode(name='schema_root')
 
 		current_node = root_node
 		node_depth = 0
+		last_indentation = 0
 
 		for line_num, line in enumerate(schema.split('\n')):
-			indentation = self._indentation_count(line)
+			indentation = self._indentation_count(line, line_num+1)
+
+			if indentation > last_indentation + 1:
+				raise SchemaError('Inconsistent indentation.', line_num+1)
+
+			last_indentation = indentation
+			
 			name = line.strip()
 			if len(name) == 0:
 				continue
 
 			# comments get ignored
 			if name.startswith(self.comment_token):
 				continue
```

### Comparing `pathschema-0.1.0/pathschema/utils.py` & `pathschema-0.2.0/pathschema/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 	childs = node.childs
 	if sort:
 		childs = sorted(childs, key=lambda x: x.name)
 
 	for i, child in enumerate(childs):
 
 		color = Fore.RESET
-		match(child.necessity):
-			case Necessity.REQUIRED:
-				color = Fore.RED + Style.BRIGHT
-			case Necessity.FORBIDDEN:
-				color = Fore.GREEN + Style.BRIGHT
+
+		if child.necessity == Necessity.REQUIRED:
+			color = Fore.RED + Style.BRIGHT
+		elif child.necessity == Necessity.FORBIDDEN:
+			color = Fore.GREEN + Style.BRIGHT
 
 		if i == len(childs) - 1:
 
 			if isinstance(child, DirPathNode):
 				print(f'{prefix}╰── 📁 {color}{child.name}/{Style.RESET_ALL}')
 				print_node_tree(child, sort, prefix + "    ")
 				continue
```

### Comparing `pathschema-0.1.0/pathschema/validator.py` & `pathschema-0.2.0/pathschema/validator.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/tests/test_DirPathNode.py` & `pathschema-0.2.0/tests/test_DirPathNode.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/tests/test_PathNode.py` & `pathschema-0.2.0/tests/test_PathNode.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/tests/test_Validator.py` & `pathschema-0.2.0/tests/test_Validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,23 +71,23 @@
 		os.makedirs(dir_to_validate.joinpath('should_fail'))
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_dir_only_simple_pass(self):
 		schema =  'Assets/\n'
-		schema += '\tGlobals/\n'
-		schema += '\t\tMaterials/\n'
-		schema += '\t\tTextures/\n'
-		schema += '\t\tModels/\n'
-		schema += '\t\tScripts/\n'
-		schema += '\t\tAnimations/\n'
-		schema += '\tPrefabs/\n'
-		schema += '\tCommunityAssets/\n'
-		schema += '\tScenes/\n'
+		schema += '  Globals/\n'
+		schema += '    Materials/\n'
+		schema += '    Textures/\n'
+		schema += '    Models/\n'
+		schema += '    Scripts/\n'
+		schema += '    Animations/\n'
+		schema += '  Prefabs/\n'
+		schema += '  CommunityAssets/\n'
+		schema += '  Scenes/\n'
 
 		dir_to_validate = self._temp_dir()
 
 		os.makedirs(dir_to_validate / 'Assets')
 		os.makedirs(dir_to_validate / 'Assets' / 'Globals')
 		os.makedirs(dir_to_validate / 'Assets' / 'Globals' / 'Materials')
 		os.makedirs(dir_to_validate / 'Assets' / 'Globals' / 'Textures')
@@ -99,23 +99,23 @@
 		os.makedirs(dir_to_validate / 'Assets' / 'Scenes')
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_dir_only_simple_fail(self):
 		schema =  'Assets/\n'
-		schema += '\tGlobals/\n'
-		schema += '\t\tMaterials/\n'
-		schema += '\t\tTextures/\n'
-		schema += '\t\tModels/\n'
-		schema += '\t\tScripts/\n'
-		schema += '\t\tAnimations/\n'
-		schema += '\tPrefabs/\n'
-		schema += '\tCommunityAssets/\n'
-		schema += '\tScenes/\n'
+		schema += '  Globals/\n'
+		schema += '    Materials/\n'
+		schema += '    Textures/\n'
+		schema += '    Models/\n'
+		schema += '    Scripts/\n'
+		schema += '    Animations/\n'
+		schema += '  Prefabs/\n'
+		schema += '  CommunityAssets/\n'
+		schema += '  Scenes/\n'
 
 		dir_to_validate = self._temp_dir()
 
 		os.makedirs(dir_to_validate / 'Assets')
 		os.makedirs(dir_to_validate / 'Assets' / 'Globals')
 		os.makedirs(dir_to_validate / 'Assets' / 'Globals' / 'Wrong')
 		os.makedirs(dir_to_validate / 'Assets' / 'Globals' / 'Textures')
@@ -127,17 +127,17 @@
 		os.makedirs(dir_to_validate / 'Assets' / 'Scenes')
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_dir_and_files_simple_pass(self):
 		schema =  'Textures/\n'
-		schema += '\trobot.png\n'
+		schema += '  robot.png\n'
 		schema += 'Models/\n'
-		schema += '\trobot.fbx\n'
+		schema += '  robot.fbx\n'
 
 		dir_to_validate = self._temp_dir()
 
 		texture_dir = dir_to_validate.joinpath('Textures')
 		os.makedirs(texture_dir)
 		(texture_dir / 'robot.png').touch()
 
@@ -146,17 +146,17 @@
 		(models_dir / 'robot.fbx').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_dir_and_files_simple_fail(self):
 		schema =  'Textures/\n'
-		schema += '\trobot.png\n'
+		schema += '  robot.png\n'
 		schema += 'Models/\n'
-		schema += '\trobot.fbx\n'
+		schema += '  robot.fbx\n'
 
 		dir_to_validate = self._temp_dir()
 
 		texture_dir = dir_to_validate.joinpath('Textures')
 		os.makedirs(texture_dir)
 		(texture_dir / 'robot.png').touch()
 
@@ -167,94 +167,94 @@
 		os.makedirs(texture_dir / 'invalid_dir')
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_star_file_pass(self):
 		schema =  'Notes/\n'
-		schema += '\t*\n'
+		schema += '  *\n'
 
 		dir_to_validate = self._temp_dir()
 
 		note_dir = dir_to_validate.joinpath('Notes')
 		os.makedirs(note_dir)
 		(note_dir / 'robot.md').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_regex_file_pass(self):
 		schema =  'Notes/\n'
-		schema += '\t".*\\.md"\n'
+		schema += '  ".*\\.md"\n'
 
 		dir_to_validate = self._temp_dir()
 
 		note_dir = dir_to_validate.joinpath('Notes')
 		os.makedirs(note_dir)
 		(note_dir / 'robot.md').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_regex_file_fail(self):
 		schema =  'Notes/\n'
-		schema += '\t".*\\.md"\n'
+		schema += '  ".*\\.md"\n'
 
 		dir_to_validate = self._temp_dir()
 
 		note_dir = dir_to_validate.joinpath('Notes')
 		os.makedirs(note_dir)
 		(note_dir / 'robot.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_star_dir_pass(self):
 		schema =  'Notes/\n'
-		schema += '\t*/\n'
+		schema += '  */\n'
 
 		dir_to_validate = self._temp_dir()
 
 		dirs = dir_to_validate.joinpath('Notes', 'Things')
 		os.makedirs(dirs)
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_regex_dir_pass(self):
 		schema =  'Notes/\n'
-		schema += '\t"\\d+"/\n'
+		schema += '  "\\d+"/\n'
 
 		dir_to_validate = self._temp_dir()
 
 		dirs = dir_to_validate.joinpath('Notes', '123456')
 		os.makedirs(dirs)
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_regex_dir_fail(self):
 		schema =  'Notes/\n'
-		schema += '\t"\\d"/\n'
+		schema += '  "\\d"/\n'
 
 		dir_to_validate = self._temp_dir()
 
 		dirs = dir_to_validate.joinpath('Notes', 'abcde')
 		os.makedirs(dirs)
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_star_and_dir_pass(self):
 		schema =  'Assets/\n'
-		schema += '\tTextures/\n'
-		schema += '\t\t".*\\.png"\n'
-		schema += '\tModels/\n'
-		schema += '\t\t".*\\.fbx"\n'
-		schema += '\t*\n'
+		schema += '  Textures/\n'
+		schema += '    ".*\\.png"\n'
+		schema += '  Models/\n'
+		schema += '    ".*\\.fbx"\n'
+		schema += '  *\n'
 
 		dir_to_validate = self._temp_dir()
 
 		assets_dir = dir_to_validate / 'Assets'
 		os.makedirs(assets_dir)
 		textures_dir = assets_dir / 'Textures'
 		os.makedirs(textures_dir)
@@ -265,19 +265,19 @@
 		(models_dir / 'robot.fbx').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_star_and_dir_fail(self):
 		schema =  'Assets/\n'
-		schema += '\tTextures/\n'
-		schema += '\t\t".*\\.png"\n'
-		schema += '\tModels/\n'
-		schema += '\t\t".*\\.fbx"\n'
-		schema += '\t*\n'
+		schema += '  Textures/\n'
+		schema += '    ".*\\.png"\n'
+		schema += '  Models/\n'
+		schema += '    ".*\\.fbx"\n'
+		schema += '  *\n'
 
 		dir_to_validate = self._temp_dir()
 
 		assets_dir = dir_to_validate / 'Assets'
 		os.makedirs(assets_dir)
 		textures_dir = assets_dir / 'Textures'
 		os.makedirs(textures_dir)
@@ -288,15 +288,15 @@
 		(models_dir / 'robot.obj').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_any_pass(self):
 		schema =  'Assets/\n'
-		schema += '\t...\n'
+		schema += '  ...\n'
 
 		dir_to_validate = self._temp_dir()
 
 		assets_dir = dir_to_validate / 'Assets'
 		os.makedirs(assets_dir)
 		textures_dir = assets_dir / 'Textures'
 		os.makedirs(textures_dir)
@@ -307,16 +307,16 @@
 		(models_dir / 'robot.fbx').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_pattern_star_pass(self):
 		schema =  'Assets/\n'
-		schema += '\tTextures/\n'
-		schema += '\t\t*.png\n'
+		schema += '  Textures/\n'
+		schema += '    *.png\n'
 
 		dir_to_validate = self._temp_dir()
 
 		assets_dir = dir_to_validate / 'Assets'
 		os.makedirs(assets_dir)
 		textures_dir = assets_dir / 'Textures'
 		os.makedirs(textures_dir)
@@ -325,16 +325,16 @@
 		(textures_dir / 'planet.png').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_pattern_star_fail(self):
 		schema =  'Assets/\n'
-		schema += '\tTextures/\n'
-		schema += '\t\t*.png\n'
+		schema += '  Textures/\n'
+		schema += '    *.png\n'
 
 		dir_to_validate = self._temp_dir()
 
 		assets_dir = dir_to_validate / 'Assets'
 		os.makedirs(assets_dir)
 		textures_dir = assets_dir / 'Textures'
 		os.makedirs(textures_dir)
@@ -343,15 +343,15 @@
 		(textures_dir / 'planet.jpeg').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_pattern_question_mark_pass(self):
 		schema =  'Folder/\n'
-		schema += '\tFile_?.txt\n'
+		schema += '  File_?.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'File_0.txt').touch()
@@ -362,134 +362,134 @@
 		(folder_dir / 'File_C.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_pattern_question_mark_fail(self):
 		schema =  'Folder/\n'
-		schema += '\tFile_?.txt\n'
+		schema += '  File_?.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'Fails_00.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_forbiden_pass(self):
 		schema =  'Folder/\n'
-		schema += '\t-File.txt\n'
-		schema += '\tAnAcceptableFile.txt\n'
+		schema += '  -File.txt\n'
+		schema += '  AnAcceptableFile.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'AnAcceptableFile.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_forbiden_fail(self):
 		schema =  'Folder/\n'
-		schema += '\t-File.txt\n'
+		schema += '  -File.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'File.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_forbiden_with_start_fail(self):
 		schema =  'Folder/\n'
-		schema += '\t-File.txt\n'
-		schema += '\t*.txt\n'
+		schema += '  -File.txt\n'
+		schema += '  *.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'File.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_forbiden_with_start2_fail(self):
 		schema =  'Folder/\n'
-		schema += '\t*.txt\n'
-		schema += '\t-File.txt\n'
+		schema += '  *.txt\n'
+		schema += '  -File.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'File.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_required_pass(self):
 		schema =  'Folder/\n'
-		schema += '\t+File.txt\n'
-		schema += '\tSomeOtherFile.txt\n'
+		schema += '  +File.txt\n'
+		schema += '  SomeOtherFile.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'File.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_no_errors(result)
 
 	def test_validate_required_fail(self):
 		schema =  'Folder/\n'
-		schema += '\t+File.txt\n'
-		schema += '\tSomeOtherFile.txt\n'
+		schema += '  +File.txt\n'
+		schema += '  SomeOtherFile.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'SomeOtherFile.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_required_with_start_fail(self):
 		schema =  'Folder/\n'
-		schema += '\t+File.txt\n'
-		schema += '\t*.txt\n'
+		schema += '  +File.txt\n'
+		schema += '  *.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'SomeOtherFile.txt').touch()
 
 		result = Validator().validate(dir_to_validate, schema)
 		self.assert_validation_result_has_errors(result)
 
 	def test_validate_required_with_start2_fail(self):
 		schema =  'Folder/\n'
-		schema += '\t*.txt\n'
-		schema += '\t+File.txt\n'
+		schema += '  *.txt\n'
+		schema += '  +File.txt\n'
 
 		dir_to_validate = self._temp_dir()
 
 		folder_dir = dir_to_validate / 'Folder'
 		os.makedirs(folder_dir)
 
 		(folder_dir / 'SomeOtherFile.txt').touch()
```

### Comparing `pathschema-0.1.0/tests/experimentations/generate_massive.py` & `pathschema-0.2.0/tests/experimentations/generate_massive.py`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/tests/experimentations/test_schema.txt` & `pathschema-0.2.0/tests/experimentations/test_schema.txt`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/.gitignore` & `pathschema-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/LICENSE` & `pathschema-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathschema-0.1.0/README.md` & `pathschema-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 | `""` | Quotes adds regex validation to the file name | `"file[0-9]{3}"` |
 | `""/` | Quotes with a slash adds regex validation to the folder name | `"folder[0-9]{3}"/` |
 | `*` | Unix style pattern matching for files | `*.txt` |
 | `*/` | Unix style pattern matching for folders | `log_*/` |
 | `...` | Allows any (and nested) files and folder | `...` |
 | `+` | A `+` at the start makes the file or folder required | `+required_file.txt` |
 | `-` | A `-` at the start makes the file or folder forbidden | `-forbidden_folder/` |
+| `#` | Write a comment | `# cool comment` |
 
 ## Command line
 
 pathschema can be used directly in the command line.
 
 ```bash
 python -m pathschema path/to/schema.txt path/to/dir/to/validate
```

### Comparing `pathschema-0.1.0/pyproject.toml` & `pathschema-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathschema"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Apollo-Roboto", email="Apollo_Roboto@outlook.com" },
 ]
 description  = "Standardize and plan out a file structure!"
 readme = "README.md"
 license = "MIT"
 keywords = ["Validation", "Schema", "File System", "File", "Directory", "Folder"]
 dependencies = [
 	"colorama==0.4.6",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
 	"Programming Language :: Python :: 3",
+	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
 	"Natural Language :: English",
 	"Typing :: Typed",
 	"Topic :: Software Development :: Libraries",
```

### Comparing `pathschema-0.1.0/PKG-INFO` & `pathschema-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: pathschema
-Version: 0.1.0
+Version: 0.2.0
 Summary: Standardize and plan out a file structure!
 Project-URL: Source, https://github.com/Apollo-Roboto/python-pathschema
 Author-email: Apollo-Roboto <Apollo_Roboto@outlook.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Directory,File,File System,Folder,Schema,Validation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: colorama==0.4.6
 Description-Content-Type: text/markdown
 
 # Path Schema
 
 ![PyPi Version](https://img.shields.io/pypi/v/pathschema.svg) ![PyPI Python Version](https://img.shields.io/pypi/pyversions/pathschema.svg?logo=python&logoColor=gold) ![License MIT](https://img.shields.io/pypi/l/pathschema)
 
@@ -56,14 +57,15 @@
 | `""` | Quotes adds regex validation to the file name | `"file[0-9]{3}"` |
 | `""/` | Quotes with a slash adds regex validation to the folder name | `"folder[0-9]{3}"/` |
 | `*` | Unix style pattern matching for files | `*.txt` |
 | `*/` | Unix style pattern matching for folders | `log_*/` |
 | `...` | Allows any (and nested) files and folder | `...` |
 | `+` | A `+` at the start makes the file or folder required | `+required_file.txt` |
 | `-` | A `-` at the start makes the file or folder forbidden | `-forbidden_folder/` |
+| `#` | Write a comment | `# cool comment` |
 
 ## Command line
 
 pathschema can be used directly in the command line.
 
 ```bash
 python -m pathschema path/to/schema.txt path/to/dir/to/validate
```

