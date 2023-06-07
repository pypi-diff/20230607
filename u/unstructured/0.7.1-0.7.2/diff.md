# Comparing `tmp/unstructured-0.7.1.tar.gz` & `tmp/unstructured-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.1.tar", last modified: Thu Jun  1 20:53:22 2023, max compression
+gzip compressed data, was "unstructured-0.7.2.tar", last modified: Wed Jun  7 18:12:05 2023, max compression
```

## Comparing `unstructured-0.7.1.tar` & `unstructured-0.7.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-01 20:53:14.000000 unstructured-0.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-01 20:53:14.000000 unstructured-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-06-01 20:53:22.964075 unstructured-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-06-01 20:53:14.000000 unstructured-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-01 20:53:22.968075 unstructured-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-01 20:53:14.000000 unstructured-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.321691 unstructured-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-07 18:11:51.000000 unstructured-0.7.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 18:11:51.000000 unstructured-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-07 18:12:05.321691 unstructured-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-07 18:11:51.000000 unstructured-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 18:12:05.321691 unstructured-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-07 18:11:51.000000 unstructured-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.317691 unstructured-0.7.2/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.321691 unstructured-0.7.2/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.321691 unstructured-0.7.2/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.1/LICENSE.md` & `unstructured-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/PKG-INFO` & `unstructured-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -68,18 +68,18 @@
         		- If you do not need to process PDFs or images, you can run `pip install unstructured`
         - Install the following system dependencies if they are not already available on your system.
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
-        - If you are parsing PDFs, run the following to install the `detectron2` model, which
-          `unstructured` uses for layout detection:
-            - `pip install tensorboard>=2.12.2`
-            - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
+        
+        - If you are parsing PDFs and want to use a model from the [layoutparser model
+          zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-from-the-layoutparser-model-zoo),
+          use the instructions [here](https://github.com/Unstructured-IO/unstructured-inference#detectron2).
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/fake-email.eml")
@@ -94,25 +94,25 @@
         about the library.
         
         | Document Type | Partition Function | Strategies | Table Support | Options |
         | --- | --- | --- | --- | --- |
         | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
         | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
         | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
-        | EPubs (`.epub`) | `partition_epub` | N/A | No | Include Page Breaks |
+        | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-        | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
+        | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
-        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
+        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
         
         
         
         ## :dizzy: Instructions for using the docker image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.1 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.2 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -38,46 +38,46 @@
 currently support python 3.11, please use an older version. - Install the
 Python SDK with `pip install "unstructured[local-inference]"` - If you do not
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
-- If you are parsing PDFs, run the following to install the `detectron2` model,
-which `unstructured` uses for layout detection: - `pip install
-tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
-facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
-should be able to run the following code: ```python from
+- If you are parsing PDFs and want to use a model from the [layoutparser model
+zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-
+from-the-layoutparser-model-zoo), use the instructions [here](https://
+github.com/Unstructured-IO/unstructured-inference#detectron2). At this point,
+you should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
 (filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
 elements])) ``` The following table shows the document types the `unstructured`
 library currently supports. `partition` will recognize each of these document
 types and route the document to the appropriate partitioning function. If you
 already know your document type, you can use the partitioning function listed
 in the table directly. See our [documentation page](https://unstructured-
 io.github.io/unstructured/) for more details about the library. | Document Type
 | Partition Function | Strategies | Table Support | Options | | --- | --- | --
 - | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
 E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
 `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
-N/A | No | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
+N/A | Yes | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
 `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
 | N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
 `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
 Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
-Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
+Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
-Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
-Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include
+Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
+| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.1/README.md` & `unstructured-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 		- If you do not need to process PDFs or images, you can run `pip install unstructured`
 - Install the following system dependencies if they are not already available on your system.
   Depending on what document types you're parsing, you may not need all of these.
     - `libmagic-dev` (filetype detection)
     - `poppler-utils` (images and PDFs)
     - `tesseract-ocr` (images and PDFs)
     - `libreoffice` (MS Office docs)
