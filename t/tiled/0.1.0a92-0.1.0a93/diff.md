# Comparing `tmp/tiled-0.1.0a92.tar.gz` & `tmp/tiled-0.1.0a93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiled-0.1.0a92.tar", last modified: Fri Jun  2 00:30:38 2023, max compression
+gzip compressed data, was "tiled-0.1.0a93.tar", last modified: Wed Jun  7 14:06:01 2023, max compression
```

## Comparing `tiled-0.1.0a92.tar` & `tiled-0.1.0a93.tar`

### file list

```diff
@@ -1,434 +1,434 @@
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.601040 tiled-0.1.0a92/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1538 2023-01-06 15:55:44.000000 tiled-0.1.0a92/LICENSE
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      783 2023-03-22 13:14:07.000000 tiled-0.1.0a92/MANIFEST.in
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-02 00:30:38.601040 tiled-0.1.0a92/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6555 2023-03-16 20:17:15.000000 tiled-0.1.0a92/README.md
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.537040 tiled-0.1.0a92/benchmarks/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/benchmarks/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1065 2023-02-10 13:17:36.000000 tiled-0.1.0a92/benchmarks/benchmarks.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.537040 tiled-0.1.0a92/docs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-01-06 15:55:44.000000 tiled-0.1.0a92/docs/Makefile
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-01-06 15:55:44.000000 tiled-0.1.0a92/docs/make.bat
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.537040 tiled-0.1.0a92/docs/source/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9186 2023-02-10 13:17:36.000000 tiled-0.1.0a92/docs/source/conf.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.537040 tiled-0.1.0a92/docs/source/reference/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    51041 2023-03-31 20:25:00.000000 tiled-0.1.0a92/docs/source/reference/api.yml
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.553040 tiled-0.1.0a92/docs/source/reference/generated/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      554 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      194 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.read_csv.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      722 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1269 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1516 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      741 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1181 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      532 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      510 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.tiff.TiffAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      191 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.xarray.DatasetAdapter.from_dataset.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.ArrayClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.ArrayClient.read_block.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1110 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.ArrayClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.DaskArrayClient.export.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read_block.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1242 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.formats.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.item.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.login.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.logout.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.metadata.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      170 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.new_variation.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      669 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.specs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      180 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseStructureClient.download.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      177 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseStructureClient.refresh.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseStructureClient.structure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.cache.Cache.in_memory.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.cache.Cache.on_disk.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      508 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.cache.Cache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      266 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.cache.Scorer.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      125 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.cache.download.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.authenticate.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      187 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.force_auth_refresh.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      169 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.from_any_uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.from_app.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.login.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.logout.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.offline.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1029 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      149 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.tokens.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.export.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      215 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read_partition.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1199 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      171 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read_partition.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      121 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.from_profile.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      109 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.from_uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.distinct.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.download.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      120 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.get.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      126 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.items.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.keys.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      137 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.metadata.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.references.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      132 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.refresh.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.search.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.sort.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      134 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.sorting.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.specs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      122 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.node.Node.values.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.sparse.SparseClient.export.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      153 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.sparse.SparseClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1068 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      168 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1555 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      156 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.xarray.DatasetClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1403 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.config.construct_build_app_kwargs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.config.parse_configs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      138 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.iterviews.ValuesView.first.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.iterviews.ValuesView.head.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.iterviews.ValuesView.last.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.iterviews.ValuesView.tail.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      223 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.aliases.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      237 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.media_types.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      226 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.register.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      732 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      202 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.media_type_registration.serialization_registry.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      425 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Comparison.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      382 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Contains.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Eq.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      392 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.FullText.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.In.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      219 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Key.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      367 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.KeyLookup.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.NotEq.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.NotIn.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      388 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Regex.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       98 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Spec.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      364 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.Specs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.queries.StructureFamily.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      459 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.query_registration.QueryRegistry.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      145 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.query_registration.register.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.app.build_app.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      164 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.app.build_app_from_config.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      207 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.available_bytes.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      173 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.clear.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      198 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.dask_context.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard_dask.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.get.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.put.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      541 2023-03-31 20:25:01.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.get_object_cache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.set_object_cache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      538 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      433 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.ArrayStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      557 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      330 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.Endianness.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      485 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.Kind.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      567 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      660 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      473 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.dataframe.DataFrameStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      505 2023-03-31 20:25:02.000000 tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.sparse.COOStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1083 2023-01-06 15:55:44.000000 tiled-0.1.0a92/docs/source/reference/min-versions.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-01-06 15:55:44.000000 tiled-0.1.0a92/docs/source/reference/release-history.rst
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.553040 tiled-0.1.0a92/docs/source/tutorials/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2347 2023-01-06 15:55:44.000000 tiled-0.1.0a92/docs/source/tutorials/installation.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      280 2023-01-06 15:55:44.000000 tiled-0.1.0a92/pyproject.toml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-01-06 15:55:44.000000 tiled-0.1.0a92/requirements-array.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      175 2023-03-16 20:17:15.000000 tiled-0.1.0a92/requirements-client.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-01-06 15:55:44.000000 tiled-0.1.0a92/requirements-compression.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a92/requirements-dataframe.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      478 2023-06-01 16:59:28.000000 tiled-0.1.0a92/requirements-dev.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      111 2023-01-06 15:55:44.000000 tiled-0.1.0a92/requirements-formats.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      410 2023-06-01 16:59:28.000000 tiled-0.1.0a92/requirements-server.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       23 2023-01-06 15:55:44.000000 tiled-0.1.0a92/requirements-sparse.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a92/requirements-xarray.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      174 2023-06-02 00:30:38.601040 tiled-0.1.0a92/setup.cfg
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4316 2023-03-31 19:58:35.000000 tiled-0.1.0a92/setup.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.533040 tiled-0.1.0a92/share/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.553040 tiled-0.1.0a92/share/tiled/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.553040 tiled-0.1.0a92/share/tiled/static/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/static/favicon.ico
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.553040 tiled-0.1.0a92/share/tiled/templates/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/templates/device_code_failure.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      733 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/templates/device_code_form.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      276 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/templates/device_code_success.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/templates/index.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      491 2023-01-06 15:55:44.000000 tiled-0.1.0a92/share/tiled/templates/page.html
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.557040 tiled-0.1.0a92/share/tiled/ui/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7954 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/asset-manifest.json
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.557040 tiled-0.1.0a92/share/tiled/ui/config/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1588 2023-02-10 13:17:31.000000 tiled-0.1.0a92/share/tiled/ui/config/default.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-02-10 13:17:31.000000 tiled-0.1.0a92/share/tiled/ui/configuration_manifest.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/favicon.ico
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      674 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/index.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      292 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/manifest.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       67 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/robots.txt
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.533040 tiled-0.1.0a92/share/tiled/ui/static/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.557040 tiled-0.1.0a92/share/tiled/ui/static/css/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9577 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/css/main.da25efef.css
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12761 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/css/main.da25efef.css.map
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.577040 tiled-0.1.0a92/share/tiled/ui/static/js/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8354 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/113.a6dabf86.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    25023 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      492 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/128.74bef542.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      869 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/128.74bef542.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    95776 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/197.6f7f332e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   490879 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10212 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/214.2a10743e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    46572 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/214.2a10743e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13141 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/276.0058e750.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/276.0058e750.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37684 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/276.0058e750.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3633 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/321.c6b9dcec.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14931 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3549 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/356.6a2946e1.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10402 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   436519 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/393.73e08fb5.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      808 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   943354 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5877 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/446.ae1590fd.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    25688 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   407639 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/470.a78b4c62.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3921 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1832576 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7736 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/485.0ed51a45.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18509 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13996 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/494.3371b974.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    64957 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/494.3371b974.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    50521 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/689.0cde4405.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      245 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/689.0cde4405.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   221121 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/689.0cde4405.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      534 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/69.c379776e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1255 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/69.c379776e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    39133 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/705.eeca3f97.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       68 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/705.eeca3f97.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   168665 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1175 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/741.fbe96b6d.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2715 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1032300 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/773.590aa2f4.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1877220 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4591 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/787.54a97274.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10281 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/787.54a97274.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5344 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/837.22b95b21.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14836 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/837.22b95b21.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27323 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/858.2658cad8.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   124490 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/858.2658cad8.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4386 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/883.31ddd2ac.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14318 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/921.22e363f6.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1293 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/921.22e363f6.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    22754 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    84726 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   257278 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/main.5cc3eaa8.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1898 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   898204 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/js/main.5cc3eaa8.js.map
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.585040 tiled-0.1.0a92/share/tiled/ui/static/media/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    64952 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65244 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65492 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65292 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9500 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9688 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9776 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9544 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14988 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15344 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15080 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14720 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7120 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7100 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7000 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6888 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1476 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1492 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1508 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15732 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15688 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15920 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15828 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11812 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11860 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11768 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11836 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5460 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5540 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5580 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5524 2023-02-01 14:32:01.000000 tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.601040 tiled-0.1.0a92/tiled/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       73 2023-02-28 19:49:29.000000 tiled-0.1.0a92/tiled/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       43 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/__main__.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.593040 tiled-0.1.0a92/tiled/_tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1792 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/_tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7046 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/_tests/test_access_control.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1072 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_allow_origins.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5569 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16121 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1453 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/test_authenticators.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2224 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/test_caches.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6182 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/_tests/test_client.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13661 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_client_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3285 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_config.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.593040 tiled-0.1.0a92/tiled/_tests/test_configs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      166 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/_tests/test_configs/config_missing_api_key.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      332 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/_tests/test_configs/config_missing_secret_keys.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      448 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      195 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/_tests/test_configs/config_public_no_authenticator.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/_tests/test_configs/config_with_api_key.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      434 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_configs/config_with_secret_keys.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1475 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_custom_format.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2297 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11651 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_directory_walker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4037 2023-06-01 16:59:34.000000 tiled-0.1.0a92/tiled/_tests/test_distinct.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4628 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_export.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4090 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      555 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_history.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1189 2023-04-01 11:07:41.000000 tiled-0.1.0a92/tiled/_tests/test_import_object.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2782 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_indexers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3958 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_inlined_contents.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      780 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/test_json.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1565 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_metrics.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/test_no_heavy_imports.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5087 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_object_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1385 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_openapi.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1369 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_pickle.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5203 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      362 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/test_routes.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1125 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_scaled_config_option.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1999 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_search.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      290 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_sentinel.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2408 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_size_limit.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      621 2023-06-02 00:09:11.000000 tiled-0.1.0a92/tiled/_tests/test_slash.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3364 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_sort.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2357 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_specs_and_references.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1211 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_structured_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4237 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_tiff.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      342 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/test_tokenize.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4233 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_validation.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12165 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_writing.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4967 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/_tests/test_xarray.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      657 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/_tests/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3991 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/_tests/writable_adapters.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      500 2023-06-02 00:30:38.601040 tiled-0.1.0a92/tiled/_version.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2797 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/access_policies.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.593040 tiled-0.1.0a92/tiled/adapters/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/adapters/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3846 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/adapters/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5288 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/adapters/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1942 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/adapters/excel.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    30376 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/adapters/files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4874 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/adapters/hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14630 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/adapters/mapping.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3639 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/adapters/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7634 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/adapters/tiff.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1195 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/adapters/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1890 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/adapters/xarray.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    32406 2023-06-02 00:28:47.000000 tiled-0.1.0a92/tiled/authenticators.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.593040 tiled-0.1.0a92/tiled/client/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      244 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/client/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    29314 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/client/_testclient.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8896 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/client/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6561 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/client/auth.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10204 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/client/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27705 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/client/cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10172 2023-04-01 11:07:41.000000 tiled-0.1.0a92/tiled/client/constructors.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    36538 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/client/context.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9129 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/client/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    33534 2023-06-02 00:28:44.000000 tiled-0.1.0a92/tiled/client/node.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4934 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/client/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13106 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/client/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7262 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/client/xarray.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/commandline/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/commandline/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4919 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/commandline/_admin.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3230 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/commandline/_api_key.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1411 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/commandline/_profile.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9116 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/commandline/_serve.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2487 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/commandline/_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7916 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/commandline/main.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15934 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/config.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/config_schemas/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5275 2023-02-10 13:17:31.000000 tiled-0.1.0a92/tiled/config_schemas/client_profiles.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16272 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/config_schemas/service_configuration.yml
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/database/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/database/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2658 2023-01-06 15:55:44.000000 tiled-0.1.0a92/tiled/database/alembic.ini.template
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2690 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/database/alembic_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/database/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1704 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/database/connection_pool.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11164 2023-06-02 00:28:47.000000 tiled-0.1.0a92/tiled/database/core.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/database/migrations/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2261 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/database/migrations/env.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      494 2023-01-06 15:55:44.000000 tiled-0.1.0a92/tiled/database/migrations/script.py.mako
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/database/migrations/versions/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4023 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/database/migrations/versions/481830dd6c11_initialize.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      889 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1270 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1292 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7283 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/database/orm.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/examples/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1234 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/generate_files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4902 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/generated.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      941 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/generated_minimal.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      963 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/nexus.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      454 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/numpy_structured_dtypes.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      582 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/toy_authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4762 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/examples/xdi.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6544 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/iterviews.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10964 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/media_type_registration.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8917 2023-03-27 20:02:34.000000 tiled-0.1.0a92/tiled/profiles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11716 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4595 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/query_registration.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      690 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/scopes.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.597040 tiled-0.1.0a92/tiled/serialization/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      960 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5187 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3880 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12962 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/image_serializer_helpers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2860 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/node.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3016 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4836 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/serialization/xarray.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.601040 tiled-0.1.0a92/tiled/server/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/server/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    33375 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/server/app.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37839 2023-06-02 00:28:47.000000 tiled-0.1.0a92/tiled/server/authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6204 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/server/compression.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27685 2023-06-02 00:28:44.000000 tiled-0.1.0a92/tiled/server/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4757 2023-06-02 00:28:44.000000 tiled-0.1.0a92/tiled/server/dependencies.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1082 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/server/etag.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5637 2023-03-22 13:14:07.000000 tiled-0.1.0a92/tiled/server/metrics.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5845 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/server/object_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8486 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/server/pydantic_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2451 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/server/pydantic_dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      570 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/server/pydantic_sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    31642 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/server/router.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9685 2023-06-01 16:59:28.000000 tiled-0.1.0a92/tiled/server/schemas.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3071 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/server/settings.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4608 2023-06-01 17:19:46.000000 tiled-0.1.0a92/tiled/server/utils.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.601040 tiled-0.1.0a92/tiled/structures/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/structures/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7821 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/structures/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/structures/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2529 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/structures/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1035 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/structures/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18076 2023-03-31 19:58:35.000000 tiled-0.1.0a92/tiled/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      645 2023-02-10 13:17:36.000000 tiled-0.1.0a92/tiled/validation_registration.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-02 00:30:38.589040 tiled-0.1.0a92/tiled.egg-info/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-02 00:30:38.000000 tiled-0.1.0a92/tiled.egg-info/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    19902 2023-06-02 00:30:38.000000 tiled-0.1.0a92/tiled.egg-info/SOURCES.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2023-06-02 00:30:38.000000 tiled-0.1.0a92/tiled.egg-info/dependency_links.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       54 2023-06-02 00:30:38.000000 tiled-0.1.0a92/tiled.egg-info/entry_points.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2165 2023-06-02 00:30:38.000000 tiled-0.1.0a92/tiled.egg-info/requires.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       17 2023-06-02 00:30:38.000000 tiled-0.1.0a92/tiled.egg-info/top_level.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    80049 2023-02-10 13:17:37.000000 tiled-0.1.0a92/versioneer.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1538 2023-01-06 15:55:44.000000 tiled-0.1.0a93/LICENSE
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      783 2023-03-22 13:14:07.000000 tiled-0.1.0a93/MANIFEST.in
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-07 14:06:01.257600 tiled-0.1.0a93/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6555 2023-03-16 20:17:15.000000 tiled-0.1.0a93/README.md
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.205599 tiled-0.1.0a93/benchmarks/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/benchmarks/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1065 2023-02-10 13:17:36.000000 tiled-0.1.0a93/benchmarks/benchmarks.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.205599 tiled-0.1.0a93/docs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/Makefile
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/make.bat
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.205599 tiled-0.1.0a93/docs/source/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9186 2023-02-10 13:17:36.000000 tiled-0.1.0a93/docs/source/conf.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.209599 tiled-0.1.0a93/docs/source/reference/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    51041 2023-03-31 20:25:00.000000 tiled-0.1.0a93/docs/source/reference/api.yml
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/docs/source/reference/generated/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      554 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      194 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.read_csv.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      722 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1269 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1516 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      741 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1181 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      532 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      510 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.tiff.TiffAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      191 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.xarray.DatasetAdapter.from_dataset.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.read_block.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1110 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.export.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read_block.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1242 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.formats.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.item.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.login.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.logout.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.metadata.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      170 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.new_variation.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      669 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.specs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      180 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseStructureClient.download.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      177 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseStructureClient.refresh.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseStructureClient.structure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Cache.in_memory.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Cache.on_disk.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      508 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Cache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      266 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Scorer.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      125 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.download.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.authenticate.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      187 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.force_auth_refresh.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      169 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.from_any_uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.from_app.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.login.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.logout.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.offline.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1029 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      149 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.tokens.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.export.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      215 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read_partition.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1199 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      171 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read_partition.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      121 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.from_profile.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      109 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.from_uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.distinct.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.download.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      120 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.get.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      126 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.items.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.keys.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      137 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.metadata.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.references.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      132 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.refresh.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.search.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.sort.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      134 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.sorting.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.specs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      122 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.values.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.export.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      153 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1068 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      168 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1555 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      156 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DatasetClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1403 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.config.construct_build_app_kwargs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.config.parse_configs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      138 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.first.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.head.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.last.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.tail.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      223 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.aliases.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      237 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.media_types.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      226 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.register.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      732 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      202 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.serialization_registry.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      425 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Comparison.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      382 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Contains.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Eq.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      392 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.FullText.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.In.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      219 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Key.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      367 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.KeyLookup.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.NotEq.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.NotIn.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      388 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Regex.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       98 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Spec.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      364 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Specs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.StructureFamily.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      459 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.query_registration.QueryRegistry.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      145 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.query_registration.register.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.app.build_app.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      164 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.app.build_app_from_config.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      207 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.available_bytes.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      173 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.clear.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      198 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.dask_context.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard_dask.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.get.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.put.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      541 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.get_object_cache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.set_object_cache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      538 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      433 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.ArrayStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      557 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      330 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.Endianness.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      485 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.Kind.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      567 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      660 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      473 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      505 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.sparse.COOStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1083 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/source/reference/min-versions.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/source/reference/release-history.rst
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/docs/source/tutorials/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2347 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/source/tutorials/installation.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      280 2023-01-06 15:55:44.000000 tiled-0.1.0a93/pyproject.toml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-array.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      175 2023-03-16 20:17:15.000000 tiled-0.1.0a93/requirements-client.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-compression.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-dataframe.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      478 2023-06-07 13:54:46.000000 tiled-0.1.0a93/requirements-dev.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      111 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-formats.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      410 2023-06-07 13:54:46.000000 tiled-0.1.0a93/requirements-server.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       23 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-sparse.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-xarray.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      174 2023-06-07 14:06:01.257600 tiled-0.1.0a93/setup.cfg
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4316 2023-03-31 19:58:35.000000 tiled-0.1.0a93/setup.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.201599 tiled-0.1.0a93/share/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/static/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/static/favicon.ico
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/templates/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/device_code_failure.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      733 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/device_code_form.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      276 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/device_code_success.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/index.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      491 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/page.html
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/ui/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7954 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/asset-manifest.json
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/ui/config/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1588 2023-02-10 13:17:31.000000 tiled-0.1.0a93/share/tiled/ui/config/default.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-02-10 13:17:31.000000 tiled-0.1.0a93/share/tiled/ui/configuration_manifest.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/favicon.ico
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      674 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/index.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      292 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/manifest.json
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       67 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/robots.txt
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.201599 tiled-0.1.0a93/share/tiled/ui/static/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/ui/static/css/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9577 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12761 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css.map
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.237599 tiled-0.1.0a93/share/tiled/ui/static/js/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8354 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    25023 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      492 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/128.74bef542.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      869 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/128.74bef542.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    95776 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   490879 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10212 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    46572 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13141 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37684 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3633 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14931 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3549 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10402 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   436519 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      808 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   943354 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5877 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    25688 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   407639 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3921 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1832576 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7736 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18509 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13996 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    64957 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    50521 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      245 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   221121 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      534 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1255 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    39133 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       68 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   168665 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1175 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2715 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1032300 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1877220 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4591 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10281 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5344 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14836 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27323 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   124490 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4386 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14318 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1293 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    22754 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    84726 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   257278 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1898 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   898204 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.map
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.241599 tiled-0.1.0a93/share/tiled/ui/static/media/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    64952 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65244 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65492 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65292 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9500 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9688 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9776 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9544 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14988 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15344 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15080 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14720 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7120 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7100 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7000 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6888 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1476 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1492 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1508 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15732 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15688 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15920 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15828 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11812 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11860 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11768 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11836 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5460 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5540 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5580 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5524 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       73 2023-02-28 19:49:29.000000 tiled-0.1.0a93/tiled/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       43 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/__main__.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.249600 tiled-0.1.0a93/tiled/_tests/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1792 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/conftest.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7046 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/test_access_control.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1072 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_allow_origins.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5569 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16121 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1453 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_authenticators.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2224 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_caches.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6224 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/_tests/test_client.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13661 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_client_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3285 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_config.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.249600 tiled-0.1.0a93/tiled/_tests/test_configs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      166 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_missing_api_key.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      332 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_missing_secret_keys.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      448 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      195 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_public_no_authenticator.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_with_api_key.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      434 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_with_secret_keys.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1475 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_custom_format.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2297 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11651 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_directory_walker.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4037 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/test_distinct.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4628 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_export.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4090 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_hdf5.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      555 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_history.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1189 2023-04-01 11:07:41.000000 tiled-0.1.0a93/tiled/_tests/test_import_object.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2782 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_indexers.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3958 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_inlined_contents.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      780 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_json.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1565 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_metrics.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_no_heavy_imports.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5087 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_object_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1385 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_openapi.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1369 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_pickle.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5203 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_queries.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      362 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_routes.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1125 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_scaled_config_option.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1999 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_search.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      290 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_sentinel.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2408 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_size_limit.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      621 2023-06-02 00:09:11.000000 tiled-0.1.0a93/tiled/_tests/test_slash.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3364 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_sort.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2357 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_specs_and_references.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1211 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_structured_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4237 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_tiff.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      342 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_tokenize.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4233 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_validation.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12165 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_writing.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4967 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_xarray.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      657 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3991 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/writable_adapters.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      500 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/_version.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2797 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/access_policies.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.249600 tiled-0.1.0a93/tiled/adapters/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3846 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5288 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1942 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/excel.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    30376 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/adapters/files.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4874 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/hdf5.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14630 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/mapping.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3639 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/adapters/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7634 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/tiff.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1195 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1890 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/xarray.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    32406 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/authenticators.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/client/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      244 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/client/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    29314 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/_testclient.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8896 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/client/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6561 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/auth.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10204 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/client/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27705 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10173 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/client/constructors.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37433 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/client/context.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9129 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/client/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    33534 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/client/node.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4934 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13106 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/client/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7262 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/xarray.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/commandline/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4919 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/commandline/_admin.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3230 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/commandline/_api_key.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1411 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/_profile.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9116 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/commandline/_serve.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2487 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/_utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7916 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/main.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15934 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/config.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/config_schemas/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5275 2023-02-10 13:17:31.000000 tiled-0.1.0a93/tiled/config_schemas/client_profiles.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16272 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/config_schemas/service_configuration.yml
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/database/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2658 2023-01-06 15:55:44.000000 tiled-0.1.0a93/tiled/database/alembic.ini.template
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2690 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/alembic_utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1704 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/connection_pool.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11164 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/database/core.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/database/migrations/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2261 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/migrations/env.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      494 2023-01-06 15:55:44.000000 tiled-0.1.0a93/tiled/database/migrations/script.py.mako
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/database/migrations/versions/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4023 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/481830dd6c11_initialize.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      889 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1270 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1292 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7283 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/database/orm.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/examples/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1234 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/generate_files.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4902 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/generated.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      941 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/generated_minimal.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      963 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/nexus.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      454 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/numpy_structured_dtypes.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      582 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/toy_authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4762 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/xdi.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6544 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/iterviews.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10964 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/media_type_registration.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8917 2023-03-27 20:02:34.000000 tiled-0.1.0a93/tiled/profiles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11716 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/queries.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4595 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/query_registration.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      690 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/scopes.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/serialization/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      960 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5187 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3880 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12962 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/image_serializer_helpers.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2860 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/node.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3016 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4836 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/xarray.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/server/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    33375 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/app.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37847 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/server/authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6204 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/compression.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27685 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/core.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4757 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/dependencies.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1082 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/etag.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5637 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/server/metrics.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5845 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/object_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8486 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/pydantic_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2451 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/pydantic_dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      570 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/pydantic_sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    31642 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/router.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9685 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/schemas.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3071 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/server/settings.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4608 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/utils.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/structures/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7821 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/structures/core.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2529 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1035 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18076 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      645 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/validation_registration.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.241599 tiled-0.1.0a93/tiled.egg-info/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    19902 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/SOURCES.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/dependency_links.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       54 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/entry_points.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2165 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/requires.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       17 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/top_level.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    80049 2023-02-10 13:17:37.000000 tiled-0.1.0a93/versioneer.py
```

### Comparing `tiled-0.1.0a92/LICENSE` & `tiled-0.1.0a93/LICENSE`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/MANIFEST.in` & `tiled-0.1.0a93/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/PKG-INFO` & `tiled-0.1.0a93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiled
-Version: 0.1.0a92
+Version: 0.1.0a93
 Summary: Tile-based access to SciPy/PyData data structures over the web in many formats
 Home-page: https://github.com/bluesky/tiled
 Author: Bluesky Collaboration
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `tiled-0.1.0a92/README.md` & `tiled-0.1.0a93/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/benchmarks/benchmarks.py` & `tiled-0.1.0a93/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/Makefile` & `tiled-0.1.0a93/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/make.bat` & `tiled-0.1.0a93/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/conf.py` & `tiled-0.1.0a93/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/api.yml` & `tiled-0.1.0a93/docs/source/reference/api.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.ArrayClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.base.BaseClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.context.Context.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst` & `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/reference/min-versions.rst` & `tiled-0.1.0a93/docs/source/reference/min-versions.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/docs/source/tutorials/installation.rst` & `tiled-0.1.0a93/docs/source/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/setup.py` & `tiled-0.1.0a93/setup.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/static/favicon.ico` & `tiled-0.1.0a93/share/tiled/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/templates/device_code_form.html` & `tiled-0.1.0a93/share/tiled/templates/device_code_form.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/templates/index.html` & `tiled-0.1.0a93/share/tiled/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/asset-manifest.json` & `tiled-0.1.0a93/share/tiled/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/config/default.yml` & `tiled-0.1.0a93/share/tiled/ui/config/default.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/favicon.ico` & `tiled-0.1.0a93/share/tiled/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/index.html` & `tiled-0.1.0a93/share/tiled/ui/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/css/main.da25efef.css` & `tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/css/main.da25efef.css.map` & `tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/113.a6dabf86.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/128.74bef542.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/128.74bef542.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/197.6f7f332e.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/214.2a10743e.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/214.2a10743e.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/276.0058e750.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/276.0058e750.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/321.c6b9dcec.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/356.6a2946e1.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/393.73e08fb5.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt` & `tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/446.ae1590fd.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/470.a78b4c62.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt` & `tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/485.0ed51a45.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/494.3371b974.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/494.3371b974.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/689.0cde4405.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/689.0cde4405.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/69.c379776e.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/69.c379776e.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/705.eeca3f97.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/741.fbe96b6d.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/773.590aa2f4.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/787.54a97274.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/787.54a97274.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/837.22b95b21.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/837.22b95b21.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/858.2658cad8.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/858.2658cad8.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/883.31ddd2ac.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/921.22e363f6.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/921.22e363f6.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/main.5cc3eaa8.js` & `tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt` & `tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/js/main.5cc3eaa8.js.map` & `tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2` & `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/conftest.py` & `tiled-0.1.0a93/tiled/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_access_control.py` & `tiled-0.1.0a93/tiled/_tests/test_access_control.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_allow_origins.py` & `tiled-0.1.0a93/tiled/_tests/test_allow_origins.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_array.py` & `tiled-0.1.0a93/tiled/_tests/test_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_authentication.py` & `tiled-0.1.0a93/tiled/_tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_authenticators.py` & `tiled-0.1.0a93/tiled/_tests/test_authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_caches.py` & `tiled-0.1.0a93/tiled/_tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_client.py` & `tiled-0.1.0a93/tiled/_tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,20 @@
         with fail_with_status_code(400):
             list(client)
 
 
 def test_direct(tmpdir):
     profile_content = {
         "test": {
+            "structure_clients": "dask",
             "direct": {
                 "trees": [
                     {"path": "/", "tree": "tiled.examples.generated_minimal:tree"}
                 ]
-            }
+            },
         }
     }
     with open(tmpdir / "example.yml", "w") as file:
         file.write(yaml.dump(profile_content))
     profile_dir = Path(tmpdir)
     try:
         paths.append(profile_dir)
