# Comparing `tmp/cbers4asat-0.6.8.tar.gz` & `tmp/cbers4asat-0.6.9.tar.gz`

## Comparing `cbers4asat-0.6.8.tar` & `cbers4asat-0.6.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/.readthedocs.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/en-US_README.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/mkdocs.yml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/api_reference.md
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/examples.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/index.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/installation.md
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/quickstart.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/requirements.txt
--rw-r--r--   0        0        0    42275 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/img/collections.png
--rw-r--r--   0        0        0  2098371 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/img/pansharp.png
--rw-r--r--   0        0        0   947297 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/docs/img/rgbn_composite_true_color.png
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/__init__.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/cbers4asat.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/cbers4a/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/cbers4a/collection.py
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/cbers4a/item.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/cbers4a/itemCollection.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/cbers4a/search.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/tools/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/tools/geometry.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/tools/grid.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/src/cbers4asat/tools/image.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/LICENSE
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/README.md
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 cbers4asat-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/.readthedocs.yml
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/en-US_README.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/mkdocs.yml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/api_reference.md
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/examples.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/index.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/installation.md
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/quickstart.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/requirements.txt
+-rw-r--r--   0        0        0    42275 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/img/collections.png
+-rw-r--r--   0        0        0  2098371 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/img/pansharp.png
+-rw-r--r--   0        0        0   947297 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/docs/img/rgbn_composite_true_color.png
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/__init__.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/cbers4asat.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/cbers4a/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/cbers4a/collection.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/cbers4a/item.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/cbers4a/itemCollection.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/cbers4a/search.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/tools/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/tools/geometry.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/tools/grid.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/src/cbers4asat/tools/image.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/LICENSE
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/README.md
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 cbers4asat-0.6.9/PKG-INFO
```

### Comparing `cbers4asat-0.6.8/en-US_README.md` & `cbers4asat-0.6.9/en-US_README.md`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/docs/api_reference.md` & `cbers4asat-0.6.9/docs/api_reference.md`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/docs/examples.md` & `cbers4asat-0.6.9/docs/examples.md`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/docs/index.md` & `cbers4asat-0.6.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/docs/quickstart.md` & `cbers4asat-0.6.9/docs/quickstart.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 # A classe date é utilizada para padronizar o formato de data na biblioteca
 from datetime import date
 
 # Instanciando o objeto com o usuário cadastrado na plataforma
 api = Cbers4aAPI('seu.login@email.com')
 
 # Bouding Box escolhido
-bbox = [-63.92944335937501,
-        -8.819260401678381,
-        -63.79211425781251,
-        -8.722218306198739]
+#   O bounding box é formado por 4 coordenadas: [x_min, y_min, x_max, y_max],
+#   correspondendo respectivamente a: [oeste, sul, leste, norte].
+#   Sendo essa ordem um fator importante para o funcionamento da busca
+bbox = [-63.92944335937501, # Oeste
+        -8.819260401678381, # Sul
+        -63.79211425781251, # Leste
+        -8.722218306198739] # Norte
 
 # Intervalo de data para a busca
 data_inicial = date(2021, 8, 25)
 data_final = date(2021, 9, 25)
 
 # Fazer uma busca no catálogo e exibir resultados
 produtos = api.query(location=bbox,
```

