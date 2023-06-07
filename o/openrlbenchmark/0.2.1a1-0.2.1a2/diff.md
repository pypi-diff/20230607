# Comparing `tmp/openrlbenchmark-0.2.1a1.tar.gz` & `tmp/openrlbenchmark-0.2.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrlbenchmark-0.2.1a1.tar", max compression
+gzip compressed data, was "openrlbenchmark-0.2.1a2.tar", max compression
```

## Comparing `openrlbenchmark-0.2.1a1.tar` & `openrlbenchmark-0.2.1a2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.1a1/LICENSE
--rw-r--r--   0        0        0    19299 2023-06-06 15:14:33.209492 openrlbenchmark-0.2.1a1/README.md
--rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.1a1/openrlbenchmark/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.1a1/openrlbenchmark/cache.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.1a1/openrlbenchmark/cache_legacy.py
--rw-r--r--   0        0        0     6147 2023-05-01 14:06:32.647152 openrlbenchmark-0.2.1a1/openrlbenchmark/capped_hns.py
--rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.1a1/openrlbenchmark/hns.py
--rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.1a1/openrlbenchmark/offline_db.py
--rw-r--r--   0        0        0    36839 2023-06-06 16:06:15.870857 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops.py
--rw-r--r--   0        0        0    30368 2023-06-05 02:01:01.027169 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_hns.py
--rw-r--r--   0        0        0    25008 2023-06-06 20:21:31.794579 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_multi_metrics.py
--rw-r--r--   0        0        0    36984 2023-06-06 15:06:30.132573 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl.py
--rw-r--r--   0        0        0    25220 2023-06-07 11:59:12.598806 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl_multi_metrics.py
--rw-r--r--   0        0        0     2074 2023-06-06 20:28:58.991774 openrlbenchmark-0.2.1a1/openrlbenchmark/test.json
--rw-r--r--   0        0        0      748 2023-06-07 15:34:13.833615 openrlbenchmark-0.2.1a1/pyproject.toml
--rw-r--r--   0        0        0    20262 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.1a2/LICENSE
+-rw-r--r--   0        0        0    20353 2023-06-07 20:05:43.595075 openrlbenchmark-0.2.1a2/README.md
+-rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.1a2/openrlbenchmark/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.1a2/openrlbenchmark/cache.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.1a2/openrlbenchmark/cache_legacy.py
+-rw-r--r--   0        0        0     6147 2023-06-07 19:47:32.024056 openrlbenchmark-0.2.1a2/openrlbenchmark/capped_hns.py
+-rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.1a2/openrlbenchmark/hns.py
+-rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.1a2/openrlbenchmark/offline_db.py
+-rw-r--r--   0        0        0    36776 2023-06-07 20:11:32.988139 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops.py
+-rw-r--r--   0        0        0    30367 2023-06-07 20:11:32.994334 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_hns.py
+-rw-r--r--   0        0        0    24942 2023-06-07 20:11:32.989025 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_multi_metrics.py
+-rw-r--r--   0        0        0    36919 2023-06-07 20:07:01.541242 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl.py
+-rw-r--r--   0        0        0    25177 2023-06-07 20:11:32.986812 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl_multi_metrics.py
+-rw-r--r--   0        0        0      748 2023-06-07 20:26:31.890615 openrlbenchmark-0.2.1a2/pyproject.toml
+-rw-r--r--   0        0        0    21316 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a2/PKG-INFO
```

### Comparing `openrlbenchmark-0.2.1a1/LICENSE` & `openrlbenchmark-0.2.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a1/README.md` & `openrlbenchmark-0.2.1a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -217,14 +217,38 @@
     --pc.ncols-legend 3 \
     --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
     --scan-history
 ```
 ![](static/baselines_vs_cleanrl_vs_jaxrl.png)
 
 
+### Multi-metrics
+
+**Experimental! API may change.**
+
+Sometimes you want to compare multiple metrics at once.
+
+```shell
+python -m openrlbenchmark.rlops_multi_metrics \
+    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metrics=charts/episodic_return&metrics=charts/episodic_length&metrics=charts/SPS&metrics=losses/actor_loss&metrics=losses/qf1_values&metrics=losses/qf1_loss' \
+        'ddpg_continuous_action?tag=pr-371' \
+        'ddpg_continuous_action?tag=pr-299' \
+        'ddpg_continuous_action?tag=rlops-pilot' \
+        'ddpg_continuous_action_jax?tag=pr-371-jax' \
+        'ddpg_continuous_action_jax?tag=pr-298' \
+    --env-ids HalfCheetah-v2 Hopper-v2 Walker2d-v2 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 2 \
+    --output-filename static/multi-metrics \
+    --scan-history --offline
+```
+![](static/multi-metrics.png)
+
+
 
 ### Compare Tianshou's algorithms with `openai/baselines`'s PPO2 on Atari:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward' 'iqn' 'ppo' 'rainbow' 'fqf' 'c51' 'dqn' 'qrdqn' \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
@@ -270,25 +294,26 @@
 ![](static/td3_vs_cleanrl.png)
 
 
 
 ### Compare MORL Baselines algorithms on deterministic environments
 
 ```shell