```

### Comparing `tiled-0.1.0a92/tiled/_tests/test_client_cache.py` & `tiled-0.1.0a93/tiled/_tests/test_client_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_config.py` & `tiled-0.1.0a93/tiled/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_custom_format.py` & `tiled-0.1.0a93/tiled/_tests/test_custom_format.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_dataframe.py` & `tiled-0.1.0a93/tiled/_tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_directory_walker.py` & `tiled-0.1.0a93/tiled/_tests/test_directory_walker.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_distinct.py` & `tiled-0.1.0a93/tiled/_tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_export.py` & `tiled-0.1.0a93/tiled/_tests/test_export.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_hdf5.py` & `tiled-0.1.0a93/tiled/_tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_history.py` & `tiled-0.1.0a93/tiled/_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_import_object.py` & `tiled-0.1.0a93/tiled/_tests/test_import_object.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_indexers.py` & `tiled-0.1.0a93/tiled/_tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_inlined_contents.py` & `tiled-0.1.0a93/tiled/_tests/test_inlined_contents.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_json.py` & `tiled-0.1.0a93/tiled/_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_metrics.py` & `tiled-0.1.0a93/tiled/_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_object_cache.py` & `tiled-0.1.0a93/tiled/_tests/test_object_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_openapi.py` & `tiled-0.1.0a93/tiled/_tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_pickle.py` & `tiled-0.1.0a93/tiled/_tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_queries.py` & `tiled-0.1.0a93/tiled/_tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_scaled_config_option.py` & `tiled-0.1.0a93/tiled/_tests/test_scaled_config_option.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_search.py` & `tiled-0.1.0a93/tiled/_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_size_limit.py` & `tiled-0.1.0a93/tiled/_tests/test_size_limit.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_slash.py` & `tiled-0.1.0a93/tiled/_tests/test_slash.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_sort.py` & `tiled-0.1.0a93/tiled/_tests/test_sort.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_sparse.py` & `tiled-0.1.0a93/tiled/_tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_specs_and_references.py` & `tiled-0.1.0a93/tiled/_tests/test_specs_and_references.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_structured_array.py` & `tiled-0.1.0a93/tiled/_tests/test_structured_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_tiff.py` & `tiled-0.1.0a93/tiled/_tests/test_tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_validation.py` & `tiled-0.1.0a93/tiled/_tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_writing.py` & `tiled-0.1.0a93/tiled/_tests/test_writing.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/test_xarray.py` & `tiled-0.1.0a93/tiled/_tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/utils.py` & `tiled-0.1.0a93/tiled/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/_tests/writable_adapters.py` & `tiled-0.1.0a93/tiled/_tests/writable_adapters.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/access_policies.py` & `tiled-0.1.0a93/tiled/access_policies.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/array.py` & `tiled-0.1.0a93/tiled/adapters/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/dataframe.py` & `tiled-0.1.0a93/tiled/adapters/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/excel.py` & `tiled-0.1.0a93/tiled/adapters/excel.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/files.py` & `tiled-0.1.0a93/tiled/adapters/files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/hdf5.py` & `tiled-0.1.0a93/tiled/adapters/hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/mapping.py` & `tiled-0.1.0a93/tiled/adapters/mapping.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/sparse.py` & `tiled-0.1.0a93/tiled/adapters/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/tiff.py` & `tiled-0.1.0a93/tiled/adapters/tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/utils.py` & `tiled-0.1.0a93/tiled/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/adapters/xarray.py` & `tiled-0.1.0a93/tiled/adapters/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/authenticators.py` & `tiled-0.1.0a93/tiled/authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/_testclient.py` & `tiled-0.1.0a93/tiled/client/_testclient.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/array.py` & `tiled-0.1.0a93/tiled/client/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/auth.py` & `tiled-0.1.0a93/tiled/client/auth.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/base.py` & `tiled-0.1.0a93/tiled/client/base.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/cache.py` & `tiled-0.1.0a93/tiled/client/cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/constructors.py` & `tiled-0.1.0a93/tiled/client/constructors.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,12 +264,12 @@
             jsonschema.validate(instance=config, schema=schema())
         except jsonschema.ValidationError as err:
             msg = err.args[0]
             raise ConfigError(
                 f"ValidationError while parsing configuration file {filepath}: {msg}"
             ) from err
         context = Context.from_app(
-            build_app_from_config(config, source_filepath=filepath), **merged
+            build_app_from_config(config, source_filepath=filepath),
         )
