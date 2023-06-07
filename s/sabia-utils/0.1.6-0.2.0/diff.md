# Comparing `tmp/sabia-utils-0.1.6.tar.gz` & `tmp/sabia-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabia-utils-0.1.6.tar", last modified: Mon Mar 27 20:37:10 2023, max compression
+gzip compressed data, was "sabia-utils-0.2.0.tar", last modified: Wed Jun  7 12:51:04 2023, max compression
```

## Comparing `sabia-utils-0.1.6.tar` & `sabia-utils-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 20:37:10.844869 sabia-utils-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1060 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2619 2023-03-27 20:37:10.843869 sabia-utils-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2358 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 20:37:10.840869 sabia-utils-0.1.6/sabia_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2825 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/concat.py
--rw-rw-rw-   0 root         (0) root         (0)     5225 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/group.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/pre_process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 20:37:10.843869 sabia-utils-0.1.6/sabia_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3633 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/utils/group_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/utils/parquet_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/sabia_utils/utils/preprocess_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 20:37:10.842869 sabia-utils-0.1.6/sabia_utils.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2619 2023-03-27 20:37:10.000000 sabia-utils-0.1.6/sabia_utils.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-03-27 20:37:10.000000 sabia-utils-0.1.6/sabia_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-27 20:37:10.000000 sabia-utils-0.1.6/sabia_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-03-27 20:37:10.000000 sabia-utils-0.1.6/sabia_utils.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-27 20:37:10.000000 sabia-utils-0.1.6/sabia_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 20:37:10.844869 sabia-utils-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-27 20:36:42.000000 sabia-utils-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:51:04.506068 sabia-utils-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-06-07 12:51:04.505068 sabia-utils-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:51:04.504068 sabia-utils-0.2.0/sabia_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/concat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11071 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4506 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/evaluateExperiments.py
+-rw-rw-rw-   0 root         (0) root         (0)     4668 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/pre_process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:51:04.505068 sabia-utils-0.2.0/sabia_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3305 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/utils/group_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/utils/parquet_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/sabia_utils/utils/preprocess_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:51:04.505068 sabia-utils-0.2.0/sabia_utils.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-06-07 12:51:04.000000 sabia-utils-0.2.0/sabia_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-07 12:51:04.000000 sabia-utils-0.2.0/sabia_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-07 12:51:04.000000 sabia-utils-0.2.0/sabia_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-07 12:51:04.000000 sabia-utils-0.2.0/sabia_utils.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-07 12:51:04.000000 sabia-utils-0.2.0/sabia_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 12:51:04.506068 sabia-utils-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-06-07 12:50:57.000000 sabia-utils-0.2.0/setup.py
```

### Comparing `sabia-utils-0.1.6/LICENSE` & `sabia-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabia-utils-0.1.6/PKG-INFO` & `sabia-utils-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sabia-utils
-Version: 0.1.6
+Version: 0.2.0
 Summary: Group of utilities for Sabia
-Author: Pedro Jesus
-Author-email: pedrovitora.jesus@gmail.com
+Author: AI Lab Unb
+Author-email: ailabunb@gmail.com
 License: MIT License
 Keywords: sabia utils
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sabia Utils
 
@@ -23,47 +23,47 @@
 * Returns a concatenated dataframe from all files in a path.
 * Can save the concatenated dataframe to a file.
 
 ```python
 from sabia_utils import concat
 
 concat.concatenate_all_from_path(
-    path='path//to//files',
-    output_file='output//file//path', # optional
+    path='path\\to\\files',
+    output_file='output\\file\\path', # optional
     fine_name='file_name'           # optional 
 )
 ```
 
 ### Concatenate some files from a path
 
 * Returns a concatenated dataframe from some files in a path.
 * Can save the concatenated dataframe to a file.
 
 ```python
 from sabia_utils import concat
 
 concat.concatenate_files(
-    path='path//to//files',
+    path='path\\to\\files',
     files=['file1', 'file2'],
-    output_file='output//file//path', # optional
+    output_file='output\\file\\path', # optional
     fine_name='file_name'           # optional 
 )
 ```
 
 
 ### Copy files from a path to another
 
 * Verify if the files exist in the path before copy.
 
 ```python
 from sabia_utils import group
 
 group.copy_new_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ## Group Module
 
 This module is used to group files.
 
@@ -71,30 +71,30 @@
 
 * Verify if the files exist in the path before process.
 
 ```python
 from sabia_utils import group
 
 group.process_existent_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ### Process all files
 
 * apply the function of copy and process files between the paths.
 
 ```python
 
 from sabia_utils import group
 
 group.process_all_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ## Pre_process Module
 
 This module is used to pre_process parquet files.
 
@@ -110,13 +110,13 @@
 from sabia_utils import pre_process
 
 class MyProcessor(Processing):
     def apply_to_df(self, df, column): 
         # Your pre-processing steps
 
 pre_process.pre_process_parquets(
-    folder_path='path//to//folder',
+    folder_path='path\\to\\folder',
     colomun_to_pre_process='column_name_to_be_processed',
     pre_processed_column='processed_column_name',
     processor=MyProcessor()
 )
 ```
