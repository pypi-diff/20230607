# Comparing `tmp/vlmc-0.1.5.tar.gz` & `tmp/vlmc-0.2.0.tar.gz`

## Comparing `vlmc-0.1.5.tar` & `vlmc-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 vlmc-0.1.5/Cargo.toml
--rw-r--r--   0     1001      123     2676 2023-06-06 17:44:45.000000 vlmc-0.1.5/.github/workflows/build_release.yml
--rw-r--r--   0     1001      123       43 2023-06-06 17:44:45.000000 vlmc-0.1.5/.gitignore
--rw-r--r--   0     1001      123     3951 2023-06-06 17:44:45.000000 vlmc-0.1.5/README.md
--rw-r--r--   0     1001      123       10 2023-06-06 17:46:47.000000 vlmc-0.1.5/dist/vlmc-0.1.5.tar.gz
--rw-r--r--   0     1001      123      571 2023-06-06 17:44:45.000000 vlmc-0.1.5/pyproject.toml
--rw-r--r--   0     1001      123     5537 2023-06-06 17:44:45.000000 vlmc-0.1.5/src/lib.rs
--rw-r--r--   0     1001      123     3439 2023-06-06 17:44:45.000000 vlmc-0.1.5/src/peres_shield.rs
--rw-r--r--   0     1001      123     9705 2023-06-06 17:44:45.000000 vlmc-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 vlmc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 vlmc-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2676 2023-06-07 16:01:27.000000 vlmc-0.2.0/.github/workflows/build_release.yml
+-rw-r--r--   0     1001      123       43 2023-06-07 16:01:27.000000 vlmc-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     4247 2023-06-07 16:01:27.000000 vlmc-0.2.0/README.md
+-rw-r--r--   0     1001      123       10 2023-06-07 16:03:21.000000 vlmc-0.2.0/dist/vlmc-0.2.0.tar.gz
+-rw-r--r--   0     1001      123      571 2023-06-07 16:01:27.000000 vlmc-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     5546 2023-06-07 16:01:27.000000 vlmc-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     3483 2023-06-07 16:01:27.000000 vlmc-0.2.0/src/peres_shield.rs
+-rw-r--r--   0     1001      123     9705 2023-06-07 16:03:20.000000 vlmc-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     4609 1970-01-01 00:00:00.000000 vlmc-0.2.0/PKG-INFO
```

### Comparing `vlmc-0.1.5/.github/workflows/build_release.yml` & `vlmc-0.2.0/.github/workflows/build_release.yml`

 * *Files identical despite different names*

### Comparing `vlmc-0.1.5/README.md` & `vlmc-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,106 +1,117 @@
 # Variable Length Markov Model (VLMC)
