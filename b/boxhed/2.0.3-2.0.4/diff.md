# Comparing `tmp/boxhed-2.0.3.tar.gz` & `tmp/boxhed-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxhed-2.0.3.tar", last modified: Thu Mar 23 16:31:58 2023, max compression
+gzip compressed data, was "boxhed-2.0.4.tar", last modified: Wed Jun  7 00:13:45 2023, max compression
```

## Comparing `boxhed-2.0.3.tar` & `boxhed-2.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-03-23 16:31:58.475507 boxhed-2.0.3/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-03-08 18:09:37.000000 boxhed-2.0.3/MANIFEST.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-03-23 16:31:58.475507 boxhed-2.0.3/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      825 2023-03-08 18:09:37.000000 boxhed-2.0.3/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-03-23 16:31:58.475507 boxhed-2.0.3/boxhed/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-03-08 18:09:37.000000 boxhed-2.0.3/boxhed/__init__.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17805 2023-03-23 16:29:04.000000 boxhed-2.0.3/boxhed/boxhed.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12520 2023-03-08 18:09:37.000000 boxhed-2.0.3/boxhed/model_selection.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4305 2023-03-08 18:09:37.000000 boxhed-2.0.3/boxhed/utils.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-03-23 16:31:58.475507 boxhed-2.0.3/boxhed.egg-info/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-03-23 16:31:58.000000 boxhed-2.0.3/boxhed.egg-info/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-03-23 16:31:58.000000 boxhed-2.0.3/boxhed.egg-info/SOURCES.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-03-23 16:31:58.000000 boxhed-2.0.3/boxhed.egg-info/dependency_links.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-03-23 16:31:58.000000 boxhed-2.0.3/boxhed.egg-info/not-zip-safe
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       70 2023-03-23 16:31:58.000000 boxhed-2.0.3/boxhed.egg-info/requires.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        7 2023-03-23 16:31:58.000000 boxhed-2.0.3/boxhed.egg-info/top_level.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-03-23 16:31:58.475507 boxhed-2.0.3/setup.cfg
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      664 2023-03-23 16:29:20.000000 boxhed-2.0.3/setup.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:13:45.258593 boxhed-2.0.4/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-05-30 19:24:43.000000 boxhed-2.0.4/MANIFEST.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 00:13:45.258593 boxhed-2.0.4/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      825 2023-05-30 19:24:43.000000 boxhed-2.0.4/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:13:45.258593 boxhed-2.0.4/boxhed/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-05-30 19:24:43.000000 boxhed-2.0.4/boxhed/__init__.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18195 2023-06-07 00:02:32.000000 boxhed-2.0.4/boxhed/boxhed.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14339 2023-05-30 19:24:43.000000 boxhed-2.0.4/boxhed/model_selection.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4836 2023-05-30 19:24:43.000000 boxhed-2.0.4/boxhed/utils.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-07 00:13:45.258593 boxhed-2.0.4/boxhed.egg-info/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      980 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/not-zip-safe
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       70 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/requires.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        7 2023-06-07 00:13:45.000000 boxhed-2.0.4/boxhed.egg-info/top_level.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-06-07 00:13:45.258593 boxhed-2.0.4/setup.cfg
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      664 2023-06-07 00:11:22.000000 boxhed-2.0.4/setup.py
```

### Comparing `boxhed-2.0.3/PKG-INFO` & `boxhed-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxhed
-Version: 2.0.3
+Version: 2.0.4
 Summary: BoXHED2.0
 Author: Arash Pakbin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 **B**oosted e**X**act **H**azard **E**stimator with **D**ynamic covariates v2.0 (BoXHED2.0, pronounced 'box-head') is a software package for nonparametrically estimating hazard functions via gradient boosted trees. BoXHED2.0 accommodates both time-static and time-dependent covariates.
