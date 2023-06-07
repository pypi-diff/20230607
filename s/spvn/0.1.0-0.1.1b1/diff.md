# Comparing `tmp/spvn-0.1.0.tar.gz` & `tmp/spvn-0.1.1b1.tar.gz`

## Comparing `spvn-0.1.0.tar` & `spvn-0.1.1b1.tar`

### file list

```diff
@@ -1,7 +1,51 @@
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 spvn-0.1.0/crates/spvn_py/Cargo.toml
--rw-r--r--   0      501       20      380 2023-05-26 20:29:37.000000 spvn-0.1.0/crates/spvn_py/src/lib.rs
--rw-r--r--   0      501       20      510 2023-05-26 20:30:02.000000 spvn-0.1.0/pyproject.toml
--rw-r--r--   0      501       20    30070 2023-05-26 19:56:59.000000 spvn-0.1.0/crates/spvn_py/Cargo.lock
--rw-r--r--   0      501       20       31 2023-05-26 20:29:41.000000 spvn-0.1.0/python/spvn/__init__.py
--rw-r--r--   0      501       20      564 2023-05-26 01:12:17.000000 spvn-0.1.0/python/spvn/__main__.py
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 spvn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/Cargo.toml
+-rw-r--r--   0     1001      123       20 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/README.md
+-rw-r--r--   0     1001      123     2678 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/src/lib.rs
+-rw-r--r--   0     1001      123    11705 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/src/service/caller.rs
+-rw-r--r--   0     1001      123     4534 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/src/service/imports.rs
+-rw-r--r--   0     1001      123     1104 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/src/service/lifespan.rs
+-rw-r--r--   0     1001      123       51 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_caller/src/service/mod.rs
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/Cargo.toml
+-rw-r--r--   0     1001      123     5731 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/asgi_scope.rs
+-rw-r--r--   0     1001      123     2323 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/asgi_sender.rs
+-rw-r--r--   0     1001      123     1234 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/body_receiver.rs
+-rw-r--r--   0     1001      123     3516 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/call_async.rs
+-rw-r--r--   0     1001      123     2416 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/coalesced.rs
+-rw-r--r--   0     1001      123     2129 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/event_receiver.rs
+-rw-r--r--   0     1001      123     2325 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/event_sender.rs
+-rw-r--r--   0     1001      123      955 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/implementation.rs
+-rw-r--r--   0     1001      123     9292 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/lib.rs
+-rw-r--r--   0     1001      123      572 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_serde/src/state.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 spvn-0.1.1b1/local_dependencies/spvn_macros/Cargo.toml
+-rw-r--r--   0     1001      123     5177 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_macros/src/lib.rs
+-rw-r--r--   0        0        0      176 1970-01-01 00:00:00.000000 spvn-0.1.1b1/local_dependencies/spvn_dev/Cargo.toml
+-rw-r--r--   0     1001      123      453 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_dev/src/lib.rs
+-rw-r--r--   0     1001      123       13 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn_dev/src/main.rs
+-rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 spvn-0.1.1b1/local_dependencies/spvn/Cargo.toml
+-rw-r--r--   0     1001      123       13 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/README.md
+-rw-r--r--   0     1001      123     6384 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/handlers/http.rs
+-rw-r--r--   0     1001      123      874 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/handlers/logging.rs
+-rw-r--r--   0     1001      123       46 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/handlers/mod.rs
+-rw-r--r--   0     1001      123     1945 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/handlers/tasks.rs
+-rw-r--r--   0     1001      123       50 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/lib.rs
+-rw-r--r--   0     1001      123     6210 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/spvn.rs
+-rw-r--r--   0     1001      123      820 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/startup/listen.rs
+-rw-r--r--   0     1001      123     1208 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/startup/message.rs
+-rw-r--r--   0     1001      123       60 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/startup/mod.rs
+-rw-r--r--   0     1001      123      890 2023-06-07 02:02:06.000000 spvn-0.1.1b1/local_dependencies/spvn/src/startup/tls.rs
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 spvn-0.1.1b1/crates/spvn_cli/Cargo.toml
+-rw-r--r--   0     1001      123      124 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/build.rs
+-rw-r--r--   0     1001      123      765 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/src/args.rs
+-rw-r--r--   0     1001      123        0 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/src/bin/.gitkeep
+-rw-r--r--   0     1001      123      568 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/src/bin/spvn.rs
+-rw-r--r--   0     1001      123       22 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/src/commands/mod.rs
+-rw-r--r--   0     1001      123     7321 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/src/commands/serve.rs
+-rw-r--r--   0     1001      123      873 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/src/lib.rs
+-rw-r--r--   0     1001      123     2427 2023-06-07 02:02:06.000000 spvn-0.1.1b1/pyproject.toml
+-rw-r--r--   0     1001      123    42130 2023-06-07 02:02:06.000000 spvn-0.1.1b1/crates/spvn_cli/Cargo.lock
+-rw-r--r--   0     1001      123       36 2023-06-07 02:02:06.000000 spvn-0.1.1b1/src/spvn/__init__.py
+-rw-r--r--   0     1001      123      855 2023-06-07 02:02:06.000000 spvn-0.1.1b1/src/spvn/types.py
+-rw-r--r--   0     1001      123      565 2023-06-07 02:02:06.000000 spvn-0.1.1b1/src/spvn/__main__.py
+-rw-r--r--   0     1001      123        0 2023-06-07 02:02:06.000000 spvn-0.1.1b1/src/spvn/py.typed
+-rw-r--r--   0     1001      123     4680 2023-06-07 02:02:06.000000 spvn-0.1.1b1/README.md
+-rw-r--r--   0        0        0     6115 1970-01-01 00:00:00.000000 spvn-0.1.1b1/PKG-INFO
```