-        return from_context(context)
+        return from_context(context, **merged)
     else:
         return from_uri(**merged)
```

### Comparing `tiled-0.1.0a92/tiled/client/context.py` & `tiled-0.1.0a93/tiled/client/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -677,17 +677,15 @@
     ):
         """
         See login. This is for programmatic use.
         """
         if prompt_for_reauthentication is UNSET:
             prompt_for_reauthentication = PROMPT_FOR_REAUTHENTICATION
         if prompt_for_reauthentication is None:
-            prompt_for_reauthentication = (
-                not sys.__stdin__.closed
-            ) and sys.__stdin__.isatty()
+            prompt_for_reauthentication = _can_prompt()
         providers = self.server_info["authentication"]["providers"]
         spec = _choose_identity_provider(providers, provider)
         provider = spec["provider"]
         if self.api_key is not None:
             # Check that API key authenticates us as this user,
             # and then either return or raise.
             identities = self.whoami()["identities"]
@@ -722,15 +720,22 @@
             else:
                 # We have a live session for the specified provider and username already.
                 # No need to log in again.
                 return
 
         if not prompt_for_reauthentication:
             raise CannotPrompt(
-                "Authentication is needed but the client cannot prompt for it."
+                """Authentication is needed but Tiled has detected that it is running
+in a 'headless' context where it cannot prompt the user to provide
+credentials in the stdin. Options:
+
+- If Tiled has detected this wrongly, pass prompt_for_reauthentication=True
+  to force it to prompt.
+- Provide an API key in the environment variable TILED_API_KEY for Tiled to use.
+"""
             )
         self.http_client.auth = None
         mode = spec["mode"]
         auth_endpoint = spec["links"]["auth_endpoint"]
         if mode == "password":
             if username:
                 print(f"Username {username}")