-- If you are parsing PDFs, run the following to install the `detectron2` model, which
-  `unstructured` uses for layout detection:
-    - `pip install tensorboard>=2.12.2`
-    - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
+
+- If you are parsing PDFs and want to use a model from the [layoutparser model
+  zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-from-the-layoutparser-model-zoo),
+  use the instructions [here](https://github.com/Unstructured-IO/unstructured-inference#detectron2).
 
 At this point, you should be able to run the following code:
 
 ```python
 from unstructured.partition.auto import partition
 
 elements = partition(filename="example-docs/fake-email.eml")
@@ -86,25 +86,25 @@
 about the library.
 
 | Document Type | Partition Function | Strategies | Table Support | Options |
 | --- | --- | --- | --- | --- |
 | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
 | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
 | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
-| EPubs (`.epub`) | `partition_epub` | N/A | No | Include Page Breaks |
+| EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
 | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
 | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
 | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-| Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
+| Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
 | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
 | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
 | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
 | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
-| Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
+| Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
 | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
 | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
 | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
 
 
 
 ## :dizzy: Instructions for using the docker image
```

#### html2text {}

```diff
@@ -34,46 +34,46 @@
 currently support python 3.11, please use an older version. - Install the
 Python SDK with `pip install "unstructured[local-inference]"` - If you do not
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
-- If you are parsing PDFs, run the following to install the `detectron2` model,
-which `unstructured` uses for layout detection: - `pip install
-tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
-facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
-should be able to run the following code: ```python from
+- If you are parsing PDFs and want to use a model from the [layoutparser model
+zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-
+from-the-layoutparser-model-zoo), use the instructions [here](https://
+github.com/Unstructured-IO/unstructured-inference#detectron2). At this point,
+you should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
 (filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
 elements])) ``` The following table shows the document types the `unstructured`
 library currently supports. `partition` will recognize each of these document
 types and route the document to the appropriate partitioning function. If you
 already know your document type, you can use the partitioning function listed
 in the table directly. See our [documentation page](https://unstructured-
 io.github.io/unstructured/) for more details about the library. | Document Type
 | Partition Function | Strategies | Table Support | Options | | --- | --- | --
 - | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
 E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
 `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
-N/A | No | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
+N/A | Yes | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
 `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
 | N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
 `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
 Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
-Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
+Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
-Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
-Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include
+Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
+| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.1/setup.py` & `unstructured-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.2/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.2/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/test_unstructured/test_utils.py` & `unstructured-0.7.2/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/cleaners/core.py` & `unstructured-0.7.2/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/cleaners/extract.py` & `unstructured-0.7.2/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/cleaners/translate.py` & `unstructured-0.7.2/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/documents/base.py` & `unstructured-0.7.2/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/documents/elements.py` & `unstructured-0.7.2/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/documents/email_elements.py` & `unstructured-0.7.2/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/documents/html.py` & `unstructured-0.7.2/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/documents/xml.py` & `unstructured-0.7.2/unstructured/documents/xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional, Union
 
 from lxml import etree
 
 from unstructured.documents.base import Document, Page
+from unstructured.file_utils.encoding import read_txt_file
 from unstructured.logger import logger
 
 VALID_PARSERS = Union[etree.HTMLParser, etree.XMLParser, None]
 
 
 class XMLDocument(Document):
     """Class for handling .xml documents. This class uses rules based parsing to identify
@@ -100,12 +101,11 @@
 
     @classmethod
     def from_file(
         cls,
         filename,
         parser: VALID_PARSERS = None,
         stylesheet: Optional[str] = None,
-        encoding: Optional[str] = "utf-8",
+        encoding: Optional[str] = None,
     ):
-        with open(filename, encoding=encoding) as f:
-            content = f.read()
+        _, content = read_txt_file(filename=filename, encoding=encoding)
         return cls.from_string(content, parser=parser, stylesheet=stylesheet)
```

### Comparing `unstructured-0.7.1/unstructured/file_utils/encoding.py` & `unstructured-0.7.2/unstructured/file_utils/encoding.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import IO, Optional, Tuple
+from typing import IO, Optional, Tuple, Union
 
 import chardet
 
 ENCODE_REC_THRESHOLD = 0.5
 
 # popular encodings from https://en.wikipedia.org/wiki/Popularity_of_text_encodings
 COMMON_ENCODINGS = [
@@ -23,28 +23,34 @@
     "gb18030",
     "shift_jis",
     "shift_jis_2004",
     "shift_jisx0213",
 ]
 
 
-def detect_file_encoding(filename: str = "", file: Optional[IO] = None) -> Tuple[str, str]:
+def detect_file_encoding(
+    filename: str = "",
+    file: Optional[Union[bytes, IO]] = None,
+) -> Tuple[str, str]:
     if filename:
         with open(filename, "rb") as f:
-            binary_data = f.read()
+            byte_data = f.read()
     elif file:
-        if "b" in file.mode:
-            binary_data = file.read()
+        if isinstance(file, bytes):
+            byte_data = file
         else:
-            with open(file.name, "rb") as f:
-                binary_data = f.read()
+            if not hasattr(file, "mode") or "b" in file.mode:
+                byte_data = file.read()
+            else:
+                with open(file.name, "rb") as f:
+                    byte_data = f.read()
     else:
         raise FileNotFoundError("No filename nor file were specified")
 
-    result = chardet.detect(binary_data)
+    result = chardet.detect(byte_data)
     encoding = result["encoding"]
     confidence = result["confidence"]
 
     if encoding is None or confidence < ENCODE_REC_THRESHOLD:
         # Encoding detection failed, fallback to predefined encodings
         for enc in COMMON_ENCODINGS:
             try:
@@ -54,29 +60,29 @@
                 break
             except (UnicodeDecodeError, UnicodeError):
                 continue
         else:
             raise UnicodeDecodeError(
                 "Unable to determine the encoding of the file or match it with any "
                 "of the specified encodings.",
-                binary_data,
+                byte_data,
                 0,
-                len(binary_data),
+                len(byte_data),
                 "Invalid encoding",
             )
 
     else:
-        file_text = binary_data.decode(encoding)
+        file_text = byte_data.decode(encoding)
 
     return encoding, file_text
 
 
 def read_txt_file(
     filename: str = "",
-    file: Optional[IO] = None,
+    file: Optional[Union[bytes, IO]] = None,
     encoding: Optional[str] = None,
 ) -> Tuple[str, str]:
     """Extracts document metadata from a plain text document."""
     if filename:
         if encoding:
             with open(filename, encoding=encoding) as f:
                 try:
@@ -84,15 +90,15 @@
                 except (UnicodeDecodeError, UnicodeError) as error:
                     raise error
         else:
             encoding, file_text = detect_file_encoding(filename)
     elif file:
         if encoding:
             try:
-                file_content = file.read()
+                file_content = file if isinstance(file, bytes) else file.read()
                 if isinstance(file_content, bytes):
                     file_text = file_content.decode(encoding)
                 else:
                     file_text = file_content
             except (UnicodeDecodeError, UnicodeError) as error:
                 raise error
         else:
```

### Comparing `unstructured-0.7.1/unstructured/file_utils/exploration.py` & `unstructured-0.7.2/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.2/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/file_utils/filetype.py` & `unstructured-0.7.2/unstructured/file_utils/filetype.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,18 +156,39 @@
     ".ppt": FileType.PPT,
     ".rtf": FileType.RTF,
     ".json": FileType.JSON,
     ".epub": FileType.EPUB,
     ".msg": FileType.MSG,
     ".odt": FileType.ODT,
     ".csv": FileType.CSV,
+    # NOTE(robinson) - for now we are treating code files as plain text
+    ".js": FileType.TXT,
+    ".py": FileType.TXT,
+    ".java": FileType.TXT,
+    ".cpp": FileType.TXT,
+    ".cc": FileType.TXT,
+    ".cxx": FileType.TXT,
+    ".c": FileType.TXT,
+    ".cs": FileType.TXT,
+    ".php": FileType.TXT,
+    ".rb": FileType.TXT,
+    ".swift": FileType.TXT,
+    ".ts": FileType.TXT,
+    ".go": FileType.TXT,
     None: FileType.UNK,
 }
 
 