### Comparing `spvn-0.1.0/crates/spvn_py/Cargo.toml` & `spvn-0.1.1b1/local_dependencies/spvn_caller/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 [package]
-name = "spvn_py"
-version = "0.1.0"
-publish = false
-edition = "2021"
-rust-version = "1.69.0"
+name = "spvn_caller"
+version= "0.1.1-beta.1"
+authors= ["Joshua A. <joshua.auchincloss@proton.me>"]
+edition= "2021"
+rust-version= "1.69.0"
+documentation= "https://github.com/spvn-rs/spvn"
+description= "asgi rust bindings"
+homepage= "https://spvn-rs.github.io/spvn/"
+repository= "https://github.com/spvn-rs/spvn"
+readme = "README.md"
+license = "MIT"
 
 [lib]
-crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = {version = "0.18.3", features = ["auto-initialize", "extension-module","generate-import-lib"]}
-pyo3-asyncio = { version = "0.18", features = ["attributes", "tokio-runtime"] }
 
+pyo3 = { version = "0.19.0" , features = ["abi3"] }
+futures = { version = "0.3.28" , features = [] }
+crossbeam = "0.8"
+
+deadpool = "0.9.5"
+
+spvn_serde = { path = "../spvn_serde" }
+spvn_dev = { path = "../spvn_dev" }
+
+syncpool = { version = "0.1.6" }
+async-trait = {version = "0.1.68"}
+tokio = {version = "1.9", features = ["sync", "rt"]}
+libc = { version = "0.2.145" }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
-pythonize = { version = "0.18.0" }
-tokio = {version = "1.9", features = ["sync"]}
-async-trait = {version = "0.1.68"}
-simple_logger = "4.1.0"
-log = "0.4.17"
+
 anyhow = { version = "1.0.71" }