@@ -754,17 +759,19 @@
             handle_error(verification_response)
             verification = verification_response.json()
             authorization_uri = verification["authorization_uri"]
             print(
                 f"""
 You have {int(verification['expires_in']) // 60} minutes visit this URL
 
-{authorization_uri}
+  {authorization_uri}
+
+and enter the code:
 
-and enter the code: {verification['user_code']}
+  {verification['user_code']}
 
 """
             )
             import webbrowser
 
             webbrowser.open(authorization_uri)
             deadline = verification["expires_in"] + time.monotonic()
@@ -800,15 +807,15 @@
         auth.sync_set_token("refresh_token", tokens["refresh_token"])
         self.http_client.auth = auth
         confirmation_message = spec.get("confirmation_message")
         if confirmation_message:
             print(confirmation_message.format(id=username))
         return spec, username
 
-    def login(self, username=None, provider=None):
+    def login(self, username=None, provider=None, prompt_for_reauthentication=UNSET):
         """
         Depending on the server's authentication method, this will prompt for username/password:
 
         >>> c.login()
         Username: USERNAME
         Password: <input is hidden>
 
@@ -817,15 +824,17 @@
         >>> c.login()
         You have ... minutes visit this URL
 
         https://...
 
         and enter the code: XXXX-XXXX
         """