+def _resolve_symlink(file_path):
+    # Resolve the symlink to get the actual file path
+    if os.path.islink(file_path):
+        file_path = os.path.realpath(file_path)
+    return file_path
+
+
 def detect_filetype(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
 ) -> Optional[FileType]:
     """Use libmagic to determine a file's type. Helps determine which partition brick
@@ -181,15 +202,18 @@
             return filetype
 
     if filename or file_filename:
         _filename = filename or file_filename or ""
         _, extension = os.path.splitext(_filename)
         extension = extension.lower()
         if os.path.isfile(_filename) and LIBMAGIC_AVAILABLE:
-            mime_type = magic.from_file(filename or file_filename, mime=True)  # type: ignore
+            mime_type = magic.from_file(
+                _resolve_symlink(filename or file_filename),
+                mime=True,
+            )  # type: ignore
         else:
             return EXT_TO_FILETYPE.get(extension.lower(), FileType.UNK)
 
     elif file is not None:
         extension = None
         # NOTE(robinson) - the python-magic docs recommend reading at least the first 2048 bytes
         # Increased to 4096 because otherwise .xlsx files get detected as a zip file
@@ -261,14 +285,20 @@
 
         extension = extension if extension else ""
         if filetype == FileType.UNK:
             return EXT_TO_FILETYPE.get(extension.lower(), FileType.ZIP)
         else:
             return EXT_TO_FILETYPE.get(extension.lower(), filetype)
 
+    elif _is_code_mime_type(mime_type):
+        # NOTE(robinson) - we'll treat all code files as plain text for now.
+        # we can update this logic and add filetypes for specific languages
+        # later if needed.
+        return FileType.TXT
+
     # For everything else
     elif mime_type in STR_TO_FILETYPE:
         return STR_TO_FILETYPE[mime_type]
 
     logger.warning(
         f"The MIME type{f' of {filename!r}' if filename else ''} is {mime_type!r}. "
         "This file type is not currently supported in unstructured.",
@@ -359,14 +389,40 @@
         elements,
         include_page_breaks=include_page_breaks,
         filetype=filetype,
     )
     return elements
 
 
+PROGRAMMING_LANGUAGES = [
+    "javascript",
+    "python",
+    "java",
+    "c++",
+    "cpp",
+    "csharp",
+    "c#",
+    "php",
+    "ruby",
+    "swift",
+    "typescript",
+]
+
+
+def _is_code_mime_type(mime_type: str) -> bool:
+    """Checks to see if the MIME type is a MIME type that would be used for a code
+    file."""
+    mime_type = mime_type.lower()
+    # NOTE(robinson) - check this one explicitly to avoid conflicts with other
+    # MIME types that contain "go"
+    if mime_type == "text/x-go":
+        return True
+    return any(language in mime_type for language in PROGRAMMING_LANGUAGES)
+
+
 def add_metadata_with_filetype(filetype: FileType):
     def decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
             elements = func(*args, **kwargs)
             sig = inspect.signature(func)
             params = dict(**dict(zip(sig.parameters, args)), **kwargs)
```

### Comparing `unstructured-0.7.1/unstructured/file_utils/metadata.py` & `unstructured-0.7.2/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/azure.py` & `unstructured-0.7.2/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.2/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/discord.py` & `unstructured-0.7.2/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.2/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/git.py` & `unstructured-0.7.2/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/github.py` & `unstructured-0.7.2/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.2/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.2/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/local.py` & `unstructured-0.7.2/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.2/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/s3.py` & `unstructured-0.7.2/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/slack.py` & `unstructured-0.7.2/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.2/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.2/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/interfaces.py` & `unstructured-0.7.2/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/ingest/main.py` & `unstructured-0.7.2/unstructured/ingest/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import collections
 import hashlib
 import logging
 import multiprocessing as mp
 import sys
 import warnings
 from contextlib import suppress
 from functools import partial
@@ -92,14 +93,15 @@
         ) as pool:
             pool.map(self.doc_processor_fn, docs)
 
         self.cleanup()
 
 
 @click.command()
+@click.pass_context
 @click.option(
     "--max-docs",
     default=None,
     type=int,
     help="If specified, process at most specified number of documents.",
 )
 @click.option(
@@ -388,14 +390,15 @@
     "--num-processes",
     default=2,
     show_default=True,
     help="Number of parallel processes to process docs in.",
 )
 @click.option("-v", "--verbose", is_flag=True, default=False)
 def main(
+    ctx,
     remote_url,
     s3_anonymous,
     azure_account_name,
     azure_account_key,
     azure_connection_string,
     drive_id,
     drive_service_account_key,
@@ -441,14 +444,18 @@
     partition_endpoint,
     partition_strategy,
     local_input_path,
     local_recursive,
     local_file_glob,
     download_only,
 ):
+    default_values = collections.Counter([option.default for option in ctx.command.params])
+    passed_values = collections.Counter(ctx.params.values())
+    if default_values == passed_values:
+        return click.echo(ctx.get_help())
     if flatten_metadata and "metadata" not in fields_include:
         logger.warning(
             "`--flatten-metadata` is specified, but there is no metadata to flatten, "
             "since `metadata` is not specified in `--fields-include`.",
         )
     if "metadata" not in fields_include and (metadata_include or metadata_exclude):
         logger.warning(
```

### Comparing `unstructured-0.7.1/unstructured/nlp/english-words.txt` & `unstructured-0.7.2/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/nlp/english_words.py` & `unstructured-0.7.2/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/nlp/patterns.py` & `unstructured-0.7.2/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/nlp/tokenize.py` & `unstructured-0.7.2/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/__init__.py` & `unstructured-0.7.2/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/api.py` & `unstructured-0.7.2/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/auto.py` & `unstructured-0.7.2/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "auto",
-    encoding: str = "utf-8",
+    encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     ocr_languages: str = "eng",
     pdf_infer_table_structure: bool = False,
     xml_keep_tags: bool = False,
 ):
@@ -153,15 +153,14 @@
         )
     elif filetype == FileType.PDF:
         elements = partition_pdf(
             filename=filename,  # type: ignore
             file=file,  # type: ignore
             url=None,
             include_page_breaks=include_page_breaks,
-            encoding=encoding,
             infer_table_structure=pdf_infer_table_structure,
             strategy=strategy,
             ocr_languages=ocr_languages,
         )
     elif (filetype == FileType.PNG) or (filetype == FileType.JPG):
         elements = partition_image(
             filename=filename,  # type: ignore
```

### Comparing `unstructured-0.7.1/unstructured/partition/common.py` & `unstructured-0.7.2/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/csv.py` & `unstructured-0.7.2/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/doc.py` & `unstructured-0.7.2/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/docx.py` & `unstructured-0.7.2/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/email.py` & `unstructured-0.7.2/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/epub.py` & `unstructured-0.7.2/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/html.py` & `unstructured-0.7.2/unstructured/partition/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import IO, Dict, List, Optional
 
 import requests
 
 from unstructured.documents.elements import Element
 from unstructured.documents.html import HTMLDocument
 from unstructured.documents.xml import VALID_PARSERS
+from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.file_conversion import convert_file_to_html_text
 from unstructured.file_utils.filetype import (
     FileType,
     add_metadata_with_filetype,
     document_to_element_list,
 )
 from unstructured.partition.common import (
@@ -58,27 +59,19 @@
     """
     if text is not None and text.strip() == "" and not file and not filename and not url:
         return []
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text, url=url)
 