```

### Comparing `boxhed-2.0.3/README.md` & `boxhed-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `boxhed-2.0.3/boxhed/boxhed.py` & `boxhed-2.0.4/boxhed/boxhed.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,29 @@
         self.max_depth     = max_depth
         self.n_estimators  = n_estimators
         self.eta           = eta
         self.gpu_id        = gpu_id
         self.nthread       = nthread
 
 
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        out = ""
+        for line in [
+                "a BoXHED estimator instance",
+                f"    max_depth:    {self.max_depth}",
+                f"    n_estimators: {self.n_estimators}",
+                f"    eta:          {self.eta}"
+            ]:
+            out += line+"\n"
+        return out
+
+
     def _X_y_to_dmat(self, X, y=None, w=None):
         if not hasattr(self, 'X_colnames'):
             self.X_colnames = None #model probably created for CV, no need for data name matching
         dmat = xgb.DMatrix(pd.DataFrame(X, columns=self.X_colnames))
 
         if (y is not None):
             dmat.set_float_info('label',  y)
```

### Comparing `boxhed-2.0.3/boxhed/model_selection.py` & `boxhed-2.0.4/boxhed/model_selection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-from boxhed.boxhed import boxhed
-
-
-from sklearn.utils import indexable
+import os
+import copy
 import numpy as np
+from tqdm import tqdm
 import multiprocessing as mp
+from itertools import product
+from boxhed.boxhed import boxhed
+from boxhed.utils import temp_seed
+from multiprocessing import Manager
+from sklearn.utils import indexable
 from joblib import Parallel, delayed
-import numpy as np
-import copy
-from tqdm import tqdm
+from multiprocessing.shared_memory import SharedMemory
+from multiprocessing.managers import SharedMemoryManager
 #'''
-import os
 #TODO: CAN I DO ANYTHING ABOUT OMP_NUM_THREADS
 os.environ['OMP_NUM_THREADS'] = "1"
 #'''
-from itertools import product
-from multiprocessing import Manager
-from multiprocessing.shared_memory import SharedMemory
-from multiprocessing.managers import SharedMemoryManager
-from sklearn.model_selection import GroupKFold 
-
-
+#from sklearn.model_selection import GroupKFold
 
 def _to_shared_mem(smm, arr_np):
     shared_mem       = smm.SharedMemory(size=arr_np.nbytes)
     arr_np_shared    = np.ndarray(shape = arr_np.shape, dtype = arr_np.dtype, buffer = shared_mem.buf)
     arr_np_shared[:] = arr_np[:]
     return shared_mem
 
@@ -57,54 +53,63 @@
     delta = np.ndarray(shape = delta_shape, dtype = delta_dtype, buffer = smem_delta.buf)
 
 
 
     def _fit_single_model(param_dict):
         estimator = boxhed()
         estimator.set_params(**param_dict)
-        
+
         fold = param_dict["fold"]
         estimator.fit(X    [data_idx[fold]['train'], :], 
                       delta[data_idx[fold]['train']],
                       w    [data_idx[fold]['train']])
 
         return estimator
 
 
-    def _fill_rslt(rslt_idx):
-        est_idx   = rslt_idx // test_block_size
-        test_idx  = rslt_idx %  test_block_size
+    def _get_score_batch_est_test(idx_dict):
+        est_idx   = idx_dict['est_idx']
+        test_idx  = idx_dict['test_idx']
         abs_idx   = batch_idx*batch_size+est_idx
-
-        est       = trained_models[est_idx]
         test_dict = param_dicts_test[test_block_size*abs_idx + test_idx]
 
         n_trees = test_dict['n_estimators']
         fold    = test_dict['fold']
 