-        self.authenticate(username, provider)
+        self.authenticate(
+            username, provider, prompt_for_reauthentication=prompt_for_reauthentication
+        )
         # For programmatic access to the return values, use authenticate().
         # This returns None in order to provide a clean UX in an interpreter.
         return None
 
     def _token_directory(self, provider, username):
         # ~/.config/tiled/tokens/{host:port}/{provider}/{username}
         # with each templated element URL-encoded so it is a valid filename.
@@ -974,7 +983,24 @@
         )
         handle_error(response)
         return response.json()
 
 
 class CannotPrompt(Exception):
     pass
+
+
+def _can_prompt():
+    "Infer whether the user can be prompted for a password or user code."
+
+    if (not sys.__stdin__.closed) and sys.__stdin__.isatty():
+        return True
+    # In IPython (TerminalInteractiveShell) the above is true, but in
+    # Jupyter (ZMQInteractiveShell) it is False.
+    # Jupyter own mechanism for giving a prompt, so we always return
+    # True if we detect IPython/Jupyter.
+    if "IPython" in sys.modules:
+        import IPython
+
+        if IPython.get_ipython() is not None:
+            return True
+    return False
```

### Comparing `tiled-0.1.0a92/tiled/client/dataframe.py` & `tiled-0.1.0a93/tiled/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/node.py` & `tiled-0.1.0a93/tiled/client/node.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/sparse.py` & `tiled-0.1.0a93/tiled/client/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/utils.py` & `tiled-0.1.0a93/tiled/client/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/client/xarray.py` & `tiled-0.1.0a93/tiled/client/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/commandline/_admin.py` & `tiled-0.1.0a93/tiled/commandline/_admin.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/commandline/_api_key.py` & `tiled-0.1.0a93/tiled/commandline/_api_key.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/commandline/_profile.py` & `tiled-0.1.0a93/tiled/commandline/_profile.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/commandline/_serve.py` & `tiled-0.1.0a93/tiled/commandline/_serve.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/commandline/_utils.py` & `tiled-0.1.0a93/tiled/commandline/_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/commandline/main.py` & `tiled-0.1.0a93/tiled/commandline/main.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/config.py` & `tiled-0.1.0a93/tiled/config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/config_schemas/client_profiles.yml` & `tiled-0.1.0a93/tiled/config_schemas/client_profiles.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/config_schemas/service_configuration.yml` & `tiled-0.1.0a93/tiled/config_schemas/service_configuration.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/alembic.ini.template` & `tiled-0.1.0a93/tiled/database/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/alembic_utils.py` & `tiled-0.1.0a93/tiled/database/alembic_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/connection_pool.py` & `tiled-0.1.0a93/tiled/database/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/core.py` & `tiled-0.1.0a93/tiled/database/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/migrations/env.py` & `tiled-0.1.0a93/tiled/database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/migrations/versions/481830dd6c11_initialize.py` & `tiled-0.1.0a93/tiled/database/migrations/versions/481830dd6c11_initialize.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py` & `tiled-0.1.0a93/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py` & `tiled-0.1.0a93/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py` & `tiled-0.1.0a93/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/database/orm.py` & `tiled-0.1.0a93/tiled/database/orm.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/examples/generate_files.py` & `tiled-0.1.0a93/tiled/examples/generate_files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/examples/generated.py` & `tiled-0.1.0a93/tiled/examples/generated.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/examples/generated_minimal.py` & `tiled-0.1.0a93/tiled/examples/generated_minimal.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/examples/nexus.py` & `tiled-0.1.0a93/tiled/examples/nexus.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/examples/toy_authentication.py` & `tiled-0.1.0a93/tiled/examples/toy_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/examples/xdi.py` & `tiled-0.1.0a93/tiled/examples/xdi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/iterviews.py` & `tiled-0.1.0a93/tiled/iterviews.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/media_type_registration.py` & `tiled-0.1.0a93/tiled/media_type_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/profiles.py` & `tiled-0.1.0a93/tiled/profiles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/queries.py` & `tiled-0.1.0a93/tiled/queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/query_registration.py` & `tiled-0.1.0a93/tiled/query_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/scopes.py` & `tiled-0.1.0a93/tiled/scopes.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/__init__.py` & `tiled-0.1.0a93/tiled/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/array.py` & `tiled-0.1.0a93/tiled/serialization/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/dataframe.py` & `tiled-0.1.0a93/tiled/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/image_serializer_helpers.py` & `tiled-0.1.0a93/tiled/serialization/image_serializer_helpers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/node.py` & `tiled-0.1.0a93/tiled/serialization/node.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/sparse.py` & `tiled-0.1.0a93/tiled/serialization/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/serialization/xarray.py` & `tiled-0.1.0a93/tiled/serialization/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/app.py` & `tiled-0.1.0a93/tiled/server/app.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/authentication.py` & `tiled-0.1.0a93/tiled/server/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,20 +566,20 @@
         settings: BaseSettings = Depends(get_settings),
         db=Depends(get_database_session),
     ):
         request.state.endpoint = "auth"
         action = (
             f"{get_base_url(request)}/auth/provider/{provider}/device_code?code={code}"
         )