-python -m openrlbenchmark.rlops \
-  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metric=eval/hypervolume' \
+python -m openrlbenchmark.rlops_multi_metrics \
+  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metrics=eval/hypervolume&metrics=eval/igd&metrics=eval/sparsity&metrics=eval/eum&metrics=eval/mul' \
   'Pareto Q-Learning?cl=Pareto Q-Learning' \
   'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning' \
   'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)' \
-  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 \
-  --pc.ncols 2 \
-  --pc.ncols-legend 1 \
+  'MultiPolicy MO Q-Learning (GPI-LS)?cl=MultiPolicy MO Q-Learning (GPI-LS)' \
+  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 fruit-tree-v0 \
+  --pc.ncols 3 \
+  --pc.ncols-legend 4 \
   --pc.xlabel 'Training steps' \
-  --pc.ylabel 'Hypervolume' \
-  --output-filename morl_deterministic_envs \
+  --pc.ylabel '' \
+  --output-filename morl_deterministic_envs/ \
   --scan-history
 ```
 
 ![](static/morl_deterministic_envs.png)
 ![](static/morl_deterministic_envs-time.png)
 
 ### Calculate human normalized scores
```

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/cache.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/cache.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/cache_legacy.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/cache_legacy.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/capped_hns.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/capped_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/hns.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/offline_db.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/offline_db.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     """the ids of the environment to compare"""
     output_filename: str = "compare"
     """the output filename of the plot, without extension"""
     metric_last_n_average_window: int = 100
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
-    check_empty_runs: bool = False
+    check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
     report: bool = False
     """if toggled, a wandb report will be created"""
     wandb_project_name: str = "cleanrl"
     """the wandb project name for the report creation"""
     offline: bool = False
     """if toggled, we will use the offline database instead of wandb"""
@@ -386,15 +386,16 @@
         ax_time.set_xlabel("")
         ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    os.makedirs(os.path.dirname(output_filename), exist_ok=True)
+    if len(os.path.dirname(output_filename)) > 0:
+        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
     average_runtime.columns = ["Environment", "Average Runtime"]
@@ -417,16 +418,14 @@
     # remove the empty axes
     for ax in axes_flatten[len(env_ids) :]:
         ax.remove()
     for ax in axes_time_flatten[len(env_ids) :]:
         ax.remove()
 
     print(f"saving figures and tables to {output_filename}")
