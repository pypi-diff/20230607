# Comparing `tmp/peachdb-0.0.9.tar.gz` & `tmp/peachdb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-0.0.9.tar", last modified: Tue May 30 17:36:35 2023, max compression
+gzip compressed data, was "peachdb-0.1.0.tar", last modified: Tue Jun  6 22:10:17 2023, max compression
```

## Comparing `peachdb-0.0.9.tar` & `peachdb-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.9/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.9/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:36:35.331771 peachdb-0.0.9/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.9/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.9/peachdb/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/backends/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.9/peachdb/backends/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.9/peachdb/backends/backend_base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.9/peachdb/backends/hnsw_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.9/peachdb/backends/numpy_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.9/peachdb/backends/torch_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      388 2023-05-30 17:33:07.000000 peachdb-0.0.9/peachdb/constants.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/embedder/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.9/peachdb/embedder/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/embedder/containers/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:50:04.000000 peachdb-0.0.9/peachdb/embedder/containers/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2169 2023-05-30 17:33:37.000000 peachdb-0.0.9/peachdb/embedder/containers/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1568 2023-05-29 20:32:06.000000 peachdb-0.0.9/peachdb/embedder/containers/sentence_transformer.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb/embedder/models/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:49:59.000000 peachdb-0.0.9/peachdb/embedder/models/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-26 16:27:29.000000 peachdb-0.0.9/peachdb/embedder/models/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      598 2023-05-29 10:12:31.000000 peachdb-0.0.9/peachdb/embedder/models/sentence_transformer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.9/peachdb/embedder/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:36:35.331771 peachdb-0.0.9/peachdb.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      727 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      151 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 17:36:35.000000 peachdb-0.0.9/peachdb.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.9/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      151 2023-05-30 17:08:02.000000 peachdb-0.0.9/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 17:36:35.331771 peachdb-0.0.9/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 17:17:02.000000 peachdb-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.295055 peachdb-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-06 22:10:08.000000 peachdb-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 22:10:08.000000 peachdb-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-06 22:10:17.295055 peachdb-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-06 22:10:08.000000 peachdb-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.287055 peachdb-0.1.0/peachdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.291056 peachdb-0.1.0/peachdb/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/backends/backend_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/backends/hnsw_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/backends/torch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.291056 peachdb-0.1.0/peachdb/embedder/
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.295055 peachdb-0.1.0/peachdb/embedder/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/containers/multimodal_imagebind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/containers/sentence_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.295055 peachdb-0.1.0/peachdb/embedder/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/models/multimodal_imagebind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/models/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/embedder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-06 22:10:08.000000 peachdb-0.1.0/peachdb/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:10:17.291056 peachdb-0.1.0/peachdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-06 22:10:17.000000 peachdb-0.1.0/peachdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-06 22:10:17.000000 peachdb-0.1.0/peachdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-06 22:10:17.000000 peachdb-0.1.0/peachdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-06 22:10:17.000000 peachdb-0.1.0/peachdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 22:10:17.000000 peachdb-0.1.0/peachdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 22:10:08.000000 peachdb-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-06 22:10:08.000000 peachdb-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:10:17.295055 peachdb-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-06 22:10:08.000000 peachdb-0.1.0/setup.py
```

### Comparing `peachdb-0.0.9/LICENSE` & `peachdb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.9/PKG-INFO` & `peachdb-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-Metadata-Version: 2.1
-Name: peachdb
-Version: 0.0.9
-License: Apache License 2.0
-Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
-Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PeachDB
 
 <h3 align="center"><strong>PeachDB - the AI-First, Embeddings Database</strong></h3>
 <h4 align="center">Build memory for your AI products in <strong>minutes!</strong></h4>
 
 <br/>
 