```

### Comparing `sabia-utils-0.1.6/README.md` & `sabia-utils-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,47 +12,47 @@
 * Returns a concatenated dataframe from all files in a path.
 * Can save the concatenated dataframe to a file.
 
 ```python
 from sabia_utils import concat
 
 concat.concatenate_all_from_path(
-    path='path//to//files',
-    output_file='output//file//path', # optional
+    path='path\\to\\files',
+    output_file='output\\file\\path', # optional
     fine_name='file_name'           # optional 
 )
 ```
 
 ### Concatenate some files from a path
 
 * Returns a concatenated dataframe from some files in a path.
 * Can save the concatenated dataframe to a file.
 
 ```python
 from sabia_utils import concat
 
 concat.concatenate_files(
-    path='path//to//files',
+    path='path\\to\\files',
     files=['file1', 'file2'],
-    output_file='output//file//path', # optional
+    output_file='output\\file\\path', # optional
     fine_name='file_name'           # optional 
 )
 ```
 
 
 ### Copy files from a path to another
 
 * Verify if the files exist in the path before copy.
 
 ```python
 from sabia_utils import group
 
 group.copy_new_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ## Group Module
 
 This module is used to group files.
 
@@ -60,30 +60,30 @@
 
 * Verify if the files exist in the path before process.
 
 ```python
 from sabia_utils import group
 
 group.process_existent_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ### Process all files
 
 * apply the function of copy and process files between the paths.
 
 ```python
 
 from sabia_utils import group
 
 group.process_all_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ## Pre_process Module
 
 This module is used to pre_process parquet files.
 
@@ -99,13 +99,13 @@
 from sabia_utils import pre_process
 
 class MyProcessor(Processing):
     def apply_to_df(self, df, column): 
         # Your pre-processing steps
 
 pre_process.pre_process_parquets(
-    folder_path='path//to//folder',
+    folder_path='path\\to\\folder',
     colomun_to_pre_process='column_name_to_be_processed',
     pre_processed_column='processed_column_name',
     processor=MyProcessor()
 )
 ```
```

### Comparing `sabia-utils-0.1.6/sabia_utils/concat.py` & `sabia-utils-0.2.0/sabia_utils/concat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,76 @@
-from alei_utils import adapt_logger
 import logging
-from sabia_utils.utils.parquet_utils import (
-    concatenate_parquet_files,
-    delete_duplicate_rows,
-    take_files_from_path
-)
 import timeit
 
+from alei_utils import adapt_logger
+
+from sabia_utils.utils.parquet_utils import (concatenate_parquet_files,
+                                             delete_duplicate_rows,
+                                             take_files_from_path)
+
 logging.basicConfig(level="DEBUG")
 
 logger = logging.getLogger(__name__)
 
-adapter = adapt_logger(logger, {
-    "servico": "IJ",
-    "modulo": "IJ_CONCATENADOR_MAIN"
-    })
+adapter = adapt_logger(logger, {"servico": "IJ", "modulo": "IJ_CONCATENADOR_MAIN"})
 
 
-def concatenate_all_from_path(
-        path_in, path_out=None,
-        file_name='concatenated.parquet'
-        ):
-    '''
+def concatenate_all_from_path(path_in, path_out=None, file_name="concatenated.parquet"):
+    """
     Concatena todos os arquivos parquet de um determinado path
     :param path_in: path de entrada
     :param path_out: path de saida
     :param file_name: nome do arquivo de saida
     :return: dataframe concatenado
-    '''
+    """
     try:
         parquet_files = take_files_from_path(path_in)
         parquet_files.sort()
         inicio = timeit.default_timer()
         df = concatenate_parquet_files(parquet_files)
         df = delete_duplicate_rows(df)
         fim = timeit.default_timer()
-        tempo = fim-inicio
+        tempo = fim - inicio
         adapter.debug(
             f"tempo da concatenacao: {round(round(tempo,2)/60,2)} minutos",
             evento_status="E_S",
-            tag_evento="TEMPO DE EXECUCAO"
-        )
-        adapter.info(
-            "concatenacao finalizada",
-            evento_status="E_S",
-            tag_evento="CONCATECAO FINALIZADA"
+            tag_evento="TEMPO DE EXECUCAO",
         )
+        adapter.info("concatenacao finalizada", evento_status="E_S", tag_evento="CONCATECAO FINALIZADA")
         if path_out is not None:
-            df.to_parquet(path_out + '/' + file_name, index=False)
+            df.to_parquet(path_out + "/" + file_name, index=False)
         return df
     except Exception as erro:
         adapter.error(
-            f"Erro ao concatenar os arquivos: {erro}",
-            evento_status="E_E",
-            tag_evento="CONCATECAO ENCERRADA COM ERRO"
+            f"Erro ao concatenar os arquivos: {erro}", evento_status="E_E", tag_evento="CONCATECAO ENCERRADA COM ERRO"
         )
+
+
 # concat in the past is concated
 
 
-def concatenate_files(
-        files, path_out=None,
-        file_name='concatenated.parquet'
-        ):
-    '''
+def concatenate_files(files, path_out=None, file_name="concatenated.parquet"):
+    """
     Concatena aruivos parquet
     :param files: lista de arquivos
     :param path_out: path de saida
     :param file_name: nome do arquivo de saida
     :return: dataframe concatenado