-    if not encoding:
-        encoding = "utf-8"
-
     if filename is not None:
         document = HTMLDocument.from_file(filename, parser=parser, encoding=encoding)
 
     elif file is not None:
-        file_content = file.read()
-        if isinstance(file_content, bytes):
-            file_text = file_content.decode(encoding)
-        else:
-            file_text = file_content
-
+        _, file_text = read_txt_file(file=file, encoding=encoding)
         document = HTMLDocument.from_string(file_text, parser=parser)
 
     elif text is not None:
         _text: str = str(text)
         document = HTMLDocument.from_string(_text, parser=parser)
 
     elif url is not None:
```

### Comparing `unstructured-0.7.1/unstructured/partition/image.py` & `unstructured-0.7.2/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/json.py` & `unstructured-0.7.2/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/md.py` & `unstructured-0.7.2/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/msg.py` & `unstructured-0.7.2/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/odt.py` & `unstructured-0.7.2/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/pdf.py` & `unstructured-0.7.2/unstructured/partition/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
-    encoding: str = "utf-8",
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
@@ -64,46 +63,42 @@
     infer_table_structure
         Only applicable if `strategy=hi_res`.
         If True, any Table elements that are extracted will also have a metadata field
         named "text_as_html" where the table's text content is rendered into an html string.
         I.e., rows and cells are preserved.
         Whether True or False, the "text" field is always present in any Table element
         and is the text content of the table (no structure).