### Comparing `cbers4asat-0.6.8/docs/img/collections.png` & `cbers4asat-0.6.9/docs/img/collections.png`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/docs/img/pansharp.png` & `cbers4asat-0.6.9/docs/img/pansharp.png`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/docs/img/rgbn_composite_true_color.png` & `cbers4asat-0.6.9/docs/img/rgbn_composite_true_color.png`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/src/cbers4asat/cbers4asat.py` & `cbers4asat-0.6.9/src/cbers4asat/cbers4asat.py`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/src/cbers4asat/cbers4a/collection.py` & `cbers4asat-0.6.9/src/cbers4asat/cbers4a/collection.py`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/src/cbers4asat/cbers4a/item.py` & `cbers4asat-0.6.9/src/cbers4asat/cbers4a/item.py`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/src/cbers4asat/cbers4a/itemCollection.py` & `cbers4asat-0.6.9/src/cbers4asat/cbers4a/itemCollection.py`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/src/cbers4asat/cbers4a/search.py` & `cbers4asat-0.6.9/src/cbers4asat/cbers4a/search.py`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/src/cbers4asat/tools/grid.py` & `cbers4asat-0.6.9/src/cbers4asat/tools/grid.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,19 +17,19 @@
         - grid_download("cbers4a", "mux")
         - grid_download(satellite="amazonia1", "wfi", outdir="./downloads")
     Returns:
         .zip file
     """
     grids = {
         "cbers4a": {
-            "mux": "http://www.dgi.inpe.br/documentacao/arquivos/grid_cbers4a_mux.zip/@@download/file/grid_cbers4a_mux.zip",
-            "wfi": "http://www.dgi.inpe.br/documentacao/arquivos/grid_cbers4a_wfi.zip/@@download/file/grid_cbers4a_wfi.zip",
+            "mux": "http://www.dgi.inpe.br/documentacao/arquivos/grid_cbers4a_mux.zip",
+            "wfi": "http://www.dgi.inpe.br/documentacao/arquivos/grid_cbers4a_wfi.zip",
         },
         "amazonia1": {
-            "wfi": "http://www.dgi.inpe.br/documentacao/arquivos/grid_amazonia1_wfi_sa.zip/@@download/file/grid_amazonia1_wfi_sa.zip"
+            "wfi": "http://www.dgi.inpe.br/documentacao/arquivos/grid_amazonia1_wfi_sa.zip"
         },
     }
 
     get_satellite = grids.get(satellite.lower(), None)
 
     if get_satellite:
         get_sensor = get_satellite.get(sensor.lower(), None)
```

### Comparing `cbers4asat-0.6.8/src/cbers4asat/tools/image.py` & `cbers4asat-0.6.9/src/cbers4asat/tools/image.py`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/LICENSE` & `cbers4asat-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cbers4asat-0.6.8/README.md` & `cbers4asat-0.6.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Cbers4asat
 
 ## Descrição
 
-Biblioteca Python para consultar o catálogo e realizar operações com dados do CBERS4A e AMAZONIA1.
+Biblioteca Python para realizar a busca e processamento de imagens dos satélites CBERS4A e AMAZONIA-1.
 
 A biblioteca `cbers4asat` surgiu da necessidade de automatizar a busca e manipulação de imagens do satélite
-sino-brasileiro CBERS-04A utilizando linguagens de programação.
+sino-brasileiro CBERS-04A utilizando linguagens de programação. Posteriormente foi incluido a automação do satélite AMAZONIA-1.
 
 O design do projeto foi inspirado no [sentinelsat](https://github.com/sentinelsat/sentinelsat), onde é possível de forma
 intuitiva, pesquisar por imagens e realizar o download com poucas linhas de código, além de poder ser integrado com
-outras bibiliotecas como o geopandas.
+outras bibiliotecas como o geopandas. 
 
 ---
 [![Latest Version](https://img.shields.io/pypi/v/cbers4asat?style=plastic)](https://pypi.python.org/pypi/cbers4asat/)
 [![Latest Version](https://img.shields.io/pypi/l/cbers4asat?style=plastic)](https://github.com/gabriel-russo/cbers4asat/blob/master/LICENSE)
 [![Latest Version](https://img.shields.io/pypi/pyversions/cbers4asat?style=plastic)](https://pypi.python.org/pypi/cbers4asat/)
 [![Latest Version](https://img.shields.io/pypi/dm/cbers4asat?style=plastic)](https://pypi.python.org/pypi/cbers4asat/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -32,15 +32,16 @@
 
 # Inicializando a biblioteca
 api = Cbers4aAPI('email@mail.com')
 
 # Área de interesse (bbox, path row ou polígono)
 path_row = (229, 124)
 
-# Buscando metadados
+# Buscando metadados. A localização é feita a partir do path_row (órbita/ponto). 
+# Consulte a órbita/ponto: http://www.dgi.inpe.br/documentacao/grades
 produtos = api.query(location=path_row,
                      initial_date=date(2021, 6, 1),
                      end_date=date(2021, 7, 1),
                      cloud=100,
                      limit=10,
                      collections=['AMAZONIA1_WFI_L2_DN', 'CBERS4A_WPM_L4_DN'])
 
@@ -101,8 +102,8 @@
 
 Copyright (c) 2022 Gabriel Russo
 
 Copyright (c) 2020 Sandro Klippel
 
 O uso é fornecido sob a Licença do MIT. Veja
 em [LICENSE](https://github.com/gabriel-russo/cbers4asat/blob/master/LICENSE)
-para mais detalhes.
+para mais detalhes.
```

### Comparing `cbers4asat-0.6.8/pyproject.toml` & `cbers4asat-0.6.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cbers4asat"
-version = "0.6.8"
+version = "0.6.9"
 description = "Biblioteca Python para consultar o catálogo e realizar operações com dados do CBERS4A"
 authors = [
     { name = "Gabriel Russo", email = "gabrielrusso@protonmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["cbers", "cbers4a", "remote sensing", "geoprocessing"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cbers4asat-0.6.8/PKG-INFO` & `cbers4asat-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbers4asat
-Version: 0.6.8
+Version: 0.6.9
 Summary: Biblioteca Python para consultar o catálogo e realizar operações com dados do CBERS4A
 Project-URL: Homepage, https://github.com/gabriel-russo/cbers4asat
 Project-URL: Bug Tracker, https://github.com/gabriel-russo/cbers4asat/issues
 Project-URL: Repository, https://github.com/gabriel-russo/cbers4asat.git
 Author-email: Gabriel Russo <gabrielrusso@protonmail.com>
 License: MIT License
         
@@ -51,22 +51,22 @@
 Requires-Dist: scikit-image>=0.20.0; extra == 'tools'
 Description-Content-Type: text/markdown
 
 # Cbers4asat
 
 ## Descrição
 
-Biblioteca Python para consultar o catálogo e realizar operações com dados do CBERS4A e AMAZONIA1.
+Biblioteca Python para realizar a busca e processamento de imagens dos satélites CBERS4A e AMAZONIA-1.
 
 A biblioteca `cbers4asat` surgiu da necessidade de automatizar a busca e manipulação de imagens do satélite
-sino-brasileiro CBERS-04A utilizando linguagens de programação.
+sino-brasileiro CBERS-04A utilizando linguagens de programação. Posteriormente foi incluido a automação do satélite AMAZONIA-1.
 
 O design do projeto foi inspirado no [sentinelsat](https://github.com/sentinelsat/sentinelsat), onde é possível de forma
 intuitiva, pesquisar por imagens e realizar o download com poucas linhas de código, além de poder ser integrado com
-outras bibiliotecas como o geopandas.
+outras bibiliotecas como o geopandas. 
 
 ---
 [![Latest Version](https://img.shields.io/pypi/v/cbers4asat?style=plastic)](https://pypi.python.org/pypi/cbers4asat/)
 [![Latest Version](https://img.shields.io/pypi/l/cbers4asat?style=plastic)](https://github.com/gabriel-russo/cbers4asat/blob/master/LICENSE)
 [![Latest Version](https://img.shields.io/pypi/pyversions/cbers4asat?style=plastic)](https://pypi.python.org/pypi/cbers4asat/)
 [![Latest Version](https://img.shields.io/pypi/dm/cbers4asat?style=plastic)](https://pypi.python.org/pypi/cbers4asat/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -85,15 +85,16 @@
 
 # Inicializando a biblioteca
 api = Cbers4aAPI('email@mail.com')
 
 # Área de interesse (bbox, path row ou polígono)
 path_row = (229, 124)
 
-# Buscando metadados
+# Buscando metadados. A localização é feita a partir do path_row (órbita/ponto). 
+# Consulte a órbita/ponto: http://www.dgi.inpe.br/documentacao/grades
 produtos = api.query(location=path_row,
                      initial_date=date(2021, 6, 1),
                      end_date=date(2021, 7, 1),
                      cloud=100,
                      limit=10,
                      collections=['AMAZONIA1_WFI_L2_DN', 'CBERS4A_WPM_L4_DN'])
 
@@ -154,8 +155,8 @@
 
 Copyright (c) 2022 Gabriel Russo
 
 Copyright (c) 2020 Sandro Klippel
 
 O uso é fornecido sob a Licença do MIT. Veja
 em [LICENSE](https://github.com/gabriel-russo/cbers4asat/blob/master/LICENSE)
-para mais detalhes.
+para mais detalhes.
```