-    '''
+    """
     try:
         inicio = timeit.default_timer()
         df = concatenate_parquet_files(files)
         fim = timeit.default_timer()
-        tempo = fim-inicio
+        tempo = fim - inicio
         adapter.debug(
             f"tempo da concatenacao: {round(round(tempo,2)/60,2)} minutos",
             evento_status="E_S",
-            tag_evento="TEMPO DE EXECUCAO"
-        )
-        adapter.info(
-            "concatenacao finalizada",
-            evento_status="E_S",
-            tag_evento="CONCATECAO FINALIZADA"
+            tag_evento="TEMPO DE EXECUCAO",
         )
+        adapter.info("concatenacao finalizada", evento_status="E_S", tag_evento="CONCATECAO FINALIZADA")
         if path_out is not None:
-            df.to_parquet(path_out + '/' + file_name, index=False)
+            df.to_parquet(path_out + "/" + file_name, index=False)
         return df
     except Exception as erro:
         adapter.error(
-            f"Erro ao concatenar os arquivos: {erro}",
-            evento_status="E_E",
-            tag_evento="CONCATECAO ENCERRADA COM ERRO"
+            f"Erro ao concatenar os arquivos: {erro}", evento_status="E_E", tag_evento="CONCATECAO ENCERRADA COM ERRO"
         )
```

### Comparing `sabia-utils-0.1.6/sabia_utils/group.py` & `sabia-utils-0.2.0/sabia_utils/group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,120 @@
-from alei_utils import adapt_logger
-from sabia_utils.utils.group_utils import diff_list, same_list, outer_join
-
 import logging
-import timeit
 import shutil
+import timeit
+
 import pandas as pd
+from alei_utils import adapt_logger
+
+from sabia_utils.utils.group_utils import diff_list, outer_join, same_list
+
 logging.basicConfig(level="DEBUG")
 logger = logging.getLogger(__name__)
 
-adapter = adapt_logger(logger, {
-    "servico": "IJ",
-    "modulo": "IJ_AGRUPADOR_GROUPER"
-    })
+adapter = adapt_logger(logger, {"servico": "IJ", "modulo": "IJ_AGRUPADOR_GROUPER"})
 
 
 def copy_new_files(PATH_IN, PATH_OUT):
-    '''
+    """
     Copia do path in para o path out os arquivos que não existem no path in
+
     :param PATH_IN: path de origem dos arquivos
     :param PATH_OUT: path de destino e comparação dos arquivos
     :return: None
-    '''
+    """
     try:
         inicio = timeit.default_timer()
         diff_files = diff_list(PATH_IN, PATH_OUT)
         if bool(diff_files):
             adapter.info(
-                f'''arquivos diferentes: {
+                f"""arquivos diferentes: {
                     diff_files
-                    }''',
-                evento_status="E_S",
-                tag_evento="ARQUIVOS DIFERENTES"
-                )
-            adapter.debug(
-                "copia de arquivos iniciada",
+                    }""",
                 evento_status="E_S",
-                tag_evento="COPIA INICIADA"
+                tag_evento="ARQUIVOS DIFERENTES",
             )
+            adapter.debug("copia de arquivos iniciada", evento_status="E_S", tag_evento="COPIA INICIADA")
             for file in diff_files:
-                shutil.copy(f'{PATH_IN}/{file}', PATH_OUT)
-                adapter.debug(
-                    f'arquivo copiado: {file}',
-                    evento_status="E_S",
-                    tag_evento="ARQUIVO COPIADO"
-                )
+                shutil.copy(f"{PATH_IN}/{file}", PATH_OUT)
+                adapter.debug(f"arquivo copiado: {file}", evento_status="E_S", tag_evento="ARQUIVO COPIADO")
             fim = timeit.default_timer()
-            tempo = fim-inicio
+            tempo = fim - inicio
             adapter.debug(
                 f"tempo de agrupamento: {round(round(tempo,2)/60,2)} minutos",
                 evento_status="E_S",
-                tag_evento="TEMPO DE EXECUCAO"
-            )
-            adapter.info(
-                "copia finalizada",
-                evento_status="E_S",
-                tag_evento="COPIA FINALIZADA"
+                tag_evento="TEMPO DE EXECUCAO",
             )
+            adapter.info("copia finalizada", evento_status="E_S", tag_evento="COPIA FINALIZADA")
         else:
-            adapter.debug(
-                "nenhum arquivo diferente encontrado",
-                evento_status="E_S",
-                tag_evento="PATHS SEM DIFERENÇAS"
-            )
+            adapter.debug("nenhum arquivo diferente encontrado", evento_status="E_S", tag_evento="PATHS SEM DIFERENÇAS")
 
     except Exception as erro:
         adapter.error(
-            f"Erro ao agrupar os arquivos: {erro}",
-            evento_status="E_E",
-            tag_evento="AGRUPAMENTO ENCERRADO COM ERRO"
+            f"Erro ao agrupar os arquivos: {erro}", evento_status="E_E", tag_evento="AGRUPAMENTO ENCERRADO COM ERRO"
         )
 
 
 def process_existent_files(PATH_IN, PATH_OUT):
-    '''
+    """
     Agrupa os arquivos que existem nos dois paths, fazendo um outer join