-    encoding
-        The encoding method used to decode the text input. If None, utf-8 will be used.
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to isntall the appropriate Tesseract language pack.
     """
     exactly_one(filename=filename, file=file)
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         url=url,
         template=template,
         token=token,
         include_page_breaks=include_page_breaks,
         strategy=strategy,
         infer_table_structure=infer_table_structure,
-        encoding=encoding,
         ocr_languages=ocr_languages,
     )
 
 
 def partition_pdf_or_image(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = "https://ml.unstructured.io/",
     template: str = "layout/pdf",
     token: Optional[str] = None,
     is_image: bool = False,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
-    encoding: str = "utf-8",
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     if url is None:
         # TODO(alan): Extract information about the filetype to be processed from the template
         # route. Decoding the routing should probably be handled by a single function designed for
         # that task so as routing design changes, those changes are implemented in a single
@@ -137,15 +132,14 @@
                 )
 
         elif strategy == "fast":
             return _partition_pdf_with_pdfminer(
                 filename=filename,
                 file=spooled_to_bytes_io_if_needed(file),
                 include_page_breaks=include_page_breaks,
-                encoding=encoding,
             )
 
         elif strategy == "ocr_only":
             # NOTE(robinson): Catches file conversion warnings when running with PDFs
             with warnings.catch_warnings():
                 return _partition_pdf_or_image_with_ocr(
                     filename=filename,
@@ -227,15 +221,14 @@
 
 
 @requires_dependencies("pdfminer", "local-inference")
 def _partition_pdf_with_pdfminer(
     filename: str = "",
     file: Optional[BinaryIO] = None,
     include_page_breaks: bool = False,
-    encoding: str = "utf-8",
 ) -> List[Element]:
     """Partitions a PDF using PDFMiner instead of using a layoutmodel. Used for faster
     processing or detectron2 is not available.
 
     Implementation is based on the `extract_text` implemenation in pdfminer.six, but
     modified to support tracking page numbers and working with file-like objects.
 
