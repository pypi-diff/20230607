# Comparing `tmp/mfhpo_simulator-1.0.0-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17516 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      483 b- defN 23-May-27 14:57 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     2715 b- defN 23-May-26 21:31 benchmark_simulator/_constants.py
+Zip file size: 17634 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      483 b- defN 23-Jun-07 06:50 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     2797 b- defN 23-May-28 09:29 benchmark_simulator/_constants.py
 -rw-rw-r--  2.0 unx     9482 b- defN 23-May-27 16:40 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1846 b- defN 23-May-25 06:25 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    27804 b- defN 23-May-27 16:40 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      871 b- defN 23-May-27 16:42 mfhpo_simulator-1.0.0.dist-info/RECORD
-10 files, 54380 bytes uncompressed, 16016 bytes compressed:  70.5%
+-rw-rw-r--  2.0 unx    28381 b- defN 23-May-28 09:34 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      871 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/RECORD
+10 files, 55039 bytes uncompressed, 16134 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-1.0.0.dist-info/LICENSE
+Filename: mfhpo_simulator-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.0.0.dist-info/METADATA
+Filename: mfhpo_simulator-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.0.0.dist-info/WHEEL
+Filename: mfhpo_simulator-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.0.0.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.0.0.dist-info/RECORD
+Filename: mfhpo_simulator-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import ObjectiveFuncType
 from benchmark_simulator.simulator import CentralWorkerManager, ObjectiveFuncWorker
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -20,14 +20,23 @@
 class _StateType:
     runtime: float = 0.0
     cumtime: float = 0.0
     fidel: int = 0
     seed: int | None = None
 
 
+@dataclass(frozen=True)
+class _InfoPaths:
+    proc_alloc: str
+    result: str
+    state_cache: str
+    worker_cumtime: str
+    timestamp: str
+
+
 class _SharedDataLocations(Enum):
     proc_alloc: str = "proc_alloc.json"
     result: str = "results.json"
     state_cache: str = "state_cache.json"
     worker_cumtime: str = "simulated_cumtime.json"
     timestamp: str = "timestamp.json"
 