+
     :param PATH_IN: path de origem dos arquivos
     :param PATH_OUT: path de destino e comparação dos arquivos
     :return: None
-    '''
+    """
     try:
         same_files = same_list(PATH_IN, PATH_OUT)
         if bool(same_files):
             inicio = timeit.default_timer()
             adapter.info(
-                "agrupamento iniciado de arquivos existentes",
-                evento_status="E_S",
-                tag_evento="AGRUPAMENTO INICIADO"
+                "agrupamento iniciado de arquivos existentes", evento_status="E_S", tag_evento="AGRUPAMENTO INICIADO"
             )
             for file in same_files:
-                CACH_IN = f'{PATH_IN}/{file}'
-                CACH_OUT = f'{PATH_OUT}/{file}'
+                CACH_IN = f"{PATH_IN}/{file}"
+                CACH_OUT = f"{PATH_OUT}/{file}"
                 df_base = pd.read_parquet(CACH_OUT)
                 df_compare = pd.read_parquet(CACH_IN)
                 df_merge = outer_join(df_base, df_compare)
                 df_merge.to_parquet(CACH_OUT, index=False)
             fim = timeit.default_timer()
-            tempo = fim-inicio
+            tempo = fim - inicio
             adapter.debug(
                 f"tempo de agrupamento: {round(round(tempo,2)/60,2)} minutos",
                 evento_status="E_S",
-                tag_evento="TEMPO DE EXECUCAO"
-            )
-            adapter.info(
-                "agrupamento finalizado",
-                evento_status="E_S",
-                tag_evento="AGRUPAMENTO FINALIZADO"
+                tag_evento="TEMPO DE EXECUCAO",
             )
+            adapter.info("agrupamento finalizado", evento_status="E_S", tag_evento="AGRUPAMENTO FINALIZADO")
         else:
             adapter.debug(
-                "nenhum arquivo semelhante foi encontrado",
-                evento_status="E_S",
-                tag_evento="PATHS SEM DIFERENÇAS"
+                "nenhum arquivo semelhante foi encontrado", evento_status="E_S", tag_evento="PATHS SEM DIFERENÇAS"
             )
     except Exception as error:
         adapter.error(
-            f"Erro ao agrupar os arquivos: {error}",
-            evento_status="E_E",
-            tag_evento="AGRUPAMENTO ENCERRADO COM ERRO"
+            f"Erro ao agrupar os arquivos: {error}", evento_status="E_E", tag_evento="AGRUPAMENTO ENCERRADO COM ERRO"
         )
 
 
 def process_all_files(PATH_IN, PATH_OUT):
-    '''
+    """
     Agrupa todos os arquivos dos paths de maneira fazer um outer join e copy
+
     :param PATH_IN: path de origem dos arquivos
     :param PATH_OUT: path de destino e comparação dos arquivos
     :return: None
-    '''
+    """
     try:
         inicio = timeit.default_timer()
-        adapter.info(
-            "agrupamento geral iniciado",
-            evento_status="E_S",
-            tag_evento="AGRUPAMENTO INICIADO"
-        )
+        adapter.info("agrupamento geral iniciado", evento_status="E_S", tag_evento="AGRUPAMENTO INICIADO")
         copy_new_files(PATH_IN, PATH_OUT)
         process_existent_files(PATH_IN, PATH_OUT)
         fim = timeit.default_timer()
-        tempo = fim-inicio
+        tempo = fim - inicio
         adapter.debug(
             f"tempo de agrupamento: {round(round(tempo,2)/60,2)} minutos",
             evento_status="E_S",
-            tag_evento="TEMPO DE EXECUCAO"
-        )
-        adapter.info(
-            "agrupamento finalizado",
-            evento_status="E_S",
-            tag_evento="AGRUPAMENTO FINALIZADO"
+            tag_evento="TEMPO DE EXECUCAO",
         )