@@ -244,34 +237,31 @@
     exactly_one(filename=filename, file=file)
     if filename:
         with open_filename(filename, "rb") as fp:
             fp = cast(BinaryIO, fp)
             elements = _process_pdfminer_pages(
                 fp=fp,
                 filename=filename,
-                encoding=encoding,
                 include_page_breaks=include_page_breaks,
             )
 
     elif file:
         fp = cast(BinaryIO, file)
         elements = _process_pdfminer_pages(
             fp=fp,
             filename=filename,
-            encoding=encoding,
             include_page_breaks=include_page_breaks,
         )
 
     return elements
 
 
 def _process_pdfminer_pages(
     fp: BinaryIO,
     filename: str = "",
-    encoding: str = "utf-8",
     include_page_breaks: bool = False,
 ):
     """Uses PDF miner to split a document into pages and process them."""
     elements: List[Element] = []
 
     for i, page in enumerate(extract_pages(fp)):  # type: ignore
         metadata = ElementMetadata(filename=filename, page_number=i + 1)
```

### Comparing `unstructured-0.7.1/unstructured/partition/ppt.py` & `unstructured-0.7.2/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/pptx.py` & `unstructured-0.7.2/unstructured/partition/pptx.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,25 +61,27 @@
         )
 
     elements: List[Element] = []
     metadata_filename = metadata_filename or filename
     metadata = ElementMetadata(filename=metadata_filename)
     num_slides = len(presentation.slides)
     for i, slide in enumerate(presentation.slides):