+
+[![Downloads](https://pepy.tech/badge/vlmc)](https://pepy.tech/project/vlmc) 
+[![PyPI version](https://badge.fury.io/py/vlmc.svg)](https://pypi.org/project/vlmc/)
+
 Implementation of Variable Length Markov Chains (VLMC) for Python.
-Suffix tree building is done top-down using the ![Peres-Shield](https://link.springer.com/chapter/10.1007/11557067_24) order estimation method.
-It is written in Rust and ported to Python with PyO3.
+Suffix tree building is done top-down using the [Peres-Shield](https://link.springer.com/chapter/10.1007/11557067_24) order estimation method.
+It is written in Rust with Python Bindings.
 
-## Installation
+##### Contents
+  - [Installation](#installation)
+    * [Compiling from source](#compilation-from-source)  
+  - [Usage](#usage)
+    - [`fit`](#fit)
+    - [`suffix`](#get_suffix)
+    - [`counts`](#get_counts)
+    - [`distribution`](#get_distribution)
+    - [`contexts`](#get_contexts)
+  - [Future](#todo)
 
-### Installation with pip 
+
+## Installation
 
 Pre-built packages for many Linux, Windows, and OSX systems are available
 in [PyPI](https://pypi.org/project/vlmc/) and can be installed with:
 
 ```sh
 pip install vlmc
 ```
 On uncommon architectures, you may need to first
-[install Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html)
-(i.e., the Rust programming language) first, and a subsequent
-`pip install vlmc` will try to compile the package for your CPU architecture and operating system.
-
+[install Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) before running `pip install vlmc`.
 ### Compilation from source
 
-You need to [install Rust/Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html).
-
-Installation uses [maturin](https://github.com/PyO3/maturin#maturin) for compiling and installing the Rust extension.
+In order to compile from source you will need to [install Rust/Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) and [maturin](https://github.com/PyO3/maturin#maturin) for the python bindings.
 Maturin is best used within a Python virtual environment:
 
 ```sh
 # activate your desired virtual environment first, then:
 pip install maturin
 git clone https://github.com/antonio-leitao/vlmc.git
 cd vlmc
 # build and install the package:
 maturin develop --release
 ```
 
-# Basic Usage
+# Usage
 
 ```python
 import vlmc
 tree = vlmc.VLMC(max_depth, alphabet_size, n_jobs=-1)
 ```
 Parameters:
 - `max_depth`: Maximum depth of tree. Subsequences whose length exceed the `max_depth` will not be considered nor counted. 
 - `alphabet_size`: Total number of symbols in the alphabet. This number has to be bigger than the highest integer encountered, else it will cause runtime errors. 
 - `n_jobs`: Number of subprocesses to spawn when running the vlmc. Choose `-1` for using all available processes.  
 
-# Methods
-
 ### `fit`
 
+> **Note**
+> fit method returns `None` and not `self`. This is by design as to not expose the rust object to python.
+
 ```python
 data = [
-[1,2,3],
-[2,3],
-[1,0,1],
-[2]
+  [1,2,3],
+  [2,3],
+  [1,0,1],
+  [2]
 ]
 
 tree.fit(data)
 ```
-> **Note**
-> fit method returns `None` and not `self`. This is by design as to not expose the rust object to python.
 
-Parameters:
+Arguments:
 - `data`: List of lists containing sequences of discrete values to fit on. Values are assumed to be integers form `0` to `alphabet_size`. List is expected to be two dimensional.
 
 ### `get_suffix`
 Given a sequence, returns the longest suffix that is present in the VLMC.
 
 ```python
 suffix = tree.get_suffix(sequence)
 ```
 Arguments:
 - `sequence`: list of integers representing a sequence of discrete varaibles. 
+
 Returns:
 - `suffix` : longest suffix of sequence that is present in the VLMC. 
 
 ### `get_counts`
 Gets the total number of occurences of a given sequence of integers.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 counts = tree.get_counts(sequence)
 ```
 Arguments:
-- `sequence`: list of integers representing a sequence of discrete varaibles. 
+- `sequence`: list of integers representing a sequence of discrete varaibles.
+ 
 Returns:
 - `counts` : integer 
 
 ### `get_distribution`
 Gets the vector of probabilities over the entire alphabet for the given sequence.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 probabilities = tree.get_distribution(sequence)
 ```
 Arguments:
 - `sequence`: list of integers representing a sequence of discrete variables. 
+
 Returns:
 - `probabilities` : list of floats representing the probability of observing a specific state (index) as the next symbol.
 
 ### `get_contexts`
 
 ```python
 contexts = tree.get_contexts()
@@ -110,7 +121,8 @@
 
 # TODO
 ### Paralelization
 After experimentation the best possible idea for paralelization would be to create different hashmaps for each sunsequence length.
 Hashmaps are then joined from longest to smallest.
 The hashmap at `max_depth + 1` can be discarded after.
 Could be very fast depending on merging algo.
+
```

### Comparing `vlmc-0.1.5/pyproject.toml` & `vlmc-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.maturin]
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 features = ["pyo3/extension-module"]
 
 [project]
 name = "vlmc"
-version = "0.1.5"
+version = "0.2.0"
 authors = [
   { name="António Leitão", email="aleitao@novaims.unl.pt" },
 ]
 description = "Variable Length Markov Chain"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `vlmc-0.1.5/src/lib.rs` & `vlmc-0.2.0/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,14 @@
                     node.distribution[element] += 1
                 }
             }
         }
     }
     let zero_node = Node {
         count: zero_counts,
-        precedents: HashSet::new(),
+        precedents: zero_successors.clone(),
         successors: zero_successors,
         distribution: zero_distribution,
     };
     counts.insert(vec![], zero_node);
     counts
 }
```

### Comparing `vlmc-0.1.5/src/peres_shield.rs` & `vlmc-0.2.0/src/peres_shield.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 use hashbrown::HashSet;
 use std::collections::VecDeque;
 
 impl VLMCObject {
     // Define additional methods here
     pub fn peres_shield_prune(&mut self) {
         //threshold parameters
-        let maximum_extension = (self.total_symbols as f32).log(10.0).log(10.0) as usize;
-        let divergence_threshold = (self.total_symbols as f32).powf(3.0 / 4.0);
+        let maximum_extension = (self.total_symbols as f32).log(10.0).log(10.0).ceil() as usize;
+        let divergence_threshold = (self.total_symbols as f32).powf(1.0 / 4.0);
         //instantiate data structures
         let mut definitive_seqs = HashSet::new();
         let mut queue = VecDeque::new();
         //Add the root node
         definitive_seqs.insert(vec![]);
         queue.push_back(vec![]);
 
@@ -35,15 +35,16 @@
                 queue.push_back(new_parent);
             }
         }
         //discard all but the ones we selected
         self.nodes.retain(|key, _| definitive_seqs.contains(key));
     }
     fn peres_shield_extend_sequence(
-        &self,
+        //FIXME &self when you finish debugging!!!!!!!!!!!
+        &mut self,
         parent_key: Vec<usize>,
         maximum_extension: usize,
         divergence_threshold: f32,
     ) -> Vec<Vec<usize>> {
         let mut queue = VecDeque::new();
         let mut accepted_sequences = Vec::new();
         let maximum_len = self.max_depth.min(parent_key.len() + maximum_extension);
@@ -62,28 +63,27 @@
                 queue.push_back(child_key.clone());
                 accepted_sequences.push(child_key);
             }
         }
         accepted_sequences
     }
 
-    fn peres_shield_divergence(&self, seq1: &Vec<usize>, seq2: &Vec<usize>) -> f32 {
-        let n_v = self.nodes.get(seq1).unwrap();
-        let n_w = self.nodes.get(seq2).unwrap();
+    fn peres_shield_divergence(&self, parent: &Vec<usize>, child: &Vec<usize>) -> f32 {
+        let n_v = self.nodes.get(child).unwrap();
+        let n_w = self.nodes.get(parent).unwrap();
         let mut max_divergence: f32 = 0.0;
 
         for successor in n_v.successors.union(&n_w.successors) {
             let divergence: f32;
-            let n_va = n_v.distribution[*successor];
-            let n_wa = n_w.distribution[*successor];
+            let n_va = n_v.distribution[*successor] as f32;
+            let n_wa = n_w.distribution[*successor] as f32;
             if n_w.count == 0 {
-                divergence = n_w.count as f32;
+                divergence = n_va;
             } else {
-                divergence =
-                    (n_va as f32 - (n_wa as f32 * n_v.count as f32 / n_w.count as f32)).abs();
+                divergence = (n_va - (n_wa * n_v.count as f32 / n_w.count as f32)).abs();
             }
             if divergence >= max_divergence {
                 max_divergence = divergence;
             }
         }
         max_divergence
     }
```

### Comparing `vlmc-0.1.5/Cargo.lock` & `vlmc-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "vlmc"
-version = "0.1.5"
+version = "0.2.0"
 dependencies = [
  "hashbrown",
  "pyo3",
  "rand",
 ]
 
 [[package]]
```

### Comparing `vlmc-0.1.5/PKG-INFO` & `vlmc-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,127 @@
 Metadata-Version: 2.1
 Name: vlmc
-Version: 0.1.5
+Version: 0.2.0
 Summary: Variable Length Markov Chain
 Author-email: António Leitão <aleitao@novaims.unl.pt>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/antonio-leitao/vlmc
 Project-URL: repository, https://github.com/antonio-leitao/vlmc
 
 # Variable Length Markov Model (VLMC)
+
+[![Downloads](https://pepy.tech/badge/vlmc)](https://pepy.tech/project/vlmc) 
+[![PyPI version](https://badge.fury.io/py/vlmc.svg)](https://pypi.org/project/vlmc/)
+
 Implementation of Variable Length Markov Chains (VLMC) for Python.
-Suffix tree building is done top-down using the ![Peres-Shield](https://link.springer.com/chapter/10.1007/11557067_24) order estimation method.
-It is written in Rust and ported to Python with PyO3.
+Suffix tree building is done top-down using the [Peres-Shield](https://link.springer.com/chapter/10.1007/11557067_24) order estimation method.
+It is written in Rust with Python Bindings.
 
-## Installation
+##### Contents
+  - [Installation](#installation)
+    * [Compiling from source](#compilation-from-source)  
+  - [Usage](#usage)
+    - [`fit`](#fit)
+    - [`suffix`](#get_suffix)
+    - [`counts`](#get_counts)
+    - [`distribution`](#get_distribution)
+    - [`contexts`](#get_contexts)
+  - [Future](#todo)
 
-### Installation with pip 
+
+## Installation
 
 Pre-built packages for many Linux, Windows, and OSX systems are available
 in [PyPI](https://pypi.org/project/vlmc/) and can be installed with:
 
 ```sh
 pip install vlmc
 ```
 On uncommon architectures, you may need to first
-[install Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html)
-(i.e., the Rust programming language) first, and a subsequent
-`pip install vlmc` will try to compile the package for your CPU architecture and operating system.
-
+[install Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) before running `pip install vlmc`.
 ### Compilation from source
 
-You need to [install Rust/Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html).
-
-Installation uses [maturin](https://github.com/PyO3/maturin#maturin) for compiling and installing the Rust extension.
+In order to compile from source you will need to [install Rust/Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) and [maturin](https://github.com/PyO3/maturin#maturin) for the python bindings.
 Maturin is best used within a Python virtual environment:
 
 ```sh
 # activate your desired virtual environment first, then:
 pip install maturin
 git clone https://github.com/antonio-leitao/vlmc.git
 cd vlmc
 # build and install the package:
 maturin develop --release
 ```
 
-# Basic Usage
+# Usage
 
 ```python
 import vlmc
 tree = vlmc.VLMC(max_depth, alphabet_size, n_jobs=-1)
 ```
 Parameters:
 - `max_depth`: Maximum depth of tree. Subsequences whose length exceed the `max_depth` will not be considered nor counted. 
 - `alphabet_size`: Total number of symbols in the alphabet. This number has to be bigger than the highest integer encountered, else it will cause runtime errors. 
 - `n_jobs`: Number of subprocesses to spawn when running the vlmc. Choose `-1` for using all available processes.  
 
-# Methods
-
 ### `fit`
 
+> **Note**
+> fit method returns `None` and not `self`. This is by design as to not expose the rust object to python.
+
 ```python
 data = [
-[1,2,3],
-[2,3],
-[1,0,1],
-[2]
+  [1,2,3],
+  [2,3],
+  [1,0,1],
+  [2]
 ]
 
 tree.fit(data)
 ```
-> **Note**
-> fit method returns `None` and not `self`. This is by design as to not expose the rust object to python.
 
-Parameters:
+Arguments:
 - `data`: List of lists containing sequences of discrete values to fit on. Values are assumed to be integers form `0` to `alphabet_size`. List is expected to be two dimensional.
 
 ### `get_suffix`
 Given a sequence, returns the longest suffix that is present in the VLMC.
 
 ```python
 suffix = tree.get_suffix(sequence)
 ```
 Arguments:
 - `sequence`: list of integers representing a sequence of discrete varaibles. 
+
 Returns:
 - `suffix` : longest suffix of sequence that is present in the VLMC. 
 
 ### `get_counts`
 Gets the total number of occurences of a given sequence of integers.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 counts = tree.get_counts(sequence)
 ```
 Arguments:
-- `sequence`: list of integers representing a sequence of discrete varaibles. 
+- `sequence`: list of integers representing a sequence of discrete varaibles.
+ 
 Returns:
 - `counts` : integer 
 
 ### `get_distribution`
 Gets the vector of probabilities over the entire alphabet for the given sequence.
 Will throw a `KeyError` if the sequence is not a tree node. Consider using `get_suffix` to make sure to get a tree node.
 
 ```python
 probabilities = tree.get_distribution(sequence)
 ```
 Arguments:
 - `sequence`: list of integers representing a sequence of discrete variables. 
+
 Returns:
 - `probabilities` : list of floats representing the probability of observing a specific state (index) as the next symbol.
 
 ### `get_contexts`
 
 ```python
 contexts = tree.get_contexts()
@@ -121,7 +132,8 @@
 # TODO
 ### Paralelization
 After experimentation the best possible idea for paralelization would be to create different hashmaps for each sunsequence length.
 Hashmaps are then joined from longest to smallest.
 The hashmap at `max_depth + 1` can be discarded after.
 Could be very fast depending on merging algo.
 
+
```