+        adapter.info("agrupamento finalizado", evento_status="E_S", tag_evento="AGRUPAMENTO FINALIZADO")
     except Exception as error:
         adapter.error(
-            f"Erro ao agrupar os arquivos: {error}",
-            evento_status="E_E",
-            tag_evento="AGRUPAMENTO ENCERRADO COM ERRO"
+            f"Erro ao agrupar os arquivos: {error}", evento_status="E_E", tag_evento="AGRUPAMENTO ENCERRADO COM ERRO"
         )
```

### Comparing `sabia-utils-0.1.6/sabia_utils/pre_process.py` & `sabia-utils-0.2.0/sabia_utils/pre_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,29 @@
 import os
 
 from sabia_utils.utils.preprocess_utils import read_parquet_files
 
 
 class Processing:
     def __init__(self):
-        self.method = ''
+        self.method = ""
 
     def apply_to_df(self, df, column):
         pass
 
 
-def pre_process_parquets(
-        folder_path, column_to_pre_process, pre_processed_column, processor):
-    '''
-    Pega todos os parquets do folder_path, seleciona todas as informações da
-    coluna column_to_pre_process e as pre-processa, criando a coluna pre_pro
-    cessed_column
+def pre_process_parquets(folder_path, column_to_pre_process, pre_processed_column, processor):
+    """
+    Pega todos os parquets do folder_path, seleciona todas as informações da coluna column_to_pre_process e as pre-processa, criando a coluna pre_processed_column
+
     :param folder_path: path de origem dos arquivos
     :param column_to_pre_process: nome da coluna a ser processada
     :param pre_processed_column: nome da coluna processada
-    :param processor: objeto de classe herdeira da classe Processing,
-    responsável por definir o pre-processamento
+    :param processor: objeto de classe herdeira da classe Processing, responsável por definir o pre-processamento
     :return: None
-    '''
+    """  # noqa: E501
     parquet_files = glob.glob(os.path.join(folder_path, "*.parquet"))
 
-    processed_df_list = read_parquet_files(
-        parquet_files, column_to_pre_process, pre_processed_column, processor)
+    processed_df_list = read_parquet_files(parquet_files, column_to_pre_process, pre_processed_column, processor)
 
     for df, f in processed_df_list:
         df.to_parquet(f)
```

### Comparing `sabia-utils-0.1.6/sabia_utils/utils/group_utils.py` & `sabia-utils-0.2.0/sabia_utils/utils/group_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,88 @@
 import logging
 import os
+
 from alei_utils import adapt_logger
+
 from sabia_utils.utils.parquet_utils import take_files_from_path
 
 logging.basicConfig(level="DEBUG")
 logger = logging.getLogger(__name__)
 
-adapter = adapt_logger(logger, {
-    "servico": "IJ",
-    "modulo": "IJ_AGRUPADOR_UTILS"
-    })
+adapter = adapt_logger(logger, {"servico": "IJ", "modulo": "IJ_AGRUPADOR_UTILS"})
 
 
 def diff_list(PATH_IN, PATH_OUT):
     try:
         parquet_files_int = take_files_from_path(PATH_IN)
         parquet_files_out = take_files_from_path(PATH_OUT)
         adapter.debug(
-            f"Arquivo tst encontrado: {parquet_files_int}",
-            evento_status="E_S",
-            tag_evento="ARQUIVO TST ENCONTRADO"
-        )
-        adapter.debug(
-            f"Arquivo sabia encontrado: {parquet_files_out}",
-            evento_status="E_S",
-            tag_evento="ARQUIVO SABIA ENCONTRADO"
-        )
-
-        list_tst = [
-            os.path.basename(file)
-            for file in parquet_files_int if file.endswith('.parquet')
-            ]
-        list_sabia = [
-            os.path.basename(file)
-            for file in parquet_files_out if file.endswith('.parquet')
-            ]
-        adapter.debug(
-            "busca de diferenças entre listas",
-            evento_status="E_S",
-            tag_evento="BUSCA DE DIFERENÇAS ENTRE LISTAS"
+            f"Arquivo tst encontrado: {parquet_files_int}", evento_status="E_S", tag_evento="ARQUIVO TST ENCONTRADO"
+        )
+        adapter.debug(
+            f"Arquivo sabia encontrado: {parquet_files_out}", evento_status="E_S", tag_evento="ARQUIVO SABIA ENCONTRADO"
+        )
+
+        list_tst = [os.path.basename(file) for file in parquet_files_int if file.endswith(".parquet")]
+        list_sabia = [os.path.basename(file) for file in parquet_files_out if file.endswith(".parquet")]
+        adapter.debug(
+            "busca de diferenças entre listas", evento_status="E_S", tag_evento="BUSCA DE DIFERENÇAS ENTRE LISTAS"
         )
         return list(set(list_tst) - set(list_sabia))
     except Exception as error:
         adapter.error(
             f"erro ao buscar diferenças entre listas: {error}",
             evento_status="E_E",
-            tag_evento="ERRO AO BUSCAR DIFERENÇAS ENTRE LISTAS"
+            tag_evento="ERRO AO BUSCAR DIFERENÇAS ENTRE LISTAS",
         )
         return None
 
 
 def same_list(PATH_IN, PATH_OUT):
     try:
         parquet_files_int = take_files_from_path(PATH_IN)
         parquet_files_out = take_files_from_path(PATH_OUT)
         adapter.debug(
-            f"Arquivo in encontrado: {parquet_files_int}",
-            evento_status="E_S",
-            tag_evento="ARQUIVO IN ENCONTRADO"
-        )
-        adapter.debug(
-            f"Arquivo out encontrado: {parquet_files_out}",
-            evento_status="E_S",
-            tag_evento="ARQUIVO OUT ENCONTRADO"
-        )
-
-        list_tst = [
-            os.path.basename(file)
-            for file in parquet_files_int if file.endswith('.parquet')
-            ]
-        list_sabia = [
-            os.path.basename(file)
-            for file in parquet_files_out if file.endswith('.parquet')
-            ]
-        adapter.debug(
-            "busca de semelhanças entre listas",
-            evento_status="E_S",
-            tag_evento="BUSCA DE SEMELHANÇAS ENTRE LISTAS"
+            f"Arquivo in encontrado: {parquet_files_int}", evento_status="E_S", tag_evento="ARQUIVO IN ENCONTRADO"
+        )
+        adapter.debug(
+            f"Arquivo out encontrado: {parquet_files_out}", evento_status="E_S", tag_evento="ARQUIVO OUT ENCONTRADO"
+        )
+
+        list_tst = [os.path.basename(file) for file in parquet_files_int if file.endswith(".parquet")]
+        list_sabia = [os.path.basename(file) for file in parquet_files_out if file.endswith(".parquet")]
+        adapter.debug(
+            "busca de semelhanças entre listas", evento_status="E_S", tag_evento="BUSCA DE SEMELHANÇAS ENTRE LISTAS"
         )
         return list(set(list_tst) & set(list_sabia))
     except Exception as error:
         adapter.error(
             f"erro ao buscar semelhanças entre listas: {error}",
             evento_status="E_E",
-            tag_evento="ERRO AO BUSCAR SEMELHANÇAS ENTRE LISTAS"
+            tag_evento="ERRO AO BUSCAR SEMELHANÇAS ENTRE LISTAS",
         )
         return None
 
 
 def outer_join(df_base, df_compare):
     try:
         adapter.debug(
-            "busca de diferenças entre linhas",
-            evento_status="E_S",
-            tag_evento="BUSCA DE DIFERENÇAS ENTRE LINHAS"
+            "busca de diferenças entre linhas", evento_status="E_S", tag_evento="BUSCA DE DIFERENÇAS ENTRE LINHAS"
         )
-        return df_base.merge(df_compare, how='outer', indicator=False)
+        return df_base.merge(df_compare, how="outer", indicator=False)
 
     except Exception as error:
         adapter.error(
             f"erro ao buscar diferenças entre linhas: {error}",
             evento_status="E_E",
-            tag_evento="ERRO AO BUSCAR DIFERENÇAS ENTRE LINHAS"
+            tag_evento="ERRO AO BUSCAR DIFERENÇAS ENTRE LINHAS",
         )
         return None
 
+
 # import pandas as pd
 # df1 = pd.read_parquet('../test/data/df1_test.parquet')
 # df2 = pd.read_parquet('../test/data/df2_test.parquet')
 # print(df1)
 # print(df2)
 # print(diff_lines('../test/data/df1_test.parquet',
 #  '../test/data/df2_test.parquet'))
```

### Comparing `sabia-utils-0.1.6/sabia_utils/utils/parquet_utils.py` & `sabia-utils-0.2.0/sabia_utils/utils/parquet_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,71 @@
-import logging
-import pandas as pd
 import glob
+import logging
 import os
-from alei_utils import adapt_logger
 import timeit
 
+import pandas as pd
+from alei_utils import adapt_logger
 
 logging.basicConfig(level="DEBUG")
 logger = logging.getLogger(__name__)
 
-adapter = adapt_logger(logger, {
-    "servico": "IJ",
-    "modulo": "IJ_CONCATENADOR_PACKAGE"
-    })
+adapter = adapt_logger(logger, {"servico": "IJ", "modulo": "IJ_CONCATENADOR_PACKAGE"})
 
 
 def concatenate_parquet_files(files):
     try:
         inicio = timeit.default_timer()
         files.sort()
-        adapter.info(
-            "concatenacao iniciada",
-            evento_status="E_S",
-            tag_evento="CONCATENACAO INICIADA"
-        )
+        adapter.info("concatenacao iniciada", evento_status="E_S", tag_evento="CONCATENACAO INICIADA")
         ct = 0
         parquet = []
         for f in files:
             try:
                 parquet.append(pd.read_parquet(f))
                 df = pd.concat(parquet, ignore_index=True)
                 ct += 1
-                if (ct >= 10):
-                    tempo = timeit.default_timer()-inicio
+                if ct >= 10:
+                    tempo = timeit.default_timer() - inicio
                     ct = 0
                     adapter.debug(
                         f"tempo da concatenacao parcial: {tempo} segundos",
                         evento_status="E_S",
-                        tag_evento="TEMPO DE EXECUCAO"
+                        tag_evento="TEMPO DE EXECUCAO",
                     )
-                adapter.info(
-                    f"concatenando parquet: {f}",
-                    evento_status="E_S",
-                    tag_evento=f"CONCATENANDO PARQUET: {f}"
-                )
+                adapter.info(f"concatenando parquet: {f}", evento_status="E_S", tag_evento=f"CONCATENANDO PARQUET: {f}")
 
             except Exception as error:
                 adapter.error(
                     f"erro ao concatenar arquivo: {f} {error}",
                     evento_status="E_E",
-                    tag_evento=f"ERRO AO CONCATENAR ARQUIVO: {f}"
+                    tag_evento=f"ERRO AO CONCATENAR ARQUIVO: {f}",
                 )
         return df
     except Exception as error:
         adapter.error(
-            f"erro ao concatenar arquivos: {error}",
-            evento_status="E_E",
-            tag_evento="ERRO AO CONCATENAR ARQUIVOS"
+            f"erro ao concatenar arquivos: {error}", evento_status="E_E", tag_evento="ERRO AO CONCATENAR ARQUIVOS"
         )
         return None
 
 
 def delete_duplicate_rows(df):
     try:
-        adapter.info(
-            "remocao de duplicatas iniciada",
-            evento_status="E_S",
-            tag_evento="REMOCAO DE DUPLICATAS INICIADA"
-        )
+        adapter.info("remocao de duplicatas iniciada", evento_status="E_S", tag_evento="REMOCAO DE DUPLICATAS INICIADA")
         adapter.debug(
-            "remocao de duplicatas iniciada",
-            evento_status="E_S",
-            tag_evento="REMOCAO DE DUPLICATAS INICIADA"
+            "remocao de duplicatas iniciada", evento_status="E_S", tag_evento="REMOCAO DE DUPLICATAS INICIADA"
         )
-        return df.drop_duplicates(subset=['processo_numero'], keep='last')
+        return df.drop_duplicates(subset=["processo_numero"], keep="last")
     except Exception as error:
         adapter.error(
-            f"erro ao remover duplicatas: {error}",
-            evento_status="E_E",
-            tag_evento="ERRO AO REMOVER DUPLICATAS"
+            f"erro ao remover duplicatas: {error}", evento_status="E_E", tag_evento="ERRO AO REMOVER DUPLICATAS"
         )
         return None
 
 
 def take_files_from_path(path):
     try:
-        adapter.info(
-            "busca de arquivos iniciada",
-            evento_status="E_S",
-            tag_evento="BUSCA DE ARQUIVOS INICIADA"
-        )
+        adapter.info("busca de arquivos iniciada", evento_status="E_S", tag_evento="BUSCA DE ARQUIVOS INICIADA")
         return glob.glob(os.path.join(path, "*.parquet"))
     except Exception as error:
-        adapter.error(
-            f"erro ao buscar arquivos: {error}",
-            evento_status="E_E",
-            tag_evento="ERRO AO BUSCAR ARQUIVOS"
-        )
+        adapter.error(f"erro ao buscar arquivos: {error}", evento_status="E_E", tag_evento="ERRO AO BUSCAR ARQUIVOS")
         return None
```

### Comparing `sabia-utils-0.1.6/sabia_utils/utils/preprocess_utils.py` & `sabia-utils-0.2.0/sabia_utils/utils/preprocess_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,51 @@
-import pandas as pd
+import datetime
 import logging
+
+import pandas as pd
 from alei_utils import adapt_logger
-import datetime
 
 logging.basicConfig(level="DEBUG")
 
 logger = logging.getLogger(__name__)
 
-adapter = adapt_logger(logger, {
-    "servico": "IJ",
-    "modulo": "IJ_PRE_PROCESSAMENTO"
-    })
+adapter = adapt_logger(logger, {"servico": "IJ", "modulo": "IJ_PRE_PROCESSAMENTO"})
 
 
-def read_parquet_files(
-        files, column_to_pre_process, pre_processed_column, processor):
-
+def read_parquet_files(files, column_to_pre_process, pre_processed_column, processor):
     try:
         df_list = []
         inicio = datetime.datetime.now()
         for f in files:
-            adapter.info(
-                f"pre-processando arquivo: {f}",
-                evento_status="E_S",
-                tag_evento="PRE-PROCESSAMENTO INICIADO"
-            )
+            adapter.info(f"pre-processando arquivo: {f}", evento_status="E_S", tag_evento="PRE-PROCESSAMENTO INICIADO")
             inicio_arquivo = datetime.datetime.now()
             df = pd.read_parquet(f)
             processor.apply_to_df(df, column_to_pre_process)
             if pre_processed_column in df.columns:
                 null_rows = df[df[pre_processed_column].isnull()]
                 if not null_rows.empty:
-                    null_rows = processor.apply_to_df(
-                        null_rows, column_to_pre_process)
+                    null_rows = processor.apply_to_df(null_rows, column_to_pre_process)
                     df.loc[null_rows.index] = null_rows
             else:
                 df = processor.apply_to_df(df, column_to_pre_process)
             df_list.append((df, f))
             final_arquivo = datetime.datetime.now()
             tempo_arquivo = final_arquivo - inicio_arquivo
             tempo_arquivo_str = str(tempo_arquivo).split(".")[0]
             adapter.debug(
                 f"tempo de processamento do arquivo {f}: {tempo_arquivo_str}",
                 evento_status="E_S",
-                tag_evento="TEMPO DE PRE-PROCESSAMENTO"
+                tag_evento="TEMPO DE PRE-PROCESSAMENTO",
             )
         fim = datetime.datetime.now()
         tempo = fim - inicio
         tempo_str = str(tempo).split(".")[0]
         adapter.debug(
-            f"tempo total de pre-processamento: {tempo_str}",
-            evento_status="E_S",
-            tag_evento="TEMPO DE EXECUCAO"
-        )
-        adapter.info(
-            "pre-processamento finalizado",
-            evento_status="E_S",
-            tag_evento="PRE-PROCESSAMENTO FINALIZADO"
+            f"tempo total de pre-processamento: {tempo_str}", evento_status="E_S", tag_evento="TEMPO DE EXECUCAO"
         )
+        adapter.info("pre-processamento finalizado", evento_status="E_S", tag_evento="PRE-PROCESSAMENTO FINALIZADO")
 
         return df_list
     except Exception as erro:
         adapter.error(
-            f"Erro ao processar os arquivos: {erro}",
-            evento_status="E_E",
-            tag_evento="PRE-PROCESSAMENTO COM ERRO"
+            f"Erro ao processar os arquivos: {erro}", evento_status="E_E", tag_evento="PRE-PROCESSAMENTO COM ERRO"
         )
```

### Comparing `sabia-utils-0.1.6/sabia_utils.egg-info/PKG-INFO` & `sabia-utils-0.2.0/sabia_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sabia-utils
-Version: 0.1.6
+Version: 0.2.0
 Summary: Group of utilities for Sabia
-Author: Pedro Jesus
-Author-email: pedrovitora.jesus@gmail.com
+Author: AI Lab Unb
+Author-email: ailabunb@gmail.com
 License: MIT License
 Keywords: sabia utils
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sabia Utils
 
@@ -23,47 +23,47 @@
 * Returns a concatenated dataframe from all files in a path.
 * Can save the concatenated dataframe to a file.
 
 ```python
 from sabia_utils import concat
 
 concat.concatenate_all_from_path(
-    path='path//to//files',
-    output_file='output//file//path', # optional
+    path='path\\to\\files',
+    output_file='output\\file\\path', # optional
     fine_name='file_name'           # optional 
 )
 ```
 
 ### Concatenate some files from a path
 
 * Returns a concatenated dataframe from some files in a path.
 * Can save the concatenated dataframe to a file.
 
 ```python
 from sabia_utils import concat
 
 concat.concatenate_files(
-    path='path//to//files',
+    path='path\\to\\files',
     files=['file1', 'file2'],
-    output_file='output//file//path', # optional
+    output_file='output\\file\\path', # optional
     fine_name='file_name'           # optional 
 )
 ```
 
 
 ### Copy files from a path to another
 
 * Verify if the files exist in the path before copy.
 
 ```python
 from sabia_utils import group
 
 group.copy_new_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ## Group Module
 
 This module is used to group files.
 
@@ -71,30 +71,30 @@
 
 * Verify if the files exist in the path before process.
 
 ```python
 from sabia_utils import group
 
 group.process_existent_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ### Process all files
 
 * apply the function of copy and process files between the paths.
 
 ```python
 
 from sabia_utils import group
 
 group.process_all_files(
-    PATH_IN='path//to//files1',
-    PATH_OUT='path//to//files2'
+    PATH_IN='path\\to\\files1',
+    PATH_OUT='path\\to\\files2'
 )
 ```
 
 ## Pre_process Module
 
 This module is used to pre_process parquet files.
 
@@ -110,13 +110,13 @@
 from sabia_utils import pre_process
 
 class MyProcessor(Processing):
     def apply_to_df(self, df, column): 
         # Your pre-processing steps
 
 pre_process.pre_process_parquets(
-    folder_path='path//to//folder',
+    folder_path='path\\to\\folder',
     colomun_to_pre_process='column_name_to_be_processed',
     pre_processed_column='processed_column_name',
     processor=MyProcessor()
 )
 ```
```

