# Comparing `tmp/sybil-scorer-0.1.1.tar.gz` & `tmp/sybil-scorer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-scorer-0.1.1.tar", last modified: Mon May  8 09:47:39 2023, max compression
+gzip compressed data, was "sybil-scorer-0.1.3.tar", last modified: Wed Jun  7 16:11:51 2023, max compression
```

## Comparing `sybil-scorer-0.1.1.tar` & `sybil-scorer-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 09:47:39.037737 sybil-scorer-0.1.1/
--rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     9689 2023-05-08 09:47:39.037737 sybil-scorer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.1.1/README.md
--rw-rw-rw-   0        0        0     1142 2023-05-08 09:46:03.000000 sybil-scorer-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-08 09:47:38.978854 sybil-scorer-0.1.1/sbscorer/
-drwxrwxrwx   0        0        0        0 2023-05-08 09:47:38.990856 sybil-scorer-0.1.1/sbscorer/sbdata/
--rw-rw-rw-   0        0        0    22880 2023-05-08 09:36:36.000000 sybil-scorer-0.1.1/sbscorer/sbdata/FlipsideApi.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.1/sbscorer/sbdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:47:39.001869 sybil-scorer-0.1.1/sbscorer/sblegos/
--rw-rw-rw-   0        0        0    30403 2023-02-16 10:48:13.000000 sybil-scorer-0.1.1/sbscorer/sblegos/TransactionAnalyser.py
--rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.1.1/sbscorer/sblegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:47:39.012289 sybil-scorer-0.1.1/sbscorer/sbutils/
--rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.1.1/sbscorer/sbutils/LoadData.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.1/sbscorer/sbutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:47:39.035773 sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/
--rw-rw-rw-   0        0        0     9689 2023-05-08 09:47:38.000000 sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-05-08 09:47:38.000000 sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:47:38.000000 sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-05-08 09:47:38.000000 sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-08 09:47:38.000000 sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      748 2023-05-08 09:47:39.039736 sybil-scorer-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.988542 sybil-scorer-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     9689 2023-06-07 16:11:50.989545 sybil-scorer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1142 2023-06-07 16:06:07.000000 sybil-scorer-0.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.906542 sybil-scorer-0.1.3/sbscorer/
+drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.938541 sybil-scorer-0.1.3/sbscorer/sbdata/
+-rw-rw-rw-   0        0        0    22880 2023-05-08 09:36:36.000000 sybil-scorer-0.1.3/sbscorer/sbdata/FlipsideApi.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.3/sbscorer/sbdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.942541 sybil-scorer-0.1.3/sbscorer/sblegos/
+-rw-rw-rw-   0        0        0    18460 2023-06-07 16:04:36.000000 sybil-scorer-0.1.3/sbscorer/sblegos/TransactionAnalyser.py
+-rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.1.3/sbscorer/sblegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.946539 sybil-scorer-0.1.3/sbscorer/sbutils/
+-rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.1.3/sbscorer/sbutils/LoadData.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.1.3/sbscorer/sbutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 16:11:50.986542 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/
+-rw-rw-rw-   0        0        0     9689 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-07 16:11:50.000000 sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      748 2023-06-07 16:11:51.003541 sybil-scorer-0.1.3/setup.cfg
```

### Comparing `sybil-scorer-0.1.1/LICENSE` & `sybil-scorer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.1/PKG-INFO` & `sybil-scorer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.1.1
+Version: 0.1.3
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.1.1/README.md` & `sybil-scorer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.1/pyproject.toml` & `sybil-scorer-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ['setuptools>=61.0.0', "wheel"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "sybil-scorer"
-version = "0.1.1"
+version = "0.1.3"
 description = "A sybil scoring tool"
 readme = "README.md"
 authors = [{ name = "Poupou", email = "poupou-web3@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Sybil", "OSS", "Gitcoin", "Quadratic"]
 dependencies = [
     "pandas==2.0.1",
-    "flipside==2.0.3",
+    "flipside>=2.0.7",
     'tomli; python_version < "3.11"',
     'pylcs==0.0.8',
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black",
```

### Comparing `sybil-scorer-0.1.1/sbscorer/sbdata/FlipsideApi.py` & `sybil-scorer-0.1.3/sbscorer/sbdata/FlipsideApi.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.1/sbscorer/sblegos/TransactionAnalyser.py` & `sybil-scorer-0.1.3/sbscorer/sblegos/TransactionAnalyser.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         ----------
         df_transactions : pd.DataFrame
             The dataframe containing all the transactions of the addresses
         df_address : pd.DataFrame
             The dataframe containing a 'address' column 
         """
         self.df_transactions = df_transactions
-        # holds a df of address/seed wallet so we don't have to create it each time
+        # holds a df of address/seed wallet we don't have to create it each time
         self.df_seed_wallet_naive = None
         self.df_seed_wallet = None
         self.gb_EOA_sorted = None
         self.df_address = df_address
-        # We use a df address so we can load all transactions in memmory and then change the address list easily
+        # We use a df address we can load all transactions in memory and then change the address list easily
         # for example to calculate on a specific project
 
         # store the array of string transactions
         self.dict_add_string_tx = None
         self.dict_add_value_string_tx = None
 
     def has_same_seed_naive(self, address):
@@ -152,15 +152,15 @@
         if self.gb_EOA_sorted is None:
             self.set_group_by_sorted_EOA()
         self.df_seed_wallet_naive = self.gb_EOA_sorted.first().loc[:, ['from_address', 'to_address']]
 
     def set_seed_wallet(self):
         """
         Set the df_seed_wallet attribute of the class. It holds the seed wallet of the addresses in 'EOA'
-        of df_transactions. It is a non naive method that look for the first incoming transaction of the address to get
+        of df_transactions. It is a non-naive method that look for the first incoming transaction of the address to get
         the seed wallet.
         Returns
         -------
         None
             Set the df_seed_wallet attribute of the class
         """
         df_filtered = self.df_transactions[self.df_transactions['EOA'] == self.df_transactions['to_address']]
@@ -229,17 +229,18 @@
         Returns
         -------
         contributors : narray
             The array of contributors of the grant
         """
         return self.df_transactions['EOA'].unique()
 
-    def transaction_similitude(self, address, algo_type="address_only", char_tolerance=0):
+    def transaction_similitude_pylcs(self, address, algo_type="address_only", minimum_sim_tx=5):
         """
         Return a boolean and the list of addresses if it finds other addresses with similar actions.
+        it first stores some repetitive tasks into a class attribute and then use it to speed up the process.
 
         The algorithm is the following:
         1. Transform all transactions in to a String of the form: "from_address,
         to_address, from_address, to_address, ..."
         2. Replace the address of the wallet by "x" to ba able to compare the behavior of two addresses.
         3. Run the algorithm common longest substring on all the transactions
         4. If the longest common substring is longer than 5, return true for the current address.
@@ -250,82 +251,16 @@
         Parameters
         ----------
         address : str
             The address to check
         algo_type : str
             The type of algorithm to use. Default is "address_only" which only use the address to compare.
             options are: address_only, address_and_value
-        char_tolerance : int
-            The number of character to skip when using the longest common substring algorithm. Default is 0.
-            1 may be a good choice when algo_type is "address_and_value".
-
-        Returns
-        -------
-        has_similar_behavior : bool
-            True if the address has similar behavior as another address
-        score_similar_behavior : float
-            The similarity score of the address
-        list_similar_address : map
-            The map of address and their similarity score
-
-        """
-
-        # Get all the transactions of the address in a 1D array
-        df_address_transactions = self.get_address_transactions(address)
-        shape_target = df_address_transactions.shape[0]
-        min_shape = max(1, shape_target / 3)
-        max_shape = max(shape_target, shape_target * 3)
-        array_transactions_target = self.get_array_transactions(df_address_transactions, address, algo_type)
-
-        # Get all the transactions from other contributors into an 1D array
-        df_other_address = self.df_address.loc[self.df_address['address'] != address, :]
-        df_other_address['lcs'] = 0
-        df_other_address.set_index('address', inplace=True)
-        for add, df_other_address_transactions in self.gb_EOA_sorted:
-            if add != address:
-                shape_other = df_other_address_transactions.shape[0]
-                if shape_other <= 1:
-                    df_other_address.loc[add, 'lcs'] = 0
-                elif min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too
-                    # different shapes
-                    array_transactions_other = self.get_array_transactions(df_other_address_transactions, add,
-                                                                           algo_type)
-                    lcs = self.longest_common_sub_string(array_transactions_target, array_transactions_other,
-                                                         char_tolerance)
-                    df_other_address.loc[add, 'lcs'] = lcs
-                else:
-                    df_other_address.loc[add, 'lcs'] = 0
-
-        df_similar_address = df_other_address.loc[df_other_address['lcs'] > 5, :]
-        df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
-            lambda x: min(x / (len(array_transactions_target) / 2), 1))
-        return df_similar_address
-
-    def transaction_similitude_opti(self, address, algo_type="address_only", char_tolerance=0):
-        """
-        Return a boolean and the list of addresses if it finds other addresses with similar actions.
-        it first store some repetitive tasks into a class variable and then use it to speed up the process.
-
-        The algorithm is the following:
-        1. Transform all transactions in to a String of the form: "from_address,
-        to_address, from_address, to_address, ..."
-        2. Replace the address of the wallet by "x" to ba able to compare the behavior of two addresses.
-        3. Run the algorithm common longest substring on all the transactions
-        4. If the longest common substring is longer than 5, return true for the current address.
-        5. Keep iterating to find the longest common substring and then the score is
-        the length of the longest common substring divided by half the length of the target address string.
-        The score is the min(score, 1) to avoid having a score > 1.
-
-        Parameters
-        ----------
-        address : str
-            The address to check
-        algo_type : str
-            The type of algorithm to use. Default is "address_only" which only use the address to compare.
-            options are: address_only, address_and_value
+        minimum_sim_tx : int
+            The number of transactions to use to compare. Default is 5.
         char_tolerance : int
             The number of character to skip when using the longest common substring algorithm. Default is 0.
             1 may be a good choice when algo_type is "address_and_value".
 
         Returns
         -------
         has_similar_behavior : bool
@@ -334,134 +269,58 @@
             The similarity score of the address
         list_similar_address : map
             The map of address and their similarity score
 
         """
 
         # Transform all transactions into a 1D string
-        if algo_type == "address_only" and self.dict_add_string_tx is None:
-            self.set_dict_add_string_transactions(algo_type)
-        elif algo_type == "address_and_value" and self.dict_add_value_string_tx is None:
-            self.set_dict_add_string_transactions(algo_type)
-        else:
-            Exception("algo_type not supported")
-
-        # Get all the transactions of the address in a 1D array
         if algo_type == "address_only":
-            array_transactions_target = self.dict_add_string_tx.get(address)
+            if self.dict_add_string_tx is None:
+                self.set_dict_add_string_transactions(algo_type)
+            str_transactions_target = self.dict_add_string_tx.get(address)
         elif algo_type == "address_and_value":
-            array_transactions_target = self.dict_add_value_string_tx.get(address)
-
-        shape_target = array_transactions_target.shape[0]
-        min_shape = max(1, shape_target / 4)
-        max_shape = max(shape_target, shape_target * 3)
-
-        # Get all the transactions from other contributors into an 1D array
-        df_other_address = self.df_address.loc[self.df_address['address'] != address, :]
-        df_other_address['lcs'] = 0
-        df_other_address.set_index('address', inplace=True)
-        for add in df_other_address.index:
-            df_other_address_transactions = self.get_address_transactions(add)
-            shape_other = df_other_address_transactions.shape[0]
-            if df_other_address_transactions.shape[0] <= 1:
-                df_other_address.loc[add, 'lcs'] = 0
-            elif min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too different shapes
-                if algo_type == "address_only":
-                    array_transactions_other = self.dict_add_string_tx.get(add)
-                elif algo_type == "address_and_value":
-                    array_transactions_other = self.dict_add_value_string_tx.get(add)
-                lcs = self.longest_common_sub_string(array_transactions_target, array_transactions_other,
-                                                     char_tolerance)
-                df_other_address.loc[add, 'lcs'] = lcs
-            else:
-                df_other_address.loc[add, 'lcs'] = 0
-
-        df_similar_address = df_other_address.loc[df_other_address['lcs'] > 5, :]
-        df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
-            lambda x: min(x / (len(array_transactions_target) / 2), 1))
-        return df_similar_address
-
-    def transaction_similitude_pylcs(self, address, algo_type="address_only"):
-        """
-        Return a boolean and the list of addresses if it finds other addresses with similar actions.
-        it first store some repetitive tasks into a class attribute and then use it to speed up the process.
-
-        The algorithm is the following:
-        1. Transform all transactions in to a String of the form: "from_address,
-        to_address, from_address, to_address, ..."
-        2. Replace the address of the wallet by "x" to ba able to compare the behavior of two addresses.
-        3. Run the algorithm common longest substring on all the transactions
-        4. If the longest common substring is longer than 5, return true for the current address.
-        5. Keep iterating to find the longest common substring and then the score is
-        the length of the longest common substring divided by half the length of the target address string.
-        The score is the min(score, 1) to avoid having a score > 1.
-
-        Parameters
-        ----------
-        address : str
-            The address to check
-        algo_type : str
-            The type of algorithm to use. Default is "address_only" which only use the address to compare.
-            options are: address_only, address_and_value
-        char_tolerance : int
-            The number of character to skip when using the longest common substring algorithm. Default is 0.
-            1 may be a good choice when algo_type is "address_and_value".
-
-        Returns
-        -------
-        has_similar_behavior : bool
-            True if the address has similar behavior as another address
-        score_similar_behavior : float
-            The similarity score of the address
-        list_similar_address : map
-            The map of address and their similarity score
-
-        """
-
-        # Transform all transactions into a 1D string
-        if algo_type == "address_only" and self.dict_add_string_tx is None:
-            self.set_dict_add_string_transactions(algo_type)
-        elif algo_type == "address_and_value" and self.dict_add_value_string_tx is None:
-            self.set_dict_add_string_transactions(algo_type)
+            if self.dict_add_value_string_tx is None:
+                self.set_dict_add_string_transactions(algo_type)
+            # Get all the transactions of the address in a 1D array
+            str_transactions_target = self.dict_add_value_string_tx.get(address)
         else:
             Exception("algo_type not supported")
 
-        # Get all the transactions of the address in a 1D array
-        if algo_type == "address_only":
-            array_transactions_target = self.dict_add_string_tx.get(address)
-        elif algo_type == "address_and_value":
-            array_transactions_target = self.dict_add_value_string_tx.get(address)
-
-        shape_target = array_transactions_target.shape[0]
+        shape_target = self.get_address_transactions(address).shape[0]
         min_shape = max(1, shape_target / 4)
         max_shape = max(shape_target, shape_target * 3)
 
-        # Get all the transactions from other contributors into an 1D array
-        df_other_address = self.df_address.loc[self.df_address['address'] != address, :]
-        df_other_address['lcs'] = 0
-        df_other_address.set_index('address', inplace=True)
-        for add in df_other_address.index:
-            df_other_address_transactions = self.get_address_transactions(add)
-            shape_other = df_other_address_transactions.shape[0]
-            if df_other_address_transactions.shape[0] <= 1:
-                df_other_address.loc[add, 'lcs'] = 0
-            elif min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too different shapes
-                if algo_type == "address_only":
-                    array_transactions_other = self.dict_add_string_tx.get(add)
-                elif algo_type == "address_and_value":
-                    array_transactions_other = self.dict_add_value_string_tx.get(add)
-                lcs = self.longest_common_sub_string_pylcs(array_transactions_target, array_transactions_other)
-                df_other_address.loc[add, 'lcs'] = lcs
+        if self.df_address.columns != ['address']:
+            self.df_address.columns = ['address']
+        list_lcs = []
+        for add in self.df_address['address']:
+            if add != address:
+                shape_other = self.get_address_transactions(add).shape[0]
+                if min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too different shapes
+                    if algo_type == "address_only":
+                        str_transactions_other = self.dict_add_string_tx.get(add)
+                    else:
+                        str_transactions_other = self.dict_add_value_string_tx.get(add)
+                    lcs = self.longest_common_sub_string_pylcs(str_transactions_target, str_transactions_other)
+                    list_lcs.append(lcs)
+                else:
+                    list_lcs.append(0)
             else:
-                df_other_address.loc[add, 'lcs'] = 0
+                list_lcs.append(0)
 
-        df_similar_address = df_other_address.loc[df_other_address['lcs'] > 5, :]
+        if minimum_sim_tx == -1:
+            mask = np.array(list_lcs) > max(3, min(10, shape_target / 4))
+        else:
+            mask = np.array(list_lcs) > minimum_sim_tx
+        df_similar_address = self.df_address.loc[mask, :].copy()
+        df_similar_address['lcs'] = np.array(list_lcs)[mask]
+        len_tx = len(str_transactions_target) / 2  # Divide by 2 because we have from_address and to_address
         df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
-            lambda x: min(x / (len(array_transactions_target) / 2), 1))
-        return df_similar_address
+            lambda x: min(x / len_tx, 1))
+        return df_similar_address.set_index('address')
 
     @staticmethod
     def get_array_transactions(df_address_transactions, address, algo_type="address_only"):
         """
         This method replace the target address by an arbitrary "x" to be able to compare the similitude of two wallet.
 
         Parameters
@@ -502,82 +361,36 @@
                     .values
             except Exception as e:
                 array_transactions = []
         else:
             raise ValueError("algo_type must be either address_only or address_and_value")
         return array_transactions
 
-    def has_transaction_similitude(self, address, algo_type="address_only", char_tolerance=0):
-        """
-        Return a boolean whether the address has similar behavior as another address.
-        The algorithm check against all addresses in df_transactions using transaction_similitude
-
-        Parameters
-        ----------
-        algo_type : str
-            The type of algorithm to use. Default is "address_only".
-        char_tolerance : int
-            The number of character to skip when using the longest common substring algorithm. Default is 0.
-        address : str
-            The address to check
-
-        Returns
-        -------
-        has_similar_behavior : bool
-            True if the address has similar transactional behavior as another address
-
-        """
-        df_similar_address = self.transaction_similitude(address, algo_type=algo_type, char_tolerance=char_tolerance)
-        return df_similar_address.shape[0] > 0
-
-    def has_transaction_similitude_opti(self, address, algo_type="address_only", char_tolerance=0):
-        """
-        Return a boolean whether the address has similar behavior as another address.
-        The algorithm check against all addresses in df_transactions using transaction_similitude
-
-        Parameters
-        ----------
-        algo_type : str
-            The type of algorithm to use. Default is "address_only".
-        char_tolerance : int
-            The number of character to skip when using the longest common substring algorithm. Default is 0.
-        address : str
-            The address to check
-
-        Returns
-        -------
-        has_similar_behavior : bool
-            True if the address has similar transactional behavior as another address
-
-        """
-        df_similar_address = self.transaction_similitude_opti(address,
-                                                              algo_type=algo_type,
-                                                              char_tolerance=char_tolerance)
-        return df_similar_address.shape[0] > 0
-
     def get_address_transactions(self, address):
         """
         Get transactions of an address from the self.df_transaction df using the group by
         Parameters
         ----------
         address : str
             The address to retrieve transactions
 
         Returns
         -------
         df : pd.DataFrame
             The data frame with the transactions of the address
 
         """
-        if self.gb_EOA_sorted is None:
-            self.set_group_by_sorted_EOA()
         try:
             df = self.gb_EOA_sorted.get_group(address)
         except Exception as e:
-            df = pd.DataFrame()
+            if self.gb_EOA_sorted is None:
+                self.set_group_by_sorted_EOA()
+                df = self.get_address_transactions(address)
+            else:
+                df = pd.DataFrame()
         return df
 
     def get_address_transactions_add(self, df, address):
         """
         Get transactions of an address from a dataframe df
         Parameters
         ----------