+        metadata = ElementMetadata(**metadata.to_dict())
         metadata.page_number = i + 1
 
         for shape in _order_shapes(slide.shapes):
             if shape.has_table:
                 table: pptx.table.Table = shape.table
                 html_table = convert_ms_office_table_to_text(table, as_html=True)
                 text_table = convert_ms_office_table_to_text(table, as_html=False)
                 if (text_table := text_table.strip()) != "":
                     metadata = ElementMetadata(
                         filename=metadata_filename,
                         text_as_html=html_table,
+                        page_number=metadata.page_number,
                     )
                     elements.append(Table(text=text_table, metadata=metadata))
                 continue
             if not shape.has_text_frame:
                 continue
             # NOTE(robinson) - avoid processing shapes that are not on the actual slide
             if shape.top < 0 or shape.left < 0:
```

### Comparing `unstructured-0.7.1/unstructured/partition/rtf.py` & `unstructured-0.7.2/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/strategies.py` & `unstructured-0.7.2/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/text.py` & `unstructured-0.7.2/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/text_type.py` & `unstructured-0.7.2/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/xlsx.py` & `unstructured-0.7.2/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/partition/xml.py` & `unstructured-0.7.2/unstructured/partition/xml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import xml.etree.ElementTree as ET
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, Optional, Union, cast
 
+from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text import partition_text
 
 
 def is_leaf(elem):
     return not bool(elem)
@@ -13,22 +14,24 @@
 
 def get_leaf_elements(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     xml_path: str = ".",
 ):
     if filename:
-        tree = ET.parse(filename)
+        _, raw_text = read_txt_file(filename=filename)
     elif file:
         f = spooled_to_bytes_io_if_needed(
             cast(Union[BinaryIO, SpooledTemporaryFile], file),
         )
-        tree = ET.parse(f)  # type: ignore
+        _, raw_text = read_txt_file(file=f)
+    else:
+        raise ValueError("Either 'filename' or 'file' must be provided.")
 
-    root = tree.getroot()
+    root = ET.fromstring(raw_text)
     leaf_elements = []
 
     for elem in root.findall(xml_path):
         for subelem in elem.iter():
             if is_leaf(subelem):
                 leaf_elements.append(subelem.text)
 
@@ -39,15 +42,15 @@
 def partition_xml(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     xml_keep_tags: bool = False,
     xml_path: str = ".",
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
-    encoding: str = "utf-8",
+    encoding: Optional[str] = None,
 ):
     """Partitions an XML document into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
@@ -67,21 +70,22 @@
         elements in the output.
     """
     exactly_one(filename=filename, file=file)
     metadata_filename = metadata_filename or filename
 
     if xml_keep_tags:
         if filename:
-            with open(filename) as f:
-                raw_text = f.read()
+            _, raw_text = read_txt_file(filename=filename, encoding=encoding)
         elif file:
