# Comparing `tmp/openrlbenchmark-0.2.0b4.tar.gz` & `tmp/openrlbenchmark-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrlbenchmark-0.2.0b4.tar", max compression
+gzip compressed data, was "openrlbenchmark-0.2.1a1.tar", max compression
```

## Comparing `openrlbenchmark-0.2.0b4.tar` & `openrlbenchmark-0.2.1a1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.0b4/LICENSE
--rw-r--r--   0        0        0    18408 2023-06-05 02:27:41.017161 openrlbenchmark-0.2.0b4/README.md
--rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.0b4/openrlbenchmark/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.0b4/openrlbenchmark/cache.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.0b4/openrlbenchmark/cache_legacy.py
--rw-r--r--   0        0        0     6147 2023-05-01 14:06:32.647152 openrlbenchmark-0.2.0b4/openrlbenchmark/capped_hns.py
--rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.0b4/openrlbenchmark/hns.py
--rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.0b4/openrlbenchmark/offline_db.py
--rw-r--r--   0        0        0    36045 2023-06-05 02:19:44.068997 openrlbenchmark-0.2.0b4/openrlbenchmark/rlops copy.py
--rw-r--r--   0        0        0    36839 2023-06-05 02:35:20.353512 openrlbenchmark-0.2.0b4/openrlbenchmark/rlops.py
--rw-r--r--   0        0        0    30368 2023-06-05 02:01:01.027169 openrlbenchmark-0.2.0b4/openrlbenchmark/rlops_hns.py
--rw-r--r--   0        0        0      748 2023-06-05 02:48:19.404041 openrlbenchmark-0.2.0b4/pyproject.toml
--rw-r--r--   0        0        0    19371 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.1a1/LICENSE
+-rw-r--r--   0        0        0    19299 2023-06-06 15:14:33.209492 openrlbenchmark-0.2.1a1/README.md
+-rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.1a1/openrlbenchmark/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.1a1/openrlbenchmark/cache.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.1a1/openrlbenchmark/cache_legacy.py
+-rw-r--r--   0        0        0     6147 2023-05-01 14:06:32.647152 openrlbenchmark-0.2.1a1/openrlbenchmark/capped_hns.py
+-rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.1a1/openrlbenchmark/hns.py
+-rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.1a1/openrlbenchmark/offline_db.py
+-rw-r--r--   0        0        0    36839 2023-06-06 16:06:15.870857 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops.py
+-rw-r--r--   0        0        0    30368 2023-06-05 02:01:01.027169 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_hns.py
+-rw-r--r--   0        0        0    25008 2023-06-06 20:21:31.794579 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_multi_metrics.py
+-rw-r--r--   0        0        0    36984 2023-06-06 15:06:30.132573 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl.py
+-rw-r--r--   0        0        0    25220 2023-06-07 11:59:12.598806 openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl_multi_metrics.py
+-rw-r--r--   0        0        0     2074 2023-06-06 20:28:58.991774 openrlbenchmark-0.2.1a1/openrlbenchmark/test.json
+-rw-r--r--   0        0        0      748 2023-06-07 15:34:13.833615 openrlbenchmark-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0    20262 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a1/PKG-INFO
```

### Comparing `openrlbenchmark-0.2.0b4/LICENSE` & `openrlbenchmark-0.2.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/README.md` & `openrlbenchmark-0.2.1a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: openrlbenchmark
+Version: 0.2.1a1
+Summary: 
+Author: Costa Huang
+Author-email: costa.huang@outlook.com
+Requires-Python: >=3.7.1,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: dotmap (>=1.3.30,<2.0.0)
+Requires-Dist: expt (>=0.4.1,<0.5.0)
+Requires-Dist: importlib-metadata (>=5.1.0,<6.0.0)
+Requires-Dist: multiprocess (>=0.70.13,<0.71.0)
+Requires-Dist: peewee (>=3.16.2,<4.0.0)
+Requires-Dist: pip (>=22.1.2,<23.0.0)
+Requires-Dist: rich (<12.0)
+Requires-Dist: rliable (>=1.0.8,<2.0.0)
+Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: tueplots (>=0.0.4,<0.0.5)
+Requires-Dist: tyro (>=0.5.0,<0.6.0)
+Requires-Dist: wandb (>=0.13.7,<0.14.0)
+Description-Content-Type: text/markdown
+
 # Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning
 
 
 [<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)
@@ -60,52 +87,63 @@
     --rc.sample_efficiency_plots \
     --rc.sample_efficiency_and_walltime_efficiency_method Median \
     --rc.performance_profile_plots  \
     --rc.aggregate_metrics_plots  \
     --rc.sample_efficiency_num_bootstrap_reps 10 \
     --rc.performance_profile_num_bootstrap_reps 10 \
     --rc.interval_estimates_num_bootstrap_reps 10 \
-    --output-filename static/0compare \
+    --output-filename compare \
     --scan-history
 ```
 
-Here, we created multiple filters. The first string in the first filter is `'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean'`, which is a query string that specifies the following:
+Here, we created multiple filters. The first string in the first filter is `'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return'`, which is a query string that specifies the following:
 
 * `we`: the W&B entity name
 * `wpn`: the W&B project name
 * `ceik`: the custom key for the environment id
 * `cen`: the custom key for the experiment name
 * `metric`: the metric we are interested in
 
-So we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.
+So we are fetching metrics from [https://wandb.ai/openrlbenchmark/baselines](https://wandb.ai/openrlbenchmark/baselines). The environment id is stored in the `env` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`.
 
-Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.
+Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `baselines-ppo2-mlp?cl=openai/baselines PPO2`.
 
 The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
 
-The command above generates the following plot:
+The `--rliable` toggles our [rliable](https://github.com/google-research/rliable) integration, and its configuration can be tweeked via `--rc`. The command above generates the following plot:
 
-|    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |
-|:----------------------------------:|:----------------------------------------:|
-|  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |
+![](static/baseline_vs_cleanrl.png)
+![](static/baseline_vs_cleanrl-time.png)
+![](static/baseline_vs_cleanrl_sample_walltime_efficiency.png)
+![](static/baseline_vs_cleanrl_sample_efficiency.png)
+![](static/baseline_vs_cleanrl_performance_profile.png)
+![](static/baseline_vs_cleanrl_aggregate.png)
 
 
 
-The `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-sac_continuous_action--VmlldzozMTY4NDQ3)
+The `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-openai-baselines-PPO2--Vmlldzo0NTU4MTE5)
 
 
 The command also generates a `compare.png`, a `compare.md`, and a `compare.csv` in the current directory.
 
 **Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.
 
 **Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.
 
 
 > **Warning**
-> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. If you are using `openrlbenchmark` repeatedly or you wanto to generate consistent `compare.md` and learning curves, we recommend you to use `--scan-history` to get all of the data points, but initially it may take a while to run.
+> We recommend you to use `--scan-history` which pullts all of the data points, but initially it will cache the data and may take a while to run. If you don't use `--scan-history`, it will only pull 500 data points from wandb randomly, which could generate different learning curves each time you run the command.
+
+
+## Offline mode
+
+We introduced an experimental **offline** mode. Sometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. 
+
+No worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs. Then, you can run `python -m openrlbenchmark.rlops ... --scan-history --offline` to generate the plots without having access to the internet. It should considerably speed up the plotting process as well. We are still working on improving the offline mode, so please let us know if you encounter any issues. 
+
 
 
 ## Currently supported libraries
 
 * [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)
     * `ceik`: `env_id`
     * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)
@@ -149,62 +187,53 @@
 
 ## More examples
 
 ### Compare CleanRL's PPO with `openai/baselines`'s PPO2 on Atari games:
 
 Sometimes the same environments could have different names in different libraries. For example, `openai/baselines` uses `BreakoutNoFrameskip-v4` while [EnvPool](https://envpool.readthedocs.io/en/latest/env/atari.html) uses `Breakout-v5`. To compare the two libraries, we need to specify the `env_id` for `CleanRL` and `env` for `openai/baselines`. In this case, can specify the corresponding `env_ids` for each filter.
 
-For Atari games, we have additional batteries included `openrlbenchmark.rlops_hns` to show human normalized-scores and further statistical analysis through [`rliable`](https://github.com/google-research/rliable).
+For Atari games, we can toggle `--rc.score_normalization_method atari` option to use human-normalized scores for `rliable` analysis.
 
 
 ```shell
-python -m openrlbenchmark.rlops_hns \
+python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
     --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation' \
     --env-ids AlienNoFrameskip-v4 AmidarNoFrameskip-v4 AssaultNoFrameskip-v4 AsterixNoFrameskip-v4 AsteroidsNoFrameskip-v4 AtlantisNoFrameskip-v4 BankHeistNoFrameskip-v4 BattleZoneNoFrameskip-v4 BeamRiderNoFrameskip-v4 BerzerkNoFrameskip-v4 BowlingNoFrameskip-v4 BoxingNoFrameskip-v4 BreakoutNoFrameskip-v4 CentipedeNoFrameskip-v4 ChopperCommandNoFrameskip-v4 CrazyClimberNoFrameskip-v4 DefenderNoFrameskip-v4 DemonAttackNoFrameskip-v4 DoubleDunkNoFrameskip-v4 EnduroNoFrameskip-v4 FishingDerbyNoFrameskip-v4 FreewayNoFrameskip-v4 FrostbiteNoFrameskip-v4 GopherNoFrameskip-v4 GravitarNoFrameskip-v4 HeroNoFrameskip-v4 IceHockeyNoFrameskip-v4 PrivateEyeNoFrameskip-v4 QbertNoFrameskip-v4 RiverraidNoFrameskip-v4 RoadRunnerNoFrameskip-v4 RobotankNoFrameskip-v4 SeaquestNoFrameskip-v4 SkiingNoFrameskip-v4 SolarisNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 StarGunnerNoFrameskip-v4 SurroundNoFrameskip-v4 TennisNoFrameskip-v4 TimePilotNoFrameskip-v4 TutankhamNoFrameskip-v4 UpNDownNoFrameskip-v4 VentureNoFrameskip-v4 VideoPinballNoFrameskip-v4 WizardOfWorNoFrameskip-v4 YarsRevengeNoFrameskip-v4 ZaxxonNoFrameskip-v4 JamesbondNoFrameskip-v4 KangarooNoFrameskip-v4 KrullNoFrameskip-v4 KungFuMasterNoFrameskip-v4 MontezumaRevengeNoFrameskip-v4 MsPacmanNoFrameskip-v4 NameThisGameNoFrameskip-v4 PhoenixNoFrameskip-v4 PitfallNoFrameskip-v4 PongNoFrameskip-v4 \
     --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
     --no-check-empty-runs \
     --pc.ncols 5 \
     --pc.ncols-legend 2 \
-    --output-filename static/cleanrl_vs_baselines \
-    --scan-history --rliable
+    --rliable \
+    --rc.score_normalization_method atari \
+    --rc.normalized_score_threshold 8.0 \
+    --rc.sample_efficiency_plots \
+    --rc.sample_efficiency_and_walltime_efficiency_method Median \
+    --rc.performance_profile_plots  \
+    --rc.aggregate_metrics_plots  \
+    --rc.sample_efficiency_num_bootstrap_reps 50000 \
+    --rc.performance_profile_num_bootstrap_reps 2000 \
+    --rc.interval_estimates_num_bootstrap_reps 2000 \
+    --output-filename static/cleanrl_vs_baselines_atari \
+    --scan-history
 ```
 
-In the individual learning curves below, the right y-axis is the human normalized score. The left y-axis is the raw episodic return.
-![](static/cleanrl_vs_baselines.png) The script also generates `cleanrl_vs_baselines_hns_median.png`, the learning curves for median human-normalized scores. 
 
 Furthermore, the `--rliable` integration generates `cleanrl_vs_baselines_iqm_profile.png`, the  Interquartile Mean (IQM) and performance profile ([Agarwal et al., 2022](https://arxiv.org/pdf/2108.13264.pdf)), and `cleanrl_vs_baselines_hns_aggregate.png`, the aggregate human-normalized scores with Stratified Bootstrap Confidence Intervals (see @araffin's excellent blog post [explainer](https://araffin.github.io/post/rliable/)). 
 
 
-![](static/cleanrl_vs_baselines_hns_median.png)
-
-![](static/cleanrl_vs_baselines_iqm_profile.png)
-
-![](static/cleanrl_vs_baselines_hns_aggregate.png)
-
 
-### Offline mode
+![](static/cleanrl_vs_baselines_atari.png)
+![](static/cleanrl_vs_baselines_atari-time.png)
+![](static/cleanrl_vs_baselines_atari_sample_walltime_efficiency.png)
+![](static/cleanrl_vs_baselines_atari_sample_efficiency.png)
+![](static/cleanrl_vs_baselines_atari_performance_profile.png)
+![](static/cleanrl_vs_baselines_atari_aggregate.png)
 
-Sometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. 
 
-No worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs, enabling us to run the script without internet connection.
-
-```shell
-python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
-    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
-    --filters '?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return' 'sac' \
-    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \
-    --no-check-empty-runs \
-    --pc.ncols 3 \
-    --pc.ncols-legend 3 \
-    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
-    --scan-history \
-    --offline
-```
 
 ### Compare CleanRL's PPO with `openai/baselines`'s PPO2 and `jaxrl`'s SAC on Mujoco:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
@@ -318,7 +347,22 @@
 This is a project we are slowly working on. There is no specific timeline or roadmap, but if you want to get involved. Feel free to reach out to me or open an issue. We are looking for volunteers to help us with the following:
 
 * Add experiments from other libraries
 * Run more experiments from currently supported libraries
 * Documentation and designing standards
 * Download the tensorboard metrics from the tracked experiments and load them locally to save time
 
+## Citation
+
+If you have used this software in your work, please use the following citation.
+
+```bibtex
+@software{
+    Huang_openrlbenchmark_2023,
+    author = {Huang, Shengyi and Gallouédec, Quentin and Felten, Florian and Raffin, Antonin and Dossa, Rousslan Fernand Julien and Zhao, Yanxiao and Sullivan, Ryan and Makoviychuk, Viktor and Makoviichuk, Denys and Roumégous, Cyril and Weng, Jiayi and Chen, Chufan and Rahman, Masudur and M. Araújo, João G. and Quan, Guorui and Tan, Daniel and Klein, Timo and Charakorn, Rujikorn and Towers, Mark and Berthelot, Yann and Mehta, Kinal and Chakraborty, Dipam and KG, Arjun and Charraut, Valentin and Ye, Chang and Liu, Zichen and Alegre, Lucas N. and Choi, Jongwook and Yi, Brent},
+    month = may,
+    title = {{openrlbenchmark}},
+    url = {https://github.com/openrlbenchmark/openrlbenchmark},
+    year = {2023}
+}
+```
+
```

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/cache.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/cache.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/cache_legacy.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/cache_legacy.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/capped_hns.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/capped_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/hns.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/offline_db.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/offline_db.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/rlops copy.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_trl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from collections import defaultdict
 import copy
 import os
+from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Dict, List, Literal, Optional
 from urllib.parse import parse_qs, urlparse
 
 import expt
 import matplotlib.pyplot as plt
 import numpy as np
@@ -40,19 +40,19 @@
     """if toggled, we will generate sample efficiency plots"""
     sample_efficiency_and_walltime_efficiency_method: Optional[Literal["Median", "IQM", "Mean", "Optimality Gap"]] = "Median"
     """the method to compute the sample efficiency and walltime efficiency"""
     performance_profile_plots: bool = True
     """if toggled, we will generate performance profile plots"""
     aggregate_metrics_plots: bool = True
     """if toggled, we will generate aggregate metrics plots"""
-    sample_efficiency_num_bootstrap_reps: int = 10 # 50000
+    sample_efficiency_num_bootstrap_reps: int = 10  # 50000
     """the number of bootstrap replications in `rliable` to use for computing the sample efficiency"""
-    performance_profile_num_bootstrap_reps: int = 10 # 2000
+    performance_profile_num_bootstrap_reps: int = 10  # 2000
     """the number of bootstrap replications in `rliable` to use for computing the performance profile"""
-    interval_estimates_num_bootstrap_reps: int = 10 # 2000
+    interval_estimates_num_bootstrap_reps: int = 10  # 2000
     """the number of bootstrap replications in `rliable` to use for computing the the interval estimates"""
 
 
 @dataclass
 class PlotConfig:
     ncols: int = 2
     """the number of columns in the chart"""
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
@@ -141,18 +141,18 @@
         self.offline_db = offline_db
         self.offline = offline
 
         user = [{"username": self.username}] if self.username else []
         include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
         self.wandb_filters = {
             "$and": [
-                {f"config.{self.custom_env_id_key}.value": self.env_id},
+                {f"config.trl_ppo_trainer_config.value.{self.custom_env_id_key}": self.env_id},
                 *include_tag_groups,
                 *user,
-                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
+                {f"config.trl_ppo_trainer_config.value.{self.custom_exp_name_key}": self.exp_name},
             ]
         }
 
     @property
     def runs(self):
         if not self.offline:
             return wandb.Api().runs(
@@ -236,29 +236,30 @@
             run_df = run.run_df
         else:
             run_df = run.history(samples=1500)
         if "videos" in run_df:
             run_df = run_df.drop(columns=["videos"], axis=1)
         if len(runset.metric) > 0:
             run_df["charts/episodic_return"] = run_df[runset.metric]
+        if "global_step" not in run_df:
+            run_df["global_step"] = run_df["_step"]
         cleaned_df = run_df[["global_step", "_runtime", "charts/episodic_return"]].dropna()
         runs += [Run(f"seed{idx}", cleaned_df)]
     return Hypothesis(runset.name, runs)
 
 
 def compare(
     console: Console,
     runsetss: List[List[Runset]],
     env_ids: List[str],
     metric_last_n_average_window: int,
     scan_history: bool = False,
     output_filename: str = "compare",
     report: bool = False,
     pc: PlotConfig = None,
-    rc: RliableConfig = None,
 ):
     blocks = []
     if report:
         for idx, env_id in enumerate(env_ids):
             metric_over_step = wb.LinePlot(
                 x="global_step",
                 y=list({runsets[idx].metric for runsets in runsetss}),
@@ -324,37 +325,29 @@
     if len(env_ids) == 1:
         axes = np.array([axes])
         axes_time = np.array([axes_time])
     axes_flatten = axes.flatten()
     axes_time_flatten = axes_time.flatten()
 
     result_table = pd.DataFrame(index=env_ids, columns=[runsets[0].name for runsets in runsetss])
-    min_num_seeds_per_hypothesis = {}
-    for runsets in runsetss:
-        min_num_seeds_per_hypothesis[runsets[0].name] = float("inf")
     exs = []
     runtimes = []
     global_steps = []
     for idx, env_id in enumerate(env_ids):
         print(f"collecting runs for {env_id}")
-        ex = expt.Experiment("Comparison")
-        for runsets in runsetss:
-            hypo = create_hypothesis(runsets[idx], scan_history)
-            ex.add_hypothesis(hypo)
+        hypotheses = [create_hypothesis(runsets[idx], scan_history) for runsets in runsetss]
+        ex = expt.Experiment("Comparison", hypotheses)
         exs.append(ex)
 
         # for each run `i` get the average of the last `rolling` episodes as r_i
         # then take the average and std of r_i as the results.
         result = []
         for hypothesis in ex.hypotheses:
             metric_result = []
             console.print(f"{hypothesis.name} has {len(hypothesis.runs)} runs", style="bold")
-            min_num_seeds_per_hypothesis[hypothesis.name] = min(
-                min_num_seeds_per_hypothesis[hypothesis.name], len(hypothesis.runs)
-            )
             for run in hypothesis.runs:
                 metric_result += [run.df["charts/episodic_return"].dropna()[-metric_last_n_average_window:].mean()]
 
                 # convert time unit in place
                 if pc.time_unit == "m":
                     run.df["_runtime"] /= 60
                 elif pc.time_unit == "h":
@@ -394,39 +387,14 @@
         )
         ax_time.set_xlabel("")
         ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
-    # for each run set, for each seed, plot 57 curves and get their median curves, then plot the average of the median curves
-    score_dict = {}
-    max_global_steps = defaultdict(int)
-    for runsets_idx, runsets in enumerate(runsetss):
-        score_dict[runsets[0].name] = np.zeros((min_num_seeds_per_hypothesis[runsets[0].name], len(env_ids), rc.nsubsamples))
-        # for each seed
-        for seed_idx, _ in enumerate(range(min_num_seeds_per_hypothesis[runsets[0].name])):  # exs[0][runsets_idx]
-            min_global_step = float("inf")
-            print(f"collecting runs for {runsets[0].name} seed {seed_idx}")
-
-            runs_of_one_seed = []
-            for ex_idx, ex in enumerate(exs):
-                run_of_one_seed = ex[runsets_idx][seed_idx]
-                min_global_step = min(min_global_step, run_of_one_seed.df["global_step"].iloc[-1])
-                runs_of_one_seed.append(run_of_one_seed)
-
-                # interpolate
-                x_samples = np.linspace(
-                    min(run_of_one_seed.df["global_step"]), max(run_of_one_seed.df["global_step"]), num=rc.nsubsamples
-                )
-                score_dict[runsets[0].name][seed_idx, ex_idx, :] = np.interp(
-                    x_samples, run_of_one_seed.df["global_step"], run_of_one_seed.df["charts/episodic_return"]
-                )
-            max_global_steps[runsets[0].name] = max(max_global_steps[runsets[0].name], min_global_step)
-
     # create the required directory for `output_filename`
     os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
@@ -461,39 +429,35 @@
     fig_time.subplots_adjust(hspace=pc.hspace, wspace=pc.wspace)
     fig.savefig(f"{output_filename}.png", bbox_inches="tight")
     fig.savefig(f"{output_filename}.pdf", bbox_inches="tight")
     fig.savefig(f"{output_filename}.svg", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.png", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.pdf", bbox_inches="tight")
     fig_time.savefig(f"{output_filename}-time.svg", bbox_inches="tight")
-    return blocks, score_dict, max_global_steps, runtimes, global_steps
+    return blocks, runtimes, global_steps, exs
 
 
 def normalize_score(score_dict: Dict[str, np.ndarray], max_scores: np.ndarray, min_scores: np.ndarray):
     """
     Each item in `score_dict` has shape (num_seeds, num_envs, num_subsamples)
     `max_scores` has shape (num_envs)
     `min_scores` has shape (num_envs)
     """
     normalized_score_dict = {}
     for key in score_dict:
-        normalized_score_dict[key] = (score_dict[key] - min_scores.reshape(1, -1, 1)) / (max_scores.reshape(1, -1, 1) - min_scores.reshape(1, -1, 1))
+        normalized_score_dict[key] = (score_dict[key] - min_scores.reshape(1, -1, 1)) / (
+            max_scores.reshape(1, -1, 1) - min_scores.reshape(1, -1, 1)
+        )
     return normalized_score_dict
 
 
 def maxmin_normalize_score(score_dict: Dict[str, np.ndarray]):
     all_scores = np.concatenate([score_dict[key] for key in score_dict], axis=0)
-    max_scores = (all_scores
-        .max(0) # max over all experiments and seds
-        .max(1) # max over all steps
-    )
-    min_scores = (all_scores
-        .min(0) # min over all experiments and seds
-        .min(1) # min over all steps
-    )
+    max_scores = all_scores.max(0).max(1)  # 1) max over all experiments and seds 2) max over all steps
+    min_scores = all_scores.min(0).min(1)  # 1) min over all experiments and seds 2) min over all steps
     return normalize_score(score_dict, max_scores, min_scores)
 
 
 def atari_normalize_score(original_env_ids):
     env_ids = []
     for env_id in original_env_ids:
         if env_id.endswith("NoFrameskip-v4"):
@@ -539,17 +503,15 @@
                 "custom_env_id_key": custom_env_id_key,
                 "custom_exp_name_key": custom_exp_name_key,
                 "metric": metric,
             },
             expand_all=True,
         )
         if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
-            offline_db_folder = os.path.join(
-                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}"
-            )
+            offline_db_folder = os.path.join(openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}")
             offline_db_path = os.path.join(offline_db_folder, "offline.sqlite")
             print(offline_db_path)
             os.makedirs(offline_db_folder, exist_ok=True)
             offline_db = pw.SqliteDatabase(offline_db_path)
             database_proxy.initialize(offline_db)
             offline_db.connect()
             offline_db.create_tables([OfflineRun, Tag, OfflineRunTag])
@@ -592,61 +554,111 @@
                 if args.check_empty_runs:
                     console.print(f"{exp_name} [green]({query})[/] in [purple]{env_id}[/] has {len(runsets[-1].runs)} runs")
                     for run in runsets[-1].runs:
                         console.print(f"┣━━ [link={run.url}]{run.name}[/link] with tags = {run.tags}")
                     assert len(runsets[0].runs) > 0, f"{exp_name} ({query}) in {env_id} has no runs"
             runsetss.append(runsets)
 
-    blocks, score_dict, max_global_steps, runtimes, global_steps = compare(
+    blocks, runtimes, global_steps, exs = compare(
         console,
         runsetss,
         args.env_ids[0],
         output_filename=args.output_filename,
         metric_last_n_average_window=args.metric_last_n_average_window,
         scan_history=args.scan_history,
         report=args.report,
         pc=args.pc,
-        rc=args.rc,
     )
 
     if args.rliable:
+        # get min num seeds per hypothesis
+        min_num_seeds_per_hypothesis = {}
+        for runsets in runsetss:
+            min_num_seeds_per_hypothesis[runsets[0].name] = float("inf")
+        for ex in exs:
+            for hypothesis in ex.hypotheses:
+                console.print(f"{hypothesis.name} has {len(hypothesis.runs)} runs", style="bold")
+                min_num_seeds_per_hypothesis[hypothesis.name] = min(
+                    min_num_seeds_per_hypothesis[hypothesis.name], len(hypothesis.runs)
+                )
+
+        # create `score_dict`; each item in `score_dict` has shape (num_seeds, len(args.env_ids[0]), nsubsamples)
+        score_dict = {}
+        max_global_steps = defaultdict(int)
+        for runsets_idx, runsets in enumerate(runsetss):
+            score_dict[runsets[0].name] = np.zeros(
+                (min_num_seeds_per_hypothesis[runsets[0].name], len(args.env_ids[0]), args.rc.nsubsamples)
+            )
+            # for each seed
+            for seed_idx, _ in enumerate(range(min_num_seeds_per_hypothesis[runsets[0].name])):  # exs[0][runsets_idx]
+                min_global_step = float("inf")
+                print(f"collecting runs for {runsets[0].name} seed {seed_idx}")
+
+                runs_of_one_seed = []
+                for ex_idx, ex in enumerate(exs):
+                    run_of_one_seed = ex[runsets_idx][seed_idx]
+                    min_global_step = min(min_global_step, run_of_one_seed.df["global_step"].iloc[-1])
+                    runs_of_one_seed.append(run_of_one_seed)
+
+                    # interpolate
+                    x_samples = np.linspace(
+                        min(run_of_one_seed.df["global_step"]), max(run_of_one_seed.df["global_step"]), num=args.rc.nsubsamples
+                    )
+                    score_dict[runsets[0].name][seed_idx, ex_idx, :] = np.interp(
+                        x_samples, run_of_one_seed.df["global_step"], run_of_one_seed.df["charts/episodic_return"]
+                    )
+                max_global_steps[runsets[0].name] = max(max_global_steps[runsets[0].name], min_global_step)
+
         exp_names = list(reversed(list(score_dict.keys())))
         colors_flatten = colors_flatten_original
         colors = dict(zip(list(score_dict.keys()), colors_flatten))
         frames = np.linspace(0, max(max_global_steps.values()), args.rc.nsubsamples)
-        print_rich_table(f"Items in the `score_dict` used for `rliable`", pd.DataFrame(
-            data=[score_dict[key].shape for key in score_dict],
-            columns=["Number of Seeds", "Number of Environments", "Number of Sub-samples"],
-            index=list(score_dict.keys())).rename_axis("Experiments").reset_index(), console)
+        print_rich_table(
+            f"Items in the `score_dict` used for `rliable`",
+            pd.DataFrame(
+                data=[score_dict[key].shape for key in score_dict],
+                columns=["Number of Seeds", "Number of Environments", "Number of Sub-samples"],
+                index=list(score_dict.keys()),
+            )
+            .rename_axis("Experiments")
+            .reset_index(),
+            console,
+        )
 
-        # normalize scores. Each item in `score_dict` has shape (num_runs, len(args.env_ids[0]), nsubsamples)
+        # normalize scores.
         if args.rc.score_normalization_method == "maxmin":
             normalized_score_dict = maxmin_normalize_score(score_dict)
-        elif args.rc.score_normalization_method == "atari": 
+        elif args.rc.score_normalization_method == "atari":
             normalized_score_dict = atari_normalize_score(args.env_ids[0])
         else:
             raise NotImplementedError(f"Normalization method {args.rc.score_normalization_method} not implemented")
         performance_profile_normalized_score_dict = {}
         for key, value in normalized_score_dict.items():
             performance_profile_normalized_score_dict[key] = np.nanmean(value[:, :, -1:], axis=-1)
-        metric_fns = [metrics.aggregate_median, metrics.aggregate_iqm, metrics.aggregate_mean, metrics.aggregate_optimality_gap]
+        metric_fns = [
+            metrics.aggregate_median,
+            metrics.aggregate_iqm,
+            metrics.aggregate_mean,
+            metrics.aggregate_optimality_gap,
+        ]
         metric_names = ["Median", "IQM", "Mean", "Optimality Gap"]
 
-
         if args.rc.sample_efficiency_plots:
             print("plotting sample efficiency curve (this is slow and may take several minutes)")
             fig_sample_efficiency, axes_sample_efficiency = plt.subplots(
                 ncols=2,
                 nrows=2,
                 figsize=(7 * 2, 3.4 * 2),
                 sharex=args.pc.sharex,
             )
             for metric_fn, ax, metric_name in zip(metric_fns, axes_sample_efficiency.flatten(), metric_names):
                 aggregate_fn = lambda scores: np.array([metric_fn(scores[..., frame]) for frame in range(scores.shape[-1])])
-                aggregate_scores, aggregate_cis = rly.get_interval_estimates(normalized_score_dict, aggregate_fn, reps=args.rc.sample_efficiency_num_bootstrap_reps)
+                aggregate_scores, aggregate_cis = rly.get_interval_estimates(
+                    normalized_score_dict, aggregate_fn, reps=args.rc.sample_efficiency_num_bootstrap_reps
+                )
                 for exp_name in score_dict.keys():
                     global_step = global_steps[exp_name].mean()
                     global_step_xaxis = np.linspace(0, global_step, args.rc.nsubsamples)
                     plot_utils.plot_sample_efficiency_curve(
                         global_step_xaxis,
                         {exp_name: aggregate_scores[exp_name]},
                         {exp_name: aggregate_cis[exp_name]},
@@ -681,36 +693,54 @@
                             ylabel=metric_name,
                             labelsize="x-large",
                             ticklabelsize="x-large",
                         )
                     expt.plot.autoformat_xaxis(axes_median_sample_walltime_efficiency[0])
                     for exp_name in score_dict.keys():
                         runtime = runtimes[exp_name].mean()
-                        runtime_xaxis =  np.linspace(0, runtime, args.rc.nsubsamples)
+                        runtime_xaxis = np.linspace(0, runtime, args.rc.nsubsamples)
                         plot_utils.plot_sample_efficiency_curve(
                             runtime_xaxis,
                             {exp_name: aggregate_scores[exp_name]},
                             {exp_name: aggregate_cis[exp_name]},
                             algorithms=[exp_name],
                             colors=colors,
                             xlabel=f"Time ({args.pc.time_unit})",
                             ax=axes_median_sample_walltime_efficiency[1],
                             ylabel=metric_name,
                             labelsize="x-large",
                             ticklabelsize="x-large",
                         )
                     axes_median_sample_walltime_efficiency[1].set_ylabel("")
                     h, l = axes_median_sample_walltime_efficiency[1].get_legend_handles_labels()
-                    fig_median_sample_walltime_efficiency.legend(h, l, loc="lower center", ncol=args.pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_median_sample_walltime_efficiency.transFigure)
+                    fig_median_sample_walltime_efficiency.legend(
+                        h,
+                        l,
+                        loc="lower center",
+                        ncol=args.pc.ncols_legend,
+                        bbox_to_anchor=(0.5, 1.0),
+                        bbox_transform=fig_median_sample_walltime_efficiency.transFigure,
+                    )
                     fig_median_sample_walltime_efficiency.tight_layout()
-                    fig_median_sample_walltime_efficiency.savefig(f"{args.output_filename}_sample_walltime_efficiency.png", bbox_inches="tight")
-                    fig_median_sample_walltime_efficiency.savefig(f"{args.output_filename}_sample_walltime_efficiency.pdf", bbox_inches="tight")
+                    fig_median_sample_walltime_efficiency.savefig(
+                        f"{args.output_filename}_sample_walltime_efficiency.png", bbox_inches="tight"
+                    )
+                    fig_median_sample_walltime_efficiency.savefig(
+                        f"{args.output_filename}_sample_walltime_efficiency.pdf", bbox_inches="tight"
+                    )
 
             h, l = axes_sample_efficiency[0][0].get_legend_handles_labels()
-            fig_sample_efficiency.legend(h, l, loc="lower center", ncol=args.pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_sample_efficiency.transFigure)
+            fig_sample_efficiency.legend(
+                h,
+                l,
+                loc="lower center",
+                ncol=args.pc.ncols_legend,
+                bbox_to_anchor=(0.5, 1.0),
+                bbox_transform=fig_sample_efficiency.transFigure,
+            )
             fig_sample_efficiency.supxlabel(args.pc.xlabel, fontsize="x-large")
             fig_sample_efficiency.tight_layout()
             fig_sample_efficiency.savefig(f"{args.output_filename}_sample_efficiency.png", bbox_inches="tight")
             fig_sample_efficiency.savefig(f"{args.output_filename}_sample_efficiency.pdf", bbox_inches="tight")
 
         if args.rc.performance_profile_plots:
             print("plotting performance profiles")
@@ -744,34 +774,43 @@
                 performance_profile_cis=avg_score_distributions_cis,
                 colors=colors,
                 xlabel=r"Normalized Score $(\tau)$",
                 ylabel=r"Fraction of tasks with score > $\tau$",
                 ax=axes_performance_profile[1],
             )
             h, l = axes_performance_profile[0].get_legend_handles_labels()
-            fig_performance_profile.legend(h, l, loc="lower center", ncol=args.pc.ncols_legend, bbox_to_anchor=(0.5, 1.0), bbox_transform=fig_performance_profile.transFigure)
+            fig_performance_profile.legend(
+                h,
+                l,
+                loc="lower center",
+                ncol=args.pc.ncols_legend,
+                bbox_to_anchor=(0.5, 1.0),
+                bbox_transform=fig_performance_profile.transFigure,
+            )
             fig_performance_profile.tight_layout()
             fig_performance_profile.savefig(f"{args.output_filename}_performance_profile.png", bbox_inches="tight")
             fig_performance_profile.savefig(f"{args.output_filename}_performance_profile.pdf", bbox_inches="tight")
 
         if args.rc.aggregate_metrics_plots:
             print("plotting aggregate metrics")
             aggregate_func = lambda x: np.array([metric_fn(x) for metric_fn in metric_fns])
             aggregate_scores, aggregate_score_cis = rly.get_interval_estimates(
                 performance_profile_normalized_score_dict, aggregate_func, reps=args.rc.interval_estimates_num_bootstrap_reps
             )
-            aggregate_scores_df = pd.DataFrame.from_dict(aggregate_scores, orient="index", columns=["Median", "IQM", "Mean", "Optimality Gap"])
+            aggregate_scores_df = pd.DataFrame.from_dict(
+                aggregate_scores, orient="index", columns=["Median", "IQM", "Mean", "Optimality Gap"]
+            )
             print_rich_table(f"Aggregate Scores", aggregate_scores_df.reset_index(), console)
             fig, axes = plot_utils.plot_interval_estimates(
                 aggregate_scores,
                 aggregate_score_cis,
                 metric_names=["Median", "IQM", "Mean", "Optimality Gap"],
                 algorithms=exp_names,
                 colors=colors,
-                xlabel='',
+                xlabel="",
                 # xlabel='Normalized Score',
                 # xlabel_y_coordinate=-0.08, # this variable needs to be adjusted for each plot... :( so we just disable xlabel for now.
             )
             axes[1].set_xlabel("Normalized Score", fontsize="xx-large")
             fig.tight_layout()
             plt.savefig(f"{args.output_filename}_aggregate.png", bbox_inches="tight")
             plt.savefig(f"{args.output_filename}_aggregate.pdf", bbox_inches="tight")
```

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/rlops.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/openrlbenchmark/rlops_hns.py` & `openrlbenchmark-0.2.1a1/openrlbenchmark/rlops_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b4/pyproject.toml` & `openrlbenchmark-0.2.1a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrlbenchmark"
-version = "0.2.0b4"
+version = "0.2.1a1"
 description = ""
 authors = ["Costa Huang <costa.huang@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "openrlbenchmark" },
 ]
```

### Comparing `openrlbenchmark-0.2.0b4/PKG-INFO` & `openrlbenchmark-0.2.1a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: openrlbenchmark
-Version: 0.2.0b4
-Summary: 
-Author: Costa Huang
-Author-email: costa.huang@outlook.com
-Requires-Python: >=3.7.1,<3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: dotmap (>=1.3.30,<2.0.0)
-Requires-Dist: expt (>=0.4.1,<0.5.0)
-Requires-Dist: importlib-metadata (>=5.1.0,<6.0.0)
-Requires-Dist: multiprocess (>=0.70.13,<0.71.0)
-Requires-Dist: peewee (>=3.16.2,<4.0.0)
-Requires-Dist: pip (>=22.1.2,<23.0.0)
-Requires-Dist: rich (<12.0)
-Requires-Dist: rliable (>=1.0.8,<2.0.0)
-Requires-Dist: seaborn (>=0.12.1,<0.13.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: tueplots (>=0.0.4,<0.0.5)
-Requires-Dist: tyro (>=0.5.0,<0.6.0)
-Requires-Dist: wandb (>=0.13.7,<0.14.0)
-Description-Content-Type: text/markdown
-
 # Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning
 
 
 [<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)
@@ -87,52 +60,63 @@
     --rc.sample_efficiency_plots \
     --rc.sample_efficiency_and_walltime_efficiency_method Median \
     --rc.performance_profile_plots  \
     --rc.aggregate_metrics_plots  \
     --rc.sample_efficiency_num_bootstrap_reps 10 \
     --rc.performance_profile_num_bootstrap_reps 10 \
     --rc.interval_estimates_num_bootstrap_reps 10 \
-    --output-filename static/0compare \
+    --output-filename compare \
     --scan-history
 ```
 
-Here, we created multiple filters. The first string in the first filter is `'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean'`, which is a query string that specifies the following:
+Here, we created multiple filters. The first string in the first filter is `'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return'`, which is a query string that specifies the following:
 
 * `we`: the W&B entity name
 * `wpn`: the W&B project name
 * `ceik`: the custom key for the environment id
 * `cen`: the custom key for the experiment name
 * `metric`: the metric we are interested in
 
-So we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.
+So we are fetching metrics from [https://wandb.ai/openrlbenchmark/baselines](https://wandb.ai/openrlbenchmark/baselines). The environment id is stored in the `env` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`.
 
-Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.
+Similarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `baselines-ppo2-mlp?cl=openai/baselines PPO2`.
 
 The labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure
 
-The command above generates the following plot:
+The `--rliable` toggles our [rliable](https://github.com/google-research/rliable) integration, and its configuration can be tweeked via `--rc`. The command above generates the following plot:
 
-|    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |
-|:----------------------------------:|:----------------------------------------:|
-|  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |
+![](static/baseline_vs_cleanrl.png)
+![](static/baseline_vs_cleanrl-time.png)
+![](static/baseline_vs_cleanrl_sample_walltime_efficiency.png)
+![](static/baseline_vs_cleanrl_sample_efficiency.png)
+![](static/baseline_vs_cleanrl_performance_profile.png)
+![](static/baseline_vs_cleanrl_aggregate.png)
 
 
 
-The `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-sac_continuous_action--VmlldzozMTY4NDQ3)
+The `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-openai-baselines-PPO2--Vmlldzo0NTU4MTE5)
 
 
 The command also generates a `compare.png`, a `compare.md`, and a `compare.csv` in the current directory.
 
 **Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.
 
 **Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.
 
 
 > **Warning**
-> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. If you are using `openrlbenchmark` repeatedly or you wanto to generate consistent `compare.md` and learning curves, we recommend you to use `--scan-history` to get all of the data points, but initially it may take a while to run.
+> We recommend you to use `--scan-history` which pullts all of the data points, but initially it will cache the data and may take a while to run. If you don't use `--scan-history`, it will only pull 500 data points from wandb randomly, which could generate different learning curves each time you run the command.
+
+
+## Offline mode
+
+We introduced an experimental **offline** mode. Sometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. 
+
+No worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs. Then, you can run `python -m openrlbenchmark.rlops ... --scan-history --offline` to generate the plots without having access to the internet. It should considerably speed up the plotting process as well. We are still working on improving the offline mode, so please let us know if you encounter any issues. 
+
 
 
 ## Currently supported libraries
 
 * [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)
     * `ceik`: `env_id`
     * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)
@@ -176,62 +160,53 @@
 
 ## More examples
 
 ### Compare CleanRL's PPO with `openai/baselines`'s PPO2 on Atari games:
 
 Sometimes the same environments could have different names in different libraries. For example, `openai/baselines` uses `BreakoutNoFrameskip-v4` while [EnvPool](https://envpool.readthedocs.io/en/latest/env/atari.html) uses `Breakout-v5`. To compare the two libraries, we need to specify the `env_id` for `CleanRL` and `env` for `openai/baselines`. In this case, can specify the corresponding `env_ids` for each filter.
 
-For Atari games, we have additional batteries included `openrlbenchmark.rlops_hns` to show human normalized-scores and further statistical analysis through [`rliable`](https://github.com/google-research/rliable).
+For Atari games, we can toggle `--rc.score_normalization_method atari` option to use human-normalized scores for `rliable` analysis.
 
 
 ```shell
-python -m openrlbenchmark.rlops_hns \
+python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-cnn' \
     --filters '?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return' 'ppo_atari_envpool_xla_jax_truncation' \
     --env-ids AlienNoFrameskip-v4 AmidarNoFrameskip-v4 AssaultNoFrameskip-v4 AsterixNoFrameskip-v4 AsteroidsNoFrameskip-v4 AtlantisNoFrameskip-v4 BankHeistNoFrameskip-v4 BattleZoneNoFrameskip-v4 BeamRiderNoFrameskip-v4 BerzerkNoFrameskip-v4 BowlingNoFrameskip-v4 BoxingNoFrameskip-v4 BreakoutNoFrameskip-v4 CentipedeNoFrameskip-v4 ChopperCommandNoFrameskip-v4 CrazyClimberNoFrameskip-v4 DefenderNoFrameskip-v4 DemonAttackNoFrameskip-v4 DoubleDunkNoFrameskip-v4 EnduroNoFrameskip-v4 FishingDerbyNoFrameskip-v4 FreewayNoFrameskip-v4 FrostbiteNoFrameskip-v4 GopherNoFrameskip-v4 GravitarNoFrameskip-v4 HeroNoFrameskip-v4 IceHockeyNoFrameskip-v4 PrivateEyeNoFrameskip-v4 QbertNoFrameskip-v4 RiverraidNoFrameskip-v4 RoadRunnerNoFrameskip-v4 RobotankNoFrameskip-v4 SeaquestNoFrameskip-v4 SkiingNoFrameskip-v4 SolarisNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 StarGunnerNoFrameskip-v4 SurroundNoFrameskip-v4 TennisNoFrameskip-v4 TimePilotNoFrameskip-v4 TutankhamNoFrameskip-v4 UpNDownNoFrameskip-v4 VentureNoFrameskip-v4 VideoPinballNoFrameskip-v4 WizardOfWorNoFrameskip-v4 YarsRevengeNoFrameskip-v4 ZaxxonNoFrameskip-v4 JamesbondNoFrameskip-v4 KangarooNoFrameskip-v4 KrullNoFrameskip-v4 KungFuMasterNoFrameskip-v4 MontezumaRevengeNoFrameskip-v4 MsPacmanNoFrameskip-v4 NameThisGameNoFrameskip-v4 PhoenixNoFrameskip-v4 PitfallNoFrameskip-v4 PongNoFrameskip-v4 \
     --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \
     --no-check-empty-runs \
     --pc.ncols 5 \
     --pc.ncols-legend 2 \
-    --output-filename static/cleanrl_vs_baselines \
-    --scan-history --rliable
+    --rliable \
+    --rc.score_normalization_method atari \
+    --rc.normalized_score_threshold 8.0 \
+    --rc.sample_efficiency_plots \
+    --rc.sample_efficiency_and_walltime_efficiency_method Median \
+    --rc.performance_profile_plots  \
+    --rc.aggregate_metrics_plots  \
+    --rc.sample_efficiency_num_bootstrap_reps 50000 \
+    --rc.performance_profile_num_bootstrap_reps 2000 \
+    --rc.interval_estimates_num_bootstrap_reps 2000 \
+    --output-filename static/cleanrl_vs_baselines_atari \
+    --scan-history
 ```
 
-In the individual learning curves below, the right y-axis is the human normalized score. The left y-axis is the raw episodic return.
-![](static/cleanrl_vs_baselines.png) The script also generates `cleanrl_vs_baselines_hns_median.png`, the learning curves for median human-normalized scores. 
 
 Furthermore, the `--rliable` integration generates `cleanrl_vs_baselines_iqm_profile.png`, the  Interquartile Mean (IQM) and performance profile ([Agarwal et al., 2022](https://arxiv.org/pdf/2108.13264.pdf)), and `cleanrl_vs_baselines_hns_aggregate.png`, the aggregate human-normalized scores with Stratified Bootstrap Confidence Intervals (see @araffin's excellent blog post [explainer](https://araffin.github.io/post/rliable/)). 
 
 
-![](static/cleanrl_vs_baselines_hns_median.png)
-
-![](static/cleanrl_vs_baselines_iqm_profile.png)
-
-![](static/cleanrl_vs_baselines_hns_aggregate.png)
 
+![](static/cleanrl_vs_baselines_atari.png)
+![](static/cleanrl_vs_baselines_atari-time.png)
+![](static/cleanrl_vs_baselines_atari_sample_walltime_efficiency.png)
+![](static/cleanrl_vs_baselines_atari_sample_efficiency.png)
+![](static/cleanrl_vs_baselines_atari_performance_profile.png)
+![](static/cleanrl_vs_baselines_atari_aggregate.png)
 
-### Offline mode
 
-Sometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. 
-
-No worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs, enabling us to run the script without internet connection.
-
-```shell
-python -m openrlbenchmark.rlops \
-    --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
-    --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
-    --filters '?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return' 'sac' \
-    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \
-    --no-check-empty-runs \
-    --pc.ncols 3 \
-    --pc.ncols-legend 3 \
-    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \
-    --scan-history \
-    --offline
-```
 
 ### Compare CleanRL's PPO with `openai/baselines`'s PPO2 and `jaxrl`'s SAC on Mujoco:
 
 ```shell
 python -m openrlbenchmark.rlops \
     --filters '?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return' 'baselines-ppo2-mlp' \
     --filters '?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return' 'ppo_continuous_action?tag=v1.0.0-27-gde3f410' \
@@ -345,8 +320,21 @@
 This is a project we are slowly working on. There is no specific timeline or roadmap, but if you want to get involved. Feel free to reach out to me or open an issue. We are looking for volunteers to help us with the following:
 
 * Add experiments from other libraries
 * Run more experiments from currently supported libraries
 * Documentation and designing standards
 * Download the tensorboard metrics from the tracked experiments and load them locally to save time
 
+## Citation
+
+If you have used this software in your work, please use the following citation.
 
+```bibtex
+@software{
+    Huang_openrlbenchmark_2023,
+    author = {Huang, Shengyi and Gallouédec, Quentin and Felten, Florian and Raffin, Antonin and Dossa, Rousslan Fernand Julien and Zhao, Yanxiao and Sullivan, Ryan and Makoviychuk, Viktor and Makoviichuk, Denys and Roumégous, Cyril and Weng, Jiayi and Chen, Chufan and Rahman, Masudur and M. Araújo, João G. and Quan, Guorui and Tan, Daniel and Klein, Timo and Charakorn, Rujikorn and Towers, Mark and Berthelot, Yann and Mehta, Kinal and Chakraborty, Dipam and KG, Arjun and Charraut, Valentin and Ye, Chang and Liu, Zichen and Alegre, Lucas N. and Choi, Jongwook and Yi, Brent},
+    month = may,
+    title = {{openrlbenchmark}},
+    url = {https://github.com/openrlbenchmark/openrlbenchmark},
+    year = {2023}
+}
+```
```