@@ -591,67 +404,14 @@
         -------
         df : pd.DataFrame
             The data frame with the transactions of the address
 
         """
         return df[self.df_transactions['EOA'] == address]
 
-    @staticmethod
-    def longest_common_sub_string(target_array, comp_array, char_tolerance=0):
-        """
-        This method return the length of the longest common substring between two arrays of strings.
-        Parameters
-        ----------
-        target_array : narray
-            The array of strings to compare
-        comp_array : narray
-            The array of strings to compare
-        char_tolerance : int
-            The number of character to skip when comparing two strings not available yet
-        Returns
-        -------
-        lcs : int
-            The length of the longest common substring
-        """
-
-        if char_tolerance == 0:
-            m = len(comp_array)
-            n = len(target_array)
-            # dp will store solutions as the iteration goes on
-            dp = np.zeros((2, m + 1), dtype=int)
-
-            res = 0
-
-            for i in range(1, n + 1):
-                for j in range(1, m + 1):
-                    if target_array[i - 1] == comp_array[j - 1]:
-                        dp[i % 2][j] = dp[(i - 1) % 2][j - 1] + 1
-                        if dp[i % 2][j] > res:
-                            res = dp[i % 2][j]
-                    else:
-                        dp[i % 2][j] = 0
-            return res
-
-        else:
-            substring = []
-            longest = 0
-            for i in range(len(input)):
-                c_set = set()
-                for j in range(i, len(input)):
-                    c_set.add(input[j])
-                    if len(c_set) > 2:
-                        break
-                    if j + 1 - i == longest:
-                        substring.append(input[i:j + 1])
-                    if j + 1 - i > longest:
-                        longest = j + 1 - i
-                        substring = []
-                        substring.append(input[i:j + 1])
-            return len(substring)
-
     def set_dict_add_string_transactions(self, algo_type="address_only"):
         """
         This method create a dictionary with the address as key and the array of transactions as value.
         The array of transactions is the array crated with the get_array_transactions method.
         Parameters
         ----------
         algo_type : str