-            f = spooled_to_bytes_io_if_needed(  # type: ignore
+            f = spooled_to_bytes_io_if_needed(
                 cast(Union[BinaryIO, SpooledTemporaryFile], file),
             )
-            raw_text = f.read().decode(encoding)  # type: ignore
+            _, raw_text = read_txt_file(file=f, encoding=encoding)
+        else:
+            raise ValueError("Either 'filename' or 'file' must be provided.")
     else:
         raw_text = get_leaf_elements(filename=filename, file=file, xml_path=xml_path)
     elements = partition_text(
         text=raw_text,
         metadata_filename=metadata_filename,
         include_metadata=include_metadata,
     )
```

### Comparing `unstructured-0.7.1/unstructured/staging/argilla.py` & `unstructured-0.7.2/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/base.py` & `unstructured-0.7.2/unstructured/staging/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,22 +43,23 @@
     return convert_to_isd(elements)
 
 
 def elements_to_json(
     elements: List[Element],
     filename: Optional[str] = None,
     indent: int = 4,
+    encoding: str = "utf-8",
 ) -> Optional[str]:
     """
     Saves a list of elements to a JSON file if filename is specified.
     Otherwise, return the list of elements as a string.
     """
     element_dict = convert_to_dict(elements)
     if filename is not None:
-        with open(filename, "w") as f:
+        with open(filename, "w", encoding=encoding) as f:
             json.dump(element_dict, f, indent=indent)
             return None
     else:
         return json.dumps(element_dict, indent=indent)
 
 
 def isd_to_elements(isd: List[Dict[str, Any]]) -> List[Element]:
@@ -101,20 +102,24 @@
 
 
 def dict_to_elements(element_dict: List[Dict[str, Any]]) -> List[Element]:
     """Converts a dictionary representation of an element list into List[Element]."""
     return isd_to_elements(element_dict)
 
 
-def elements_from_json(filename: str = "", text: str = "") -> List[Element]:
+def elements_from_json(
+    filename: str = "",
+    text: str = "",
+    encoding: str = "utf-8",
+) -> List[Element]:
     """Loads a list of elements from a JSON file or a string."""
     exactly_one(filename=filename, text=text)
 
     if filename:
-        with open(filename) as f:
+        with open(filename, encoding=encoding) as f:
             element_dict = json.load(f)
         return dict_to_elements(element_dict)
     else:
         element_dict = json.loads(text)
         return dict_to_elements(element_dict)
```

### Comparing `unstructured-0.7.1/unstructured/staging/baseplate.py` & `unstructured-0.7.2/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/datasaur.py` & `unstructured-0.7.2/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/huggingface.py` & `unstructured-0.7.2/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/label_box.py` & `unstructured-0.7.2/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/label_studio.py` & `unstructured-0.7.2/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/prodigy.py` & `unstructured-0.7.2/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/staging/weaviate.py` & `unstructured-0.7.2/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured/utils.py` & `unstructured-0.7.2/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.1/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.2/unstructured.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -68,18 +68,18 @@
         		- If you do not need to process PDFs or images, you can run `pip install unstructured`
         - Install the following system dependencies if they are not already available on your system.
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
-        - If you are parsing PDFs, run the following to install the `detectron2` model, which
-          `unstructured` uses for layout detection:
-            - `pip install tensorboard>=2.12.2`
-            - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
+        
+        - If you are parsing PDFs and want to use a model from the [layoutparser model
+          zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-from-the-layoutparser-model-zoo),
+          use the instructions [here](https://github.com/Unstructured-IO/unstructured-inference#detectron2).
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
         elements = partition(filename="example-docs/fake-email.eml")
@@ -94,25 +94,25 @@
         about the library.
         
         | Document Type | Partition Function | Strategies | Table Support | Options |
         | --- | --- | --- | --- | --- |
         | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None |
         | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding |
         | E-mails (`.msg`) | `partition_msg` | N/A | No | Encoding |
-        | EPubs (`.epub`) | `partition_epub` | N/A | No | Include Page Breaks |
+        | EPubs (`.epub`) | `partition_epub` | N/A | Yes | Include Page Breaks |
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
-        | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
+        | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
-        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
+        | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
         
         
         
         ## :dizzy: Instructions for using the docker image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.1 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.2 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -38,46 +38,46 @@
 currently support python 3.11, please use an older version. - Install the
 Python SDK with `pip install "unstructured[local-inference]"` - If you do not
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
-- If you are parsing PDFs, run the following to install the `detectron2` model,
-which `unstructured` uses for layout detection: - `pip install
-tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
-facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
-should be able to run the following code: ```python from
+- If you are parsing PDFs and want to use a model from the [layoutparser model
+zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-
+from-the-layoutparser-model-zoo), use the instructions [here](https://
+github.com/Unstructured-IO/unstructured-inference#detectron2). At this point,
+you should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
 (filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
 elements])) ``` The following table shows the document types the `unstructured`
 library currently supports. `partition` will recognize each of these document
 types and route the document to the appropriate partitioning function. If you
 already know your document type, you can use the partitioning function listed
 in the table directly. See our [documentation page](https://unstructured-
 io.github.io/unstructured/) for more details about the library. | Document Type
 | Partition Function | Strategies | Table Support | Options | | --- | --- | --
 - | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
 E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
 `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
-N/A | No | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
+N/A | Yes | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
 `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
 | N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
 `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
 Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
-Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
+Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
-Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
-Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include
+Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
+| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.1/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.2/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