+tracing = "0.1"
+colored = { version = "2.0.0" }
+
+
+
+bytes = "1"
+crossbeam-utils = "0.8.15"
+
+
```

### Comparing `spvn-0.1.0/crates/spvn_py/Cargo.lock` & `spvn-0.1.1b1/crates/spvn_cli/Cargo.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "aho-corasick"
-version = "1.0.1"
+name = "ahash"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
- "memchr",
+ "cfg-if",
+ "getrandom",
+ "once_cell",
+ "version_check",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
@@ -70,15 +73,15 @@
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
@@ -91,65 +94,99 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bumpalo"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
+name = "byteorder"
+version = "1.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+
+[[package]]
+name = "bytes"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+
+[[package]]
+name = "bytes-expand"
+version = "0.4.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db996977b03d0f6294aee499b45a794ea03f942a68ca92aff9e79c615c28c99e"
+dependencies = [
+ "byteorder",
+ "iovec",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.3.0"
+version = "4.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
+checksum = "b4ed2379f8603fa2b7509891660e802b88c70a79a6427a70abb5968054de2c28"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.0"
+version = "4.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
+checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.0"
+version = "4.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "191d9573962933b4027f932c600cd252ce27a8ad5979418fe78e43c07996f27b"
+checksum = "59e9ef9a08ee1c0e1f2e162121665ac45ac3783b0f897db7244ae75ad9a8f65b"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
@@ -168,26 +205,100 @@
 dependencies = [
  "atty",
  "lazy_static",
  "winapi",
 ]
 
 [[package]]
-name = "cpython"
-version = "0.7.1"
+name = "crossbeam"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3052106c29da7390237bc2310c1928335733b286287754ea85e6093d2495280e"
+checksum = "2801af0d36612ae591caa9568261fddce32ce6e08a7275ea334a06a4ad021a2c"
 dependencies = [
- "libc",
- "num-traits",
- "paste",
- "python3-sys",
+ "cfg-if",
+ "crossbeam-channel",
+ "crossbeam-deque",
+ "crossbeam-epoch",
+ "crossbeam-queue",
+ "crossbeam-utils",
 ]
 
 [[package]]
+name = "crossbeam-channel"
+version = "0.5.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-deque"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+dependencies = [
+ "cfg-if",
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "crossbeam-utils",
+ "memoffset 0.8.0",
+ "scopeguard",
+]
+
+[[package]]
+name = "crossbeam-queue"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d1cfb3ea8a53f37c40dea2c7bedcbd88bdfae54f5e2175d6ecaff1c988353add"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
+name = "deadpool"
+version = "0.9.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "421fe0f90f2ab22016f32a9881be5134fdd71c65298917084b0c7477cbc3856e"
+dependencies = [
+ "async-trait",
+ "deadpool-runtime",
+ "num_cpus",
+ "retain_mut",
+ "tokio",
+]
+
+[[package]]
+name = "deadpool-runtime"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eaa37046cc0f6c3cc6090fbdbf73ef0b8ef4cfcc37f6befc0020f63e8cf121e1"
+
+[[package]]
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
@@ -201,14 +312,41 @@
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
+name = "filetime"
+version = "0.2.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "redox_syscall",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
+name = "fsevent-sys"
+version = "4.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76ee7a02da4d231650c7cea31349b889be2f45ddb3ef3032d2ec8185f6313fd2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "futures"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -256,15 +394,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -290,14 +428,44 @@
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
+name = "getrandom"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
+name = "h2"
+version = "0.3.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
@@ -326,14 +494,72 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "http"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
+
+[[package]]
+name = "hyper"
+version = "0.14.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2 0.4.9",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -342,25 +568,54 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "inotify"
+version = "0.9.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8069d3ec154eb856955c1c0fbffefbf5f3c40a104ec912d4797314c1801abff"
+dependencies = [
+ "bitflags",
+ "inotify-sys",
+ "libc",
+]
+
+[[package]]
+name = "inotify-sys"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e05c02b5e89bff3b946cedeca278abc628fe811e604f027c45a8aa3cf793d0eb"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "iovec"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2b3ea6ff95e175473f8ffe6a7eb7c00d054240321b84c57051175fe3c1e075e"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
@@ -371,24 +626,53 @@
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "js-sys"
+version = "0.3.63"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "kqueue"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c8fc60ba15bf51257aa9807a48a61013db043fcf3a78cb0d916e8e396dcad98"
+dependencies = [
+ "kqueue-sys",
+ "libc",
+]
+
+[[package]]
+name = "kqueue-sys"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8367585489f01bc55dd27404dcf56b95e6da061a256a666ab23be9ba96a2e587"
+dependencies = [
+ "bitflags",
+ "libc",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.145"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "fc86cde3ff845662b8f4ef6cb50ea0e20c524eb3d29ae048287e06a1b3fa6a81"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
@@ -400,20 +684,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -423,58 +704,83 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "log",
  "wasi",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "notify"
+version = "6.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d9ba6c734de18ca27c8cef5cd7058aa4ac9f63596131e4c7e41e579319032a2"
+dependencies = [
+ "bitflags",
+ "crossbeam-channel",
+ "filetime",
+ "fsevent-sys",
+ "inotify",
+ "kqueue",
+ "libc",
+ "mio",
+ "walkdir",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
-name = "num-traits"
-version = "0.2.15"
+name = "nu-ansi-term"
+version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
- "autocfg",
+ "overload",
+ "winapi",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
-name = "num_threads"
-version = "0.1.6"
+name = "once_cell"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
-dependencies = [
- "libc",
-]
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
-name = "once_cell"
-version = "1.17.1"
+name = "overload"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -492,20 +798,14 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
-name = "paste"
-version = "1.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
-
-[[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "pin-utils"
@@ -520,128 +820,73 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.9.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
-name = "pyo3-asyncio"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3564762e37035cfc486228e10b0528460fa026d681b5763873c693aa0d5c260"
-dependencies = [
- "futures",
- "once_cell",
- "pin-project-lite",
- "pyo3",
- "pyo3-asyncio-macros",
- "tokio",
-]
-
-[[package]]
-name = "pyo3-asyncio-macros"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be72d4cd43a27530306bd0d20d3932182fbdd072c6b98d3638bc37efb9d559dd"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
- "python3-dll-a",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "python3-dll-a"
-version = "0.2.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "212d74540270e3a22eed5f0d4bbc0765dff20958d694e9d4f5ebe6e22778c422"
-dependencies = [
- "cc",
-]
-
-[[package]]
-name = "python3-sys"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49f8b50d72fb3015735aa403eebf19bbd72c093bfeeae24ee798be5f2f1aab52"
-dependencies = [
- "libc",
- "regex",
-]
-
-[[package]]
-name = "pythonize"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a0e1bbcd2a3856284bf4f4ef09ccb1157e9467847792754556f153ea3fe6b42"
-dependencies = [
- "pyo3",
- "serde",
-]
-
-[[package]]
 name = "quote"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
@@ -652,29 +897,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "regex"
-version = "1.8.3"
+name = "retain_mut"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-syntax",
-]
+checksum = "4389f1d5789befaf6029ebd9f7dac4af7f7e3d61b69d4f30e2ac02b57e7712b0"
 
 [[package]]
-name = "regex-syntax"
-version = "0.7.2"
+name = "ring"
+version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
+dependencies = [
+ "cc",
+ "libc",
+ "once_cell",
+ "spin",
+ "untrusted",
+ "web-sys",
+ "winapi",
+]
 
 [[package]]
 name = "rustix"
 version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
@@ -683,26 +932,76 @@
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "rustls"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-webpki",
+ "sct",
+]
+
+[[package]]
+name = "rustls-pemfile"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+dependencies = [
+ "base64",
+]
+
+[[package]]
+name = "rustls-webpki"
+version = "0.100.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
+name = "same-file"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
+dependencies = [
+ "winapi-util",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "sct"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
 name = "serde"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
@@ -711,48 +1010,35 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "serde_spanned"
-version = "0.6.2"
+name = "sharded-slab"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93107647184f6027e3b7dcb2e11034cf95ffa1e3a682c67951963ac69c1c007d"
+checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
- "serde",
-]
-
-[[package]]
-name = "simple_logger"
-version = "4.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78beb34673091ccf96a8816fce8bfd30d1292c7621ca2bcb5f2ba0fae4f558d"
-dependencies = [
- "atty",
- "colored",
- "log",
- "time",
- "windows-sys 0.42.0",
+ "lazy_static",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
@@ -773,120 +1059,149 @@
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
-name = "spvn"
-version = "0.1.0"
+name = "socket2"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2538b18701741680e0322a2302176d3253a35388e2e62f172f64f4f16605f877"
 dependencies = [
- "spvn_lifespan",
- "spvn_py",
+ "libc",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "spvn_caller"
-version = "0.1.0"
+name = "spin"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
+
+[[package]]
+name = "spvn"
+version = "0.1.1-beta.1"
 dependencies = [
+ "ahash",
  "anyhow",
  "async-trait",
+ "bytes",
+ "bytes-expand",
  "colored",
- "cpython",
- "libc",
- "log",
- "serde",
- "serde_json",
- "simple_logger",
+ "crossbeam",
+ "deadpool",
+ "futures",
+ "http",
+ "http-body",
+ "hyper",
+ "pyo3",
+ "rustls-pemfile",
+ "socket2 0.5.3",
+ "spvn_caller",
+ "spvn_dev",
+ "spvn_serde",
+ "tokio",
+ "tokio-rustls",
+ "tokio-stream",
+ "tokio-util",
+ "tower",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+ "tracing-core",
+ "tracing-subscriber",
 ]
 
 [[package]]
-name = "spvn_cfg"
-version = "0.1.0"
+name = "spvn_caller"
+version = "0.1.1-beta.1"
 dependencies = [
- "clap",
- "log",
+ "anyhow",
+ "async-trait",
+ "bytes",
+ "colored",
+ "crossbeam",
+ "crossbeam-utils",
+ "deadpool",
+ "futures",
+ "libc",
+ "pyo3",
  "serde",
- "simple_logger",
- "spvn",
- "toml",
+ "serde_json",
+ "spvn_dev",
+ "spvn_serde",
+ "syncpool",
+ "tokio",
+ "tracing",
 ]
 
 [[package]]
 name = "spvn_cli"
-version = "0.1.0"
+version = "0.1.1-beta.1"
 dependencies = [
  "anyhow",
  "clap",
  "colored",
- "log",
- "simple_logger",
+ "futures",
+ "notify",
+ "num_cpus",
+ "pyo3",
+ "pyo3-build-config",
  "spvn",
  "spvn_caller",
- "spvn_cfg",
- "spvn_listen",
+ "spvn_serde",
  "tokio",
+ "tokio-rustls",
+ "tracing",
+ "tracing-subscriber",
 ]
 
 [[package]]
 name = "spvn_dev"
-version = "0.1.0"
+version = "0.1.1-beta.1"
 dependencies = [
- "log",
- "simple_logger",
- "spvn",
- "spvn_cfg",
- "spvn_cli",
+ "colored",
+ "tracing",
 ]
 
 [[package]]
-name = "spvn_lifespan"
-version = "0.1.0"
+name = "spvn_macros"
+version = "0.1.1-beta.1"
 dependencies = [
- "async-trait",
- "log",
+ "colored",
+ "crossbeam",
+ "futures",
+ "hyper",
  "pyo3",
- "pyo3-asyncio",
- "pythonize",
- "serde",
- "simple_logger",
- "tokio",
-]
-
-[[package]]
-name = "spvn_listen"
-version = "0.1.0"
-dependencies = [
- "anyhow",
+ "quote",
+ "syn 2.0.18",
  "tokio",
+ "tracing",
 ]
 
 [[package]]
-name = "spvn_log"
-version = "0.1.0"
+name = "spvn_serde"
+version = "0.1.1-beta.1"
 dependencies = [
+ "ahash",
+ "bytes",
+ "bytes-expand",
  "colored",
- "log",
- "simple_logger",
-]
-
-[[package]]
-name = "spvn_py"
-version = "0.1.0"
-dependencies = [
- "anyhow",
- "async-trait",
- "log",
+ "crossbeam",
+ "futures",
+ "http",
+ "hyper",
+ "libc",
  "pyo3",
- "pyo3-asyncio",
- "pythonize",
  "serde",
  "serde_json",
- "simple_logger",
+ "spvn_macros",
  "tokio",
+ "tracing",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
@@ -900,132 +1215,326 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.17"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45b6ddbb36c5b969c182aec3c4a0bce7df3fbad4b77114706a49aacc80567388"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syncpool"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "276c1fc00f41ad03bdcf390e81f967adfdb9c828c0a967e1c92df8050471c6bd"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
-name = "time"
-version = "0.3.21"
+name = "thread_local"
+version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
+checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
- "itoa",
+ "cfg-if",
+ "once_cell",
+]
+
+[[package]]
+name = "tokio"
+version = "1.28.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+dependencies = [
+ "autocfg",
+ "bytes",
  "libc",
- "num_threads",
- "serde",
- "time-core",
- "time-macros",
+ "mio",
+ "num_cpus",
+ "pin-project-lite",
+ "socket2 0.4.9",
+ "tokio-macros",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "time-core"
-version = "0.1.1"
+name = "tokio-macros"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
 
 [[package]]
-name = "time-macros"
-version = "0.2.9"
+name = "tokio-rustls"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+checksum = "e0d409377ff5b1e3ca6437aa86c1eb7d40c134bfec254e44c830defa92669db5"
 dependencies = [
- "time-core",
+ "rustls",
+ "tokio",
 ]
 
 [[package]]
-name = "tokio"
-version = "1.28.1"
+name = "tokio-stream"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
- "autocfg",
- "libc",
- "mio",
- "num_cpus",
+ "futures-core",
  "pin-project-lite",
- "socket2",
- "windows-sys 0.48.0",
+ "tokio",
 ]
 
 [[package]]
-name = "toml"
-version = "0.7.4"
+name = "tokio-util"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6135d499e69981f9ff0ef2167955a5333c35e36f6937d382974566b3d5b94ec"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
- "serde",
- "serde_spanned",
- "toml_datetime",
- "toml_edit",
+ "bytes",
+ "futures-core",
+ "futures-sink",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
 ]
 
 [[package]]
-name = "toml_datetime"
-version = "0.6.2"
+name = "tower"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
- "serde",
+ "futures-util",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
 ]
 
 [[package]]
-name = "toml_edit"
-version = "0.19.10"
+name = "tower-layer"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
+name = "tracing"
+version = "0.1.37"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
- "indexmap",
- "serde",
- "serde_spanned",
- "toml_datetime",
- "winnow",
+ "cfg-if",
+ "log",
+ "pin-project-lite",
+ "tracing-attributes",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-attributes"
+version = "0.1.24"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "tracing-core"
+version = "0.1.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+dependencies = [
+ "once_cell",
+ "valuable",
 ]
 
 [[package]]
+name = "tracing-log"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "78ddad33d2d10b1ed7eb9d1f518a5674713876e97e5bb9b7345a7984fbb4f922"
+dependencies = [
+ "lazy_static",
+ "log",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-subscriber"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
+dependencies = [
+ "nu-ansi-term",
+ "sharded-slab",
+ "smallvec",
+ "thread_local",
+ "tracing-core",
+ "tracing-log",
+]
+
+[[package]]
+name = "try-lock"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "untrusted"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
+
+[[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
+name = "valuable"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
+
+[[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
+name = "walkdir"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
+dependencies = [
+ "same-file",
+ "winapi-util",
+]
+
+[[package]]
+name = "want"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+dependencies = [
+ "log",
+ "try-lock",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.86"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+
+[[package]]
+name = "web-sys"
+version = "0.3.63"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -1034,33 +1543,27 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "winapi-util"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+dependencies = [
+ "winapi",
+]
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
@@ -1185,16 +1688,7 @@
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
-
-[[package]]
-name = "winnow"
-version = "0.4.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
-dependencies = [
- "memchr",
-]
```

### Comparing `spvn-0.1.0/python/spvn/__main__.py` & `spvn-0.1.1b1/src/spvn/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 import os
+import sys
 import sysconfig
 from pathlib import Path
 
 
 def get_binary() -> Path:
     exe = "spvn" + sysconfig.get_config_var("EXE")
     path = Path(sysconfig.get_path("scripts")) / exe
@@ -15,8 +15,8 @@
         return path
 
     raise FileNotFoundError(path)
 
 
 if __name__ == "__main__":
     spvn = get_binary()
-    sys.exit(os.spawnv(os.P_WAIT, spvn, ["spvn", *sys.argv[1:]]))
+    sys.exit(os.spawnv(os.P_WAIT, spvn, ["spvn", *sys.argv[1:]]))
```