-        normalized_user_code = user_code.upper().replace("-", "")
+        normalized_user_code = user_code.upper().replace("-", "").strip()
         pending_session = await lookup_valid_pending_session_by_user_code(
             db, normalized_user_code
         )
         if pending_session is None:
-            message = "Invalid user_code. It may have been mistyped, or the pending request may have expired."
+            message = "Invalid user code. It may have been mistyped, or the pending request may have expired."
             return templates.TemplateResponse(
                 "device_code_form.html",
                 {
                     "request": request,
                     "code": code,
                     "action": action,
                     "message": message,
```

### Comparing `tiled-0.1.0a92/tiled/server/compression.py` & `tiled-0.1.0a93/tiled/server/compression.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/core.py` & `tiled-0.1.0a93/tiled/server/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/dependencies.py` & `tiled-0.1.0a93/tiled/server/dependencies.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/etag.py` & `tiled-0.1.0a93/tiled/server/etag.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/metrics.py` & `tiled-0.1.0a93/tiled/server/metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/object_cache.py` & `tiled-0.1.0a93/tiled/server/object_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/pydantic_array.py` & `tiled-0.1.0a93/tiled/server/pydantic_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/pydantic_dataframe.py` & `tiled-0.1.0a93/tiled/server/pydantic_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/pydantic_sparse.py` & `tiled-0.1.0a93/tiled/server/pydantic_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/router.py` & `tiled-0.1.0a93/tiled/server/router.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/schemas.py` & `tiled-0.1.0a93/tiled/server/schemas.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/settings.py` & `tiled-0.1.0a93/tiled/server/settings.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/server/utils.py` & `tiled-0.1.0a93/tiled/server/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/structures/array.py` & `tiled-0.1.0a93/tiled/structures/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/structures/core.py` & `tiled-0.1.0a93/tiled/structures/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/structures/dataframe.py` & `tiled-0.1.0a93/tiled/structures/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/structures/sparse.py` & `tiled-0.1.0a93/tiled/structures/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/utils.py` & `tiled-0.1.0a93/tiled/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled/validation_registration.py` & `tiled-0.1.0a93/tiled/validation_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled.egg-info/PKG-INFO` & `tiled-0.1.0a93/tiled.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiled
-Version: 0.1.0a92
+Version: 0.1.0a93
 Summary: Tile-based access to SciPy/PyData data structures over the web in many formats
 Home-page: https://github.com/bluesky/tiled
 Author: Bluesky Collaboration
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `tiled-0.1.0a92/tiled.egg-info/SOURCES.txt` & `tiled-0.1.0a93/tiled.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/tiled.egg-info/requires.txt` & `tiled-0.1.0a93/tiled.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a92/versioneer.py` & `tiled-0.1.0a93/versioneer.py`

 * *Files identical despite different names*