@@ -37,14 +46,15 @@
     crashed: float = float(1 << 41)
 
 
 class ObjectiveFuncType(Protocol):
     def __call__(
         self,
         eval_config: dict[str, Any],
+        *,
         fidels: dict[str, int | float] | None = None,
         seed: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         """The prototype of the objective function.
 
         Args:
@@ -69,12 +79,9 @@
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
         raise NotImplementedError
 
 
-def _get_file_paths(dir_name: str) -> tuple[str, str, str, str, str]:
-    ret: tuple[str, str, str, str, str] = (
-        os.path.join(dir_name, fn.value) for fn in _SharedDataLocations
-    )  # type: ignore
-    return ret
+def _get_file_paths(dir_name: str) -> _InfoPaths:
+    return _InfoPaths(**{fn.name: os.path.join(dir_name, fn.value) for fn in _SharedDataLocations})
```

## benchmark_simulator/simulator.py

```diff
@@ -76,15 +76,14 @@
 from multiprocessing import Pool
 from typing import Any
 
 from benchmark_simulator._constants import (
     DIR_NAME,
     INF,
     ObjectiveFuncType,
-    _SharedDataLocations,
     _StateType,
     _TimeStampDictType,
     _TimeValue,
     _get_file_paths,
 )
 from benchmark_simulator._secure_proc import (
     _allocate_proc_to_worker,
@@ -109,29 +108,39 @@
 )
 from benchmark_simulator._utils import _generate_time_hash
 
 import numpy as np
 
 
 @dataclass(frozen=True)
-class _WrapperArgs:
+class _WrapperVars:
     subdir_name: str
     n_workers: int
     obj_func: ObjectiveFuncType
     n_actual_evals_in_opt: int
     n_evals: int
     obj_keys: list[str]
     runtime_key: str
     fidel_keys: list[str] | None
     seed: int | None
     continual_max_fidel: int | None
     max_waiting_time: float
     store_config: bool
 
 
+@dataclass(frozen=True)
+class _WorkerVars:
+    continual_eval: bool
+    worker_id: str
+    worker_index: int
+    rng: np.random.RandomState
+    use_fidel: bool
+    stored_obj_keys: list[str]
+
+
 class _BaseWrapperInterface(metaclass=ABCMeta):
     """A base wrapper class for each worker or manager.
     This wrapper class serves the shared interface of worker and manager class.
 
     Attributes:
         dir_name (str):
             The directory name where all the information will be stored.
@@ -209,29 +218,30 @@
                 The maximum waiting time to judge hang.
                 If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
             store_config (bool):
                 Whether to store all config/fidel information.
                 The information is sorted chronologically.
                 When you do large-scale experiments, this may incur too much storage consumption.
         """
-        self._wrapper_args = _WrapperArgs(
+        self._wrapper_vars = _WrapperVars(
             subdir_name=subdir_name,
             n_workers=n_workers,
             obj_func=obj_func,
             n_actual_evals_in_opt=n_actual_evals_in_opt,
             n_evals=n_evals,
             fidel_keys=fidel_keys,
             obj_keys=obj_keys,
             runtime_key=runtime_key,
             seed=seed,
             continual_max_fidel=continual_max_fidel,
             max_waiting_time=max_waiting_time,
             store_config=store_config,
         )
         self._dir_name = os.path.join(DIR_NAME, subdir_name)
+        self._paths = _get_file_paths(self.dir_name)
         self._obj_keys, self._runtime_key = obj_keys[:], runtime_key
         self._fidel_keys = [] if fidel_keys is None else fidel_keys[:]
         self._init_wrapper()
 
     @property
     def dir_name(self) -> str:
         return self._dir_name
@@ -255,240 +265,247 @@
 
 class ObjectiveFuncWorker(_BaseWrapperInterface):
     """A worker class for each worker.
     This worker class is supposed to be instantiated for each worker.
     For example, if we use 4 workers for an optimization, then four instances should be created.
     """
 
-    def _init_wrapper(self) -> None:
-        self._guarantee_no_hang()
-        self._worker_id = _generate_time_hash()
-        _, self._result_path, self._state_path, self._cumtime_path, self._timestamp_path = _get_file_paths(
-            self.dir_name
-        )
-        self._init_worker()
-
-        self._rng = np.random.RandomState(self._wrapper_args.seed)
-        self._use_fidel = self._wrapper_args.fidel_keys is not None
-        self._obj_func = self._wrapper_args.obj_func
-        self._stored_obj_keys = list(set(self.obj_keys + [self.runtime_key]))
-        self._index = self._alloc_index()
-        self._cumtime = 0.0
-        self._continual_eval = self._wrapper_args.continual_max_fidel is not None
-        self._terminated = False
-        self._crashed = False
-        self._used_config: dict[str, Any] = {}
-        self._validate_fidel_args()
-
     def __repr__(self) -> str:
-        return f"Worker-{self._worker_id}"
-
-    def _query_obj_func(
-        self,
-        eval_config: dict[str, Any],
-        fidels: dict[str, int | float] | None,
-        seed: int | None,
-        **data_to_scatter: Any,
-    ) -> dict[str, float]:
-        if self._wrapper_args.store_config:
-            self._used_config = eval_config.copy()
-            self._used_config.update(**(fidels if fidels is not None else {}), seed=seed)
-
-        return self._obj_func(eval_config=eval_config, fidels=fidels, seed=seed, **data_to_scatter)
+        return f"Worker-{self._worker_vars.worker_id}"
 
     def _guarantee_no_hang(self) -> None:
-        n_workers, n_evals = self._wrapper_args.n_workers, self._wrapper_args.n_evals
-        n_actual_evals_in_opt = self._wrapper_args.n_actual_evals_in_opt
+        n_workers, n_evals = self._wrapper_vars.n_workers, self._wrapper_vars.n_evals
+        n_actual_evals_in_opt = self._wrapper_vars.n_actual_evals_in_opt
         if n_actual_evals_in_opt < n_workers + n_evals:
             threshold = n_workers + n_evals
             # In fact, n_workers + n_evals - 1 is the real minimum threshold.
             raise ValueError(
                 "Cannot guarantee that optimziers will not hang. "
                 f"Use n_actual_evals_in_opt >= {threshold} (= n_evals + n_workers) at least. "
                 "Note that our package cannot change your optimizer setting, so "
                 "make sure that you changed your optimizer setting, but not only `n_actual_evals_in_opt`."
             )
 
-    def _validate_fidel_args(self) -> None:
-        # Guarantee the sufficiency: self._continual_eval ==> len(self._fidel_keys) == 1
-        if self._continual_eval and len(self._fidel_keys) != 1:
+    def _validate_fidel_args(self, continual_eval: bool) -> None:
+        # Guarantee the sufficiency: continual_eval ==> len(fidel_keys) == 1
+        if continual_eval and len(self._fidel_keys) != 1:
             raise ValueError(
                 f"continual_max_fidel is valid only if fidel_keys has only one element, but got {self._fidel_keys}"
             )
 
-    def _init_worker(self) -> None:
+    def _init_worker(self, worker_id: str) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
         _init_simulator(dir_name=self.dir_name)
-        _start_worker_timer(path=self._cumtime_path, worker_id=self._worker_id)
+        _start_worker_timer(path=self._paths.worker_cumtime, worker_id=worker_id)
 
-    def _alloc_index(self) -> int:
-        worker_id_to_index = _wait_all_workers(path=self._cumtime_path, n_workers=self._wrapper_args.n_workers)
+    def _alloc_index(self, worker_id: str) -> int:
+        worker_id_to_index = _wait_all_workers(path=self._paths.worker_cumtime, n_workers=self._wrapper_vars.n_workers)
         time.sleep(1e-2)  # buffer before the optimization
-        return worker_id_to_index[self._worker_id]
+        return worker_id_to_index[worker_id]
+
+    def _init_wrapper(self) -> None:
+        continual_eval = self._wrapper_vars.continual_max_fidel is not None
+        worker_id = _generate_time_hash()
+        self._guarantee_no_hang()
+        self._validate_fidel_args(continual_eval)
+        self._init_worker(worker_id)
+        worker_index = self._alloc_index(worker_id)
+        self._worker_vars = _WorkerVars(
+            continual_eval=continual_eval,
+            worker_id=worker_id,
+            worker_index=worker_index,
+            rng=np.random.RandomState(self._wrapper_vars.seed),
+            use_fidel=self._wrapper_vars.fidel_keys is not None,
+            stored_obj_keys=list(set(self.obj_keys + [self.runtime_key])),
+        )
+
+        # These variables change over time and must be either loaded from file system or updated.
+        self._cumtime = 0.0
+        self._terminated = False
+        self._crashed = False
+        self._used_config: dict[str, Any] = {}
+
+    def _validate(self, fidels: dict[str, int | float] | None) -> None:
+        if self._crashed:
+            raise InterruptedError(
+                "The simulation is interrupted due to deadlock or the dead of at least one of the workers.\n"
+                "This error could be avoided by increasing `max_waiting_time` (however, np.inf is discouraged).\n"
+            )
+        if not self._worker_vars.use_fidel and fidels is not None:
+            raise ValueError(
+                "Objective function got keyword `fidels`, but fidel_keys was not provided in worker instantiation."
+            )
+        if self._worker_vars.use_fidel and fidels is None:
+            raise ValueError(
+                "Objective function did not get keyword `fidels`, but fidel_keys was provided in worker instantiation."
+            )
+
+    def _validate_output(self, results: dict[str, float]) -> None:
+        keys_in_output = set(results.keys())
+        keys = set(self._worker_vars.stored_obj_keys)
+        if keys_in_output.intersection(keys) != keys:
+            raise KeyError(
+                f"The output of objective must be a superset of {list(keys)} specified in obj_keys and runtime_key, "
+                f"but got {results}"
+            )
 
-    def _get_init_state(self) -> tuple[_StateType, int | None]:
-        # initial seed, note: 1 << 30 is a huge number that fits 32bit.
-        init_state = _StateType(seed=self._rng.randint(1 << 30))
-        return init_state, None
+    @staticmethod
+    def _validate_provided_fidels(fidels: dict[str, int | float] | None) -> int:
+        if fidels is None or len(fidels.values()) != 1:
+            raise ValueError(
+                f"fidels must have only one element when continual_max_fidel is provided, but got {fidels}"
+            )
+
+        fidel = next(iter(fidels.values()))
+        if not isinstance(fidel, int):
+            raise ValueError(f"Fidelity for continual evaluation must be integer, but got {fidel}")
+        if fidel < 0:
+            raise ValueError(f"Fidelity for continual evaluation must be non-negative, but got {fidel}")
+
+        return fidel
 
     def _get_cached_state_and_index(self, config_hash: int, fidel: int) -> tuple[_StateType, int | None]:
-        cached_states = _fetch_cache_states(self._state_path, config_hash=config_hash)
+        cached_states = _fetch_cache_states(self._paths.state_cache, config_hash=config_hash)
         intermediate_avail = [state.cumtime <= self._cumtime and state.fidel < fidel for state in cached_states]
         cached_state_index = intermediate_avail.index(True) if any(intermediate_avail) else None
         if cached_state_index is None:
-            return self._get_init_state()
+            # initial seed, note: 1 << 30 is a huge number that fits 32bit.
+            init_state = _StateType(seed=self._worker_vars.rng.randint(1 << 30))
+            return init_state, None
         else:
             return cached_states[cached_state_index], cached_state_index
 
     def _update_state(
         self,
         config_hash: int,
         fidel: int,
         total_runtime: float,
         seed: int | None,
         cached_state_index: int | None,
     ) -> None:
-        kwargs = dict(path=self._state_path, config_hash=config_hash)
-        if fidel != self._wrapper_args.continual_max_fidel:  # update the cache data
+        kwargs = dict(path=self._paths.state_cache, config_hash=config_hash)
+        if fidel != self._wrapper_vars.continual_max_fidel:  # update the cache data
             new_state = _StateType(runtime=total_runtime, cumtime=self._cumtime, fidel=fidel, seed=seed)
             _cache_state(new_state=new_state, update_index=cached_state_index, **kwargs)
         elif cached_state_index is not None:  # if None, newly start and train till the end, so no need to delete.
             _delete_state(index=cached_state_index, **kwargs)
 
-    def _validate_output(self, results: dict[str, float]) -> None:
-        keys_in_output = set(results.keys())
-        keys = set(self._stored_obj_keys)
-        if keys_in_output.intersection(keys) != keys:
-            raise KeyError(
-                f"The output of objective must be a superset of {list(keys)} specified in obj_keys and runtime_key, "
-                f"but got {results}"
-            )
+    def _wait_other_workers(self) -> None:
+        """
+        Wait until the worker's cumulative runtime becomes the smallest.
+        The smallest cumulative runtime implies that the order in the record will not disturbed
+        even if the worker reports its results now.
+        """
+        wait_start, worker_id = time.time(), self._worker_vars.worker_id
+        max_waiting_time = self._wrapper_vars.max_waiting_time
+        _wait_until_next(path=self._paths.worker_cumtime, worker_id=worker_id, max_waiting_time=max_waiting_time)
+        _record_timestamp(
+            path=self._paths.timestamp,
+            worker_id=worker_id,
+            prev_timestamp=time.time(),
+            waited_time=time.time() - wait_start,
+        )
+
+    def _query_obj_func(
+        self,
+        eval_config: dict[str, Any],
+        fidels: dict[str, int | float] | None,
+        seed: int | None,
+        **data_to_scatter: Any,
+    ) -> dict[str, float]:
+        if self._wrapper_vars.store_config:
+            self._used_config = eval_config.copy()
+            self._used_config.update(**(fidels if fidels is not None else {}), seed=seed)
+
+        return self._wrapper_vars.obj_func(eval_config=eval_config, fidels=fidels, seed=seed, **data_to_scatter)
 
     def _proc_output_from_scratch(
         self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
     ) -> dict[str, float]:
         _fidels: dict[str, int | float] = {} if fidels is None else fidels.copy()
-        if self._use_fidel and set(_fidels.keys()) != set(self._fidel_keys):
+        if self._worker_vars.use_fidel and set(_fidels.keys()) != set(self._fidel_keys):
             raise KeyError(f"The keys in fidels must be identical to fidel_keys, but got {fidels}")
 
-        seed = self._rng.randint(1 << 30)
+        seed = self._worker_vars.rng.randint(1 << 30)
         results = self._query_obj_func(eval_config=eval_config, seed=seed, fidels=fidels, **data_to_scatter)
         self._validate_output(results)
-        self._cumtime += results[self._runtime_key]
-        return {k: results[k] for k in self._stored_obj_keys}
+        self._cumtime += results[self.runtime_key]
+        return {k: results[k] for k in self._worker_vars.stored_obj_keys}
 
     def _proc_output_from_existing_state(
         self, eval_config: dict[str, Any], fidel: int, **data_to_scatter: Any
     ) -> dict[str, float]:
         config_hash: int = hash(str(eval_config))
         cached_state, cached_state_index = self._get_cached_state_and_index(config_hash=config_hash, fidel=fidel)
         _fidels: dict[str, int | float] = {self._fidel_keys[0]: fidel}
         results = self._query_obj_func(
             eval_config=eval_config, seed=cached_state.seed, fidels=_fidels, **data_to_scatter
         )
         self._validate_output(results)
-        total_runtime = results[self._runtime_key]
+        total_runtime = results[self.runtime_key]
         actual_runtime = max(0.0, total_runtime - cached_state.runtime)
         self._cumtime += actual_runtime
         self._update_state(
             total_runtime=total_runtime,
             cached_state_index=cached_state_index,
             seed=cached_state.seed,
             config_hash=config_hash,
             fidel=fidel,
         )
-        return {**{k: results[k] for k in self._obj_keys}, self._runtime_key: actual_runtime}
-
-    def _validate_provided_fidels(self, fidels: dict[str, int | float] | None) -> int:
-        if fidels is None or len(fidels.values()) != 1:
-            raise ValueError(
-                f"fidels must have only one element when continual_max_fidel is provided, but got {fidels}"
-            )
-
-        fidel = next(iter(fidels.values()))
-        if not isinstance(fidel, int):
-            raise ValueError(f"Fidelity for continual evaluation must be integer, but got {fidel}")
-        if fidel < 0:
-            raise ValueError(f"Fidelity for continual evaluation must be non-negative, but got {fidel}")
-
-        return fidel
+        return {**{k: results[k] for k in self._obj_keys}, self.runtime_key: actual_runtime}
 
     def _proc_output(
         self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
     ) -> dict[str, float]:
-        if not self._continual_eval:
+        if not self._worker_vars.continual_eval:
             return self._proc_output_from_scratch(eval_config=eval_config, fidels=fidels, **data_to_scatter)
 
         # Otherwise, we try the continual evaluation
         fidel = self._validate_provided_fidels(fidels)
         return self._proc_output_from_existing_state(eval_config=eval_config, fidel=fidel, **data_to_scatter)
 
-    def _wait_other_workers(self) -> None:
-        """
-        Wait until the worker's cumulative runtime becomes the smallest.
-        The smallest cumulative runtime implies that the order in the record will not disturbed
-        even if the worker reports its results now.
-        """
-        wait_start = time.time()
-        max_waiting_time = self._wrapper_args.max_waiting_time
-        _wait_until_next(path=self._cumtime_path, worker_id=self._worker_id, max_waiting_time=max_waiting_time)
-        _record_timestamp(
-            path=self._timestamp_path,
-            worker_id=self._worker_id,
-            prev_timestamp=time.time(),
-            waited_time=time.time() - wait_start,
-        )
-
     def _post_proc(self, results: dict[str, float]) -> None:
         # First, record the simulated cumulative runtime after calling the objective
-        _record_cumtime(path=self._cumtime_path, worker_id=self._worker_id, cumtime=self._cumtime)
+        _record_cumtime(path=self._paths.worker_cumtime, worker_id=self._worker_vars.worker_id, cumtime=self._cumtime)
         # Wait till the cumulative runtime becomes the smallest
         self._wait_other_workers()
 
         row = dict(
-            cumtime=self._cumtime, index=self._index, **{k: results[k] for k in self._obj_keys}, **self._used_config
+            cumtime=self._cumtime,
+            worker_index=self._worker_vars.worker_index,
+            **{k: results[k] for k in self._obj_keys},
+            **self._used_config,
         )
         # Record the results to the main database when the cumulative runtime is the smallest
-        _record_result(self._result_path, results=row, fixed=bool(not self._wrapper_args.store_config))
+        _record_result(self._paths.result, results=row, fixed=bool(not self._wrapper_vars.store_config))
         self._used_config = {}  # Make it empty
-        if _is_simulator_terminated(self._result_path, max_evals=self._wrapper_args.n_evals):
+        if _is_simulator_terminated(self._paths.result, max_evals=self._wrapper_vars.n_evals):
             self._finish()
 
     def _load_timestamps(self) -> _TimeStampDictType:
-        timestamp_dict = _fetch_timestamps(self._timestamp_path)
-        if self._worker_id not in timestamp_dict:  # Initialize the timestamp
+        timestamp_dict, worker_id = _fetch_timestamps(self._paths.timestamp), self._worker_vars.worker_id
+        if worker_id not in timestamp_dict:  # Initialize the timestamp
             init_timestamp = _TimeStampDictType(prev_timestamp=time.time(), waited_time=0.0)
             _start_timestamp(
-                path=self._timestamp_path, worker_id=self._worker_id, prev_timestamp=init_timestamp.prev_timestamp
+                path=self._paths.timestamp, worker_id=worker_id, prev_timestamp=init_timestamp.prev_timestamp
             )
             return init_timestamp
 
-        timestamp = timestamp_dict[self._worker_id]
-        self._cumtime = _fetch_cumtimes(self._cumtime_path)[self._worker_id]
+        timestamp = timestamp_dict[worker_id]
+        self._cumtime = _fetch_cumtimes(self._paths.worker_cumtime)[worker_id]
         self._terminated = self._cumtime >= _TimeValue.terminated.value - 1e-5
         self._crashed = self._cumtime >= _TimeValue.crashed.value - 1e-5
         return timestamp
 
-    def _validate(self, fidels: dict[str, int | float] | None) -> None:
-        if self._crashed:
-            raise InterruptedError(
-                "The simulation is interrupted due to deadlock or the dead of at least one of the workers.\n"
-                "This error could be avoided by increasing `max_waiting_time` (however, np.inf is discouraged).\n"
-            )
-        if not self._use_fidel and fidels is not None:
-            raise ValueError(
-                "Objective function got keyword `fidels`, but fidel_keys was not provided in worker instantiation."
-            )
-        if self._use_fidel and fidels is None:
-            raise ValueError(
-                "Objective function did not get keyword `fidels`, but fidel_keys was provided in worker instantiation."
-            )
-
     def __call__(
-        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None = None, **data_to_scatter: Any
+        self,
+        eval_config: dict[str, Any],
+        *,
+        fidels: dict[str, int | float] | None = None,
+        **data_to_scatter: Any,
     ) -> dict[str, float]:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
         If not called, optimization modules are likely to hang at the end.
 
         Args:
             eval_config (dict[str, Any]):
@@ -510,29 +527,29 @@
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
         timestamp = self._load_timestamps()
         self._validate(fidels=fidels)
         if self._terminated:
-            return {**{k: INF for k in self._obj_keys}, self._runtime_key: INF}
+            return {**{k: INF for k in self._obj_keys}, self.runtime_key: INF}
 
         sampling_time = max(0.0, time.time() - timestamp.prev_timestamp - timestamp.waited_time)
         self._cumtime += sampling_time
 
         results = self._proc_output(eval_config, fidels, **data_to_scatter)
         self._post_proc(results)
         return results
 
     def _finish(self) -> None:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
         If not called, optimization modules are likely to hang.
         """
-        _finish_worker_timer(path=self._cumtime_path, worker_id=self._worker_id)
+        _finish_worker_timer(path=self._paths.worker_cumtime, worker_id=self._worker_vars.worker_id)
         self._terminated = True
 
 
 class CentralWorkerManager(_BaseWrapperInterface):
     """A central worker manager class.
     This class is supposed to be instantiated if the optimizer module uses multiprocessing.
     For example, Dask, multiprocessing, and joblib would need this class.
@@ -548,31 +565,35 @@
 
     def _init_workers(self) -> None:
         if os.path.exists(self.dir_name):
             raise FileExistsError(f"The directory `{self.dir_name}` already exists. Remove it first.")
 
         pool = Pool()
         results = []
-        for _ in range(self._wrapper_args.n_workers):
-            results.append(pool.apply_async(ObjectiveFuncWorker, kwds=self._wrapper_args.__dict__))
+        for _ in range(self._wrapper_vars.n_workers):
+            results.append(pool.apply_async(ObjectiveFuncWorker, kwds=self._wrapper_vars.__dict__))
 
         pool.close()
         pool.join()
         self._workers = [result.get() for result in results]
 
     def _init_alloc(self, pid: int) -> None:
-        _path = os.path.join(self._dir_name, _SharedDataLocations.proc_alloc.value)
-        if not _is_allocation_ready(path=_path, n_workers=self._wrapper_args.n_workers):
-            _allocate_proc_to_worker(path=_path, pid=pid)
-            self._pid_to_index = _wait_proc_allocation(path=_path, n_workers=self._wrapper_args.n_workers)
+        path = self._paths.proc_alloc
+        if not _is_allocation_ready(path=path, n_workers=self._wrapper_vars.n_workers):
+            _allocate_proc_to_worker(path=path, pid=pid)
+            self._pid_to_index = _wait_proc_allocation(path=path, n_workers=self._wrapper_vars.n_workers)
         else:
-            self._pid_to_index = _fetch_proc_alloc(path=_path)
+            self._pid_to_index = _fetch_proc_alloc(path=path)
 
     def __call__(
-        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None = None, **data_to_scatter: Any
+        self,
+        eval_config: dict[str, Any],
+        *,
+        fidels: dict[str, int | float] | None = None,
+        **data_to_scatter: Any,
     ) -> dict[str, float]:
         """The meta-wrapper method of the objective function method in WorkerFunc instances.
 
         This method recognizes each WorkerFunc by process ID and call the corresponding worker based on the ID.
 
         Args:
             eval_config (dict[str, Any]):
@@ -593,15 +614,15 @@
             results (dict[str, float]):
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
         pid = os.getpid()
         pid = threading.get_ident() if pid == self._main_pid else pid
-        if len(self._pid_to_index) != self._wrapper_args.n_workers:
+        if len(self._pid_to_index) != self._wrapper_vars.n_workers:
             self._init_alloc(pid)
 
         if pid not in self._pid_to_index:
             raise ProcessLookupError(
                 f"An unknown process/thread with ID {pid} was specified.\n"
                 "It is likely that one of the workers crashed and a new worker was added.\n"
                 f"However, worker additions are not allowed in {self.__class__.__name__}."
```

## Comparing `mfhpo_simulator-1.0.0.dist-info/LICENSE` & `mfhpo_simulator-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-1.0.0.dist-info/RECORD` & `mfhpo_simulator-1.0.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-benchmark_simulator/__init__.py,sha256=_scJ9QFQlCNO-SOP0IiXA2v12vtmbUYmRB6MFEwtPoI,483
-benchmark_simulator/_constants.py,sha256=gaepOQcAjQ93qam80HE0EPI1-DqSZWOPpGF2jbbwmk8,2715
+benchmark_simulator/__init__.py,sha256=Pu7318Lf3aAu3i2O5x3mR6JiWz-VAUPQ3MCgNI3mxO4,483
+benchmark_simulator/_constants.py,sha256=QcxWnAEPfhh-h9Es0LY0otgG6cVWwG54Y9sGcEjX-0M,2797
 benchmark_simulator/_secure_proc.py,sha256=ywV45-q1pUC-tHI_tiHgRH_8BKpMmhXttuJPOf5Bpqw,9482
 benchmark_simulator/_utils.py,sha256=SBu3r9mAYgwgB2CLo4YVxGcSthUZOO8quyX7cGbikks,1846
-benchmark_simulator/simulator.py,sha256=4CfuY4g8S-v18NZq6vF_1_0YwQXuIAUfv9eHvNEh7mA,27804
-mfhpo_simulator-1.0.0.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-1.0.0.dist-info/METADATA,sha256=_2cuQ-5Qc6skGeTcHPcIb7SLp3qyRg6FTZ040rKKtQg,307
-mfhpo_simulator-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_simulator-1.0.0.dist-info/top_level.txt,sha256=pT5LiPwT78978UOly1oZst_RacTpjrU_SDaUE8xvA_c,20
-mfhpo_simulator-1.0.0.dist-info/RECORD,,
+benchmark_simulator/simulator.py,sha256=T6n3xA0UHgXRtv4LRDEMtuLVzTH3BmB60IWgaI0G84Q,28381
+mfhpo_simulator-1.0.1.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-1.0.1.dist-info/METADATA,sha256=UgXuiNVF2R-kvIyG2VE72MUHOJwRT5eTfRpZ3AqCusM,307
+mfhpo_simulator-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_simulator-1.0.1.dist-info/top_level.txt,sha256=pT5LiPwT78978UOly1oZst_RacTpjrU_SDaUE8xvA_c,20
+mfhpo_simulator-1.0.1.dist-info/RECORD,,
```