@@ -677,18 +437,16 @@
         else:
             raise ValueError("algo_type must be either address_only or address_and_value")
 
     def get_dict_string_tx(self, gb_address, algo_type="address_only"):
         dict_string_tx = {}
         for address, df_address in gb_address:
             array_transactions = self.get_array_transactions(df_address, address, algo_type)
-            dict_string_tx[address] = array_transactions
+            dict_string_tx[address] = "".join(array_transactions)
         return dict_string_tx
 
     @staticmethod
-    def longest_common_sub_string_pylcs(array_transactions_target, array_transactions_other):
-        string_target = "".join(array_transactions_target)
-        string_other = "".join(array_transactions_other)
+    def longest_common_sub_string_pylcs(string_target, string_other):
 
         # 1 similar transaction equals to 8 first char of the address + "-" + "x" = 10 char
         lcs = pylcs.lcs_string_length(string_target, string_other)
         return lcs // 10  # quotient of the division
```

### Comparing `sybil-scorer-0.1.1/sbscorer/sbutils/LoadData.py` & `sybil-scorer-0.1.3/sbscorer/sbutils/LoadData.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.1.1/sbscorer/sybil_scorer.egg-info/PKG-INFO` & `sybil-scorer-0.1.3/sbscorer/sybil_scorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.1.1
+Version: 0.1.3
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.1.1/setup.cfg` & `sybil-scorer-0.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7962 696c 2d73 636f 7265 720d   = sybil-scorer.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e31  .version = 0.1.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e33  .version = 0.1.3
 00000030: 0d0a 6175 7468 6f72 203d 2050 6f75 706f  ..author = Poupo
 00000040: 750d 0a61 7574 686f 725f 656d 6169 6c20  u..author_email 
 00000050: 3d20 706f 7570 6f75 2d77 6562 3340 7072  = poupou-web3@pr
 00000060: 6f74 6f6e 6d61 696c 2e63 6f6d 0d0a 6465  otonmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7379  scription = A sy
 00000080: 6269 6c20 7363 6f72 696e 6720 746f 6f6c  bil scoring tool
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