-        score = est.score(
+        est       = trained_models[est_idx]
+        
+        return est.score(
             X    [data_idx[fold]['test'], :], 
             delta[data_idx[fold]['test']],
             w    [data_idx[fold]['test']],
             ntree_limit = n_trees)
 
-        rslts[test_block_size*abs_idx+test_idx] = score
-
-
-    def _fill_rslts():
-
-        Parallel(n_jobs = -1, prefer = "threads")(delayed (_fill_rslt)(rslt_idx) for rslt_idx in range(test_block_size*len(trained_models)))
-
+    def _get_score_batch_est(idx_dicts):
+        scores = [None] * len(idx_dicts)
+        for i, idx_dict in enumerate(idx_dicts):
+            scores[i] = _get_score_batch_est_test(idx_dict)
+        return scores
+
+
+    def _fill_rslt():
+        batch_block_size = test_block_size*len(trained_models)
+        idx_dicts = [{"est_idx": rslt_idx // test_block_size, "test_idx":rslt_idx % test_block_size} 
+            for rslt_idx in range(batch_block_size)]
+        idx_dicts = [idx_dicts[i : i + test_block_size] for i in range(0, len(idx_dicts), test_block_size)]
+        scores = Parallel(n_jobs = batch_size, prefer = "threads")(delayed (_get_score_batch_est)(idx_dicts_) 
+            for idx_dicts_ in idx_dicts)
+        scores = [item for sublist in scores for item in sublist]
+        rslts [batch_block_size*batch_idx:batch_block_size*(batch_idx+1)] = scores
 
+    
     trained_models = Parallel(n_jobs=-1, prefer="threads")(delayed(_fit_single_model)(param_dict) 
             for param_dict in param_dicts_train[batch_idx*batch_size:
                 (batch_idx+1)*batch_size])
 
-
-    _fill_rslts()
+    _fill_rslt()
 
 
 class collapsed_gs_:
 
     def _remove_keys(self, dict_, keys):
         dict_ = copy.copy(dict_)
         for key in keys:
@@ -132,15 +137,14 @@
         self.batch_size = batch_size
         self.model_per_gpu = batch_size//len(GPU_LIST)
         
         self.collapsed     = 'n_estimators'
         self.not_collapsed = 'max_depth'
 
         self.param_grid_train = copy.copy(self.param_grid)
-        #self.param_grid_fit["fold"] = [x for x in range(len(cv))]
 
         self.param_grid_train[self.collapsed] = [
                 max(self.param_grid_train[self.collapsed])
                 ]
 
         self.GPU_LIST = GPU_LIST
 
@@ -150,15 +154,14 @@
         self.param_dicts_test = self._make_indiv_dicts(self.param_grid)
 
         self.param_dicts_test.sort(key=lambda dict_: 
                 (dict_[self.not_collapsed], dict_['fold']))
 
         self.test_block_size = len(self.param_grid[self.collapsed])
 
-        #raise
         self.cv         = cv
 
         self.data_idx   = {}
         self._fill_data_idx()
 
         manager                = Manager()
         self.rslts             = manager.list(['0']*len(self.param_dicts_test))
@@ -175,19 +178,16 @@
                     self.GPU_LIST[(idx // self.model_per_gpu) 
                         % len(self.GPU_LIST)]
                     })
 
         return dicts
 
 
-    #TODO: what if it was on CPU?
     def _batched_train_test(self):
 
-        #batch_size = len(self.GPU_LIST)*self.model_per_gpu
-
         smm = SharedMemoryManager()
         smm.start()
 
         X_shared     = _to_shared_mem(smm, self.X)
         w_shared     = _to_shared_mem(smm, self.w)
         delta_shared = _to_shared_mem(smm, self.delta)
 
@@ -218,20 +218,24 @@
                 param_dict_mngd['batch_idx'] = batch_idx
 
                 '''
                 _run_batch_process(param_dict_mngd, rslt_mngd)
                 print (rslt_mngd)
                 raise
                 '''
+
                 p = mp.Process(target = _run_batch_process, args = (param_dict_mngd, rslt_mngd))
 
                 p.start() 
                 p.join()
+                
                 p.terminate()
-
+                if p.exitcode != 0:
+                    raise MemoryError("ERROR: Cross validation did not finish successfully due to memory error. Consider reducing nthread and/or models_per_gpu to cut down on the memory used by cross validation.")
+            
             smm.shutdown()
             
             self.rslts = list(rslt_mngd)
 
     def _calculate_output_statistics(self):
         def sort_pred(dict_):
             return (dict_['max_depth'], dict_['n_estimators'], dict_['fold'])
@@ -257,30 +261,56 @@
 
 
     def fit(self, X, w, delta):
         self.X     = np.array(X)
         self.w     = np.array(w)
         self.delta = np.array(delta)
 
-
         self._batched_train_test()
 
         self._calculate_output_statistics()
 
 
         return {
             "params":          np.array(self.srtd_param_dict_test, dtype='object'),
             "mean_test_score": self.srtd_param_dict_test_scores,
             "std_test_score":  self.srtd_param_dict_test_std,
             "se_test_score":   self.srtd_param_dict_test_std/np.sqrt(len(self.cv)),
             "best_params":     self.srtd_param_dict_test[np.argmax(self.srtd_param_dict_test_scores)]
         }
 
 
-def cv(param_grid, X_post, num_folds, gpu_list, nthread=-1, models_per_gpu=1):
+def group_k_fold(ID, num_folds, seed=None):
+    ID             = ID.astype(int)
+    ID_unique_srtd = np.sort(np.unique(ID))
+
+    ID_counts = [len(ID_unique_srtd)//num_folds] * num_folds
+    for i in range(len(ID_unique_srtd)%num_folds):
+        ID_counts[i]+=1
+
+    assert sum(ID_counts)==len(ID_unique_srtd)
+
+    fold_idxs = np.hstack([[i]*id_count for i, id_count in enumerate(ID_counts)])
+
+    if seed is not None:
+        with temp_seed(seed):
+            np.random.shuffle(fold_idxs)
+    else:
+        np.random.shuffle(fold_idxs)
+
+    gkf = []
+    for fold_idx in range(num_folds):
+        train_ids = ID_unique_srtd[np.where(fold_idxs!=fold_idx)[0]]
+        test_ids  = ID_unique_srtd[np.where(fold_idxs==fold_idx)[0]]
+        gkf.append((np.where(np.isin(ID, train_ids))[0], np.where(np.isin(ID, test_ids))[0]))
+    
+    return gkf
+
+
+def cv(param_grid, X_post, num_folds, gpu_list, nthread=-1, models_per_gpu=1, seed=None, ID=None):
     """cross validate different hyperpatameter combinations based on likelihood risk.
 
     :param param_grid: a dictionary containing candidate values for the hyperparameters to cross-validate on. An example would be:
     param_grid = {
         'max_depth':    [1, 2, 3, 4, 5],
         'n_estimators': [50, 100, 150, 200, 250, 300],
         'eta':          [0.1]
@@ -307,24 +337,34 @@
     """
 
     if gpu_list == [-1]:
         batch_size = nthread if nthread != -1 else mp.cpu_count()-1
     else:
         batch_size = models_per_gpu * len(gpu_list)
 
-    X, w, delta, ID = indexable(X_post['X'], X_post['w'], X_post['delta'], X_post['ID'])
+    X, w, delta, ID_ = indexable(X_post['X'], X_post['w'], X_post['delta'], X_post['ID'])
 
-    gkf = list(GroupKFold(n_splits=num_folds).split(X,delta,ID))
+    ID = ID_ if ID is None else ID
+    
+    gkf = group_k_fold(ID, num_folds, seed)
 
     collapsed_ntree_gs_  = collapsed_gs_(param_grid, gkf, gpu_list, batch_size)
  
-    results     = collapsed_ntree_gs_.fit(X,w,delta)
-    means       = results['mean_test_score']
-    stds        = results['std_test_score']
-    params      = results['params']
+    try:
+        results     = collapsed_ntree_gs_.fit(X,w,delta)
+        means       = results['mean_test_score']
+        stds        = results['std_test_score']
+        params      = results['params']
+
+    except MemoryError as me:
+        print (me)
+        means       = np.array([])
+        stds        = np.array([])
+        params      = np.array([])
+
 
     return {"params":params , "score_mean":means, "score_ste":stds/np.sqrt(num_folds)}
 
 
 def best_param_1se_rule(cv_results, model_complexity, bounded_search=True):
     params, means, stes               = [cv_results[key] for key in ["params", "score_mean", "score_ste"]]
     highest_mean_idx                  = np.argmax(means)
```

### Comparing `boxhed-2.0.3/boxhed/utils.py` & `boxhed-2.0.4/boxhed/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from datetime import datetime
 from pytz import timezone
 import os
+import contextlib
 import numpy as np
-from sklearn.model_selection import StratifiedKFold
+#from sklearn.model_selection import StratifiedKFold
 from py3nvml import get_free_gpus
 import pickle
-from joblib import Parallel, delayed
-import itertools
-from collections import namedtuple
+#from joblib import Parallel, delayed
+#import itertools
+#from collections import namedtuple
 from scipy.stats import beta # beta distribution.
 import math
 
 
 import warnings
 warnings.simplefilter(action='ignore', category=Warning)
 
-import pandas as pd
+#import pandas as pd
 from pathlib import Path
 import sys
 sys.path.append(os.path.join(os.path.expanduser("~"), "survival_analysis/BoXHED2.0/xgboost/python-package/"))
 
 CACHE_ADDRESS = './tmp/'
 
 # calc_L2: calculate L2 distance and its 95% confidence interval.
@@ -113,18 +114,18 @@
         return round(time_now()-self.t_start, 3)
 
 def create_dir_if_not_exist(path):
     if not os.path.exists(path):
         os.makedirs(path)
 
 import functools
-import multiprocessing
-from sys import platform
-if platform == "linux" or platform == "linux2":
-    multiprocessing.set_start_method('fork', force=True)
+#import multiprocessing
+#from sys import platform
+#if platform == "linux" or platform == "linux2":
+#    multiprocessing.set_start_method('fork', force=True)
 from multiprocessing import Process, Queue
 
 
 def run_as_process(func):
     @functools.wraps(func)
     def run_as_process(*args, **kwargs):
 
@@ -160,7 +161,31 @@
         pickle.dump(obj, handle)
 
 
 def load_pickle(addr):
     with open(addr, 'rb') as handle:
         obj = pickle.load(handle)
     return obj
+
+
+from threading import Thread
+def run_as_threads(f, args_dict_list):
+
+    T = []
+    for args_dict in args_dict_list:
+        t=Thread(target = f, kwargs = args_dict)
+        t.start()
+        T.append(t)
+
+    for t in T:
+        t.join()
+
+
+#https://stackoverflow.com/questions/49555991/can-i-create-a-local-numpy-random-seed
+@contextlib.contextmanager
+def temp_seed(seed):
+    state = np.random.get_state()
+    np.random.seed(seed)
+    try:
+        yield
+    finally:
+        np.random.set_state(state)
```

### Comparing `boxhed-2.0.3/boxhed.egg-info/PKG-INFO` & `boxhed-2.0.4/boxhed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxhed
-Version: 2.0.3
+Version: 2.0.4
 Summary: BoXHED2.0
 Author: Arash Pakbin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 **B**oosted e**X**act **H**azard **E**stimator with **D**ynamic covariates v2.0 (BoXHED2.0, pronounced 'box-head') is a software package for nonparametrically estimating hazard functions via gradient boosted trees. BoXHED2.0 accommodates both time-static and time-dependent covariates.
```

### Comparing `boxhed-2.0.3/setup.py` & `boxhed-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="boxhed",
-    version="2.0.3",
+    version="2.0.4",
     long_description=long_description,
     long_description_content_type='text/markdown',
     description="BoXHED2.0",
     author='Arash Pakbin',
     packages=find_packages(),
     python_requires=">=3.8",
     include_package_data=True,
```