-**Our core API has 3 functions**
+**Our core API has 4 functions**
 
 ```python
 from peachdb import PeachDB
 
-# Create a new PeachDB instance
-# Embeddings are automatically computed at scale using the selected `embedding_generator` model on Modal.
-db = PeachDB.create(
+# Create a new PeachDB instance or reference an existing one
+db = PeachDB(
     project_name="my_app",
+    embedding_generator="imagebind",  # "imagebind" or "sentence_transformer_L12"
+    embedding_backend="exact_cpu",  # "exact_cpu", "exact_gpu", or "approx"
+    distance_metric="cosine",  # "cosine" or "l2"
+)
+
+# Auto-compute & upsert embeddings at scale using the specified `embedding_generator` model on Modal
+db.upsert_text(  # or "upsert_image" or "upsert_audio"
     csv_path="/path/to/local/csv",  # or "s3://path/to/csv"
-    column_to_embed="foo",
+    column_to_embed="foo",  # column values can either be string or public URI to image/audio
     id_column_name="id",
-    max_rows=None, # or N, to process N rows of the dataset 
-    distance_metric="cosine",  # or "l2"
-    embedding_backend="exact_cpu",  # or "exact_gpu" or "approx"
-    embedding_generator="sentence_transformer_L12",
-    embeddings_output_s3_bucket_uri=None, # required when using S3 URI for `csv_path`
+    embeddings_output_s3_bucket_uri=None,  # required when using S3 URI for `csv_path`
+    max_rows=None,  # or N to process N rows
 )
-# Once the database has been successfully setup, you can reference it in the future via
-# db = PeachDB(project_name="my_app")
 
-# Query/search 5 most similar results
-results_df = db.query(text='An example query', top_k=5)
+# Query top 5 similar results
+ids, distances, results_df = db.query(
+    query_input='An example query',  # or path to an image/audio file
+    modality='text',  # "text", "image", or "audio"
+    top_k=5
+)
 
-# Deploy the database as a publicly available FastAPI server
-# Call GET /query?text='An example query'&top_k=5 to fetch 5 most similar results
+# Deploy database as a publicly accessible FastAPI server
+# GET /query?query_input='An example query'&modality=[text|image|audio]&top_k=5 to fetch 5 most similar results
 db.deploy()
 ```
 
 ## Why another embedding database?
 We've streamlined the entire end-to-end process of creating, storing, and retrieving embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
 
 Our key features include:
 * **Automated, cost-effective & large-scale embedding computation**: We leverage serverless GPU functions (through [Modal](https://modal.com/)) to compute embeddings on a large scale efficiently and affordably.
     - For instance, we processed the [Kaggle 5M song lyrics dataset](https://www.kaggle.com/datasets/nikhilnayak123/5-million-song-lyrics-dataset?resource=download&select=ds2.csv) in just *12 minutes at a cost of $4.90*, using sentence transformers!
-    - We've developed a Modal wrapper for [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2).
-        - *Coming soon*: Modal wrappers for open-source embedding models such as [ImageBind](https://github.com/facebookresearch/ImageBind), [OpenCLIP](https://github.com/mlfoundations/open_clip), and more.
-        - *Coming soon*: Support for multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
+    - We've developed Modal wrappers for:
+        - [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2)
+        - [ImageBind](https://github.com/facebookresearch/ImageBind),
+        - *Coming soon*, support for:
+            - Open-source embedding models such as [OpenCLIP](https://github.com/mlfoundations/open_clip), [Microsoft E5-v2](https://arxiv.org/pdf/2212.03533.pdf), and more.
+            - Multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
     - *Coming soon*: Bring your own embeddings.
     - *Coming soon*: Custom embedding functions for even more flexibility.
 * **Multimodality**: Native support for data with mixture of modalities (such as image/audio/video).
 * **Highly Customizable**: PeachDB allows you to tailor its features to your needs. You can customize:
     - Embedding computation: as described above.
     - Backend: choose between `exact_cpu` (numpy), `exact_gpu` (torch), or `approx` (HNSW).
     - Distance metrics: `cosine` or `l2`.
@@ -75,53 +73,46 @@
 - Create & activate a new conda environment `conda create -n spoti_vibe python=3.10` & `conda activate spoti_vibe`
 - Install PeachDB: `pip install peachdb`
 - Setup [Modal](https://modal.com)
     - Create an account at [modal.com](https://modal.com)
     - Install the modal-client package: `pip install modal-client`
     - Setup token: `modal token new`
 
-- (optional) PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, create & configure your .env file as below.
-    ```python
-    # Fetch the below values from ~/.aws/credentials
-    AWS_ACCESS_KEY_ID=
-    AWS_SECRET_ACCESS_KEY=
-    ```
-    Please ensure the credentials have read & write access to the relevant bucket you plan to use.
+- (optional: for AWS S3) PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, ensure you've installed the `aws` cli and run `aws configure`. The credentials should have read & write access to the relevant bucket you plan to use.
 - `mkdir spoti_vibe/`
 - Create a new module inside the directory `server.py`
 - Add the following code
     ```python
     from peachdb import PeachDB
 
     import os
+
     # Fetch the username & key by creating a new API token at https://www.kaggle.com/settings
-    os.environ['KAGGLE_USERNAME'] = None # set user name
-    os.environ['KAGGLE_KEY'] = None # set key
+    os.environ["KAGGLE_USERNAME"] = None  # set user name
+    os.environ["KAGGLE_KEY"] = None  # set key
 
-    import kaggle # make sure you've run `pip install kaggle`
+    import kaggle  # make sure you've run `pip install kaggle`
 
     kaggle.api.authenticate()
-    kaggle.api.dataset_download_files(
-        'nikhilnayak123/5-million-song-lyrics-dataset',
-        path='.',
-        unzip=True
-    )
+    # It can take a few mins to download depending on the network speed
+    kaggle.api.dataset_download_files("nikhilnayak123/5-million-song-lyrics-dataset", path=".", unzip=True)
 
-    db = PeachDB.create(
+    db = PeachDB(
         project_name="spoti_vibe",
-        csv_path='./ds2.csv',  # dataset name as observed on Kaggle
-        column_to_embed="lyrics",
-        id_column_name="id",
-        max_rows=None,
         distance_metric="cosine",
         embedding_backend="exact_cpu",
         embedding_generator="sentence_transformer_L12",
     )
+    db.upsert_text(
+        csv_path="./ds2.csv",  # dataset name as observed on Kaggle
+        column_to_embed="lyrics",
+        id_column_name="id",
+    )
 
-    db.deploy() # Public URL will be printed to console
+    db.deploy()  # Public URL will be printed to console
     ```
 
 And that's it! You should now have a publicly available server that can listen to query requests from the user on: <br/>
 `GET <PUBLIC_URL>/query?text='Happy, upbeat summer'&top_k=5`
 
 ## Use-cases
 - Build web apps like - [clip.audio](https://www.clip.audio/) & [awesome-movies.life](https://awesome-movies.life/)
```

### Comparing `peachdb-0.0.9/README.md` & `peachdb-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,70 @@
+Metadata-Version: 2.1
+Name: peachdb
+Version: 0.1.0
+License: Apache License 2.0
+Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
+Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PeachDB
 
 <h3 align="center"><strong>PeachDB - the AI-First, Embeddings Database</strong></h3>
 <h4 align="center">Build memory for your AI products in <strong>minutes!</strong></h4>
 
 <br/>
 
-**Our core API has 3 functions**
+**Our core API has 4 functions**
 
 ```python
 from peachdb import PeachDB
 
-# Create a new PeachDB instance
-# Embeddings are automatically computed at scale using the selected `embedding_generator` model on Modal.
-db = PeachDB.create(
+# Create a new PeachDB instance or reference an existing one
+db = PeachDB(
     project_name="my_app",
+    embedding_generator="imagebind",  # "imagebind" or "sentence_transformer_L12"
+    embedding_backend="exact_cpu",  # "exact_cpu", "exact_gpu", or "approx"
+    distance_metric="cosine",  # "cosine" or "l2"
+)
+
+# Auto-compute & upsert embeddings at scale using the specified `embedding_generator` model on Modal
+db.upsert_text(  # or "upsert_image" or "upsert_audio"
     csv_path="/path/to/local/csv",  # or "s3://path/to/csv"
-    column_to_embed="foo",
+    column_to_embed="foo",  # column values can either be string or public URI to image/audio
     id_column_name="id",
-    max_rows=None, # or N, to process N rows of the dataset 
-    distance_metric="cosine",  # or "l2"
-    embedding_backend="exact_cpu",  # or "exact_gpu" or "approx"
-    embedding_generator="sentence_transformer_L12",
-    embeddings_output_s3_bucket_uri=None, # required when using S3 URI for `csv_path`
+    embeddings_output_s3_bucket_uri=None,  # required when using S3 URI for `csv_path`
+    max_rows=None,  # or N to process N rows
 )
-# Once the database has been successfully setup, you can reference it in the future via
-# db = PeachDB(project_name="my_app")
 
-# Query/search 5 most similar results
-results_df = db.query(text='An example query', top_k=5)
+# Query top 5 similar results
+ids, distances, results_df = db.query(
+    query_input='An example query',  # or path to an image/audio file
+    modality='text',  # "text", "image", or "audio"
+    top_k=5
+)
 
-# Deploy the database as a publicly available FastAPI server
-# Call GET /query?text='An example query'&top_k=5 to fetch 5 most similar results
+# Deploy database as a publicly accessible FastAPI server
+# GET /query?query_input='An example query'&modality=[text|image|audio]&top_k=5 to fetch 5 most similar results
 db.deploy()
 ```
 
 ## Why another embedding database?
 We've streamlined the entire end-to-end process of creating, storing, and retrieving embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
 
 Our key features include:
 * **Automated, cost-effective & large-scale embedding computation**: We leverage serverless GPU functions (through [Modal](https://modal.com/)) to compute embeddings on a large scale efficiently and affordably.
     - For instance, we processed the [Kaggle 5M song lyrics dataset](https://www.kaggle.com/datasets/nikhilnayak123/5-million-song-lyrics-dataset?resource=download&select=ds2.csv) in just *12 minutes at a cost of $4.90*, using sentence transformers!
-    - We've developed a Modal wrapper for [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2).
-        - *Coming soon*: Modal wrappers for open-source embedding models such as [ImageBind](https://github.com/facebookresearch/ImageBind), [OpenCLIP](https://github.com/mlfoundations/open_clip), and more.
-        - *Coming soon*: Support for multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
+    - We've developed Modal wrappers for:
+        - [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2)
+        - [ImageBind](https://github.com/facebookresearch/ImageBind),
+        - *Coming soon*, support for:
+            - Open-source embedding models such as [OpenCLIP](https://github.com/mlfoundations/open_clip), [Microsoft E5-v2](https://arxiv.org/pdf/2212.03533.pdf), and more.
+            - Multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
     - *Coming soon*: Bring your own embeddings.
     - *Coming soon*: Custom embedding functions for even more flexibility.
 * **Multimodality**: Native support for data with mixture of modalities (such as image/audio/video).
 * **Highly Customizable**: PeachDB allows you to tailor its features to your needs. You can customize:
     - Embedding computation: as described above.
     - Backend: choose between `exact_cpu` (numpy), `exact_gpu` (torch), or `approx` (HNSW).
     - Distance metrics: `cosine` or `l2`.
@@ -65,53 +83,46 @@
 - Create & activate a new conda environment `conda create -n spoti_vibe python=3.10` & `conda activate spoti_vibe`
 - Install PeachDB: `pip install peachdb`
 - Setup [Modal](https://modal.com)
     - Create an account at [modal.com](https://modal.com)
     - Install the modal-client package: `pip install modal-client`
     - Setup token: `modal token new`
 
-- (optional) PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, create & configure your .env file as below.
-    ```python
-    # Fetch the below values from ~/.aws/credentials
-    AWS_ACCESS_KEY_ID=
-    AWS_SECRET_ACCESS_KEY=
-    ```
-    Please ensure the credentials have read & write access to the relevant bucket you plan to use.
+- (optional: for AWS S3) PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, ensure you've installed the `aws` cli and run `aws configure`. The credentials should have read & write access to the relevant bucket you plan to use.
 - `mkdir spoti_vibe/`
 - Create a new module inside the directory `server.py`
 - Add the following code
     ```python
     from peachdb import PeachDB
 
     import os
+
     # Fetch the username & key by creating a new API token at https://www.kaggle.com/settings
-    os.environ['KAGGLE_USERNAME'] = None # set user name
-    os.environ['KAGGLE_KEY'] = None # set key
+    os.environ["KAGGLE_USERNAME"] = None  # set user name
+    os.environ["KAGGLE_KEY"] = None  # set key
 
-    import kaggle # make sure you've run `pip install kaggle`
+    import kaggle  # make sure you've run `pip install kaggle`
 
     kaggle.api.authenticate()
-    kaggle.api.dataset_download_files(
-        'nikhilnayak123/5-million-song-lyrics-dataset',
-        path='.',
-        unzip=True
-    )
+    # It can take a few mins to download depending on the network speed
+    kaggle.api.dataset_download_files("nikhilnayak123/5-million-song-lyrics-dataset", path=".", unzip=True)
 
-    db = PeachDB.create(
+    db = PeachDB(
         project_name="spoti_vibe",
-        csv_path='./ds2.csv',  # dataset name as observed on Kaggle
-        column_to_embed="lyrics",
-        id_column_name="id",
-        max_rows=None,
         distance_metric="cosine",
         embedding_backend="exact_cpu",
         embedding_generator="sentence_transformer_L12",
     )
+    db.upsert_text(
+        csv_path="./ds2.csv",  # dataset name as observed on Kaggle
+        column_to_embed="lyrics",
+        id_column_name="id",
+    )
 
-    db.deploy() # Public URL will be printed to console
+    db.deploy()  # Public URL will be printed to console
     ```
 
 And that's it! You should now have a publicly available server that can listen to query requests from the user on: <br/>
 `GET <PUBLIC_URL>/query?text='Happy, upbeat summer'&top_k=5`
 
 ## Use-cases
 - Build web apps like - [clip.audio](https://www.clip.audio/) & [awesome-movies.life](https://awesome-movies.life/)
```

### Comparing `peachdb-0.0.9/peachdb/backends/backend_base.py` & `peachdb-0.1.0/peachdb/embedder/containers/sentence_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,92 @@
-import abc
-import os
+from typing import Optional, Union
 
-import duckdb
-import numpy as np
-import pandas as pd
-from rich import print
+import modal
+import pyarrow as pa  # type: ignore
 
+from peachdb.embedder.containers.base import EmbeddingModelBase, base_container_image, modal_compute_spec_decorator
 from peachdb.embedder.models.sentence_transformer import SentenceTransformerModel
-from peachdb.embedder.utils import S3File, S3Folder, is_s3_uri
 
+SENTENCE_TRANSFORMER_BATCH_SIZE = 64
 
-class BackendBase(abc.ABC):
-    def __init__(
+sbert_stub = modal.Stub("SBERT")
+
+
+def download_model():
+    SentenceTransformerModel.download_model()
+
+
+image = base_container_image.run_function(download_model)
+
+
+@modal_compute_spec_decorator(stub=sbert_stub, image=image)
+class SentenceTransformerEmbedder(EmbeddingModelBase):
+    def __enter__(self):
+        self.model = SentenceTransformerModel()
+
+    def _calculate_text_embeddings(self, texts, show_progress_bar: bool):
+        return self.model.encode_texts(
+            texts,
+            batch_size=SENTENCE_TRANSFORMER_BATCH_SIZE,
+            show_progress_bar=show_progress_bar,
+        )
+
+    # TODO: are defining these functions necessary?
+    def _calculate_audio_embeddings(self, audio_paths, show_progress_bar: bool):
+        raise NotImplementedError
+
+    def _calculate_image_embeddings(self, image_paths: list, show_progress_bar: bool):
+        raise NotImplementedError
+
+    @property
+    def _can_take_text_input(cls):
+        return True
+
+    @property
+    def _can_take_audio_input(cls):
+        return False
+
+    @property
+    def _can_take_image_input(cls):
+        # return True - once implemented!
+        return False
+
+    # We need to rewrite this function in all the inherited class so we can use the @modal method decorator.
+    # TODO: check if above statement is true / if we can factor this out.
+    @modal.method()
+    def calculate_embeddings(  # type: ignore
         self,
-        embeddings_dir: str,
-        metadata_path: str,
-        embedding_generator: str,
-        distance_metric: str,
-        id_column_name: str,
-    ):
-        self._distance_metric = distance_metric
-        self._id_column_name = id_column_name
-        self._metadata_filepath = self._get_metadata_filepath(metadata_path)
-
-        self._embeddings, self._ids = self._get_embeddings(embeddings_dir)
-        if len(set(self._ids)) != len(self._ids):
-            raise ValueError("Duplicate ids found in the embeddings file.")
-
-        if embedding_generator == "sentence_transformer_L12":
-            self._encoder = SentenceTransformerModel()
-        else:
-            raise ValueError(f"Unknown embedding generator: {embedding_generator}")
-
-    @abc.abstractmethod
-    def _process_query(self, query_embedding, top_k: int = 5) -> tuple:
-        pass
-
-    def process_query(self, query, top_k: int = 5) -> tuple:
-        print("Embedding query...")
-        query_embedding = self._encoder.encode(texts=[query], batch_size=1, show_progress_bar=True)
-
-        return self._process_query(query_embedding, top_k)
-
-    def fetch_metadata(self, ids) -> pd.DataFrame:
-        print("Fetching metadata...")
-
-        data = duckdb.read_csv(self._metadata_filepath)
-        id_str = " OR ".join([f"{self._id_column_name} = {id}" for id in ids])
-        metadata = duckdb.sql(f"SELECT * FROM data WHERE {id_str}").df()
-
-        return metadata
-
-    def _get_embeddings(self, embeddings_dir: str):
-        if not is_s3_uri(embeddings_dir):
-            return self._load_embeddings(embeddings_dir)
-
-        print("[bold]Downloading calculated embeddings...[/bold]")
-        with S3Folder(embeddings_dir) as tmp_local_embeddings_dir:
-            return self._load_embeddings(tmp_local_embeddings_dir)
-
-    def _load_embeddings(self, embeddings_dir: str) -> tuple:
-        """Loads and preprocesses the embeddings from a parquet file."""
-        assert os.path.exists(embeddings_dir)
-
-        print("[bold]Loading embeddings from parquet file...[/bold]")
-        df = pd.read_parquet(embeddings_dir, "pyarrow")
-
-        print("[bold]Converting embeddings to numpy array...[/bold]")
-        embeddings = np.array(df["embeddings"].values.tolist()).astype("float32")
-        ids = np.array(df["ids"].values.tolist()).astype("int64")
-        return embeddings, ids
-
-    def _get_metadata_filepath(self, metadata_path: str) -> str:
-        if not is_s3_uri(metadata_path):
-            return metadata_path
-
-        print("[bold]Downloading metadata file...[/bold]")
-        self._metadata_fileref = S3File(metadata_path)
-        return self._metadata_fileref.download()
-
-    def cleanup(self):
-        if is_s3_uri(self._metadata_path):
-            self._metadata_fileref.cleanup()
+        ids: list,
+        output_path: str,
+        texts: Optional[list] = None,
+        audio_paths: Optional[list] = None,
+        image_paths: Optional[list] = None,
+        show_progress_bar: bool = False,
+    ) -> Union[None, pa.Table]:
+        return super().calculate_embeddings(
+            ids=ids,
+            output_path=output_path,
+            texts=texts,
+            audio_paths=audio_paths,
+            image_paths=image_paths,
+            show_progress_bar=show_progress_bar,
+        )
+
+
+# We have a function here instead of putting it into __main__ so that `modal shell` works
+@sbert_stub.function(image=image)
+def test(s3_bucket_path: str):
+    st = SentenceTransformerEmbedder()
+    embeddings = st.calculate_embeddings.call(
+        texts=["hello", "world"],
+        ids=[1, 2],
+        output_path=s3_bucket_path,
+        show_progress_bar=True,
+    )
+
+
+if __name__ == "__main__":
+    # Run as "python sentence_transformer.py s3://<bucket_name>/test_mainfn/"
+    import sys
 
-        if is_s3_uri(self._embeddings_dir):
-            self._embeddings_dir.cleanup()
+    with sbert_stub.run():
+        test.call(sys.argv[1])
```

### Comparing `peachdb-0.0.9/peachdb/backends/numpy_backend.py` & `peachdb-0.1.0/peachdb/backends/numpy_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,31 +41,31 @@
     """
     query_embed, embeds = _check_dims(query_embed, embeds)
 
     return (1 - (query_embed @ embeds.T) / (np.linalg.norm(query_embed, axis=1) * np.linalg.norm(embeds, axis=1)))[0]
 
 
 class NumpyBackend(BackendBase):
-    def _process_query(self, query_embedding, top_k: int = 5):
+    def _process_query(self, query_embedding, top_k: int = 5) -> tuple:
         """Compute query embedding, calculate distance of query embedding and get top k."""
         print("Calculating distances...")
         distances = (
             l2(query_embedding, self._embeddings)
             if self._distance_metric == "l2"
             else cosine(query_embedding, self._embeddings)
         )
 
         print("Getting top results...")
         results = np.argsort(distances)[:top_k]
         return self._ids[results], distances[results]
 
 
 if __name__ == "__main__":
-    import scipy.spatial.distance as scipy_distance
-    from sentence_transformers.util import cos_sim as st_cos_sim
+    import scipy.spatial.distance as scipy_distance  # type: ignore
+    from sentence_transformers.util import cos_sim as st_cos_sim  # type: ignore
 
     for dim in [3, 384, 1536]:
         a = np.random.rand(dim)
         b = np.random.rand(3, dim)
 
         # cosine
         cosine_result = cosine(a, b)
```

### Comparing `peachdb-0.0.9/peachdb/backends/torch_backend.py` & `peachdb-0.1.0/peachdb/backends/torch_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import torch
 
-from peachdb.backends.backend_base import BackendBase
+from peachdb.backends.backend_base import BackendBase, BackendConfig
+from peachdb.embedder.utils import Modality
 
 
 def _check_dims(query_embed: torch.Tensor, embeds: torch.Tensor):
     if query_embed.dim() == 1:
         query_embed = query_embed.unsqueeze(0)
     elif query_embed.dim() == 2:
         if query_embed.size(0) != 1:
@@ -42,34 +43,26 @@
         / (torch.norm(query_embed, dim=1).unsqueeze(1) * torch.norm(embeds, dim=1).unsqueeze(0))
     )[0]
 
 
 class TorchBackend(BackendBase):
     def __init__(
         self,
-        embeddings_dir: str,
-        metadata_path: str,
-        embedding_generator: str,
-        distance_metric: str,
-        id_column_name: str,
+        backend_config: BackendConfig,
     ):
         if not torch.cuda.is_available():
             raise RuntimeError("CUDA is required to use TorchDB")
 
         super().__init__(
-            embeddings_dir=embeddings_dir,
-            metadata_path=metadata_path,
-            embedding_generator=embedding_generator,
-            distance_metric=distance_metric,
-            id_column_name=id_column_name,
+            backend_config=backend_config,
         )
         self.device = torch.device("cuda")
         self._embeddings = torch.from_numpy(self._embeddings).to(self.device)  # Ensure the tensor is on the GPU
 
-    def _process_query(self, query_embedding, top_k: int = 5):
+    def _process_query(self, query_embedding, top_k: int = 5) -> tuple:
         """Compute query embedding, calculate distance of query embedding and get top k."""
         query_embedding = torch.from_numpy(query_embedding).to(self.device)
 
         print("Calculating distances...")
         distances = (
             l2(query_embedding, self._embeddings)
             if self._distance_metric == "l2"
@@ -78,16 +71,16 @@
 
         print("Getting top results...")
         results = torch.argsort(distances)[:top_k].cpu().numpy()
         return self._ids[results], distances[results].cpu().numpy()
 
 
 if __name__ == "__main__":
-    import scipy.spatial.distance as scipy_distance
-    from sentence_transformers.util import cos_sim as st_cos_sim
+    import scipy.spatial.distance as scipy_distance  # type: ignore
+    from sentence_transformers.util import cos_sim as st_cos_sim  # type: ignore
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     for dim in [3, 384, 1536]:
         a = torch.rand(dim, device=device)
         b = torch.rand(3, dim, device=device)
```

### Comparing `peachdb-0.0.9/peachdb/embedder/__init__.py` & `peachdb-0.1.0/peachdb/embedder/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,68 @@
-import asyncio
 import os
 import shutil
 from collections import namedtuple
-from typing import List, Optional
+from typing import List, Optional, Type
 
 import duckdb
-import pyarrow.parquet as pq
+import pyarrow.parquet as pq  # type: ignore
 from rich import print
 
+import peachdb.embedder.containers.base
 from peachdb.constants import BLOB_STORE
-from peachdb.embedder.utils import S3File, is_s3_uri
+from peachdb.embedder.utils import Modality, S3File, is_s3_uri
 
-Chunk = namedtuple("Chunk", ["texts", "ids"])
+Chunk = namedtuple("Chunk", ["texts_or_paths", "ids"])
 
 
 # TODO: split into two separate classes LocalEmbeddingsProcessor & S3EmbeddingsProcessor
 class EmbeddingProcessor:
     def __init__(
         self,
         csv_path: str,
         column_to_embed: str,
         id_column_name: str,
         embedding_model_name: str,
         project_name: str,
-        s3_bucket: Optional[str] = None,
+        modality: Modality,
+        embeddings_output_s3_bucket_uri: Optional[str] = None,
         max_rows: Optional[int] = None,
     ):
         self._csv_path = csv_path
         self._column_to_embed = column_to_embed
         self._id_column_name = id_column_name
         self._embedding_model_name = embedding_model_name
         self._max_rows = max_rows
         self._project_name = project_name
-        self._s3_bucket = s3_bucket.strip("/") + "/" if s3_bucket else None
+        self._embeddings_output_s3_bucket_uri = (
+            embeddings_output_s3_bucket_uri.strip("/") + "/" if embeddings_output_s3_bucket_uri else None
+        )
+        self._modality = modality
 
         if self._embedding_model_name == "sentence_transformer_L12":
             from peachdb.embedder.containers.sentence_transformer import SentenceTransformerEmbedder, sbert_stub
 
-            self._embedding_model = SentenceTransformerEmbedder
+            self._embedding_model: Type[
+                peachdb.embedder.containers.base.EmbeddingModelBase
+            ] = SentenceTransformerEmbedder
             self._embedding_model_stub = sbert_stub
             self._embedding_model_chunk_size = 10000
+        elif self._embedding_model_name == "imagebind":
+            from peachdb.embedder.containers.multimodal_imagebind import ImageBindEmbdedder, imagebind_stub
+
+            self._embedding_model = ImageBindEmbdedder
+            self._embedding_model_stub = imagebind_stub
+            self._embedding_model_chunk_size = 1000
         else:
             raise ValueError(f"Invalid embedding model name: {self._embedding_model_name}")
 
     @property
     def embeddings_output_dir(self):
         if is_s3_uri(self._csv_path):
-            return f"s3://{self._s3_bucket}{self._project_name}/embeddings"
+            return f"{self._embeddings_output_s3_bucket_uri}{self._project_name}/embeddings"
 
         dir = f"{BLOB_STORE}/{self._project_name}/embeddings"
         os.makedirs(dir, exist_ok=True)
         return dir
 
     def process(self):
         dataset = self._download_and_read_dataset(self._csv_path)
@@ -60,14 +72,15 @@
 
         print("[bold]Running embedding model on each chunk in parallel...[/bold]")
         self._run_model(chunked_data)
 
     def _download_and_read_dataset(self, csv_path: str) -> str:
         """Supports a local/s3 reference to the csv formatted dataset"""
         if not is_s3_uri(self._csv_path):
+            print("[bold]Loading data into memory...[/bold]")
             # local ref has been provided. make a copy within .peachdb for persistence
             project_blob_dir = f"{BLOB_STORE}/{self._project_name}"
             os.makedirs(project_blob_dir, exist_ok=True)
 
             fname = self._csv_path.split("/")[-1]
             dataset_path = f"{project_blob_dir}/{fname}"
             shutil.copy2(self._csv_path, dataset_path)
@@ -75,53 +88,55 @@
         else:
             print("[bold]Downloading data from S3...[/bold]")
             with S3File(self._csv_path) as downloaded_dataset:
                 print("[bold]Loading data into memory...[/bold]")
                 return self._read_dataset(downloaded_dataset)
 
     def _read_dataset(self, dataset_path: str):
-        # TODO: implement audio/image support. (#multimodality)
-        data = duckdb.read_csv(dataset_path)
+        data = duckdb.read_csv(dataset_path, header=True)
         sql_query = f"SELECT {self._column_to_embed}, {self._id_column_name} FROM data"
         if self._max_rows:
             sql_query += f" LIMIT {self._max_rows}"
         return duckdb.sql(sql_query).fetchall()  # NOTE: takes 2 mins 10 seconds for a large dataset
 
     def _chunk_data(self, fetched_data) -> List[Chunk]:
         chunk_size = self._embedding_model_chunk_size
         chunked_data = [fetched_data[i : i + chunk_size] for i in range(0, len(fetched_data), chunk_size)]
         print(f"[bold]...{len(fetched_data)} rows were split into {len(chunked_data)} chunks[/bold]")
 
         inputs = []
 
         for chunk in chunked_data:
-            texts = []
+            texts_or_paths = []
             ids = []
-            for text, id in chunk:
-                texts.append(text)
+            for text_or_path, id in chunk:
+                texts_or_paths.append(text_or_path)
                 ids.append(id)
-            inputs += [Chunk(texts, ids)]
+            inputs += [Chunk(texts_or_paths, ids)]
 
         return inputs
 
     def _run_model(self, chunks: List[Chunk]):
         with self._embedding_model_stub.run():
             st = self._embedding_model()
 
             fname = self._csv_path.split("/")[-1].split(".")[0]
             input_tuples = [
-                # expected: (texts, ids, output_path, show_progress)
+                # expected: (ids, output_path, texts, audio_paths, image_paths, show_progress)
                 (
-                    chunk.texts,
                     chunk.ids,
                     f"{self.embeddings_output_dir}/{fname}_{idx}_{self._embedding_model_name}.parquet",
+                    # TODO: enable support of using multiple modalities at the same time here (#multi-modality)
+                    chunk.texts_or_paths if self._modality == Modality.TEXT else None,
+                    chunk.texts_or_paths if self._modality == Modality.AUDIO else None,
+                    chunk.texts_or_paths if self._modality == Modality.IMAGE else None,
                     True,
                 )
                 for idx, chunk in enumerate(chunks)
             ]
-            results = list(st.calculate_embeddings.starmap(input_tuples))
+            results = list(st.calculate_embeddings.starmap(input_tuples))  # type: ignore
 
             if not is_s3_uri(self._csv_path):
                 for idx, result in enumerate(results):
                     pq.write_table(
                         result, f"{self.embeddings_output_dir}/{fname}_{idx}_{self._embedding_model_name}.parquet"
                     )
```

### Comparing `peachdb-0.0.9/peachdb.egg-info/PKG-INFO` & `peachdb-0.1.0/peachdb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.9
+Version: 0.1.0
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PeachDB
 
 <h3 align="center"><strong>PeachDB - the AI-First, Embeddings Database</strong></h3>
 <h4 align="center">Build memory for your AI products in <strong>minutes!</strong></h4>
 
 <br/>
 
-**Our core API has 3 functions**
+**Our core API has 4 functions**
 
 ```python
 from peachdb import PeachDB
 
-# Create a new PeachDB instance
-# Embeddings are automatically computed at scale using the selected `embedding_generator` model on Modal.
-db = PeachDB.create(
+# Create a new PeachDB instance or reference an existing one
+db = PeachDB(
     project_name="my_app",
+    embedding_generator="imagebind",  # "imagebind" or "sentence_transformer_L12"
+    embedding_backend="exact_cpu",  # "exact_cpu", "exact_gpu", or "approx"
+    distance_metric="cosine",  # "cosine" or "l2"
+)
+
+# Auto-compute & upsert embeddings at scale using the specified `embedding_generator` model on Modal
+db.upsert_text(  # or "upsert_image" or "upsert_audio"
     csv_path="/path/to/local/csv",  # or "s3://path/to/csv"
-    column_to_embed="foo",
+    column_to_embed="foo",  # column values can either be string or public URI to image/audio
     id_column_name="id",
-    max_rows=None, # or N, to process N rows of the dataset 
-    distance_metric="cosine",  # or "l2"
-    embedding_backend="exact_cpu",  # or "exact_gpu" or "approx"
-    embedding_generator="sentence_transformer_L12",
-    embeddings_output_s3_bucket_uri=None, # required when using S3 URI for `csv_path`
+    embeddings_output_s3_bucket_uri=None,  # required when using S3 URI for `csv_path`
+    max_rows=None,  # or N to process N rows
 )
-# Once the database has been successfully setup, you can reference it in the future via
-# db = PeachDB(project_name="my_app")
 
-# Query/search 5 most similar results
-results_df = db.query(text='An example query', top_k=5)
+# Query top 5 similar results
+ids, distances, results_df = db.query(
+    query_input='An example query',  # or path to an image/audio file
+    modality='text',  # "text", "image", or "audio"
+    top_k=5
+)
 
-# Deploy the database as a publicly available FastAPI server
-# Call GET /query?text='An example query'&top_k=5 to fetch 5 most similar results
+# Deploy database as a publicly accessible FastAPI server
+# GET /query?query_input='An example query'&modality=[text|image|audio]&top_k=5 to fetch 5 most similar results
 db.deploy()
 ```
 
 ## Why another embedding database?
 We've streamlined the entire end-to-end process of creating, storing, and retrieving embeddings, making it developer-friendly, seamless, and cost-effective. You no longer have to build custom pipelines or fret over hardware setups & scalability issues. PeachDB ensures you can get started within minutes, leaving the worries of cost optimization and scale to us.
 
 Our key features include:
 * **Automated, cost-effective & large-scale embedding computation**: We leverage serverless GPU functions (through [Modal](https://modal.com/)) to compute embeddings on a large scale efficiently and affordably.
     - For instance, we processed the [Kaggle 5M song lyrics dataset](https://www.kaggle.com/datasets/nikhilnayak123/5-million-song-lyrics-dataset?resource=download&select=ds2.csv) in just *12 minutes at a cost of $4.90*, using sentence transformers!
-    - We've developed a Modal wrapper for [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2).
-        - *Coming soon*: Modal wrappers for open-source embedding models such as [ImageBind](https://github.com/facebookresearch/ImageBind), [OpenCLIP](https://github.com/mlfoundations/open_clip), and more.
-        - *Coming soon*: Support for multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
+    - We've developed Modal wrappers for:
+        - [Sentence Transformer L12](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2)
+        - [ImageBind](https://github.com/facebookresearch/ImageBind),
+        - *Coming soon*, support for:
+            - Open-source embedding models such as [OpenCLIP](https://github.com/mlfoundations/open_clip), [Microsoft E5-v2](https://arxiv.org/pdf/2212.03533.pdf), and more.
+            - Multi-threaded [OpenAI](https://platform.openai.com/docs/guides/embeddings) embedding calculation.
     - *Coming soon*: Bring your own embeddings.
     - *Coming soon*: Custom embedding functions for even more flexibility.
 * **Multimodality**: Native support for data with mixture of modalities (such as image/audio/video).
 * **Highly Customizable**: PeachDB allows you to tailor its features to your needs. You can customize:
     - Embedding computation: as described above.
     - Backend: choose between `exact_cpu` (numpy), `exact_gpu` (torch), or `approx` (HNSW).
     - Distance metrics: `cosine` or `l2`.
@@ -75,53 +83,46 @@
 - Create & activate a new conda environment `conda create -n spoti_vibe python=3.10` & `conda activate spoti_vibe`
 - Install PeachDB: `pip install peachdb`
 - Setup [Modal](https://modal.com)
     - Create an account at [modal.com](https://modal.com)
     - Install the modal-client package: `pip install modal-client`
     - Setup token: `modal token new`
 
-- (optional) PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, create & configure your .env file as below.
-    ```python
-    # Fetch the below values from ~/.aws/credentials
-    AWS_ACCESS_KEY_ID=
-    AWS_SECRET_ACCESS_KEY=
-    ```
-    Please ensure the credentials have read & write access to the relevant bucket you plan to use.
+- (optional: for AWS S3) PeachDB accepts local & S3 paths to datasets for embedding computation. To use S3 URIs, ensure you've installed the `aws` cli and run `aws configure`. The credentials should have read & write access to the relevant bucket you plan to use.
 - `mkdir spoti_vibe/`
 - Create a new module inside the directory `server.py`
 - Add the following code
     ```python
     from peachdb import PeachDB
 
     import os
+
     # Fetch the username & key by creating a new API token at https://www.kaggle.com/settings
-    os.environ['KAGGLE_USERNAME'] = None # set user name
-    os.environ['KAGGLE_KEY'] = None # set key
+    os.environ["KAGGLE_USERNAME"] = None  # set user name
+    os.environ["KAGGLE_KEY"] = None  # set key
 
-    import kaggle # make sure you've run `pip install kaggle`
+    import kaggle  # make sure you've run `pip install kaggle`
 
     kaggle.api.authenticate()
-    kaggle.api.dataset_download_files(
-        'nikhilnayak123/5-million-song-lyrics-dataset',
-        path='.',
-        unzip=True
-    )
+    # It can take a few mins to download depending on the network speed
+    kaggle.api.dataset_download_files("nikhilnayak123/5-million-song-lyrics-dataset", path=".", unzip=True)
 
-    db = PeachDB.create(
+    db = PeachDB(
         project_name="spoti_vibe",
-        csv_path='./ds2.csv',  # dataset name as observed on Kaggle
-        column_to_embed="lyrics",
-        id_column_name="id",
-        max_rows=None,
         distance_metric="cosine",
         embedding_backend="exact_cpu",
         embedding_generator="sentence_transformer_L12",
     )
+    db.upsert_text(
+        csv_path="./ds2.csv",  # dataset name as observed on Kaggle
+        column_to_embed="lyrics",
+        id_column_name="id",
+    )
 
-    db.deploy() # Public URL will be printed to console
+    db.deploy()  # Public URL will be printed to console
     ```
 
 And that's it! You should now have a publicly available server that can listen to query requests from the user on: <br/>
 `GET <PUBLIC_URL>/query?text='Happy, upbeat summer'&top_k=5`
 
 ## Use-cases
 - Build web apps like - [clip.audio](https://www.clip.audio/) & [awesome-movies.life](https://awesome-movies.life/)
```

### Comparing `peachdb-0.0.9/peachdb.egg-info/SOURCES.txt` & `peachdb-0.1.0/peachdb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 peachdb/__init__.py
 peachdb/constants.py
+peachdb/validators.py
 peachdb.egg-info/PKG-INFO
 peachdb.egg-info/SOURCES.txt
 peachdb.egg-info/dependency_links.txt
 peachdb.egg-info/requires.txt
 peachdb.egg-info/top_level.txt
 peachdb/backends/__init__.py
 peachdb/backends/backend_base.py
 peachdb/backends/hnsw_backend.py
 peachdb/backends/numpy_backend.py
 peachdb/backends/torch_backend.py
 peachdb/embedder/__init__.py
 peachdb/embedder/utils.py
 peachdb/embedder/containers/__init__.py
 peachdb/embedder/containers/base.py
+peachdb/embedder/containers/multimodal_imagebind.py
 peachdb/embedder/containers/sentence_transformer.py
 peachdb/embedder/models/__init__.py
 peachdb/embedder/models/base.py
+peachdb/embedder/models/multimodal_imagebind.py
 peachdb/embedder/models/sentence_transformer.py
```

### Comparing `peachdb-0.0.9/setup.py` & `peachdb-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
 
-from setuptools import find_packages, setup
+from setuptools import find_packages, setup  # type: ignore
 
 requirements = []
 
 # Read requirements from files
 with open("requirements.txt", "r") as f:
     requirements.extend(f.read().splitlines())
 
 # read the contents README
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="peachdb",
-    version="0.0.9",
+    version="0.1.0",
     packages=find_packages(),
     install_requires=requirements,
     dependency_links=["https://download.pytorch.org/whl/cu113"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     project_urls={
```