-    if os.path.dirname(output_filename) != "":
-        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     fig.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig_time.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig.savefig(f"{output_filename}.png", bbox_inches="tight")
     fig.savefig(f"{output_filename}.pdf", bbox_inches="tight")
     fig.savefig(f"{output_filename}.svg", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
```

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_hns.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_hns.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """the ids of the environment to compare"""
     output_filename: str = "compare"
     """the output filename of the plot, without extension"""
     metric_last_n_average_window: int = 100
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
-    check_empty_runs: bool = False
+    check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
     report: bool = False
     """if toggled, a wandb report will be created"""
     wandb_project_name: str = "cleanrl"
     """the wandb project name for the report creation"""
     offline: bool = False
     """if toggled, we will use the offline database instead of wandb"""
```

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_multi_metrics.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_multi_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     """the ids of the environment to compare"""
     output_filename: str = "compare"
     """the output filename of the plot, without extension"""
     metric_last_n_average_window: int = 100
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
-    check_empty_runs: bool = False
+    check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
     report: bool = False
     """if toggled, a wandb report will be created"""
     wandb_project_name: str = "cleanrl"
     """the wandb project name for the report creation"""
     offline: bool = False
     """if toggled, we will use the offline database instead of wandb"""
@@ -406,15 +406,16 @@
             else:
                 ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    os.makedirs(os.path.dirname(output_filename), exist_ok=True)
+    if os.path.dirname(output_filename) != "":
+        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
     average_runtime.columns = ["Environment", "Average Runtime"]
@@ -435,16 +436,14 @@
     # remove the empty axes
     for ax in axes_flatten[len(env_ids) * len(metrics):]:
         ax.remove()
     for ax in axes_time_flatten[len(env_ids) * len(metrics):]:
         ax.remove()
 
     print(f"saving figures and tables to {output_filename}")
-    if os.path.dirname(output_filename) != "":
-        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     fig.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig_time.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig.savefig(f"{output_filename}.png", bbox_inches="tight")
     fig.savefig(f"{output_filename}.pdf", bbox_inches="tight")
     fig.savefig(f"{output_filename}.svg", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
```

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,16 @@
         ax_time.set_xlabel("")
         ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    os.makedirs(os.path.dirname(output_filename), exist_ok=True)
+    if os.path.dirname(output_filename) != "":
+        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
     average_runtime.columns = ["Environment", "Average Runtime"]
@@ -419,16 +420,14 @@
     # remove the empty axes
     for ax in axes_flatten[len(env_ids) :]:
         ax.remove()
     for ax in axes_time_flatten[len(env_ids) :]:
         ax.remove()
 
     print(f"saving figures and tables to {output_filename}")
-    if os.path.dirname(output_filename) != "":
-        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     fig.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig_time.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig.savefig(f"{output_filename}.png", bbox_inches="tight")
     fig.savefig(f"{output_filename}.pdf", bbox_inches="tight")
     fig.savefig(f"{output_filename}.svg", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
```

### Comparing `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl_multi_metrics.py` & `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl_multi_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     """the ids of the environment to compare"""
     output_filename: str = "static/0compare"
     """the output filename of the plot, without extension"""
     metric_last_n_average_window: int = 100
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
-    check_empty_runs: bool = False
+    check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
     report: bool = False
     """if toggled, a wandb report will be created"""
     wandb_project_name: str = "cleanrl"
     """the wandb project name for the report creation"""
     offline: bool = False
     """if toggled, we will use the offline database instead of wandb"""
@@ -262,15 +262,15 @@
     blocks = []
     if report:
         for idx, env_id in enumerate(env_ids):
             metrics_over_step = []
             metrics_over_time = []
             for i in range(len(runsetss[0][idx].metrics)):
                 metric_over_step = wb.LinePlot(
-                    x="global_step",
+                    x="_step",
                     y=list({runsets[idx].metrics[i] for runsets in runsetss}),
                     title=runsetss[0][idx].metrics[i] + " " + env_id,
                     title_x="Steps",
                     title_y="Episodic Return",
                     max_runs_to_show=100,
                     smoothing_factor=0.8,
                     groupby_rangefunc="stderr",
@@ -299,15 +299,15 @@
             )
             custom_run_colors = {}
             for runsets in runsetss:
                 custom_run_colors.update(
                     {
                         (
                             runsets[idx].report_runset.name,
-                            runsets[idx].runs[0].config[runsets[idx].custom_exp_name_key],
+                            runsets[idx].runs[0].config['trl_ppo_trainer_config'][runsets[idx].custom_exp_name_key],
                         ): runsets[idx].color
                     }
                 )
             pg.custom_run_colors = custom_run_colors  # IMPORTANT: custom_run_colors is implemented as a custom `setter` that needs to be overwritten unlike regular dictionaries
             blocks += [pg]
 
     figsize = (pc.ncols * pc.cm, pc.nrows * pc.rm)
@@ -408,15 +408,16 @@
             else:
                 ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    os.makedirs(os.path.dirname(output_filename), exist_ok=True)
+    if len(os.path.dirname(output_filename)) > 0:
+        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
     average_runtime.columns = ["Environment", "Average Runtime"]
@@ -437,16 +438,14 @@
     # remove the empty axes
     for ax in axes_flatten[len(env_ids) * len(metrics):]:
         ax.remove()
     for ax in axes_time_flatten[len(env_ids) * len(metrics):]:
         ax.remove()
 
     print(f"saving figures and tables to {output_filename}")
-    if os.path.dirname(output_filename) != "":
-        os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     fig.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig_time.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig.savefig(f"{output_filename}.png", bbox_inches="tight")
     fig.savefig(f"{output_filename}.pdf", bbox_inches="tight")
     fig.savefig(f"{output_filename}.svg", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
```

### Comparing `openrlbenchmark-0.2.1a1/pyproject.toml` & `openrlbenchmark-0.2.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrlbenchmark"
-version = "0.2.1a1"
+version = "0.2.1a2"
 description = ""
 authors = ["Costa Huang <costa.huang@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "openrlbenchmark" },
 ]
```

### Comparing `openrlbenchmark-0.2.1a1/PKG-INFO` & `openrlbenchmark-0.2.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrlbenchmark
-Version: 0.2.1a1
+Version: 0.2.1a2
 Summary: 
 Author: Costa Huang
 Author-email: costa.huang@outlook.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -244,14 +244,38 @@
     --pc.ncols-legend 3 \
     --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
     --scan-history
 ```
 ![](static/baselines_vs_cleanrl_vs_jaxrl.png)
 
 
+### Multi-metrics
+
+**Experimental! API may change.**
+
+Sometimes you want to compare multiple metrics at once.
+
+```shell
+python -m openrlbenchmark.rlops_multi_metrics \
+    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metrics=charts/episodic_return&metrics=charts/episodic_length&metrics=charts/SPS&metrics=losses/actor_loss&metrics=losses/qf1_values&metrics=losses/qf1_loss' \
+        'ddpg_continuous_action?tag=pr-371' \
+        'ddpg_continuous_action?tag=pr-299' \
+        'ddpg_continuous_action?tag=rlops-pilot' \
+        'ddpg_continuous_action_jax?tag=pr-371-jax' \
+        'ddpg_continuous_action_jax?tag=pr-298' \
+    --env-ids HalfCheetah-v2 Hopper-v2 Walker2d-v2 \
+    --no-check-empty-runs \
+    --pc.ncols 3 \
+    --pc.ncols-legend 2 \
+    --output-filename static/multi-metrics \
+    --scan-history --offline
+```
+![](static/multi-metrics.png)
+
+
 
 ### Compare Tianshou's algorithms with `openai/baselines`'s PPO2 on Atari:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward' 'iqn' 'ppo' 'rainbow' 'fqf' 'c51' 'dqn' 'qrdqn' \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
@@ -297,25 +321,26 @@
 ![](static/td3_vs_cleanrl.png)
 
 
 
 ### Compare MORL Baselines algorithms on deterministic environments
 
 ```shell
-python -m openrlbenchmark.rlops \
-  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metric=eval/hypervolume' \
+python -m openrlbenchmark.rlops_multi_metrics \
+  --filters '?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metrics=eval/hypervolume&metrics=eval/igd&metrics=eval/sparsity&metrics=eval/eum&metrics=eval/mul' \
   'Pareto Q-Learning?cl=Pareto Q-Learning' \
   'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning' \
   'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)' \
-  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 \
-  --pc.ncols 2 \
-  --pc.ncols-legend 1 \
+  'MultiPolicy MO Q-Learning (GPI-LS)?cl=MultiPolicy MO Q-Learning (GPI-LS)' \
+  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 fruit-tree-v0 \
+  --pc.ncols 3 \
+  --pc.ncols-legend 4 \
   --pc.xlabel 'Training steps' \
-  --pc.ylabel 'Hypervolume' \
-  --output-filename morl_deterministic_envs \
+  --pc.ylabel '' \
+  --output-filename morl_deterministic_envs/ \
   --scan-history
 ```
 
 ![](static/morl_deterministic_envs.png)
 ![](static/morl_deterministic_envs-time.png)
 
 ### Calculate human normalized scores
```

